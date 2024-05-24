# Comparing `tmp/fastapi_file_router-0.1.8.tar.gz` & `tmp/fastapi_file_router-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_file_router-0.1.8.tar", max compression
+gzip compressed data, was "fastapi_file_router-0.1.9.tar", max compression
```

## Comparing `fastapi_file_router-0.1.8.tar` & `fastapi_file_router-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-12 19:24:46.691424 fastapi_file_router-0.1.8/README.md
--rw-r--r--   0        0        0     2452 2024-05-13 04:56:04.171226 fastapi_file_router-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-12 19:23:28.924492 fastapi_file_router-0.1.8/src/fastapi_file_router/__init__.py
--rw-r--r--   0        0        0     3410 2024-05-12 19:30:34.476536 fastapi_file_router-0.1.8/src/fastapi_file_router/router.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 fastapi_file_router-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-12 19:24:46.691424 fastapi_file_router-0.1.9/README.md
+-rw-r--r--   0        0        0     2452 2024-05-13 04:57:10.533857 fastapi_file_router-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-12 19:23:28.924492 fastapi_file_router-0.1.9/src/fastapi_file_router/__init__.py
+-rw-r--r--   0        0        0     3436 2024-05-13 04:57:06.593701 fastapi_file_router-0.1.9/src/fastapi_file_router/router.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 fastapi_file_router-0.1.9/PKG-INFO
```

### Comparing `fastapi_file_router-0.1.8/pyproject.toml` & `fastapi_file_router-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-file-router"
-version = "0.1.8"
+version = "0.1.9"
 description = "File-based routing for FastAPI"
 authors = ["Bewinxed <bewinxed@gmail.com>"]
 license = "WhoCares"
 readme = "README.md"
 packages = [
     # include the router in src
     { include = "fastapi_file_router", from = "./src" },
```

### Comparing `fastapi_file_router-0.1.8/src/fastapi_file_router/router.py` & `fastapi_file_router-0.1.9/src/fastapi_file_router/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import importlib
 import os
 from time import time
 from typing import Generator, Tuple
 
+__all__ = ["load_routes"]
 
 def log(message: str, verbose: bool):
     if verbose:
         print(message)  # Simple print can be replaced with any logging mechanism
 
 
 def square_to_curly_brackets(path: str) -> str:
```

