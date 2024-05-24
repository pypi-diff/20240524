# Comparing `tmp/hyapp-0.1.0.tar.gz` & `tmp/hyapp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyapp-0.1.0.tar", max compression
+gzip compressed data, was "hyapp-0.2.0.tar", max compression
```

## Comparing `hyapp-0.1.0.tar` & `hyapp-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       36 2024-05-01 07:45:48.674852 hyapp-0.1.0/README.md
--rw-r--r--   0        0        0      612 2024-05-01 08:06:18.180863 hyapp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-01 07:47:44.523418 hyapp-0.1.0/src/hyapp/__init__.py
--rw-r--r--   0        0        0    11323 2024-05-01 07:54:04.641276 hyapp-0.1.0/src/hyapp/aio.py
--rw-r--r--   0        0        0      704 2024-05-01 07:47:44.527418 hyapp-0.1.0/src/hyapp/alembic.py
--rw-r--r--   0        0        0     1799 2024-05-01 08:08:44.321577 hyapp-0.1.0/src/hyapp/api.py
--rw-r--r--   0        0        0     3481 2024-05-01 08:10:30.302095 hyapp-0.1.0/src/hyapp/base.py
--rw-r--r--   0        0        0     1066 2024-05-01 07:47:57.115480 hyapp-0.1.0/src/hyapp/datetimes.py
--rw-r--r--   0        0        0     3648 2024-05-01 07:47:44.527418 hyapp-0.1.0/src/hyapp/funcutils.py
--rw-r--r--   0        0        0     7260 2024-05-01 07:47:44.531418 hyapp-0.1.0/src/hyapp/http.py
--rw-r--r--   0        0        0      855 2024-05-01 07:47:44.531418 hyapp-0.1.0/src/hyapp/jsons.py
--rw-r--r--   0        0        0     1394 2024-05-01 07:47:44.531418 hyapp-0.1.0/src/hyapp/lifetime.py
--rw-r--r--   0        0        0     1934 2024-05-01 07:47:31.367354 hyapp-0.1.0/src/hyapp/pydantics.py
--rw-r--r--   0        0        0      605 2024-05-01 08:12:53.934797 hyapp-0.1.0/src/hyapp/pydsettings.py
--rw-r--r--   0        0        0     2002 2024-05-01 07:47:44.531418 hyapp-0.1.0/src/hyapp/pytests.py
--rw-r--r--   0        0        0     2012 2024-05-01 07:47:44.531418 hyapp-0.1.0/src/hyapp/runlib.py
--rw-r--r--   0        0        0      380 2024-05-01 07:47:44.535418 hyapp-0.1.0/src/hyapp/trace.py
--rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 hyapp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2024-05-01 07:45:48.674852 hyapp-0.2.0/README.md
+-rw-r--r--   0        0        0      612 2024-05-24 11:01:32.134634 hyapp-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 10:57:46.805533 hyapp-0.2.0/src/hyapp/__init__.py
+-rw-r--r--   0        0        0    11323 2024-05-24 10:57:58.633591 hyapp-0.2.0/src/hyapp/aio.py
+-rw-r--r--   0        0        0      704 2024-05-24 10:56:54.325276 hyapp-0.2.0/src/hyapp/alembic.py
+-rw-r--r--   0        0        0     1876 2024-05-24 11:00:37.838369 hyapp-0.2.0/src/hyapp/api.py
+-rw-r--r--   0        0        0     3481 2024-05-24 10:58:07.533634 hyapp-0.2.0/src/hyapp/base.py
+-rw-r--r--   0        0        0     1066 2024-05-24 10:57:46.809533 hyapp-0.2.0/src/hyapp/datetimes.py
+-rw-r--r--   0        0        0     3648 2024-05-24 10:57:46.809533 hyapp-0.2.0/src/hyapp/funcutils.py
+-rw-r--r--   0        0        0     7260 2024-05-24 10:58:16.541678 hyapp-0.2.0/src/hyapp/http.py
+-rw-r--r--   0        0        0      855 2024-05-24 10:57:46.809533 hyapp-0.2.0/src/hyapp/jsons.py
+-rw-r--r--   0        0        0     1394 2024-05-24 10:57:46.809533 hyapp-0.2.0/src/hyapp/lifetime.py
+-rw-r--r--   0        0        0     1934 2024-05-24 10:57:46.809533 hyapp-0.2.0/src/hyapp/pydantics.py
+-rw-r--r--   0        0        0      605 2024-05-24 10:57:31.373457 hyapp-0.2.0/src/hyapp/pydsettings.py
+-rw-r--r--   0        0        0     2002 2024-05-24 10:56:54.329276 hyapp-0.2.0/src/hyapp/pytests.py
+-rw-r--r--   0        0        0     3573 2024-05-24 10:57:46.809533 hyapp-0.2.0/src/hyapp/runlib.py
+-rw-r--r--   0        0        0      521 2024-05-24 11:00:07.622221 hyapp-0.2.0/src/hyapp/trace.py
+-rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 hyapp-0.2.0/PKG-INFO
```

### Comparing `hyapp-0.1.0/pyproject.toml` & `hyapp-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyapp"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["HoverHell <hoverhell@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyapp", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `hyapp-0.1.0/src/hyapp/aio.py` & `hyapp-0.2.0/src/hyapp/aio.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.1.0/src/hyapp/alembic.py` & `hyapp-0.2.0/src/hyapp/alembic.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.1.0/src/hyapp/api.py` & `hyapp-0.2.0/src/hyapp/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,36 +13,36 @@
 
 @dataclasses.dataclass()
 class TraceIdMiddleware:
     app: starlette.types.ASGIApp
     header_name: str = "X-Request-ID"
     header_validation_re: str = r"^[a-z0-9]{12,20}$"
     trace_id_var: ContextVar[str | None] = TRACE_ID_VAR
