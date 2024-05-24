# Comparing `tmp/python_115-0.0.8.1.tar.gz` & `tmp/python_115-0.0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.1.tar", max compression
+gzip compressed data, was "python_115-0.0.8.2.tar", max compression
```

## Comparing `python_115-0.0.8.1.tar` & `python_115-0.0.8.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.1/LICENSE
--rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.1/p115/__init__.py
--rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.1/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.1/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.1/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8.1/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.1/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.1/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.1/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.1/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.1/p115/component/cipher.py
--rwxr-xr-x   0        0        0   241090 2024-05-23 16:00:08.933463 python_115-0.0.8.1/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.1/p115/component/exception.py
--rwxr-xr-x   0        0        0    56840 2024-05-23 15:52:16.591932 python_115-0.0.8.1/p115/component/fs.py
--rwxr-xr-x   0        0        0    48067 2024-05-22 14:42:11.490047 python_115-0.0.8.1/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    12217 2024-05-23 16:03:44.547969 python_115-0.0.8.1/p115/component/fs_share.py
--rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.1/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     4816 2024-05-22 14:03:48.259741 python_115-0.0.8.1/p115/component/labellist.py
--rwxr-xr-x   0        0        0     7086 2024-05-22 14:03:58.992780 python_115-0.0.8.1/p115/component/offline.py
--rwxr-xr-x   0        0        0     3877 2024-05-22 14:04:09.272894 python_115-0.0.8.1/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     4950 2024-05-22 14:04:19.641910 python_115-0.0.8.1/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.1/p115/py.typed
--rwxr-xr-x   0        0        0     3217 2024-05-09 09:59:33.438651 python_115-0.0.8.1/p115/tool/__init__.py
--rw-r--r--   0        0        0     1593 2024-05-23 16:05:10.412650 python_115-0.0.8.1/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.1/readme.md
--rw-r--r--   0        0        0    36272 1970-01-01 00:00:00.000000 python_115-0.0.8.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.2/LICENSE
+-rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.2/p115/__init__.py
+-rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.2/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.2/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.2/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8.2/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.2/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.2/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.2/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.2/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   245406 2024-05-24 10:28:17.844082 python_115-0.0.8.2/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.2/p115/component/exception.py
+-rwxr-xr-x   0        0        0    56840 2024-05-23 15:52:16.591932 python_115-0.0.8.2/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48067 2024-05-22 14:42:11.490047 python_115-0.0.8.2/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.2/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.2/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     4816 2024-05-22 14:03:48.259741 python_115-0.0.8.2/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     7086 2024-05-22 14:03:58.992780 python_115-0.0.8.2/p115/component/offline.py
+-rwxr-xr-x   0        0        0     3877 2024-05-22 14:04:09.272894 python_115-0.0.8.2/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     4950 2024-05-22 14:04:19.641910 python_115-0.0.8.2/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.2/p115/py.typed
+-rwxr-xr-x   0        0        0     3217 2024-05-09 09:59:33.438651 python_115-0.0.8.2/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1593 2024-05-24 10:28:42.454135 python_115-0.0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.2/readme.md
+-rw-r--r--   0        0        0    36272 1970-01-01 00:00:00.000000 python_115-0.0.8.2/PKG-INFO
```

### Comparing `python_115-0.0.8.1/LICENSE` & `python_115-0.0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/cmd/iterdir.py` & `python_115-0.0.8.2/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/cmd/qrcode.py` & `python_115-0.0.8.2/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/component/__init__.py` & `python_115-0.0.8.2/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/component/cipher.py` & `python_115-0.0.8.2/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/component/client.py` & `python_115-0.0.8.2/p115/component/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,33 +11,32 @@
 from asyncio import to_thread
 from base64 import b64encode
 from binascii import b2a_hex
 from collections.abc import (
     AsyncIterable, AsyncIterator, Awaitable, Callable, Iterable, Iterator, Mapping, Sequence, 
 )
 from concurrent.futures import Future
-from contextlib import asynccontextmanager, closing
+from contextlib import asynccontextmanager, aclosing, closing
 from datetime import date, datetime
 from email.utils import formatdate
 from functools import cached_property, partial, update_wrapper
 from hashlib import md5, sha1
 from hmac import digest as hmac_digest
 from http.cookiejar import Cookie
 from http.cookies import Morsel
