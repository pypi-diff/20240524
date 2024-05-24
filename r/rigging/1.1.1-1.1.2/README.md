# Comparing `tmp/rigging-1.1.1.tar.gz` & `tmp/rigging-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigging-1.1.1.tar", max compression
+gzip compressed data, was "rigging-1.1.2.tar", max compression
```

## Comparing `rigging-1.1.1.tar` & `rigging-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1066 2024-05-21 20:29:39.787529 rigging-1.1.1/LICENSE
--rw-r--r--   0        0        0     1477 2024-05-21 20:29:39.787529 rigging-1.1.1/README.md
--rw-r--r--   0        0        0     2609 2024-05-21 20:29:39.795529 rigging-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      879 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/__init__.py
--rw-r--r--   0        0        0    45447 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/chat.py
--rw-r--r--   0        0        0    29216 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/completion.py
--rw-r--r--   0        0        0     3116 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/data.py
--rw-r--r--   0        0        0     1787 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/error.py
--rw-r--r--   0        0        0      762 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/generator/__init__.py
--rw-r--r--   0        0        0    15211 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/generator/base.py
--rw-r--r--   0        0        0     6459 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/generator/litellm_.py
--rw-r--r--   0        0        0     7302 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/generator/transformers_.py
--rw-r--r--   0        0        0     5804 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/generator/vllm_.py
--rw-r--r--   0        0        0     1791 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/logging.py
--rw-r--r--   0        0        0    13711 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/message.py
--rw-r--r--   0        0        0    13511 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/model.py
--rw-r--r--   0        0        0     3748 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/parsing.py
--rw-r--r--   0        0        0     1090 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/prompt.py
--rw-r--r--   0        0        0        0 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/py.typed
--rw-r--r--   0        0        0    10466 2024-05-21 20:29:39.795529 rigging-1.1.1/rigging/tool.py
--rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 rigging-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-24 04:26:38.225791 rigging-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1477 2024-05-24 04:26:38.225791 rigging-1.1.2/README.md
+-rw-r--r--   0        0        0     3012 2024-05-24 04:26:38.229791 rigging-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      879 2024-05-24 04:26:38.229791 rigging-1.1.2/rigging/__init__.py
+-rw-r--r--   0        0        0    45371 2024-05-24 04:26:38.229791 rigging-1.1.2/rigging/chat.py
+-rw-r--r--   0        0        0    29155 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/completion.py
+-rw-r--r--   0        0        0     3491 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/data.py
+-rw-r--r--   0        0        0     1775 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/error.py
+-rw-r--r--   0        0        0      762 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/generator/__init__.py
+-rw-r--r--   0        0        0    15398 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/generator/base.py
+-rw-r--r--   0        0        0     6417 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/generator/litellm_.py
+-rw-r--r--   0        0        0     7306 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/generator/transformers_.py
+-rw-r--r--   0        0        0     5808 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/generator/vllm_.py
+-rw-r--r--   0        0        0     1852 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/logging.py
+-rw-r--r--   0        0        0    13758 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/message.py
+-rw-r--r--   0        0        0    13572 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/model.py
+-rw-r--r--   0        0        0     3829 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/parsing.py
+-rw-r--r--   0        0        0     1090 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/prompt.py
+-rw-r--r--   0        0        0        0 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/py.typed
+-rw-r--r--   0        0        0    10516 2024-05-24 04:26:38.233791 rigging-1.1.2/rigging/tool.py
+-rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 rigging-1.1.2/PKG-INFO
```

### Comparing `rigging-1.1.1/LICENSE` & `rigging-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rigging-1.1.1/README.md` & `rigging-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rigging-1.1.1/pyproject.toml` & `rigging-1.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 [tool.poetry]
 name = "rigging"
-version = "1.1.1"
+version = "1.1.2"
 description = "LLM Interaction Framework"
 authors = ["Nick Landers <monoxgas@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/dreadnode/rigging"
 readme = "README.md"
 packages = [
     {include = "rigging"}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-pydantic = "2.5.3"
-pydantic-xml = "2.7.0"
+python = "^3.9"
+pydantic = "2.6.1"
+pydantic-xml = "2.11.0"
 loguru = "^0.7.2"
 litellm = "1.35.21"
 pandas = "^2.2.2"
+eval-type-backport = "^0.2.0" # For 3.9 future annotations
 
 vllm = { version = "0.4.2", optional = true }
 transformers = { version = "^4.41.0", optional = true }
 accelerate = { version = "^0.30.1", optional = true }
 
+asyncssh = { version = "2.14.2", optional = true }
+types-requests = { version = "2.32.0.20240523", optional = true }
+
 [tool.poetry.extras]
-all = ["vllm", "transformers", "accelerate"]
+examples = ["asyncssh", "types-requests"]
+all = ["vllm", "transformers", "accelerate", "asyncssh", "types-requests"]
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.27.1"
 mypy = "^1.8.0"
 ruff = "^0.1.14"
 pytest = "^8.0.0"
-pandas = "^2.2.2"
 pandas-stubs = "^2.2.1.240316"
 coverage = "^7.5.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.6.0"
 mkdocs-material = {extras = ["imaging"], version = "^9.5.20"}
 mkdocstrings = "^0.25.0"
@@ -74,19 +78,22 @@
     "B",   # flake8-bugbear
     "UP",  # pyupgrade
     "NPY", # numpydoc
     "TCH", # typecheck
     "A",   # flake8-annotations
 ]
 ignore = [
-    "E501", # line too long, handled by black
-    "B008", # do not perform function calls in argument defaults
-    "C901", # too complex
-    "W191", # indentation contains tabs
-    "F722", # syntax error in forward annotation
+    "E501",  # line too long, handled by black
+    "B008",  # do not perform function calls in argument defaults
+    "C901",  # too complex
+    "W191",  # indentation contains tabs
+    "F722",  # syntax error in forward annotation
+    "UP007", # X | Y syntax while we're still supporting 3.9
+    "UP038", # isinstance() X | Y instance ^
+    "B905",  # zip() without strict (isn't supported in 3.9)
 ]
 
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
```

### Comparing `rigging-1.1.1/rigging/__init__.py` & `rigging-1.1.2/rigging/__init__.py`

 * *Files identical despite different names*

### Comparing `rigging-1.1.1/rigging/chat.py` & `rigging-1.1.2/rigging/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Chats are used pre and post generation to hold messages.
 
 They are the primary way to interact with the generator.
 """
 
+from __future__ import annotations
+
 import asyncio
 import typing as t
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 from typing import runtime_checkable
 from uuid import UUID, uuid4
@@ -40,17 +42,17 @@
     messages: list[Message]
     """The list of messages prior to generation."""
     generated: list[Message] = Field(default_factory=list)
     """The list of messages resulting from the generation."""
     metadata: dict[str, t.Any] = Field(default_factory=dict)
     """Additional metadata for the chat."""
 
-    generator: t.Optional["Generator"] = Field(None, exclude=True, repr=False)
+    generator: t.Optional[Generator] = Field(None, exclude=True, repr=False)
     """The generator associated with the chat."""
-    params: t.Optional["GenerateParams"] = Field(None, exclude=True, repr=False)
+    params: t.Optional[GenerateParams] = Field(None, exclude=True, repr=False)
     """Any additional generation params used for this chat."""
 
     failed: bool = Field(False, exclude=True, repr=False)
     """
     Indicates whether conditions during generation were not met.
     This is typically used for graceful error handling when parsing.
     """
@@ -63,15 +65,15 @@
             return self.generator.to_identifier(self.params)
         return None
 
     def __init__(
         self,
         messages: Messages,
         generated: Messages | None = None,
-        generator: t.Optional["Generator"] = None,
+        generator: t.Optional[Generator] = None,
         **kwargs: t.Any,
     ):
         """
         Initialize a Chat object.
 
         Args:
             messages: The messages for the chat.
@@ -125,28 +127,28 @@
         Returns the chat as a minimal message dictionaries.
 
         Returns:
             The MessageDict list
         """
         return [t.cast(MessageDict, m.model_dump(include={"role", "content"})) for m in self.all]
 
-    def meta(self, **kwargs: t.Any) -> "Chat":
+    def meta(self, **kwargs: t.Any) -> Chat:
         """
         Updates the metadata of the chat with the provided key-value pairs.
 
         Args:
             **kwargs: Key-value pairs representing the metadata to be updated.
 
         Returns:
             The updated chat object.
         """
         self.metadata.update(kwargs)
         return self
 
-    def restart(self, *, generator: t.Optional["Generator"] = None, include_all: bool = False) -> "PendingChat":
+    def restart(self, *, generator: t.Optional[Generator] = None, include_all: bool = False) -> PendingChat:
         """
         Attempt to convert back to a PendingChat for further generation.
 
         Args:
             generator: The generator to use for the restarted chat. Otherwise
                 the generator from the original PendingChat will be used.
             include_all: Whether to include the next messages in the restarted chat.
@@ -165,45 +167,45 @@
         return generator.chat(messages, self.params)
 
     def fork(
         self,
         messages: t.Sequence[Message] | t.Sequence[MessageDict] | Message | MessageDict | str,
         *,
         include_all: bool = False,
-    ) -> "PendingChat":
+    ) -> PendingChat:
         """
         Forks the chat by creating calling [rigging.chat.Chat.restart][] and appending the specified messages.
 
         Args:
             messages:
                 The messages to be added to the new `PendingChat` instance.
             include_all: Whether to include the next messages in the restarted chat.
 
         Returns:
             A new instance of `PendingChat` with the specified messages added.
 
         """
         return self.restart(include_all=include_all).add(messages)
 
