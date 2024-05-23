# Comparing `tmp/trace_attributes-3.0.8.tar.gz` & `tmp/trace_attributes-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trace_attributes-3.0.8.tar", last modified: Fri May 17 15:56:19 2024, max compression
+gzip compressed data, was "trace_attributes-4.0.0.tar", last modified: Thu May 23 17:10:41 2024, max compression
```

## Comparing `trace_attributes-3.0.8.tar` & `trace_attributes-4.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:19.007717 trace_attributes-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 15:56:08.000000 trace_attributes-3.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-17 15:56:19.007717 trace_attributes-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    47682 2024-05-17 15:56:08.000000 trace_attributes-3.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:56:19.007717 trace_attributes-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-17 15:56:08.000000 trace_attributes-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:19.003717 trace_attributes-3.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:19.003717 trace_attributes-3.0.8/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:19.003717 trace_attributes-3.0.8/src/python/langtrace/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 15:56:08.000000 trace_attributes-3.0.8/src/python/langtrace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:19.003717 trace_attributes-3.0.8/src/python/langtrace/trace_attributes/
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-17 15:56:08.000000 trace_attributes-3.0.8/src/python/langtrace/trace_attributes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:19.007717 trace_attributes-3.0.8/src/python/langtrace/trace_attributes/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 15:56:08.000000 trace_attributes-3.0.8/src/python/langtrace/trace_attributes/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-17 15:56:08.000000 trace_attributes-3.0.8/src/python/langtrace/trace_attributes/models/database_span_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-17 15:56:08.000000 trace_attributes-3.0.8/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-17 15:56:08.000000 trace_attributes-3.0.8/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:56:19.007717 trace_attributes-3.0.8/src/python/trace_attributes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-17 15:56:18.000000 trace_attributes-3.0.8/src/python/trace_attributes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-17 15:56:18.000000 trace_attributes-3.0.8/src/python/trace_attributes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:56:18.000000 trace_attributes-3.0.8/src/python/trace_attributes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-17 15:56:18.000000 trace_attributes-3.0.8/src/python/trace_attributes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 15:56:18.000000 trace_attributes-3.0.8/src/python/trace_attributes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:10:41.448571 trace_attributes-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 17:10:29.000000 trace_attributes-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 17:10:41.448571 trace_attributes-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    47682 2024-05-23 17:10:29.000000 trace_attributes-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:10:41.448571 trace_attributes-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-23 17:10:29.000000 trace_attributes-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:10:41.444571 trace_attributes-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:10:41.444571 trace_attributes-4.0.0/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:10:41.448571 trace_attributes-4.0.0/src/python/langtrace/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 17:10:29.000000 trace_attributes-4.0.0/src/python/langtrace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:10:41.448571 trace_attributes-4.0.0/src/python/langtrace/trace_attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-23 17:10:29.000000 trace_attributes-4.0.0/src/python/langtrace/trace_attributes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:10:41.448571 trace_attributes-4.0.0/src/python/langtrace/trace_attributes/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 17:10:29.000000 trace_attributes-4.0.0/src/python/langtrace/trace_attributes/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-23 17:10:29.000000 trace_attributes-4.0.0/src/python/langtrace/trace_attributes/models/database_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-23 17:10:29.000000 trace_attributes-4.0.0/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-23 17:10:29.000000 trace_attributes-4.0.0/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:10:41.448571 trace_attributes-4.0.0/src/python/trace_attributes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 17:10:41.000000 trace_attributes-4.0.0/src/python/trace_attributes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-23 17:10:41.000000 trace_attributes-4.0.0/src/python/trace_attributes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:10:41.000000 trace_attributes-4.0.0/src/python/trace_attributes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 17:10:41.000000 trace_attributes-4.0.0/src/python/trace_attributes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 17:10:41.000000 trace_attributes-4.0.0/src/python/trace_attributes.egg-info/top_level.txt
```

### Comparing `trace_attributes-3.0.8/LICENSE` & `trace_attributes-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.8/PKG-INFO` & `trace_attributes-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 3.0.8
+Version: 4.0.0
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trace_attributes-3.0.8/README.md` & `trace_attributes-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.8/setup.py` & `trace_attributes-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='trace-attributes',  # Choose a unique name for PyPI
-    version='3.0.8',
+    version='4.0.0',
     author='Karthik Kalyanaraman',
     author_email='karthik@scale3labs.com',
     description='LangTrace - Trace Attributes',
     long_description="LangTrace - Trace Attributes",
     long_description_content_type='text/markdown',
     url='https://github.com/Scale3-Labs/langtrace-trace-attributes',  # Project home page
     package_dir={'': 'src/python'},
