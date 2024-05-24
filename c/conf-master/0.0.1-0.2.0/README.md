# Comparing `tmp/conf_master-0.0.1.tar.gz` & `tmp/conf_master-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_master-0.0.1.tar", max compression
+gzip compressed data, was "conf_master-0.2.0.tar", max compression
```

## Comparing `conf_master-0.0.1.tar` & `conf_master-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1107 2024-05-24 17:39:25.661378 conf_master-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1358 2024-05-24 18:11:16.261536 conf_master-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      525 2024-05-24 18:10:55.413632 conf_master-0.0.1/README.md
--rw-r--r--   0        0        0      109 2024-05-24 17:39:25.660379 conf_master-0.0.1/src/conf_master/__init__.py
--rw-r--r--   0        0        0     1158 2024-05-24 18:10:44.178660 conf_master-0.0.1/src/conf_master/conf_master.py
--rw-r--r--   0        0        0     1490 1970-01-01 00:00:00.000000 conf_master-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1107 2024-05-24 17:39:25.661378 conf_master-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1358 2024-05-24 18:17:33.627410 conf_master-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      519 2024-05-24 18:12:30.119187 conf_master-0.2.0/README.md
+-rw-r--r--   0        0        0      109 2024-05-24 17:39:25.660379 conf_master-0.2.0/src/conf_master/__init__.py
+-rw-r--r--   0        0        0     1721 2024-05-24 18:17:13.043462 conf_master-0.2.0/src/conf_master/conf_master.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 conf_master-0.2.0/PKG-INFO
```

### Comparing `conf_master-0.0.1/LICENSE.txt` & `conf_master-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conf_master-0.0.1/pyproject.toml` & `conf_master-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "conf-master"
-version = "0.0.1"
+version = "0.2.0"
 description = ""
 readme = "README.md"
 authors = ["alvaroroco <alvaroroco@gmail.com>"]
 license = "MIT"
 keywords = []
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `conf_master-0.0.1/README.md` & `conf_master-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Py Config Handler
+# Conf Master
 
 [![PyPI - Version](https://img.shields.io/pypi/v/conf-master.svg)](https://pypi.org/project/conf-master)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/conf-master.svg)](https://pypi.org/project/conf-master)
 
 -----
 
 ## Table of Contents
```

### Comparing `conf_master-0.0.1/src/conf_master/conf_master.py` & `conf_master-0.2.0/src/conf_master/conf_master.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import json
+import yaml
 from typing import Any
 
 class ConfMaster():
     def __init__(self):
         self.config = {}
 
     def load_from_json(self, file_path: str) -> None:
         try:
             with open(file_path, 'r') as f:
                 self.config.update(json.load(f))
         except Exception as e:
             raise Exception(f"Error loading JSON config: {e}")
 
+    def load_from_yaml(self, file_path: str) -> None:
+        try:
+            with open(file_path, 'r') as f:
+                self.config.update(yaml.safe_load(f))
+        except Exception as e:
+            raise Exception(f"Error loading YAML config: {e}")
+
     def get(self, key: str, default: Any=None) -> Any:
         keys = key.split('.')
         value = self.config
         try:
             for k in keys:
                 value = value[k]
             return value
@@ -34,8 +42,15 @@
             d[keys[-1]] = value
 
     def save_to_json(self, file_path: str) -> None:
         try:
             with open(file_path, 'w') as f:
                 json.dump(self.config, f, indent=4)
         except Exception as e:
-            raise Exception(f"Error saving JSON config: {e}")
+            raise Exception(f"Error saving JSON config: {e}")
+
+    def save_to_yaml(self, file_path: str) -> None:
+        try:
+            with open(file_path, 'w') as f:
+                yaml.safe_dump(self.config, f, default_flow_style=False)
+        except Exception as e:
+            raise Exception(f"Error saving YAML config: {e}")
```

### Comparing `conf_master-0.0.1/PKG-INFO` & `conf_master-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-master
-Version: 0.0.1
+Version: 0.2.0
 Summary: 
 License: MIT
 Author: alvaroroco
 Author-email: alvaroroco@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Project-URL: documentation, https://github.com/alvaroroco/conf-master#readme
 Project-URL: issues, https://github.com/alvaroroco/conf-master/issues
 Project-URL: source, https://github.com/alvaroroco/conf-master
 Description-Content-Type: text/markdown
 
-# Py Config Handler
+# Conf Master
 
 [![PyPI - Version](https://img.shields.io/pypi/v/conf-master.svg)](https://pypi.org/project/conf-master)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/conf-master.svg)](https://pypi.org/project/conf-master)
 
 -----
 
 ## Table of Contents
```

