# Comparing `tmp/idbt-0.0.3.tar.gz` & `tmp/idbt-0.0.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbt-0.0.3.tar", last modified: Fri May 24 03:17:49 2024, max compression
+gzip compressed data, was "idbt-0.0.3rc0.tar", last modified: Fri Apr  5 03:47:07 2024, max compression
```

## Comparing `idbt-0.0.3.tar` & `idbt-0.0.3rc0.tar`

### file list

```diff
@@ -1,40 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/
--rw-r--r--   0 root         (0) root         (0)      876 2024-05-24 03:17:49.742943 idbt-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-21 08:25:20.000000 idbt-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt/
--rw-r--r--   0 root         (0) root         (0)      340 2024-03-21 08:42:30.000000 idbt-0.0.3/idbt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt/compiler/
--rw-r--r--   0 root         (0) root         (0)     1217 2024-03-23 09:26:53.000000 idbt-0.0.3/idbt/compiler/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt/context/
--rw-r--r--   0 root         (0) root         (0)      467 2024-03-26 08:12:43.000000 idbt-0.0.3/idbt/context/i_unit_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt/events/
--rw-r--r--   0 root         (0) root         (0)     1353 2024-03-28 02:46:30.000000 idbt-0.0.3/idbt/events/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt/exception/
--rw-r--r--   0 root         (0) root         (0)      235 2024-04-05 04:11:28.000000 idbt-0.0.3/idbt/exception/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt/graph/
--rw-r--r--   0 root         (0) root         (0)     1310 2024-03-25 08:02:44.000000 idbt-0.0.3/idbt/graph/selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt/loader/
--rw-r--r--   0 root         (0) root         (0)     1464 2024-03-27 02:22:53.000000 idbt-0.0.3/idbt/loader/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1398 2024-04-13 03:45:00.000000 idbt-0.0.3/idbt/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt/manifest/
--rw-r--r--   0 root         (0) root         (0)      838 2024-03-27 02:28:06.000000 idbt-0.0.3/idbt/manifest/__init__.py
--rw-r--r--   0 root         (0) root         (0)       75 2024-03-22 04:44:29.000000 idbt-0.0.3/idbt/manifest/base.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-04-05 04:11:42.000000 idbt-0.0.3/idbt/manifest/i_unit_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt/parser/
--rw-r--r--   0 root         (0) root         (0)      282 2024-03-22 03:44:12.000000 idbt-0.0.3/idbt/parser/base.py
--rw-r--r--   0 root         (0) root         (0)     1656 2024-04-05 04:10:15.000000 idbt-0.0.3/idbt/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt/task/
--rw-r--r--   0 root         (0) root         (0)    15204 2024-03-28 03:06:12.000000 idbt-0.0.3/idbt/task/i_unit_test.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-03-26 10:28:26.000000 idbt-0.0.3/idbt/task/seed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt/unittest_func_hook/
--rw-r--r--   0 root         (0) root         (0)     2187 2024-03-21 08:11:56.000000 idbt-0.0.3/idbt/unittest_func_hook/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 03:17:49.742943 idbt-0.0.3/idbt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      876 2024-05-24 03:17:49.000000 idbt-0.0.3/idbt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      597 2024-05-24 03:17:49.000000 idbt-0.0.3/idbt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 03:17:49.000000 idbt-0.0.3/idbt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-05-24 03:17:49.000000 idbt-0.0.3/idbt.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 03:45:04.000000 idbt-0.0.3/idbt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-24 03:17:49.000000 idbt-0.0.3/idbt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-24 03:17:49.000000 idbt-0.0.3/idbt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 03:17:49.742943 idbt-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2341 2024-05-24 03:17:08.000000 idbt-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.728370 idbt-0.0.3rc0/
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-05 03:47:07.728370 idbt-0.0.3rc0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 03:46:28.000000 idbt-0.0.3rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.720370 idbt-0.0.3rc0/idbt/
+-rw-rw-rw-   0 root         (0) root         (0)      340 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.724370 idbt-0.0.3rc0/idbt/compiler/
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/compiler/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.724370 idbt-0.0.3rc0/idbt/context/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/context/i_unit_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.724370 idbt-0.0.3rc0/idbt/events/
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/events/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.724370 idbt-0.0.3rc0/idbt/graph/
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/graph/selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.724370 idbt-0.0.3rc0/idbt/loader/
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/loader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.724370 idbt-0.0.3rc0/idbt/manifest/
+-rw-rw-rw-   0 root         (0) root         (0)      838 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/manifest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/manifest/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/manifest/i_unit_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.724370 idbt-0.0.3rc0/idbt/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/parser/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1653 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.728370 idbt-0.0.3rc0/idbt/task/
+-rw-rw-rw-   0 root         (0) root         (0)    15204 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/task/i_unit_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2296 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/task/seed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.728370 idbt-0.0.3rc0/idbt/unittest_func_hook/
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/idbt/unittest_func_hook/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 03:47:07.728370 idbt-0.0.3rc0/idbt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-05 03:47:07.000000 idbt-0.0.3rc0/idbt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      570 2024-04-05 03:47:07.000000 idbt-0.0.3rc0/idbt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 03:47:07.000000 idbt-0.0.3rc0/idbt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-05 03:47:07.000000 idbt-0.0.3rc0/idbt.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 03:47:07.000000 idbt-0.0.3rc0/idbt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-05 03:47:07.000000 idbt-0.0.3rc0/idbt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-05 03:47:07.000000 idbt-0.0.3rc0/idbt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 03:47:07.728370 idbt-0.0.3rc0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2311 2024-04-05 03:43:43.000000 idbt-0.0.3rc0/setup.py
```

### Comparing `idbt-0.0.3/PKG-INFO` & `idbt-0.0.3rc0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbt
-Version: 0.0.3
+Version: 0.0.3rc0
 Summary: This is inter-k internal tool to help data practice becomes more testable
 Home-page: https://gitlab.inter-k.com/inter-k/internal-software/rnd/idbt
 Author: Bảo Phan
 Author-email: bao.phan1441@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -13,8 +13,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: dbt-core==1.7.15
