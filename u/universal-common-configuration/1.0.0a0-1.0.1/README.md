# Comparing `tmp/universal_common_configuration-1.0.0a0.tar.gz` & `tmp/universal_common_configuration-1.0.1.tar.gz`

## Comparing `universal_common_configuration-1.0.0a0.tar` & `universal_common_configuration-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.0a0/src/universal_common_configuration/__init__.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.0a0/src/universal_common_configuration/abstractions.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.0a0/src/universal_common_configuration/environment_variables.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.0a0/src/universal_common_configuration/json.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.0a0/src/universal_common_configuration/user_secrets.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.0a0/.gitignore
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.0a0/LICENSE
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.0a0/README.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/src/universal_common_configuration/__init__.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/src/universal_common_configuration/abstractions.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/src/universal_common_configuration/environment_variables.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/src/universal_common_configuration/json.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/src/universal_common_configuration/user_secrets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/tests/test_configuration.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/.gitignore
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/LICENSE
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/README.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 universal_common_configuration-1.0.1/PKG-INFO
```

### Comparing `universal_common_configuration-1.0.0a0/src/universal_common_configuration/__init__.py` & `universal_common_configuration-1.0.1/src/universal_common_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `universal_common_configuration-1.0.0a0/src/universal_common_configuration/abstractions.py` & `universal_common_configuration-1.0.1/src/universal_common_configuration/abstractions.py`

 * *Files identical despite different names*

### Comparing `universal_common_configuration-1.0.0a0/src/universal_common_configuration/environment_variables.py` & `universal_common_configuration-1.0.1/src/universal_common_configuration/environment_variables.py`

 * *Files identical despite different names*

### Comparing `universal_common_configuration-1.0.0a0/src/universal_common_configuration/json.py` & `universal_common_configuration-1.0.1/src/universal_common_configuration/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,18 @@
         self._data = dict()
         self._paths = list()
 
     @staticmethod
     def parse_file(path: str) -> dict[str, Optional[str]]:
         if os.path.isfile(path):
             with open(path, encoding="utf-8-sig") as file:
-                return JsonConfigurationParser().parse(json.load(file))
+                try:
+                    return JsonConfigurationParser().parse(json.load(file))
+                except:
+                    return dict()
 
         return dict()
 
     @staticmethod
     def parse_string(json_string: str) -> dict[str, Optional[str]]:
         return JsonConfigurationParser().parse(json.loads(json_string))
```

### Comparing `universal_common_configuration-1.0.0a0/src/universal_common_configuration/user_secrets.py` & `universal_common_configuration-1.0.1/src/universal_common_configuration/user_secrets.py`

 * *Files identical despite different names*

### Comparing `universal_common_configuration-1.0.0a0/LICENSE` & `universal_common_configuration-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `universal_common_configuration-1.0.0a0/pyproject.toml` & `universal_common_configuration-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "universal_common_configuration"
-version = "1.0.0-alpha"
+version = "1.0.1"
 authors = [
   { name="Andrew Ong", email="ong.andrew@gmail.com" },
 ]
 description = "A configuration management library inspired by Microsoft.Extensions.Configuration."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -15,8 +15,13 @@
 ]
 dependencies = [
   "userpaths"
 ]
 
 [build-system]
 requires = ["hatchling"]
-build-backend = "hatchling.build"
+build-backend = "hatchling.build"
+
+[tool.pytest.ini_options]
+pythonpath = [
+  "src"
+]
```

### Comparing `universal_common_configuration-1.0.0a0/PKG-INFO` & `universal_common_configuration-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: universal_common_configuration
-Version: 1.0.0a0
+Version: 1.0.1
 Summary: A configuration management library inspired by Microsoft.Extensions.Configuration.
 Author-email: Andrew Ong <ong.andrew@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

