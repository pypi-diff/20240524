# Comparing `tmp/qdrant_haystack-3.5.0.tar.gz` & `tmp/qdrant_haystack-3.6.0.tar.gz`

## Comparing `qdrant_haystack-3.5.0.tar` & `qdrant_haystack-3.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/examples/embedding_retrieval.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/pydoc/config.yml
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/src/haystack_integrations/components/retrievers/qdrant/__init__.py
--rw-r--r--   0        0        0    13384 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/src/haystack_integrations/components/retrievers/qdrant/retriever.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/src/haystack_integrations/document_stores/qdrant/__init__.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/src/haystack_integrations/document_stores/qdrant/converters.py
--rw-r--r--   0        0        0    26260 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/src/haystack_integrations/document_stores/qdrant/document_store.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/src/haystack_integrations/document_stores/qdrant/filters.py
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/src/haystack_integrations/document_stores/qdrant/migrate_to_sparse.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/tests/__init__.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/tests/conftest.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/tests/test_converters.py
--rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/tests/test_dict_converters.py
--rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/tests/test_document_store.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/tests/test_filters.py
--rw-r--r--   0        0        0    20208 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/tests/test_legacy_filters.py
--rw-r--r--   0        0        0    15628 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/tests/test_retriever.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/LICENSE.txt
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/README.md
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 qdrant_haystack-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/examples/embedding_retrieval.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/pydoc/config.yml
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/src/haystack_integrations/components/retrievers/qdrant/__init__.py
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/src/haystack_integrations/components/retrievers/qdrant/retriever.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/src/haystack_integrations/document_stores/qdrant/__init__.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/src/haystack_integrations/document_stores/qdrant/converters.py
+-rw-r--r--   0        0        0    26827 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/src/haystack_integrations/document_stores/qdrant/document_store.py
+-rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/src/haystack_integrations/document_stores/qdrant/filters.py
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/src/haystack_integrations/document_stores/qdrant/migrate_to_sparse.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/tests/test_converters.py
+-rw-r--r--   0        0        0     4328 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/tests/test_dict_converters.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/tests/test_filters.py
+-rw-r--r--   0        0        0    20208 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/tests/test_legacy_filters.py
+-rw-r--r--   0        0        0    15628 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/tests/test_retriever.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/LICENSE.txt
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/README.md
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 qdrant_haystack-3.6.0/PKG-INFO
```

### Comparing `qdrant_haystack-3.5.0/examples/embedding_retrieval.py` & `qdrant_haystack-3.6.0/examples/embedding_retrieval.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/pydoc/config.yml` & `qdrant_haystack-3.6.0/pydoc/config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     expression:
     documented_only: true
     do_not_filter_modules: false
     skip_empty_modules: true
   - type: smart
   - type: crossref
 renderer:
-  type: haystack_pydoc_tools.renderers.ReadmePreviewRenderer
+  type: haystack_pydoc_tools.renderers.ReadmeIntegrationRenderer
   excerpt: Qdrant integration for Haystack
   category_slug: integrations-api
   title: Qdrant
   slug: integrations-qdrant
   order: 210
   markdown:
     descriptive_class_title: false
```

### Comparing `qdrant_haystack-3.5.0/src/haystack_integrations/components/retrievers/qdrant/retriever.py` & `qdrant_haystack-3.6.0/src/haystack_integrations/components/retrievers/qdrant/retriever.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from haystack import Document, component, default_from_dict, default_to_dict
 from haystack.dataclasses.sparse_embedding import SparseEmbedding
 from haystack_integrations.document_stores.qdrant import QdrantDocumentStore
+from qdrant_client.http import models
 
 
 @component
 class QdrantEmbeddingRetriever:
     """
     A component for retrieving documents from an QdrantDocumentStore using dense vectors.
 
     Usage example:
     ```python
+    from haystack.dataclasses import Document
     from haystack_integrations.components.retrievers.qdrant import QdrantEmbeddingRetriever
     from haystack_integrations.document_stores.qdrant import QdrantDocumentStore
 
     document_store = QdrantDocumentStore(
         ":memory:",
         recreate_index=True,
         return_embedding=True,
@@ -29,29 +31,29 @@
     retriever.run(query_embedding=[0.1]*768)
     ```
     """
 
     def __init__(
         self,
         document_store: QdrantDocumentStore,
-        filters: Optional[Dict[str, Any]] = None,
+        filters: Optional[Union[Dict[str, Any], models.Filter]] = None,
         top_k: int = 10,
         scale_score: bool = True,
         return_embedding: bool = False,
     ):
         """
         Create a QdrantEmbeddingRetriever component.
 
         :param document_store: An instance of QdrantDocumentStore.
-        :param filters: A dictionary with filters to narrow down the search space. Default is None.
-        :param top_k: The maximum number of documents to retrieve. Default is 10.
-        :param scale_score: Whether to scale the scores of the retrieved documents or not. Default is True.
-        :param return_embedding: Whether to return the embedding of the retrieved Documents. Default is False.
+        :param filters: A dictionary with filters to narrow down the search space.
+        :param top_k: The maximum number of documents to retrieve.
+        :param scale_score: Whether to scale the scores of the retrieved documents or not.
+        :param return_embedding: Whether to return the embedding of the retrieved Documents.
 
-        :raises ValueError: If 'document_store' is not an instance of QdrantDocumentStore.
+        :raises ValueError: If `document_store` is not an instance of `QdrantDocumentStore`.
         """
 
         if not isinstance(document_store, QdrantDocumentStore):
             msg = "document_store must be an instance of QdrantDocumentStore"
             raise ValueError(msg)
 
         self._document_store = document_store
