# Comparing `tmp/pymedx-0.4.0.tar.gz` & `tmp/pymedx-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymedx-0.4.0.tar", max compression
+gzip compressed data, was "pymedx-0.5.0.tar", max compression
```

## Comparing `pymedx-0.4.0.tar` & `pymedx-0.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-05-17 20:45:25.247554 pymedx-0.4.0/LICENCE
--rw-r--r--   0        0        0     1925 2024-05-17 20:45:25.247554 pymedx-0.4.0/docs/index.md
--rw-r--r--   0        0        0     1909 2024-05-17 20:46:41.088431 pymedx-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      496 2024-05-17 20:46:41.088431 pymedx-0.4.0/src/pymedx/__init__.py
--rw-r--r--   0        0        0    12639 2024-05-17 20:45:25.251554 pymedx-0.4.0/src/pymedx/api.py
--rw-r--r--   0        0        0    13221 2024-05-17 20:45:25.251554 pymedx-0.4.0/src/pymedx/article.py
--rw-r--r--   0        0        0     6004 2024-05-17 20:45:25.251554 pymedx-0.4.0/src/pymedx/book.py
--rw-r--r--   0        0        0     4552 2024-05-17 20:45:25.251554 pymedx-0.4.0/src/pymedx/helpers.py
--rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 pymedx-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-24 14:10:50.559299 pymedx-0.5.0/LICENCE
+-rw-r--r--   0        0        0     1925 2024-05-24 14:10:50.559299 pymedx-0.5.0/docs/index.md
+-rw-r--r--   0        0        0     1909 2024-05-24 14:12:06.095555 pymedx-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-05-24 14:12:06.091555 pymedx-0.5.0/src/pymedx/__init__.py
+-rw-r--r--   0        0        0    19409 2024-05-24 14:10:50.563299 pymedx-0.5.0/src/pymedx/api.py
+-rw-r--r--   0        0        0    13221 2024-05-24 14:10:50.563299 pymedx-0.5.0/src/pymedx/article.py
+-rw-r--r--   0        0        0     6004 2024-05-24 14:10:50.563299 pymedx-0.5.0/src/pymedx/book.py
+-rw-r--r--   0        0        0    11109 2024-05-24 14:10:50.563299 pymedx-0.5.0/src/pymedx/helpers.py
+-rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 pymedx-0.5.0/PKG-INFO
```

### Comparing `pymedx-0.4.0/LICENCE` & `pymedx-0.5.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pymedx-0.4.0/docs/index.md` & `pymedx-0.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pymedx-0.4.0/pyproject.toml` & `pymedx-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymedx"
-version = "0.4.0"  # semantic-release
+version = "0.5.0"  # semantic-release
 description = "PyMedX is a tool set for handling multimedia files."
 readme = "docs/index.md"
 authors = ["Gijs Wobben <gijswobben@gmail.com>", "Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 packages = [
   {include = "pymedx", from="src"},
 ]
 license = "MIT"
```

### Comparing `pymedx-0.4.0/src/pymedx/article.py` & `pymedx-0.5.0/src/pymedx/article.py`

 * *Files identical despite different names*

### Comparing `pymedx-0.4.0/src/pymedx/book.py` & `pymedx-0.5.0/src/pymedx/book.py`

 * *Files identical despite different names*

### Comparing `pymedx-0.4.0/PKG-INFO` & `pymedx-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymedx
-Version: 0.4.0
+Version: 0.5.0
 Summary: PyMedX is a tool set for handling multimedia files.
 License: MIT
 Author: Gijs Wobben
 Author-email: gijswobben@gmail.com
 Requires-Python: >3.8.1,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

