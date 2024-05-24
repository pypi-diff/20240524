# Comparing `tmp/rfc9457-0.0.7.tar.gz` & `tmp/rfc9457-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfc9457-0.0.7.tar", max compression
+gzip compressed data, was "rfc9457-0.0.8.tar", max compression
```

## Comparing `rfc9457-0.0.7.tar` & `rfc9457-0.0.8.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    11307 2024-05-23 08:06:56.991648 rfc9457-0.0.7/LICENSE
--rw-r--r--   0        0        0     1789 2024-05-23 08:06:56.991648 rfc9457-0.0.7/README.md
--rw-r--r--   0        0        0     2021 2024-05-23 08:06:56.995648 rfc9457-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3308 2024-05-23 08:06:56.995648 rfc9457-0.0.7/src/rfc9457/__init__.py
--rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 rfc9457-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-05-24 09:29:50.446730 rfc9457-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1789 2024-05-24 09:29:50.446730 rfc9457-0.0.8/README.md
+-rw-r--r--   0        0        0     2021 2024-05-24 09:29:50.450730 rfc9457-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3308 2024-05-24 09:29:50.450730 rfc9457-0.0.8/src/rfc9457/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:29:50.450730 rfc9457-0.0.8/src/rfc9457/py.typed
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 rfc9457-0.0.8/PKG-INFO
```

### Comparing `rfc9457-0.0.7/LICENSE` & `rfc9457-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.7/README.md` & `rfc9457-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.7/pyproject.toml` & `rfc9457-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rfc9457"
-version = "0.0.7"
+version = "0.0.8"
 description = "Implementation of RFC9457 problems."
 authors = ["Daniel Edgecombe <daniel@nrwl.co>"]
 license = "Apache-2.0"
 repository="https://github.com/NRWLDev/rfc9457/"
 homepage="https://github.com/NRWLDev/rfc9457/"
 readme = "README.md"
 
@@ -19,15 +19,15 @@
 pytest-random-order = "^1.0"
 
 # Style
 ruff = "^0.3"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.0.7"
+current_version = "0.0.8"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `rfc9457-0.0.7/src/rfc9457/__init__.py` & `rfc9457-0.0.8/src/rfc9457/__init__.py`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.7/PKG-INFO` & `rfc9457-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfc9457
-Version: 0.0.7
+Version: 0.0.8
 Summary: Implementation of RFC9457 problems.
 Home-page: https://github.com/NRWLDev/rfc9457/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: daniel@nrwl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

