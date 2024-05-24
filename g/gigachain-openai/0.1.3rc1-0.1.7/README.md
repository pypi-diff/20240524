# Comparing `tmp/gigachain_openai-0.1.3rc1.tar.gz` & `tmp/gigachain_openai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain_openai-0.1.3rc1.tar", max compression
+gzip compressed data, was "gigachain_openai-0.1.7.tar", max compression
```

## Comparing `gigachain_openai-0.1.3rc1.tar` & `gigachain_openai-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-01-18 15:16:41.009869 gigachain_openai-0.1.3rc1/LICENSE
--rw-r--r--   0        0        0     1627 2024-01-18 15:16:41.010661 gigachain_openai-0.1.3rc1/README.md
--rw-r--r--   0        0        0      371 2024-01-18 15:16:41.011302 gigachain_openai-0.1.3rc1/langchain_openai/__init__.py
--rw-r--r--   0        0        0      176 2024-01-18 15:16:41.012203 gigachain_openai-0.1.3rc1/langchain_openai/chat_models/__init__.py
--rw-r--r--   0        0        0    10508 2024-03-28 12:44:20.752636 gigachain_openai-0.1.3rc1/langchain_openai/chat_models/azure.py
--rw-r--r--   0        0        0    44617 2024-04-11 07:23:40.046099 gigachain_openai-0.1.3rc1/langchain_openai/chat_models/base.py
--rw-r--r--   0        0        0      198 2024-01-18 15:16:41.014232 gigachain_openai-0.1.3rc1/langchain_openai/embeddings/__init__.py
--rw-r--r--   0        0        0     6567 2024-04-10 15:22:17.494741 gigachain_openai-0.1.3rc1/langchain_openai/embeddings/azure.py
--rw-r--r--   0        0        0    23294 2024-03-28 12:44:20.755225 gigachain_openai-0.1.3rc1/langchain_openai/embeddings/base.py
--rw-r--r--   0        0        0      146 2024-01-18 15:16:41.016012 gigachain_openai-0.1.3rc1/langchain_openai/llms/__init__.py
--rw-r--r--   0        0        0     8008 2024-03-28 12:44:20.756153 gigachain_openai-0.1.3rc1/langchain_openai/llms/azure.py
--rw-r--r--   0        0        0    24477 2024-04-10 15:22:17.495379 gigachain_openai-0.1.3rc1/langchain_openai/llms/base.py
--rw-r--r--   0        0        0      229 2024-03-28 12:44:20.757798 gigachain_openai-0.1.3rc1/langchain_openai/output_parsers/__init__.py
--rw-r--r--   0        0        0      229 2024-03-28 12:44:20.758114 gigachain_openai-0.1.3rc1/langchain_openai/output_parsers/tools.py
--rw-r--r--   0        0        0        0 2024-01-18 15:16:41.017389 gigachain_openai-0.1.3rc1/langchain_openai/py.typed
--rw-r--r--   0        0        0     2915 2024-04-11 09:52:44.491735 gigachain_openai-0.1.3rc1/pyproject.toml
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 gigachain_openai-0.1.3rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-01-18 15:16:41.009869 gigachain_openai-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1627 2024-04-19 07:38:34.397800 gigachain_openai-0.1.7/README.md
+-rw-r--r--   0        0        0      371 2024-01-18 15:16:41.011302 gigachain_openai-0.1.7/langchain_openai/__init__.py
+-rw-r--r--   0        0        0      176 2024-01-18 15:16:41.012203 gigachain_openai-0.1.7/langchain_openai/chat_models/__init__.py
+-rw-r--r--   0        0        0    11248 2024-05-24 11:13:19.640304 gigachain_openai-0.1.7/langchain_openai/chat_models/azure.py
+-rw-r--r--   0        0        0    48036 2024-05-24 11:13:19.641268 gigachain_openai-0.1.7/langchain_openai/chat_models/base.py
+-rw-r--r--   0        0        0      198 2024-01-18 15:16:41.014232 gigachain_openai-0.1.7/langchain_openai/embeddings/__init__.py
+-rw-r--r--   0        0        0     6567 2024-04-19 07:38:34.400710 gigachain_openai-0.1.7/langchain_openai/embeddings/azure.py
+-rw-r--r--   0        0        0    24289 2024-05-24 11:13:19.642839 gigachain_openai-0.1.7/langchain_openai/embeddings/base.py
+-rw-r--r--   0        0        0      146 2024-01-18 15:16:41.016012 gigachain_openai-0.1.7/langchain_openai/llms/__init__.py
+-rw-r--r--   0        0        0     8354 2024-05-06 14:45:39.112754 gigachain_openai-0.1.7/langchain_openai/llms/azure.py
+-rw-r--r--   0        0        0    24578 2024-05-21 13:05:24.576486 gigachain_openai-0.1.7/langchain_openai/llms/base.py
+-rw-r--r--   0        0        0      229 2024-03-28 12:44:20.757798 gigachain_openai-0.1.7/langchain_openai/output_parsers/__init__.py
+-rw-r--r--   0        0        0      229 2024-03-28 12:44:20.758114 gigachain_openai-0.1.7/langchain_openai/output_parsers/tools.py
+-rw-r--r--   0        0        0        0 2024-01-18 15:16:41.017389 gigachain_openai-0.1.7/langchain_openai/py.typed
+-rw-r--r--   0        0        0     2889 2024-05-24 11:13:19.647095 gigachain_openai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2480 1970-01-01 00:00:00.000000 gigachain_openai-0.1.7/PKG-INFO
```

### Comparing `gigachain_openai-0.1.3rc1/LICENSE` & `gigachain_openai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain_openai-0.1.3rc1/README.md` & `gigachain_openai-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This package contains the LangChain integrations for OpenAI through their `openai` SDK.
 
 ## Installation and Setup
 
 - Install the LangChain partner package
 ```bash
-pip install langchain-openai
+pip install gigachain-openai
 ```
 - Get an OpenAI api key and set it as an environment variable (`OPENAI_API_KEY`)
 
 
 ## LLM
 
 See a [usage example](http://python.langchain.com/docs/integrations/llms/openai).
```

### Comparing `gigachain_openai-0.1.3rc1/langchain_openai/chat_models/azure.py` & `gigachain_openai-0.1.7/langchain_openai/chat_models/azure.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 from __future__ import annotations
 
 import logging
 import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import openai
+from langchain_core.language_models.chat_models import LangSmithParams
 from langchain_core.outputs import ChatResult
 from langchain_core.pydantic_v1 import Field, SecretStr, root_validator
 from langchain_core.utils import convert_to_secret_str, get_from_dict_or_env
 
-from langchain_openai.chat_models.base import ChatOpenAI
+from langchain_openai.chat_models.base import BaseChatOpenAI
 
 logger = logging.getLogger(__name__)
 
 
-class AzureChatOpenAI(ChatOpenAI):
+class AzureChatOpenAI(BaseChatOpenAI):
     """`Azure OpenAI` Chat Completion API.
 
     To use this class you
     must have a deployed model on Azure OpenAI. Use `deployment_name` in the
     constructor to refer to the "Model deployment name" in the Azure portal.
 
     In addition, you should have the
@@ -96,14 +97,25 @@
     """
 
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
         """Get the namespace of the langchain object."""
         return ["langchain", "chat_models", "azure_openai"]
 
+    @property
+    def lc_secrets(self) -> Dict[str, str]:
+        return {
+            "openai_api_key": "AZURE_OPENAI_API_KEY",
+            "azure_ad_token": "AZURE_OPENAI_AD_TOKEN",
+        }
+
+    @classmethod
+    def is_lc_serializable(cls) -> bool:
+        return True
+
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         if values["n"] < 1:
             raise ValueError("n must be at least 1.")
         if values["n"] > 1 and values["streaming"]:
             raise ValueError("n must be 1 when streaming.")
@@ -213,14 +225,24 @@
     @property
     def lc_attributes(self) -> Dict[str, Any]:
         return {
             "openai_api_type": self.openai_api_type,
             "openai_api_version": self.openai_api_version,
         }
 
+    def _get_ls_params(
+        self, stop: Optional[List[str]] = None, **kwargs: Any
+    ) -> LangSmithParams:
+        """Get the parameters used to invoke the model."""
+        params = super()._get_ls_params(stop=stop, **kwargs)
+        params["ls_provider"] = "azure"
+        if self.deployment_name:
+            params["ls_model_name"] = self.deployment_name
+        return params
+
     def _create_chat_result(
         self, response: Union[dict, openai.BaseModel]
     ) -> ChatResult:
         if not isinstance(response, dict):
             response = response.model_dump()
         for res in response["choices"]:
             if res.get("finish_reason", None) == "content_filter":
```

### Comparing `gigachain_openai-0.1.3rc1/langchain_openai/chat_models/base.py` & `gigachain_openai-0.1.7/langchain_openai/chat_models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """OpenAI chat wrapper."""
 
 from __future__ import annotations
 
+import json
 import logging
 import os
 import sys
 from operator import itemgetter
 from typing import (
     Any,
     AsyncIterator,
@@ -24,38 +25,40 @@
     Union,
     cast,
     overload,
 )
 
 import openai
 import tiktoken
-from langchain_core._api import beta
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
+    LangSmithParams,
     agenerate_from_stream,
     generate_from_stream,
 )
 from langchain_core.messages import (
     AIMessage,
     AIMessageChunk,
     BaseMessage,
     BaseMessageChunk,
     ChatMessage,
     ChatMessageChunk,
     FunctionMessage,
     FunctionMessageChunk,
     HumanMessage,
     HumanMessageChunk,
+    InvalidToolCall,
     SystemMessage,
     SystemMessageChunk,
+    ToolCall,
     ToolMessage,
     ToolMessageChunk,
 )
 from langchain_core.output_parsers import (
     JsonOutputParser,
     PydanticOutputParser,
 )
