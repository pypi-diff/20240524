# Comparing `tmp/ragstack_ai_langchain-1.0.5.tar.gz` & `tmp/ragstack_ai_langchain-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_langchain-1.0.5.tar", max compression
+gzip compressed data, was "ragstack_ai_langchain-1.0.6.tar", max compression
```

## Comparing `ragstack_ai_langchain-1.0.5.tar` & `ragstack_ai_langchain-1.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      371 2024-05-24 12:58:54.330623 ragstack_ai_langchain-1.0.5/README.md
--rw-r--r--   0        0        0     1219 2024-05-24 12:58:54.330623 ragstack_ai_langchain-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      271 2024-05-24 12:58:54.330623 ragstack_ai_langchain-1.0.5/ragstack_langchain/__init__.py
--rw-r--r--   0        0        0      434 2024-05-24 12:58:54.330623 ragstack_ai_langchain-1.0.5/ragstack_langchain/colbert/__init__.py
--rw-r--r--   0        0        0     2715 2024-05-24 12:58:54.330623 ragstack_ai_langchain-1.0.5/ragstack_langchain/colbert/colbert_retriever.py
--rw-r--r--   0        0        0     9303 2024-05-24 12:58:54.330623 ragstack_ai_langchain-1.0.5/ragstack_langchain/colbert/colbert_vector_store.py
--rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 ragstack_ai_langchain-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      371 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/README.md
+-rw-r--r--   0        0        0     1243 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/ragstack_langchain/__init__.py
+-rw-r--r--   0        0        0      434 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/ragstack_langchain/colbert/__init__.py
+-rw-r--r--   0        0        0     2715 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/ragstack_langchain/colbert/colbert_retriever.py
+-rw-r--r--   0        0        0     9303 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/ragstack_langchain/colbert/colbert_vector_store.py
+-rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 ragstack_ai_langchain-1.0.6/PKG-INFO
```

### Comparing `ragstack_ai_langchain-1.0.5/pyproject.toml` & `ragstack_ai_langchain-1.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ragstack-ai-langchain"
-version = "1.0.5"
+version = "1.0.6"
 description = "DataStax RAGStack Langchain"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_langchain" }]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.9,<3.13"
 astrapy = "^1"
 cassio = "~0.1.4"
 unstructured = "0.14.2"
-ragstack-ai-colbert = "1.0.4"
+ragstack-ai-colbert = "1.0.5"
 
 # langchain
 langchain = "0.1.19"
 langchain-core = "0.1.52"
 langchain-community = "0.0.38"
 langchain-astradb = "0.3.0"
 langchain-openai = "0.1.3"
@@ -31,10 +31,12 @@
 
 google = ["langchain-google-genai", "langchain-google-vertexai"]
 nvidia = ["langchain-nvidia-ai-endpoints"]
 
 [tool.poetry.group.test.dependencies]
 ragstack-ai-tests-utils = { path = "../tests-utils", develop = true }
 ragstack-ai-colbert = { path = "../colbert", develop = true }
-[tool.poetry.group.dev.dependencies]
 pytest-asyncio = "^0.23.6"
 
+[tool.poetry.group.dev.dependencies]
+setuptools = "^70.0.0"
+
```

### Comparing `ragstack_ai_langchain-1.0.5/ragstack_langchain/colbert/colbert_retriever.py` & `ragstack_ai_langchain-1.0.6/ragstack_langchain/colbert/colbert_retriever.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_langchain-1.0.5/ragstack_langchain/colbert/colbert_vector_store.py` & `ragstack_ai_langchain-1.0.6/ragstack_langchain/colbert/colbert_vector_store.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_langchain-1.0.5/PKG-INFO` & `ragstack_ai_langchain-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-langchain
-Version: 1.0.5
+Version: 1.0.6
 Summary: DataStax RAGStack Langchain
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: colbert
 Provides-Extra: google
 Provides-Extra: nvidia
 Requires-Dist: astrapy (>=1,<2)
 Requires-Dist: cassio (>=0.1.4,<0.2.0)
 Requires-Dist: langchain (==0.1.19)
 Requires-Dist: langchain-astradb (==0.3.0)
 Requires-Dist: langchain-community (==0.0.38)
 Requires-Dist: langchain-core (==0.1.52)
 Requires-Dist: langchain-google-genai (==0.0.11) ; extra == "google"
 Requires-Dist: langchain-google-vertexai (==1.0.1) ; extra == "google"
 Requires-Dist: langchain-nvidia-ai-endpoints (==0.0.9) ; extra == "nvidia"
 Requires-Dist: langchain-openai (==0.1.3)
-Requires-Dist: ragstack-ai-colbert (==1.0.4) ; extra == "colbert"
+Requires-Dist: ragstack-ai-colbert (==1.0.5) ; extra == "colbert"
 Requires-Dist: unstructured (==0.14.2)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack LangChain
```

