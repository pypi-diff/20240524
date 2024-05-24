# Comparing `tmp/mistral_common-1.0.2.tar.gz` & `tmp/mistral_common-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistral_common-1.0.2.tar", max compression
+gzip compressed data, was "mistral_common-1.1.0.tar", max compression
```

## Comparing `mistral_common-1.0.2.tar` & `mistral_common-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11339 2024-04-17 14:26:20.275663 mistral_common-1.0.2/LICENCE
--rw-r--r--   0        0        0     2949 2024-04-17 14:18:35.356766 mistral_common-1.0.2/README.md
--rw-r--r--   0        0        0     1288 2024-04-17 14:26:42.134667 mistral_common-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 12:28:15.315166 mistral_common-1.0.2/src/mistral_common/__init__.py
--rw-r--r--   0        0        0      244 2024-04-17 12:28:15.512167 mistral_common-1.0.2/src/mistral_common/base.py
--rw-r--r--   0        0        0   587404 2024-04-17 12:28:15.524166 mistral_common-1.0.2/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2
--rw-r--r--   0        0        0   587404 2024-04-17 12:28:15.529175 mistral_common-1.0.2/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3
--rw-r--r--   0        0        0   493443 2024-04-17 12:28:15.536165 mistral_common-1.0.2/src/mistral_common/data/tokenizer.model.v1
--rw-r--r--   0        0        0     1807 2024-04-17 12:28:15.516164 mistral_common-1.0.2/src/mistral_common/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-17 12:28:15.328168 mistral_common-1.0.2/src/mistral_common/protocol/__init__.py
--rw-r--r--   0        0        0      199 2024-04-17 12:28:15.333167 mistral_common-1.0.2/src/mistral_common/protocol/base.py
--rw-r--r--   0        0        0      400 2024-04-17 12:28:15.339167 mistral_common-1.0.2/src/mistral_common/protocol/embedding/request.py
--rw-r--r--   0        0        0      873 2024-04-17 12:28:15.344167 mistral_common-1.0.2/src/mistral_common/protocol/embedding/response.py
--rw-r--r--   0        0        0        0 2024-04-17 12:28:15.375166 mistral_common-1.0.2/src/mistral_common/protocol/instruct/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-17 12:28:15.380167 mistral_common-1.0.2/src/mistral_common/protocol/instruct/messages.py
--rw-r--r--   0        0        0      956 2024-04-17 12:28:15.397171 mistral_common-1.0.2/src/mistral_common/protocol/instruct/request.py
--rw-r--r--   0        0        0     1918 2024-04-17 12:28:15.384183 mistral_common-1.0.2/src/mistral_common/protocol/instruct/response.py
--rw-r--r--   0        0        0      658 2024-04-17 12:28:15.388166 mistral_common-1.0.2/src/mistral_common/protocol/instruct/tool_calls.py
--rw-r--r--   0        0        0    10534 2024-04-17 12:28:15.393166 mistral_common-1.0.2/src/mistral_common/protocol/instruct/validator.py
--rw-r--r--   0        0        0       73 2024-04-17 12:28:15.403166 mistral_common-1.0.2/src/mistral_common/protocol/utils.py
--rw-r--r--   0        0        0        0 2024-04-17 12:28:15.408165 mistral_common-1.0.2/src/mistral_common/py.typed
--rw-r--r--   0        0        0        0 2024-04-17 12:28:15.421165 mistral_common-1.0.2/src/mistral_common/tokens/__init__.py
--rw-r--r--   0        0        0     6119 2024-04-17 12:28:15.443166 mistral_common-1.0.2/src/mistral_common/tokens/instruct/normalize.py
--rw-r--r--   0        0        0      418 2024-04-17 12:28:15.448166 mistral_common-1.0.2/src/mistral_common/tokens/instruct/request.py
--rw-r--r--   0        0        0     1481 2024-04-17 12:28:15.481165 mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/base.py
--rw-r--r--   0        0        0     4660 2024-04-17 14:19:11.465776 mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/mistral.py
--rw-r--r--   0        0        0    12394 2024-04-17 12:28:15.490165 mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/sentencepiece.py
--rw-r--r--   0        0        0      187 2024-04-17 12:28:15.476165 mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/utils.py
--rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 mistral_common-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-05-24 08:24:49.429905 mistral_common-1.1.0/LICENCE
+-rw-r--r--   0        0        0     2971 2024-05-24 09:56:33.893366 mistral_common-1.1.0/README.md
+-rw-r--r--   0        0        0     1289 2024-05-24 09:56:33.933324 mistral_common-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 08:23:05.965233 mistral_common-1.1.0/src/mistral_common/__init__.py
+-rw-r--r--   0        0        0      261 2024-05-24 09:56:33.942009 mistral_common-1.1.0/src/mistral_common/base.py
+-rw-r--r--   0        0        0   587404 2024-05-24 08:23:06.338148 mistral_common-1.1.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2
+-rw-r--r--   0        0        0   587404 2024-05-24 08:23:05.997657 mistral_common-1.1.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3
+-rw-r--r--   0        0        0   493443 2024-05-24 08:23:06.013826 mistral_common-1.1.0/src/mistral_common/data/tokenizer.model.v1
+-rw-r--r--   0        0        0     1807 2024-05-24 08:23:04.706356 mistral_common-1.1.0/src/mistral_common/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:23:04.729841 mistral_common-1.1.0/src/mistral_common/protocol/__init__.py
+-rw-r--r--   0        0        0      199 2024-05-24 08:23:04.721302 mistral_common-1.1.0/src/mistral_common/protocol/base.py
+-rw-r--r--   0        0        0      400 2024-05-24 08:23:04.850885 mistral_common-1.1.0/src/mistral_common/protocol/embedding/request.py
+-rw-r--r--   0        0        0      873 2024-05-24 08:23:04.833933 mistral_common-1.1.0/src/mistral_common/protocol/embedding/response.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:23:05.198296 mistral_common-1.1.0/src/mistral_common/protocol/instruct/__init__.py
+-rw-r--r--   0        0        0     2173 2024-05-24 09:56:33.952798 mistral_common-1.1.0/src/mistral_common/protocol/instruct/messages.py
+-rw-r--r--   0        0        0     7506 2024-05-24 09:56:33.959793 mistral_common-1.1.0/src/mistral_common/protocol/instruct/normalize.py
+-rw-r--r--   0        0        0      986 2024-05-24 09:56:33.980403 mistral_common-1.1.0/src/mistral_common/protocol/instruct/request.py
+-rw-r--r--   0        0        0     1918 2024-05-24 08:23:05.423807 mistral_common-1.1.0/src/mistral_common/protocol/instruct/response.py
+-rw-r--r--   0        0        0     1043 2024-05-24 09:56:33.987559 mistral_common-1.1.0/src/mistral_common/protocol/instruct/tool_calls.py
+-rw-r--r--   0        0        0    12976 2024-05-24 09:56:33.998965 mistral_common-1.1.0/src/mistral_common/protocol/instruct/validator.py
+-rw-r--r--   0        0        0       73 2024-05-24 08:23:05.959141 mistral_common-1.1.0/src/mistral_common/protocol/utils.py
+-rw-r--r--   0        0        0        0 2024-05-24 08:23:06.580639 mistral_common-1.1.0/src/mistral_common/py.typed
+-rw-r--r--   0        0        0        0 2024-05-24 08:23:06.561184 mistral_common-1.1.0/src/mistral_common/tokens/__init__.py
+-rw-r--r--   0        0        0      479 2024-05-24 09:56:34.014187 mistral_common-1.1.0/src/mistral_common/tokens/instruct/request.py
+-rw-r--r--   0        0        0     2134 2024-05-24 09:56:34.021362 mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/base.py
+-rw-r--r--   0        0        0     5367 2024-05-24 09:56:34.029681 mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/mistral.py
+-rw-r--r--   0        0        0    12947 2024-05-24 09:56:34.037770 mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/sentencepiece.py
+-rw-r--r--   0        0        0      187 2024-05-24 08:23:06.552824 mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/utils.py
+-rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 mistral_common-1.1.0/PKG-INFO
```

### Comparing `mistral_common-1.0.2/LICENCE` & `mistral_common-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.2/README.md` & `mistral_common-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,22 @@
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 
 
 ```py
 # Import needed packages:
-from mistral_common.protocol.instruct.messages import UserMessage
+from mistral_common.protocol.instruct.messages import (
+    UserMessage,
+)
 from mistral_common.protocol.instruct.request import ChatCompletionRequest
-from mistral_common.protocol.instruct.tool_calls import Function, Tool
+from mistral_common.protocol.instruct.tool_calls import (
+    Function,
+    Tool,
+)
 from mistral_common.tokens.tokenizers.mistral import MistralTokenizer
 
 # Load Mistral tokenizer
 
 model_name = "open-mixtral-8x22b"
 
 tokenizer = MistralTokenizer.from_model(model_name)
```

