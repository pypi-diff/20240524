# Comparing `tmp/ragstack_ai_colbert-1.0.3.tar.gz` & `tmp/ragstack_ai_colbert-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_colbert-1.0.3.tar", max compression
+gzip compressed data, was "ragstack_ai_colbert-1.0.4.tar", max compression
```

## Comparing `ragstack_ai_colbert-1.0.3.tar` & `ragstack_ai_colbert-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      374 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/README.md
--rw-r--r--   0        0        0      662 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1542 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/__init__.py
--rw-r--r--   0        0        0     3531 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/base_database.py
--rw-r--r--   0        0        0     1848 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/base_embedding_model.py
--rw-r--r--   0        0        0     5645 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/base_retriever.py
--rw-r--r--   0        0        0     5436 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/base_vector_store.py
--rw-r--r--   0        0        0    14323 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/cassandra_database.py
--rw-r--r--   0        0        0     5403 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_embedding_model.py
--rw-r--r--   0        0        0    15736 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_retriever.py
--rw-r--r--   0        0        0     7252 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_vector_store.py
--rw-r--r--   0        0        0      664 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/constant.py
--rw-r--r--   0        0        0     2178 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/objects.py
--rw-r--r--   0        0        0     4579 2024-05-21 18:44:38.654207 ragstack_ai_colbert-1.0.3/ragstack_colbert/text_encoder.py
--rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 ragstack_ai_colbert-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      374 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/README.md
+-rw-r--r--   0        0        0      662 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1542 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/__init__.py
+-rw-r--r--   0        0        0     3531 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/base_database.py
+-rw-r--r--   0        0        0     1848 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/base_embedding_model.py
+-rw-r--r--   0        0        0     5645 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/base_retriever.py
+-rw-r--r--   0        0        0     5431 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/base_vector_store.py
+-rw-r--r--   0        0        0    13772 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/cassandra_database.py
+-rw-r--r--   0        0        0     5403 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/colbert_embedding_model.py
+-rw-r--r--   0        0        0    15736 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/colbert_retriever.py
+-rw-r--r--   0        0        0     7252 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/colbert_vector_store.py
+-rw-r--r--   0        0        0      664 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/constant.py
+-rw-r--r--   0        0        0     2178 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/objects.py
+-rw-r--r--   0        0        0     4579 2024-05-24 12:52:36.097363 ragstack_ai_colbert-1.0.4/ragstack_colbert/text_encoder.py
+-rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 ragstack_ai_colbert-1.0.4/PKG-INFO
```

### Comparing `ragstack_ai_colbert-1.0.3/pyproject.toml` & `ragstack_ai_colbert-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ragstack-ai-colbert"
-version = "1.0.3"
+version = "1.0.4"
 description = "DataStax RAGStack Colbert implementation"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_colbert" }]
```

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/__init__.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/__init__.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/base_database.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/base_database.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/base_embedding_model.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/base_embedding_model.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/base_retriever.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/base_retriever.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/base_vector_store.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/base_vector_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,16 +75,15 @@
         Parameters:
             doc_ids (List[str]): A list of document identifiers specifying the chunks to be deleted.
 
         Returns:
             True if the all the deletes were successful.
         """
 
-        # handles LlamaIndex add
-
+    # handles LlamaIndex add
     @abstractmethod
     async def aadd_chunks(self, chunks: List[Chunk], concurrent_inserts: Optional[int] = 100) -> List[Tuple[str, int]]:
         """
         Stores a list of embedded text chunks in the vector store
 
         Parameters:
             chunks (List[Chunk]): A list of `Chunk` instances to be stored.
```

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/cassandra_database.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/cassandra_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import asyncio
 import logging
 from collections import defaultdict
 from typing import Any, Dict, List, Optional, Set, Tuple
 
 import cassio
-from cassandra.cluster import ResponseFuture, Session
+from cassandra.cluster import Session
 from cassio.table.query import Predicate, PredicateOperator
 from cassio.table.tables import ClusteredMetadataVectorCassandraTable
 
 from .base_database import BaseDatabase
 from .constant import DEFAULT_COLBERT_DIM
 from .objects import Chunk, Vector
 