+    trace_id_prefix: str = "aa"  # "API App"
 
-    @staticmethod
-    def _new_trace_id() -> str:
-        return new_trace_id("aa")  # API App
+    def _new_trace_id(self, parent: str | None = None) -> str:
+        return new_trace_id(self.trace_id_prefix, parent=parent)
 
     async def __call__(
         self, scope: starlette.types.Scope, receive: starlette.types.Receive, send: starlette.types.Send
     ) -> None:
         if scope["type"] not in ("http", "websocket"):
             await self.app(scope, receive, send)
             return
 
         headers = starlette.datastructures.MutableHeaders(scope=scope)
         header_value = headers.get(self.header_name.lower())
+        parent_trace_id = None
         if header_value:
             if re.search(self.header_validation_re, header_value):
-                trace_id = header_value
+                parent_trace_id = header_value
             else:
                 LOGGER.debug("Invalid trace id in header %r: %r", self.header_name, header_value)
-            trace_id = self._new_trace_id()
-        else:
-            trace_id = self._new_trace_id()
+
+        trace_id = self._new_trace_id(parent=parent_trace_id)
 
         self.trace_id_var.set(trace_id)
 
         async def handle_outgoing_request(message: starlette.types.Message) -> None:
             local_trace_id = self.trace_id_var.get()
             if message["type"] == "http.response.start" and local_trace_id:
                 headers = starlette.datastructures.MutableHeaders(scope=message)
```

### Comparing `hyapp-0.1.0/src/hyapp/base.py` & `hyapp-0.2.0/src/hyapp/base.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.1.0/src/hyapp/datetimes.py` & `hyapp-0.2.0/src/hyapp/datetimes.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.1.0/src/hyapp/funcutils.py` & `hyapp-0.2.0/src/hyapp/funcutils.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.1.0/src/hyapp/http.py` & `hyapp-0.2.0/src/hyapp/http.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.1.0/src/hyapp/jsons.py` & `hyapp-0.2.0/src/hyapp/jsons.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.1.0/src/hyapp/lifetime.py` & `hyapp-0.2.0/src/hyapp/lifetime.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.1.0/src/hyapp/pydantics.py` & `hyapp-0.2.0/src/hyapp/pydantics.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.1.0/src/hyapp/pydsettings.py` & `hyapp-0.2.0/src/hyapp/pydsettings.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.1.0/src/hyapp/pytests.py` & `hyapp-0.2.0/src/hyapp/pytests.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.1.0/PKG-INFO` & `hyapp-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyapp
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: HoverHell
 Author-email: hoverhell@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

