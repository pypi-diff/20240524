# Comparing `tmp/conf_master-0.2.0.tar.gz` & `tmp/conf_master-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_master-0.2.0.tar", max compression
+gzip compressed data, was "conf_master-1.0.0.tar", max compression
```

## Comparing `conf_master-0.2.0.tar` & `conf_master-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     1107 2024-05-24 17:39:25.661378 conf_master-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1358 2024-05-24 18:17:33.627410 conf_master-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      519 2024-05-24 18:12:30.119187 conf_master-0.2.0/README.md
--rw-r--r--   0        0        0      109 2024-05-24 17:39:25.660379 conf_master-0.2.0/src/conf_master/__init__.py
--rw-r--r--   0        0        0     1721 2024-05-24 18:17:13.043462 conf_master-0.2.0/src/conf_master/conf_master.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 conf_master-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1107 2024-05-24 17:39:25.661378 conf_master-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     1358 2024-05-24 18:40:28.445182 conf_master-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      519 2024-05-24 18:12:30.119187 conf_master-1.0.0/README.md
+-rw-r--r--   0        0        0      109 2024-05-24 17:39:25.660379 conf_master-1.0.0/src/conf_master/__init__.py
+-rw-r--r--   0        0        0     2112 2024-05-24 18:39:37.523033 conf_master-1.0.0/src/conf_master/conf_master.py
+-rw-r--r--   0        0        0      332 2024-05-24 18:37:34.117998 conf_master-1.0.0/src/conf_master/exceptions.py
+-rw-r--r--   0        0        0      634 2024-05-24 18:35:56.694292 conf_master-1.0.0/src/conf_master/loaders.py
+-rw-r--r--   0        0        0      345 2024-05-24 18:25:51.397917 conf_master-1.0.0/src/conf_master/validators.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 conf_master-1.0.0/PKG-INFO
```

### Comparing `conf_master-0.2.0/LICENSE.txt` & `conf_master-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conf_master-0.2.0/pyproject.toml` & `conf_master-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "conf-master"
-version = "0.2.0"
+version = "1.0.0"
 description = ""
 readme = "README.md"
 authors = ["alvaroroco <alvaroroco@gmail.com>"]
 license = "MIT"
 keywords = []
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `conf_master-0.2.0/README.md` & `conf_master-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `conf_master-0.2.0/src/conf_master/conf_master.py` & `conf_master-1.0.0/src/conf_master/conf_master.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import json
 import yaml
+import os
 from typing import Any
 
+from .loaders import load_json, load_yaml, load_env
+from .validators import validate_config
+from .exceptions import ConfigLoadError, ConfigValidationError
+
 class ConfMaster():
     def __init__(self):
         self.config = {}
 
     def load_from_json(self, file_path: str) -> None:
         try:
-            with open(file_path, 'r') as f:
-                self.config.update(json.load(f))
+            self.config.update(load_json(file_path))
         except Exception as e:
-            raise Exception(f"Error loading JSON config: {e}")
+            raise ConfigLoadError(f"Error loading JSON config: {e}")
 
     def load_from_yaml(self, file_path: str) -> None:
         try:
-            with open(file_path, 'r') as f:
-                self.config.update(yaml.safe_load(f))
+            self.config.update(load_yaml(file_path))
         except Exception as e:
-            raise Exception(f"Error loading YAML config: {e}")
+            raise ConfigLoadError(f"Error loading YAML config: {e}")
+
+    def load_from_env(self) -> None:
+        self.config.update(load_env())
 
     def get(self, key: str, default: Any=None) -> Any:
         keys = key.split('.')
         value = self.config
         try:
             for k in keys:
                 value = value[k]
@@ -37,20 +43,26 @@
         for k in keys[:-1]:
             if k not in d:
                 d[k] = {}
 
             d = d[k]
             d[keys[-1]] = value
 
+    def validate(self, schema):
+        try:
+            validate_config(self.config, schema)
+        except ValueError as e:
+            raise ConfigValidationError(f"Configuration validation error: {e}")
+
     def save_to_json(self, file_path: str) -> None:
         try:
             with open(file_path, 'w') as f:
                 json.dump(self.config, f, indent=4)
         except Exception as e:
             raise Exception(f"Error saving JSON config: {e}")
 
     def save_to_yaml(self, file_path: str) -> None:
         try:
             with open(file_path, 'w') as f:
                 yaml.safe_dump(self.config, f, default_flow_style=False)
         except Exception as e:
-            raise Exception(f"Error saving YAML config: {e}")
+            raise Exception(f"Error saving YAML config: {e}")
```

### Comparing `conf_master-0.2.0/PKG-INFO` & `conf_master-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-master
-Version: 0.2.0
+Version: 1.0.0
 Summary: 
 License: MIT
 Author: alvaroroco
 Author-email: alvaroroco@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