@@ -93,15 +95,15 @@
         data["init_parameters"]["document_store"] = document_store
         return default_from_dict(cls, data)
 
     @component.output_types(documents=List[Document])
     def run(
         self,
         query_embedding: List[float],
-        filters: Optional[Dict[str, Any]] = None,
+        filters: Optional[Union[Dict[str, Any], models.Filter]] = None,
         top_k: Optional[int] = None,
         scale_score: Optional[bool] = None,
         return_embedding: Optional[bool] = None,
     ):
         """
         Run the Embedding Retriever on the given input data.
 
@@ -130,15 +132,15 @@
     """
     A component for retrieving documents from an QdrantDocumentStore using sparse vectors.
 
     Usage example:
     ```python
     from haystack_integrations.components.retrievers.qdrant import QdrantSparseEmbeddingRetriever
     from haystack_integrations.document_stores.qdrant import QdrantDocumentStore
-    from haystack.dataclasses.sparse_embedding import SparseEmbedding
+    from haystack.dataclasses import Document, SparseEmbedding
 
     document_store = QdrantDocumentStore(
         ":memory:",
         use_sparse_embeddings=True,
         recreate_index=True,
         return_embedding=True,
     )
@@ -151,29 +153,29 @@
     retriever.run(query_sparse_embedding=sparse_embedding)
     ```
     """
 
     def __init__(
         self,
         document_store: QdrantDocumentStore,
-        filters: Optional[Dict[str, Any]] = None,
+        filters: Optional[Union[Dict[str, Any], models.Filter]] = None,
         top_k: int = 10,
         scale_score: bool = True,
         return_embedding: bool = False,
     ):
         """
         Create a QdrantSparseEmbeddingRetriever component.
 
         :param document_store: An instance of QdrantDocumentStore.
-        :param filters: A dictionary with filters to narrow down the search space. Default is None.
-        :param top_k: The maximum number of documents to retrieve. Default is 10.
-        :param scale_score: Whether to scale the scores of the retrieved documents or not. Default is True.
-        :param return_embedding: Whether to return the sparse embedding of the retrieved Documents. Default is False.
+        :param filters: A dictionary with filters to narrow down the search space.
+        :param top_k: The maximum number of documents to retrieve.
+        :param scale_score: Whether to scale the scores of the retrieved documents or not.
+        :param return_embedding: Whether to return the sparse embedding of the retrieved Documents.
 
-        :raises ValueError: If 'document_store' is not an instance of QdrantDocumentStore.
+        :raises ValueError: If `document_store` is not an instance of `QdrantDocumentStore`.
         """
 
         if not isinstance(document_store, QdrantDocumentStore):
             msg = "document_store must be an instance of QdrantDocumentStore"
             raise ValueError(msg)
 
         self._document_store = document_store
@@ -215,15 +217,15 @@
         data["init_parameters"]["document_store"] = document_store
         return default_from_dict(cls, data)
 
     @component.output_types(documents=List[Document])
     def run(
         self,
         query_sparse_embedding: SparseEmbedding,
-        filters: Optional[Dict[str, Any]] = None,
+        filters: Optional[Union[Dict[str, Any], models.Filter]] = None,
         top_k: Optional[int] = None,
         scale_score: Optional[bool] = None,
         return_embedding: Optional[bool] = None,
     ):
         """
         Run the Sparse Embedding Retriever on the given input data.
 
