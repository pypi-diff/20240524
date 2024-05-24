# Comparing `tmp/python_115-0.0.8.2.tar.gz` & `tmp/python_115-0.0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.2.tar", max compression
+gzip compressed data, was "python_115-0.0.8.3.tar", max compression
```

## Comparing `python_115-0.0.8.2.tar` & `python_115-0.0.8.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.2/LICENSE
--rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.2/p115/__init__.py
--rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.2/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.2/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.2/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8.2/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.2/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.2/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.2/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.2/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.2/p115/component/cipher.py
--rwxr-xr-x   0        0        0   245406 2024-05-24 10:28:17.844082 python_115-0.0.8.2/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.2/p115/component/exception.py
--rwxr-xr-x   0        0        0    56840 2024-05-23 15:52:16.591932 python_115-0.0.8.2/p115/component/fs.py
--rwxr-xr-x   0        0        0    48067 2024-05-22 14:42:11.490047 python_115-0.0.8.2/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.2/p115/component/fs_share.py
--rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.2/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     4816 2024-05-22 14:03:48.259741 python_115-0.0.8.2/p115/component/labellist.py
--rwxr-xr-x   0        0        0     7086 2024-05-22 14:03:58.992780 python_115-0.0.8.2/p115/component/offline.py
--rwxr-xr-x   0        0        0     3877 2024-05-22 14:04:09.272894 python_115-0.0.8.2/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     4950 2024-05-22 14:04:19.641910 python_115-0.0.8.2/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.2/p115/py.typed
--rwxr-xr-x   0        0        0     3217 2024-05-09 09:59:33.438651 python_115-0.0.8.2/p115/tool/__init__.py
--rw-r--r--   0        0        0     1593 2024-05-24 10:28:42.454135 python_115-0.0.8.2/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.2/readme.md
--rw-r--r--   0        0        0    36272 1970-01-01 00:00:00.000000 python_115-0.0.8.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.3/LICENSE
+-rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.3/p115/__init__.py
+-rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.3/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.3/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.3/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8.3/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.3/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.3/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.3/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.3/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   246219 2024-05-24 16:29:48.050265 python_115-0.0.8.3/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.3/p115/component/exception.py
+-rwxr-xr-x   0        0        0    56840 2024-05-23 15:52:16.591932 python_115-0.0.8.3/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48067 2024-05-24 16:16:56.781105 python_115-0.0.8.3/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.3/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.3/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     4816 2024-05-22 14:03:48.259741 python_115-0.0.8.3/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     7086 2024-05-22 14:03:58.992780 python_115-0.0.8.3/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4338 2024-05-24 16:52:21.603382 python_115-0.0.8.3/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6373 2024-05-24 16:52:41.937491 python_115-0.0.8.3/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.3/p115/py.typed
+-rwxr-xr-x   0        0        0     3217 2024-05-09 09:59:33.438651 python_115-0.0.8.3/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1593 2024-05-24 16:53:14.433582 python_115-0.0.8.3/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.3/readme.md
+-rw-r--r--   0        0        0    36272 1970-01-01 00:00:00.000000 python_115-0.0.8.3/PKG-INFO
```

### Comparing `python_115-0.0.8.2/LICENSE` & `python_115-0.0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/p115/cmd/iterdir.py` & `python_115-0.0.8.3/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/p115/cmd/qrcode.py` & `python_115-0.0.8.3/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/p115/component/__init__.py` & `python_115-0.0.8.3/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/p115/component/cipher.py` & `python_115-0.0.8.3/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/p115/component/client.py` & `python_115-0.0.8.3/p115/component/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from concurrent.futures import Future
 from contextlib import asynccontextmanager, aclosing, closing
 from datetime import date, datetime
 from email.utils import formatdate
 from functools import cached_property, partial, update_wrapper
 from hashlib import md5, sha1
 from hmac import digest as hmac_digest
-from http.cookiejar import Cookie
+from http.cookiejar import Cookie, CookieJar
 from http.cookies import Morsel
 from inspect import iscoroutinefunction
 from itertools import count, takewhile
 from json import dumps, loads
 from os import fsdecode, fstat, stat, PathLike
 from os import path as ospath
 from re import compile as re_compile