-    def continue_(self, messages: t.Sequence[Message] | t.Sequence[MessageDict] | Message | str) -> "PendingChat":
+    def continue_(self, messages: t.Sequence[Message] | t.Sequence[MessageDict] | Message | str) -> PendingChat:
         """Alias for the [rigging.chat.Chat.fork][] with `include_all=True`."""
         return self.fork(messages, include_all=True)
 
-    def clone(self, *, only_messages: bool = False) -> "Chat":
+    def clone(self, *, only_messages: bool = False) -> Chat:
         """Creates a deep copy of the chat."""
         new = Chat(
             [m.model_copy() for m in self.messages],
             [m.model_copy() for m in self.generated],
             self.generator,
         )
         if not only_messages:
             new.metadata = deepcopy(self.metadata)
         return new
 
-    def apply(self, **kwargs: str) -> "Chat":
+    def apply(self, **kwargs: str) -> Chat:
         """
         Calls [rigging.message.Message.apply][] on the last message in the chat with the given keyword arguments.
 
         Args:
             **kwargs: The string mapping of replacements.
 
         Returns:
@@ -211,29 +213,29 @@
         """
         if self.generated:
             self.generated[-1] = self.generated[-1].apply(**kwargs)
         else:
             self.messages[-1] = self.messages[-1].apply(**kwargs)
         return self
 
-    def apply_to_all(self, **kwargs: str) -> "Chat":
+    def apply_to_all(self, **kwargs: str) -> Chat:
         """
         Calls [rigging.message.Message.apply][] on all messages in the chat with the given keyword arguments.
 
         Args:
             **kwargs: The string mapping of replacements.
 
         Returns:
             The modified chat object.
         """
         self.messages = Message.apply_to_list(self.messages, **kwargs)
         self.generated = Message.apply_to_list(self.generated, **kwargs)
         return self
 
-    def strip(self, model_type: type[Model], fail_on_missing: bool = False) -> "Chat":
+    def strip(self, model_type: type[Model], fail_on_missing: bool = False) -> Chat:
         """
         Strips all parsed parts of a particular type from the message content.
 
         Args:
             model_type: The type of model to keep in the chat.
             fail_on_missing: Whether to raise an exception if a message of the specified model type is not found.
 
@@ -337,60 +339,58 @@
     async def __call__(self, chats: list[Chat]) -> list[Chat]:
         """
         async variant of the [rigging.chat.MapChatCallback][] protocol.
         """
         ...
 
 
-ThenChatCallbacks = ThenChatCallback | AsyncThenChatCallback
-MapChatCallbacks = MapChatCallback | AsyncMapChatCallback
+ThenChatCallbacks = t.Union[ThenChatCallback, AsyncThenChatCallback]
+MapChatCallbacks = t.Union[MapChatCallback, AsyncMapChatCallback]
 
 # Generators
 
 MessageProducer = t.Generator[t.Sequence[Message], None, None]
 MessagesProducer = t.Generator[t.Sequence[t.Sequence[Message]], None, None]
 
 # Helper classes to manage complexity inside the run functions
 
 
 @dataclass
 class RunState:
     messages: list[Message]
-    params: "GenerateParams"
+    params: GenerateParams
     processor: t.Generator[list[Message], Message, list[Message]]
     chat: Chat | None = None
     done: bool = False
 
 
 @dataclass
 class BatchRunState:
     inputs: list[Message]
     messages: list[Message]
-    params: "GenerateParams"
+    params: GenerateParams
     processor: t.Generator[list[Message], Message, list[Message]]
     chat: Chat | None = None
     done: bool = False
 
 
 @dataclass
 class BatchRunPool:
-    generator: "Generator"
+    generator: Generator
     finished_states: list[BatchRunState]
     pending_states: list[BatchRunState]
 
 
 class PendingChat:
     """
     Represents a pending chat that can be modified and executed.
     """
 
-    def __init__(
-        self, generator: "Generator", messages: t.Sequence[Message], params: t.Optional["GenerateParams"] = None
-    ):
-        self.generator: "Generator" = generator
+    def __init__(self, generator: Generator, messages: t.Sequence[Message], params: t.Optional[GenerateParams] = None):
+        self.generator: Generator = generator
         """The generator object responsible for generating the chat."""
         self.chat: Chat = Chat(messages, pending=self)
         """The chat object representing the conversation."""
         self.params = params
         """The parameters for generating messages."""
         self.metadata: dict[str, t.Any] = {}
         """Additional metadata associated with the chat."""
@@ -404,15 +404,15 @@
         self.then_chat_callbacks: list[ThenChatCallbacks] = []
         self.map_chat_callbacks: list[MapChatCallbacks] = []
         # self.producer: MessageProducer | None = None
 
     def __len__(self) -> int:
         return len(self.chat)
 
-    def with_(self, params: t.Optional["GenerateParams"] = None, **kwargs: t.Any) -> "PendingChat":
+    def with_(self, params: t.Optional[GenerateParams] = None, **kwargs: t.Any) -> PendingChat:
         """
         Assign specific generation parameter overloads for this chat.
 
         Note:
             This will trigger a `clone` if overload params have already been set.
 
         Args:
@@ -429,17 +429,15 @@
             new = self.clone()
             new.params = self.params.merge_with(params)
             return new
 
         self.params = params
         return self
 
-    def add(
-        self, messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str
-    ) -> "PendingChat":
+    def add(self, messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str) -> PendingChat:
         """
         Appends new message(s) to the internal chat before generation.
 
         Note:
             If the last message in the chat is the same role as the first new message,
             the content will be appended. instead of a new message being created.
 
@@ -456,29 +454,29 @@
             message_list = message_list[1:]
         else:
             self.chat.generated += message_list
         return self
 
     def fork(
         self, messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str
-    ) -> "PendingChat":
+    ) -> PendingChat:
         """
         Creates a new instance of `PendingChat` by forking the current chat and adding the specified messages.
 
         This is a convenience method for calling `clone().add(messages)`.
 
         Args:
             messages: A sequence of messages or a single message to be added to the new chat.
 
         Returns:
             A new instance the pending chat with the specified messages added.
         """
         return self.clone().add(messages)
 
-    def clone(self, *, only_messages: bool = False) -> "PendingChat":
+    def clone(self, *, only_messages: bool = False) -> PendingChat:
         """
         Creates a clone of the current `PendingChat` instance.
 
         Args:
             only_messages: If True, only the messages will be cloned.
                 If False (default), the entire `PendingChat` instance will be cloned
                 including until callbacks, types, and tools.
@@ -493,28 +491,28 @@
             new.until_types = self.until_types.copy()
             new.until_tools = self.until_tools.copy()
             new.inject_tool_prompt = self.inject_tool_prompt
             new.force_tool = self.force_tool
             new.metadata = deepcopy(self.metadata)
         return new
 
-    def meta(self, **kwargs: t.Any) -> "PendingChat":
+    def meta(self, **kwargs: t.Any) -> PendingChat:
         """
         Updates the metadata of the chat with the provided key-value pairs.
 
         Args:
             **kwargs: Key-value pairs representing the metadata to be updated.
 
         Returns:
             The updated chat object.
         """
         self.metadata.update(kwargs)
         return self
 
-    def then(self, callback: ThenChatCallback | AsyncThenChatCallback) -> "PendingChat":
+    def then(self, callback: ThenChatCallback | AsyncThenChatCallback) -> PendingChat:
         """
         Registers a callback to be executed after the generation process completes.
 
         Note:
             Returning a Chat object from the callback will replace the current chat.
             for the remainder of the callbacks + return value of `run()`. This is
             optional.
@@ -535,15 +533,15 @@
 
         Returns:
             The current instance of the chat.
         """
         self.then_chat_callbacks.append(callback)
         return self
 
-    def map(self, callback: MapChatCallback | AsyncMapChatCallback) -> "PendingChat":
+    def map(self, callback: MapChatCallback | AsyncMapChatCallback) -> PendingChat:
         """
         Registers a callback to be executed after the generation process completes.
 
         Note:
             You must return a list of Chat objects from the callback which will
             represent the state of chats for the remainder of the callbacks and return.
 
@@ -581,29 +579,29 @@
     #         ValueError: If a producer has already been set.
     #     """
     #     if self.producer is not None:
     #         raise ValueError("A producer has already been set")
     #     self.producer = producer
     #     return self
 
-    def apply(self, **kwargs: str) -> "PendingChat":
+    def apply(self, **kwargs: str) -> PendingChat:
         """
         Clones this pending chat and calls [rigging.chat.Chat.apply][] with the given keyword arguments.
 
         Args:
             **kwargs: Keyword arguments to be applied to the chat.
 
         Returns:
             A new instance of PendingChat with the applied arguments.
         """
         new = self.clone()
         new.chat.apply(**kwargs)
         return new
 
