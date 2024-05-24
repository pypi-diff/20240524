# Comparing `tmp/epyfun-0.3.3.tar.gz` & `tmp/epyfun-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epyfun-0.3.3.tar", max compression
+gzip compressed data, was "epyfun-0.3.4.tar", max compression
```

## Comparing `epyfun-0.3.3.tar` & `epyfun-0.3.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1078 2024-05-23 16:33:24.360636 epyfun-0.3.3/LICENSE
--rw-r--r--   0        0        0     2242 2024-05-23 16:33:24.360636 epyfun-0.3.3/README.md
--rw-r--r--   0        0        0     1840 2024-05-23 16:33:34.060649 epyfun-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       14 2024-05-23 16:33:24.364636 epyfun-0.3.3/src/epyfun/__init__.py
--rw-r--r--   0        0        0     3666 2024-05-23 16:33:24.364636 epyfun-0.3.3/src/epyfun/fs.py
--rw-r--r--   0        0        0        0 2024-05-23 16:33:24.364636 epyfun-0.3.3/src/epyfun/py.typed
--rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 epyfun-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-24 09:12:04.796986 epyfun-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2242 2024-05-24 09:12:04.796986 epyfun-0.3.4/README.md
+-rw-r--r--   0        0        0     1946 2024-05-24 09:12:18.485009 epyfun-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       14 2024-05-24 09:12:04.800987 epyfun-0.3.4/src/epyfun/__init__.py
+-rw-r--r--   0        0        0     3666 2024-05-24 09:12:04.800987 epyfun-0.3.4/src/epyfun/fs.py
+-rw-r--r--   0        0        0     7093 2024-05-24 09:12:04.800987 epyfun-0.3.4/src/epyfun/plotly.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:12:04.800987 epyfun-0.3.4/src/epyfun/py.typed
+-rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 epyfun-0.3.4/PKG-INFO
```

### Comparing `epyfun-0.3.3/LICENSE` & `epyfun-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.3/README.md` & `epyfun-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.3/pyproject.toml` & `epyfun-0.3.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epyfun"
-version = "0.3.3"
+version = "0.3.4"
 description = "epyfun"
 authors = ["Eduardo Alfonso-Sierra <edalfon@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/edalfon/epyfun"
 repository = "https://github.com/edalfon/epyfun"
 documentation = "https://epyfun.readthedocs.io"
@@ -16,14 +16,15 @@
 Changelog = "https://github.com/edalfon/epyfun/releases"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 chardet = ">=5.2.0"
 plotly = ">=5.18.0"
 pandas = ">=2.1.4"
+pandas-stubs = "^2.2.2.240514"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
@@ -72,10 +73,14 @@
 [tool.mypy]
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_context = true
 
+[[tool.mypy.overrides]]
+module = "plotly.*"
+ignore_missing_imports = true
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `epyfun-0.3.3/src/epyfun/fs.py` & `epyfun-0.3.4/src/epyfun/fs.py`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.3/PKG-INFO` & `epyfun-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epyfun
-Version: 0.3.3
+Version: 0.3.4
 Summary: epyfun
 Home-page: https://github.com/edalfon/epyfun
 License: MIT
 Author: Eduardo Alfonso-Sierra
 Author-email: edalfon@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chardet (>=5.2.0)
 Requires-Dist: pandas (>=2.1.4)
+Requires-Dist: pandas-stubs (>=2.2.2.240514,<3.0.0.0)
 Requires-Dist: plotly (>=5.18.0)
 Project-URL: Changelog, https://github.com/edalfon/epyfun/releases
 Project-URL: Documentation, https://epyfun.readthedocs.io
 Project-URL: Repository, https://github.com/edalfon/epyfun
 Description-Content-Type: text/markdown
 
 # epyfun
```

