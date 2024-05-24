# Comparing `tmp/epyfun-0.3.4.tar.gz` & `tmp/epyfun-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epyfun-0.3.4.tar", max compression
+gzip compressed data, was "epyfun-0.3.5.tar", max compression
```

## Comparing `epyfun-0.3.4.tar` & `epyfun-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-05-24 09:12:04.796986 epyfun-0.3.4/LICENSE
--rw-r--r--   0        0        0     2242 2024-05-24 09:12:04.796986 epyfun-0.3.4/README.md
--rw-r--r--   0        0        0     1946 2024-05-24 09:12:18.485009 epyfun-0.3.4/pyproject.toml
--rw-r--r--   0        0        0       14 2024-05-24 09:12:04.800987 epyfun-0.3.4/src/epyfun/__init__.py
--rw-r--r--   0        0        0     3666 2024-05-24 09:12:04.800987 epyfun-0.3.4/src/epyfun/fs.py
--rw-r--r--   0        0        0     7093 2024-05-24 09:12:04.800987 epyfun-0.3.4/src/epyfun/plotly.py
--rw-r--r--   0        0        0        0 2024-05-24 09:12:04.800987 epyfun-0.3.4/src/epyfun/py.typed
--rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 epyfun-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-24 11:52:03.135346 epyfun-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2242 2024-05-24 11:52:03.135346 epyfun-0.3.5/README.md
+-rw-r--r--   0        0        0     2003 2024-05-24 11:52:12.571368 epyfun-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      149 2024-05-24 11:52:03.139346 epyfun-0.3.5/src/epyfun/__init__.py
+-rw-r--r--   0        0        0     3666 2024-05-24 11:52:03.139346 epyfun-0.3.5/src/epyfun/fs.py
+-rw-r--r--   0        0        0     7093 2024-05-24 11:52:03.139346 epyfun-0.3.5/src/epyfun/plotly.py
+-rw-r--r--   0        0        0        0 2024-05-24 11:52:03.139346 epyfun-0.3.5/src/epyfun/py.typed
+-rw-r--r--   0        0        0     1424 2024-05-24 11:52:03.139346 epyfun-0.3.5/src/epyfun/web.py
+-rw-r--r--   0        0        0     3281 1970-01-01 00:00:00.000000 epyfun-0.3.5/PKG-INFO
```

### Comparing `epyfun-0.3.4/LICENSE` & `epyfun-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.4/README.md` & `epyfun-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.4/pyproject.toml` & `epyfun-0.3.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "epyfun"
-version = "0.3.4"
+version = "0.3.5"
 description = "epyfun"
 authors = ["Eduardo Alfonso-Sierra <edalfon@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/edalfon/epyfun"
 repository = "https://github.com/edalfon/epyfun"
 documentation = "https://epyfun.readthedocs.io"
@@ -17,14 +17,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 chardet = ">=5.2.0"
 plotly = ">=5.18.0"
 pandas = ">=2.1.4"
 pandas-stubs = "^2.2.2.240514"
+requests = "^2.32.2"
+types-requests = "^2.32.0.20240523"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
```

### Comparing `epyfun-0.3.4/src/epyfun/fs.py` & `epyfun-0.3.5/src/epyfun/fs.py`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.4/src/epyfun/plotly.py` & `epyfun-0.3.5/src/epyfun/plotly.py`

 * *Files identical despite different names*

### Comparing `epyfun-0.3.4/PKG-INFO` & `epyfun-0.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epyfun
-Version: 0.3.4
+Version: 0.3.5
 Summary: epyfun
 Home-page: https://github.com/edalfon/epyfun
 License: MIT
 Author: Eduardo Alfonso-Sierra
 Author-email: edalfon@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chardet (>=5.2.0)
 Requires-Dist: pandas (>=2.1.4)
 Requires-Dist: pandas-stubs (>=2.2.2.240514,<3.0.0.0)
 Requires-Dist: plotly (>=5.18.0)
+Requires-Dist: requests (>=2.32.2,<3.0.0)
+Requires-Dist: types-requests (>=2.32.0.20240523,<3.0.0.0)
 Project-URL: Changelog, https://github.com/edalfon/epyfun/releases
 Project-URL: Documentation, https://epyfun.readthedocs.io
 Project-URL: Repository, https://github.com/edalfon/epyfun
 Description-Content-Type: text/markdown
 
 # epyfun
```