-    def apply_to_all(self, **kwargs: str) -> "PendingChat":
+    def apply_to_all(self, **kwargs: str) -> PendingChat:
         """
         Clones this pending chat and calls [rigging.chat.Chat.apply_to_all][] with the given keyword arguments.
 
         Args:
             **kwargs: Keyword arguments to be applied to the chat.
 
         Returns:
@@ -616,15 +614,15 @@
     def until(
         self,
         callback: UntilMessageCallback,
         *,
         attempt_recovery: bool = True,
         drop_dialog: bool = True,
         max_rounds: int = DEFAULT_MAX_ROUNDS,
-    ) -> "PendingChat":
+    ) -> PendingChat:
         """
         Registers a callback to participate in validating the generation process.
 
         ```py
         # Takes the next message being generated, and returns whether or not to continue
         # generating new messages in addition to a list of messages to append before continuing
 
@@ -661,15 +659,15 @@
         self,
         *tools: Tool,
         force: bool = False,
         attempt_recovery: bool = True,
         drop_dialog: bool = False,
         max_rounds: int = DEFAULT_MAX_ROUNDS,
         inject_prompt: bool | None = None,
-    ) -> "PendingChat":
+    ) -> PendingChat:
         """
         Adds a tool or a sequence of tools to participate in the generation process.
 
         Args:
             tools: The tool or sequence of tools to be added.
             force: Whether to force the use of the tool(s) at least once.
             attempt_recovery: Whether to attempt recovery if the tool(s) fail by providing
@@ -700,15 +698,15 @@
 
     def until_parsed_as(
         self,
         *types: type[ModelT],
         attempt_recovery: bool = False,
         drop_dialog: bool = True,
         max_rounds: int = DEFAULT_MAX_ROUNDS,
-    ) -> "PendingChat":
+    ) -> PendingChat:
         """
         Adds the specified types to the list of types which should successfully parse
         before the generation process completes.
 
         Args:
             *types: The type or types of models to wait for.
             attempt_recovery: Whether to attempt recovery if parsing fails by providing
@@ -728,15 +726,15 @@
 
     def _until_tools_callback(self, message: Message) -> tuple[bool, list[Message]]:
         generated: list[Message] = [message]
 
         try:
             tool_calls = message.try_parse(ToolCalls)
         except ValidationError as e:
-            generated.append(Message.from_model(ValidationErrorModel(content=e)))
+            generated.append(Message.from_model(ValidationErrorModel(content=str(e))))
             return (True, generated)
 
         if tool_calls is None:
             if self.force_tool:
                 logger.debug("No tool calls or types, returning error")
                 generated.append(Message.from_model(SystemErrorModel(content="You must use a tool")))
             else:
@@ -774,23 +772,24 @@
 
         try:
             message.parse_many(*self.until_types)
         except ValidationError as e:
             should_continue = True
             generated.append(
                 Message.from_model(
-                    ValidationErrorModel(content=e),
+                    ValidationErrorModel(content=str(e)),
                     suffix="Rewrite your entire message with all the required elements.",
                 )
             )
         except Exception as e:
             should_continue = True
             generated.append(
                 Message.from_model(
-                    SystemErrorModel(content=e), suffix="Rewrite your entire message with all the required elements."
+                    SystemErrorModel(content=str(e)),
+                    suffix="Rewrite your entire message with all the required elements.",
                 )
             )
 
         return (should_continue, generated)
 
     def _until(
         self,
@@ -889,16 +888,16 @@
             # the stop sequence as part of the response. This behavior
             # seems like a larger issue than the model continuining after
             # requesting a tool call, so we'll remove it for now.
             #
             # self.params.stop = [ToolCalls.xml_end_tag()]
 
     def _fit_params(
-        self, count: int, params: t.Sequence[t.Optional["GenerateParams"] | None] | None = None
-    ) -> list["GenerateParams"]:
+        self, count: int, params: t.Sequence[t.Optional[GenerateParams] | None] | None = None
+    ) -> list[GenerateParams]:
         params = [None] * count if params is None else list(params)
         if len(params) != count:
             raise ValueError(f"The number of params must be {count}")
         if self.params is not None:
             params = [self.params.merge_with(p) for p in params]
         return [(p or GenerateParams()) for p in params]
 
@@ -940,15 +939,15 @@
 
     # Many messages
 
     def run_many(
         self,
         count: int,
         *,
-        params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
+        params: t.Sequence[t.Optional[GenerateParams]] | None = None,
         skip_failed: bool = False,
         include_failed: bool = False,
     ) -> list[Chat]:
         """
         Executes the generation process multiple times with the same inputs.
 
         Parameters:
@@ -969,15 +968,15 @@
 
         pending_states = states
         while pending_states:
             inbounds = self.generator.generate_messages(
                 [self.chat.all + s.messages for s in pending_states], [s.params for s in pending_states]
             )
 
-            for inbound, state in zip(inbounds, pending_states, strict=True):
+            for inbound, state in zip(inbounds, pending_states):
                 try:
                     state.messages = state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
                     state.chat = Chat(
                         self.chat.all,
                         t.cast(list[Message], stop.value),
@@ -1003,15 +1002,15 @@
 
         return self._post_run([s.chat for s in states if s.chat is not None])
 
     async def arun_many(
         self,
         count: int,
         *,
-        params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
+        params: t.Sequence[t.Optional[GenerateParams]] | None = None,
         skip_failed: bool = False,
         include_failed: bool = False,
     ) -> list[Chat]:
         """async variant of the [rigging.chat.PendingChat.run_many][] method."""
         if skip_failed and include_failed:
             raise ValueError("Cannot use both skip_failed and include_failed")
 
@@ -1020,15 +1019,15 @@
 
         pending_states = states
         while pending_states:
             inbounds = await self.generator.agenerate_messages(
                 [self.chat.all + s.messages for s in pending_states], [s.params for s in pending_states]
             )
 
-            for inbound, state in zip(inbounds, pending_states, strict=True):
+            for inbound, state in zip(inbounds, pending_states):
                 try:
                     state.messages = state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
                     state.chat = Chat(
                         self.chat.all,
                         t.cast(list[Message], stop.value),
@@ -1060,15 +1059,15 @@
         self,
         many: t.Sequence[t.Sequence[Message]]
         | t.Sequence[Message]
         | t.Sequence[MessageDict]
         | t.Sequence[str]
         | MessageDict
         | str,
-        params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
+        params: t.Sequence[t.Optional[GenerateParams]] | None = None,
         *,
         size: int | None = None,
         skip_failed: bool = False,
         include_failed: bool = False,
     ) -> list[Chat]:
         """
         Executes the generation process accross multiple input messages.
@@ -1088,36 +1087,36 @@
         Returns:
             A list of generatated Chats.
         """
         if skip_failed and include_failed:
             raise ValueError("Cannot use both skip_failed and include_failed")
 
         if isinstance(many, dict) or isinstance(many, str):  # Some strange typechecking here
-            many = t.cast(t.Sequence[str] | t.Sequence[MessageDict], [many])
+            many = t.cast(t.Union[t.Sequence[str], t.Sequence[MessageDict]], [many])
 
         count = max(len(many), len(params) if params is not None else 0)
         many = self._fit_many(count, many)
         params = self._fit_params(count, params)
 
         states: list[BatchRunState] = [
-            BatchRunState(self.chat.all + m, [], p, self._process()) for m, p in zip(many, params, strict=True)
+            BatchRunState(self.chat.all + m, [], p, self._process()) for m, p in zip(many, params)
         ]
         _ = [next(state.processor) for state in states]
 
         size = size or len(states)
 
         pending_states = states
         while pending_states:
             for chunk in [pending_states[i : i + size] for i in range(0, len(pending_states), size)]:
                 inbounds = self.generator.generate_messages(
                     [s.inputs + s.messages for s in chunk],
                     [s.params for s in chunk],
                 )
 
-                for inbound, state in zip(inbounds, chunk, strict=True):
+                for inbound, state in zip(inbounds, chunk):
                     try:
                         state.messages = state.processor.send(inbound)
                     except StopIteration as stop:
                         state.done = True
                         state.chat = Chat(
                             state.inputs,
                             t.cast(list[Message], stop.value),
@@ -1147,48 +1146,48 @@
         self,
         many: t.Sequence[t.Sequence[Message]]
         | t.Sequence[Message]
         | t.Sequence[MessageDict]
         | t.Sequence[str]
         | MessageDict
         | str,
-        params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
+        params: t.Sequence[t.Optional[GenerateParams]] | None = None,
         *,
         size: int | None = None,
         skip_failed: bool = False,
         include_failed: bool = False,
     ) -> list[Chat]:
         """async variant of the [rigging.chat.PendingChat.run_batch][] method."""
 
         if skip_failed and include_failed:
             raise ValueError("Cannot use both skip_failed and include_failed")
 
         if isinstance(many, dict) or isinstance(many, str):  # Some strange typechecking here
-            many = t.cast(t.Sequence[str] | t.Sequence[MessageDict], [many])
+            many = t.cast(t.Union[t.Sequence[str], t.Sequence[MessageDict]], [many])
 
         count = max(len(many), len(params) if params is not None else 0)
         many = self._fit_many(count, many)
         params = self._fit_params(count, params)
 
         states: list[BatchRunState] = [
-            BatchRunState(self.chat.all + m, [], p, self._process()) for m, p in zip(many, params, strict=True)
+            BatchRunState(self.chat.all + m, [], p, self._process()) for m, p in zip(many, params)
         ]
         _ = [next(state.processor) for state in states]
 
         size = size or len(states)
 
         pending_states = states
         while pending_states:
             for chunk in [pending_states[i : i + size] for i in range(0, len(pending_states), size)]:
                 inbounds = await self.generator.agenerate_messages(
                     [s.inputs + s.messages for s in chunk],
                     [s.params for s in chunk],
                 )
 
-                for inbound, state in zip(inbounds, chunk, strict=True):
+                for inbound, state in zip(inbounds, chunk):
                     try:
                         state.messages = state.processor.send(inbound)
                     except StopIteration as stop:
                         state.done = True
                         state.chat = Chat(
                             state.inputs,
                             t.cast(list[Message], stop.value),
```

