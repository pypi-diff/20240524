# Comparing `tmp/request_api_builder-2.0.2.tar.gz` & `tmp/request_api_builder-2.0.3.tar.gz`

## Comparing `request_api_builder-2.0.2.tar` & `request_api_builder-2.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 request_api_builder-2.0.2/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 request_api_builder-2.0.2/src/request-api-builder/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 request_api_builder-2.0.2/src/request-api-builder/request_builder.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 request_api_builder-2.0.2/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 request_api_builder-2.0.2/LICENSE
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 request_api_builder-2.0.2/README.md
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 request_api_builder-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 request_api_builder-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/src/request_api_builder/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/src/request_api_builder/request_builder.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/LICENSE
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/README.md
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/PKG-INFO
```

### Comparing `request_api_builder-2.0.2/src/request-api-builder/request_builder.py` & `request_api_builder-2.0.3/src/request_api_builder/request_builder.py`

 * *Files identical despite different names*

### Comparing `request_api_builder-2.0.2/.gitignore` & `request_api_builder-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `request_api_builder-2.0.2/LICENSE` & `request_api_builder-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `request_api_builder-2.0.2/README.md` & `request_api_builder-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `request_api_builder-2.0.2/pyproject.toml` & `request_api_builder-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "request-api-builder"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
  { name="Kateryna Levashova", email="voxquietam.md@gmail.com" },
 ]
 description = "Request builder for testing API"
 readme = "README.md"
 requires-python = ">=3.10.0"
 classifiers = [
@@ -41,15 +41,15 @@
 follow_imports = 'silent'
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/request-api-builder"]
+packages = ["src/request_api_builder"]
 
 [tool.semantic_release.branches.main]
 match = "(master)"
 prerelease_token = "rc"
 prerelease = false
 
 [tool.semantic_release]
```

### Comparing `request_api_builder-2.0.2/PKG-INFO` & `request_api_builder-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: request-api-builder
-Version: 2.0.2
+Version: 2.0.3
 Summary: Request builder for testing API
 Author-email: Kateryna Levashova <voxquietam.md@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
```

