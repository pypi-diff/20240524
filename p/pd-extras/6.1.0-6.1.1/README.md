# Comparing `tmp/pd_extras-6.1.0.tar.gz` & `tmp/pd_extras-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pd_extras-6.1.0.tar", max compression
+gzip compressed data, was "pd_extras-6.1.1.tar", max compression
```

## Comparing `pd_extras-6.1.0.tar` & `pd_extras-6.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2024-05-08 01:34:38.591303 pd_extras-6.1.0/LICENSE
--rw-r--r--   0        0        0     2912 2024-05-08 01:34:38.591303 pd_extras-6.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/check/__init__.py
--rw-r--r--   0        0        0     3245 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/check/sanitize.py
--rw-r--r--   0        0        0        0 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/extra/__init__.py
--rw-r--r--   0        0        0     3794 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/extra/flattener.py
--rw-r--r--   0        0        0     2635 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/extra/operations.py
--rw-r--r--   0        0        0        0 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/optimize/__init__.py
--rw-r--r--   0        0        0     1775 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/optimize/df_ops.py
--rw-r--r--   0        0        0        0 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/write/__init__.py
--rw-r--r--   0        0        0     1503 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/write/common.py
--rw-r--r--   0        0        0      192 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/write/driver.py
--rw-r--r--   0        0        0     5670 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/write/nosql_writer.py
--rw-r--r--   0        0        0     8787 2024-05-08 01:34:38.591303 pd_extras-6.1.0/pd_extras/write/sql_writer.py
--rw-r--r--   0        0        0      729 2024-05-08 01:34:38.595303 pd_extras-6.1.0/pyproject.toml
--rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 pd_extras-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-24 02:53:38.986354 pd_extras-6.1.1/LICENSE
+-rw-r--r--   0        0        0     2912 2024-05-24 02:53:38.986354 pd_extras-6.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/check/__init__.py
+-rw-r--r--   0        0        0     3245 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/check/sanitize.py
+-rw-r--r--   0        0        0        0 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/extra/__init__.py
+-rw-r--r--   0        0        0     3794 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/extra/flattener.py
+-rw-r--r--   0        0        0     2635 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/extra/operations.py
+-rw-r--r--   0        0        0        0 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/optimize/__init__.py
+-rw-r--r--   0        0        0     1775 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/optimize/df_ops.py
+-rw-r--r--   0        0        0        0 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/write/__init__.py
+-rw-r--r--   0        0        0     1503 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/write/common.py
+-rw-r--r--   0        0        0      192 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/write/driver.py
+-rw-r--r--   0        0        0     5670 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/write/nosql_writer.py
+-rw-r--r--   0        0        0     8787 2024-05-24 02:53:38.986354 pd_extras-6.1.1/pd_extras/write/sql_writer.py
+-rw-r--r--   0        0        0      749 2024-05-24 02:53:38.990354 pd_extras-6.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 pd_extras-6.1.1/PKG-INFO
```

### Comparing `pd_extras-6.1.0/LICENSE` & `pd_extras-6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pd_extras-6.1.0/README.md` & `pd_extras-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pd_extras-6.1.0/pd_extras/check/sanitize.py` & `pd_extras-6.1.1/pd_extras/check/sanitize.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.1.0/pd_extras/extra/flattener.py` & `pd_extras-6.1.1/pd_extras/extra/flattener.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.1.0/pd_extras/extra/operations.py` & `pd_extras-6.1.1/pd_extras/extra/operations.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.1.0/pd_extras/optimize/df_ops.py` & `pd_extras-6.1.1/pd_extras/optimize/df_ops.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.1.0/pd_extras/write/common.py` & `pd_extras-6.1.1/pd_extras/write/common.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.1.0/pd_extras/write/nosql_writer.py` & `pd_extras-6.1.1/pd_extras/write/nosql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.1.0/pd_extras/write/sql_writer.py` & `pd_extras-6.1.1/pd_extras/write/sql_writer.py`

 * *Files identical despite different names*

### Comparing `pd_extras-6.1.0/pyproject.toml` & `pd_extras-6.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [tool.poetry]
 name = "pd-extras"
-version = "6.1.0"
+version = "6.1.1"
 description = "Some utility functions on top of pandas."
 authors = ["Masum Billal <billalmasum93@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/proafxin/pd-extras"
 documentation = "https://pd-extras.readthedocs.io/en/latest/"
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.11"
 pandas = ">=1.5.3"
 pymongo = "^4.7.1"
 sqlalchemy-utils = "^0.41.2"
 mysqlclient = "^2.2.4"
 psycopg2 = "^2.9.9"
 pymssql = "^2.3.0"
 sqlalchemy = "^2.0.30"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.3.7"
+furo = "^2024.5.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 coverage = "^7.5.0"
 
 [build-system]
```

### Comparing `pd_extras-6.1.0/PKG-INFO` & `pd_extras-6.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: pd-extras
-Version: 6.1.0
+Version: 6.1.1
 Summary: Some utility functions on top of pandas.
 Home-page: https://github.com/proafxin/pd-extras
 License: MIT
 Author: Masum Billal
 Author-email: billalmasum93@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mysqlclient (>=2.2.4,<3.0.0)
 Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
 Requires-Dist: pymongo (>=4.7.1,<5.0.0)
 Requires-Dist: pymssql (>=2.3.0,<3.0.0)
```