### Comparing `mistral_common-1.0.2/pyproject.toml` & `mistral_common-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mistral_common"
-version = "v1.0.2"
+version = "v1.1.0"
 description = ""
 authors = ["bam4d <bam4d@mistral.ai>"]
 readme = "README.md"
 packages = [{ include = "mistral_common", from = "src" }]
 
 [tool.ruff]
 lint.select = ["E", "F", "W", "Q", "I"]
@@ -51,8 +51,8 @@
 [tool.pytest.ini_options]
 testpaths = ["./tests"]
 
 [tool.coverage.run]
 omit = ["tests", "*src/mistral_common/data*"]
 
 [tool.coverage.report]
-skip_covered = true
+skip_covered = true
```

### Comparing `mistral_common-1.0.2/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2` & `mistral_common-1.1.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.2/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3` & `mistral_common-1.1.0/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.2/src/mistral_common/data/tokenizer.model.v1` & `mistral_common-1.1.0/src/mistral_common/data/tokenizer.model.v1`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.2/src/mistral_common/exceptions.py` & `mistral_common-1.1.0/src/mistral_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.2/src/mistral_common/protocol/embedding/response.py` & `mistral_common-1.1.0/src/mistral_common/protocol/embedding/response.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.2/src/mistral_common/protocol/instruct/request.py` & `mistral_common-1.1.0/src/mistral_common/protocol/instruct/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from enum import Enum
-from typing import List, Optional
+from typing import Generic, List, Optional
 
 from pydantic import Field
 
 from mistral_common.base import MistralBase
-from mistral_common.protocol.instruct.messages import ChatMessage
+from mistral_common.protocol.instruct.messages import ChatMessageType
 from mistral_common.protocol.instruct.tool_calls import Tool, ToolChoice
 
 
 class ResponseFormats(str, Enum):
     text: str = "text"
     json: str = "json_object"
 
 
 class ResponseFormat(MistralBase):
     type: ResponseFormats = ResponseFormats.text
 
 
-class ChatCompletionRequest(MistralBase):
+class ChatCompletionRequest(MistralBase, Generic[ChatMessageType]):
     model: Optional[str] = None
-    messages: List[ChatMessage]
+    messages: List[ChatMessageType]
     response_format: ResponseFormat = Field(default_factory=ResponseFormat)
-    tools: List[Tool] = Field(default_factory=list)
+    tools: Optional[List[Tool]] = None
     tool_choice: ToolChoice = ToolChoice.auto
     temperature: float = Field(default=0.7, ge=0.0, le=1.0)
     top_p: float = Field(default=1.0, ge=0.0, le=1.0)
     max_tokens: Optional[int] = Field(default=None, ge=0)
     random_seed: Optional[int] = Field(default=None, ge=0)
```

