# Comparing `tmp/galileo_core-1.1.0.tar.gz` & `tmp/galileo_core-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_core-1.1.0.tar", max compression
+gzip compressed data, was "galileo_core-1.2.0.tar", max compression
```

## Comparing `galileo_core-1.1.0.tar` & `galileo_core-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0    10946 2024-05-22 17:11:51.017023 galileo_core-1.1.0/LICENSE
--rw-r--r--   0        0        0       80 2024-05-22 17:11:51.017023 galileo_core-1.1.0/README.md
--rw-r--r--   0        0        0     2389 2024-05-22 17:11:52.369038 galileo_core-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-22 17:11:52.369038 galileo_core-1.1.0/src/galileo_core/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/constants/__init__.py
--rw-r--r--   0        0        0      573 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/constants/http_headers.py
--rw-r--r--   0        0        0      190 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/constants/request_method.py
--rw-r--r--   0        0        0      424 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/constants/routes.py
--rw-r--r--   0        0        0        0 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/helpers/__init__.py
--rw-r--r--   0        0        0     2977 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/helpers/api_client.py
--rw-r--r--   0        0        0     6398 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/helpers/config.py
--rw-r--r--   0        0        0      369 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/helpers/dependencies.py
--rw-r--r--   0        0        0     1291 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/helpers/execution.py
--rw-r--r--   0        0        0       60 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/helpers/logger.py
--rw-r--r--   0        0        0     2146 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/helpers/project.py
--rw-r--r--   0        0        0       60 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/logger.py
--rw-r--r--   0        0        0        0 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/py.typed
--rw-r--r--   0        0        0        0 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/core/__init__.py
--rw-r--r--   0        0        0      738 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/core/project.py
--rw-r--r--   0        0        0        0 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/protect/__init__.py
--rw-r--r--   0        0        0     1382 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/protect/action.py
--rw-r--r--   0        0        0      246 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/protect/execution_status.py
--rw-r--r--   0        0        0      890 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/protect/metric.py
--rw-r--r--   0        0        0      795 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/protect/payload.py
--rw-r--r--   0        0        0     3905 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/protect/request.py
--rw-r--r--   0        0        0      521 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/protect/response.py
--rw-r--r--   0        0        0     2886 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/protect/rule.py
--rw-r--r--   0        0        0      831 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/protect/ruleset.py
--rw-r--r--   0        0        0      840 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/protect/stage.py
--rw-r--r--   0        0        0        0 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/shared/__init__.py
--rw-r--r--   0        0        0      176 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/shared/chains.py
--rw-r--r--   0        0        0      149 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/schemas/shared/metric.py
--rw-r--r--   0        0        0        0 2024-05-22 17:11:51.017023 galileo_core-1.1.0/src/galileo_core/utils/__init__.py
--rw-r--r--   0        0        0      204 2024-05-22 17:11:51.021023 galileo_core-1.1.0/src/galileo_core/utils/name.py
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 galileo_core-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-05-23 17:05:04.114945 galileo_core-1.2.0/LICENSE
+-rw-r--r--   0        0        0       80 2024-05-23 17:05:04.114945 galileo_core-1.2.0/README.md
+-rw-r--r--   0        0        0     2652 2024-05-23 17:05:05.434947 galileo_core-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-23 17:05:05.434947 galileo_core-1.2.0/src/galileo_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/constants/__init__.py
+-rw-r--r--   0        0        0      573 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/constants/http_headers.py
+-rw-r--r--   0        0        0      190 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/constants/request_method.py
+-rw-r--r--   0        0        0      424 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/helpers/__init__.py
+-rw-r--r--   0        0        0     2977 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/helpers/api_client.py
+-rw-r--r--   0        0        0     6398 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/helpers/config.py
+-rw-r--r--   0        0        0      369 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/helpers/dependencies.py
+-rw-r--r--   0        0        0     1291 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/helpers/execution.py
+-rw-r--r--   0        0        0       60 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/helpers/logger.py
+-rw-r--r--   0        0        0     2146 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/helpers/project.py
+-rw-r--r--   0        0        0       60 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/logger.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:05:04.114945 galileo_core-1.2.0/src/galileo_core/py.typed
+-rw-r--r--   0        0        0        0 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/core/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/core/project.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/protect/__init__.py
+-rw-r--r--   0        0        0     1382 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/protect/action.py
+-rw-r--r--   0        0        0      246 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/protect/execution_status.py
+-rw-r--r--   0        0        0      890 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/protect/metric.py
+-rw-r--r--   0        0        0      795 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/protect/payload.py
+-rw-r--r--   0        0        0     3905 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/protect/request.py
+-rw-r--r--   0        0        0      521 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/protect/response.py
+-rw-r--r--   0        0        0     2886 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/protect/rule.py
+-rw-r--r--   0        0        0      831 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/protect/ruleset.py
+-rw-r--r--   0        0        0      840 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/protect/stage.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/shared/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/shared/chains.py
+-rw-r--r--   0        0        0      149 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/schemas/shared/metric.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/testing/__init__.py
+-rw-r--r--   0        0        0     1144 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/testing/request_mocker.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/utils/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-23 17:05:04.118945 galileo_core-1.2.0/src/galileo_core/utils/name.py
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 galileo_core-1.2.0/PKG-INFO
```

### Comparing `galileo_core-1.1.0/LICENSE` & `galileo_core-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/pyproject.toml` & `galileo_core-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "galileo-core"
-version = "1.1.0"
+version = "1.2.0"
 description = "Shared schemas and configuration for Galileo's Python packages."
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_core", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
 pydantic = "^2.6.0"
 pydantic-settings = "^2.2.1"
 pyjwt = "^2.8.0"
 importlib-metadata = "^7.1.0"
 httpx = "^0.27.0"
 typing-extensions = "^4.11.0"