### Comparing `rigging-1.1.1/rigging/completion.py` & `rigging-1.1.2/rigging/completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """
 Completions work with isolated strings of text pre and post generation.
 """
 
+from __future__ import annotations
+
 import asyncio
 import string
 import typing as t
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
 from typing import runtime_checkable
 from uuid import UUID, uuid4
 
 from loguru import logger
 from pydantic import BaseModel, ConfigDict, Field, computed_field
 
 from rigging.error import CompletionExhaustedMaxRoundsError
 from rigging.generator import GenerateParams, Generator, get_generator
-from rigging.model import Model, ModelT
 from rigging.parsing import parse_many
 
+if t.TYPE_CHECKING:
+    from rigging.model import Model, ModelT
+
 DEFAULT_MAX_ROUNDS = 5
 
 # TODO: Chats and Completions share a lot of structure and code.
 # Ideally we should build out a base class which they both inherit from.
 
 
 class Completion(BaseModel):
@@ -39,17 +43,17 @@
     text: str
     """The original text."""
     generated: str
     """The generated text."""
     metadata: dict[str, t.Any] = Field(default_factory=dict)
     """Additional metadata for the completion."""
 
-    generator: t.Optional["Generator"] = Field(None, exclude=True, repr=False)
+    generator: t.Optional[Generator] = Field(None, exclude=True, repr=False)
     """The generator associated with the completion."""
-    params: t.Optional["GenerateParams"] = Field(None, exclude=True, repr=False)
+    params: t.Optional[GenerateParams] = Field(None, exclude=True, repr=False)
     """Any additional generation params used for this completion."""
 
     failed: bool = Field(default=False, repr=False)
     """
     Indicates whether conditions during generation were not met.
     This is typically used for graceful error handling when parsing.
     """
@@ -62,15 +66,15 @@
             return self.generator.to_identifier(self.params)
         return None
 
     def __init__(
         self,
         text: str,
         generated: str,
-        generator: t.Optional["Generator"] = None,
+        generator: t.Optional[Generator] = None,
         **kwargs: t.Any,
     ):
         """
         Initialize a Completion object.
 
         Args:
             text: The original text.
@@ -93,15 +97,15 @@
         return len(self.text) + len(self.generated)
 
     @property
     def all(self) -> str:
         """Returns both the text and the generation."""
         return self.text + self.generated
 
-    def restart(self, *, generator: t.Optional["Generator"] = None, include_all: bool = False) -> "PendingCompletion":
+    def restart(self, *, generator: t.Optional[Generator] = None, include_all: bool = False) -> PendingCompletion:
         """
         Attempt to convert back to a PendingCompletion for further generation.
 
         Args:
             generator: The generator to use for the restarted completion. Otherwise
                 the generator from the original PendingCompletion will be used.
             include_all: Whether to include the generation before the next round.
@@ -116,38 +120,38 @@
         text = self.all if include_all else self.generated
         if generator is None:
             generator = self.generator
         if generator is None:
             raise ValueError("Cannot restart a completion without an associated generator")
         return generator.complete(text, self.params)
 
-    def fork(self, text: str, *, include_all: bool = False) -> "PendingCompletion":
+    def fork(self, text: str, *, include_all: bool = False) -> PendingCompletion:
         """
         Forks the completion by creating calling [rigging.completion.Completion.restart][] and appends the specified text.
 
         Args:
             text: The text to append.
 
         Returns:
             A new instance of a pending competion with the specified messages added.
         """
         return self.restart(include_all=include_all).add(text)
 
-    def continue_(self, text: str) -> "PendingCompletion":
+    def continue_(self, text: str) -> PendingCompletion:
         """Alias for the [rigging.completion.Completion.fork][] with `include_all=True`."""
         return self.fork(text, include_all=True)
 
-    def clone(self, *, only_messages: bool = False) -> "Completion":
+    def clone(self, *, only_messages: bool = False) -> Completion:
         """Creates a deep copy of the completion."""
         new = Completion(self.text, self.generated, self.generator)
         if not only_messages:
             new.metadata = deepcopy(self.metadata)
         return new
 
-    def meta(self, **kwargs: t.Any) -> "Completion":
+    def meta(self, **kwargs: t.Any) -> Completion:
         """
         Updates the metadata of the completion with the provided key-value pairs.
 
         Args:
             **kwargs: Key-value pairs representing the metadata to be updated.
 
         Returns:
@@ -203,34 +207,34 @@
     async def __call__(self, completions: list[Completion]) -> list[Completion]:
         """
         async variant of the [rigging.completion.MapCompletionCallback][] protocol.
         """
         ...
 
 
-ThenCompletionCallbacks = ThenCompletionCallback | AsyncThenCompletionCallback
-MapCompletionCallbacks = MapCompletionCallback | AsyncMapCompletionCallback
+ThenCompletionCallbacks = t.Union[ThenCompletionCallback, AsyncThenCompletionCallback]
+MapCompletionCallbacks = t.Union[MapCompletionCallback, AsyncMapCompletionCallback]
 
 
 @dataclass
 class RunState:
     text: str
-    params: "GenerateParams"
+    params: GenerateParams
     processor: t.Generator[None, str, str]
     completion: Completion | None = None
     done: bool = False
 
 
 class PendingCompletion:
     """
     Represents a pending completion that can be modified and executed.
     """
 
-    def __init__(self, generator: "Generator", text: str, params: t.Optional["GenerateParams"] = None):
-        self.generator: "Generator" = generator
+    def __init__(self, generator: Generator, text: str, params: t.Optional[GenerateParams] = None):
+        self.generator: Generator = generator
         """The generator object responsible for generating the completion."""
         self.text = text
         """The text to be completed."""
         self.params = params
         """The parameters for generating the completion."""
         self.metadata: dict[str, t.Any] = {}
         """Additional metadata associated with the completion."""
@@ -240,15 +244,15 @@
         self.until_types: list[type[Model]] = []
         self.then_callbacks: list[ThenCompletionCallbacks] = []
         self.map_callbacks: list[MapCompletionCallbacks] = []
 
     def __len__(self) -> int:
         return len(self.text)
 
-    def with_(self, params: t.Optional["GenerateParams"] = None, **kwargs: t.Any) -> "PendingCompletion":
+    def with_(self, params: t.Optional[GenerateParams] = None, **kwargs: t.Any) -> PendingCompletion:
         """
         Assign specific generation parameter overloads for this completion.
 
         Note:
             This will trigger a `clone` if overload params have already been set.
 
         Args:
@@ -265,15 +269,15 @@
             new = self.clone()
             new.params = self.params.merge_with(params)
             return new
 
         self.params = params
         return self
 
-    def then(self, callback: ThenCompletionCallback) -> "PendingCompletion":
+    def then(self, callback: ThenCompletionCallback) -> PendingCompletion:
         """
         Registers a callback to be executed after the generation process completes.
 
         Note:
             Returning a Completion object from the callback will replace the current completion.
             for the remainder of the callbacks + return value of `run()`.
 
@@ -289,15 +293,15 @@
 
         Returns:
             The current instance of the pending completion.
         """
         self.then_callbacks.append(callback)
         return self
 
-    def map(self, callback: MapCompletionCallback | AsyncMapCompletionCallback) -> "PendingCompletion":
+    def map(self, callback: MapCompletionCallback | AsyncMapCompletionCallback) -> PendingCompletion:
         """
         Registers a callback to be executed after the generation process completes.
 
         Note:
             You must return a list of completion objects from the callback which will
             represent the state of completions for the remainder of the callbacks and return.
 
