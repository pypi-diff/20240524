# Comparing `tmp/docmesh_agent-0.0.8.tar.gz` & `tmp/docmesh_agent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_agent-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_agent-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_agent-0.0.8.tar` & `docmesh_agent-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.8/README.md
--rw-r--r--   0        0        0       22 2024-05-18 04:23:37.470614 docmesh_agent-0.0.8/docmesh_agent/__init__.py
--rw-r--r--   0        0        0     4291 2024-05-18 04:22:43.654304 docmesh_agent-0.0.8/docmesh_agent/agent.py
--rw-r--r--   0        0        0      136 2024-05-14 03:33:52.820396 docmesh_agent-0.0.8/docmesh_agent/embeddings/__init__.py
--rw-r--r--   0        0        0     1404 2024-05-14 03:33:17.744088 docmesh_agent-0.0.8/docmesh_agent/embeddings/embeddings.py
--rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.8/docmesh_agent/parser/__init__.py
--rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.8/docmesh_agent/parser/output_parser.py
--rw-r--r--   0        0        0      241 2024-05-16 11:24:43.283487 docmesh_agent-0.0.8/docmesh_agent/toolkit/__init__.py
--rw-r--r--   0        0        0      344 2024-05-16 11:24:22.979445 docmesh_agent-0.0.8/docmesh_agent/toolkit/common.py
--rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.8/docmesh_agent/toolkit/entity.py
--rw-r--r--   0        0        0     1035 2024-05-16 03:38:06.823760 docmesh_agent-0.0.8/docmesh_agent/toolkit/paper.py
--rw-r--r--   0        0        0      625 2024-05-13 03:31:55.262732 docmesh_agent-0.0.8/docmesh_agent/toolkit/recommend.py
--rw-r--r--   0        0        0      940 2024-05-16 11:23:32.443342 docmesh_agent-0.0.8/docmesh_agent/tools/__init__.py
--rw-r--r--   0        0        0     1139 2024-05-16 10:38:39.849612 docmesh_agent-0.0.8/docmesh_agent/tools/base.py
--rw-r--r--   0        0        0      721 2024-05-17 03:08:13.917254 docmesh_agent-0.0.8/docmesh_agent/tools/common.py
--rw-r--r--   0        0        0     2021 2024-05-16 10:36:55.425382 docmesh_agent-0.0.8/docmesh_agent/tools/entity.py
--rw-r--r--   0        0        0     3936 2024-05-13 04:13:58.033801 docmesh_agent-0.0.8/docmesh_agent/tools/graph_tools.py
--rw-r--r--   0        0        0     8572 2024-05-16 10:44:03.526324 docmesh_agent-0.0.8/docmesh_agent/tools/paper.py
--rw-r--r--   0        0        0     4351 2024-05-16 11:14:29.378232 docmesh_agent-0.0.8/docmesh_agent/tools/recommend.py
--rw-r--r--   0        0        0      750 2024-05-17 06:29:59.523015 docmesh_agent-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 docmesh_agent-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.9/README.md
+-rw-r--r--   0        0        0       22 2024-05-18 04:40:44.380583 docmesh_agent-0.0.9/docmesh_agent/__init__.py
+-rw-r--r--   0        0        0     4291 2024-05-18 04:22:43.654304 docmesh_agent-0.0.9/docmesh_agent/agent.py
+-rw-r--r--   0        0        0      136 2024-05-14 03:33:52.820396 docmesh_agent-0.0.9/docmesh_agent/embeddings/__init__.py
+-rw-r--r--   0        0        0     1404 2024-05-14 03:33:17.744088 docmesh_agent-0.0.9/docmesh_agent/embeddings/embeddings.py
+-rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.9/docmesh_agent/parser/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.9/docmesh_agent/parser/output_parser.py
+-rw-r--r--   0        0        0      241 2024-05-16 11:24:43.283487 docmesh_agent-0.0.9/docmesh_agent/toolkit/__init__.py
+-rw-r--r--   0        0        0      344 2024-05-16 11:24:22.979445 docmesh_agent-0.0.9/docmesh_agent/toolkit/common.py
+-rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.9/docmesh_agent/toolkit/entity.py
+-rw-r--r--   0        0        0     1035 2024-05-16 03:38:06.823760 docmesh_agent-0.0.9/docmesh_agent/toolkit/paper.py
+-rw-r--r--   0        0        0      625 2024-05-13 03:31:55.262732 docmesh_agent-0.0.9/docmesh_agent/toolkit/recommend.py
+-rw-r--r--   0        0        0      940 2024-05-16 11:23:32.443342 docmesh_agent-0.0.9/docmesh_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-16 10:38:39.849612 docmesh_agent-0.0.9/docmesh_agent/tools/base.py
+-rw-r--r--   0        0        0      721 2024-05-17 03:08:13.917254 docmesh_agent-0.0.9/docmesh_agent/tools/common.py
+-rw-r--r--   0        0        0     2021 2024-05-16 10:36:55.425382 docmesh_agent-0.0.9/docmesh_agent/tools/entity.py
+-rw-r--r--   0        0        0     3936 2024-05-13 04:13:58.033801 docmesh_agent-0.0.9/docmesh_agent/tools/graph_tools.py
+-rw-r--r--   0        0        0     8572 2024-05-16 10:44:03.526324 docmesh_agent-0.0.9/docmesh_agent/tools/paper.py
+-rw-r--r--   0        0        0     4351 2024-05-16 11:14:29.378232 docmesh_agent-0.0.9/docmesh_agent/tools/recommend.py
+-rw-r--r--   0        0        0      785 2024-05-18 04:39:17.792069 docmesh_agent-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 docmesh_agent-0.0.9/PKG-INFO
```

### Comparing `docmesh_agent-0.0.8/docmesh_agent/agent.py` & `docmesh_agent-0.0.9/docmesh_agent/agent.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/embeddings/embeddings.py` & `docmesh_agent-0.0.9/docmesh_agent/embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/parser/output_parser.py` & `docmesh_agent-0.0.9/docmesh_agent/parser/output_parser.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/toolkit/entity.py` & `docmesh_agent-0.0.9/docmesh_agent/toolkit/entity.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/toolkit/paper.py` & `docmesh_agent-0.0.9/docmesh_agent/toolkit/paper.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/toolkit/recommend.py` & `docmesh_agent-0.0.9/docmesh_agent/toolkit/recommend.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/tools/__init__.py` & `docmesh_agent-0.0.9/docmesh_agent/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/tools/base.py` & `docmesh_agent-0.0.9/docmesh_agent/tools/base.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/tools/common.py` & `docmesh_agent-0.0.9/docmesh_agent/tools/common.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/tools/entity.py` & `docmesh_agent-0.0.9/docmesh_agent/tools/entity.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/tools/graph_tools.py` & `docmesh_agent-0.0.9/docmesh_agent/tools/graph_tools.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/tools/paper.py` & `docmesh_agent-0.0.9/docmesh_agent/tools/paper.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/docmesh_agent/tools/recommend.py` & `docmesh_agent-0.0.9/docmesh_agent/tools/recommend.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.8/pyproject.toml` & `docmesh_agent-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -20,12 +20,13 @@
 dependencies = [
     "docmesh-core>=0.0.5",
     "colorama>=0.4.6",
     "pymupdf>=1.24.3",
     "faiss-cpu>=1.8.0",
     "langchain>=0.1.15",
     "langchain-openai>=0.1.3",
+    "langchain-community>=0.0.38",
     "langchainhub>=0.1.15",
 ]
 
 [tool.flake8]
 max-line-length = 120
```

### Comparing `docmesh_agent-0.0.8/PKG-INFO` & `docmesh_agent-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: docmesh_agent
-Version: 0.0.8
+Version: 0.0.9
 Summary: Agent helps you dig the paper connection!
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Dist: docmesh-core>=0.0.5
 Requires-Dist: colorama>=0.4.6
 Requires-Dist: pymupdf>=1.24.3
 Requires-Dist: faiss-cpu>=1.8.0
 Requires-Dist: langchain>=0.1.15
 Requires-Dist: langchain-openai>=0.1.3
+Requires-Dist: langchain-community>=0.0.38
 Requires-Dist: langchainhub>=0.1.15
 
 # docmesh agent
```