@@ -141,46 +144,77 @@
             name=name,
             id=id_,
         )
     else:
         return ChatMessage(content=_dict.get("content", ""), role=role, id=id_)
 
 
+def _format_message_content(content: Any) -> Any:
+    """Format message content."""
+    if content and isinstance(content, list):
+        # Remove unexpected block types
+        formatted_content = []
+        for block in content:
+            if (
+                isinstance(block, dict)
+                and "type" in block
+                and block["type"] == "tool_use"
+            ):
+                continue
+            else:
+                formatted_content.append(block)
+    else:
+        formatted_content = content
+
+    return formatted_content
+
+
 def _convert_message_to_dict(message: BaseMessage) -> dict:
     """Convert a LangChain message to a dictionary.
 
     Args:
         message: The LangChain message.
 
     Returns:
         The dictionary.
     """
     message_dict: Dict[str, Any] = {
-        "content": message.content,
+        "content": _format_message_content(message.content),
     }
     if (name := message.name or message.additional_kwargs.get("name")) is not None:
         message_dict["name"] = name
 
     # populate role and additional message data
     if isinstance(message, ChatMessage):
         message_dict["role"] = message.role
     elif isinstance(message, HumanMessage):
         message_dict["role"] = "user"
     elif isinstance(message, AIMessage):
         message_dict["role"] = "assistant"
         if "function_call" in message.additional_kwargs:
             message_dict["function_call"] = message.additional_kwargs["function_call"]
-            # If function call only, content is None not empty string
-            if message_dict["content"] == "":
-                message_dict["content"] = None
-        if "tool_calls" in message.additional_kwargs:
+        if message.tool_calls or message.invalid_tool_calls:
+            message_dict["tool_calls"] = [
+                _lc_tool_call_to_openai_tool_call(tc) for tc in message.tool_calls
+            ] + [
+                _lc_invalid_tool_call_to_openai_tool_call(tc)
+                for tc in message.invalid_tool_calls
+            ]
+        elif "tool_calls" in message.additional_kwargs:
             message_dict["tool_calls"] = message.additional_kwargs["tool_calls"]