@@ -253,15 +255,15 @@
     A component for retrieving documents from an QdrantDocumentStore using both dense and sparse vectors
     and fusing the results using Reciprocal Rank Fusion.
 
     Usage example:
     ```python
     from haystack_integrations.components.retrievers.qdrant import QdrantHybridRetriever
     from haystack_integrations.document_stores.qdrant import QdrantDocumentStore
-    from haystack.dataclasses.sparse_embedding import SparseEmbedding
+    from haystack.dataclasses import Document, SparseEmbedding
 
     document_store = QdrantDocumentStore(
         ":memory:",
         use_sparse_embeddings=True,
         recreate_index=True,
         return_embedding=True,
         wait_result_from_api=True,
@@ -279,15 +281,15 @@
     retriever.run(query_embedding=embedding, query_sparse_embedding=sparse_embedding)
     ```
     """
 
     def __init__(
         self,
         document_store: QdrantDocumentStore,
-        filters: Optional[Dict[str, Any]] = None,
+        filters: Optional[Union[Dict[str, Any], models.Filter]] = None,
         top_k: int = 10,
         return_embedding: bool = False,
     ):
         """
         Create a QdrantHybridRetriever component.
 
         :param document_store: An instance of QdrantDocumentStore.
@@ -337,15 +339,15 @@
         return default_from_dict(cls, data)
 
     @component.output_types(documents=List[Document])
     def run(
         self,
         query_embedding: List[float],
         query_sparse_embedding: SparseEmbedding,
-        filters: Optional[Dict[str, Any]] = None,
+        filters: Optional[Union[Dict[str, Any], models.Filter]] = None,
         top_k: Optional[int] = None,
         return_embedding: Optional[bool] = None,
     ):
         """
         Run the Sparse Embedding Retriever on the given input data.
 
         :param query_embedding: Dense embedding of the query.
```

### Comparing `qdrant_haystack-3.5.0/src/haystack_integrations/document_stores/qdrant/converters.py` & `qdrant_haystack-3.6.0/src/haystack_integrations/document_stores/qdrant/converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/src/haystack_integrations/document_stores/qdrant/document_store.py` & `qdrant_haystack-3.6.0/src/haystack_integrations/document_stores/qdrant/document_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         url: Optional[str] = None,
         port: int = 6333,
         grpc_port: int = 6334,
         prefer_grpc: bool = False,
         https: Optional[bool] = None,
         api_key: Optional[Secret] = None,
         prefix: Optional[str] = None,
-        timeout: Optional[float] = None,
+        timeout: Optional[int] = None,
         host: Optional[str] = None,
         path: Optional[str] = None,
         index: str = "Document",
         embedding_dim: int = 768,
         on_disk: bool = False,
         content_field: str = "content",
         name_field: str = "name",
@@ -92,45 +92,29 @@
         init_from: Optional[dict] = None,
         wait_result_from_api: bool = True,
         metadata: Optional[dict] = None,
         write_batch_size: int = 100,
         scroll_size: int = 10_000,
         payload_fields_to_index: Optional[List[dict]] = None,
     ):
-        super().__init__()
-
-        metadata = metadata or {}
-        self.client = qdrant_client.QdrantClient(
-            location=location,
-            url=url,
-            port=port,
-            grpc_port=grpc_port,
-            prefer_grpc=prefer_grpc,
-            https=https,
-            api_key=api_key.resolve_value() if api_key else None,
-            prefix=prefix,
-            timeout=timeout,
-            host=host,
-            path=path,
-            metadata=metadata,
-        )
+        self._client = None
 
         # Store the Qdrant client specific attributes
         self.location = location
         self.url = url
         self.port = port
         self.grpc_port = grpc_port
         self.prefer_grpc = prefer_grpc
         self.https = https
         self.api_key = api_key
         self.prefix = prefix
         self.timeout = timeout
         self.host = host
         self.path = path
-        self.metadata = metadata
+        self.metadata = metadata or {}
         self.api_key = api_key
 
         # Store the Qdrant collection specific attributes
         self.shard_number = shard_number
         self.replication_factor = replication_factor
         self.write_consistency_factor = write_consistency_factor
         self.on_disk_payload = on_disk_payload
@@ -139,54 +123,77 @@
         self.wal_config = wal_config
         self.quantization_config = quantization_config
         self.init_from = init_from
         self.wait_result_from_api = wait_result_from_api
         self.recreate_index = recreate_index
         self.payload_fields_to_index = payload_fields_to_index
         self.use_sparse_embeddings = use_sparse_embeddings
-
-        # Make sure the collection is properly set up
-        self._set_up_collection(
-            index, embedding_dim, recreate_index, similarity, use_sparse_embeddings, on_disk, payload_fields_to_index
-        )
-
         self.embedding_dim = embedding_dim
         self.on_disk = on_disk
         self.content_field = content_field
         self.name_field = name_field
         self.embedding_field = embedding_field
         self.similarity = similarity
         self.index = index
         self.return_embedding = return_embedding
         self.progress_bar = progress_bar
         self.duplicate_documents = duplicate_documents
         self.write_batch_size = write_batch_size
         self.scroll_size = scroll_size
 
+    @property
+    def client(self):
+        if not self._client:
+            self._client = qdrant_client.QdrantClient(
+                location=self.location,
+                url=self.url,
+                port=self.port,
+                grpc_port=self.grpc_port,
+                prefer_grpc=self.prefer_grpc,
+                https=self.https,
+                api_key=self.api_key.resolve_value() if self.api_key else None,
+                prefix=self.prefix,
+                timeout=self.timeout,
+                host=self.host,
+                path=self.path,
+                metadata=self.metadata,
+            )
+            # Make sure the collection is properly set up
+            self._set_up_collection(
+                self.index,
+                self.embedding_dim,
+                self.recreate_index,
+                self.similarity,
+                self.use_sparse_embeddings,
+                self.on_disk,
+                self.payload_fields_to_index,
+            )
+        return self._client
+
     def count_documents(self) -> int:
         try:
             response = self.client.count(
                 collection_name=self.index,
             )
             return response.count
         except (UnexpectedResponse, ValueError):
             # Qdrant local raises ValueError if the collection is not found, but
             # with the remote server UnexpectedResponse is raised. Until that's unified,
             # we need to catch both.
             return 0
 
     def filter_documents(
         self,
-        filters: Optional[Dict[str, Any]] = None,
+        filters: Optional[Union[Dict[str, Any], rest.Filter]] = None,
     ) -> List[Document]:
-        if filters and not isinstance(filters, dict):
-            msg = "Filter must be a dictionary"
+        if filters and not isinstance(filters, dict) and not isinstance(filters, rest.Filter):
+            msg = "Filter must be a dictionary or an instance of `qdrant_client.http.models.Filter`"
             raise ValueError(msg)
 
-        if filters and "operator" not in filters:
+        if filters and not isinstance(filters, rest.Filter) and "operator" not in filters:
             filters = convert_legacy_filters(filters)
         return list(
             self.get_documents_generator(
                 filters,
             )
         )
 
@@ -256,15 +263,15 @@
         return default_to_dict(
             self,
             **init_params,
         )
 
     def get_documents_generator(
         self,
-        filters: Optional[Dict[str, Any]] = None,
+        filters: Optional[Union[Dict[str, Any], rest.Filter]] = None,
     ) -> Generator[Document, None, None]:
         index = self.index
         qdrant_filters = convert_filters_to_qdrant(filters)
 
         next_offset = None
         stop_scrolling = False
         while not stop_scrolling:
@@ -307,15 +314,15 @@
                 convert_qdrant_point_to_haystack_document(record, use_sparse_embeddings=self.use_sparse_embeddings)
             )
         return documents
 
     def _query_by_sparse(
         self,
         query_sparse_embedding: SparseEmbedding,
-        filters: Optional[Dict[str, Any]] = None,
+        filters: Optional[Union[Dict[str, Any], rest.Filter]] = None,
         top_k: int = 10,
         scale_score: bool = True,
         return_embedding: bool = False,
     ) -> List[Document]:
         if not self.use_sparse_embeddings:
             message = (
                 "You are trying to query using sparse embeddings, but the Document Store "
@@ -349,15 +356,15 @@
                 score = float(1 / (1 + np.exp(-score / 100)))
                 document.score = score
         return results
 
     def _query_by_embedding(
         self,
         query_embedding: List[float],
-        filters: Optional[Dict[str, Any]] = None,
+        filters: Optional[Union[Dict[str, Any], rest.Filter]] = None,
         top_k: int = 10,
         scale_score: bool = True,
         return_embedding: bool = False,
     ) -> List[Document]:
         qdrant_filters = convert_filters_to_qdrant(filters)
 
         points = self.client.search(
@@ -384,15 +391,15 @@
                 document.score = score
         return results
 
     def _query_hybrid(
         self,
         query_embedding: List[float],
         query_sparse_embedding: SparseEmbedding,
-        filters: Optional[Dict[str, Any]] = None,
+        filters: Optional[Union[Dict[str, Any], rest.Filter]] = None,
         top_k: int = 10,
         return_embedding: bool = False,
     ) -> List[Document]:
         """
         Retrieves documents based on dense and sparse embeddings and fuses the results using Reciprocal Rank Fusion.
 
         This method is not part of the public interface of `QdrantDocumentStore` and shouldn't be used directly.
