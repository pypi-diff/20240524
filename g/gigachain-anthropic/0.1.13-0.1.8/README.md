# Comparing `tmp/gigachain_anthropic-0.1.13.tar.gz` & `tmp/gigachain_anthropic-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachain_anthropic-0.1.13.tar", max compression
+gzip compressed data, was "gigachain_anthropic-0.1.8.tar", max compression
```

## Comparing `gigachain_anthropic-0.1.13.tar` & `gigachain_anthropic-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-01-10 09:04:40.690050 gigachain_anthropic-0.1.13/LICENSE
--rw-r--r--   0        0        0     1215 2024-04-19 07:38:34.294261 gigachain_anthropic-0.1.13/README.md
--rw-r--r--   0        0        0      225 2024-03-28 12:44:20.640749 gigachain_anthropic-0.1.13/langchain_anthropic/__init__.py
--rw-r--r--   0        0        0    33510 2024-05-24 11:13:19.482258 gigachain_anthropic-0.1.13/langchain_anthropic/chat_models.py
--rw-r--r--   0        0        0     4908 2024-05-24 11:13:19.484541 gigachain_anthropic-0.1.13/langchain_anthropic/experimental.py
--rw-r--r--   0        0        0    12430 2024-05-24 11:13:19.485852 gigachain_anthropic-0.1.13/langchain_anthropic/llms.py
--rw-r--r--   0        0        0     2493 2024-04-19 07:38:34.307152 gigachain_anthropic-0.1.13/langchain_anthropic/output_parsers.py
--rw-r--r--   0        0        0        0 2024-01-10 09:04:40.692021 gigachain_anthropic-0.1.13/langchain_anthropic/py.typed
--rw-r--r--   0        0        0     2816 2024-05-24 11:13:19.491623 gigachain_anthropic-0.1.13/pyproject.toml
--rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 gigachain_anthropic-0.1.13/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-01-10 09:04:40.690050 gigachain_anthropic-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1215 2024-03-28 12:44:20.640287 gigachain_anthropic-0.1.8/README.md
+-rw-r--r--   0        0        0      225 2024-03-28 12:44:20.640749 gigachain_anthropic-0.1.8/langchain_anthropic/__init__.py
+-rw-r--r--   0        0        0    26817 2024-04-16 13:13:31.615776 gigachain_anthropic-0.1.8/langchain_anthropic/chat_models.py
+-rw-r--r--   0        0        0     4908 2024-04-11 16:04:03.824691 gigachain_anthropic-0.1.8/langchain_anthropic/experimental.py
+-rw-r--r--   0        0        0    11687 2024-04-11 16:04:03.825940 gigachain_anthropic-0.1.8/langchain_anthropic/llms.py
+-rw-r--r--   0        0        0     2493 2024-04-11 16:04:03.826390 gigachain_anthropic-0.1.8/langchain_anthropic/output_parsers.py
+-rw-r--r--   0        0        0        0 2024-01-10 09:04:40.692021 gigachain_anthropic-0.1.8/langchain_anthropic/py.typed
+-rw-r--r--   0        0        0     2807 2024-04-16 16:21:28.033581 gigachain_anthropic-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 gigachain_anthropic-0.1.8/PKG-INFO
```

### Comparing `gigachain_anthropic-0.1.13/LICENSE` & `gigachain_anthropic-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachain_anthropic-0.1.13/README.md` & `gigachain_anthropic-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `gigachain_anthropic-0.1.13/langchain_anthropic/chat_models.py` & `gigachain_anthropic-0.1.8/langchain_anthropic/chat_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     Dict,
     Iterator,
     List,
-    Literal,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypedDict,
     Union,
@@ -26,25 +25,23 @@
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
-    LangSmithParams,
     agenerate_from_stream,
     generate_from_stream,
 )
 from langchain_core.messages import (
     AIMessage,
     AIMessageChunk,
     BaseMessage,
     HumanMessage,
     SystemMessage,
-    ToolCall,
     ToolMessage,
 )
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
 from langchain_core.pydantic_v1 import BaseModel, Field, SecretStr, root_validator
 from langchain_core.runnables import (
     Runnable,
     RunnableMap,
@@ -92,20 +89,19 @@
         "type": "base64",
         "media_type": match.group("media_type"),
         "data": match.group("data"),
     }
 
 
 def _merge_messages(
-    messages: Sequence[BaseMessage],
+    messages: List[BaseMessage],
 ) -> List[Union[SystemMessage, AIMessage, HumanMessage]]:
     """Merge runs of human/tool messages into single human messages with content blocks."""  # noqa: E501
     merged: list = []
     for curr in messages:
-        curr = curr.copy(deep=True)
         if isinstance(curr, ToolMessage):
             if isinstance(curr.content, str):
                 curr = HumanMessage(
                     [
                         {
                             "type": "tool_result",
                             "content": curr.content,
@@ -156,15 +152,15 @@
                     "System message must be a string, "
                     f"instead was: {type(message.content)}"
                 )
             system = message.content
             continue
 
         role = _message_type_lookups[message.type]
-        content: Union[str, List]
+        content: Union[str, List[Dict]]
 
         if not isinstance(message.content, str):
             # parse as dict
             assert isinstance(
                 message.content, list
             ), "Anthropic message content must be str or list of dicts"
 
@@ -189,46 +185,20 @@
                                 "type": "image",
                                 "source": source,
                             }
                         )
                     elif item["type"] == "tool_use":
                         item.pop("text", None)
                         content.append(item)
-                    elif item["type"] == "text":
-                        text = item.get("text", "")
-                        # Only add non-empty strings for now as empty ones are not
-                        # accepted.
-                        # https://github.com/anthropics/anthropic-sdk-python/issues/461
-                        if text.strip():
-                            content.append(
-                                {
-                                    "type": "text",
-                                    "text": text,
-                                }
-                            )
                     else:
                         content.append(item)
                 else:
                     raise ValueError(
                         f"Content items must be str or dict, instead was: {type(item)}"
                     )
-        elif (
-            isinstance(message, AIMessage)
-            and not isinstance(message.content, list)
-            and message.tool_calls
-        ):
-            content = (
-                []
-                if not message.content
-                else [{"type": "text", "text": message.content}]
-            )
-            # Note: Anthropic can't have invalid tool calls as presently defined,
-            # since the model already returns dicts args not JSON strings, and invalid
-            # tool calls are those with invalid JSON for args.
-            content += _lc_tool_calls_to_anthropic_tool_use_blocks(message.tool_calls)
         else:
             content = message.content
 
         formatted_messages.append(
             {
                 "role": role,
                 "content": content,
@@ -277,15 +247,15 @@
     default_request_timeout: Optional[float] = Field(None, alias="timeout")
     """Timeout for requests to Anthropic Completion API."""
 
     # sdk default = 2: https://github.com/anthropics/anthropic-sdk-python?tab=readme-ov-file#retries
     max_retries: int = 2
     """Number of retries allowed for requests sent to the Anthropic Completion API."""
 
-    anthropic_api_url: Optional[str] = None
+    anthropic_api_url: str = "https://api.anthropic.com"
 
     anthropic_api_key: Optional[SecretStr] = Field(None, alias="api_key")
     """Automatically read from env var `ANTHROPIC_API_KEY` if not provided."""
 
     default_headers: Optional[Mapping[str, str]] = None
     """Headers to pass to the Anthropic clients, will be used for every API call."""
 
@@ -295,59 +265,14 @@
     """Whether to use streaming or not."""
 
     @property
     def _llm_type(self) -> str:
         """Return type of chat model."""
         return "anthropic-chat"
 
-    @property
-    def lc_secrets(self) -> Dict[str, str]:
-        return {"anthropic_api_key": "ANTHROPIC_API_KEY"}
-
-    @classmethod
-    def is_lc_serializable(cls) -> bool:
-        return True
-
-    @classmethod
-    def get_lc_namespace(cls) -> List[str]:
-        """Get the namespace of the langchain object."""
-        return ["langchain", "chat_models", "anthropic"]
-
-    @property
-    def _identifying_params(self) -> Dict[str, Any]:
-        """Get the identifying parameters."""
-        return {
-            "model": self.model,
-            "max_tokens": self.max_tokens,
-            "temperature": self.temperature,
-            "top_k": self.top_k,
-            "top_p": self.top_p,
-            "model_kwargs": self.model_kwargs,
-            "streaming": self.streaming,
-            "max_retries": self.max_retries,
-            "default_request_timeout": self.default_request_timeout,
-        }
-
-    def _get_ls_params(
-        self, stop: Optional[List[str]] = None, **kwargs: Any
-    ) -> LangSmithParams:
-        """Get the parameters used to invoke the model."""
-        params = self._get_invocation_params(stop=stop, **kwargs)
-        ls_params = LangSmithParams(
-            ls_provider="anthropic",
-            ls_model_name=self.model,
-            ls_model_type="chat",
-            ls_temperature=params.get("temperature", self.temperature),
-        )
-        if ls_max_tokens := params.get("max_tokens", self.max_tokens):
-            ls_params["ls_max_tokens"] = ls_max_tokens
-        if ls_stop := stop or params.get("stop", None):
-            ls_params["ls_stop"] = ls_stop
-        return ls_params
-
     @root_validator(pre=True)
     def build_extra(cls, values: Dict) -> Dict:
         extra = values.get("model_kwargs", {})
         all_required_field_names = get_pydantic_field_names(cls)
         values["model_kwargs"] = build_extra_kwargs(
             extra, values, all_required_field_names
         )
@@ -556,126 +481,53 @@
             data = await self._async_client.messages.create(**params)
         return self._format_output(data, **kwargs)
 
     @beta()
     def bind_tools(
         self,
         tools: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable, BaseTool]],
-        *,
-        tool_choice: Optional[
-            Union[Dict[str, str], Literal["any", "auto"], str]
-        ] = None,
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, BaseMessage]:
         """Bind tool-like objects to this chat model.
 
         Args:
             tools: A list of tool definitions to bind to this chat model.
                 Can be  a dictionary, pydantic model, callable, or BaseTool. Pydantic
                 models, callables, and BaseTools will be automatically converted to
                 their schema dictionary representation.
-            tool_choice: Which tool to require the model to call.
-                Options are:
-                    name of the tool (str): calls corresponding tool;
-                    "auto" or None: automatically selects a tool (including no tool);
-                    "any": force at least one tool to be called;
-                    or a dict of the form:
-                        {"type": "tool", "name": "tool_name"},
-                        or {"type: "any"},
-                        or {"type: "auto"};
             **kwargs: Any additional parameters to bind.
 
         Example:
             .. code-block:: python
 
                 from langchain_anthropic import ChatAnthropic
                 from langchain_core.pydantic_v1 import BaseModel, Field
 
                 class GetWeather(BaseModel):
                     '''Get the current weather in a given location'''
 
                     location: str = Field(..., description="The city and state, e.g. San Francisco, CA")
 
-                class GetPrice(BaseModel):
-                    '''Get the price of a specific product.'''
-
-                    product: str = Field(..., description="The product to look up.")
-
 
                 llm = ChatAnthropic(model="claude-3-opus-20240229", temperature=0)
-                llm_with_tools = llm.bind_tools([GetWeather, GetPrice])
+                llm_with_tools = llm.bind_tools([GetWeather])
                 llm_with_tools.invoke("what is the weather like in San Francisco",)
                 # -> AIMessage(
                 #     content=[
                 #         {'text': '<thinking>\nBased on the user\'s question, the relevant function to call is GetWeather, which requires the "location" parameter.\n\nThe user has directly specified the location as "San Francisco". Since San Francisco is a well known city, I can reasonably infer they mean San Francisco, CA without needing the state specified.\n\nAll the required parameters are provided, so I can proceed with the API call.\n</thinking>', 'type': 'text'},
                 #         {'text': None, 'type': 'tool_use', 'id': 'toolu_01SCgExKzQ7eqSkMHfygvYuu', 'name': 'GetWeather', 'input': {'location': 'San Francisco, CA'}}
                 #     ],
                 #     response_metadata={'id': 'msg_01GM3zQtoFv8jGQMW7abLnhi', 'model': 'claude-3-opus-20240229', 'stop_reason': 'tool_use', 'stop_sequence': None, 'usage': {'input_tokens': 487, 'output_tokens': 145}},
                 #     id='run-87b1331e-9251-4a68-acef-f0a018b639cc-0'
                 # )
-
-        Example — force tool call with tool_choice 'any':
-            .. code-block:: python
-
-                from langchain_anthropic import ChatAnthropic
-                from langchain_core.pydantic_v1 import BaseModel, Field
-
-                class GetWeather(BaseModel):
-                    '''Get the current weather in a given location'''
-
-                    location: str = Field(..., description="The city and state, e.g. San Francisco, CA")
-
-                class GetPrice(BaseModel):
-                    '''Get the price of a specific product.'''
-
-                    product: str = Field(..., description="The product to look up.")
-
-
-                llm = ChatAnthropic(model="claude-3-opus-20240229", temperature=0)
-                llm_with_tools = llm.bind_tools([GetWeather, GetPrice], tool_choice="any")
-                llm_with_tools.invoke("what is the weather like in San Francisco",)
-
-
-        Example — force specific tool call with tool_choice '<name_of_tool>':
-            .. code-block:: python
-
-                from langchain_anthropic import ChatAnthropic
-                from langchain_core.pydantic_v1 import BaseModel, Field
-
-                class GetWeather(BaseModel):
-                    '''Get the current weather in a given location'''
-
-                    location: str = Field(..., description="The city and state, e.g. San Francisco, CA")
-
-                class GetPrice(BaseModel):
-                    '''Get the price of a specific product.'''
-
-                    product: str = Field(..., description="The product to look up.")
-
-
-                llm = ChatAnthropic(model="claude-3-opus-20240229", temperature=0)
-                llm_with_tools = llm.bind_tools([GetWeather, GetPrice], tool_choice="GetWeather")
-                llm_with_tools.invoke("what is the weather like in San Francisco",)
         """  # noqa: E501
         formatted_tools = [convert_to_anthropic_tool(tool) for tool in tools]
-        if not tool_choice:
-            pass
-        elif isinstance(tool_choice, dict):
-            kwargs["tool_choice"] = tool_choice
-        elif isinstance(tool_choice, str) and tool_choice in ("any", "auto"):
-            kwargs["tool_choice"] = {"type": tool_choice}
-        elif isinstance(tool_choice, str):
-            kwargs["tool_choice"] = {"type": "tool", "name": tool_choice}
-        else:
-            raise ValueError(
-                f"Unrecognized 'tool_choice' type {tool_choice=}. Expected dict, "
-                f"str, or None."
-            )
         return self.bind(tools=formatted_tools, **kwargs)
 
+    @beta()
     def with_structured_output(
         self,
         schema: Union[Dict, Type[BaseModel]],
         *,
         include_raw: bool = False,
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, Union[Dict, BaseModel]]:
@@ -771,15 +623,15 @@
                 structured_llm.invoke("What weighs more a pound of bricks or a pound of feathers")
                 # -> {
                 #     'answer': 'They weigh the same',
                 #     'justification': 'Both a pound of bricks and a pound of feathers weigh one pound. The weight is the same, but the volume and density of the two substances differ.'
                 # }
 
         """  # noqa: E501
-        llm = self.bind_tools([schema], tool_choice="any")
+        llm = self.bind_tools([schema])
         if isinstance(schema, type) and issubclass(schema, BaseModel):
             output_parser = ToolsOutputParser(
                 first_tool_only=True, pydantic_schemas=[schema]
             )
         else:
             output_parser = ToolsOutputParser(first_tool_only=True, args_only=True)
 
@@ -821,33 +673,10 @@
 
 def _tools_in_params(params: dict) -> bool:
     return "tools" in params or (
         "extra_body" in params and params["extra_body"].get("tools")
     )
 
 
-class _AnthropicToolUse(TypedDict):
-    type: Literal["tool_use"]
-    name: str
-    input: dict
-    id: str
-
-
-def _lc_tool_calls_to_anthropic_tool_use_blocks(
-    tool_calls: List[ToolCall],
-) -> List[_AnthropicToolUse]:
-    blocks = []
-    for tool_call in tool_calls:
-        blocks.append(
-            _AnthropicToolUse(
-                type="tool_use",
-                name=tool_call["name"],
-                input=tool_call["args"],
-                id=cast(str, tool_call["id"]),
-            )
-        )
-    return blocks
-
-
-@deprecated(since="0.1.0", removal="0.3.0", alternative="ChatAnthropic")
+@deprecated(since="0.1.0", removal="0.2.0", alternative="ChatAnthropic")
 class ChatAnthropicMessages(ChatAnthropic):
     pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gigachain_anthropic-0.1.13/langchain_anthropic/experimental.py` & `gigachain_anthropic-0.1.8/langchain_anthropic/experimental.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     invokes = elem.findall("invoke")
 
     return [_xml_to_function_call(invoke, tools) for invoke in invokes]
 
 
 @deprecated(
     "0.1.5",
-    removal="0.3.0",
+    removal="0.2.0",
     alternative="ChatAnthropic",
     message=(
         "Tool-calling is now officially supported by the Anthropic API so this "
         "workaround is no longer needed."
     ),
 )
 class ChatAnthropicTools(ChatAnthropic):
```