-            # If tool calls only, content is None not empty string
-            if message_dict["content"] == "":
-                message_dict["content"] = None
+            tool_call_supported_props = {"id", "type", "function"}
+            message_dict["tool_calls"] = [
+                {k: v for k, v in tool_call.items() if k in tool_call_supported_props}
+                for tool_call in message_dict["tool_calls"]
+            ]
+        else:
+            pass
+        # If tool calls present, content null value should be None not empty string.
+        if "function_call" in message_dict or "tool_calls" in message_dict:
+            message_dict["content"] = message_dict["content"] or None
     elif isinstance(message, SystemMessage):
         message_dict["role"] = "system"
     elif isinstance(message, FunctionMessage):
         message_dict["role"] = "function"
     elif isinstance(message, ToolMessage):
         message_dict["role"] = "tool"
         message_dict["tool_call_id"] = message.tool_call_id
@@ -254,60 +288,15 @@
 
 class _AllReturnType(TypedDict):
     raw: BaseMessage
     parsed: Optional[_DictOrPydantic]
     parsing_error: Optional[BaseException]
 
 
-class ChatOpenAI(BaseChatModel):
-    """`OpenAI` Chat large language models API.
-
-    To use, you should have the environment variable ``OPENAI_API_KEY``
-    set with your API key, or pass it as a named parameter to the constructor.
-
-    Any parameters that are valid to be passed to the openai.create call can be passed
-    in, even if not explicitly saved on this class.
-
-    Example:
-        .. code-block:: python
-
-            from langchain_openai import ChatOpenAI
-
-            model = ChatOpenAI(model="gpt-3.5-turbo")
-    """
-
-    @property
-    def lc_secrets(self) -> Dict[str, str]:
-        return {"openai_api_key": "OPENAI_API_KEY"}
-
-    @classmethod
-    def get_lc_namespace(cls) -> List[str]:
-        """Get the namespace of the langchain object."""
-        return ["langchain", "chat_models", "openai"]
-
-    @property
-    def lc_attributes(self) -> Dict[str, Any]:
-        attributes: Dict[str, Any] = {}
-
-        if self.openai_organization:
-            attributes["openai_organization"] = self.openai_organization
-
-        if self.openai_api_base:
-            attributes["openai_api_base"] = self.openai_api_base
-
-        if self.openai_proxy:
-            attributes["openai_proxy"] = self.openai_proxy
-
-        return attributes
-
-    @classmethod
-    def is_lc_serializable(cls) -> bool:
-        """Return whether this model can be serialized by Langchain."""
-        return True
-
+class BaseChatOpenAI(BaseChatModel):
     client: Any = Field(default=None, exclude=True)  #: :meta private:
     async_client: Any = Field(default=None, exclude=True)  #: :meta private:
     model_name: str = Field(default="gpt-3.5-turbo", alias="model")
     """Model name to use."""
     temperature: float = 0.7
     """What sampling temperature to use."""
     model_kwargs: Dict[str, Any] = Field(default_factory=dict)
@@ -647,14 +636,31 @@
         return {
             "model": self.model_name,
             **super()._get_invocation_params(stop=stop),
             **self._default_params,
             **kwargs,
         }
 
+    def _get_ls_params(
+        self, stop: Optional[List[str]] = None, **kwargs: Any
+    ) -> LangSmithParams:
+        """Get standard params for tracing."""
+        params = self._get_invocation_params(stop=stop, **kwargs)
+        ls_params = LangSmithParams(
+            ls_provider="openai",
+            ls_model_name=self.model_name,
+            ls_model_type="chat",
+            ls_temperature=params.get("temperature", self.temperature),
+        )
+        if ls_max_tokens := params.get("max_tokens", self.max_tokens):
+            ls_params["ls_max_tokens"] = ls_max_tokens
+        if ls_stop := stop or params.get("stop", None):
+            ls_params["ls_stop"] = ls_stop
+        return ls_params
+
     @property
     def _llm_type(self) -> str:
         """Return type of chat model."""
         return "openai-chat"
 
     def _get_encoding_model(self) -> Tuple[str, tiktoken.Encoding]:
         if self.tiktoken_model_name is not None:
@@ -666,14 +672,16 @@
         except KeyError:
             model = "cl100k_base"
             encoding = tiktoken.get_encoding(model)
         return model, encoding
 
     def get_token_ids(self, text: str) -> List[int]:
         """Get the tokens present in the text with tiktoken package."""
+        if self.custom_get_token_ids is not None:
+            return self.custom_get_token_ids(text)
         # tiktoken NOT supported for Python 3.7 or below
         if sys.version_info[1] <= 7:
             return super().get_token_ids(text)
         _, encoding_model = self._get_encoding_model()
         return encoding_model.encode(text)
 
     def get_num_tokens_from_messages(self, messages: List[BaseMessage]) -> int:
@@ -769,58 +777,78 @@
             **kwargs,
         )
 
     def bind_tools(
         self,
         tools: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable, BaseTool]],
         *,
-        tool_choice: Optional[Union[dict, str, Literal["auto", "none"], bool]] = None,
+        tool_choice: Optional[
+            Union[dict, str, Literal["auto", "none", "required", "any"], bool]
+        ] = None,
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, BaseMessage]:
         """Bind tool-like objects to this chat model.
 
         Assumes model is compatible with OpenAI tool-calling API.
 
         Args:
             tools: A list of tool definitions to bind to this chat model.
                 Can be  a dictionary, pydantic model, callable, or BaseTool. Pydantic
                 models, callables, and BaseTools will be automatically converted to
                 their schema dictionary representation.
             tool_choice: Which tool to require the model to call.
-                Must be the name of the single provided function or
-                "auto" to automatically determine which function to call
-                (if any), or a dict of the form:
+                Options are:
+                name of the tool (str): calls corresponding tool;
+                "auto": automatically selects a tool (including no tool);
+                "none": does not call a tool;
+                "any" or "required": force at least one tool to be called;
+                True: forces tool call (requires `tools` be length 1);
+                False: no effect;
+
+                or a dict of the form:
                 {"type": "function", "function": {"name": <<tool_name>>}}.
             **kwargs: Any additional parameters to pass to the
                 :class:`~langchain.runnable.Runnable` constructor.
         """
 
         formatted_tools = [convert_to_openai_tool(tool) for tool in tools]
