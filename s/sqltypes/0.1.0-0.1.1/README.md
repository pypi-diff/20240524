# Comparing `tmp/sqltypes-0.1.0.tar.gz` & `tmp/sqltypes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqltypes-0.1.0.tar", last modified: Sun May 12 06:53:59 2024, max compression
+gzip compressed data, was "sqltypes-0.1.1.tar", last modified: Fri May 24 18:14:27 2024, max compression
```

## Comparing `sqltypes-0.1.0.tar` & `sqltypes-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 06:53:59.766931 sqltypes-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      841 2024-05-12 06:53:59.766931 sqltypes-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      478 2024-05-12 06:53:14.000000 sqltypes-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      575 2024-05-12 06:53:31.000000 sqltypes-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-12 06:53:59.766931 sqltypes-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 06:53:59.766931 sqltypes-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 06:53:59.766931 sqltypes-0.1.0/src/sqltypes/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-05-12 06:53:14.000000 sqltypes-0.1.0/src/sqltypes/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      253 2024-05-12 06:53:14.000000 sqltypes-0.1.0/src/sqltypes/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      811 2024-05-12 06:53:14.000000 sqltypes-0.1.0/src/sqltypes/meta.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      446 2024-05-12 06:53:14.000000 sqltypes-0.1.0/src/sqltypes/pydantic.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      641 2024-05-12 06:53:14.000000 sqltypes-0.1.0/src/sqltypes/string.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-12 06:53:59.766931 sqltypes-0.1.0/src/sqltypes.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      841 2024-05-12 06:53:59.000000 sqltypes-0.1.0/src/sqltypes.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      323 2024-05-12 06:53:59.000000 sqltypes-0.1.0/src/sqltypes.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-12 06:53:59.000000 sqltypes-0.1.0/src/sqltypes.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       32 2024-05-12 06:53:59.000000 sqltypes-0.1.0/src/sqltypes.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-12 06:53:59.000000 sqltypes-0.1.0/src/sqltypes.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 18:14:27.714126 sqltypes-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      841 2024-05-24 18:14:27.714126 sqltypes-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      478 2024-05-12 06:53:14.000000 sqltypes-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      575 2024-05-24 18:14:22.000000 sqltypes-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-24 18:14:27.714126 sqltypes-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 18:14:27.704126 sqltypes-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 18:14:27.704126 sqltypes-0.1.1/src/sqltypes/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-05-12 06:53:14.000000 sqltypes-0.1.1/src/sqltypes/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      311 2024-05-24 18:14:14.000000 sqltypes-0.1.1/src/sqltypes/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      549 2024-05-24 18:14:03.000000 sqltypes-0.1.1/src/sqltypes/literal.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      811 2024-05-12 06:53:14.000000 sqltypes-0.1.1/src/sqltypes/meta.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      446 2024-05-12 06:53:14.000000 sqltypes-0.1.1/src/sqltypes/pydantic.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      641 2024-05-12 06:53:14.000000 sqltypes-0.1.1/src/sqltypes/string.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-24 18:14:27.714126 sqltypes-0.1.1/src/sqltypes.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      841 2024-05-24 18:14:27.000000 sqltypes-0.1.1/src/sqltypes.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      347 2024-05-24 18:14:27.000000 sqltypes-0.1.1/src/sqltypes.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-24 18:14:27.000000 sqltypes-0.1.1/src/sqltypes.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       32 2024-05-24 18:14:27.000000 sqltypes-0.1.1/src/sqltypes.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-24 18:14:27.000000 sqltypes-0.1.1/src/sqltypes.egg-info/top_level.txt
```

### Comparing `sqltypes-0.1.0/PKG-INFO` & `sqltypes-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqltypes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Custom types for SQLModel/SQLalchemy
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: sqlalchemy
```

### Comparing `sqltypes-0.1.0/pyproject.toml` & `sqltypes-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqltypes"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Custom types for SQLModel/SQLalchemy"
 dependencies = [
   "pydantic", "sqlalchemy", "lazy-loader"
 ]
```

### Comparing `sqltypes-0.1.0/src/sqltypes/meta.py` & `sqltypes-0.1.1/src/sqltypes/meta.py`

 * *Files identical despite different names*

### Comparing `sqltypes-0.1.0/src/sqltypes/string.py` & `sqltypes-0.1.1/src/sqltypes/string.py`

 * *Files identical despite different names*

### Comparing `sqltypes-0.1.0/src/sqltypes.egg-info/PKG-INFO` & `sqltypes-0.1.1/src/sqltypes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqltypes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Custom types for SQLModel/SQLalchemy
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: sqlalchemy
```