@@ -317,42 +321,42 @@
 
         Returns:
             The current instance of the completion.
         """
         self.map_callbacks.append(callback)
         return self
 
-    def add(self, text: str) -> "PendingCompletion":
+    def add(self, text: str) -> PendingCompletion:
         """
         Appends new text to the internal text before generation.
 
         Args:
             text: The text to be added to the completion.
 
         Returns:
             The updated PendingCompletion object.
         """
         self.text += text
         return self
 
-    def fork(self, text: str) -> "PendingCompletion":
+    def fork(self, text: str) -> PendingCompletion:
         """
         Creates a new instance of `PendingCompletion` by forking the current completion and adding the specified text.
 
         This is a convenience method for calling `clone().add(text)`.
 
         Args:
             text: The text to be added to the new completion.
 
         Returns:
             A new instance of `PendingCompletion` with the specified text added.
         """
         return self.clone().add(text)
 
-    def clone(self, *, only_text: bool = False) -> "PendingCompletion":
+    def clone(self, *, only_text: bool = False) -> PendingCompletion:
         """
         Creates a clone of the current `PendingCompletion` instance.
 
         Args:
             only_text: If True, only the text will be cloned.
                 If False (default), the entire `PendingCompletion` instance will be cloned
                 including until callbacks and types.
@@ -363,28 +367,28 @@
         new = PendingCompletion(self.generator, self.text, self.params)
         if not only_text:
             new.until_callbacks = self.until_callbacks.copy()
             new.until_types = self.until_types.copy()
             new.metadata = deepcopy(self.metadata)
         return new
 
-    def meta(self, **kwargs: t.Any) -> "PendingCompletion":
+    def meta(self, **kwargs: t.Any) -> PendingCompletion:
         """
         Updates the metadata of the completion with the provided key-value pairs.
 
         Args:
             **kwargs: Key-value pairs representing the metadata to be updated.
 
         Returns:
             The updated completion object.
         """
         self.metadata.update(kwargs)
         return self
 
-    def apply(self, **kwargs: str) -> "PendingCompletion":
+    def apply(self, **kwargs: str) -> PendingCompletion:
         """
         Applies keyword arguments to the text using string template substitution.
 
         Note:
             This produces a clone of the PendingCompletion, leaving the original unchanged.
 
         Args:
@@ -400,15 +404,15 @@
 
     def until(
         self,
         callback: UntilCompletionCallback,
         *,
         use_all_text: bool = False,
         max_rounds: int = DEFAULT_MAX_ROUNDS,
-    ) -> "PendingCompletion":
+    ) -> PendingCompletion:
         """
         Registers a callback to participate in validating the generation process.
 
         ```py
         # Takes the generated text, and returns whether or not to retry generation.
 
         def callback(text: str) -> bool:
@@ -434,15 +438,15 @@
         return self
 
     def until_parsed_as(
         self,
         *types: type[ModelT],
         use_all_text: bool = False,
         max_rounds: int = DEFAULT_MAX_ROUNDS,
-    ) -> "PendingCompletion":
+    ) -> PendingCompletion:
         """
         Adds the specified types to the list of types which should successfully parse
         before the generation process completes.
 
         Args:
             *types: The type or types of models to wait for.
             use_all_text: Whether to pass the entire text (including prompt) to the parser.
@@ -497,16 +501,16 @@
                 )
             updated = [await then_callback(completion) for completion in completions]
             completions = [updated[i] or completion for i, completion in enumerate(completions)]
 
         return completions
 
     def _fit_params(
-        self, count: int, params: t.Sequence[t.Optional["GenerateParams"] | None] | None = None
-    ) -> list["GenerateParams"]:
+        self, count: int, params: t.Sequence[t.Optional[GenerateParams] | None] | None = None
+    ) -> list[GenerateParams]:
         params = [None] * count if params is None else list(params)
         if len(params) != count:
             raise ValueError(f"The number of params must be {count}")
         if self.params is not None:
             params = [self.params.merge_with(p) for p in params]
         return [(p or GenerateParams()) for p in params]
 
@@ -559,15 +563,15 @@
 
     # Many messages
 
     def run_many(
         self,
         count: int,
         *,
-        params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
+        params: t.Sequence[t.Optional[GenerateParams]] | None = None,
         skip_failed: bool = False,
         include_failed: bool = False,
     ) -> list[Completion]:
         """
         Executes the generation process multiple times with the same inputs.
 
         Parameters:
@@ -586,15 +590,15 @@
 
         pending_states = states
         while pending_states:
             inbounds = self.generator.generate_texts(
                 [s.text for s in pending_states], [s.params for s in pending_states]
             )
 
-            for inbound, state in zip(inbounds, pending_states, strict=True):
+            for inbound, state in zip(inbounds, pending_states):
                 try:
                     state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
                         self.text,
                         t.cast(str, stop.value),
@@ -620,15 +624,15 @@
 
         return self._post_run([s.completion for s in states if s.completion is not None])
 
     async def arun_many(
         self,
         count: int,
         *,
-        params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
+        params: t.Sequence[t.Optional[GenerateParams]] | None = None,
         skip_failed: bool = False,
         include_failed: bool = False,
     ) -> list[Completion]:
         """async variant of the [rigging.completion.PendingCompletion.run_many][] method."""
         if skip_failed and include_failed:
             raise ValueError("Cannot use both skip_failed and include_failed")
 
@@ -637,15 +641,15 @@
 
         pending_states = states
         while pending_states:
             inbounds = await self.generator.agenerate_texts(
                 [s.text for s in pending_states], [s.params for s in pending_states]
             )
 
-            for inbound, state in zip(inbounds, pending_states, strict=True):
+            for inbound, state in zip(inbounds, pending_states):
                 try:
                     state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
                         self.text,
                         t.cast(str, stop.value),
@@ -672,15 +676,15 @@
         return self._post_run([s.completion for s in states if s.completion is not None])
 
     # Batch completions
 
     def run_batch(
         self,
         many: t.Sequence[str],
-        params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
+        params: t.Sequence[t.Optional[GenerateParams]] | None = None,
         *,
         skip_failed: bool = False,
         include_failed: bool = False,
     ) -> list[Completion]:
         """
         Executes the generation process accross multiple input messages.
 
@@ -696,25 +700,25 @@
         Returns:
             A list of generatated Completions.
         """
         if skip_failed and include_failed:
             raise ValueError("Cannot use both skip_failed and include_failed")
 
         params = self._fit_params(len(many), params)
-        states: list[RunState] = [RunState(m, p, self._process()) for m, p in zip(many, params, strict=True)]
+        states: list[RunState] = [RunState(m, p, self._process()) for m, p in zip(many, params)]
         _ = [next(state.processor) for state in states]
 
         pending_states = states
         while pending_states:
             inbounds = self.generator.generate_texts(
                 [self.text + s.text for s in pending_states],
                 [s.params for s in pending_states],
             )
 
-            for inbound, state in zip(inbounds, pending_states, strict=True):
+            for inbound, state in zip(inbounds, pending_states):
                 try:
                     state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
                         self.text,
                         t.cast(str, stop.value),
@@ -739,35 +743,35 @@
             pending_states = [s for s in pending_states if not s.done]
 
         return self._post_run([s.completion for s in states if s.completion is not None])
 
     async def arun_batch(
         self,
         many: t.Sequence[str],
-        params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
+        params: t.Sequence[t.Optional[GenerateParams]] | None = None,
         *,
         skip_failed: bool = False,
         include_failed: bool = False,
     ) -> list[Completion]:
         """async variant of the [rigging.completion.PendingCompletion.run_batch][] method."""
         if skip_failed and include_failed:
             raise ValueError("Cannot use both skip_failed and include_failed")
 
         params = self._fit_params(len(many), params)
-        states: list[RunState] = [RunState(m, p, self._process()) for m, p in zip(many, params, strict=True)]
+        states: list[RunState] = [RunState(m, p, self._process()) for m, p in zip(many, params)]
         _ = [next(state.processor) for state in states]
 
         pending_states = states
         while pending_states:
             inbounds = await self.generator.agenerate_texts(
                 [self.text + s.text for s in pending_states],
                 [s.params for s in pending_states],
             )
 
-            for inbound, state in zip(inbounds, pending_states, strict=True):
+            for inbound, state in zip(inbounds, pending_states):
                 try:
                     state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
                         self.text,
                         t.cast(str, stop.value),
```

### Comparing `rigging-1.1.1/rigging/data.py` & `rigging-1.1.2/rigging/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import typing as t
 
 import pandas as pd
 
 from rigging.chat import Chat
 from rigging.message import Message
@@ -24,27 +26,30 @@
     """
     chats = [chats] if isinstance(chats, Chat) else chats
 
     data: list[dict[t.Any, t.Any]] = []
     for chat in chats:
         generator_id = chat.generator_id
         metadata = json.dumps(chat.metadata)
+
         generated = False
         for messages in [chat.messages, chat.generated]:
             for message in messages:
-                message_dict = message.model_dump()
-                message_dict["message_id"] = message_dict.pop("uuid")
+                message_dict = message.model_dump(exclude={"uuid"})
+                message_parts_json = json.dumps(message_dict.pop("parts"))
                 data.append(
                     {
                         "chat_id": chat.uuid,
                         "chat_metadata": metadata,
                         "chat_generator_id": generator_id,
                         "chat_timestamp": chat.timestamp,
                         "generated": generated,
+                        "message_id": str(message.uuid),
                         **message_dict,
+                        "parts": message_parts_json,
                     }
                 )
             generated = True
 
     df = pd.DataFrame(data).astype(
         {
             "chat_id": "string",
@@ -85,16 +90,19 @@
         messages = []
         generated = []
 
         for _, message_data in chat_group.iterrows():
             message = Message(
                 role=message_data["role"],
                 content=message_data["content"],
-                parts=json.loads(message_data["parts"]),
                 **{"uuid": message_data["message_id"]},
+                # TODO: I don't believe this is safe to deserialize
+                # here as we aren't bonded to the underlying rg.Model
+                # which was the original object. Skipping for now.
+                # parts=json.loads(message_data["parts"]),
             )
             if message_data["generated"]:
                 generated.append(message)
             else:
                 messages.append(message)
 
         chat = Chat(
```

### Comparing `rigging-1.1.1/rigging/error.py` & `rigging-1.1.2/rigging/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 We try to avoid creating custom exceptions unless they are necessary.
 
 We use the built-in and pydantic exceptions as much as possible.
 """
 