### Comparing `gigachain_anthropic-0.1.13/langchain_anthropic/llms.py` & `gigachain_anthropic-0.1.8/langchain_anthropic/llms.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,37 +169,14 @@
         return values
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "anthropic-llm"
 
-    @property
-    def lc_secrets(self) -> Dict[str, str]:
-        return {"anthropic_api_key": "ANTHROPIC_API_KEY"}
-
-    @classmethod
-    def is_lc_serializable(cls) -> bool:
-        return True
-
-    @property
-    def _identifying_params(self) -> Dict[str, Any]:
-        """Get the identifying parameters."""
-        return {
-            "model": self.model,
-            "max_tokens": self.max_tokens_to_sample,
-            "temperature": self.temperature,
-            "top_k": self.top_k,
-            "top_p": self.top_p,
-            "model_kwargs": self.model_kwargs,
-            "streaming": self.streaming,
-            "default_request_timeout": self.default_request_timeout,
-            "max_retries": self.max_retries,
-        }
-
     def _wrap_prompt(self, prompt: str) -> str:
         if not self.HUMAN_PROMPT or not self.AI_PROMPT:
             raise NameError("Please ensure the anthropic package is loaded")
 
         if prompt.startswith(self.HUMAN_PROMPT):
             return prompt  # Already wrapped.
 
