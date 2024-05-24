# Comparing `tmp/langchain_anthropic-0.1.8rc1.tar.gz` & `tmp/langchain_anthropic-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_anthropic-0.1.8rc1.tar", max compression
+gzip compressed data, was "langchain_anthropic-0.1.9.tar", max compression
```

## Comparing `langchain_anthropic-0.1.8rc1.tar` & `langchain_anthropic-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/LICENSE
--rw-r--r--   0        0        0     1215 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/README.md
--rw-r--r--   0        0        0      225 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/__init__.py
--rw-r--r--   0        0        0    26903 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/chat_models.py
--rw-r--r--   0        0        0     4908 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/experimental.py
--rw-r--r--   0        0        0    11687 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/llms.py
--rw-r--r--   0        0        0     2493 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/output_parsers.py
--rw-r--r--   0        0        0        0 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/langchain_anthropic/py.typed
--rw-r--r--   0        0        0     2723 2024-04-10 00:56:53.994481 langchain_anthropic-0.1.8rc1/pyproject.toml
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 langchain_anthropic-0.1.8rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-16 23:06:35.216096 langchain_anthropic-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1215 2024-04-16 23:06:35.216096 langchain_anthropic-0.1.9/README.md
+-rw-r--r--   0        0        0      225 2024-04-16 23:06:35.216096 langchain_anthropic-0.1.9/langchain_anthropic/__init__.py
+-rw-r--r--   0        0        0    28894 2024-04-16 23:06:35.216096 langchain_anthropic-0.1.9/langchain_anthropic/chat_models.py
+-rw-r--r--   0        0        0     4908 2024-04-16 23:06:35.216096 langchain_anthropic-0.1.9/langchain_anthropic/experimental.py
+-rw-r--r--   0        0        0    12423 2024-04-16 23:06:35.216096 langchain_anthropic-0.1.9/langchain_anthropic/llms.py
+-rw-r--r--   0        0        0     2493 2024-04-16 23:06:35.216096 langchain_anthropic-0.1.9/langchain_anthropic/output_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-16 23:06:35.216096 langchain_anthropic-0.1.9/langchain_anthropic/py.typed
+-rw-r--r--   0        0        0     2752 2024-04-16 23:06:35.220096 langchain_anthropic-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 langchain_anthropic-0.1.9/PKG-INFO
```

### Comparing `langchain_anthropic-0.1.8rc1/LICENSE` & `langchain_anthropic-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.8rc1/README.md` & `langchain_anthropic-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.8rc1/langchain_anthropic/chat_models.py` & `langchain_anthropic-0.1.9/langchain_anthropic/chat_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     Dict,
     Iterator,
     List,
+    Literal,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypedDict,
     Union,
@@ -34,14 +35,15 @@
 )
 from langchain_core.messages import (
     AIMessage,
     AIMessageChunk,
     BaseMessage,
     HumanMessage,
     SystemMessage,
+    ToolCall,
     ToolMessage,
 )
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
 from langchain_core.pydantic_v1 import BaseModel, Field, SecretStr, root_validator
 from langchain_core.runnables import (
     Runnable,
     RunnableMap,
@@ -152,15 +154,15 @@
                     "System message must be a string, "
                     f"instead was: {type(message.content)}"
                 )
             system = message.content
             continue
 
         role = _message_type_lookups[message.type]
-        content: Union[str, List[Dict]]
+        content: Union[str, List]
 
         if not isinstance(message.content, str):
             # parse as dict
             assert isinstance(
                 message.content, list
             ), "Anthropic message content must be str or list of dicts"
 
@@ -191,14 +193,28 @@
                         content.append(item)
                     else:
                         content.append(item)
                 else:
                     raise ValueError(
                         f"Content items must be str or dict, instead was: {type(item)}"
                     )
