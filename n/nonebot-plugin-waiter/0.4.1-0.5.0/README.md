# Comparing `tmp/nonebot_plugin_waiter-0.4.1.tar.gz` & `tmp/nonebot_plugin_waiter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_waiter-0.4.1.tar", last modified: Tue May  7 18:09:22 2024, max compression
+gzip compressed data, was "nonebot_plugin_waiter-0.5.0.tar", last modified: Fri May 24 08:46:18 2024, max compression
```

## Comparing `nonebot_plugin_waiter-0.4.1.tar` & `nonebot_plugin_waiter-0.5.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3901 2024-05-07 18:08:35.670728 nonebot_plugin_waiter-0.4.1/README.md
--rw-r--r--   0        0        0     1387 2024-05-07 18:09:22.897737 nonebot_plugin_waiter-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     7769 2024-05-07 18:08:35.679727 nonebot_plugin_waiter-0.4.1/src/nonebot_plugin_waiter/__init__.py
--rw-r--r--   0        0        0      177 2024-03-24 06:49:37.131645 nonebot_plugin_waiter-0.4.1/src/nonebot_plugin_waiter/config.py
--rw-r--r--   0        0        0     4025 1970-01-01 00:00:00.000000 nonebot_plugin_waiter-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4979 2024-05-24 08:44:11.872144 nonebot_plugin_waiter-0.5.0/README.md
+-rw-r--r--   0        0        0     1387 2024-05-24 08:46:18.359299 nonebot_plugin_waiter-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9825 2024-05-24 08:44:17.978654 nonebot_plugin_waiter-0.5.0/src/nonebot_plugin_waiter/__init__.py
+-rw-r--r--   0        0        0      318 2024-05-24 08:44:17.915515 nonebot_plugin_waiter-0.5.0/src/nonebot_plugin_waiter/config.py
+-rw-r--r--   0        0        0     5067 1970-01-01 00:00:00.000000 nonebot_plugin_waiter-0.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_waiter-0.4.1/README.md` & `nonebot_plugin_waiter-0.5.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -41,25 +41,33 @@
 
 可直接用 `Waiter.wait` 等待函数返回结果：
 
 ```python
 resp = await check.wait(timeout=60, default=False)
 ```
 
+参数：
+
+- before: 等待前发送的消息
+- default: 超时时返回的默认值
+- timeout: 等待超时时间
+
 或使用异步迭代器持续等待，直到满足结果才退出循环。适合多轮对话：
 
 ```python
 async for resp in check(timeout=60, default=False):
     ...
 ```
 
 参数：
 
 - default: 超时时返回的默认值
 - timeout: 等待超时时间
+- retry: 重试次数，不设置则无限重试
+- prompt: 重试时发送的消息，若没有设置 `retry` 则不发送
 
 ### 便捷函数
 
 插件提供了一个 `prompt` 函数用于直接等待用户输入，适用于等待用户输入文本消息：
 
 ```python
 from nonebot_plugin_waiter import prompt
@@ -82,23 +90,51 @@
 async def _():
     await test.send("请输入数字")
 
     @waiter(waits=["message"], keep_session=True)
     async def check(event: Event):
         return event.get_plaintext()
 
-    async for resp in check(timeout=60):
+    resp = await check.wait(timeout=60)
+    if resp is None:
+        await test.send("等待超时")
+        return
+    if not resp.isdigit():
+        await test.send("无效输入")
+        return
+    await test.finish(f"你输入了{resp}")
+```
+
+等待用户输入数字，超时时间为 30 秒，只允许重试 5 次，此时 waits 接收所有来自当前用户的消息事件。
+
+```python
+from nonebot import on_command
+from nonebot.adapters import Event
+from nonebot_plugin_waiter import waiter
+
+test = on_command("test")
+
+@test.handle()
+async def _():
+    await test.send("请输入数字")
+
+    @waiter(waits=["message"], keep_session=True)
+    async def check(event: Event):
+        return event.get_plaintext()
+
+    async for resp in check(timeout=30, retry=5, prompt="输入错误，请输入数字。剩余次数：{count}"):
         if resp is None:
             await test.send("等待超时")
             break
         if not resp.isdigit():
-            await test.send("请输入数字")
             continue
         await test.send(f"你输入了{resp}")
         break
+    else:
+        await test.send("输入失败")
 ```
 
 在 telegram 适配器下等待用户点击按钮，超时时间为 30 秒，此时 waits 接收 telegram 的 CallbackQueryEvent 事件。
 
 ```python
 from nonebot import on, on_command
 from nonebot.adapters.telegram import Bot
```

### Comparing `nonebot_plugin_waiter-0.4.1/pyproject.toml` & `nonebot_plugin_waiter-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-waiter"
-version = "0.4.1"
+version = "0.5.0"
 description = "An alternative for got-and-reject in Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "3165388245@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.3.0",
 ]
