# Comparing `tmp/docmesh_server-0.0.7.tar.gz` & `tmp/docmesh_server-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_server-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_server-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_server-0.0.7.tar` & `docmesh_server-0.0.8.tar`

### file list

```diff
@@ -1,5 +1,15 @@
--rw-r--r--   0        0        0       16 2024-05-14 04:58:32.409536 docmesh_server-0.0.7/README.md
--rw-r--r--   0        0        0       64 2024-05-21 03:08:40.384308 docmesh_server-0.0.7/docmesh_server/__init__.py
--rw-r--r--   0        0        0    11901 2024-05-21 02:58:28.078270 docmesh_server-0.0.7/docmesh_server/main.py
--rw-r--r--   0        0        0      674 2024-05-21 03:08:22.983909 docmesh_server-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 docmesh_server-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-05-14 04:58:32.409536 docmesh_server-0.0.8/README.md
+-rw-r--r--   0        0        0       64 2024-05-23 05:41:01.598019 docmesh_server-0.0.8/docmesh_server/__init__.py
+-rw-r--r--   0        0        0      707 2024-05-23 04:52:30.791699 docmesh_server-0.0.8/docmesh_server/database.py
+-rw-r--r--   0        0        0     1220 2024-05-23 05:21:51.231797 docmesh_server-0.0.8/docmesh_server/dependencies.py
+-rw-r--r--   0        0        0        0 2024-05-23 04:41:13.676269 docmesh_server-0.0.8/docmesh_server/internals/__init__.py
+-rw-r--r--   0        0        0     1361 2024-05-23 04:53:44.441375 docmesh_server-0.0.8/docmesh_server/internals/admin.py
+-rw-r--r--   0        0        0     2131 2024-05-23 05:16:56.945092 docmesh_server-0.0.8/docmesh_server/internals/collections.py
+-rw-r--r--   0        0        0      960 2024-05-23 04:55:33.875867 docmesh_server-0.0.8/docmesh_server/internals/embeddings.py
+-rw-r--r--   0        0        0     1604 2024-05-23 05:17:04.393262 docmesh_server-0.0.8/docmesh_server/internals/venues.py
+-rw-r--r--   0        0        0     1090 2024-05-23 05:38:43.318860 docmesh_server-0.0.8/docmesh_server/main.py
+-rw-r--r--   0        0        0        0 2024-05-23 03:27:04.878936 docmesh_server-0.0.8/docmesh_server/routers/__init__.py
+-rw-r--r--   0        0        0     1138 2024-05-23 05:16:42.528764 docmesh_server-0.0.8/docmesh_server/routers/agents.py
+-rw-r--r--   0        0        0     2466 2024-05-23 05:16:34.096572 docmesh_server-0.0.8/docmesh_server/routers/papers.py
+-rw-r--r--   0        0        0      674 2024-05-22 08:55:49.532998 docmesh_server-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 docmesh_server-0.0.8/PKG-INFO
```

### Comparing `docmesh_server-0.0.7/pyproject.toml` & `docmesh_server-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docmesh_server-0.0.7/PKG-INFO` & `docmesh_server-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmesh_server
-Version: 0.0.7
+Version: 0.0.8
 Summary: Server of docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