-        if tool_choice is not None and tool_choice:
-            if len(formatted_tools) != 1:
-                raise ValueError(
-                    "When specifying `tool_choice`, you must provide exactly one "
-                    f"tool. Received {len(formatted_tools)} tools."
-                )
+        if tool_choice:
             if isinstance(tool_choice, str):
-                if tool_choice not in ("auto", "none"):
+                # tool_choice is a tool/function name
+                if tool_choice not in ("auto", "none", "any", "required"):
                     tool_choice = {
                         "type": "function",
                         "function": {"name": tool_choice},
                     }
+                # 'any' is not natively supported by OpenAI API.
+                # We support 'any' since other models use this instead of 'required'.
+                if tool_choice == "any":
+                    tool_choice = "required"
             elif isinstance(tool_choice, bool):
-                tool_choice = formatted_tools[0]
+                if len(tools) > 1:
+                    raise ValueError(
+                        "tool_choice=True can only be used when a single tool is "
+                        f"passed in, received {len(tools)} tools."
+                    )
+                tool_choice = {
+                    "type": "function",
+                    "function": {"name": formatted_tools[0]["function"]["name"]},
+                }
             elif isinstance(tool_choice, dict):
-                if (
-                    formatted_tools[0]["function"]["name"]
-                    != tool_choice["function"]["name"]
+                tool_names = [
+                    formatted_tool["function"]["name"]
+                    for formatted_tool in formatted_tools
+                ]
+                if not any(
+                    tool_name == tool_choice["function"]["name"]
+                    for tool_name in tool_names
                 ):
                     raise ValueError(
                         f"Tool choice {tool_choice} was specified, but the only "
-                        f"provided tool was {formatted_tools[0]['function']['name']}."
+                        f"provided tools were {tool_names}."
                     )
             else:
                 raise ValueError(
                     f"Unrecognized tool_choice type. Expected str, bool or dict. "
                     f"Received: {tool_choice}"
                 )
             kwargs["tool_choice"] = tool_choice
@@ -844,15 +872,14 @@
         *,
         method: Literal["function_calling", "json_mode"] = "function_calling",
         include_raw: Literal[False] = False,
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, _DictOrPydantic]:
         ...
 
-    @beta()
     def with_structured_output(
         self,
         schema: Optional[_DictOrPydanticClass] = None,
         *,
         method: Literal["function_calling", "json_mode"] = "function_calling",
         include_raw: bool = False,
         **kwargs: Any,
@@ -1052,9 +1079,80 @@
                 [parser_none], exception_key="parsing_error"
             )
             return RunnableMap(raw=llm) | parser_with_fallback
         else:
             return llm | output_parser
 
 
+class ChatOpenAI(BaseChatOpenAI):
+    """`OpenAI` Chat large language models API.
+
+    To use, you should have the environment variable ``OPENAI_API_KEY``
+    set with your API key, or pass it as a named parameter to the constructor.
+
+    Any parameters that are valid to be passed to the openai.create call can be passed
+    in, even if not explicitly saved on this class.
+
+    Example:
+        .. code-block:: python
+
+            from langchain_openai import ChatOpenAI
+
+            model = ChatOpenAI(model="gpt-3.5-turbo")
+    """
+
+    @property
+    def lc_secrets(self) -> Dict[str, str]:
+        return {"openai_api_key": "OPENAI_API_KEY"}
+
+    @classmethod
+    def get_lc_namespace(cls) -> List[str]:
+        """Get the namespace of the langchain object."""
+        return ["langchain", "chat_models", "openai"]
+
+    @property
+    def lc_attributes(self) -> Dict[str, Any]:
+        attributes: Dict[str, Any] = {}
+
+        if self.openai_organization:
+            attributes["openai_organization"] = self.openai_organization
+
+        if self.openai_api_base:
+            attributes["openai_api_base"] = self.openai_api_base
+
+        if self.openai_proxy:
+            attributes["openai_proxy"] = self.openai_proxy
+
+        return attributes
+
+    @classmethod
+    def is_lc_serializable(cls) -> bool:
+        """Return whether this model can be serialized by Langchain."""
+        return True
+
+
 def _is_pydantic_class(obj: Any) -> bool:
     return isinstance(obj, type) and issubclass(obj, BaseModel)
+
+
+def _lc_tool_call_to_openai_tool_call(tool_call: ToolCall) -> dict:
+    return {
+        "type": "function",
+        "id": tool_call["id"],
+        "function": {
+            "name": tool_call["name"],
+            "arguments": json.dumps(tool_call["args"]),
+        },
+    }
+
+
+def _lc_invalid_tool_call_to_openai_tool_call(
+    invalid_tool_call: InvalidToolCall,
+) -> dict:
+    return {
+        "type": "function",
+        "id": invalid_tool_call["id"],
+        "function": {
+            "name": invalid_tool_call["name"],
+            "arguments": invalid_tool_call["args"],
+        },
+    }
```

### Comparing `gigachain_openai-0.1.3rc1/langchain_openai/embeddings/azure.py` & `gigachain_openai-0.1.7/langchain_openai/embeddings/azure.py`

 * *Files identical despite different names*

### Comparing `gigachain_openai-0.1.3rc1/langchain_openai/embeddings/base.py` & `gigachain_openai-0.1.7/langchain_openai/embeddings/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,75 @@
     get_from_dict_or_env,
     get_pydantic_field_names,
 )
 
 logger = logging.getLogger(__name__)
 
 
