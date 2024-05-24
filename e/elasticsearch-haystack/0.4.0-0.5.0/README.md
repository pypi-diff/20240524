# Comparing `tmp/elasticsearch_haystack-0.4.0.tar.gz` & `tmp/elasticsearch_haystack-0.5.0.tar.gz`

## Comparing `elasticsearch_haystack-0.4.0.tar` & `elasticsearch_haystack-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/docker-compose.yml
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/pydoc/config.yml
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/document_stores/elasticsearch/__init__.py
--rw-r--r--   0        0        0    17688 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/src/haystack_integrations/document_stores/elasticsearch/filters.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/tests/test_bm25_retriever.py
--rw-r--r--   0        0        0    13199 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/tests/test_document_store.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/tests/test_embedding_retriever.py
--rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/tests/test_filters.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/.gitignore
--rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/LICENSE
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/README.md
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/docker-compose.yml
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/pydoc/config.yml
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/document_stores/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    18304 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/src/haystack_integrations/document_stores/elasticsearch/filters.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/tests/test_bm25_retriever.py
+-rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/tests/test_document_store.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/tests/test_embedding_retriever.py
+-rw-r--r--   0        0        0     8013 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/tests/test_filters.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/.gitignore
+-rw-r--r--   0        0        0    11342 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/LICENSE
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/README.md
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 elasticsearch_haystack-0.5.0/PKG-INFO
```

### Comparing `elasticsearch_haystack-0.4.0/pydoc/config.yml` & `elasticsearch_haystack-0.5.0/pydoc/config.yml`

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
   excerpt: Elasticsearch integration for Haystack
   category_slug: integrations-api
   title: Elasticsearch
   slug: integrations-elasticsearch
   order: 70
   markdown:
     descriptive_class_title: false
```

### Comparing `elasticsearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py` & `elasticsearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/elasticsearch/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.4.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py` & `elasticsearch_haystack-0.5.0/src/haystack_integrations/components/retrievers/elasticsearch/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.4.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py` & `elasticsearch_haystack-0.5.0/src/haystack_integrations/document_stores/elasticsearch/document_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     All extra keyword arguments will be passed to the Elasticsearch client.
     """
 
     def __init__(
         self,
         *,
         hosts: Optional[Hosts] = None,
+        custom_mapping: Optional[Dict[str, Any]] = None,
         index: str = "default",
         embedding_similarity_function: Literal["cosine", "dot_product", "l2_norm", "max_inner_product"] = "cosine",
         **kwargs,
     ):
         """
         Creates a new ElasticsearchDocumentStore instance.
 
