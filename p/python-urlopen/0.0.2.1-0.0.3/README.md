# Comparing `tmp/python_urlopen-0.0.2.1.tar.gz` & `tmp/python_urlopen-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_urlopen-0.0.2.1.tar", max compression
+gzip compressed data, was "python_urlopen-0.0.3.tar", max compression
```

## Comparing `python_urlopen-0.0.2.1.tar` & `python_urlopen-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_urlopen-0.0.2.1/LICENSE
--rw-r--r--   0        0        0     1279 2024-05-22 04:39:44.178808 python_urlopen-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0      839 2024-05-14 12:36:18.615669 python_urlopen-0.0.2.1/readme.md
--rwxr-xr-x   0        0        0     7264 2024-05-22 04:33:21.207997 python_urlopen-0.0.2.1/urlopen/__init__.py
--rwxr-xr-x   0        0        0     2562 2024-05-22 04:39:19.124630 python_urlopen-0.0.2.1/urlopen/__main__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_urlopen-0.0.2.1/urlopen/py.typed
--rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 python_urlopen-0.0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_urlopen-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1277 2024-05-24 16:02:05.320956 python_urlopen-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      839 2024-05-14 12:36:18.615669 python_urlopen-0.0.3/readme.md
+-rwxr-xr-x   0        0        0     7518 2024-05-24 16:01:50.680524 python_urlopen-0.0.3/urlopen/__init__.py
+-rwxr-xr-x   0        0        0     2562 2024-05-22 04:39:19.124630 python_urlopen-0.0.3/urlopen/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_urlopen-0.0.3/urlopen/py.typed
+-rw-r--r--   0        0        0     2021 1970-01-01 00:00:00.000000 python_urlopen-0.0.3/PKG-INFO
```

### Comparing `python_urlopen-0.0.2.1/LICENSE` & `python_urlopen-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_urlopen-0.0.2.1/pyproject.toml` & `python_urlopen-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-urlopen"
-version = "0.0.2.1"
+version = "0.0.3"
 description = "Python urlopen wrapper."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-urlopen"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-urlopen"
 keywords = ["urlopen"]
```

### Comparing `python_urlopen-0.0.2.1/readme.md` & `python_urlopen-0.0.3/readme.md`

 * *Files identical despite different names*

### Comparing `python_urlopen-0.0.2.1/urlopen/__init__.py` & `python_urlopen-0.0.3/urlopen/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 2)
+__version__ = (0, 0, 3)
 __all__ = ["urlopen", "download"]
 
 import errno
 
 from collections.abc import Callable, Generator, Mapping, Sequence
 from copy import copy
 from http.client import HTTPResponse
+from http.cookiejar import CookieJar
 from inspect import isgenerator
 from json import dumps
 from os import fsdecode, fstat, makedirs, PathLike
 from os.path import abspath, dirname, isdir, join as joinpath
 from shutil import COPY_BUFSIZE # type: ignore
 from ssl import SSLContext, _create_unverified_context
 from typing import cast, Any, Optional
 from urllib.parse import urlencode, urlsplit
-from urllib.request import build_opener, HTTPSHandler, OpenerDirector, Request
+from urllib.request import build_opener, HTTPCookieProcessor, HTTPSHandler, OpenerDirector, Request
 
 from filewrap import bio_skip_iter, SupportsRead, SupportsWrite
 from http_response import get_filename, get_length, is_chunked, is_range_request
 
 
 if "__del__" not in HTTPResponse.__dict__:
     setattr(HTTPResponse, "__del__", HTTPResponse.close)
 
 
 def urlopen(
     url: str | Request, 
+    method: str = "GET", 
     params: Optional[str | Mapping | Sequence[tuple[Any, Any]]] = None, 
     data: Optional[bytes | str | Mapping | Sequence[tuple[Any, Any]]] = None, 
     json: Any = None, 
     headers: dict[str, str] = {"User-agent": ""}, 
-    method: str = "GET", 
     timeout: Optional[int | float] = None, 
+    cookies: Optional[CookieJar] = None, 
     proxy: Optional[tuple[str, str]] = None, 
     opener: OpenerDirector = build_opener(HTTPSHandler(context=_create_unverified_context())), 
     context: Optional[SSLContext] = None, 
     origin: Optional[str] = None, 
 ) -> HTTPResponse:
     if isinstance(url, str) and not urlsplit(url).scheme:
         if origin:
@@ -73,19 +75,23 @@
                 req.add_header(key, val)
         if data is not None:
             req.data = data
         req.method = method.upper()
     else:
         if params:
             url += "?&"["?" in url] + params
-        req = Request(url, data, headers=headers, method=method.upper())
+        req = Request(url, data=data, headers=headers, method=method.upper())
     if proxy:
         req.set_proxy(*proxy)
-    if context:
-        opener = build_opener(HTTPSHandler(context=context))
+    if opener is None:
+        opener = build_opener()
+    if context is not None:
+        opener.add_handler(HTTPSHandler(context=context))
+    if cookies is not None:
+        opener.add_handler(HTTPCookieProcessor(cookies))
     if timeout is None:
         return opener.open(req)
     else:
         return opener.open(req, timeout=timeout)
 
 
 def download(
```

### Comparing `python_urlopen-0.0.2.1/urlopen/__main__.py` & `python_urlopen-0.0.3/urlopen/__main__.py`

 * *Files identical despite different names*

### Comparing `python_urlopen-0.0.2.1/PKG-INFO` & `python_urlopen-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-urlopen
-Version: 0.0.2.1
+Version: 0.0.3
 Summary: Python urlopen wrapper.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-urlopen
 License: MIT
 Keywords: urlopen
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