+def _process_batched_chunked_embeddings(
+    num_texts: int,
+    tokens: List[Union[List[int], str]],
+    batched_embeddings: List[List[float]],
+    indices: List[int],
+    skip_empty: bool,
+) -> List[Optional[List[float]]]:
+    # for each text, this is the list of embeddings (list of list of floats)
+    # corresponding to the chunks of the text
+    results: List[List[List[float]]] = [[] for _ in range(num_texts)]
+
+    # for each text, this is the token length of each chunk
+    # for transformers tokenization, this is the string length
+    # for tiktoken, this is the number of tokens
+    num_tokens_in_batch: List[List[int]] = [[] for _ in range(num_texts)]
+
+    for i in range(len(indices)):
+        if skip_empty and len(batched_embeddings[i]) == 1:
+            continue
+        results[indices[i]].append(batched_embeddings[i])
+        num_tokens_in_batch[indices[i]].append(len(tokens[i]))
+
+    # for each text, this is the final embedding
+    embeddings: List[Optional[List[float]]] = []
+    for i in range(num_texts):
+        # an embedding for each chunk
+        _result: List[List[float]] = results[i]
+
+        if len(_result) == 0:
+            # this will be populated with the embedding of an empty string
+            # in the sync or async code calling this
+            embeddings.append(None)
+            continue
+
+        elif len(_result) == 1:
+            # if only one embedding was produced, use it
+            embeddings.append(_result[0])
+            continue
+
+        else:
+            # else we need to weighted average
+            # should be same as
+            # average = np.average(_result, axis=0, weights=num_tokens_in_batch[i])
+            total_weight = sum(num_tokens_in_batch[i])
+            average = [
+                sum(
+                    val * weight
+                    for val, weight in zip(embedding, num_tokens_in_batch[i])
+                )
+                / total_weight
+                for embedding in zip(*_result)
+            ]
+
+            # should be same as
+            # embeddings.append((average / np.linalg.norm(average)).tolist())
+            magnitude = sum(val**2 for val in average) ** 0.5
+            embeddings.append([val / magnitude for val in average])
+
+    return embeddings
+
+
 class OpenAIEmbeddings(BaseModel, Embeddings):
     """OpenAI embedding models.
 
     To use, you should have the
     environment variable ``OPENAI_API_KEY`` set with your API key or pass it
     as a named parameter to the constructor.
 
@@ -78,16 +139,16 @@
     openai_proxy: Optional[str] = None
     embedding_ctx_length: int = 8191
     """The maximum number of tokens to embed at once."""
     openai_api_key: Optional[SecretStr] = Field(default=None, alias="api_key")
     """Automatically inferred from env var `OPENAI_API_KEY` if not provided."""
     openai_organization: Optional[str] = Field(default=None, alias="organization")
     """Automatically inferred from env var `OPENAI_ORG_ID` if not provided."""
-    allowed_special: Union[Literal["all"], Set[str]] = set()
-    disallowed_special: Union[Literal["all"], Set[str], Sequence[str]] = "all"
+    allowed_special: Union[Literal["all"], Set[str], None] = None
+    disallowed_special: Union[Literal["all"], Set[str], Sequence[str], None] = None
     chunk_size: int = 1000
     """Maximum number of texts to embed in each batch"""
     max_retries: int = 2
     """Maximum number of retries to make when generating."""
     request_timeout: Optional[Union[float, Tuple[float, float], Any]] = Field(
         default=None, alias="timeout"
     )
@@ -125,14 +186,17 @@
     http_client: Union[Any, None] = None
     """Optional httpx.Client. Only used for sync invocations. Must specify 
         http_async_client as well if you'd like a custom client for async invocations.
     """
     http_async_client: Union[Any, None] = None
     """Optional httpx.AsyncClient. Only used for async invocations. Must specify 
         http_client as well if you'd like a custom client for sync invocations."""
+    check_embedding_ctx_length: bool = True
+    """Whether to check the token length of inputs and automatically split inputs 
+        longer than embedding_ctx_length."""
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
         allow_population_by_field_name = True
 
@@ -239,145 +303,158 @@
     @property
     def _invocation_params(self) -> Dict[str, Any]:
         params: Dict = {"model": self.model, **self.model_kwargs}
         if self.dimensions is not None:
             params["dimensions"] = self.dimensions
         return params
 
-    # please refer to
-    # https://github.com/openai/openai-cookbook/blob/main/examples/Embedding_long_inputs.ipynb
-    def _get_len_safe_embeddings(
-        self, texts: List[str], *, engine: str, chunk_size: Optional[int] = None
-    ) -> List[List[float]]:
+    def _tokenize(
+        self, texts: List[str], chunk_size: int
+    ) -> Tuple[Iterable[int], List[Union[List[int], str]], List[int]]:
         """
-        Generate length-safe embeddings for a list of texts.
+        Take the input `texts` and `chunk_size` and return 3 iterables as a tuple:
 
-        This method handles tokenization and embedding generation, respecting the
-        set embedding context length and chunk size. It supports both tiktoken
-        and HuggingFace tokenizer based on the tiktoken_enabled flag.
-
-        Args:
-            texts (List[str]): A list of texts to embed.
-            engine (str): The engine or model to use for embeddings.
-            chunk_size (Optional[int]): The size of chunks for processing embeddings.
-
-        Returns:
-            List[List[float]]: A list of embeddings for each input text.
+        We have `batches`, where batches are sets of individual texts
+        we want responses from the openai api. The length of a single batch is
+        `chunk_size` texts.
+
+        Each individual text is also split into multiple texts based on the
+        `embedding_ctx_length` parameter (based on number of tokens).
+
+        This function returns a 3-tuple of the following:
+
+        _iter: An iterable of the starting index in `tokens` for each *batch*
+        tokens: A list of tokenized texts, where each text has already been split
+            into sub-texts based on the `embedding_ctx_length` parameter. In the
+            case of tiktoken, this is a list of token arrays. In the case of
+            HuggingFace transformers, this is a list of strings.
+        indices: An iterable of the same length as `tokens` that maps each token-array
+            to the index of the original text in `texts`.
         """
-
-        tokens = []
-        indices = []
+        tokens: List[Union[List[int], str]] = []
+        indices: List[int] = []
         model_name = self.tiktoken_model_name or self.model
-        _chunk_size = chunk_size or self.chunk_size
 
         # If tiktoken flag set to False
         if not self.tiktoken_enabled:
             try:
-                from transformers import AutoTokenizer  # noqa: F401
+                from transformers import AutoTokenizer
             except ImportError:
                 raise ValueError(
                     "Could not import transformers python package. "
                     "This is needed in order to for OpenAIEmbeddings without "
                     "`tiktoken`. Please install it with `pip install transformers`. "
                 )
 
             tokenizer = AutoTokenizer.from_pretrained(
                 pretrained_model_name_or_path=model_name
             )
             for i, text in enumerate(texts):
                 # Tokenize the text using HuggingFace transformers
