# Comparing `tmp/llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3.tar.gz` & `tmp/llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4.tar", max compression
```

## Comparing `llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3.tar` & `llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      814 2024-04-12 19:02:19.240709 llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3/README.md
--rw-r--r--   0        0        0      145 2024-04-12 19:02:19.240709 llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3/llama_index/retrievers/mongodb_atlas_bm25_retriever/__init__.py
--rw-r--r--   0        0        0     4015 2024-04-12 19:02:19.240709 llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3/llama_index/retrievers/mongodb_atlas_bm25_retriever/base.py
--rw-r--r--   0        0        0     1543 2024-04-12 19:02:19.240709 llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      814 2024-05-24 14:21:57.628066 llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4/README.md
+-rw-r--r--   0        0        0      145 2024-05-24 14:21:57.628066 llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4/llama_index/retrievers/mongodb_atlas_bm25_retriever/__init__.py
+-rw-r--r--   0        0        0     4045 2024-05-24 14:21:57.628066 llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4/llama_index/retrievers/mongodb_atlas_bm25_retriever/base.py
+-rw-r--r--   0        0        0     1543 2024-05-24 14:21:57.628066 llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4/PKG-INFO
```

### Comparing `llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3/README.md` & `llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3/llama_index/retrievers/mongodb_atlas_bm25_retriever/base.py` & `llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4/llama_index/retrievers/mongodb_atlas_bm25_retriever/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,7 +98,8 @@
                     start_char_idx=node_content.get("start_char_idx", None),
                     end_char_idx=node_content.get("end_char_idx", None),
                     relationships=node_content.get("relationships", None),
                 )
 
             node_with_score = NodeWithScore(node=node, score=result["score"])
             retrieve_nodes.append(node_with_score)
+        return retrieve_nodes
```

### Comparing `llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3/pyproject.toml` & `llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index retrievers mongodb-atlas-bm25-retriever integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-retrievers-mongodb-atlas-bm25-retriever"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 pymongo = "^4.6.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.3/PKG-INFO` & `llama_index_retrievers_mongodb_atlas_bm25_retriever-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-retrievers-mongodb-atlas-bm25-retriever
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index retrievers mongodb-atlas-bm25-retriever integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

