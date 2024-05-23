# Comparing `tmp/langchain_aws-0.1.5.tar.gz` & `tmp/langchain_aws-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_aws-0.1.5.tar", max compression
+gzip compressed data, was "langchain_aws-0.1.6.tar", max compression
```

## Comparing `langchain_aws-0.1.5.tar` & `langchain_aws-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1072 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/LICENSE
--rw-r--r--   0        0        0     1537 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/README.md
--rw-r--r--   0        0        0      611 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/__init__.py
--rw-r--r--   0        0        0      113 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/chat_models/__init__.py
--rw-r--r--   0        0        0    17820 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/chat_models/bedrock.py
--rw-r--r--   0        0        0       96 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/embeddings/__init__.py
--rw-r--r--   0        0        0     7648 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/embeddings/bedrock.py
--rw-r--r--   0        0        0     3808 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/function_calling.py
--rw-r--r--   0        0        0      191 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/graphs/__init__.py
--rw-r--r--   0        0        0    14347 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/graphs/neptune_graph.py
--rw-r--r--   0        0        0    10331 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/graphs/neptune_rdf_graph.py
--rw-r--r--   0        0        0      297 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/llms/__init__.py
--rw-r--r--   0        0        0    37777 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/llms/bedrock.py
--rw-r--r--   0        0        0    13595 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0        0 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/py.typed
--rw-r--r--   0        0        0      251 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/retrievers/__init__.py
--rw-r--r--   0        0        0     5461 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/retrievers/bedrock.py
--rw-r--r--   0        0        0    15186 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/retrievers/kendra.py
--rw-r--r--   0        0        0     1033 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/langchain_aws/utils.py
--rw-r--r--   0        0        0     2743 2024-05-22 16:53:08.393308 langchain_aws-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2378 1970-01-01 00:00:00.000000 langchain_aws-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-23 23:11:54.194951 langchain_aws-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1537 2024-05-23 23:11:54.194951 langchain_aws-0.1.6/README.md
+-rw-r--r--   0        0        0      611 2024-05-23 23:11:54.194951 langchain_aws-0.1.6/langchain_aws/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-23 23:11:54.194951 langchain_aws-0.1.6/langchain_aws/chat_models/__init__.py
+-rw-r--r--   0        0        0    17820 2024-05-23 23:11:54.194951 langchain_aws-0.1.6/langchain_aws/chat_models/bedrock.py
+-rw-r--r--   0        0        0       96 2024-05-23 23:11:54.194951 langchain_aws-0.1.6/langchain_aws/embeddings/__init__.py
+-rw-r--r--   0        0        0     7648 2024-05-23 23:11:54.194951 langchain_aws-0.1.6/langchain_aws/embeddings/bedrock.py
+-rw-r--r--   0        0        0     3808 2024-05-23 23:11:54.194951 langchain_aws-0.1.6/langchain_aws/function_calling.py
+-rw-r--r--   0        0        0      191 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/langchain_aws/graphs/__init__.py
+-rw-r--r--   0        0        0    14347 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/langchain_aws/graphs/neptune_graph.py
+-rw-r--r--   0        0        0    10331 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/langchain_aws/graphs/neptune_rdf_graph.py
+-rw-r--r--   0        0        0      353 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/langchain_aws/llms/__init__.py
+-rw-r--r--   0        0        0    37781 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/langchain_aws/llms/bedrock.py
+-rw-r--r--   0        0        0    13595 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/langchain_aws/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0        0 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/langchain_aws/py.typed
+-rw-r--r--   0        0        0      251 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/langchain_aws/retrievers/__init__.py
+-rw-r--r--   0        0        0     5461 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/langchain_aws/retrievers/bedrock.py
+-rw-r--r--   0        0        0    15186 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/langchain_aws/retrievers/kendra.py
+-rw-r--r--   0        0        0     1033 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/langchain_aws/utils.py
+-rw-r--r--   0        0        0     2743 2024-05-23 23:11:54.198951 langchain_aws-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2378 1970-01-01 00:00:00.000000 langchain_aws-0.1.6/PKG-INFO
```

### Comparing `langchain_aws-0.1.5/LICENSE` & `langchain_aws-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/README.md` & `langchain_aws-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/langchain_aws/__init__.py` & `langchain_aws-0.1.6/langchain_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/langchain_aws/chat_models/bedrock.py` & `langchain_aws-0.1.6/langchain_aws/chat_models/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/langchain_aws/embeddings/bedrock.py` & `langchain_aws-0.1.6/langchain_aws/embeddings/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/langchain_aws/function_calling.py` & `langchain_aws-0.1.6/langchain_aws/function_calling.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/langchain_aws/graphs/neptune_graph.py` & `langchain_aws-0.1.6/langchain_aws/graphs/neptune_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/langchain_aws/graphs/neptune_rdf_graph.py` & `langchain_aws-0.1.6/langchain_aws/graphs/neptune_rdf_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/langchain_aws/llms/bedrock.py` & `langchain_aws-0.1.6/langchain_aws/llms/bedrock.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,15 +253,15 @@
             "text": text,
             "body": response_body,
             "usage": {
                 "prompt_tokens": prompt_tokens,
                 "completion_tokens": completion_tokens,
                 "total_tokens": prompt_tokens + completion_tokens,
             },
-            "stop_reason": response_body["stop_reason"],
+            "stop_reason": response_body.get("stop_reason"),
         }
 
     @classmethod
     def prepare_output_stream(
         cls,
         provider: str,
         response: Any,
```

### Comparing `langchain_aws-0.1.5/langchain_aws/llms/sagemaker_endpoint.py` & `langchain_aws-0.1.6/langchain_aws/llms/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/langchain_aws/retrievers/bedrock.py` & `langchain_aws-0.1.6/langchain_aws/retrievers/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/langchain_aws/retrievers/kendra.py` & `langchain_aws-0.1.6/langchain_aws/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/langchain_aws/utils.py` & `langchain_aws-0.1.6/langchain_aws/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.5/pyproject.toml` & `langchain_aws-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-aws"
-version = "0.1.5"
+version = "0.1.6"
 description = "An integration package connecting AWS and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-aws"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_aws-0.1.5/PKG-INFO` & `langchain_aws-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-aws
-Version: 0.1.5
+Version: 0.1.6
 Summary: An integration package connecting AWS and LangChain
 Home-page: https://github.com/langchain-ai/langchain-aws
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