-                tokenized = tokenizer.encode(text, add_special_tokens=False)
+                tokenized: List[int] = tokenizer.encode(text, add_special_tokens=False)
 
                 # Split tokens into chunks respecting the embedding_ctx_length
                 for j in range(0, len(tokenized), self.embedding_ctx_length):
-                    token_chunk = tokenized[j : j + self.embedding_ctx_length]
+                    token_chunk: List[int] = tokenized[
+                        j : j + self.embedding_ctx_length
+                    ]
 
                     # Convert token IDs back to a string
-                    chunk_text = tokenizer.decode(token_chunk)
+                    chunk_text: str = tokenizer.decode(token_chunk)
                     tokens.append(chunk_text)
                     indices.append(i)
         else:
             try:
                 encoding = tiktoken.encoding_for_model(model_name)
             except KeyError:
                 encoding = tiktoken.get_encoding("cl100k_base")
+            encoder_kwargs: Dict[str, Any] = {
+                k: v
+                for k, v in {
+                    "allowed_special": self.allowed_special,
+                    "disallowed_special": self.disallowed_special,
+                }.items()
+                if v is not None
+            }
             for i, text in enumerate(texts):
                 if self.model.endswith("001"):
                     # See: https://github.com/openai/openai-python/
                     #      issues/418#issuecomment-1525939500
                     # replace newlines, which can negatively affect performance.
                     text = text.replace("\n", " ")
 
-                token = encoding.encode(
-                    text=text,
-                    allowed_special=self.allowed_special,
-                    disallowed_special=self.disallowed_special,
-                )
+                if encoder_kwargs:
+                    token = encoding.encode(text, **encoder_kwargs)
+                else:
+                    token = encoding.encode_ordinary(text)
 
                 # Split tokens into chunks respecting the embedding_ctx_length
                 for j in range(0, len(token), self.embedding_ctx_length):
                     tokens.append(token[j : j + self.embedding_ctx_length])
                     indices.append(i)
 
         if self.show_progress_bar:
             try:
                 from tqdm.auto import tqdm
 
-                _iter: Iterable = tqdm(range(0, len(tokens), _chunk_size))
+                _iter: Iterable = tqdm(range(0, len(tokens), chunk_size))
             except ImportError:
-                _iter = range(0, len(tokens), _chunk_size)
+                _iter = range(0, len(tokens), chunk_size)
         else:
-            _iter = range(0, len(tokens), _chunk_size)
+            _iter = range(0, len(tokens), chunk_size)
+        return _iter, tokens, indices
+
+    # please refer to
+    # https://github.com/openai/openai-cookbook/blob/main/examples/Embedding_long_inputs.ipynb
+    def _get_len_safe_embeddings(
+        self, texts: List[str], *, engine: str, chunk_size: Optional[int] = None
+    ) -> List[List[float]]:
+        """
+        Generate length-safe embeddings for a list of texts.
 
+        This method handles tokenization and embedding generation, respecting the
+        set embedding context length and chunk size. It supports both tiktoken
+        and HuggingFace tokenizer based on the tiktoken_enabled flag.
+
+        Args:
+            texts (List[str]): A list of texts to embed.
+            engine (str): The engine or model to use for embeddings.
+            chunk_size (Optional[int]): The size of chunks for processing embeddings.
+
+        Returns:
+            List[List[float]]: A list of embeddings for each input text.
+        """
+        _chunk_size = chunk_size or self.chunk_size
+        _iter, tokens, indices = self._tokenize(texts, _chunk_size)
         batched_embeddings: List[List[float]] = []
         for i in _iter:
             response = self.client.create(
                 input=tokens[i : i + _chunk_size], **self._invocation_params
             )
             if not isinstance(response, dict):
                 response = response.model_dump()
             batched_embeddings.extend(r["embedding"] for r in response["data"])
 
-        results: List[List[List[float]]] = [[] for _ in range(len(texts))]
-        num_tokens_in_batch: List[List[int]] = [[] for _ in range(len(texts))]
-        for i in range(len(indices)):
-            if self.skip_empty and len(batched_embeddings[i]) == 1:
-                continue
-            results[indices[i]].append(batched_embeddings[i])
-            num_tokens_in_batch[indices[i]].append(len(tokens[i]))
-
-        embeddings: List[List[float]] = [[] for _ in range(len(texts))]
-        for i in range(len(texts)):
-            _result = results[i]
-            if len(_result) == 0:
+        embeddings = _process_batched_chunked_embeddings(
+            len(texts), tokens, batched_embeddings, indices, self.skip_empty
+        )
+        _cached_empty_embedding: Optional[List[float]] = None
+
+        def empty_embedding() -> List[float]:
+            nonlocal _cached_empty_embedding
+            if _cached_empty_embedding is None:
                 average_embedded = self.client.create(
                     input="", **self._invocation_params
                 )
                 if not isinstance(average_embedded, dict):
                     average_embedded = average_embedded.model_dump()
-                average = average_embedded["data"][0]["embedding"]
-            else:
-                # should be same as
-                # average = np.average(_result, axis=0, weights=num_tokens_in_batch[i])
-                total_weight = sum(num_tokens_in_batch[i])
-                average = [
-                    sum(
-                        val * weight
-                        for val, weight in zip(embedding, num_tokens_in_batch[i])
-                    )
-                    / total_weight
-                    for embedding in zip(*_result)
-                ]
+                _cached_empty_embedding = average_embedded["data"][0]["embedding"]
+            return _cached_empty_embedding
 
-            # should be same as
-            #  embeddings[i] = (average / np.linalg.norm(average)).tolist()
-            magnitude = sum(val**2 for val in average) ** 0.5
-            embeddings[i] = [val / magnitude for val in average]
-
-        return embeddings
+        return [e if e is not None else empty_embedding() for e in embeddings]
 
     # please refer to
     # https://github.com/openai/openai-cookbook/blob/main/examples/Embedding_long_inputs.ipynb
     async def _aget_len_safe_embeddings(
         self, texts: List[str], *, engine: str, chunk_size: Optional[int] = None
     ) -> List[List[float]]:
         """
@@ -392,129 +469,70 @@
             engine (str): The engine or model to use for embeddings.
             chunk_size (Optional[int]): The size of chunks for processing embeddings.
 
         Returns:
             List[List[float]]: A list of embeddings for each input text.
         """
 