+pytest = { version = "^8.2.1", optional = true }
+respx = { version = "^0.21.1", optional = true }
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 coverage = "^7.3.4"
 pytest-cov = "^5.0.0"
 pytest-xdist = "^3.5.0"
@@ -30,14 +32,23 @@
 mypy = "^1.8.0"
 pre-commit = "^3.5.0"
 invoke = "^2.2.0"
 types-jwt = "^0.1.3"
 pydantic = { extras = ["mypy"], version = "^2.6.0" }
 
 
+[tool.poetry.extras]
+testing = ["pytest", "respx"]
+
+
+[tool.poetry.plugins]
+
+[tool.poetry.plugins."pytest11"]
+"mock_request" = "galileo_core.testing.request_mocker"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 # Test.
 [tool.pytest.ini_options]
```

### Comparing `galileo_core-1.1.0/src/galileo_core/constants/http_headers.py` & `galileo_core-1.2.0/src/galileo_core/constants/http_headers.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/helpers/api_client.py` & `galileo_core-1.2.0/src/galileo_core/helpers/api_client.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/helpers/config.py` & `galileo_core-1.2.0/src/galileo_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/helpers/execution.py` & `galileo_core-1.2.0/src/galileo_core/helpers/execution.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/helpers/project.py` & `galileo_core-1.2.0/src/galileo_core/helpers/project.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/schemas/core/project.py` & `galileo_core-1.2.0/src/galileo_core/schemas/core/project.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/schemas/protect/action.py` & `galileo_core-1.2.0/src/galileo_core/schemas/protect/action.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/schemas/protect/metric.py` & `galileo_core-1.2.0/src/galileo_core/schemas/protect/metric.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/schemas/protect/payload.py` & `galileo_core-1.2.0/src/galileo_core/schemas/protect/payload.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/schemas/protect/request.py` & `galileo_core-1.2.0/src/galileo_core/schemas/protect/request.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/schemas/protect/response.py` & `galileo_core-1.2.0/src/galileo_core/schemas/protect/response.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/schemas/protect/rule.py` & `galileo_core-1.2.0/src/galileo_core/schemas/protect/rule.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/schemas/protect/ruleset.py` & `galileo_core-1.2.0/src/galileo_core/schemas/protect/ruleset.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/src/galileo_core/schemas/protect/stage.py` & `galileo_core-1.2.0/src/galileo_core/schemas/protect/stage.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.1.0/PKG-INFO` & `galileo_core-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: galileo-core
-Version: 1.1.0
+Version: 1.2.0
 Summary: Shared schemas and configuration for Galileo's Python packages.
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: testing
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: importlib-metadata (>=7.1.0,<8.0.0)
 Requires-Dist: pydantic (>=2.6.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
+Requires-Dist: pytest (>=8.2.1,<9.0.0) ; extra == "testing"
+Requires-Dist: respx (>=0.21.1,<0.22.0) ; extra == "testing"
 Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # galileo-core
 
 Shared schemas and configuration for Galileo's Python packages.
```