@@ -78,14 +79,15 @@
         For more information on connection parameters, see the official Elasticsearch
         [documentation](https://www.elastic.co/guide/en/elasticsearch/client/python-api/current/connecting.html)
 
         For the full list of supported kwargs, see the official Elasticsearch
         [reference](https://elasticsearch-py.readthedocs.io/en/stable/api.html#module-elasticsearch)
 
         :param hosts: List of hosts running the Elasticsearch client.
+        :param custom_mapping: Custom mapping for the index. If not provided, a default mapping will be used.
         :param index: Name of index in Elasticsearch.
         :param embedding_similarity_function: The similarity function used to compare Documents embeddings.
             This parameter only takes effect if the index does not yet exist and is created.
             To choose the most appropriate function, look for information about your embedding model.
             To understand how document scores are computed, see the Elasticsearch
             [documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/dense-vector.html#dense-vector-params)
         :param **kwargs: Optional arguments that `Elasticsearch` takes.
@@ -94,37 +96,45 @@
         self._client = Elasticsearch(
             hosts,
             headers={"user-agent": f"haystack-py-ds/{haystack_version}"},
             **kwargs,
         )
         self._index = index
         self._embedding_similarity_function = embedding_similarity_function
+        self._custom_mapping = custom_mapping
         self._kwargs = kwargs
 
         # Check client connection, this will raise if not connected
         self._client.info()
 
-        # configure mapping for the embedding field
-        mappings = {
-            "properties": {
-                "embedding": {"type": "dense_vector", "index": True, "similarity": embedding_similarity_function},
-                "content": {"type": "text"},
-            },
-            "dynamic_templates": [
-                {
-                    "strings": {
-                        "path_match": "*",
-                        "match_mapping_type": "string",
-                        "mapping": {
-                            "type": "keyword",
-                        },
+        if self._custom_mapping and not isinstance(self._custom_mapping, Dict):
+            msg = "custom_mapping must be a dictionary"
+            raise ValueError(msg)
+
+        if self._custom_mapping:
+            mappings = self._custom_mapping
+        else:
+            # Configure mapping for the embedding field if none is provided
+            mappings = {
+                "properties": {
+                    "embedding": {"type": "dense_vector", "index": True, "similarity": embedding_similarity_function},
+                    "content": {"type": "text"},
+                },
+                "dynamic_templates": [
+                    {
+                        "strings": {
+                            "path_match": "*",
+                            "match_mapping_type": "string",
+                            "mapping": {
+                                "type": "keyword",
+                            },
+                        }
                     }
-                }
-            ],
-        }
+                ],
+            }
 
         # Create the index if it doesn't exist
         if not self._client.indices.exists(index=index):
             self._client.indices.create(index=index, mappings=mappings)
 
     def to_dict(self) -> Dict[str, Any]:
         """
@@ -135,14 +145,15 @@
         """
         # This is not the best solution to serialise this class but is the fastest to implement.
         # Not all kwargs types can be serialised to text so this can fail. We must serialise each
         # type explicitly to handle this properly.
         return default_to_dict(
             self,
             hosts=self._hosts,
+            custom_mapping=self._custom_mapping,
             index=self._index,
             embedding_similarity_function=self._embedding_similarity_function,
             **self._kwargs,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "ElasticsearchDocumentStore":
```

### Comparing `elasticsearch_haystack-0.4.0/src/haystack_integrations/document_stores/elasticsearch/filters.py` & `elasticsearch_haystack-0.5.0/src/haystack_integrations/document_stores/elasticsearch/filters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.4.0/tests/test_bm25_retriever.py` & `elasticsearch_haystack-0.5.0/tests/test_bm25_retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     res = retriever.to_dict()
     assert res == {
         "type": "haystack_integrations.components.retrievers.elasticsearch.bm25_retriever.ElasticsearchBM25Retriever",
         "init_parameters": {
             "document_store": {
                 "init_parameters": {
                     "hosts": "some fake host",
+                    "custom_mapping": None,
                     "index": "default",
                     "embedding_similarity_function": "cosine",
                 },
                 "type": "haystack_integrations.document_stores.elasticsearch.document_store.ElasticsearchDocumentStore",
             },
             "filters": {},
             "fuzziness": "AUTO",
```

### Comparing `elasticsearch_haystack-0.4.0/tests/test_document_store.py` & `elasticsearch_haystack-0.5.0/tests/test_document_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 import random
 from typing import List
-from unittest.mock import patch
+from unittest.mock import Mock, patch
 
 import pytest
 from elasticsearch.exceptions import BadRequestError  # type: ignore[import-not-found]
 from haystack.dataclasses.document import Document
 from haystack.document_stores.errors import DocumentStoreError, DuplicateDocumentError
 from haystack.document_stores.types import DuplicatePolicy
 from haystack.testing.document_store import DocumentStoreBaseTests
@@ -19,33 +19,36 @@
 def test_to_dict(_mock_elasticsearch_client):
     document_store = ElasticsearchDocumentStore(hosts="some hosts")
     res = document_store.to_dict()
     assert res == {
         "type": "haystack_integrations.document_stores.elasticsearch.document_store.ElasticsearchDocumentStore",
         "init_parameters": {
             "hosts": "some hosts",
+            "custom_mapping": None,
             "index": "default",
             "embedding_similarity_function": "cosine",
         },
     }
 
 
 @patch("haystack_integrations.document_stores.elasticsearch.document_store.Elasticsearch")
 def test_from_dict(_mock_elasticsearch_client):
     data = {
         "type": "haystack_integrations.document_stores.elasticsearch.document_store.ElasticsearchDocumentStore",
         "init_parameters": {
             "hosts": "some hosts",
+            "custom_mapping": None,
             "index": "default",
             "embedding_similarity_function": "cosine",
         },
     }
     document_store = ElasticsearchDocumentStore.from_dict(data)
     assert document_store._hosts == "some hosts"
     assert document_store._index == "default"
+    assert document_store._custom_mapping is None
     assert document_store._embedding_similarity_function == "cosine"
 
 
 @pytest.mark.integration
 class TestDocumentStore(DocumentStoreBaseTests):
     """
     Common test cases will be provided by `DocumentStoreBaseTests` but
@@ -276,7 +279,37 @@
         docs = [
             Document(content="Hello world", embedding=[0.1, 0.2, 0.3, 0.4]),
             Document(content="Hello world", embedding=[0.1, 0.2]),
         ]
 
         with pytest.raises(DocumentStoreError):
             document_store.write_documents(docs)
+
+    @patch("haystack_integrations.document_stores.elasticsearch.document_store.Elasticsearch")
+    def test_init_with_custom_mapping(self, mock_elasticsearch):
+        custom_mapping = {
+            "properties": {
+                "embedding": {"type": "dense_vector", "index": True, "similarity": "dot_product"},
+                "content": {"type": "text"},
+            },
+            "dynamic_templates": [
+                {
+                    "strings": {
+                        "path_match": "*",
+                        "match_mapping_type": "string",
+                        "mapping": {
+                            "type": "keyword",
+                        },
+                    }
+                }
+            ],
+        }
+        mock_client = Mock(
+            indices=Mock(create=Mock(), exists=Mock(return_value=False)),
+        )
+        mock_elasticsearch.return_value = mock_client
+
+        ElasticsearchDocumentStore(hosts="some hosts", custom_mapping=custom_mapping)
+        mock_client.indices.create.assert_called_once_with(
+            index="default",
+            mappings=custom_mapping,
+        )
```

### Comparing `elasticsearch_haystack-0.4.0/tests/test_embedding_retriever.py` & `elasticsearch_haystack-0.5.0/tests/test_embedding_retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     t = "haystack_integrations.components.retrievers.elasticsearch.embedding_retriever.ElasticsearchEmbeddingRetriever"
     assert res == {
         "type": t,
         "init_parameters": {
             "document_store": {
                 "init_parameters": {
                     "hosts": "some fake host",
+                    "custom_mapping": None,
                     "index": "default",
                     "embedding_similarity_function": "cosine",
                 },
                 "type": "haystack_integrations.document_stores.elasticsearch.document_store.ElasticsearchDocumentStore",
             },
             "filters": {},
             "top_k": 10,
```

### Comparing `elasticsearch_haystack-0.4.0/tests/test_filters.py` & `elasticsearch_haystack-0.5.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.4.0/.gitignore` & `elasticsearch_haystack-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.4.0/LICENSE` & `elasticsearch_haystack-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.4.0/README.md` & `elasticsearch_haystack-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `elasticsearch_haystack-0.4.0/pyproject.toml` & `elasticsearch_haystack-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [
   { name = "Silvano Cerza", email = "silvanocerza@gmail.com" },
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

### Comparing `elasticsearch_haystack-0.4.0/PKG-INFO` & `elasticsearch_haystack-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: elasticsearch-haystack
-Version: 0.4.0
+Version: 0.5.0
 Summary: Haystack 2.x Document Store for ElasticSearch
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/elasticsearch#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/elasticsearch
 Author-email: Silvano Cerza <silvanocerza@gmail.com>
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