### Comparing `mistral_common-1.0.2/src/mistral_common/protocol/instruct/response.py` & `mistral_common-1.1.0/src/mistral_common/protocol/instruct/response.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.2/src/mistral_common/protocol/instruct/validator.py` & `mistral_common-1.1.0/src/mistral_common/protocol/instruct/validator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 import re
 from enum import Enum
-from typing import List
+from typing import Generic, List
 
 from jsonschema import Draft7Validator, SchemaError
 
 from mistral_common.exceptions import (
     InvalidAssistantMessageException,
     InvalidFunctionCallException,
     InvalidMessageStructureException,
     InvalidRequestException,
     InvalidSystemPromptException,
     InvalidToolException,
     InvalidToolMessageException,
     InvalidToolSchemaException,
 )
 from mistral_common.protocol.instruct.messages import (
-    AssistantMessage,
-    ChatMessage,
+    UATS,
+    AssistantMessageType,
+    FinetuningAssistantMessage,
     Roles,
-    SystemMessage,
-    ToolMessage,
-    UserMessage,
+    SystemMessageType,
+    ToolMessageType,
+    UserMessageType,
 )
 from mistral_common.protocol.instruct.request import ChatCompletionRequest
 from mistral_common.protocol.instruct.tool_calls import (
     Function,
     FunctionCall,
     Tool,
     ToolCall,
 )
 
 
 class ValidationMode(Enum):
     serving = "serving"
+    finetuning = "finetuning"
     test = "test"
 
 
-class MistralRequestValidator:
+class MistralRequestValidator(Generic[UserMessageType, AssistantMessageType, ToolMessageType, SystemMessageType]):
     def __init__(self, mode: ValidationMode = ValidationMode.test):
         self._mode = mode
 
-    def validate_messages(self, messages: List[ChatMessage]) -> None:
+    def validate_messages(self, messages: List[UATS]) -> None:
         """
         Validates the list of messages
         """
         self._validate_message_list_structure(messages)
         self._validate_message_list_content(messages)
 
-    def validate_request(self, request: ChatCompletionRequest) -> ChatCompletionRequest:
+    def validate_request(self, request: ChatCompletionRequest) -> ChatCompletionRequest[UATS]:
         """
         Validates the request
         """
 
         if self._mode == ValidationMode.serving:
             if request.model is None:
                 raise InvalidRequestException("Model name parameter is required for serving mode")
 
         # Validate the messages
         self.validate_messages(request.messages)
 
         # Validate the tools
-        self._validate_tools(request.tools)
+        self._validate_tools(request.tools or [])
 
         return request
 
     def _validate_function(self, function: Function) -> None:
         """
         Checks:
         - That the function schema is valid
@@ -85,30 +87,30 @@
         Checks:
         - That the tool schemas are valid
         """
 
         for tool in tools:
             self._validate_function(tool.function)
 
-    def _validate_user_message(self, message: UserMessage) -> None:
+    def _validate_user_message(self, message: UserMessageType) -> None:
         pass
 
-    def _validate_tool_message(self, message: ToolMessage) -> None:
+    def _validate_tool_message(self, message: ToolMessageType) -> None:
         """
         Checks:
         - The tool name is valid
         """
         if message.name is not None:
             if not re.match(r"^[a-zA-Z0-9_-]{1,64}$", message.name):
                 raise InvalidToolMessageException(
                     f"Function name was {message.name} but must be a-z, A-Z, 0-9, "
                     "or contain underscores and dashes, with a maximum length of 64."
                 )
 
-    def _validate_system_message(self, message: SystemMessage) -> None:
+    def _validate_system_message(self, message: SystemMessageType) -> None:
         """
         Checks:
         - That the system prompt has content
         """
         if message.content is None:
             raise InvalidSystemPromptException("System prompt must have content")
 
