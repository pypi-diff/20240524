# Comparing `tmp/request_api_builder-2.0.3.tar.gz` & `tmp/request_api_builder-2.0.4.tar.gz`

## Comparing `request_api_builder-2.0.3.tar` & `request_api_builder-2.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/src/request_api_builder/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/src/request_api_builder/request_builder.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/LICENSE
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/README.md
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 request_api_builder-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 request_api_builder-2.0.4/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 request_api_builder-2.0.4/src/request_api_builder/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 request_api_builder-2.0.4/src/request_api_builder/rab.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 request_api_builder-2.0.4/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 request_api_builder-2.0.4/LICENSE
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 request_api_builder-2.0.4/README.md
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 request_api_builder-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 request_api_builder-2.0.4/PKG-INFO
```

### Comparing `request_api_builder-2.0.3/src/request_api_builder/request_builder.py` & `request_api_builder-2.0.4/src/request_api_builder/rab.py`

 * *Files identical despite different names*

### Comparing `request_api_builder-2.0.3/.gitignore` & `request_api_builder-2.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `request_api_builder-2.0.3/LICENSE` & `request_api_builder-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `request_api_builder-2.0.3/README.md` & `request_api_builder-2.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# request-api-builder
+# request_api_builder
 Request builder for quick testing API
 
 ## Use
  1. Import RequestBuilder
 ```python
-from request_builder import RequestBuilder
+from request_api_builder.rab import BuildRequests
 ```
 2. Set cookie and base url
 ```python
 BuildRequests.set_cookie(cookie)
 BuildRequests.set_base_url(base_url)
 ```
 3. Create request
```

### Comparing `request_api_builder-2.0.3/pyproject.toml` & `request_api_builder-2.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "request-api-builder"
-version = "2.0.3"
+name = "request_api_builder"
+version = "2.0.4"
 authors = [
  { name="Kateryna Levashova", email="voxquietam.md@gmail.com" },
 ]
 description = "Request builder for testing API"
 readme = "README.md"
 requires-python = ">=3.10.0"
 classifiers = [
@@ -59,15 +59,15 @@
 branch = "master"
 match = "(master)"
 prerelease = false
 allow_zero_version = true
 tag_format = "v{version}"
 logging_use_named_masks = false
 version_variable = "setup.py:__version__"
-commit_subject = "chore(release): bump requiest-api-builder to version {version}"
+commit_subject = "chore(release): bump request_api_builder to version {version}"
 commit_author = "Kateryna Levashova <voxquietam.md@gmail.com>"
 
 [tool.semantic_release.changelog]
 changelog_file = "CHANGELOG.md"
 exclude_commit_patterns = []
 
 [tool.semantic_release.changelog.environment]
```

### Comparing `request_api_builder-2.0.3/PKG-INFO` & `request_api_builder-2.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.3
-Name: request-api-builder
-Version: 2.0.3
+Name: request_api_builder
+Version: 2.0.4
 Summary: Request builder for testing API
 Author-email: Kateryna Levashova <voxquietam.md@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 
-# request-api-builder
+# request_api_builder
 Request builder for quick testing API
 
 ## Use
  1. Import RequestBuilder
 ```python
-from request_builder import RequestBuilder
+from request_api_builder.rab import BuildRequests
 ```
 2. Set cookie and base url
 ```python
 BuildRequests.set_cookie(cookie)
 BuildRequests.set_base_url(base_url)
 ```
 3. Create request
```

