# Comparing `tmp/digrdf-0.1.6.tar.gz` & `tmp/digrdf-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digrdf-0.1.6.tar", max compression
+gzip compressed data, was "digrdf-0.1.7.tar", max compression
```

## Comparing `digrdf-0.1.6.tar` & `digrdf-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1139 2024-05-23 14:15:58.616664 digrdf-0.1.6/README.md
--rw-r--r--   0        0        0       32 2024-05-23 11:53:28.672509 digrdf-0.1.6/digrdf/__init__.py
--rw-r--r--   0        0        0     9250 2024-05-23 14:13:48.314127 digrdf-0.1.6/digrdf/__main__.py
--rw-r--r--   0        0        0      187 2024-05-23 13:59:39.819260 digrdf-0.1.6/digrdf/instance_query.sparql
--rw-r--r--   0        0        0      703 2024-05-15 11:51:48.620609 digrdf-0.1.6/digrdf/prefixes.py
--rw-r--r--   0        0        0      316 2024-05-23 11:01:26.761882 digrdf-0.1.6/digrdf/schema_query.sparql
--rw-r--r--   0        0        0      409 2024-05-23 14:16:54.995870 digrdf-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 digrdf-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1139 2024-05-23 14:15:58.616664 digrdf-0.1.7/README.md
+-rw-r--r--   0        0        0       28 2024-05-23 23:07:48.931673 digrdf-0.1.7/digrdf/__init__.py
+-rw-r--r--   0        0        0     2310 2024-05-23 23:07:01.840051 digrdf-0.1.7/digrdf/__main__.py
+-rw-r--r--   0        0        0     7127 2024-05-23 23:14:40.242263 digrdf-0.1.7/digrdf/core.py
+-rw-r--r--   0        0        0      233 2024-05-23 14:38:01.810545 digrdf-0.1.7/digrdf/instance_query.sparql
+-rw-r--r--   0        0        0      703 2024-05-15 11:51:48.620609 digrdf-0.1.7/digrdf/prefixes.py
+-rw-r--r--   0        0        0      316 2024-05-23 11:01:26.761882 digrdf-0.1.7/digrdf/schema_query.sparql
+-rw-r--r--   0        0        0      409 2024-05-23 23:16:15.318788 digrdf-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 digrdf-0.1.7/PKG-INFO
```

### Comparing `digrdf-0.1.6/README.md` & `digrdf-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `digrdf-0.1.6/digrdf/prefixes.py` & `digrdf-0.1.7/digrdf/prefixes.py`

 * *Files identical despite different names*

### Comparing `digrdf-0.1.6/PKG-INFO` & `digrdf-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digrdf
-Version: 0.1.6
+Version: 0.1.7
 Summary: RDF Schema Diagram creation tool
 Author: Lawson Lewis
 Author-email: lawson@kurrawong.ai
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