@@ -119,40 +121,47 @@
         """
         if not re.match(r"^[a-zA-Z0-9_-]{1,64}$", function_call.name):
             raise InvalidFunctionCallException(
                 f"Function name was {function_call.name} but must be a-z, A-Z, 0-9, "
                 "or contain underscores and dashes, with a maximum length of 64."
             )
 
-    def _validate_tool_call(self, tool_call: ToolCall) -> None:
+    def _validate_tool_call(self, tool_call: ToolCall, is_last_message: bool) -> None:
         """
         Checks:
         - That the tool call has a valid function
         """
 
         self._validate_function_call(tool_call.function)
 
-    def _validate_assistant_message(self, message: AssistantMessage) -> None:
+    def _validate_assistant_message(self, message: AssistantMessageType, is_last_message: bool = False) -> None:
         """
         Checks:
         - That the assistant message has either text or tool_calls, but not both
         - That the tool calls are valid
         """
 
-        # Validate that the message has either text or tool_calls, but not both
-        if (message.content is None) == (message.tool_calls is None):
-            raise InvalidAssistantMessageException("Assistant message must have either content or tool_calls")
+        # Validate that the message has either text or tool_calls
+        # but not both and not neither.
+        if bool(message.content) == bool(message.tool_calls):
+            raise InvalidAssistantMessageException(
+                "Assistant message must have either content or tool_calls, but not both."
+            )
 
         # If we have tool calls, validate them
         if message.tool_calls is not None:
             # Validate that the tool calls are valid
             for tool_call in message.tool_calls:
-                self._validate_tool_call(tool_call)
+                self._validate_tool_call(tool_call, is_last_message=is_last_message)
+
+        if self._mode == ValidationMode.finetuning and isinstance(message, FinetuningAssistantMessage):
+            if message.weight is not None and message.weight not in [0, 1]:
+                raise InvalidAssistantMessageException("Assistant message weight must be either 0 or 1")
 
-    def _validate_tool_calls_followed_by_tool_messages(self, messages: List[ChatMessage]) -> None:
+    def _validate_tool_calls_followed_by_tool_messages(self, messages: List[UATS]) -> None:
         """
         Checks:
         - That the number of tool calls and tool messages are the same
         - That the tool calls are followed by tool messages
         """
         prev_role = None
         expected_tool_messages = 0
@@ -171,112 +180,142 @@
 
                 if message.tool_calls is not None:
                     # Validate that the number of function calls and responses are the same
                     expected_tool_messages = len(message.tool_calls)
 
             prev_role = message.role
 
-        if expected_tool_messages != 0:
+        if expected_tool_messages != 0 and self._mode == ValidationMode.serving:
             raise InvalidMessageStructureException("Not the same number of function calls and responses")
+        elif expected_tool_messages not in [0, 1] and self._mode == ValidationMode.finetuning:
+            # if last assistant message has no tool calls, then same number of tool calls and messages => 0
+            # if last assistant message has a tool call we have one more tool call => 1
+            raise InvalidMessageStructureException("Too many function calls and too few responses")
 
-    def _validate_message_order(self, messages: List[ChatMessage]) -> None:
+    def _validate_message_order(self, messages: List[UATS]) -> None:
         """
         Validates the order of the messages, for example user -> assistant -> user -> assistant -> ...
         """
         previous_role = None
         for message in messages:
             current_role = message.role
 
             if previous_role is not None:
                 if previous_role == Roles.system:
                     expected_roles = {Roles.user, Roles.assistant, Roles.system}
                 elif previous_role == Roles.user:
                     expected_roles = {Roles.assistant, Roles.system, Roles.user}
                 elif previous_role == Roles.assistant:
-                    expected_roles = {Roles.user, Roles.tool}
+                    expected_roles = {Roles.assistant, Roles.user, Roles.tool}
                 elif previous_role == Roles.tool:
                     expected_roles = {Roles.assistant, Roles.tool}
 
                 if current_role not in expected_roles:
                     raise InvalidMessageStructureException(
                         f"Unexpected role '{current_role.value}' after role '{previous_role.value}'"
                     )
 
             previous_role = current_role
 
-    def _validate_message_list_structure(self, messages: List[ChatMessage]) -> None:
+    def _validate_last_message(self, message: UATS) -> None:
+        # The last message must be a user or tool message in serving mode or an assistant message in finetuning mode
+        last_message_role = message.role
+        expected_roles = (
+            {Roles.user, Roles.tool}
+            if self._mode != ValidationMode.finetuning
+            else {Roles.assistant}
+        )
+
+        if last_message_role not in expected_roles:
+            expected_roles_str = ", ".join(role.value for role in expected_roles)
+            raise InvalidMessageStructureException(
+                f"Expected last role to be one of: [{expected_roles_str}] but got {last_message_role.value}"
+            )
+
+    def _validate_message_list_structure(self, messages: List[UATS]) -> None:
         """
         Validates the structure of the list of messages
 
         For example the messages must be in the correct order of user/assistant/tool
         """
 
         if len(messages) == 0:
             raise InvalidMessageStructureException("Conversation must have at least one message")
 
         # If we have one message it must be a user or a system message
         if len(messages) == 1:
             if messages[0].role not in {Roles.user, Roles.system}:
                 raise InvalidMessageStructureException("Conversation must start with a user message or system message")
-
         else:
-            # The last message must be a user or tool message
-            last_message_role = messages[-1].role
-            expected_roles = {Roles.user, Roles.tool}
-
-            if last_message_role not in expected_roles:
-                expected_roles_str = ", ".join(role.value for role in expected_roles)
-                raise InvalidMessageStructureException(
-                    f"Expected last role to be one of: [{expected_roles_str}] but got {last_message_role.value}"
-                )
+            self._validate_last_message(messages[-1])
 
         self._validate_message_order(messages)
         self._validate_tool_calls_followed_by_tool_messages(messages)
 
-    def _validate_message_list_content(self, messages: List[ChatMessage]) -> None:
+    def _validate_message_list_content(self, messages: List[UATS]) -> None:
         """
         Validates the content of the messages
         """
 
-        for message in messages:
+        for idx, message in enumerate(messages):
             if message.role == Roles.user:
                 self._validate_user_message(message)
             elif message.role == Roles.assistant:
-                self._validate_assistant_message(message)
+                self._validate_assistant_message(message, is_last_message=idx == len(messages) - 1)
             elif message.role == Roles.tool:
                 self._validate_tool_message(message)
             elif message.role == Roles.system:
                 self._validate_system_message(message)
             else:
                 raise InvalidRequestException(f"Unsupported message type {type(message)}")
 
 
 class MistralRequestValidatorV3(MistralRequestValidator):
-    def _validate_tool_message(self, message: ToolMessage) -> None:
+    def _validate_tool_message(self, message: ToolMessageType) -> None:
         """
         Checks:
         - The tool name is valid