-from typing import TYPE_CHECKING
+import typing as t
 
-if TYPE_CHECKING:
+if t.TYPE_CHECKING:
     from rigging.message import Message
 
 
 class ExhaustedMaxRoundsError(Exception):
     """
     Raised when the maximum number of rounds is exceeded while generating.
     """
```

### Comparing `rigging-1.1.1/rigging/generator/__init__.py` & `rigging-1.1.2/rigging/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `rigging-1.1.1/rigging/generator/base.py` & `rigging-1.1.2/rigging/generator/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import inspect
 import typing as t
 
 from loguru import logger
 from pydantic import BaseModel, ConfigDict, Field, field_validator
 from typing_extensions import Self
 
@@ -9,15 +11,15 @@
 from rigging.message import Message, MessageDict
 
 if t.TYPE_CHECKING:
     from rigging.chat import PendingChat
     from rigging.completion import PendingCompletion
 
 # Global provider map
-g_providers: dict[str, type["Generator"]] = {}
+g_providers: dict[str, type[Generator]] = {}
 
 
 # TODO: Ideally we flex this to support arbitrary
 # generator params, but we'll limit things
 # for now until we understand the use cases
 #
 # TODO: We also would like to support N-style
@@ -73,15 +75,15 @@
     def validate_stop(cls, value: t.Any) -> t.Any:
         if isinstance(value, str):
             return value.split(";")
         elif isinstance(value, list) and all(isinstance(v, str) for v in value):
             return value
         raise ValueError("Stop sequences must be a list or a string separated by ';'")
 
-    def merge_with(self, *others: t.Optional["GenerateParams"]) -> "GenerateParams":
+    def merge_with(self, *others: t.Optional[GenerateParams]) -> GenerateParams:
         """
         Apply a series of parameter overrides to the current instance and return a copy.
 
         Args:
             *others: The parameters to be merged with the current instance's parameters.
                 Can be multiple and overrides will be applied in order.
 
@@ -236,30 +238,30 @@
     # params seem odd, but mypy doesn't like the TypedDict in a list otherwise
 
     @t.overload
     def chat(
         self,
         messages: t.Sequence[MessageDict],
         params: GenerateParams | None = None,
-    ) -> "PendingChat":
+    ) -> PendingChat:
         ...
 
     @t.overload
     def chat(
         self,
         messages: t.Sequence[Message] | MessageDict | Message | str | None = None,
         params: GenerateParams | None = None,
-    ) -> "PendingChat":
+    ) -> PendingChat:
         ...
 
     def chat(
         self,
         messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str | None = None,
         params: GenerateParams | None = None,
-    ) -> "PendingChat":
+    ) -> PendingChat:
         """
         Build a pending chat with the given messages and optional params overloads.
 
         Args:
             messages: The messages to be sent in the chat.
             params: Optional parameters for generating responses.
 
@@ -268,15 +270,15 @@
         """
         from rigging.chat import PendingChat
 
         return PendingChat(self, Message.fit_as_list(messages) if messages else [], params)
 
     # Helper alternative to complete(generator) -> generator.complete(...)
 
-    def complete(self, text: str, params: GenerateParams | None = None) -> "PendingCompletion":
+    def complete(self, text: str, params: GenerateParams | None = None) -> PendingCompletion:
         """
         Build a pending string completion of the given text with optional param overloads.
 
         Args:
             text: The input text to be completed.
             params: The parameters to be used for completion.
 
@@ -286,35 +288,35 @@
         from rigging.completion import PendingCompletion
 
         return PendingCompletion(self, text, params)
 
 
 @t.overload
 def chat(
-    generator: "Generator",
+    generator: Generator,
     messages: t.Sequence[MessageDict],
     params: GenerateParams | None = None,
-) -> "PendingChat":
+) -> PendingChat:
     ...
 
 
 @t.overload
 def chat(
-    generator: "Generator",
+    generator: Generator,
     messages: t.Sequence[Message] | MessageDict | Message | str | None = None,
     params: GenerateParams | None = None,
-) -> "PendingChat":
+) -> PendingChat:
     ...
 
 
 def chat(
-    generator: "Generator",
+    generator: Generator,
     messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str | None = None,
     params: GenerateParams | None = None,
-) -> "PendingChat":
+) -> PendingChat:
     """
     Creates a pending chat using the given generator, messages, and params.
 
     Args:
         generator: The generator to use for creating the chat.
         messages:
             The messages to include in the chat. Can be a single message or a sequence of messages.
@@ -326,15 +328,15 @@
     return generator.chat(messages, params)
 
 
 def complete(
     generator: Generator,
     text: str,
     params: GenerateParams | None = None,
-) -> "PendingCompletion":
+) -> PendingCompletion:
     return generator.complete(text, params)
 
 
 def get_identifier(generator: Generator, params: GenerateParams | None = None) -> str:
     """
     Converts the generator instance back into a rigging identifier string.
 
@@ -366,15 +368,15 @@
         if "stop" in params_dict:
             params_dict["stop"] = ";".join(params_dict["stop"])
         identifier += f",{','.join([f'{k}={v}' for k, v in params_dict.items()])}"
 
     return identifier
 
 
-def get_generator(identifier: str) -> Generator:
+def get_generator(identifier: str, *, params: GenerateParams | None = None) -> Generator:
     """
     Get a generator by an identifier string. Uses LiteLLM by default.
 
     Identifier strings are formatted like `<provider>!<model>,<**kwargs>`
 
     (provider is optional andif not specified)
 
@@ -390,25 +392,26 @@
     - "gpt-4-0613,temperature=0.9,max_tokens=512"
     - "claude-2.1,stop_sequences=Human:;test,max_tokens=100"
 
     (These get parsed as [rigging.generator.GenerateParams][])
 
     Args:
         identifier: The identifier string to use to get a generator.
+        params: The generation parameters to use for the generator.
+            These will override any parameters specified in the identifier string.
 
     Returns:
         The generator object.
 
     Raises:
         InvalidModelSpecified: If the identifier is invalid.
     """
 
     provider: str = list(g_providers.keys())[0]
     model: str = identifier
-    params: GenerateParams = GenerateParams()
 
     # Split provider, model, and kwargs
 
     if "!" in identifier:
         try:
             provider, model = identifier.split("!")
         except Exception as e:
@@ -445,19 +448,19 @@
         except ValueError:
             pass
 
         if isinstance(v, str) and v.lower() in ["true", "false"]:
             init_kwargs[k] = v.lower() == "true"
 
     try:
-        params = GenerateParams(**kwargs)
+        merged_params = GenerateParams(**kwargs).merge_with(params)
     except Exception as e:
         raise InvalidModelSpecifiedError(identifier) from e
 
-    return generator_cls(model=model, params=params, **init_kwargs)
+    return generator_cls(model=model, params=merged_params, **init_kwargs)
 
 
 def register_generator(provider: str, generator_cls: type[Generator]) -> None:
     """
     Register a generator class for a provider id.
 
     This let's you use [rigging.generator.get_generator][] with a custom generator class.
```

### Comparing `rigging-1.1.1/rigging/generator/litellm_.py` & `rigging-1.1.2/rigging/generator/litellm_.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 import typing as t
 
 import litellm  # type: ignore
 
 from rigging.generator.base import GenerateParams, Generator, register_generator, trace_messages, trace_str
 from rigging.message import Message
@@ -87,15 +89,15 @@
 
     def generate_messages(
         self,
         messages: t.Sequence[t.Sequence[Message]],
         params: t.Sequence[GenerateParams],
     ) -> t.Sequence[Message]:
         generated: list[Message] = []
-        for i, (_messages, _params) in enumerate(zip(messages, params, strict=True)):
+        for i, (_messages, _params) in enumerate(zip(messages, params)):
             trace_messages(_messages, f"Messages {i+1}/{len(messages)}")
             next_message = self._generate_message(_messages, _params)
             generated.append(next_message)
             trace_messages([next_message], f"Response {i+1}/{len(messages)}")
 
         return generated
 
@@ -108,32 +110,32 @@
         max_requests = self.max_requests or len(messages)
         for i in range(0, len(messages), max_requests):
             chunk_messages = messages[i : i + max_requests]
             chunk_params = params[i : i + max_requests]
             chunk_generated = await asyncio.gather(
                 *[
                     self._agenerate_message(_messages, _params)
-                    for _messages, _params in zip(chunk_messages, chunk_params, strict=True)
+                    for _messages, _params in zip(chunk_messages, chunk_params)
                 ]
             )
             generated.extend(chunk_generated)
 
