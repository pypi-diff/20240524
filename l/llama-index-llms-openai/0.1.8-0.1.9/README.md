# Comparing `tmp/llama_index_llms_openai-0.1.8.tar.gz` & `tmp/llama_index_llms_openai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_openai-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_llms_openai-0.1.9.tar", max compression
```

## Comparing `llama_index_llms_openai-0.1.8.tar` & `llama_index_llms_openai-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       38 2024-03-12 18:29:16.121123 llama_index_llms_openai-0.1.8/README.md
--rw-r--r--   0        0        0      148 2024-03-12 18:29:16.121123 llama_index_llms_openai-0.1.8/llama_index/llms/openai/__init__.py
--rw-r--r--   0        0        0    23922 2024-03-12 18:29:16.121123 llama_index_llms_openai-0.1.8/llama_index/llms/openai/base.py
--rw-r--r--   0        0        0    10815 2024-03-12 18:29:16.121123 llama_index_llms_openai-0.1.8/llama_index/llms/openai/utils.py
--rw-r--r--   0        0        0     1460 2024-03-12 18:29:16.121123 llama_index_llms_openai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 llama_index_llms_openai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       38 2024-03-13 04:31:55.461921 llama_index_llms_openai-0.1.9/README.md
+-rw-r--r--   0        0        0      148 2024-03-13 04:31:55.461921 llama_index_llms_openai-0.1.9/llama_index/llms/openai/__init__.py
+-rw-r--r--   0        0        0    25105 2024-03-13 04:31:55.461921 llama_index_llms_openai-0.1.9/llama_index/llms/openai/base.py
+-rw-r--r--   0        0        0    12610 2024-03-13 04:31:55.461921 llama_index_llms_openai-0.1.9/llama_index/llms/openai/utils.py
+-rw-r--r--   0        0        0     1461 2024-03-13 04:31:55.461921 llama_index_llms_openai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 llama_index_llms_openai-0.1.9/PKG-INFO
```

### Comparing `llama_index_llms_openai-0.1.8/llama_index/llms/openai/base.py` & `llama_index_llms_openai-0.1.9/llama_index/llms/openai/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     stream_completion_to_chat_decorator,
 )
 from llama_index.core.llms.llm import LLM
 from llama_index.core.types import BaseOutputParser, PydanticProgramMode
 from llama_index.llms.openai.utils import (
     create_retry_decorator,
     from_openai_message,
+    from_openai_token_logprobs,
+    from_openai_completion_logprobs,
     is_chat_model,
     is_function_calling_model,
     openai_modelname_to_contextsize,
     resolve_openai_credentials,
     to_openai_message_dicts,
 )
 
@@ -92,14 +94,23 @@
         gte=0.0,
         lte=1.0,
     )
     max_tokens: Optional[int] = Field(
         description="The maximum number of tokens to generate.",
         gt=0,
     )
