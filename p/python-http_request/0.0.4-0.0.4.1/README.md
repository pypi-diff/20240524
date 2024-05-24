# Comparing `tmp/python_http_request-0.0.4.tar.gz` & `tmp/python_http_request-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_http_request-0.0.4.tar", max compression
+gzip compressed data, was "python_http_request-0.0.4.1.tar", max compression
```

## Comparing `python_http_request-0.0.4.tar` & `python_http_request-0.0.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_http_request-0.0.4/LICENSE
--rwxr-xr-x   0        0        0     6169 2024-05-23 06:21:05.290392 python_http_request-0.0.4/http_request/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_http_request-0.0.4/http_request/py.typed
--rw-r--r--   0        0        0     1234 2024-05-23 06:21:39.118809 python_http_request-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      219 2024-05-17 15:05:56.280517 python_http_request-0.0.4/readme.md
--rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 python_http_request-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_http_request-0.0.4.1/LICENSE
+-rwxr-xr-x   0        0        0     6169 2024-05-23 06:21:05.290392 python_http_request-0.0.4.1/http_request/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_http_request-0.0.4.1/http_request/py.typed
+-rw-r--r--   0        0        0     1259 2024-05-24 17:03:37.634863 python_http_request-0.0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-05-17 15:05:56.280517 python_http_request-0.0.4.1/readme.md
+-rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 python_http_request-0.0.4.1/PKG-INFO
```

### Comparing `python_http_request-0.0.4/LICENSE` & `python_http_request-0.0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_http_request-0.0.4/http_request/__init__.py` & `python_http_request-0.0.4.1/http_request/__init__.py`

 * *Files identical despite different names*

### Comparing `python_http_request-0.0.4/pyproject.toml` & `python_http_request-0.0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-http_request"
-version = "0.0.4"
+version = "0.0.4.1"
 description = "Python http response utils."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request"
 keywords = ["http", "request"]
@@ -25,14 +25,15 @@
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 python-asynctools = "*"
 python-filewrap = "*"
+python-texttools = "*"
 integer_tool = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
```

### Comparing `python_http_request-0.0.4/PKG-INFO` & `python_http_request-0.0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-http_request
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: Python http response utils.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request
 License: MIT
 Keywords: http,request
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: integer_tool
 Requires-Dist: python-asynctools
 Requires-Dist: python-filewrap
+Requires-Dist: python-texttools
 Project-URL: Repository, https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-http_request
 Description-Content-Type: text/markdown
 
 # Python http response utils.
 
 ## Installation
```

