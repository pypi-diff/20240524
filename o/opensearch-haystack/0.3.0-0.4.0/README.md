# Comparing `tmp/opensearch_haystack-0.3.0.tar.gz` & `tmp/opensearch_haystack-0.4.0.tar.gz`

## Comparing `opensearch_haystack-0.3.0.tar` & `opensearch_haystack-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/docker-compose.yml
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/pydoc/config.yml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/opensearch/__init__.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/document_stores/opensearch/__init__.py
--rw-r--r--   0        0        0    13587 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/document_stores/opensearch/document_store.py
--rw-r--r--   0        0        0     9916 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/src/haystack_integrations/document_stores/opensearch/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/tests/test_bm25_retriever.py
--rw-r--r--   0        0        0    15927 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/tests/test_document_store.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/tests/test_embedding_retriever.py
--rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/tests/test_filters.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/LICENSE
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/README.md
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 opensearch_haystack-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/docker-compose.yml
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/pydoc/config.yml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/opensearch/__init__.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/document_stores/opensearch/__init__.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/document_stores/opensearch/document_store.py
+-rw-r--r--   0        0        0     9916 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/src/haystack_integrations/document_stores/opensearch/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/tests/test_bm25_retriever.py
+-rw-r--r--   0        0        0    16154 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/tests/test_embedding_retriever.py
+-rw-r--r--   0        0        0     8002 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/tests/test_filters.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/LICENSE
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/README.md
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 opensearch_haystack-0.4.0/PKG-INFO
```

### Comparing `opensearch_haystack-0.3.0/pydoc/config.yml` & `opensearch_haystack-0.4.0/pydoc/config.yml`

 * *Files 10% similar despite different names*

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
   excerpt: OpenSearch integration for Haystack
   category_slug: integrations-api
   title: OpenSearch
   slug: integrations-opensearch
   order: 180
   markdown:
     descriptive_class_title: false
```