+        - Tool call id is valid
         """
         if message.name is not None:
             if not re.match(r"^[a-zA-Z0-9_-]{1,64}$", message.name):
                 raise InvalidToolMessageException(
                     f"Function name was {message.name} but must be a-z, A-Z, 0-9, "
                     "or contain underscores and dashes, with a maximum length of 64."
                 )
 
-        if message.tool_call_id is not None:
-            if not re.match(r"^[a-zA-Z0-9]{9}$", message.tool_call_id):
-                raise InvalidToolMessageException(
-                    f"Tool call id was {message.tool_call_id} but must be a-z, A-Z, 0-9, with a length of 9."
-                )
+        if message.tool_call_id is None:
+            raise InvalidRequestException("Tool call id has to be defined.")
 
-    def _validate_tool_call(self, tool_call: ToolCall) -> None:
+        if not re.match(r"^[a-zA-Z0-9]{9}$", message.tool_call_id):
+            raise InvalidToolMessageException(
+                f"Tool call id was {message.tool_call_id} but must be a-z, A-Z, 0-9, with a length of 9."
+            )
+
+
+    def _validate_tool_call(self, tool_call: ToolCall, is_last_message: bool) -> None:
         """
         Validate that the tool call has a valid ID
         """
+        if tool_call.id != "null":
+            if not re.match(r"^[a-zA-Z0-9]{9}$", tool_call.id):
+                raise InvalidFunctionCallException(
+                    f"Tool call id was {tool_call.id} but must be a-z, A-Z, 0-9, with a length of 9."
+                )
+        if self._mode == ValidationMode.finetuning and not is_last_message and tool_call.id == "null":
+            err_message = "Tool call id of assistant message that is not last has to be defined in finetuning mode."
+            raise InvalidFunctionCallException(err_message)
 
-        if not re.match(r"^[a-zA-Z0-9]{9}$", tool_call.id):
-            raise InvalidFunctionCallException(
-                f"Tool call id was {tool_call.id} but must be a-z, A-Z, 0-9, with a length of 9."
-            )
+        if self._mode == ValidationMode.serving and tool_call.id == "null":
+            raise InvalidFunctionCallException("Tool call id has to be defined in serving mode.")
 
         self._validate_function_call(tool_call.function)
+
+    def _validate_last_message(self, message: UATS) -> None:
+        super()._validate_last_message(message)
+
+        if self._mode == ValidationMode.finetuning:
+            # in finetuning mode it has to be an assistant message
+            # as checked by parent `_validate_last_message`
+            if message.tool_calls is not None:
+                for tool_call in message.tool_calls:
+                    self._validate_tool_call(tool_call, is_last_message=True)
```

### Comparing `mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/base.py` & `mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import List, Optional, Protocol
+from typing import Generic, List, Optional, TypeVar
 
 from mistral_common.base import MistralBase
 from mistral_common.tokens.instruct.request import InstructRequest
 
 
 class SpecialTokens(str, Enum):
     bos = "<s>"
@@ -51,11 +51,33 @@
     def encode(self, s: str, bos: bool, eos: bool) -> List[int]:
         """String to token ids"""
 
     @abstractmethod
     def decode(self, t: List[int]) -> str:
         """Token ids to string"""
 
+    @abstractmethod
+    def get_control_token(self, s: str) -> int:
+        """Get the id of a control token"""
+
+    @abstractmethod
+    def to_string(self, tokens: List[int]) -> str:
+        """Convert token ids to string"""
+
+
+InstructRequestType = TypeVar("InstructRequestType", bound=InstructRequest)
+TokenizedType = TypeVar("TokenizedType", bound=Tokenized)
+
 
-class InstructTokenizer(Protocol):
-    def encode_instruct(self, request: InstructRequest) -> Tokenized:
+class InstructTokenizer(Generic[InstructRequestType, TokenizedType], ABC):
+    tokenizer: Tokenizer
+
+    def __init__(self, model_path: str):
+        """Init from model file"""
+
+    @abstractmethod
+    def encode_instruct(self, request: InstructRequestType) -> TokenizedType:
         """Instruct request to Tokenized object"""
+
+    @abstractmethod
+    def decode(self, tokens: List[int]) -> str:
+        """Convert token ids to string"""
```

### Comparing `mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/mistral.py` & `mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/mistral.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,87 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Type
+from typing import Callable, Dict, Generic, List
 
 from mistral_common.exceptions import (
     TokenizerException,
 )
+from mistral_common.protocol.instruct.messages import (
+    UATS,
+    AssistantMessageType,
+    SystemMessageType,
+    ToolMessageType,
+    UserMessageType,
+)
+from mistral_common.protocol.instruct.normalize import InstructRequestNormalizer
 from mistral_common.protocol.instruct.request import ChatCompletionRequest
 from mistral_common.protocol.instruct.validator import (
     MistralRequestValidator,
     MistralRequestValidatorV3,
     ValidationMode,
 )
-from mistral_common.tokens.instruct.normalize import InstructRequestNormalizer
-from mistral_common.tokens.tokenizers.base import InstructTokenizer, Tokenized
+from mistral_common.tokens.tokenizers.base import (
+    InstructRequest,
+    InstructRequestType,
+    InstructTokenizer,
+    Tokenized,
+    TokenizedType,
+)
 from mistral_common.tokens.tokenizers.sentencepiece import (
-    SentencePieceInstructTokenizerV1,
-    SentencePieceInstructTokenizerV2,
-    SentencePieceInstructTokenizerV3,
+    InstructTokenizerV1,
+    InstructTokenizerV2,
+    InstructTokenizerV3,
+    SentencePieceTokenizer,
 )
 
 
-class MistralTokenizer:
+class MistralTokenizer(
+    Generic[
+        UserMessageType, AssistantMessageType, ToolMessageType, SystemMessageType, TokenizedType
+    ]
+):
     def __init__(
         self,
-        instruct_tokenizer: InstructTokenizer,
-        validator: Type[MistralRequestValidator] = MistralRequestValidator,
-        request_normalizer: Type[InstructRequestNormalizer] = InstructRequestNormalizer,
-        mode: ValidationMode = ValidationMode.test,
+        instruct_tokenizer: InstructTokenizer[InstructRequest, TokenizedType],
+        validator: MistralRequestValidator[UserMessageType, AssistantMessageType, ToolMessageType, SystemMessageType],
+        request_normalizer: InstructRequestNormalizer[
+            UserMessageType, AssistantMessageType, ToolMessageType, SystemMessageType, InstructRequestType
+        ],
     ):
-        self._chat_completion_request_validator = validator(mode)
-        self._instruct_request_normalizer = request_normalizer()
+        self._chat_completion_request_validator = validator
+        self._instruct_request_normalizer = request_normalizer
         self.instruct_tokenizer = instruct_tokenizer
 
-
     @classmethod
     def _data_path(cls) -> Path:
         return Path(__file__).parents[2] / "data"
 
     @classmethod
     def v1(cls) -> MistralTokenizer:
-        """open-mistral-7B // open-mixtral-8x7B // mistral-embed"""
+        """open-mistral-7b // open-mixtral-8x7b // mistral-embed"""
         return cls.from_file(str(cls._data_path() / "tokenizer.model.v1"), mode=ValidationMode.test)
 
     @classmethod
     def v2(cls) -> MistralTokenizer:
         """mistral-small // mistral-large"""
         return cls.from_file(
             str(cls._data_path() / "mistral_instruct_tokenizer_240216.model.v2"), mode=ValidationMode.test
         )
 
     @classmethod
     def v3(cls) -> MistralTokenizer:
