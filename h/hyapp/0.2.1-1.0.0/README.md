# Comparing `tmp/hyapp-0.2.1.tar.gz` & `tmp/hyapp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyapp-0.2.1.tar", max compression
+gzip compressed data, was "hyapp-1.0.0.tar", max compression
```

## Comparing `hyapp-0.2.1.tar` & `hyapp-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       36 2024-05-01 07:45:48.674852 hyapp-0.2.1/README.md
--rw-r--r--   0        0        0      612 2024-05-24 12:08:40.562328 hyapp-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-24 10:57:46.805533 hyapp-0.2.1/src/hyapp/__init__.py
--rw-r--r--   0        0        0    11323 2024-05-24 10:57:58.633591 hyapp-0.2.1/src/hyapp/aio.py
--rw-r--r--   0        0        0      704 2024-05-24 10:56:54.325276 hyapp-0.2.1/src/hyapp/alembic.py
--rw-r--r--   0        0        0     1876 2024-05-24 11:00:37.838369 hyapp-0.2.1/src/hyapp/api.py
--rw-r--r--   0        0        0     3481 2024-05-24 10:58:07.533634 hyapp-0.2.1/src/hyapp/base.py
--rw-r--r--   0        0        0     1066 2024-05-24 10:57:46.809533 hyapp-0.2.1/src/hyapp/datetimes.py
--rw-r--r--   0        0        0     3648 2024-05-24 10:57:46.809533 hyapp-0.2.1/src/hyapp/funcutils.py
--rw-r--r--   0        0        0     7260 2024-05-24 10:58:16.541678 hyapp-0.2.1/src/hyapp/http.py
--rw-r--r--   0        0        0      855 2024-05-24 10:57:46.809533 hyapp-0.2.1/src/hyapp/jsons.py
--rw-r--r--   0        0        0     1394 2024-05-24 10:57:46.809533 hyapp-0.2.1/src/hyapp/lifetime.py
--rw-r--r--   0        0        0        0 2024-05-24 12:06:21.549649 hyapp-0.2.1/src/hyapp/py.typed
--rw-r--r--   0        0        0     1934 2024-05-24 10:57:46.809533 hyapp-0.2.1/src/hyapp/pydantics.py
--rw-r--r--   0        0        0      605 2024-05-24 10:57:31.373457 hyapp-0.2.1/src/hyapp/pydsettings.py
--rw-r--r--   0        0        0     2002 2024-05-24 10:56:54.329276 hyapp-0.2.1/src/hyapp/pytests.py
--rw-r--r--   0        0        0     3573 2024-05-24 10:57:46.809533 hyapp-0.2.1/src/hyapp/runlib.py
--rw-r--r--   0        0        0      521 2024-05-24 11:00:07.622221 hyapp-0.2.1/src/hyapp/trace.py
--rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 hyapp-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       36 2024-05-01 07:45:48.674852 hyapp-1.0.0/README.md
+-rw-r--r--   0        0        0      612 2024-05-24 12:09:53.634686 hyapp-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 10:57:46.805533 hyapp-1.0.0/src/hyapp/__init__.py
+-rw-r--r--   0        0        0    11323 2024-05-24 10:57:58.633591 hyapp-1.0.0/src/hyapp/aio.py
+-rw-r--r--   0        0        0      704 2024-05-24 10:56:54.325276 hyapp-1.0.0/src/hyapp/alembics.py
+-rw-r--r--   0        0        0     1876 2024-05-24 11:00:37.838369 hyapp-1.0.0/src/hyapp/api.py
+-rw-r--r--   0        0        0     3481 2024-05-24 10:58:07.533634 hyapp-1.0.0/src/hyapp/base.py
+-rw-r--r--   0        0        0     1066 2024-05-24 10:57:46.809533 hyapp-1.0.0/src/hyapp/datetimes.py
+-rw-r--r--   0        0        0     3648 2024-05-24 10:57:46.809533 hyapp-1.0.0/src/hyapp/funcutils.py
+-rw-r--r--   0        0        0     7260 2024-05-24 10:58:16.541678 hyapp-1.0.0/src/hyapp/http.py
+-rw-r--r--   0        0        0      855 2024-05-24 10:57:46.809533 hyapp-1.0.0/src/hyapp/jsons.py
+-rw-r--r--   0        0        0     1394 2024-05-24 10:57:46.809533 hyapp-1.0.0/src/hyapp/lifetime.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:06:21.549649 hyapp-1.0.0/src/hyapp/py.typed
+-rw-r--r--   0        0        0     1934 2024-05-24 10:57:46.809533 hyapp-1.0.0/src/hyapp/pydantics.py
+-rw-r--r--   0        0        0      605 2024-05-24 10:57:31.373457 hyapp-1.0.0/src/hyapp/pydsettings.py
+-rw-r--r--   0        0        0     2002 2024-05-24 10:56:54.329276 hyapp-1.0.0/src/hyapp/pytests.py
+-rw-r--r--   0        0        0     3573 2024-05-24 10:57:46.809533 hyapp-1.0.0/src/hyapp/runlib.py
+-rw-r--r--   0        0        0      521 2024-05-24 11:00:07.622221 hyapp-1.0.0/src/hyapp/trace.py
+-rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 hyapp-1.0.0/PKG-INFO
```

### Comparing `hyapp-0.2.1/pyproject.toml` & `hyapp-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyapp"
-version = "0.2.1"
+version = "1.0.0"
 description = ""
 authors = ["HoverHell <hoverhell@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyapp", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `hyapp-0.2.1/src/hyapp/aio.py` & `hyapp-1.0.0/src/hyapp/aio.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/alembic.py` & `hyapp-1.0.0/src/hyapp/alembics.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/api.py` & `hyapp-1.0.0/src/hyapp/api.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/base.py` & `hyapp-1.0.0/src/hyapp/base.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/datetimes.py` & `hyapp-1.0.0/src/hyapp/datetimes.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/funcutils.py` & `hyapp-1.0.0/src/hyapp/funcutils.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/http.py` & `hyapp-1.0.0/src/hyapp/http.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/jsons.py` & `hyapp-1.0.0/src/hyapp/jsons.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/lifetime.py` & `hyapp-1.0.0/src/hyapp/lifetime.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/pydantics.py` & `hyapp-1.0.0/src/hyapp/pydantics.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/pydsettings.py` & `hyapp-1.0.0/src/hyapp/pydsettings.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/pytests.py` & `hyapp-1.0.0/src/hyapp/pytests.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/runlib.py` & `hyapp-1.0.0/src/hyapp/runlib.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/src/hyapp/trace.py` & `hyapp-1.0.0/src/hyapp/trace.py`

 * *Files identical despite different names*

### Comparing `hyapp-0.2.1/PKG-INFO` & `hyapp-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyapp
-Version: 0.2.1
+Version: 1.0.0
 Summary: 
 Author: HoverHell
 Author-email: hoverhell@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