### Comparing `opensearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py` & `opensearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/opensearch/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.3.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py` & `opensearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/opensearch/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.3.0/src/haystack_integrations/document_stores/opensearch/document_store.py` & `opensearch_haystack-0.4.0/src/haystack_integrations/document_stores/opensearch/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,53 +43,57 @@
 
         For the full list of supported kwargs, see the [official OpenSearch reference](https://opensearch-project.github.io/opensearch-py/api-ref/clients/opensearch_client.html)
 
         :param hosts: List of hosts running the OpenSearch client. Defaults to None
         :param index: Name of index in OpenSearch, if it doesn't exist it will be created. Defaults to "default"
         :param **kwargs: Optional arguments that ``OpenSearch`` takes.
         """
+        self._client = None
         self._hosts = hosts
-        self._client = OpenSearch(hosts, **kwargs)
         self._index = index
         self._kwargs = kwargs
 
-        # Check client connection, this will raise if not connected
-        self._client.info()
-
-        # configure mapping for the embedding field
-        embedding_dim = kwargs.get("embedding_dim", 768)
-        method = kwargs.get("method", None)
-
-        mappings: Dict[str, Any] = {
-            "properties": {
-                "embedding": {"type": "knn_vector", "index": True, "dimension": embedding_dim},
-                "content": {"type": "text"},
-            },
-            "dynamic_templates": [
-                {
-                    "strings": {
-                        "match_mapping_type": "string",
-                        "mapping": {
-                            "type": "keyword",
-                        },
-                    }
+    @property
+    def client(self) -> OpenSearch:
+        if not self._client:
+            self._client = OpenSearch(self._hosts, **self._kwargs)
+            # Check client connection, this will raise if not connected
+            self._client.info()  # type:ignore
+
+            # Create the index if it doesn't exist
+            if not self._client.indices.exists(index=self._index):  # type:ignore
+                # configure fallback mapping for the embedding field
+                method = self._kwargs.get("method", None)
+                embedding_dim = self._kwargs.get("embedding_dim", 768)
+                default_mappings: Dict[str, Any] = {
+                    "properties": {
+                        "embedding": {"type": "knn_vector", "index": True, "dimension": embedding_dim},
+                        "content": {"type": "text"},
+                    },
+                    "dynamic_templates": [
+                        {
+                            "strings": {
+                                "match_mapping_type": "string",
+                                "mapping": {
+                                    "type": "keyword",
+                                },
+                            }
+                        }
+                    ],
                 }
-            ],
-        }
-        if method:
-            mappings["properties"]["embedding"]["method"] = method
+                if method:
+                    default_mappings["properties"]["embedding"]["method"] = method
 
-        mappings = kwargs.get("mappings", mappings)
-        settings = kwargs.get("settings", {"index.knn": True})
-
-        body = {"mappings": mappings, "settings": settings}
+                body = {
+                    "mappings": self._kwargs.get("mappings", default_mappings),
+                    "settings": self._kwargs.get("settings", {"index.knn": True}),
+                }
+                self._client.indices.create(index=self._index, body=body)  # type:ignore
 
-        # Create the index if it doesn't exist
-        if not self._client.indices.exists(index=index):
-            self._client.indices.create(index=index, body=body)
+        return self._client
 
     def to_dict(self) -> Dict[str, Any]:
         # This is not the best solution to serialise this class but is the fastest to implement.
         # Not all kwargs types can be serialised to text so this can fail. We must serialise each
         # type explicitly to handle this properly.
         """
         Serializes the component to a dictionary.
@@ -117,21 +121,21 @@
         """
         return default_from_dict(cls, data)
 
     def count_documents(self) -> int:
         """
         Returns how many documents are present in the document store.
         """
-        return self._client.count(index=self._index)["count"]
+        return self.client.count(index=self._index)["count"]
 
     def _search_documents(self, **kwargs) -> List[Document]:
         """
         Calls the OpenSearch client's search method and handles pagination.
         """
-        res = self._client.search(
+        res = self.client.search(
             index=self._index,
             body=kwargs,
         )
         documents: List[Document] = [self._deserialize_document(hit) for hit in res["hits"]["hits"]]
         return documents
 
     def filter_documents(self, filters: Optional[Dict[str, Any]] = None) -> List[Document]:
@@ -158,15 +162,15 @@
                 raise ValueError(msg)
 
         if policy == DuplicatePolicy.NONE:
             policy = DuplicatePolicy.FAIL
 
         action = "index" if policy == DuplicatePolicy.OVERWRITE else "create"
         documents_written, errors = bulk(
-            client=self._client,
+            client=self.client,
             actions=(
                 {
                     "_op_type": action,
                     "_id": doc.id,
                     "_source": doc.to_dict(),
                 }
                 for doc in documents
@@ -221,15 +225,15 @@
         """
         Deletes all documents with a matching document_ids from the document store.
 
         :param object_ids: the object_ids to delete
         """
 
         bulk(
-            client=self._client,
+            client=self.client,
             actions=({"_op_type": "delete", "_id": id_} for id_ in document_ids),
             refresh="wait_for",
             index=self._index,
             raise_on_error=False,
         )
 
     def _bm25_retrieval(
@@ -290,15 +294,15 @@
         if filters:
             body["query"]["bool"]["filter"] = normalize_filters(filters)
 
         documents = self._search_documents(**body)
 
         if scale_score:
             for doc in documents:
-                doc.score = float(1 / (1 + np.exp(-np.asarray(doc.score / BM25_SCALING_FACTOR))))
+                doc.score = float(1 / (1 + np.exp(-np.asarray(doc.score / BM25_SCALING_FACTOR))))  # type:ignore
 
         return documents
 
     def _embedding_retrieval(
         self,
         query_embedding: List[float],
         *,
```

### Comparing `opensearch_haystack-0.3.0/src/haystack_integrations/document_stores/opensearch/filters.py` & `opensearch_haystack-0.4.0/src/haystack_integrations/document_stores/opensearch/filters.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.3.0/tests/test_bm25_retriever.py` & `opensearch_haystack-0.4.0/tests/test_bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.3.0/tests/test_document_store.py` & `opensearch_haystack-0.4.0/tests/test_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,20 @@
         },
     }
     document_store = OpenSearchDocumentStore.from_dict(data)
     assert document_store._hosts == "some hosts"
     assert document_store._index == "default"
 
 
+@patch("haystack_integrations.document_stores.opensearch.document_store.OpenSearch")
+def test_init_is_lazy(_mock_opensearch_client):
+    OpenSearchDocumentStore(hosts="testhost")
+    _mock_opensearch_client.assert_not_called()
+
+
 @pytest.mark.integration
 class TestDocumentStore(DocumentStoreBaseTests):
     """
     Common test cases will be provided by `DocumentStoreBaseTests` but
     you can add more to this class.
     """
 
@@ -63,15 +69,15 @@
             index=index,
             http_auth=("admin", "admin"),
             verify_certs=False,
             embedding_dim=768,
             method={"space_type": "cosinesimil", "engine": "nmslib", "name": "hnsw"},
         )
         yield store
-        store._client.indices.delete(index=index, params={"ignore": [400, 404]})
+        store.client.indices.delete(index=index, params={"ignore": [400, 404]})
 
     @pytest.fixture
     def document_store_embedding_dim_4(self, request):
         """
         This is the most basic requirement for the child class: provide
         an instance of this document store so the base class can use it.
         """
@@ -84,15 +90,15 @@
             index=index,
             http_auth=("admin", "admin"),
             verify_certs=False,
             embedding_dim=4,
             method={"space_type": "cosinesimil", "engine": "nmslib", "name": "hnsw"},
         )
         yield store
-        store._client.indices.delete(index=index, params={"ignore": [400, 404]})
+        store.client.indices.delete(index=index, params={"ignore": [400, 404]})
 
     def assert_documents_are_equal(self, received: List[Document], expected: List[Document]):
         """
         The OpenSearchDocumentStore.filter_documents() method returns a Documents with their score set.
         We don't want to compare the score, so we set it to None before comparing the documents.
         """
         received_meta = []
```

### Comparing `opensearch_haystack-0.3.0/tests/test_embedding_retriever.py` & `opensearch_haystack-0.4.0/tests/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.3.0/tests/test_filters.py` & `opensearch_haystack-0.4.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.3.0/.gitignore` & `opensearch_haystack-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.3.0/LICENSE` & `opensearch_haystack-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.3.0/README.md` & `opensearch_haystack-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `opensearch_haystack-0.3.0/pyproject.toml` & `opensearch_haystack-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "deepset", email = "info@deepset.ai" },
 ]
 classifiers = [
+  "License :: OSI Approved :: Apache Software License",
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `opensearch_haystack-0.3.0/PKG-INFO` & `opensearch_haystack-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: opensearch-haystack
-Version: 0.3.0
+Version: 0.4.0
 Summary: Haystack 2.x Document Store for OpenSearch
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/opensearch#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/opensearch
 Author-email: deepset <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

