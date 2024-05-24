# Comparing `tmp/ragstack_ai_llamaindex-1.0.3.tar.gz` & `tmp/ragstack_ai_llamaindex-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_llamaindex-1.0.3.tar", max compression
+gzip compressed data, was "ragstack_ai_llamaindex-1.0.4.tar", max compression
```

## Comparing `ragstack_ai_llamaindex-1.0.3.tar` & `ragstack_ai_llamaindex-1.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      374 2024-05-21 20:08:01.829349 ragstack_ai_llamaindex-1.0.3/README.md
--rw-r--r--   0        0        0     1820 2024-05-21 20:08:01.829349 ragstack_ai_llamaindex-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      271 2024-05-21 20:08:01.829349 ragstack_ai_llamaindex-1.0.3/ragstack_llamaindex/__init__.py
--rw-r--r--   0        0        0      356 2024-05-21 20:08:01.829349 ragstack_ai_llamaindex-1.0.3/ragstack_llamaindex/colbert/__init__.py
--rw-r--r--   0        0        0     1801 2024-05-21 20:08:01.829349 ragstack_ai_llamaindex-1.0.3/ragstack_llamaindex/colbert/colbert_retriever.py
--rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 ragstack_ai_llamaindex-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      374 2024-05-24 12:59:06.732767 ragstack_ai_llamaindex-1.0.4/README.md
+-rw-r--r--   0        0        0     1820 2024-05-24 12:59:06.732767 ragstack_ai_llamaindex-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-05-24 12:59:06.732767 ragstack_ai_llamaindex-1.0.4/ragstack_llamaindex/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-24 12:59:06.732767 ragstack_ai_llamaindex-1.0.4/ragstack_llamaindex/colbert/__init__.py
+-rw-r--r--   0        0        0     1801 2024-05-24 12:59:06.732767 ragstack_ai_llamaindex-1.0.4/ragstack_llamaindex/colbert/colbert_retriever.py
+-rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 ragstack_ai_llamaindex-1.0.4/PKG-INFO
```

### Comparing `ragstack_ai_llamaindex-1.0.3/pyproject.toml` & `ragstack_ai_llamaindex-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ragstack-ai-llamaindex"
-version = "1.0.3"
+version = "1.0.4"
 description = "DataStax RAGStack Llama Index"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_llamaindex" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 astrapy = "^1"
 cassio = "~0.1.4"
-unstructured = "0.12.5"
-ragstack-ai-colbert = "1.0.3"
+unstructured = "0.14.2"
+ragstack-ai-colbert = "1.0.4"
 
 # llama-index
 llama-index = "0.10.31"
 llama-index-vector-stores-astra-db = "0.1.7"
 llama-index-vector-stores-cassandra = "0.1.3"
 llama-index-embeddings-langchain = "0.1.2"
 llama-parse = "0.4.1"
```

### Comparing `ragstack_ai_llamaindex-1.0.3/ragstack_llamaindex/colbert/colbert_retriever.py` & `ragstack_ai_llamaindex-1.0.4/ragstack_llamaindex/colbert/colbert_retriever.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_llamaindex-1.0.3/PKG-INFO` & `ragstack_ai_llamaindex-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-llamaindex
-Version: 1.0.3
+Version: 1.0.4
 Summary: DataStax RAGStack Llama Index
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -27,16 +27,16 @@
 Requires-Dist: llama-index-llms-bedrock (==0.1.7) ; extra == "bedrock"
 Requires-Dist: llama-index-llms-gemini (==0.1.7) ; extra == "google"
 Requires-Dist: llama-index-llms-vertex (==0.1.5) ; extra == "google"
 Requires-Dist: llama-index-multi-modal-llms-gemini (==0.1.5) ; extra == "google"
 Requires-Dist: llama-index-vector-stores-astra-db (==0.1.7)
 Requires-Dist: llama-index-vector-stores-cassandra (==0.1.3)
 Requires-Dist: llama-parse (==0.4.1)
-Requires-Dist: ragstack-ai-colbert (==1.0.3) ; extra == "colbert"
-Requires-Dist: unstructured (==0.12.5)
+Requires-Dist: ragstack-ai-colbert (==1.0.4) ; extra == "colbert"
+Requires-Dist: unstructured (==0.14.2)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack LLamaIndex
 
 RAGStack Llama Index package, part of [`ragstack-ai`](https://pypi.org/project/ragstack-ai/).
```