```

### Comparing `trace_attributes-3.0.8/src/python/langtrace/trace_attributes/__init__.py` & `trace_attributes-4.0.0/src/python/langtrace/trace_attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.8/src/python/langtrace/trace_attributes/models/database_span_attributes.py` & `trace_attributes-4.0.0/src/python/langtrace/trace_attributes/models/database_span_attributes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  database_span_attributes.json
-#   timestamp: 2024-04-10T15:00:03+00:00
+#   timestamp: 2024-05-23T16:57:17+00:00
 
 from __future__ import annotations
 
 from typing import Optional
 
 from pydantic import BaseModel, Extra, Field
 
@@ -17,19 +17,17 @@
     langtrace_service_type: str = Field(..., alias='langtrace.service.type')
     langtrace_service_version: Optional[str] = Field(
         None, alias='langtrace.service.version'
     )
     langtrace_sdk_name: str = Field(..., alias='langtrace.sdk.name')
     langtrace_version: str = Field(..., alias='langtrace.version')
     server_address: Optional[str] = Field(None, alias='server.address')
+    db_query: str = Field(..., alias='db.query')
+    db_response: Optional[str] = Field(None, alias='db.response')
     db_operation: Optional[str] = Field(None, alias='db.operation')
     db_system: str = Field(..., alias='db.system')
     db_namespace: Optional[str] = Field(None, alias='db.namespace')
     db_index: Optional[str] = Field(None, alias='db.index')
     db_collection_name: Optional[str] = Field(None, alias='db.collection.name')
-    db_pinecone_top_k: Optional[float] = Field(None, alias='db.pinecone.top_k')
-    db_chromadb_embedding_model: Optional[str] = Field(
-        None, alias='db.chromadb.embedding_model'
-    )
-    user_id: Optional[str] = Field(None, alias='user.id')
-    user_feedback_rating: Optional[int] = Field(None, alias='user.feedback.rating')
+    db_top_k: Optional[float] = Field(None, alias='db.top_k')
+    db_embedding_model: Optional[str] = Field(None, alias='db.embedding_model')
     langtrace_testId: Optional[str] = Field(None, alias='langtrace.testId')
```

### Comparing `trace_attributes-3.0.8/src/python/langtrace/trace_attributes/models/framework_span_attributes.py` & `trace_attributes-4.0.0/src/python/langtrace/trace_attributes/models/framework_span_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  framework_span_attributes.json
-#   timestamp: 2024-04-28T02:15:38+00:00
+#   timestamp: 2024-05-23T16:57:21+00:00
 
 from __future__ import annotations
 
 from typing import Optional
 
 from pydantic import BaseModel, Extra, Field
 
@@ -27,10 +27,8 @@
     langgraph_node: Optional[str] = Field(None, alias='langgraph.node')
     langgraph_edge: Optional[str] = Field(None, alias='langgraph.edge')
     langgraph_finishpoint: Optional[str] = Field(None, alias='langgraph.finishpoint')
     langgraph_task_name: Optional[str] = Field(None, alias='langgraph.task.name')
     llamaindex_task_name: Optional[str] = Field(None, alias='llamaindex.task.name')
     llamaindex_inputs: Optional[str] = Field(None, alias='llamaindex.inputs')
     llamaindex_outputs: Optional[str] = Field(None, alias='llamaindex.outputs')
-    user_id: Optional[str] = Field(None, alias='user.id')
-    user_feedback_rating: Optional[int] = Field(None, alias='user.feedback.rating')
     langtrace_testId: Optional[str] = Field(None, alias='langtrace.testId')
```

### Comparing `trace_attributes-3.0.8/src/python/langtrace/trace_attributes/models/llm_span_attributes.py` & `trace_attributes-4.0.0/src/python/langtrace/trace_attributes/models/llm_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.8/src/python/trace_attributes.egg-info/PKG-INFO` & `trace_attributes-4.0.0/src/python/trace_attributes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 3.0.8
+Version: 4.0.0
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trace_attributes-3.0.8/src/python/trace_attributes.egg-info/SOURCES.txt` & `trace_attributes-4.0.0/src/python/trace_attributes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