+    logprobs: Optional[bool] = Field(
+        description="Whether to return logprobs per token."
+    )
+    top_logprobs: int = Field(
+        description="The number of top token log probs to return.",
+        default=0,
+        gte=0,
+        lte=20,
+    )
     additional_kwargs: Dict[str, Any] = Field(
         default_factory=dict, description="Additional kwargs for the OpenAI API."
     )
     max_retries: int = Field(
         default=3,
         description="The maximum number of API retries.",
         gte=0,
@@ -293,31 +304,42 @@
     def _get_model_kwargs(self, **kwargs: Any) -> Dict[str, Any]:
         base_kwargs = {"model": self.model, "temperature": self.temperature, **kwargs}
         if self.max_tokens is not None:
             # If max_tokens is None, don't include in the payload:
             # https://platform.openai.com/docs/api-reference/chat
             # https://platform.openai.com/docs/api-reference/completions
             base_kwargs["max_tokens"] = self.max_tokens
+        if self.logprobs is not None and self.logprobs is True:
+            if self.metadata.is_chat_model:
+                base_kwargs["logprobs"] = self.logprobs
+                base_kwargs["top_logprobs"] = self.top_logprobs
+            else:
+                base_kwargs["logprobs"] = self.top_logprobs  # int in this case
         return {**base_kwargs, **self.additional_kwargs}
 
     @llm_retry_decorator
     def _chat(self, messages: Sequence[ChatMessage], **kwargs: Any) -> ChatResponse:
         client = self._get_client()
         message_dicts = to_openai_message_dicts(messages)
         response = client.chat.completions.create(
             messages=message_dicts,
             stream=False,
             **self._get_model_kwargs(**kwargs),
         )
         openai_message = response.choices[0].message
         message = from_openai_message(openai_message)
+        openai_token_logprobs = response.choices[0].logprobs
+        logprobs = None
+        if openai_token_logprobs:
+            logprobs = from_openai_token_logprobs(openai_token_logprobs.content)
 
         return ChatResponse(
             message=message,
             raw=response,
+            logprobs=logprobs,
             additional_kwargs=self._get_response_token_counts(response),
         )
 
     def _update_tool_calls(
         self,
         tool_calls: List[ChoiceDeltaToolCall],
         tool_calls_delta: Optional[List[ChoiceDeltaToolCall]],
@@ -424,17 +446,24 @@
 
         response = client.completions.create(
             prompt=prompt,
             stream=False,
             **all_kwargs,
         )
         text = response.choices[0].text
+
+        openai_completion_logprobs = response.choices[0].logprobs
+        logprobs = None
+        if openai_completion_logprobs:
+            logprobs = from_openai_completion_logprobs(openai_completion_logprobs)
+
         return CompletionResponse(
             text=text,
             raw=response,
+            logprobs=logprobs,
             additional_kwargs=self._get_response_token_counts(response),
         )
 
     @llm_retry_decorator
     def _stream_complete(self, prompt: str, **kwargs: Any) -> CompletionResponseGen:
         client = self._get_client()
         all_kwargs = self._get_model_kwargs(**kwargs)
@@ -550,14 +579,15 @@
         aclient = self._get_aclient()
         message_dicts = to_openai_message_dicts(messages)
         response = await aclient.chat.completions.create(
             messages=message_dicts, stream=False, **self._get_model_kwargs(**kwargs)
         )
         message_dict = response.choices[0].message
         message = from_openai_message(message_dict)
+        logprobs_dict = response.choices[0].logprobs
 
         return ChatResponse(
             message=message,
             raw=response,
             additional_kwargs=self._get_response_token_counts(response),
         )
```

### Comparing `llama_index_llms_openai-0.1.8/llama_index/llms/openai/utils.py` & `llama_index_llms_openai-0.1.9/llama_index/llms/openai/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Type, Union
 
 from deprecated import deprecated
-from llama_index.core.base.llms.types import ChatMessage
+from llama_index.core.base.llms.types import ChatMessage, LogProb, CompletionResponse
 from llama_index.core.bridge.pydantic import BaseModel
 from llama_index.core.base.llms.generic_utils import get_from_param_or_env
 from tenacity import (
     before_sleep_log,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
@@ -17,14 +17,17 @@
 )
 from tenacity.stop import stop_base
 
 import openai
 from openai.types.chat import ChatCompletionMessageParam, ChatCompletionMessageToolCall
 from openai.types.chat.chat_completion_chunk import ChoiceDeltaToolCall
 from openai.types.chat.chat_completion_message import ChatCompletionMessage
+from openai.types.chat.chat_completion_token_logprob import ChatCompletionTokenLogprob
+from openai.types.completion_choice import Logprobs
+from openai.types.completion import Completion
 
 DEFAULT_OPENAI_API_TYPE = "open_ai"
 DEFAULT_OPENAI_API_BASE = "https://api.openai.com/v1"
 DEFAULT_OPENAI_API_VERSION = ""
 
 
 GPT4_MODELS: Dict[str, int] = {
@@ -256,14 +259,64 @@
     if openai_message.tool_calls is not None:
         tool_calls: List[ChatCompletionMessageToolCall] = openai_message.tool_calls
         additional_kwargs.update(tool_calls=tool_calls)
 
     return ChatMessage(role=role, content=content, additional_kwargs=additional_kwargs)
 
 
+def from_openai_token_logprob(
+    openai_token_logprob: ChatCompletionTokenLogprob,
+) -> List[LogProb]:
+    """Convert a single openai token logprob to generic list of logprobs."""
+    try:
+        result = [
+            LogProb(token=el.token, logprob=el.logprob, bytes=el.bytes or [])
+            for el in openai_token_logprob.top_logprobs
+        ]
+    except Exception as e:
+        print(openai_token_logprob)
+        raise
+    return result
+
+
+def from_openai_token_logprobs(
+    openai_token_logprobs: Sequence[ChatCompletionTokenLogprob],
+) -> List[List[LogProb]]:
+    """Convert openai token logprobs to generic list of LogProb."""
+    return [
+        from_openai_token_logprob(token_logprob)
+        for token_logprob in openai_token_logprobs
+    ]
+
+
+def from_openai_completion_logprob(
+    openai_completion_logprob: Dict[str, float]
+) -> List[LogProb]:
+    """Convert openai completion logprobs to generic list of LogProb."""
+    return [
+        LogProb(token=t, logprob=v, bytes=[])
+        for t, v in openai_completion_logprob.items()
+    ]
+
+
+def from_openai_completion_logprobs(
+    openai_completion_logprobs: Logprobs,
+) -> List[List[LogProb]]:
+    """Convert openai completion logprobs to generic list of LogProb."""
+    return [
+        from_openai_completion_logprob(completion_logprob)
+        for completion_logprob in openai_completion_logprobs.top_logprobs
+    ]
+
+
+def from_openai_completion(openai_completion: Completion) -> CompletionResponse:
+    """Convert openai completion to CompletionResponse."""
+    text = openai_completion.choices[0].text
+
+
 def from_openai_messages(
     openai_messages: Sequence[ChatCompletionMessage],
 ) -> List[ChatMessage]:
     """Convert openai message dicts to generic messages."""
     return [from_openai_message(message) for message in openai_messages]
```

### Comparing `llama_index_llms_openai-0.1.8/pyproject.toml` & `llama_index_llms_openai-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 [tool.poetry]
 authors = ["llama-index"]
 description = "llama-index llms openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-openai"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.19"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_llms_openai-0.1.8/PKG-INFO` & `llama_index_llms_openai-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-openai
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index llms openai integration
 License: MIT
 Author: llama-index
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.19,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Openai
```