```

### Comparing `qdrant_haystack-3.5.0/src/haystack_integrations/document_stores/qdrant/filters.py` & `qdrant_haystack-3.6.0/src/haystack_integrations/document_stores/qdrant/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 from .converters import convert_id
 
 COMPARISON_OPERATORS = COMPARISON_OPERATORS.keys()
 LOGICAL_OPERATORS = LOGICAL_OPERATORS.keys()
 
 
 def convert_filters_to_qdrant(
-    filter_term: Optional[Union[List[dict], dict]] = None,
+    filter_term: Optional[Union[List[dict], dict, models.Filter]] = None,
 ) -> Optional[models.Filter]:
     """Converts Haystack filters to the format used by Qdrant."""
-
+    if isinstance(filter_term, models.Filter):
+        return filter_term
     if not filter_term:
         return None
 
     must_clauses, should_clauses, must_not_clauses = [], [], []
 
     if isinstance(filter_term, dict):
         filter_term = [filter_term]
```

### Comparing `qdrant_haystack-3.5.0/src/haystack_integrations/document_stores/qdrant/migrate_to_sparse.py` & `qdrant_haystack-3.6.0/src/haystack_integrations/document_stores/qdrant/migrate_to_sparse.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/tests/conftest.py` & `qdrant_haystack-3.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/tests/test_converters.py` & `qdrant_haystack-3.6.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/tests/test_dict_converters.py` & `qdrant_haystack-3.6.0/tests/test_dict_converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/tests/test_document_store.py` & `qdrant_haystack-3.6.0/tests/test_document_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,19 @@
             ":memory:",
             recreate_index=True,
             return_embedding=True,
             wait_result_from_api=True,
             use_sparse_embeddings=False,
         )
 