-        tokens = []
-        indices = []
-        model_name = self.tiktoken_model_name or self.model
         _chunk_size = chunk_size or self.chunk_size
-
-        # If tiktoken flag set to False
-        if not self.tiktoken_enabled:
-            try:
-                from transformers import AutoTokenizer
-            except ImportError:
-                raise ValueError(
-                    "Could not import transformers python package. "
-                    "This is needed in order to for OpenAIEmbeddings without "
-                    " `tiktoken`. Please install it with `pip install transformers`."
-                )
-
-            tokenizer = AutoTokenizer.from_pretrained(
-                pretrained_model_name_or_path=model_name
-            )
-            for i, text in enumerate(texts):
-                # Tokenize the text using HuggingFace transformers
-                tokenized = tokenizer.encode(text, add_special_tokens=False)
-
-                # Split tokens into chunks respecting the embedding_ctx_length
-                for j in range(0, len(tokenized), self.embedding_ctx_length):
-                    token_chunk = tokenized[j : j + self.embedding_ctx_length]
-
-                    # Convert token IDs back to a string
-                    chunk_text = tokenizer.decode(token_chunk)
-                    tokens.append(chunk_text)
-                    indices.append(i)
-        else:
-            try:
-                encoding = tiktoken.encoding_for_model(model_name)
-            except KeyError:
-                logger.warning("Warning: model not found. Using cl100k_base encoding.")
-                model = "cl100k_base"
-                encoding = tiktoken.get_encoding(model)
-            for i, text in enumerate(texts):
-                if self.model.endswith("001"):
-                    # See: https://github.com/openai/openai-python/
-                    #      issues/418#issuecomment-1525939500
-                    # replace newlines, which can negatively affect performance.
-                    text = text.replace("\n", " ")
-
-                token = encoding.encode(
-                    text=text,
-                    allowed_special=self.allowed_special,
-                    disallowed_special=self.disallowed_special,
-                )
-
-                # Split tokens into chunks respecting the embedding_ctx_length
-                for j in range(0, len(token), self.embedding_ctx_length):
-                    tokens.append(token[j : j + self.embedding_ctx_length])
-                    indices.append(i)
-
+        _iter, tokens, indices = self._tokenize(texts, _chunk_size)
         batched_embeddings: List[List[float]] = []
         _chunk_size = chunk_size or self.chunk_size
         for i in range(0, len(tokens), _chunk_size):
             response = await self.async_client.create(
                 input=tokens[i : i + _chunk_size], **self._invocation_params
             )
 
             if not isinstance(response, dict):
                 response = response.model_dump()
             batched_embeddings.extend(r["embedding"] for r in response["data"])
 
-        results: List[List[List[float]]] = [[] for _ in range(len(texts))]
-        num_tokens_in_batch: List[List[int]] = [[] for _ in range(len(texts))]
-        for i in range(len(indices)):
-            results[indices[i]].append(batched_embeddings[i])
-            num_tokens_in_batch[indices[i]].append(len(tokens[i]))
-
-        embeddings: List[List[float]] = [[] for _ in range(len(texts))]
-        for i in range(len(texts)):
-            _result = results[i]
-            if len(_result) == 0:
+        embeddings = _process_batched_chunked_embeddings(
+            len(texts), tokens, batched_embeddings, indices, self.skip_empty
+        )
+        _cached_empty_embedding: Optional[List[float]] = None
+
+        async def empty_embedding() -> List[float]:
+            nonlocal _cached_empty_embedding
+            if _cached_empty_embedding is None:
                 average_embedded = await self.async_client.create(
                     input="", **self._invocation_params
                 )
                 if not isinstance(average_embedded, dict):
                     average_embedded = average_embedded.model_dump()
-                average = average_embedded["data"][0]["embedding"]
-            else:
-                # should be same as
-                # average = np.average(_result, axis=0, weights=num_tokens_in_batch[i])
-                total_weight = sum(num_tokens_in_batch[i])
-                average = [
-                    sum(
-                        val * weight
-                        for val, weight in zip(embedding, num_tokens_in_batch[i])
-                    )
-                    / total_weight
-                    for embedding in zip(*_result)
-                ]
-            # should be same as
-            # embeddings[i] = (average / np.linalg.norm(average)).tolist()
-            magnitude = sum(val**2 for val in average) ** 0.5
-            embeddings[i] = [val / magnitude for val in average]
+                _cached_empty_embedding = average_embedded["data"][0]["embedding"]
+            return _cached_empty_embedding
 
-        return embeddings
+        return [e if e is not None else await empty_embedding() for e in embeddings]
 
     def embed_documents(
         self, texts: List[str], chunk_size: Optional[int] = 0
     ) -> List[List[float]]:
         """Call out to OpenAI's embedding endpoint for embedding search docs.
 
         Args:
             texts: The list of texts to embed.
             chunk_size: The chunk size of embeddings. If None, will use the chunk size
                 specified by the class.
 
         Returns:
             List of embeddings, one for each text.
         """