-            for j, (_messages, _generated) in enumerate(zip(chunk_messages, chunk_generated, strict=True)):
+            for j, (_messages, _generated) in enumerate(zip(chunk_messages, chunk_generated)):
                 trace_messages(_messages, f"Messages {i+j+1}/{len(messages)}")
                 trace_messages([_generated], f"Response {i+j+1}/{len(messages)}")
 
         return generated
 
     def generate_texts(
         self,
         texts: t.Sequence[str],
         params: t.Sequence[GenerateParams],
     ) -> t.Sequence[str]:
         generated: list[str] = []
-        for i, (text, _params) in enumerate(zip(texts, params, strict=True)):
+        for i, (text, _params) in enumerate(zip(texts, params)):
             trace_str(text, f"Text {i+1}/{len(texts)}")
             response = self._generate_text(text, _params)
             generated.append(response)
             trace_str(response, f"Generated {i+1}/{len(texts)}")
 
         return generated
 
@@ -144,19 +146,19 @@
     ) -> t.Sequence[str]:
         generated: list[str] = []
         max_requests = self.max_requests or len(texts)
         for i in range(0, len(texts), max_requests or len(texts)):
             chunk_texts = texts[i : i + max_requests]
             chunk_params = params[i : i + max_requests]
             chunk_generated = await asyncio.gather(
-                *[self._agenerate_text(text, _params) for text, _params in zip(chunk_texts, chunk_params, strict=True)]
+                *[self._agenerate_text(text, _params) for text, _params in zip(chunk_texts, chunk_params)]
             )
             generated.extend(chunk_generated)
 
-            for i, (text, response) in enumerate(zip(chunk_texts, chunk_generated, strict=True)):
+            for i, (text, response) in enumerate(zip(chunk_texts, chunk_generated)):
                 trace_str(text, f"Text {i+1}/{len(texts)}")
                 trace_str(response, f"Generated {i+1}/{len(texts)}")
 
         return generated
 
 
 register_generator("litellm", LiteLLMGenerator)
```

### Comparing `rigging-1.1.1/rigging/generator/transformers_.py` & `rigging-1.1.2/rigging/generator/transformers_.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import gc
 import typing as t
 
 import torch
 import transformers  # type: ignore
 from transformers import AutoModelForCausalLM, AutoTokenizer, PreTrainedTokenizer, TextGenerationPipeline
 
@@ -88,15 +90,15 @@
         cls,
         model: str,
         llm: AutoModelForCausalLM,
         tokenizer: PreTrainedTokenizer,
         *,
         pipeline: TextGenerationPipeline | None = None,
         params: GenerateParams | None = None,
-    ) -> "TransformersGenerator":
+    ) -> TransformersGenerator:
         """
         Create a new instance of TransformersGenerator from an already loaded model and tokenizer.
 
         Args:
             model: The loaded model for text generation.
             tokenizer : The tokenizer associated with the model.
             pipeline: The text generation pipeline. Defaults to None.
@@ -106,19 +108,19 @@
         """
         instance = cls(model=model, params=params or GenerateParams())
         instance._llm = model
         instance._tokenizer = tokenizer
         instance._pipeline = pipeline
         return instance
 
-    def load(self) -> "TransformersGenerator":
+    def load(self) -> TransformersGenerator:
         _ = self.pipeline
         return self
 
-    def unload(self) -> "TransformersGenerator":
+    def unload(self) -> TransformersGenerator:
         del self._pipeline
         del self._llm
         del self._tokenizer
         gc.collect()
         torch.cuda.empty_cache()
         return self
 
@@ -149,15 +151,15 @@
         messages: t.Sequence[t.Sequence[Message]],
         params: t.Sequence[GenerateParams],
     ) -> t.Sequence[Message]:
         message_dicts = [[m.model_dump(include={"role", "content"}) for m in _messages] for _messages in messages]
         outputs = self._generate(message_dicts, params)
         generated = [Message(role="assistant", content=output) for output in outputs]
 