@@ -47,15 +47,15 @@
     bytes_iter_skip, bytes_async_iter_skip, 
     bytes_to_chunk_iter, bytes_to_chunk_async_iter, 
     bytes_ensure_part_iter, bytes_ensure_part_async_iter, 
 )
 from hashtools import file_digest, file_digest_async
 from http_request import encode_multipart_data, encode_multipart_data_async, SupportsGeturl
 from http_response import get_content_length, get_filename, get_total_length, is_range_request
-from httpfile import RequestsFileReader # TODO: use urllib3 instead
+from httpfile import HTTPFileReader
 from httpx import AsyncClient, Client, Cookies, TimeoutException
 from httpx_request import request as httpx_request
 from iterutils import through, async_through, wrap_iter, wrap_aiter
 from multidict import CIMultiDict
 from qrcode import QRCode # type: ignore
 from startfile import startfile, startfile_async # type: ignore
 from urlopen import urlopen
@@ -190,15 +190,15 @@
     |      4 | A4      | ?          | 未知: ipad             |
     |      5 | B1      | ?          | 未知: android          |
     |      6 | D1      | ios        | 115生活(iOS端)         |
     |      7 | F1      | android    | 115生活(Android端)     |
     |      8 | H1      | ?          | 未知: ipad             |
     |      9 | I1      | tv         | 115网盘(Android电视端) |
     |     10 | M1      | qandriod   | 115管理(Android端)     |
-    |     11 | N1      | ?          | 115管理(iOS端)         |
+    |     11 | N1      | qios       | 115管理(iOS端)         |
     |     12 | O1      | ?          | 未知: ipad             |
     |     13 | P1      | windows    | 115生活(Windows端)     |
     |     14 | P2      | mac        | 115生活(macOS端)       |
     |     15 | P3      | linux      | 115生活(Linux端)       |
     |     16 | R1      | wechatmini | 115生活(微信小程序)    |
     |     17 | R2      | alipaymini | 115生活(支付宝小程序)  |
     """
@@ -253,14 +253,18 @@
         ns = self.__dict__
         session = AsyncClient()
         session._headers = ns["headers"]
         session._cookies = ns["cookies"]
         return session
 
     @property
+    def cookiejar(self, /) -> CookieJar:
+        return self.__dict__["cookies"].jar
+
+    @property
     def cookies(self, /) -> str:
         """115 登录的 cookies，包含 UID, CID 和 SEID 这 3 个字段
         """
         cookies = self.__dict__["cookies"]
         return "; ".join(f"{key}={cookies.get(key, '')}" for key in ("UID", "CID", "SEID"))
 
     @cookies.setter
@@ -439,15 +443,14 @@
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """获取所有的已登录设备的信息，不过当前必须未登录失效
         GET https://passportapi.115.com/app/1.0/web/9.2/login_log/login_devices
         """
         api = "https://passportapi.115.com/app/1.0/web/9.2/login_log/login_devices"
-        request_kwargs.pop("parse", None)
         return self.request(api, async_=async_, **request_kwargs)
 
     @overload
     def login(
         self, 
         /, 
         app: str, 
@@ -482,14 +485,18 @@
             - tv
             - qandroid
             - windows
             - mac
             - linux
             - wechatmini
             - alipaymini
+        还有几个备选：
+            - bios
+            - bandroid
+            - qios
 
         设备列表如下：
 
         | No.    | ssoent  | app        | description            |
         |-------:|:--------|:-----------|:-----------------------|
         |      1 | A1      | web        | 网页版                 |
         |      2 | A2      | ?          | 未知: android          |
@@ -497,15 +504,15 @@
         |      4 | A4      | ?          | 未知: ipad             |
         |      5 | B1      | ?          | 未知: android          |
         |      6 | D1      | ios        | 115生活(iOS端)         |
         |      7 | F1      | android    | 115生活(Android端)     |
         |      8 | H1      | ?          | 未知: ipad             |
         |      9 | I1      | tv         | 115网盘(Android电视端) |
         |     10 | M1      | qandriod   | 115管理(Android端)     |
-        |     11 | N1      | ?          | 115管理(iOS端)         |
+        |     11 | N1      | qios       | 115管理(iOS端)         |
         |     12 | O1      | ?          | 未知: ipad             |
         |     13 | P1      | windows    | 115生活(Windows端)     |
         |     14 | P2      | mac        | 115生活(macOS端)       |
         |     15 | P3      | linux      | 115生活(Linux端)       |
         |     16 | R1      | wechatmini | 115生活(微信小程序)    |
         |     17 | R2      | alipaymini | 115生活(支付宝小程序)  |
         """