@@ -115,58 +115,52 @@
         Parameters:
             chunks (List[Chunk]): A list of `Chunk` instances to be stored.
 
         Returns:
             a list of tuples: (doc_id, chunk_id)
         """
 
-        all_futures: List[Tuple[str, int, int, ResponseFuture]] = []
-        futures_per_chunk: Dict[Tuple[str, int], int] = defaultdict(int)
+        failed_chunks: List[Tuple[str, int]] = []
+        success_chunks: List[Tuple[str, int]] = []
 
         for chunk in chunks:
             doc_id = chunk.doc_id
             chunk_id = chunk.chunk_id
 
-            future = self._table.put_async(
+            try:
+                self._table.put(
                     partition_id=doc_id,
                     row_id=(chunk_id, -1),
                     body_blob=chunk.text,
                     metadata=chunk.metadata,
                 )
-            all_futures.append((doc_id, chunk_id, -1, future))
-            futures_per_chunk[(doc_id, chunk_id)] += 1
-
-            for embedding_id, vector in enumerate(chunk.embedding):
-                future = self._table.put_async(
-                    partition_id=doc_id, row_id=(chunk_id, embedding_id), vector=vector
-                )
-                all_futures.append((doc_id, chunk_id, embedding_id, future))
-                futures_per_chunk[(doc_id, chunk_id)] += 1
-
-        for doc_id, chunk_id, embedding_id, future in all_futures:
-            try:
-                future.result()
-                futures_per_chunk[(doc_id, chunk_id)] -= 1
             except Exception as exp:
-                self._log_insert_error(doc_id=doc_id, chunk_id=chunk_id, embedding_id=embedding_id, exp=exp)
+                self._log_insert_error(doc_id=doc_id, chunk_id=chunk_id, embedding_id=-1, exp=exp)
+                failed_chunks.append((doc_id, chunk_id))
+                continue
 
 
-        outputs: List[Tuple[str, int]] = []
-        failed_chunks: List[Tuple[str, int]] = []
+            for embedding_id, vector in enumerate(chunk.embedding):
+                try:
+                    self._table.put(
+                        partition_id=doc_id,
+                        row_id=(chunk_id, embedding_id),
+                        vector=vector,
+                    )
+                except Exception as exp:
+                    self._log_insert_error(doc_id=doc_id, chunk_id=chunk_id, embedding_id=-1, exp=exp)
+                    failed_chunks.append((doc_id, chunk_id))
+                    continue
 
-        for (doc_id, chunk_id) in futures_per_chunk:
-            if futures_per_chunk[(doc_id, chunk_id)] == 0:
-                outputs.append((doc_id, chunk_id))
-            else:
-                failed_chunks.append((doc_id, chunk_id))
+            success_chunks.append((doc_id, chunk_id))
 
         if len(failed_chunks) > 0:
             raise Exception(f"add failed for these chunks: {failed_chunks}. See error logs for more info.")
 
-        return outputs
+        return success_chunks
 
     async def _limited_put(
             self,
             sem: asyncio.Semaphore,
             doc_id: str,
             chunk_id: int,
             embedding_id: Optional[int] = -1,
@@ -264,34 +258,27 @@
         Parameters:
             doc_ids (List[str]): A list of document identifiers specifying the chunks to be deleted.
 
         Returns:
             True if the all the deletes were successful.
         """
 
-        futures = [
-            (doc_id, self._table.delete_partition_async(partition_id=doc_id))
-            for doc_id in doc_ids
-        ]
-
-        success = True
         failed_docs: List[str] = []
 
-        for doc_id, future in futures:
+        for doc_id in doc_ids:
             try:
-                future.result()
-            except Exception as e:
-                success = False
-                logging.error(f"issue on delete of document: {doc_id}: {e}")
+                self._table.delete_partition(partition_id=doc_id)
+            except Exception as exp:
+                logging.error(f"issue on delete of document: {doc_id}: {exp}")
                 failed_docs.append(doc_id)
 
         if len(failed_docs) > 0:
             raise Exception(f"delete failed for these docs: {failed_docs}. See error logs for more info.")
 
-        return success
+        return True
 
     async def _limited_delete(
             self,
             sem: asyncio.Semaphore,
             doc_id: str,
     ) -> Tuple[str, Exception]:
         exp = None
```

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_embedding_model.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/colbert_embedding_model.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_retriever.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/colbert_retriever.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/colbert_vector_store.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/colbert_vector_store.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/constant.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/constant.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/objects.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/objects.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.3/ragstack_colbert/text_encoder.py` & `ragstack_ai_colbert-1.0.4/ragstack_colbert/text_encoder.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_colbert-1.0.3/PKG-INFO` & `ragstack_ai_colbert-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-colbert
-Version: 1.0.3
+Version: 1.0.4
 Summary: DataStax RAGStack Colbert implementation
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

