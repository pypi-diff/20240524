# Comparing `tmp/conf_master-1.0.0.tar.gz` & `tmp/conf_master-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_master-1.0.0.tar", max compression
+gzip compressed data, was "conf_master-1.0.1.tar", max compression
```

## Comparing `conf_master-1.0.0.tar` & `conf_master-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1107 2024-05-24 17:39:25.661378 conf_master-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1358 2024-05-24 18:40:28.445182 conf_master-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      519 2024-05-24 18:12:30.119187 conf_master-1.0.0/README.md
--rw-r--r--   0        0        0      109 2024-05-24 17:39:25.660379 conf_master-1.0.0/src/conf_master/__init__.py
--rw-r--r--   0        0        0     2112 2024-05-24 18:39:37.523033 conf_master-1.0.0/src/conf_master/conf_master.py
--rw-r--r--   0        0        0      332 2024-05-24 18:37:34.117998 conf_master-1.0.0/src/conf_master/exceptions.py
--rw-r--r--   0        0        0      634 2024-05-24 18:35:56.694292 conf_master-1.0.0/src/conf_master/loaders.py
--rw-r--r--   0        0        0      345 2024-05-24 18:25:51.397917 conf_master-1.0.0/src/conf_master/validators.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 conf_master-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1107 2024-05-24 17:39:25.661378 conf_master-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1358 2024-05-24 18:47:26.433966 conf_master-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      519 2024-05-24 18:12:30.119187 conf_master-1.0.1/README.md
+-rw-r--r--   0        0        0      109 2024-05-24 17:39:25.660379 conf_master-1.0.1/src/conf_master/__init__.py
+-rw-r--r--   0        0        0     2072 2024-05-24 18:46:11.919554 conf_master-1.0.1/src/conf_master/conf_master.py
+-rw-r--r--   0        0        0      332 2024-05-24 18:37:34.117998 conf_master-1.0.1/src/conf_master/exceptions.py
+-rw-r--r--   0        0        0      531 2024-05-24 18:46:56.010723 conf_master-1.0.1/src/conf_master/loaders.py
+-rw-r--r--   0        0        0      345 2024-05-24 18:25:51.397917 conf_master-1.0.1/src/conf_master/validators.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 conf_master-1.0.1/PKG-INFO
```

### Comparing `conf_master-1.0.0/LICENSE.txt` & `conf_master-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conf_master-1.0.0/pyproject.toml` & `conf_master-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "conf-master"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 readme = "README.md"
 authors = ["alvaroroco <alvaroroco@gmail.com>"]
 license = "MIT"
 keywords = []
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `conf_master-1.0.0/README.md` & `conf_master-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `conf_master-1.0.0/src/conf_master/conf_master.py` & `conf_master-1.0.1/src/conf_master/conf_master.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,40 +7,40 @@
 from .validators import validate_config
 from .exceptions import ConfigLoadError, ConfigValidationError
 
 class ConfMaster():
     def __init__(self):
         self.config = {}
 
-    def load_from_json(self, file_path: str) -> None:
+    def load_from_json(self, file_path) -> None:
         try:
             self.config.update(load_json(file_path))
         except Exception as e:
             raise ConfigLoadError(f"Error loading JSON config: {e}")
 
-    def load_from_yaml(self, file_path: str) -> None:
+    def load_from_yaml(self, file_path) -> None:
         try:
             self.config.update(load_yaml(file_path))
         except Exception as e:
             raise ConfigLoadError(f"Error loading YAML config: {e}")
 
     def load_from_env(self) -> None:
         self.config.update(load_env())
 
-    def get(self, key: str, default: Any=None) -> Any:
+    def get(self, key, default=None) -> Any:
         keys = key.split('.')
         value = self.config
         try:
             for k in keys:
                 value = value[k]
             return value
         except KeyError:
             return default
 
-    def set(self, key: str, value: Any) -> None:
+    def set(self, key, value) -> None:
         keys = key.split('.')
         d = self.config
 
         for k in keys[:-1]:
             if k not in d:
                 d[k] = {}
 
@@ -49,20 +49,20 @@
 
     def validate(self, schema):
         try:
             validate_config(self.config, schema)
         except ValueError as e:
             raise ConfigValidationError(f"Configuration validation error: {e}")
 
-    def save_to_json(self, file_path: str) -> None:
+    def save_to_json(self, file_path) -> None:
         try:
             with open(file_path, 'w') as f:
                 json.dump(self.config, f, indent=4)
         except Exception as e:
             raise Exception(f"Error saving JSON config: {e}")
 
-    def save_to_yaml(self, file_path: str) -> None:
+    def save_to_yaml(self, file_path) -> None:
         try:
             with open(file_path, 'w') as f:
                 yaml.safe_dump(self.config, f, default_flow_style=False)
         except Exception as e:
             raise Exception(f"Error saving YAML config: {e}")
```

### Comparing `conf_master-1.0.0/PKG-INFO` & `conf_master-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-master
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 License: MIT
 Author: alvaroroco
 Author-email: alvaroroco@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