+        if not self.check_embedding_ctx_length:
+            embeddings: List[List[float]] = []
+            for text in texts:
+                response = self.client.create(
+                    input=text,
+                    **self._invocation_params,
+                )
+                if not isinstance(response, dict):
+                    response = response.dict()
+                embeddings.extend(r["embedding"] for r in response["data"])
+            return embeddings
+
         # NOTE: to keep things simple, we assume the list may contain texts longer
         #       than the maximum context and use length-safe embedding function.
         engine = cast(str, self.deployment)
         return self._get_len_safe_embeddings(texts, engine=engine)
 
     async def aembed_documents(
         self, texts: List[str], chunk_size: Optional[int] = 0
@@ -525,14 +543,26 @@
             texts: The list of texts to embed.
             chunk_size: The chunk size of embeddings. If None, will use the chunk size
                 specified by the class.
 
         Returns:
             List of embeddings, one for each text.
         """
+        if not self.check_embedding_ctx_length:
+            embeddings: List[List[float]] = []
+            for text in texts:
+                response = await self.async_client.create(
+                    input=text,
+                    **self._invocation_params,
+                )
+                if not isinstance(response, dict):
+                    response = response.dict()
+                embeddings.extend(r["embedding"] for r in response["data"])
+            return embeddings
+
         # NOTE: to keep things simple, we assume the list may contain texts longer
         #       than the maximum context and use length-safe embedding function.
         engine = cast(str, self.deployment)
         return await self._aget_len_safe_embeddings(texts, engine=engine)
 
     def embed_query(self, text: str) -> List[float]:
         """Call out to OpenAI's embedding endpoint for embedding query text.
```

### Comparing `gigachain_openai-0.1.3rc1/langchain_openai/llms/azure.py` & `gigachain_openai-0.1.7/langchain_openai/llms/azure.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,26 @@
     """
 
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
         """Get the namespace of the langchain object."""
         return ["langchain", "llms", "openai"]
 
+    @property
+    def lc_secrets(self) -> Dict[str, str]:
+        return {
+            "openai_api_key": "AZURE_OPENAI_API_KEY",
+            "azure_ad_token": "AZURE_OPENAI_AD_TOKEN",
+        }
+
+    @classmethod
+    def is_lc_serializable(cls) -> bool:
+        """Return whether this model can be serialized by Langchain."""
+        return True
+
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         if values["n"] < 1:
             raise ValueError("n must be at least 1.")
         if values["streaming"] and values["n"] > 1:
             raise ValueError("Cannot stream results when n > 1.")
```

### Comparing `gigachain_openai-0.1.3rc1/langchain_openai/llms/base.py` & `gigachain_openai-0.1.7/langchain_openai/llms/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,32 +64,14 @@
         ),
     )
 
 
 class BaseOpenAI(BaseLLM):
     """Base OpenAI large language model class."""
 
-    @property
-    def lc_secrets(self) -> Dict[str, str]:
-        return {"openai_api_key": "OPENAI_API_KEY"}
-
-    @property
-    def lc_attributes(self) -> Dict[str, Any]:
-        attributes: Dict[str, Any] = {}
-        if self.openai_api_base:
-            attributes["openai_api_base"] = self.openai_api_base
-
-        if self.openai_organization:
-            attributes["openai_organization"] = self.openai_organization
-
-        if self.openai_proxy:
-            attributes["openai_proxy"] = self.openai_proxy
-
-        return attributes
-
     client: Any = Field(default=None, exclude=True)  #: :meta private:
     async_client: Any = Field(default=None, exclude=True)  #: :meta private:
     model_name: str = Field(default="gpt-3.5-turbo-instruct", alias="model")
     """Model name to use."""
     temperature: float = 0.7
     """What sampling temperature to use."""
     max_tokens: int = 256
@@ -517,14 +499,16 @@
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "openai"
 
     def get_token_ids(self, text: str) -> List[int]:
         """Get the token IDs using the tiktoken package."""
+        if self.custom_get_token_ids is not None:
+            return self.custom_get_token_ids(text)
         # tiktoken NOT supported for Python < 3.8
         if sys.version_info[1] < 8:
             return super().get_num_tokens(text)
 
         model_name = self.tiktoken_model_name or self.model_name
         try:
             enc = tiktoken.encoding_for_model(model_name)
@@ -643,7 +627,25 @@
     def is_lc_serializable(cls) -> bool:
         """Return whether this model can be serialized by Langchain."""
         return True
 
     @property
     def _invocation_params(self) -> Dict[str, Any]:
         return {**{"model": self.model_name}, **super()._invocation_params}
+
+    @property
+    def lc_secrets(self) -> Dict[str, str]:
+        return {"openai_api_key": "OPENAI_API_KEY"}
+
+    @property
+    def lc_attributes(self) -> Dict[str, Any]:
+        attributes: Dict[str, Any] = {}
+        if self.openai_api_base:
+            attributes["openai_api_base"] = self.openai_api_base
+
+        if self.openai_organization:
+            attributes["openai_organization"] = self.openai_organization
+
+        if self.openai_proxy:
+            attributes["openai_proxy"] = self.openai_proxy
+
+        return attributes
```

### Comparing `gigachain_openai-0.1.3rc1/pyproject.toml` & `gigachain_openai-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [tool.poetry]
 name = "gigachain-openai"
-version = "0.1.3rc1"
+version = "0.1.7"
 description = "An integration package connecting OpenAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 packages = [
     {include = "langchain_openai"}
 ]
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-gigachain-core = { version = "^0.1.42rc1", allow-prereleases = true }
-openai = "^1.10.0"
-tiktoken = ">=0.5.2,<1"
+gigachain-core = ">=0.1.46,<0.3"
+openai = "^1.24.0"
+tiktoken = ">=0.7,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 gigachain-core = { path = "../../core", develop = true }
 pytest-cov = "^4.1.0"
 gigachain-standard-tests = { path = "../../standard-tests", develop = true }
+numpy = "^1.24"
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
```

### Comparing `gigachain_openai-0.1.3rc1/PKG-INFO` & `gigachain_openai-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: gigachain-openai
-Version: 0.1.3rc1
+Version: 0.1.7
 Summary: An integration package connecting OpenAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: gigachain-core (>=0.1.42rc1,<0.2.0)
-Requires-Dist: openai (>=1.10.0,<2.0.0)
-Requires-Dist: tiktoken (>=0.5.2,<1)
+Requires-Dist: gigachain-core (>=0.1.46,<0.3)
+Requires-Dist: openai (>=1.24.0,<2.0.0)
+Requires-Dist: tiktoken (>=0.7,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai
 Description-Content-Type: text/markdown
 
 # langchain-openai
 
 This package contains the LangChain integrations for OpenAI through their `openai` SDK.
 
 ## Installation and Setup
 
 - Install the LangChain partner package
 ```bash
-pip install langchain-openai
+pip install gigachain-openai
 ```
 - Get an OpenAI api key and set it as an environment variable (`OPENAI_API_KEY`)
 
 
 ## LLM
 
 See a [usage example](http://python.langchain.com/docs/integrations/llms/openai).
```