-        for i, (in_messages, out_message) in enumerate(zip(messages, generated, strict=True)):
+        for i, (in_messages, out_message) in enumerate(zip(messages, generated)):
             trace_messages(in_messages, f"Messages {i+1}/{len(in_messages)}")
             trace_messages([out_message], f"Response {i+1}/{len(in_messages)}")
 
         return generated
 
     async def agenerate_messages(
         self,
@@ -169,15 +171,15 @@
     def generate_texts(
         self,
         texts: t.Sequence[str],
         params: t.Sequence[GenerateParams],
     ) -> t.Sequence[str]:
         generated = self._generate(texts, params)
 
-        for i, (text, response) in enumerate(zip(texts, generated, strict=True)):
+        for i, (text, response) in enumerate(zip(texts, generated)):
             trace_str(text, f"Text {i+1}/{len(texts)}")
             trace_str(response, f"Generated {i+1}/{len(texts)}")
 
         return generated
 
     async def agenerate_texts(
         self,
```

### Comparing `rigging-1.1.1/rigging/generator/vllm_.py` & `rigging-1.1.2/rigging/generator/vllm_.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import gc
 import inspect
 import typing as t
 
 import torch
 import vllm
 
@@ -59,32 +61,32 @@
                 gpu_memory_utilization=self.gpu_memory_utilization,
                 enforce_eager=self.enforce_eager,
                 trust_remote_code=self.trust_remote_code,
             )
         return self._llm
 
     @classmethod
-    def from_obj(cls, model: str, llm: vllm.LLM, *, params: GenerateParams | None = None) -> "VLLMGenerator":
+    def from_obj(cls, model: str, llm: vllm.LLM, *, params: GenerateParams | None = None) -> VLLMGenerator:
         """Create a generator from an existing vLLM instance.
 
         Args:
             llm: The vLLM instance to create the generator from.
 
         Returns:
             The VLLMGenerator instance.
         """
         generator = cls(model=model, params=params or GenerateParams())
         generator._llm = llm
         return generator
 
-    def load(self) -> "VLLMGenerator":
+    def load(self) -> VLLMGenerator:
         _ = self.llm
         return self
 
-    def unload(self) -> "VLLMGenerator":
+    def unload(self) -> VLLMGenerator:
         del self._llm
         gc.collect()
         torch.cuda.empty_cache()
         return self
 
     def _generate(
         self,
@@ -123,15 +125,15 @@
         params: t.Sequence[GenerateParams],
     ) -> t.Sequence[Message]:
         message_dicts = [[m.model_dump(include={"role", "content"}) for m in _messages] for _messages in messages]
         texts = self.llm.get_tokenizer().apply_chat_template(message_dicts, add_generation_prompt=True, tokenize=False)
         outputs = self._generate(texts, params=params)
         generated = [Message(role="assistant", content=output) for output in outputs]
 
-        for i, (in_messages, out_message) in enumerate(zip(messages, generated, strict=True)):
+        for i, (in_messages, out_message) in enumerate(zip(messages, generated)):
             trace_messages(in_messages, f"Messages {i+1}/{len(in_messages)}")
             trace_messages([out_message], f"Response {i+1}/{len(in_messages)}")
 
         return generated
 
     async def agenerate_messages(
         self,
@@ -143,15 +145,15 @@
     def generate_texts(
         self,
         texts: t.Sequence[str],
         params: t.Sequence[GenerateParams],
     ) -> t.Sequence[str]:
         generated = self._generate(list(texts), params=params)
 
-        for i, (text, response) in enumerate(zip(texts, generated, strict=True)):
+        for i, (text, response) in enumerate(zip(texts, generated)):
             trace_str(text, f"Text {i+1}/{len(texts)}")
             trace_str(response, f"Generated {i+1}/{len(texts)}")
 
         return generated
 
     async def agenerate_texts(
         self,
```

### Comparing `rigging-1.1.1/rigging/logging.py` & `rigging-1.1.2/rigging/logging.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """
 We use loguru for logging. This module provides a function to configure logging handlers.
 
 To just enable rigging logs to flow, call `logger.enable("rigging")` after importing the module.
 """
 
-import pathlib
+from __future__ import annotations
+
 import sys
 import typing as t
 
 from loguru import logger
 
+if t.TYPE_CHECKING:
+    import pathlib
+
 g_configured: bool = False
 
 LogLevelList = ["trace", "debug", "info", "success", "warning", "error", "critical"]
 LogLevelLiteral = t.Literal["trace", "debug", "info", "success", "warning", "error", "critical"]
 """Valid logging levels."""
```

### Comparing `rigging-1.1.1/rigging/message.py` & `rigging-1.1.2/rigging/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 This module covers core message objects and handling.
 """
 
+from __future__ import annotations
+
 import copy
 import string
 import typing as t
 from textwrap import dedent
 from uuid import UUID, uuid4
 
 from pydantic import (
@@ -16,17 +18,19 @@
     SerializeAsAny,
     computed_field,
     field_serializer,
     field_validator,
 )
 
 from rigging.error import MissingModelError
-from rigging.model import Model, ModelT
 from rigging.parsing import try_parse_many
 
+if t.TYPE_CHECKING:
+    from rigging.model import Model, ModelT
+
 Role = t.Literal["system", "user", "assistant"]
 """The role of a message. Can be 'system', 'user', or 'assistant'."""
 
 
 # Helper type for messages structured
 # more similarly to other libraries
 class MessageDict(t.TypedDict):
@@ -162,19 +166,19 @@
             self._content = self._content[: part.slice_.start] + xml_content + self._content[part.slice_.stop :]
             part.slice_ = slice(part.slice_.start, part.slice_.start + new_length)
 
             shift += new_length - old_length
 
         self.parts = sorted(self.parts, key=lambda p: p.slice_.start)
 
-    def clone(self) -> "Message":
+    def clone(self) -> Message:
         """Creates a copy of the message."""
         return Message(self.role, self.content, parts=copy.deepcopy(self.parts))
 
-    def apply(self, **kwargs: str) -> "Message":
+    def apply(self, **kwargs: str) -> Message:
         """
         Applies the given keyword arguments with string templating to the content of the message.
 
         Uses [string.Template.safe_substitute](https://docs.python.org/3/library/string.html#string.Template.safe_substitute) underneath.
 
         Note:
             This call produces a clone of the message, leaving the original message unchanged.
@@ -320,16 +324,16 @@
         for model, slice_ in parsed:
             self._add_part(ParsedMessagePart(model=model, slice_=slice_))
         self._sync_parts()
         return [p[0] for p in parsed]
 
     @classmethod
     def from_model(
-        cls: type["Message"], models: Model | t.Sequence[Model], role: Role = "user", suffix: str | None = None
-    ) -> "Message":
+        cls: type[Message], models: Model | t.Sequence[Model], role: Role = "user", suffix: str | None = None
+    ) -> Message:
         """
         Create a Message object from one or more Model objects.
 
         Args:
             models: The Model object(s) to convert to a Message.
             role: The role of the Message.
             suffix: A suffix to append to the content.
@@ -348,28 +352,28 @@
         if suffix is not None:
             content += f"\n{suffix}"
 
         return cls(role=role, content=content, parts=parts)
 
     @classmethod
     def fit_as_list(
-        cls, messages: t.Sequence[MessageDict] | t.Sequence["Message"] | MessageDict | "Message" | str
-    ) -> list["Message"]:
+        cls, messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str
+    ) -> list[Message]:
         """Helper function to convert various common types to a strict list of Message objects."""
-        if isinstance(messages, Message | dict | str):
+        if isinstance(messages, (Message, dict, str)):
             return [cls.fit(messages)]
         return [cls.fit(message) for message in messages]
 
     @classmethod
-    def fit(cls, message: t.Union["Message", MessageDict, str]) -> "Message":
+    def fit(cls, message: t.Union[Message, MessageDict, str]) -> Message:
         """Helper function to convert various common types to a Message object."""
         if isinstance(message, str):
             return cls(role="user", content=message)
         return cls(**message) if isinstance(message, dict) else message
 
     @classmethod
-    def apply_to_list(cls, messages: t.Sequence["Message"], **kwargs: str) -> list["Message"]:
+    def apply_to_list(cls, messages: t.Sequence[Message], **kwargs: str) -> list[Message]:
         """Helper function to apply keyword arguments to a list of Message objects."""
         return [message.apply(**kwargs) for message in messages]
 
 
-Messages = t.Sequence[MessageDict] | t.Sequence[Message]
+Messages = t.Union[t.Sequence[MessageDict], t.Sequence[Message]]
```

### Comparing `rigging-1.1.1/rigging/model.py` & `rigging-1.1.2/rigging/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """
 Models are the core datatypes for structured parsing.
 """
 
+from __future__ import annotations
+
 import re
 import typing as t
 from xml.etree import ElementTree as ET
 
 from pydantic import SerializationInfo, ValidationError, create_model, field_serializer, field_validator
 from pydantic.alias_generators import to_snake
 from pydantic_xml import BaseXmlModel
 from pydantic_xml import attr as attr
 from pydantic_xml import element as element
 from pydantic_xml import wrapped as wrapped
-from pydantic_xml.element import SearchMode  # type: ignore [attr-defined]
 from pydantic_xml.typedefs import EntityLocation, NsMap
 
 from rigging.error import MissingModelError
 
+if t.TYPE_CHECKING:
+    from pydantic_xml.element import SearchMode  # type: ignore [attr-defined]
+
 #
 # Core XML serializable models for messages
 #
 
 ModelT = t.TypeVar("ModelT", bound="Model")
 
 # TODO: pydantic-xml isn't a great fit for our use case given
```

### Comparing `rigging-1.1.1/rigging/parsing.py` & `rigging-1.1.2/rigging/parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 """
 Parsing helpers for extracting rigging models from text
 """
 
+from __future__ import annotations
+
+import typing as t
+
 from rigging.error import MissingModelError
-from rigging.model import ModelT
+
+if t.TYPE_CHECKING:
+    from rigging.model import ModelT
 
 
 def parse(text: str, model_type: type[ModelT]) -> tuple[ModelT, slice]:
     """
     Parses a single model from text.
 
     Args:
```

### Comparing `rigging-1.1.1/rigging/prompt.py` & `rigging-1.1.2/rigging/prompt.py`

 * *Files identical despite different names*

### Comparing `rigging-1.1.1/rigging/tool.py` & `rigging-1.1.2/rigging/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 This module defines handles tool interaction with rigging generation.
 """
 
+from __future__ import annotations
+
 import inspect
 import typing as t
 
 from pydantic import Field, computed_field, model_validator
 from pydantic_xml import attr, element, wrapped
 
 from rigging.model import Model
 
-SUPPORTED_TOOL_ARGUMENT_TYPES = int | float | str | bool
+SUPPORTED_TOOL_ARGUMENT_TYPES = t.Union[int, float, str, bool]
 """Supported types for tool arguments."""
 
 SUPPORTED_TOOL_ARGUMENT_TYPES_LIST = [int, float, str, bool]
 """Supported types for tool arguments as a list."""
 
 ToolArgumentTypesCast = {
     "int": int,
@@ -36,15 +38,15 @@
 
     @computed_field  # type: ignore[misc]
     @property
     def value(self) -> SUPPORTED_TOOL_ARGUMENT_TYPES:
         return self.attr_value or self.text_value or ""
 
     @model_validator(mode="after")
-    def validate_value(self) -> "ToolCallParameter":
+    def validate_value(self) -> ToolCallParameter:
         if self.value is None:
             raise ValueError("Missing parameter value")
         return self
 
 
 class ToolCall(Model, tag="call"):
     tool: str = attr()
@@ -70,20 +72,20 @@
     @classmethod
     def xml_example(cls) -> str:
         return cls(
             calls=[
                 ToolCall(
                     tool="$TOOL_A",
                     function="$FUNCTION_A",
-                    parameters=[ToolCallParameter(name="$PARAMETER_NAME", value="$PARAMETER_VALUE")],
+                    parameters=[ToolCallParameter(name="$PARAMETER_NAME", text_value="$PARAMETER_VALUE")],
                 ),
                 ToolCall(
                     tool="$TOOL_B",
                     function="$FUNCTION_B",
-                    parameters=[ToolCallParameter(name="$PARAMETER_NAME", value="$PARAMETER_VALUE")],
+                    parameters=[ToolCallParameter(name="$PARAMETER_NAME", text_value="$PARAMETER_VALUE")],
                 ),
             ]
         ).to_pretty_xml()
 
 
 #
 # 3 - Outbound models from functions -> LLM
```

### Comparing `rigging-1.1.1/PKG-INFO` & `rigging-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: rigging
-Version: 1.1.1
+Version: 1.1.2
 Summary: LLM Interaction Framework
 Home-page: https://github.com/dreadnode/rigging
 License: MIT
 Author: Nick Landers
 Author-email: monoxgas@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
+Provides-Extra: examples
 Requires-Dist: accelerate (>=0.30.1,<0.31.0) ; extra == "all"
+Requires-Dist: asyncssh (==2.14.2) ; extra == "examples" or extra == "all"
+Requires-Dist: eval-type-backport (>=0.2.0,<0.3.0)
 Requires-Dist: litellm (==1.35.21)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
-Requires-Dist: pydantic (==2.5.3)
-Requires-Dist: pydantic-xml (==2.7.0)
+Requires-Dist: pydantic (==2.6.1)
+Requires-Dist: pydantic-xml (==2.11.0)
 Requires-Dist: transformers (>=4.41.0,<5.0.0) ; extra == "all"
+Requires-Dist: types-requests (==2.32.0.20240523) ; extra == "examples" or extra == "all"
 Requires-Dist: vllm (==0.4.2) ; extra == "all"
 Project-URL: Repository, https://github.com/dreadnode/rigging
 Description-Content-Type: text/markdown
 
 # Rigging
 
 Rigging is a lightweight LLM interaction framework built on Pydantic XML. The goal is to make leveraging LLMs in production pipelines as simple and effictive as possible. Here are the highlights:
```