+    def test_init_is_lazy(self):
+        with patch("haystack_integrations.document_stores.qdrant.document_store.qdrant_client") as mocked_qdrant:
+            QdrantDocumentStore(location=":memory:", use_sparse_embeddings=True)
+            mocked_qdrant.assert_not_called()
+
     def assert_documents_are_equal(self, received: List[Document], expected: List[Document]):
         """
         Assert that two lists of Documents are equal.
         This is used in every test.
         """
 
         # Check that the lengths of the lists are the same
```

### Comparing `qdrant_haystack-3.5.0/tests/test_filters.py` & `qdrant_haystack-3.6.0/tests/test_filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 from typing import List
 
 import pytest
 from haystack import Document
 from haystack.testing.document_store import FilterDocumentsTest
 from haystack.utils.filters import FilterError
 from haystack_integrations.document_stores.qdrant import QdrantDocumentStore
+from qdrant_client.http import models
 
 
 class TestQdrantStoreBaseTests(FilterDocumentsTest):
     @pytest.fixture
     def document_store(self) -> QdrantDocumentStore:
         return QdrantDocumentStore(
             ":memory:",
             recreate_index=True,
             return_embedding=True,
             wait_result_from_api=True,
         )
 
+    def test_filter_documents_with_qdrant_filters(self, document_store, filterable_docs):
+        document_store.write_documents(filterable_docs)
+        result = document_store.filter_documents(
+            filters=models.Filter(
+                must_not=[
+                    models.FieldCondition(key="meta.number", match=models.MatchValue(value=100)),
+                    models.FieldCondition(key="meta.name", match=models.MatchValue(value="name_0")),
+                ]
+            )
+        )
+        self.assert_documents_are_equal(
+            result,
+            [d for d in filterable_docs if (d.meta.get("number") != 100 and d.meta.get("name") != "name_0")],
+        )
+
     def assert_documents_are_equal(self, received: List[Document], expected: List[Document]):
         """
         Assert that two lists of Documents are equal.
         This is used in every test.
         """
 
         # Check that the lengths of the lists are the same
```

### Comparing `qdrant_haystack-3.5.0/tests/test_legacy_filters.py` & `qdrant_haystack-3.6.0/tests/test_legacy_filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/tests/test_retriever.py` & `qdrant_haystack-3.6.0/tests/test_retriever.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/.gitignore` & `qdrant_haystack-3.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/LICENSE.txt` & `qdrant_haystack-3.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/README.md` & `qdrant_haystack-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/pyproject.toml` & `qdrant_haystack-3.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-3.5.0/PKG-INFO` & `qdrant_haystack-3.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qdrant-haystack
-Version: 3.5.0
+Version: 3.6.0
 Summary: An integration of Qdrant ANN vector database backend with Haystack
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/blob/main/integrations/qdrant/README.md
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Author-email: Kacper Łukawski <kacper.lukawski@qdrant.com>, Anush Shetty <anush.shetty@qdrant.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