+Requires-Dist: dbt-core>=1.7.0
```

### Comparing `idbt-0.0.3/idbt/compiler/__init__.py` & `idbt-0.0.3rc0/idbt/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.3/idbt/events/types.py` & `idbt-0.0.3rc0/idbt/events/types.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.3/idbt/graph/selector.py` & `idbt-0.0.3rc0/idbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.3/idbt/loader/__init__.py` & `idbt-0.0.3rc0/idbt/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.3/idbt/main.py` & `idbt-0.0.3rc0/idbt/main.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.3/idbt/manifest/__init__.py` & `idbt-0.0.3rc0/idbt/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.3/idbt/manifest/i_unit_test.py` & `idbt-0.0.3rc0/idbt/manifest/i_unit_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from idbt.exception import FileNotFoundException, ParsingException
 from .base import BaseDefinition
 from typing import List, Optional, Any
 from pydantic import BaseModel, model_validator
 import pathlib
 import os
 
 
@@ -29,21 +28,21 @@
     expected_output_file: Optional[str]
     assert_macro: AssertMacro
     file_path: str
 
     @model_validator(mode="after")
     def post_check(self) -> "IUnitTestDefinition":
         if self.expected_output_file and os.path.exists(self.expected_output_file) == False:
-            raise FileNotFoundException(
+            raise ValueError(
                 f"""expected_output_file: {self.expected_output_file} not found in unitest: {self.file_path}.
                     Please recheck the unittest yaml file {self.file_path}"""
             )
 
         for given_input in self.given:
             if os.path.exists(given_input.file) == False:
-                raise FileNotFoundException(
+                raise ValueError(
                     f"""given.file: {given_input.file} not found in unitest: {self.file_path}.
                     Please recheck the unittest yaml file {self.file_path}
                     """
                 )
 
         return self
```

### Comparing `idbt-0.0.3/idbt/parser/yaml_parser.py` & `idbt-0.0.3rc0/idbt/parser/yaml_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,25 +20,26 @@
     def parse(self, file_path: str) -> List[BaseDefinition]:
         parsed_definitions = []
 
         try:
             with open(file_path, "r") as file:
                 # Load YAML content
                 yaml_content: dict = yaml.safe_load(file)
+
                 # parse i_unit_tests
                 parsed_definitions = parsed_definitions + self._parse_unit_test_contents(
                     yaml_content, file_path
                 )
 
         except FileNotFoundError:
             raise CompilationError(f"File '{file_path}' not found.")
         except yaml.YAMLError as e:
             raise CompilationError(f"Error parsing YAML file '{file_path}': {e}")
         except ValidationError as e:
-            raise CompilationError(e.errors())
+            raise CompilationError(str(e))
         return parsed_definitions
 
     def _parse_unit_test_contents(
         self, yaml_content: str, file_path: str
     ) -> List[IUnitTestDefinition]:
         result: List[IUnitTestDefinition] = []
         if "i_unit_tests" in yaml_content:
```

### Comparing `idbt-0.0.3/idbt/task/i_unit_test.py` & `idbt-0.0.3rc0/idbt/task/i_unit_test.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.3/idbt/task/seed.py` & `idbt-0.0.3rc0/idbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.3/idbt/unittest_func_hook/__init__.py` & `idbt-0.0.3rc0/idbt/unittest_func_hook/__init__.py`

 * *Files identical despite different names*

### Comparing `idbt-0.0.3/idbt.egg-info/PKG-INFO` & `idbt-0.0.3rc0/idbt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbt
-Version: 0.0.3
+Version: 0.0.3rc0
 Summary: This is inter-k internal tool to help data practice becomes more testable
 Home-page: https://gitlab.inter-k.com/inter-k/internal-software/rnd/idbt
 Author: Bảo Phan
 Author-email: bao.phan1441@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -13,8 +13,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: dbt-core==1.7.15
+Requires-Dist: dbt-core>=1.7.0
```

### Comparing `idbt-0.0.3/idbt.egg-info/SOURCES.txt` & `idbt-0.0.3rc0/idbt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 idbt.egg-info/entry_points.txt
 idbt.egg-info/not-zip-safe
 idbt.egg-info/requires.txt
 idbt.egg-info/top_level.txt
 idbt/compiler/__init__.py
 idbt/context/i_unit_test.py
 idbt/events/types.py
-idbt/exception/__init__.py
 idbt/graph/selector.py
 idbt/loader/__init__.py
 idbt/manifest/__init__.py
 idbt/manifest/base.py
 idbt/manifest/i_unit_test.py
 idbt/parser/base.py
 idbt/parser/yaml_parser.py
```

### Comparing `idbt-0.0.3/setup.py` & `idbt-0.0.3rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,15 @@
     entry_points={
         "console_scripts": ["idbt = idbt.main:cli"],
     },
     install_requires=[
         # ----
         # dbt-core uses these packages deeply, throughout the codebase, and there have been breaking changes in past patch releases (even though these are major-version-one).
         # Pin to the patch or minor version, and bump in each new minor version of dbt-core.
-        # "dbt-core>=1.7.0",
-        "dbt-core==1.7.15",
+        "dbt-core>=1.7.0",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