@@ -571,14 +578,18 @@
             - tv
             - qandroid
             - windows
             - mac
             - linux
             - wechatmini
             - alipaymini
+        还有几个备选：
+            - bios
+            - bandroid
+            - qios
 
         设备列表如下：
 
         | No.    | ssoent  | app        | description            |
         |-------:|:--------|:-----------|:-----------------------|
         |      1 | A1      | web        | 网页版                 |
         |      2 | A2      | ?          | 未知: android          |
@@ -586,15 +597,15 @@
         |      4 | A4      | ?          | 未知: ipad             |
         |      5 | B1      | ?          | 未知: android          |
         |      6 | D1      | ios        | 115生活(iOS端)         |
         |      7 | F1      | android    | 115生活(Android端)     |
         |      8 | H1      | ?          | 未知: ipad             |
         |      9 | I1      | tv         | 115网盘(Android电视端) |
         |     10 | M1      | qandriod   | 115管理(Android端)     |
-        |     11 | N1      | ?          | 115管理(iOS端)         |
+        |     11 | N1      | qios       | 115管理(iOS端)         |
         |     12 | O1      | ?          | 未知: ipad             |
         |     13 | P1      | windows    | 115生活(Windows端)     |
         |     14 | P2      | mac        | 115生活(macOS端)       |
         |     15 | P3      | linux      | 115生活(Linux端)       |
         |     16 | R1      | wechatmini | 115生活(微信小程序)    |
         |     17 | R2      | alipaymini | 115生活(支付宝小程序)  |
         """
@@ -605,15 +616,15 @@
                 qrcode_token = (await cls.login_qrcode_token(async_=async_, **request_kwargs))["data"]
                 qrcode = qrcode_token.pop("qrcode")
                 if open_qrcode_on_console:
                     qr = QRCode(border=1)
                     qr.add_data(qrcode)
                     qr.print_ascii(tty=True)
                 else:
-                    await startfile_async("https://qrcodeapi.115.com/api/1.0/mac/1.0/qrcode?uid=" + qrcode_token["uid"])
+                    await startfile_async("https://qrcodeapi.115.com/api/1.0/web/1.0/qrcode?uid=" + qrcode_token["uid"])
                 while True:
                     try:
                         resp = await cls.login_qrcode_status(
                             qrcode_token, async_=async_, **request_kwargs)
                     except TimeoutException:
                         continue
                     status = resp["data"].get("status")
@@ -640,15 +651,15 @@
             qrcode_token = cls.login_qrcode_token(async_=async_, **request_kwargs)["data"]
             qrcode = qrcode_token.pop("qrcode")
             if open_qrcode_on_console:
                 qr = QRCode(border=1)
                 qr.add_data(qrcode)
                 qr.print_ascii(tty=True)
             else:
-                startfile("https://qrcodeapi.115.com/api/1.0/mac/1.0/qrcode?uid=" + qrcode_token["uid"])
+                startfile("https://qrcodeapi.115.com/api/1.0/web/1.0/qrcode?uid=" + qrcode_token["uid"])
             while True:
                 try:
                     resp = cls.login_qrcode_status(
                         qrcode_token, async_=async_, **request_kwargs)
                 except TimeoutException:
                     continue
                 status = resp["data"].get("status")
@@ -713,15 +724,15 @@
         |      4 | A4      | ?          | 未知: ipad             |
         |      5 | B1      | ?          | 未知: android          |
         |      6 | D1      | ios        | 115生活(iOS端)         |
         |      7 | F1      | android    | 115生活(Android端)     |
         |      8 | H1      | ?          | 未知: ipad             |
         |      9 | I1      | tv         | 115网盘(Android电视端) |
         |     10 | M1      | qandriod   | 115管理(Android端)     |
-        |     11 | N1      | ?          | 115管理(iOS端)         |
+        |     11 | N1      | qios       | 115管理(iOS端)         |
         |     12 | O1      | ?          | 未知: ipad             |
         |     13 | P1      | windows    | 115生活(Windows端)     |
         |     14 | P2      | mac        | 115生活(macOS端)       |
         |     15 | P3      | linux      | 115生活(Linux端)       |
         |     16 | R1      | wechatmini | 115生活(微信小程序)    |
         |     17 | R2      | alipaymini | 115生活(支付宝小程序)  |
         """