+        elif (
+            isinstance(message, AIMessage)
+            and not isinstance(message.content, list)
+            and message.tool_calls
+        ):
+            content = (
+                []
+                if not message.content
+                else [{"type": "text", "text": message.content}]
+            )
+            # Note: Anthropic can't have invalid tool calls as presently defined,
+            # since the model already returns dicts args not JSON strings, and invalid
+            # tool calls are those with invalid JSON for args.
+            content += _lc_tool_calls_to_anthropic_tool_use_blocks(message.tool_calls)
         else:
             content = message.content
 
         formatted_messages.append(
             {
                 "role": role,
                 "content": content,
@@ -247,15 +263,15 @@
     default_request_timeout: Optional[float] = Field(None, alias="timeout")
     """Timeout for requests to Anthropic Completion API."""
 
     # sdk default = 2: https://github.com/anthropics/anthropic-sdk-python?tab=readme-ov-file#retries
     max_retries: int = 2
     """Number of retries allowed for requests sent to the Anthropic Completion API."""
 
-    anthropic_api_url: str = "https://api.anthropic.com"
+    anthropic_api_url: Optional[str] = None
 
     anthropic_api_key: Optional[SecretStr] = Field(None, alias="api_key")
     """Automatically read from env var `ANTHROPIC_API_KEY` if not provided."""
 
     default_headers: Optional[Mapping[str, str]] = None
     """Headers to pass to the Anthropic clients, will be used for every API call."""
 
@@ -265,14 +281,42 @@
     """Whether to use streaming or not."""
 
     @property
     def _llm_type(self) -> str:
         """Return type of chat model."""
         return "anthropic-chat"
 
+    @property
+    def lc_secrets(self) -> Dict[str, str]:
+        return {"anthropic_api_key": "ANTHROPIC_API_KEY"}
+
+    @classmethod
+    def is_lc_serializable(cls) -> bool:
+        return True
+
+    @classmethod
+    def get_lc_namespace(cls) -> List[str]:
+        """Get the namespace of the langchain object."""
+        return ["langchain", "chat_models", "anthropic"]
+
+    @property
+    def _identifying_params(self) -> Dict[str, Any]:
+        """Get the identifying parameters."""
+        return {
+            "model": self.model,
+            "max_tokens": self.max_tokens,
+            "temperature": self.temperature,
+            "top_k": self.top_k,
+            "top_p": self.top_p,
+            "model_kwargs": self.model_kwargs,
+            "streaming": self.streaming,
+            "max_retries": self.max_retries,
+            "default_request_timeout": self.default_request_timeout,
+        }
+
     @root_validator(pre=True)
     def build_extra(cls, values: Dict) -> Dict:
         extra = values.get("model_kwargs", {})
         all_required_field_names = get_pydantic_field_names(cls)
         values["model_kwargs"] = build_extra_kwargs(
             extra, values, all_required_field_names
         )
@@ -340,15 +384,14 @@
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> Iterator[ChatGenerationChunk]:
         params = self._format_params(messages=messages, stop=stop, **kwargs)
         if _tools_in_params(params):
-            warnings.warn("stream: Tool use is not yet supported in streaming mode.")
             result = self._generate(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             )
             message = result.generations[0].message
             if isinstance(message, AIMessage) and message.tool_calls is not None:
                 tool_call_chunks = [
                     {
@@ -674,10 +717,33 @@
 
 def _tools_in_params(params: dict) -> bool:
     return "tools" in params or (
         "extra_body" in params and params["extra_body"].get("tools")
     )
 
 
+class _AnthropicToolUse(TypedDict):
+    type: Literal["tool_use"]
+    name: str
+    input: dict
+    id: str
+
+
+def _lc_tool_calls_to_anthropic_tool_use_blocks(
+    tool_calls: List[ToolCall],
+) -> List[_AnthropicToolUse]:
+    blocks = []
+    for tool_call in tool_calls:
+        blocks.append(
+            _AnthropicToolUse(
+                type="tool_use",
+                name=tool_call["name"],
+                input=tool_call["args"],
+                id=cast(str, tool_call["id"]),
+            )
+        )
+    return blocks
+
+
 @deprecated(since="0.1.0", removal="0.2.0", alternative="ChatAnthropic")
 class ChatAnthropicMessages(ChatAnthropic):
     pass
```

### Comparing `langchain_anthropic-0.1.8rc1/langchain_anthropic/experimental.py` & `langchain_anthropic-0.1.9/langchain_anthropic/experimental.py`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.8rc1/langchain_anthropic/llms.py` & `langchain_anthropic-0.1.9/langchain_anthropic/llms.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,14 +169,37 @@
         return values
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "anthropic-llm"
 
+    @property
+    def lc_secrets(self) -> Dict[str, str]:
+        return {"anthropic_api_key": "ANTHROPIC_API_KEY"}
+
+    @classmethod
+    def is_lc_serializable(cls) -> bool:
+        return True
+
+    @property
+    def _identifying_params(self) -> Dict[str, Any]:
+        """Get the identifying parameters."""
+        return {
+            "model": self.model,
+            "max_tokens": self.max_tokens_to_sample,
+            "temperature": self.temperature,
+            "top_k": self.top_k,
+            "top_p": self.top_p,
+            "model_kwargs": self.model_kwargs,
+            "streaming": self.streaming,
+            "default_request_timeout": self.default_request_timeout,
+            "max_retries": self.max_retries,
+        }
+
     def _wrap_prompt(self, prompt: str) -> str:
         if not self.HUMAN_PROMPT or not self.AI_PROMPT:
             raise NameError("Please ensure the anthropic package is loaded")
 
         if prompt.startswith(self.HUMAN_PROMPT):
             return prompt  # Already wrapped.
```

### Comparing `langchain_anthropic-0.1.8rc1/langchain_anthropic/output_parsers.py` & `langchain_anthropic-0.1.9/langchain_anthropic/output_parsers.py`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.8rc1/pyproject.toml` & `langchain_anthropic-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-anthropic"
-version = "0.1.8rc1"
+version = "0.1.9"
 description = "An integration package connecting AnthropicMessages and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/anthropic"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = { version = "^0.1.42rc1", allow-prereleases = true }
+langchain-core = "^0.1.43"
 anthropic = ">=0.23.0,<1"
 defusedxml = { version = "^0.7.1", optional = true }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
@@ -24,14 +24,15 @@
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain-core = { path = "../../core", develop = true }
 defusedxml = "^0.7.1"
+langchain-standard-tests = {path = "../../standard-tests", develop = true}
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
```

### Comparing `langchain_anthropic-0.1.8rc1/PKG-INFO` & `langchain_anthropic-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-anthropic
-Version: 0.1.8rc1
+Version: 0.1.9
 Summary: An integration package connecting AnthropicMessages and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (>=0.23.0,<1)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: langchain-core (>=0.1.42rc1,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.43,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/anthropic
 Description-Content-Type: text/markdown
 
 # langchain-anthropic
 
 This package contains the LangChain integration for Anthropic's generative models.
```

