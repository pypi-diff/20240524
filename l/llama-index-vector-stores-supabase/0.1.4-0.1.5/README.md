# Comparing `tmp/llama_index_vector_stores_supabase-0.1.4.tar.gz` & `tmp/llama_index_vector_stores_supabase-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_supabase-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_supabase-0.1.5.tar", max compression
```

## Comparing `llama_index_vector_stores_supabase-0.1.4.tar` & `llama_index_vector_stores_supabase-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       49 2024-05-22 01:12:50.947597 llama_index_vector_stores_supabase-0.1.4/README.md
--rw-r--r--   0        0        0      107 2024-05-22 01:12:50.947597 llama_index_vector_stores_supabase-0.1.4/llama_index/vector_stores/supabase/__init__.py
--rw-r--r--   0        0        0     6427 2024-05-22 01:12:50.947597 llama_index_vector_stores_supabase-0.1.4/llama_index/vector_stores/supabase/base.py
--rw-r--r--   0        0        0     1483 2024-05-22 01:12:50.947597 llama_index_vector_stores_supabase-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 llama_index_vector_stores_supabase-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-05-24 14:26:14.990810 llama_index_vector_stores_supabase-0.1.5/README.md
+-rw-r--r--   0        0        0      107 2024-05-24 14:26:14.990810 llama_index_vector_stores_supabase-0.1.5/llama_index/vector_stores/supabase/__init__.py
+-rw-r--r--   0        0        0     6501 2024-05-24 14:26:14.990810 llama_index_vector_stores_supabase-0.1.5/llama_index/vector_stores/supabase/base.py
+-rw-r--r--   0        0        0     1483 2024-05-24 14:26:14.990810 llama_index_vector_stores_supabase-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 llama_index_vector_stores_supabase-0.1.5/PKG-INFO
```

### Comparing `llama_index_vector_stores_supabase-0.1.4/llama_index/vector_stores/supabase/base.py` & `llama_index_vector_stores_supabase-0.1.5/llama_index/vector_stores/supabase/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,18 @@
             )
             self._collection = self._client.create_collection(
                 name=collection_name, dimension=dimension
             )
 
     def __del__(self) -> None:
         """Close the client when the object is deleted."""
-        if self._client is not None:
+        try:  # try-catch in case the attribute is not present
             self._client.disconnect()
+        except AttributeError:
+            pass
 
     @property
     def client(self) -> None:
         """Get client."""
         return
 
     def _to_vecs_filters(self, filters: MetadataFilters) -> Any:
```

### Comparing `llama_index_vector_stores_supabase-0.1.4/pyproject.toml` & `llama_index_vector_stores_supabase-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores supabase integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-supabase"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 vecs = "^0.4.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_supabase-0.1.4/PKG-INFO` & `llama_index_vector_stores_supabase-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-supabase
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index vector_stores supabase integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