@@ -228,15 +205,15 @@
             The string generated by the model.
 
         Example:
             .. code-block:: python
 
                 prompt = "What are the biggest risks facing humanity?"
                 prompt = f"\n\nHuman: {prompt}\n\nAssistant:"
-                response = model.invoke(prompt)
+                response = model(prompt)
 
         """
         if self.streaming:
             completion = ""
             for chunk in self._stream(
                 prompt=prompt, stop=stop, run_manager=run_manager, **kwargs
             ):
@@ -356,10 +333,10 @@
     def get_num_tokens(self, text: str) -> int:
         """Calculate number of tokens."""
         if not self.count_tokens:
             raise NameError("Please ensure the anthropic package is loaded")
         return self.count_tokens(text)
 
 
-@deprecated(since="0.1.0", removal="0.3.0", alternative="AnthropicLLM")
+@deprecated(since="0.1.0", removal="0.2.0", alternative="AnthropicLLM")
 class Anthropic(AnthropicLLM):
     pass
```

### Comparing `gigachain_anthropic-0.1.13/langchain_anthropic/output_parsers.py` & `gigachain_anthropic-0.1.8/langchain_anthropic/output_parsers.py`

 * *Files identical despite different names*

### Comparing `gigachain_anthropic-0.1.13/pyproject.toml` & `gigachain_anthropic-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 
 [tool.poetry]
 name = "gigachain-anthropic"
-version = "0.1.13"
+version = "0.1.8"
 description = "An integration package connecting AnthropicMessages and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/gigachain-ai/gigachain"
 license = "MIT"
 packages = [
     {include = "langchain_anthropic"}
 ]
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/gigachain-ai/gigachain/tree/master/libs/partners/anthropic"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-gigachain-core = ">=0.1.43,<0.3"
-anthropic = ">=0.26.0,<1"
+gigachain-core = "^0.1.42"
+anthropic = ">=0.23.0,<1"
 defusedxml = { version = "^0.7.1", optional = true }
 
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
 defusedxml = "^0.7.1"
-gigachain-standard-tests = { path = "../../standard-tests", develop = true }
+gigachain-standard-tests = {path = "../../standard-tests", develop = true}
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
```

### Comparing `gigachain_anthropic-0.1.13/PKG-INFO` & `gigachain_anthropic-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: gigachain-anthropic
-Version: 0.1.13
+Version: 0.1.8
 Summary: An integration package connecting AnthropicMessages and LangChain
 Home-page: https://github.com/gigachain-ai/gigachain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: anthropic (>=0.26.0,<1)
+Requires-Dist: anthropic (>=0.23.0,<1)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: gigachain-core (>=0.1.43,<0.3)
+Requires-Dist: gigachain-core (>=0.1.42,<0.2.0)
 Project-URL: Repository, https://github.com/gigachain-ai/gigachain
 Project-URL: Source Code, https://github.com/gigachain-ai/gigachain/tree/master/libs/partners/anthropic
 Description-Content-Type: text/markdown
 
 # langchain-anthropic
 
 This package contains the LangChain integration for Anthropic's generative models.
```