-        """open-mixtral-8x22B"""
+        """open-mixtral-8x22b"""
         return cls.from_file(
             str(cls._data_path() / "mistral_instruct_tokenizer_240216.model.v3"), mode=ValidationMode.test
         )
 
     @classmethod
     def from_model(cls, model: str) -> MistralTokenizer:
-        model_name_to_tokenizer_cls = {
+        model_name_to_tokenizer_cls: Dict[str, Callable[[], MistralTokenizer]] = {
             "open-mistral-7b": MistralTokenizer.v1,
             "open-mixtral-8x7b": MistralTokenizer.v1,
             "mistral-embed": MistralTokenizer.v1,
             "mistral-small": MistralTokenizer.v2,
             "mistral-large": MistralTokenizer.v2,
             "open-mixtral-8x22b": MistralTokenizer.v3,
         }
@@ -76,42 +94,42 @@
         raise TokenizerException(f"Unrecognized model: {model}")
 
     @classmethod
     def from_file(cls, tokenizer_filename: str, mode: ValidationMode = ValidationMode.test) -> MistralTokenizer:
         """
         Depending on which model we are loading, tokenization and validation might be different. 💩
         """
+
         if tokenizer_filename.endswith(".model.v1"):
-            return cls(
-                SentencePieceInstructTokenizerV1(tokenizer_filename),
-                validator=MistralRequestValidator,
-                request_normalizer=InstructRequestNormalizer,
-                mode=mode,
+            return MistralTokenizer(
+                InstructTokenizerV1(SentencePieceTokenizer(tokenizer_filename)),
+                validator=MistralRequestValidator(mode=mode),
+                request_normalizer=InstructRequestNormalizer.normalizer(),
             )
         elif tokenizer_filename.endswith(".model.v2"):
-            return cls(
-                SentencePieceInstructTokenizerV2(tokenizer_filename),
-                validator=MistralRequestValidator,
-                request_normalizer=InstructRequestNormalizer,
-                mode=mode,
+            return MistralTokenizer(
+                InstructTokenizerV2(SentencePieceTokenizer(tokenizer_filename)),
+                validator=MistralRequestValidator(mode=mode),
+                request_normalizer=InstructRequestNormalizer.normalizer(),
             )
         elif tokenizer_filename.endswith(".model.v3"):
-            return cls(
-                SentencePieceInstructTokenizerV3(tokenizer_filename),
-                validator=MistralRequestValidatorV3,
-                request_normalizer=InstructRequestNormalizer,
-                mode=mode,
+            return MistralTokenizer(
+                InstructTokenizerV3(SentencePieceTokenizer(tokenizer_filename)),
+                validator=MistralRequestValidatorV3(mode=mode),
+                request_normalizer=InstructRequestNormalizer.normalizer(),
             )
         elif tokenizer_filename.endswith(".model"):
-            return cls(
-                SentencePieceInstructTokenizerV1(tokenizer_filename),
-                validator=MistralRequestValidator,
-                request_normalizer=InstructRequestNormalizer,
-                mode=mode,
+            return MistralTokenizer(
+                InstructTokenizerV1(SentencePieceTokenizer(tokenizer_filename)),
+                validator=MistralRequestValidator(mode=mode),
+                request_normalizer=InstructRequestNormalizer.normalizer(),
             )
         else:
             raise TokenizerException(f"Unrecognized tokenizer filename: {tokenizer_filename}")
 
-    def encode_chat_completion(self, request: ChatCompletionRequest) -> Tokenized:
+    def encode_chat_completion(self, request: ChatCompletionRequest[UATS]) -> Tokenized:
         validated_request = self._chat_completion_request_validator.validate_request(request)
         instruct_request = self._instruct_request_normalizer.from_chat_completion_request(validated_request)
         return self.instruct_tokenizer.encode_instruct(instruct_request)
+
+    def decode(self, tokens: List[int]) -> str:
+        return self.instruct_tokenizer.decode(tokens)
```

### Comparing `mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/sentencepiece.py` & `mistral_common-1.1.0/src/mistral_common/tokens/tokenizers/sentencepiece.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 import os
 from abc import abstractmethod
 from functools import cached_property
-from typing import Any, Dict, List, Optional, Set
+from typing import Any, Dict, List, Optional, Set, Tuple
 
 from mistral_common.exceptions import TokenizerException
 from mistral_common.protocol.instruct.messages import (
     AssistantMessage,
     ToolMessage,
     UserMessage,
 )
@@ -30,14 +30,17 @@
         self._model = SentencePieceProcessor(model_file=model_path)
 
         assert self._model.vocab_size() == self._model.get_piece_size()
         self._vocab = [self._model.id_to_piece(i) for i in range(self.n_words)]
 
         super().__init__()
 
+    def get_control_token(self, s: str) -> int:
+        return self._model.piece_to_id(s)  # type: ignore
+
     @property
     def n_words(self) -> int:
         return self._model.vocab_size()  # type: ignore
 
     def vocab(self) -> List[str]:
         return self._vocab
 
@@ -87,21 +90,33 @@
 
         if curr_tokens:
             text += "".join([self.id_to_piece(tok) for tok in curr_tokens])
 
         return text
 
 
-class SentencePieceInstructTokenizer(InstructTokenizer):
-    def __init__(self, model_path: str):
-        self.tokenizer = SentencePieceTokenizer(model_path)
+class InstructTokenizerBase(InstructTokenizer):
+    def __init__(self, tokenizer: Tokenizer):
+        self.tokenizer = tokenizer
 
     def start(self) -> List[int]:
         return [self.tokenizer.bos_id]
 
+    @staticmethod
+    def find_first_last_user(request: InstructRequest) -> Tuple[int, int]:
+        # find last user message
+        last_user_idx = -1
+        first_user_idx = -1
+        for i, msg in list(enumerate(request.messages)):
+            if isinstance(msg, UserMessage):
+                if first_user_idx == -1:
+                    first_user_idx = i
+                last_user_idx = i
+        return first_user_idx, last_user_idx
+
     @abstractmethod
     def encode_user_message(
         self,
         message: UserMessage,
         available_tools: Optional[List[Tool]],
         is_last: bool,
         is_first: bool,
@@ -117,21 +132,15 @@
     def encode_assistant_message(self, message: AssistantMessage, is_before_last_user_message: bool) -> List[int]:
         ...
 
     def encode_instruct(self, request: InstructRequest) -> Tokenized:
         # init at bos
         tokens = self.start()
         # find last user message
-        last_user_idx = -1
-        first_user_idx = -1
-        for i, msg in list(enumerate(request.messages)):
-            if isinstance(msg, UserMessage):
-                if first_user_idx == -1:
-                    first_user_idx = i
-                last_user_idx = i
+        first_user_idx, last_user_idx = self.find_first_last_user(request)
         for msg_idx, msg in enumerate(request.messages):
             if isinstance(msg, UserMessage):
                 new_tokens = self.encode_user_message(
                     msg,
                     request.available_tools,
                     msg_idx == last_user_idx,
                     msg_idx == first_user_idx,
@@ -142,16 +151,19 @@
             elif isinstance(msg, AssistantMessage):
                 new_tokens = self.encode_assistant_message(msg, msg_idx < last_user_idx)
 
             tokens.extend(new_tokens)
 
         return Tokenized(tokens=tokens, text=self.tokenizer.to_string(tokens))
 
+    def decode(self, tokens: List[int]) -> str:
+        return self.tokenizer.decode(tokens)
 
-class SentencePieceInstructTokenizerV1(SentencePieceInstructTokenizer):
+
+class InstructTokenizerV1(InstructTokenizerBase):
     def encode_user_message(
         self,
         message: UserMessage,
         available_tools: Optional[List[Tool]],
         is_last: bool,
         is_first: bool,
         system_prompt: Optional[str] = None,
@@ -180,28 +192,25 @@
         else:
             raise TokenizerException(f"{message.content} // {message.tool_calls}")
 
         curr_tokens.append(self.tokenizer.eos_id)
         return curr_tokens
 
 
-class SentencePieceInstructTokenizerV2(SentencePieceInstructTokenizer):
-    def __init__(self, model_path: str):
-        super().__init__(model_path)
-
-        self.BEGIN_INST = self.get_control_token(SpecialTokens.begin_inst.value)
-        self.END_INST = self.get_control_token(SpecialTokens.end_inst.value)
-        self.BEGIN_AVAILABLE_TOOLS = self.get_control_token(SpecialTokens.begin_tools.value)
-        self.END_AVAILABLE_TOOLS = self.get_control_token(SpecialTokens.end_tools.value)
-        self.BEGIN_TOOL_RESULTS = self.get_control_token(SpecialTokens.begin_tool_results.value)
-        self.END_TOOL_RESULTS = self.get_control_token(SpecialTokens.end_tool_results.value)
-        self.TOOL_CALLS = self.get_control_token(SpecialTokens.tool_calls.value)
-
-    def get_control_token(self, s: str) -> int:
-        return self.tokenizer._model.piece_to_id(s)  # type: ignore
+class InstructTokenizerV2(InstructTokenizerBase):
+    def __init__(self, tokenizer: Tokenizer):
+        super().__init__(tokenizer)
+
+        self.BEGIN_INST = self.tokenizer.get_control_token(SpecialTokens.begin_inst.value)
+        self.END_INST = self.tokenizer.get_control_token(SpecialTokens.end_inst.value)
+        self.BEGIN_AVAILABLE_TOOLS = self.tokenizer.get_control_token(SpecialTokens.begin_tools.value)
+        self.END_AVAILABLE_TOOLS = self.tokenizer.get_control_token(SpecialTokens.end_tools.value)
+        self.BEGIN_TOOL_RESULTS = self.tokenizer.get_control_token(SpecialTokens.begin_tool_results.value)
+        self.END_TOOL_RESULTS = self.tokenizer.get_control_token(SpecialTokens.end_tool_results.value)
+        self.TOOL_CALLS = self.tokenizer.get_control_token(SpecialTokens.tool_calls.value)
 
     def encode_user_message(
         self,
         message: UserMessage,
         available_tools: Optional[List[Tool]],
         is_last: bool,
         is_first: bool,
@@ -292,38 +301,44 @@
         else:
             raise TokenizerException(f"Invalid assistant message: {message.content}")
 
         curr_tokens.append(self.tokenizer.eos_id)
         return curr_tokens
 
 
-class SentencePieceInstructTokenizerV3(SentencePieceInstructTokenizerV2):
+class InstructTokenizerV3(InstructTokenizerV2):
     """
     The only difference with V3 tokenizer is that it encodes the tool messages differently
     """
 
     def _prepare_function_call(self, tool_call: ToolCall) -> Dict[str, Any]:
-        return {
+        function_call = {
             "name": tool_call.function.name,
             "arguments": self._parse_json_content(tool_call.function.arguments),
-            "id": tool_call.id,
         }
 
+        if tool_call.id and tool_call.id != "null":
+            function_call["id"] = tool_call.id
+
+        return function_call
+
     def _prepare_tool_result(self, tool_message: ToolMessage) -> Dict[str, Any]:
         assert tool_message.content is not None, "Tool message content cannot be None"
+        assert tool_message.tool_call_id is not None, "Tool message has to have the tool call id defined in v3"
+
         return {
-            "call_id": tool_message.tool_call_id,
             "content": self._parse_json_content(tool_message.content),
+            "call_id": tool_message.tool_call_id,
         }
 
     def encode_tool_message(self, message: ToolMessage, is_before_last_user_message: bool) -> List[int]:
         """
         Same as V2 but tools not wrapped in a list and history is tokenized also
         """
-        tool_result_str = json.dumps(self._prepare_tool_result(message))
+        tool_result_str = json.dumps(self._prepare_tool_result(message), ensure_ascii=False)
         curr_tokens = [
             self.BEGIN_TOOL_RESULTS,
             *self.tokenizer.encode(tool_result_str, bos=False, eos=False),
             self.END_TOOL_RESULTS,
         ]
         return curr_tokens
```

### Comparing `mistral_common-1.0.2/PKG-INFO` & `mistral_common-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistral_common
-Version: 1.0.2
+Version: 1.1.0
 Summary: 
 Author: bam4d
 Author-email: bam4d@mistral.ai
 Requires-Python: >=3.8.10,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -55,17 +55,22 @@
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 
 
 ```py
 # Import needed packages:
-from mistral_common.protocol.instruct.messages import UserMessage
+from mistral_common.protocol.instruct.messages import (
+    UserMessage,
+)
 from mistral_common.protocol.instruct.request import ChatCompletionRequest
-from mistral_common.protocol.instruct.tool_calls import Function, Tool
+from mistral_common.protocol.instruct.tool_calls import (
+    Function,
+    Tool,
+)
 from mistral_common.tokens.tokenizers.mistral import MistralTokenizer
 
 # Load Mistral tokenizer
 
 model_name = "open-mixtral-8x22b"
 
 tokenizer = MistralTokenizer.from_model(model_name)
```