-from inspect import isawaitable, iscoroutinefunction
-from io import UnsupportedOperation
+from inspect import iscoroutinefunction
 from itertools import count, takewhile
 from json import dumps, loads
 from os import fsdecode, fstat, stat, PathLike
 from os import path as ospath
 from re import compile as re_compile
 from threading import Condition, Thread
 from time import sleep, strftime, strptime, time
 from typing import (
-    cast, overload, Any, Final, Literal, Never, Optional, Self, TypeVar, 
+    cast, overload, Any, Final, Literal, Never, Self, TypeVar, 
 )
 from urllib.parse import quote, urlencode, urlsplit
 from uuid import uuid4
 from xml.etree.ElementTree import fromstring
 
 from asynctools import as_thread, ensure_aiter, ensure_async
 from cookietools import cookies_str_to_dict, create_cookie
@@ -4251,15 +4250,15 @@
         file: ( bytes | bytearray | memoryview | 
                 SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
                 Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
                 AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
         bucket: str, 
         object: str, 
         callback: dict, 
-        token: Optional[dict], 
+        token: None | dict, 
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> dict:
         ...
     @overload
     def _oss_upload(
         self, 
@@ -4267,30 +4266,30 @@
         file: ( bytes | bytearray | memoryview | 
                 SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
                 Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
                 AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
         bucket: str, 
         object: str, 
         callback: dict, 
-        token: Optional[dict], 
+        token: None | dict, 
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def _oss_upload(
         self, 
         /, 
         file: ( bytes | bytearray | memoryview | 
                 SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
                 Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
                 AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
         bucket: str, 
         object: str, 
         callback: dict, 
-        token: Optional[dict] = None, 
+        token: None | dict = None, 
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """帮助函数：上传文件到阿里云 OSS，一次上传全部（即不进行分片）
         """
         url = self.upload_endpoint_url(bucket, object)
         if isinstance(file, (bytes, bytearray, memoryview)):
@@ -4362,15 +4361,15 @@
         file: ( bytes | bytearray | memoryview | 
                 SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
                 Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
                 AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
         bucket: str, 
         object: str, 
         callback: dict, 
-        token: Optional[dict], 
+        token: None | dict, 
         upload_id: None | str, 
         part_size: int, 
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> dict:
         ...
     @overload
@@ -4380,15 +4379,15 @@
         file: ( bytes | bytearray | memoryview | 
                 SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
                 Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
                 AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
         bucket: str, 
         object: str, 
         callback: dict, 
-        token: Optional[dict], 
+        token: None | dict, 
         upload_id: None | str, 
         part_size: int, 
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def _oss_multipart_upload(
@@ -4397,15 +4396,15 @@
         file: ( bytes | bytearray | memoryview | 
                 SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
                 Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
                 AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
         bucket: str, 
         object: str, 
         callback: dict, 
-        token: Optional[dict] = None, 
+        token: None | dict = None, 
         upload_id: None | str = None, 
         part_size: int = 10 * 1 << 20, # default to: 10 MB
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         url = self.upload_endpoint_url(bucket, object)
         parts: list[dict] = []
@@ -6719,43 +6718,44 @@
         api = "https://webapi.115.com/user/captcha"
         request_kwargs.pop("parse", None)
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     ########## Other Encapsulations ##########
 
     # TODO: 支持 async_
+    # TODO: 使用 HTTPXFileReader
     @overload
     def open(
         self, 
         /, 
         url: str | Callable[[], str], 
-        headers: Optional[Mapping], 
+        headers: None | Mapping, 
         start: int, 
         seek_threshold: int,
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> RequestsFileReader:
         ...
     @overload
     def open(
         self, 
         /, 
         url: str | Callable[[], str], 
-        headers: Optional[Mapping], 
+        headers: None | Mapping, 
         start: int, 
         seek_threshold: int,
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[RequestsFileReader]:
         ...
     def open(
         self, 
         /, 
         url: str | Callable[[], str], 
-        headers: Optional[Mapping] = None, 
+        headers: None | Mapping = None, 
         start: int = 0, 
         seek_threshold: int = 1 << 20,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> RequestsFileReader | Awaitable[RequestsFileReader]:
         """
         """
@@ -6769,216 +6769,289 @@
             seek_threshold=seek_threshold, 
             urlopen=urlopen, 
         )
 
     # TODO: 返回一个 HTTPFileWriter，随时可以写入一些数据，close 代表上传完成，这个对象会持有一些信息
     def open_upload(self): ...
 
-    # TODO: 下面 3 个函数支持 async_
     @overload
     def read_bytes(
         self, 
         /, 
         url: str, 
         start: int = 0, 
-        stop: Optional[int] = None, 
-        headers: Optional[Mapping] = None,
+        stop: None | int = None, 
+        headers: None | Mapping = None,
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> bytes:
         ...
     @overload
     def read_bytes(
         self, 
         /, 
         url: str, 
         start: int, 
-        stop: Optional[int], 
-        headers: Optional[Mapping],
+        stop: None | int, 
+        headers: None | Mapping,
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[bytes]:
         ...
     def read_bytes(
         self, 
         /, 
         url: str, 
         start: int = 0, 
-        stop: Optional[int] = None, 
-        headers: Optional[Mapping] = None,
+        stop: None | int = None, 
+        headers: None | Mapping = None,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> bytes | Awaitable[bytes]:
-        """
-        """
-        length = None
-        if start < 0:
-            with closing(self.request(url, stream=True, headers={"Accept-Encoding": "identity"})) as resp:
-                resp.raise_for_status()
-                length = get_content_length(resp)
-            if length is None:
-                raise OSError(errno.ESPIPE, "can't determine content length")
-            start += length
-        if start < 0:
-            start = 0
-        if stop is None:
-            bytes_range = f"{start}-"
-        else:
-            if stop < 0:
-                if length is None:
-                    with closing(self.request(url, stream=True, headers={"Accept-Encoding": "identity"})) as resp:
+        """读取文件一定索引范围的数据
+        :param url: 115 文件的下载链接（可以从网盘、网盘上的压缩包内、分享链接中获取）
+        :param start: 开始索引，可以为负数（从文件尾部开始）
+        :param stop: 结束索引（不含），可以为负数（从文件尾部开始）
+        :param headers: 一些请求头，最好提供一个 "User-Agent"
+        :param async_: 是否异步
+        :param request_kwargs: 其它请求参数
+        """
+        need_get_length = start < 0 or (stop and stop < 0)
+        if need_get_length:
+            if headers:
+                headers = {**headers, "Accept-Encoding": "identity"}
+            else:
+                headers = {"Accept-Encoding": "identity"}
+        request_kwargs["headers"] = headers
+        if async_:
+            async def get_bytes_range_async(start, stop) -> str:
+                if need_get_length:
+                    async with aclosing(self.request(url, async_=async_, **request_kwargs)) as resp:
+                        resp.raise_for_status()
+                        length = get_total_length(resp)
+                    if length is None:
+                        raise OSError(errno.ESPIPE, "can't determine content length")
+                    if start < 0:
+                        start += length
+                    if start < 0:
+                        start = 0
+                    if stop is None:
+                        return f"{start}-"
+                    elif stop < 0:
+                        stop += length
+                if stop <= 0 or start >= stop:
+                    return ""
+                return f"{start}-{stop-1}"
+            async def async_request():
+                bytes_range = await get_bytes_range_async(start, stop)
+                if not bytes_range:
+                    return b""
+                return await self.read_bytes_range(url, bytes_range, async_=async_, **request_kwargs)
+            return async_request()
+        else:
+            def get_bytes_range(start, stop) -> str:
+                if need_get_length:
+                    with closing(self.request(url, async_=async_, **request_kwargs)) as resp:
                         resp.raise_for_status()
                         length = get_content_length(resp)
-                if length is None:
-                    raise OSError(errno.ESPIPE, "can't determine content length")
-                stop += length
-            if stop <= 0 or start >= stop:
+                    if length is None:
+                        raise OSError(errno.ESPIPE, "can't determine content length")
+                    if start < 0:
+                        start += length
+                    if start < 0:
+                        start = 0
+                    if stop is None:
+                        return f"{start}-"
+                    elif stop < 0:
+                        stop += length
+                if stop <= 0 or start >= stop:
+                    return ""
+                return f"{start}-{stop-1}"
+            bytes_range = get_bytes_range(start, stop)
+            if not bytes_range:
                 return b""
-            bytes_range = f"{start}-{stop-1}"
-        return self.read_bytes_range(url, bytes_range, headers=headers, **request_kwargs)
+            return self.read_bytes_range(url, bytes_range, async_=async_, **request_kwargs)
 
     @overload
     def read_bytes_range(
         self, 
         /, 
         url: str, 
         bytes_range: str = "0-", 
-        headers: Optional[Mapping] = None,
+        headers: None | Mapping = None,
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> bytes:
         ...
     @overload
     def read_bytes_range(
         self, 
         /, 
         url: str, 
         bytes_range: str, 
-        headers: Optional[Mapping],
+        headers: None | Mapping,
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[bytes]:
         ...
     def read_bytes_range(
         self, 
         /, 
         url: str, 
         bytes_range: str = "0-", 
-        headers: Optional[Mapping] = None,
+        headers: None | Mapping = None,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> bytes | Awaitable[bytes]:
-        """
+        """读取文件一定索引范围的数据
+        :param url: 115 文件的下载链接（可以从网盘、网盘上的压缩包内、分享链接中获取）
+        :param bytes_range: 索引范围，语法符合 [HTTP Range Requests](https://developer.mozilla.org/en-US/docs/Web/HTTP/Range_requests)
+        :param headers: 一些请求头，最好提供一个 "User-Agent"
+        :param async_: 是否异步
+        :param request_kwargs: 其它请求参数
         """
         if headers:
             headers = {**headers, "Accept-Encoding": "identity", "Range": f"bytes={bytes_range}"}
         else:
             headers = {"Accept-Encoding": "identity", "Range": f"bytes={bytes_range}"}
-        request_kwargs["stream"] = False
-        with closing(self.request(url, headers=headers, async_=async_, **request_kwargs)) as resp:
-            if resp.status_code == 416:
-                return b""
-            resp.raise_for_status()
-            return resp.content
+        request_kwargs["headers"] = headers
+        request_kwargs["parse"] = None
+        request_kwargs["raise_for_status"] = False
+        if async_:
+            async def async_request():
+                async with aclosing(self.request(url, async_=async_, **request_kwargs)) as resp:
+                    if resp.status_code == 416:
+                        return b""
+                    resp.raise_for_status()
+                    return await resp.read()
+            return async_request()
+        else:
+            with closing(self.request(url, async_=async_, **request_kwargs)) as resp:
+                if resp.status_code == 416:
+                    return b""
+                resp.raise_for_status()
+                return resp.read()
 
     @overload
     def read_block(
         self, 
         /, 
         url: str, 
         size: int = 0, 
         offset: int = 0, 
-        headers: Optional[Mapping] = None,
+        headers: None | Mapping = None,
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> bytes:
         ...
     @overload
     def read_block(
         self, 
         /, 
         url: str, 
         size: int, 
         offset: int, 
-        headers: Optional[Mapping],
+        headers: None | Mapping,
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[bytes]:
         ...
     def read_block(
         self, 
         /, 
         url: str, 
         size: int = 0, 
         offset: int = 0, 
-        headers: Optional[Mapping] = None,
+        headers: None | Mapping = None,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> bytes | Awaitable[bytes]:
-        """
+        """读取文件一定索引范围的数据
+        :param url: 115 文件的下载链接（可以从网盘、网盘上的压缩包内、分享链接中获取）
+        :param size: 下载字节数（最多下载这么多字节，如果遇到 EOF，就可能较小）
+        :param offset: 偏移索引，从 0 开始，可以为负数（从文件尾部开始）
+        :param headers: 一些请求头，最好提供一个 "User-Agent"
+        :param async_: 是否异步
+        :param request_kwargs: 其它请求参数
         """
         if size <= 0:
             return b""
-        return self.read_bytes(url, offset, offset+size, headers=headers, **request_kwargs)
+        return self.read_bytes(
+            url, 
+            offset, 
+            offset+size, 
+            headers=headers, 
+            async_=async_, 
+            **request_kwargs, 
+        )
 
     @cached_property
     def fs(self, /) -> P115FileSystem:
-        """
+        """你的网盘的文件列表的封装对象
         """
         return P115FileSystem(self)
 
     def get_fs(self, /, *args, **kwargs) -> P115FileSystem:
-        """
+        """新建你的网盘的文件列表的封装对象
         """
         return P115FileSystem(self, *args, **kwargs)
 
     def get_share_fs(self, share_link: str, /, *args, **kwargs) -> P115ShareFileSystem:
-        """
+        """新建一个分享链接的文件列表的封装对象
         """
         return P115ShareFileSystem(self, share_link, *args, **kwargs)
 
     def get_zip_fs(self, id_or_pickcode: int | str, /, *args, **kwargs) -> P115ZipFileSystem:
-        """
+        """新建压缩文件（支持 zip、rar、7z）的文件列表的封装对象（这个压缩文件在你的网盘中，且已经被云解压）
+
+        https://vip.115.com/?ct=info&ac=information
+        云解压预览规则：
+        1. 支持rar、zip、7z类型的压缩包云解压，其他类型的压缩包暂不支持；
+        2. 支持云解压20GB以下的压缩包；
+        3. 暂不支持分卷压缩包类型进行云解压，如rar.part等；
+        4. 暂不支持有密码的压缩包进行在线预览。
         """
         return P115ZipFileSystem(self, id_or_pickcode, *args, **kwargs)
 
     @cached_property
     def label(self, /) -> P115LabelList:
-        """
+        """你的标签列表的封装对象（标签是给文件或文件夹做标记的）
         """
         return P115LabelList(self)
 
     @cached_property
     def offline(self, /) -> P115Offline:
-        """
+        """你的离线任务列表的封装对象
         """
         return P115Offline(self)
 
     def get_offline(self, /, *args, **kwargs) -> P115Offline:
+        """新建你的离线任务列表的封装对象
+        """
         return P115Offline(self, *args, **kwargs)
 
     @cached_property
     def recyclebin(self, /) -> P115Recyclebin:
-        """
+        """你的回收站的封装对象
         """
         return P115Recyclebin(self)
 
     def get_recyclebin(self, /, *args, **kwargs) -> P115Recyclebin:
-        """
+        """新建你的回收站的封装对象
         """
         return P115Recyclebin(self, *args, **kwargs)
 
     @cached_property
     def sharing(self, /) -> P115Sharing:
-        """
+        """你的分享列表的封装对象
         """
         return P115Sharing(self)
 
     def get_sharing(self, /, *args, **kwargs) -> P115Sharing:
-        """
+        """新建你的分享列表的封装对象
         """
         return P115Sharing(self, *args, **kwargs)
 
 
 # TODO: 这些类再提供一个 Async 版本
 class ExportDirStatus(Future):
     _condition: Condition
```

### Comparing `python_115-0.0.8.1/p115/component/fs.py` & `python_115-0.0.8.2/p115/component/fs.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/component/fs_base.py` & `python_115-0.0.8.2/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/component/fs_share.py` & `python_115-0.0.8.2/p115/component/fs_share.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from posixpatht import escape, joins
 
 from .client import check_response, P115Client
 from .fs_base import AttrDict, IDOrPathType, P115PathBase, P115FileSystemBase
 
 
-CRE_SHARE_LINK_search = re_compile(r"/s/(?P<share_code>\w+)(\?password=(?P<receive_code>\w+))?").search
+CRE_SHARE_LINK_search = re_compile(r"(?:/s/|share\.115\.com/)(?P<share_code>[a-z0-9]+)(\?password=(?P<receive_code>\w+))?").search
 
 
 def normalize_info(
     info: Mapping, 
     keep_raw: bool = False, 
     **extra_data, 
 ) -> dict:
```

### Comparing `python_115-0.0.8.1/p115/component/fs_zip.py` & `python_115-0.0.8.2/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/component/labellist.py` & `python_115-0.0.8.2/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/component/offline.py` & `python_115-0.0.8.2/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/component/recyclebin.py` & `python_115-0.0.8.2/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/component/sharing.py` & `python_115-0.0.8.2/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/p115/tool/__init__.py` & `python_115-0.0.8.2/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/pyproject.toml` & `python_115-0.0.8.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.1"
+version = "0.0.8.2"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.1/readme.md` & `python_115-0.0.8.2/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.1/PKG-INFO` & `python_115-0.0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.1
+Version: 0.0.8.2
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

