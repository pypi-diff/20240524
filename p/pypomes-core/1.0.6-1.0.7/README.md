# Comparing `tmp/pypomes_core-1.0.6.tar.gz` & `tmp/pypomes_core-1.0.7.tar.gz`

## Comparing `pypomes_core-1.0.6.tar` & `pypomes_core-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24661 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.0.7/PKG-INFO
```

### Comparing `pypomes_core-1.0.6/src/pypomes_core/.ruff.toml` & `pypomes_core-1.0.7/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/__init__.py` & `pypomes_core-1.0.7/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/email_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/env_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/file_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/json_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/list_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/str_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.0.7/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/validation_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -616,15 +616,16 @@
     # define the dictionary keys
     name: str = "code" if VALIDATION_MSG_LANGUAGE == "en" else "codigo"
     desc: str = "description" if VALIDATION_MSG_LANGUAGE == "en" else "descricao"
 
     # traverse the list of dicts
     for error in errors:
         if isinstance(error, dict):
-            result.append(f"{error.get(name)}: {str_sanitize(error.get(desc))}")
+            desc: str = str_sanitize(error.get(desc) or "''")
+            result.append(f"{error.get(name)}: {desc}")
         else:
             result.append(error)
 
     return result
 
 
 def __validate_log(errors: list[str],
```

### Comparing `pypomes_core-1.0.6/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.0.7/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/LICENSE` & `pypomes_core-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.0.6/pyproject.toml` & `pypomes_core-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.0.6/PKG-INFO` & `pypomes_core-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.0.6
+Version: 1.0.7
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