@@ -763,69 +774,69 @@
             if replace:
                 self.cookies = data["data"]["cookie"]
                 return self
             else:
                 return type(self)(data["data"]["cookie"])
 
     @overload
-    @staticmethod
     def login_qrcode_scan(
+        self, 
         payload: str | dict, 
         /,
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> dict:
         ...
     @overload
-    @staticmethod
     def login_qrcode_scan(
+        self, 
         payload: str | dict, 
         /,
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
-    @staticmethod
     def login_qrcode_scan(
+        self, 
         payload: str | dict, 
         /,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """扫描二维码，payload 数据取自 `login_qrcode_token` 接口响应
         GET https://qrcodeapi.115.com/api/2.0/prompt.php
         payload:
             - uid: str
         """
         api = "https://qrcodeapi.115.com/api/2.0/prompt.php"
         if isinstance(payload, str):
             payload = {"uid": payload}
         request_kwargs.pop("parse", None)
-        return request(api, params=payload, async_=async_, **request_kwargs)
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     @overload
-    @staticmethod
     def login_qrcode_scan_confirm(
+        self, 
         payload: str | dict, 
         /,
         async_: Literal[False] = False, 
         **request_kwargs, 
     ) -> dict:
         ...
     @overload
-    @staticmethod
     def login_qrcode_scan_confirm(
+        self, 
         payload: str | dict, 
         /,
         async_: Literal[True], 
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
-    @staticmethod
     def login_qrcode_scan_confirm(
+        self, 
         payload: str | dict, 
         /,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """确认扫描二维码，payload 数据取自 `login_qrcode_scan` 接口响应
         GET https://hnqrcodeapi.115.com/api/2.0/slogin.php
@@ -834,15 +845,15 @@
             - uid: str
             - client: int = 0
         """
         api = "https://hnqrcodeapi.115.com/api/2.0/slogin.php"
         if isinstance(payload, str):
             payload = {"key": payload, "uid": payload, "client": 0}
         request_kwargs.pop("parse", None)
-        return request(api, params=payload, async_=async_, **request_kwargs)
+        return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     @overload
     @staticmethod
     def login_qrcode_scan_cancel(
         payload: str | dict, 
         /,
         async_: Literal[False] = False, 
@@ -1099,15 +1110,15 @@
         |      4 | A4      | ?          | 未知: ipad             |
         |      5 | B1      | ?          | 未知: android          |
         |      6 | D1      | ios        | 115生活(iOS端)         |
         |      7 | F1      | android    | 115生活(Android端)     |
         |      8 | H1      | ?          | 未知: ipad             |
         |      9 | I1      | tv         | 115网盘(Android电视端) |
         |     10 | M1      | qandriod   | 115管理(Android端)     |
-        |     11 | N1      | ?          | 115管理(iOS端)         |
+        |     11 | N1      | qios       | 115管理(iOS端)         |
         |     12 | O1      | ?          | 未知: ipad             |
         |     13 | P1      | windows    | 115生活(Windows端)     |
         |     14 | P2      | mac        | 115生活(macOS端)       |
         |     15 | P3      | linux      | 115生活(Linux端)       |
         |     16 | R1      | wechatmini | 115生活(微信小程序)    |
         |     17 | R2      | alipaymini | 115生活(支付宝小程序)  |
         """
@@ -1156,15 +1167,15 @@
         |      4 | A4      | ?          | 未知: ipad             |
         |      5 | B1      | ?          | 未知: android          |
         |      6 | D1      | ios        | 115生活(iOS端)         |
         |      7 | F1      | android    | 115生活(Android端)     |
         |      8 | H1      | ?          | 未知: ipad             |
         |      9 | I1      | tv         | 115网盘(Android电视端) |
         |     10 | M1      | qandriod   | 115管理(Android端)     |
-        |     11 | N1      | ?          | 115管理(iOS端)         |
+        |     11 | N1      | qios       | 115管理(iOS端)         |
         |     12 | O1      | ?          | 未知: ipad             |
         |     13 | P1      | windows    | 115生活(Windows端)     |
         |     14 | P2      | mac        | 115生活(macOS端)       |
         |     15 | P3      | linux      | 115生活(Linux端)       |
         |     16 | R1      | wechatmini | 115生活(微信小程序)    |
         |     17 | R2      | alipaymini | 115生活(支付宝小程序)  |
         """
@@ -4350,14 +4361,18 @@
                 async_=async_, 
                 **request_kwargs, 
             )
 
     # TODO
     def _oss_upload_future(self): ...
 
+    # TODO: 上下文管理器，需要返回的信息：bucket, object, upload_id, callback
+    # TODO: 支持断点续传，但只支持 buffer、路径、url、可 seek 的 reader，否则报错
+    def _oss_multipart_upload_ctx(self): ...
+
     @overload
     def _oss_multipart_upload(
         self, 
         /, 
         file: ( bytes | bytearray | memoryview | 
                 SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
                 Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
@@ -5006,15 +5021,14 @@
                 "sha1": file_sha1, 
                 "cid": pid, 
                 "pickcode": resp["pickcode"], 
             }
             return resp
 
     # TODO: 支持进度条和随时暂停，基于迭代器，使用一个 flag，每次迭代检查一下
-    # TODO: 支持断点续传（只支持 buffer、路径、url、可 seek 的 reader），需要保存的信息：bucket, object, upload_id, callback
     # TODO: class P115MultipartUploadTask:
     #           @classmethod
     #           def from_cache(cls, /, bucket, object, upload_id, callback, file): ...
     @overload
     def upload_file(
         self, 
         /, 
@@ -5052,14 +5066,15 @@
         **request_kwargs, 
     ) -> Awaitable[dict]:
         ...
     def upload_file(
         self, 
         /, 
         file: ( str | PathLike | URL | SupportsGeturl | 
+                # TODO: 当升级到 0.1 版本时，将强制要求 python 3.12，这 bytes | bytearray | memoryview 用 collections.abc.Buffer 
                 bytes | bytearray | memoryview | 
                 SupportsRead[bytes] | SupportsRead[bytearray] | SupportsRead[memoryview] | 
                 Iterable[bytes] | Iterable[bytearray] | Iterable[memoryview] | 
                 AsyncIterable[bytes] | AsyncIterable[bytearray] | AsyncIterable[memoryview] ), 
         filename: None | str = None, 
         pid: int = 0, 
         filesize: int = -1, 
@@ -5069,14 +5084,15 @@
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """文件上传接口，这是高层封装，推荐使用
         """
         if upload_directly:
             return self.upload_file_sample(file, filename, pid, async_=async_, **request_kwargs)
+
         if async_:
             async def async_request():
                 nonlocal async_, file, filename, filesize, file_sha1
                 async_ = cast(Literal[True], async_)
 
                 async def do_upload(file):
                     nonlocal async_
@@ -5154,17 +5170,14 @@
                     if filesize < 1 << 20:
                         async with ctx_async_read(path) as (_, read):
                             file = cast(bytes, await read())
                         if not file_sha1:
                             file_sha1 = sha1(file).hexdigest()
                     else:
                         if not file_sha1:
-                            file_digest_async
-                            h = sha1()
-                            h_update = h.update
                             async with ctx_async_read(path) as (file, _):
                                 _, hashobj = await file_digest_async(file, "sha1")
                             file_sha1 = hashobj.hexdigest()
                         async def read_range_bytes_or_hash(sign_check):
                             start, end = map(int, sign_check.split("-"))
                             async with ctx_async_read(path, start) as (_, read):
                                 return await read(end - start + 1)
@@ -5220,17 +5233,18 @@
                                 await file_seek(start)
                                 return await file_read(end - start + 1)
                             finally:
                                 await file_seek(curpos)
                 elif isinstance(file, (URL, SupportsGeturl)):
                     @asynccontextmanager
                     async def ctx_async_read(url, /, start=0):
-                        headers = None
                         if is_ranged and start:
                             headers = {"Range": "bytes=%s-" % start}
+                        else:
+                            headers = {}
                         try:
                             from aiohttp import request
                         except ImportError:
                             with (await to_thread(urlopen, url, headers=headers)) as resp:
                                 if not headers:
                                     await async_through(bio_skip_async_iter(resp, start))
                                 yield resp, as_thread(resp.read)
@@ -5262,20 +5276,17 @@
                                 return await self.upload_file_sample(resp, filename, pid, **request_kwargs)
                             return await do_upload(resp)
                 elif file_sha1:
                     if filesize < 0 or filesize >= 1 << 20:
                         filesize = 0
                 else:
                     return await self.upload_file_sample(file, filename, pid, async_=async_, **request_kwargs)
-
                 if not filename:
                     filename = str(uuid4())
-
                 return await do_upload(file)
-
             return async_request()
         else:
             def do_upload(file):
                 resp = self.upload_file_init(
                     cast(str, filename), 
                     filesize, 
                     cast(str, file_sha1), 
@@ -5395,17 +5406,18 @@
                             file_seek(start)
                             return sha1(file_read(end - start + 1)).hexdigest()
                         finally:
                             file_seek(curpos)
             elif isinstance(file, (URL, SupportsGeturl)):
                 def read_range_bytes_or_hash(sign_check: str):
                     start, end = map(int, sign_check.split("-"))
-                    headers = None
                     if is_ranged and start:
                         headers = {"Range": "bytes=%s-" % start}
+                    else:
+                        headers = {}
                     with urlopen(url, headers=headers) as resp:
                         if not headers:
                             through(bio_skip_iter(resp, start))
                         return resp.read(end - start + 1)
                 if isinstance(file, URL):
                     url = str(file)
                 else:
@@ -5425,18 +5437,16 @@
                             return self.upload_file_sample(resp, filename, pid, async_=async_, **request_kwargs)
                         return do_upload(resp)
             elif file_sha1:
                 if filesize < 0 or filesize >= 1 << 20:
                     filesize = 0
             else:
                 return self.upload_file_sample(file, filename, pid, async_=async_, **request_kwargs)
-
             if not filename:
                 filename = str(uuid4())
-
             return do_upload(file)
 
     # TODO: 提供一个可断点续传的版本
     # TODO: 支持进度条
     # TODO: 返回 future，支持 pause（暂停此任务，连接不释放）、stop（停止此任务，连接释放）、cancel（取消此任务）、resume（恢复），此时需要增加参数 wait
     def upload_file_future(self):
         ...
@@ -5863,15 +5873,15 @@
         if async_:
             async def async_request() -> str:
                 return get_url(await cast(Awaitable[dict], resp)) 
             return async_request()
         else:
             return get_url(cast(dict, resp))
 
-    # TODO
+    # TODO 支持异步
     @overload
     def extract_push_future(
         self, 
         /, 
         pickcode: str, 
         secret: str,
         async_: Literal[False] = False, 
@@ -5902,15 +5912,15 @@
             {"pick_code": pickcode, "secret": secret}, 
             **request_kwargs, 
         ))
         if resp["data"]["unzip_status"] == 4:
             return None
         return PushExtractProgress(self, pickcode)
 
-    # TODO
+    # TODO 支持异步
     @overload
     def extract_file_future(
         self, 
         /, 
         pickcode: str, 
         paths: str | Sequence[str], 
         dirname: str, 
@@ -6603,17 +6613,17 @@
     def captcha_code(
         self, 
         /,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> bytes | Awaitable[bytes]:
         """更新验证码，并获取图片数据（含 4 个汉字）
-        GET https://captchaapi.115.com/?ct=index&ac=code&ctype=0
+        GET https://captchaapi.115.com/?ct=index&ac=code
         """
-        api = "https://captchaapi.115.com/?ct=index&ac=code&ctype=0"
+        api = "https://captchaapi.115.com/?ct=index&ac=code"
         request_kwargs["parse"] = False
         return self.request(api, async_=async_, **request_kwargs)
 
     @overload
     def captcha_all(
         self, 
         /,
@@ -6704,75 +6714,78 @@
         """提交验证码
         POST https://webapi.115.com/user/captcha
         payload:
             - code: int | str # 从 0 到 9 中选取 4 个数字的一种排列
             - sign: str = <default>
             - ac: str = "security_code"
             - type: str = "web"
+            - ctype: str = <default>  # 其实不需要传，如果要传，就和 type 相同
+            - client: str = <default> # 其实不需要传，如果要传，就和 type 相同
         """
         if isinstance(payload, (int, str)):
             payload = {"code": payload, "ac": "security_code", "type": "web"}
         else:
             payload = {"ac": "security_code", "type": "web", **payload}
         if "sign" not in payload:
             payload["sign"] = self.captcha_sign()["sign"]
         api = "https://webapi.115.com/user/captcha"
         request_kwargs.pop("parse", None)
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     ########## Other Encapsulations ##########
 
-    # TODO: 支持 async_
-    # TODO: 使用 HTTPXFileReader
+    # TODO 支持异步
     @overload
     def open(
         self, 
         /, 
         url: str | Callable[[], str], 
         headers: None | Mapping, 
         start: int, 
         seek_threshold: int,
         async_: Literal[False] = False, 
-        **request_kwargs, 
-    ) -> RequestsFileReader:
+    ) -> HTTPFileReader:
         ...
     @overload
     def open(
         self, 
         /, 
         url: str | Callable[[], str], 
         headers: None | Mapping, 
         start: int, 
         seek_threshold: int,
         async_: Literal[True], 
-        **request_kwargs, 
-    ) -> Awaitable[RequestsFileReader]:
+    ) -> Awaitable[HTTPFileReader]:
         ...
     def open(
         self, 
         /, 
         url: str | Callable[[], str], 
         headers: None | Mapping = None, 
         start: int = 0, 
         seek_threshold: int = 1 << 20,
         async_: Literal[False, True] = False, 
-        **request_kwargs, 
-    ) -> RequestsFileReader | Awaitable[RequestsFileReader]:
-        """
+    ) -> HTTPFileReader | Awaitable[HTTPFileReader]:
+        """打开下载链接，可以从网盘、网盘上的压缩包内、分享链接中获取：
+            - P115Client.download_url
+            - P115Client.share_download_url
+            - P115Client.extract_download_url
         """
-        urlopen = self.session.get
-        if request_kwargs:
-            urlopen = partial(urlopen, **request_kwargs)
-        return RequestsFileReader(
-            url, 
-            headers=headers, 
-            start=start, 
-            seek_threshold=seek_threshold, 
-            urlopen=urlopen, 
-        )
+        if headers is None:
+            headers = self.headers
+        if async_:
+            raise OSError(errno.ENOSYS, "asynchronous mode not implemented")
+        else:
+            return HTTPFileReader(
+                url, 
+                headers=headers, 
+                start=start, 
+                seek_threshold=seek_threshold, 
+                urlopen=partial(urlopen, cookies=self.cookiejar), 
+            )
 
     # TODO: 返回一个 HTTPFileWriter，随时可以写入一些数据，close 代表上传完成，这个对象会持有一些信息
     def open_upload(self): ...
 
     @overload
     def read_bytes(
         self, 
@@ -6811,21 +6824,22 @@
         :param url: 115 文件的下载链接（可以从网盘、网盘上的压缩包内、分享链接中获取）
         :param start: 开始索引，可以为负数（从文件尾部开始）
         :param stop: 结束索引（不含），可以为负数（从文件尾部开始）
         :param headers: 一些请求头，最好提供一个 "User-Agent"
         :param async_: 是否异步
         :param request_kwargs: 其它请求参数
         """
-        need_get_length = start < 0 or (stop and stop < 0)
+        need_get_length = start < 0 or (stop is None or stop < 0)
         if need_get_length:
             if headers:
                 headers = {**headers, "Accept-Encoding": "identity"}
             else:
                 headers = {"Accept-Encoding": "identity"}
         request_kwargs["headers"] = headers
+        request_kwargs["parse"] = None
         if async_:
             async def get_bytes_range_async(start, stop) -> str:
                 if need_get_length:
                     async with aclosing(self.request(url, async_=async_, **request_kwargs)) as resp:
                         resp.raise_for_status()
                         length = get_total_length(resp)
                     if length is None:
```

### Comparing `python_115-0.0.8.2/p115/component/fs.py` & `python_115-0.0.8.3/p115/component/fs.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/p115/component/fs_base.py` & `python_115-0.0.8.3/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/p115/component/fs_share.py` & `python_115-0.0.8.3/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/p115/component/fs_zip.py` & `python_115-0.0.8.3/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/p115/component/labellist.py` & `python_115-0.0.8.3/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/p115/component/offline.py` & `python_115-0.0.8.3/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/p115/component/recyclebin.py` & `python_115-0.0.8.3/p115/component/recyclebin.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from collections.abc import Iterable, Iterator
 
 from .client import check_response, P115Client
 
 
 class P115Recyclebin:
+    "封装回收站"
     __slots__ = ("client", "password")
 
     def __init__(
         self, 
         client: str | P115Client, 
         /, 
         password: int | str = "", 
@@ -37,14 +38,15 @@
                 return item
         raise LookupError(f"no such id: {id!r}")
 
     def __iter__(self, /) -> Iterator[dict]:
         return self.iter()
 
     def __len__(self, /) -> int:
+        "计算回收站中的文件和文件夹数（不含文件夹内的递归计算）"
         return int(check_response(self.client.recyclebin_list({"limit": 1}))["count"])
 
     def __repr__(self, /) -> str:
         cls = type(self)
         module = cls.__module__
         name = cls.__qualname__
         if module != "__main__":
@@ -53,33 +55,36 @@
 
     @check_response
     def clear(
         self, 
         /, 
         password: None | int | str = None, 
     ) -> dict:
+        "清空回收站，如果不传入密码则用 self.password"
         if password is None:
             password = self.password
         return self.client.recyclebin_clean({"password": password})
 
     def get(
         self, 
         id: int | str, 
         /, 
         default=None, 
     ):
+        "用 id 查询回收站中的文件信息"
         ids = str(id)
         return next((item for item in self if item["id"] == ids), default)
 
     def iter(
         self, 
         /, 
         offset: int = 0, 
         page_size: int = 1 << 10, 
     ) -> Iterator[dict]:
+        "迭代获取回收站的文件信息"
         if offset < 0:
             offset = 0
         if page_size <= 0:
             page_size = 1 << 10
         payload = {"offset": offset, "limit": page_size}
         count = 0
         while True:
@@ -97,40 +102,43 @@
 
     def list(
         self, 
         /, 
         offset: int = 0, 
         limit: int = 0, 
     ) -> list[dict]:
+        "获取回收站的文件信息列表"
         if limit <= 0:
             return list(self.iter(offset))
         resp = check_response(self.client.recyclebin_list({"offset": offset, "limit": limit}))
         if resp["offset"] != offset:
             return []
         return resp["data"]
 
     @check_response
     def remove(
         self, 
         ids: int | str | Iterable[int | str], 
         /, 
         password: None | int | str = None, 
     ) -> dict:
+        "从回收站删除文件（即永久删除），如果不传入密码则用 self.password"
         if isinstance(ids, (int, str)):
             payload = {"rid[0]": ids}
         else:
             payload = {f"rid[{i}]": id for i, id in enumerate(ids)}
         payload["password"] = self.password if password is None else password
         return self.client.recyclebin_clean(payload)
 
     @check_response
     def revert(
         self, 
         ids: int | str | Iterable[int | str], 
         /, 
     ) -> dict:
+        "恢复已删除文件"
         if isinstance(ids, (int, str)):
             payload = {"rid[0]": ids}
         else:
             payload = {f"rid[{i}]": id for i, id in enumerate(ids)}
         return self.client.recyclebin_revert(payload)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `python_115-0.0.8.2/p115/tool/__init__.py` & `python_115-0.0.8.3/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/pyproject.toml` & `python_115-0.0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.2"
+version = "0.0.8.3"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.2/readme.md` & `python_115-0.0.8.3/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.2/PKG-INFO` & `python_115-0.0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.2
+Version: 0.0.8.3
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