```

### Comparing `nonebot_plugin_waiter-0.4.1/src/nonebot_plugin_waiter/__init__.py` & `nonebot_plugin_waiter-0.5.0/src/nonebot_plugin_waiter/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from nonebot.typing import T_State, _DependentCallable
 from nonebot.internal.permission import User, Permission
 from nonebot.internal.matcher import current_event, current_matcher
 from nonebot.internal.adapter import Bot, Event, Message, MessageSegment, MessageTemplate
 
 from .config import Config
 
-__version__ = "0.4.1"
+__version__ = "0.5.0"
 
 __plugin_meta__ = PluginMetadata(
     name="Waiter 插件",
     description="提供一个 got-and-reject 会话控制的替代方案，可自由控制超时时间",
     usage="@waiter(waits: list[type[Event] | str], matcher: type[Matcher] | Matcher, parameterless: Iterable[Any] | None, keep_session: bool = False)",  # noqa: E501
     homepage="https://github.com/RF-Tar-Railt/nonebot-plugin-waiter",
     type="library",
@@ -39,30 +39,54 @@
 R = TypeVar("R")
 R1 = TypeVar("R1")
 T = TypeVar("T")
 T1 = TypeVar("T1")
 
 
 class WaiterIterator(Generic[R, T]):
-    def __init__(self, waiter: Waiter[R], default: T, timeout: float = plugin_config.waiter_timeout):
+    def __init__(
+        self,
+        waiter: Waiter[R],
+        default: T,
+        timeout: float = plugin_config.waiter_timeout,
+        retry: int | None = None,
+        msg: Message | MessageTemplate = MessageTemplate(plugin_config.waiter_retry_prompt),
+    ):
         self.waiter = waiter
         self.timeout = timeout
         self.default = default
+        self.retry = retry
+        self.msg = msg
+        self._next_count = 0
 
     def __aiter__(self) -> Self:
         return self
 
     @overload
     def __anext__(self: WaiterIterator[R1, None]) -> Awaitable[R1 | None]: ...
 
     @overload
     def __anext__(self: WaiterIterator[R1, T1]) -> Awaitable[R1 | T1]: ...
 
     def __anext__(self):  # type: ignore
-        return self.waiter.wait(default=self.default, timeout=self.timeout)  # type: ignore
+        if self.retry is None:
+            return self.waiter.wait(default=self.default, timeout=self.timeout)
+        msg = None
+        if self._next_count > 0:
+            self.retry -= 1
+            if self.retry < 0:
+                raise StopAsyncIteration
+            if isinstance(self.msg, MessageTemplate):
+                msg = self.msg.format(count=f"{self.retry + 1}")
+            else:
+                msg = self.msg
+        try:
+            return self.waiter.wait(msg, default=self.default, timeout=self.timeout)
+        finally:
+            self._next_count += 1
 
 
 class Waiter(Generic[R]):
     future: asyncio.Future
     handler: _DependentCallable[R]
 
     def __init__(
@@ -90,15 +114,15 @@
             if event_types and not isinstance(event, event_types):
                 matcher.skip()
             if event_str_types and event.get_type() not in event_str_types:
                 matcher.skip()
             if self.future.done():
                 matcher.skip()
             result = await _handler(
-                matcher=self,
+                matcher=matcher,
                 bot=bot,
                 event=event,
                 state=state,
             )
             if result is not None and not self.future.done():
                 self.future.set_result(result)
                 matcher.stop_propagation()
@@ -114,43 +138,94 @@
 
     @overload
     def __call__(self, *, default: T, timeout: float = 120) -> WaiterIterator[R, T]: ...
 
     @overload
     def __call__(self, *, timeout: float = 120) -> WaiterIterator[R, None]: ...
 
+    @overload
+    def __call__(
+        self,
+        *,
+        retry: int,
+        timeout: float = 120,
+        prompt: str | Message | MessageSegment | MessageTemplate = "",
+    ) -> WaiterIterator[R, None]: ...
+
+    @overload
     def __call__(
-        self, *, default: T | None = None, timeout: float = plugin_config.waiter_timeout
+        self,
+        *,
+        retry: int,
+        default: T,
+        timeout: float = 120,
+        prompt: str | Message | MessageSegment | MessageTemplate = "",
+    ) -> WaiterIterator[R, T]: ...
+
+    def __call__(
+        self,
+        *,
+        default: T | None = None,
+        timeout: float = plugin_config.waiter_timeout,
+        retry: int | None = None,
+        prompt: str | Message | MessageSegment | MessageTemplate = plugin_config.waiter_retry_prompt,
     ) -> WaiterIterator[R, T] | WaiterIterator[R, None]:
-        """等待用户输入并返回结果
+        """循环等待用户输入并返回结果，可以设置重试次数来限制循环次数
 
         参数:
             default: 超时时返回的默认值
             timeout: 等待超时时间
+            retry:   重试次数
+            prompt:  重试的提示消息
         """
-        return WaiterIterator(self, default, timeout)  # type: ignore
+        if isinstance(prompt, str):
+            msg = MessageTemplate(prompt)
+        elif isinstance(prompt, MessageSegment):
+            msg = prompt.get_message_class()(prompt)
+        else:
+            msg = prompt
+
+        return WaiterIterator(self, default, timeout, retry, msg)  # type: ignore
 
     @overload
-    async def wait(self, *, default: R | T, timeout: float = plugin_config.waiter_timeout) -> R | T: ...
+    async def wait(
+        self,
+        before: str | Message | MessageSegment | MessageTemplate | None = None,
+        *,
+        default: R | T,
+        timeout: float = plugin_config.waiter_timeout,
+    ) -> R | T: ...
 
     @overload
-    async def wait(self, *, timeout: float = plugin_config.waiter_timeout) -> R | None: ...
+    async def wait(
+        self,
+        before: str | Message | MessageSegment | MessageTemplate | None = None,
+        *,
+        timeout: float = plugin_config.waiter_timeout,
+    ) -> R | None: ...
 
     async def wait(
-        self, *, default: R | T | None = None, timeout: float = plugin_config.waiter_timeout
+        self,
+        before: str | Message | MessageSegment | MessageTemplate | None = None,
+        *,
+        default: R | T | None = None,
+        timeout: float = plugin_config.waiter_timeout,
     ) -> R | T | None:
         """等待用户输入并返回结果
 
         参数:
+            before: 等待前发送的消息
             default: 超时时返回的默认值
             timeout: 等待超时时间
         """
         matcher = on(
             type=self.event_type, permission=self.permission, priority=0, block=False, handlers=[self.handler]
         )
+        if before:
+            await matcher.send(before)
         try:
             return await asyncio.wait_for(self.future, timeout)
         except asyncio.TimeoutError:
             return default
         finally:
             self.future = asyncio.Future()
             try:
@@ -203,20 +278,14 @@
 ) -> Message | None:
     """等待用户输入并返回结果
 
     参数:
         message: 提示消息
         timeout: 等待超时时间
     """
-    try:
-        matcher = current_matcher.get()
-    except LookupError:
-        raise RuntimeError("No matcher found.")
-
-    await matcher.send(message)
 
     async def wrapper(event: Event):
         return event.get_message()
 
     wrapper.__annotations__ = {"event": Event}
 
-    return await waiter(["message"], matcher=matcher, keep_session=True)(wrapper).wait(timeout=timeout)
+    return await waiter(["message"], keep_session=True)(wrapper).wait(message, timeout=timeout)
```

### Comparing `nonebot_plugin_waiter-0.4.1/PKG-INFO` & `nonebot_plugin_waiter-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-waiter
-Version: 0.4.1
+Version: 0.5.0
 Summary: An alternative for got-and-reject in Nonebot
 Author-Email: RF-Tar-Railt <3165388245@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: nonebot2>=2.3.0
 Description-Content-Type: text/markdown
 
@@ -51,25 +51,33 @@
 
 可直接用 `Waiter.wait` 等待函数返回结果：
 
 ```python
 resp = await check.wait(timeout=60, default=False)
 ```
 
+参数：
+
+- before: 等待前发送的消息
+- default: 超时时返回的默认值
+- timeout: 等待超时时间
+
 或使用异步迭代器持续等待，直到满足结果才退出循环。适合多轮对话：
 
 ```python
 async for resp in check(timeout=60, default=False):
     ...
 ```
 
 参数：
 
 - default: 超时时返回的默认值
 - timeout: 等待超时时间
+- retry: 重试次数，不设置则无限重试
+- prompt: 重试时发送的消息，若没有设置 `retry` 则不发送
 
 ### 便捷函数
 
 插件提供了一个 `prompt` 函数用于直接等待用户输入，适用于等待用户输入文本消息：
 
 ```python
 from nonebot_plugin_waiter import prompt
@@ -92,23 +100,51 @@
 async def _():
     await test.send("请输入数字")
 
     @waiter(waits=["message"], keep_session=True)
     async def check(event: Event):
         return event.get_plaintext()
 
-    async for resp in check(timeout=60):
+    resp = await check.wait(timeout=60)
+    if resp is None:
+        await test.send("等待超时")
+        return
+    if not resp.isdigit():
+        await test.send("无效输入")
+        return
+    await test.finish(f"你输入了{resp}")
+```
+
+等待用户输入数字，超时时间为 30 秒，只允许重试 5 次，此时 waits 接收所有来自当前用户的消息事件。
+
+```python
+from nonebot import on_command
+from nonebot.adapters import Event
+from nonebot_plugin_waiter import waiter
+
+test = on_command("test")
+
+@test.handle()
+async def _():
+    await test.send("请输入数字")
+
+    @waiter(waits=["message"], keep_session=True)
+    async def check(event: Event):
+        return event.get_plaintext()
+
+    async for resp in check(timeout=30, retry=5, prompt="输入错误，请输入数字。剩余次数：{count}"):
         if resp is None:
             await test.send("等待超时")
             break
         if not resp.isdigit():
-            await test.send("请输入数字")
             continue
         await test.send(f"你输入了{resp}")
         break
+    else:
+        await test.send("输入失败")
 ```
 
 在 telegram 适配器下等待用户点击按钮，超时时间为 30 秒，此时 waits 接收 telegram 的 CallbackQueryEvent 事件。
 
 ```python
 from nonebot import on, on_command
 from nonebot.adapters.telegram import Bot
```

