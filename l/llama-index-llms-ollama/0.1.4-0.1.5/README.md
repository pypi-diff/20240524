# Comparing `tmp/llama_index_llms_ollama-0.1.4.tar.gz` & `tmp/llama_index_llms_ollama-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_ollama-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_llms_ollama-0.1.5.tar", max compression
```

## Comparing `llama_index_llms_ollama-0.1.4.tar` & `llama_index_llms_ollama-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       38 2024-05-17 20:26:28.909530 llama_index_llms_ollama-0.1.4/README.md
--rw-r--r--   0        0        0       70 2024-05-17 20:26:28.909530 llama_index_llms_ollama-0.1.4/llama_index/llms/ollama/__init__.py
--rw-r--r--   0        0        0    12406 2024-05-17 20:26:28.909530 llama_index_llms_ollama-0.1.4/llama_index/llms/ollama/base.py
--rw-r--r--   0        0        0     1421 2024-05-17 20:26:28.909530 llama_index_llms_ollama-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 llama_index_llms_ollama-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       38 2024-05-24 18:35:27.206055 llama_index_llms_ollama-0.1.5/README.md
+-rw-r--r--   0        0        0       70 2024-05-24 18:35:27.206055 llama_index_llms_ollama-0.1.5/llama_index/llms/ollama/__init__.py
+-rw-r--r--   0        0        0    12407 2024-05-24 18:35:27.206055 llama_index_llms_ollama-0.1.5/llama_index/llms/ollama/base.py
+-rw-r--r--   0        0        0     1421 2024-05-24 18:35:27.206055 llama_index_llms_ollama-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 llama_index_llms_ollama-0.1.5/PKG-INFO
```

### Comparing `llama_index_llms_ollama-0.1.4/llama_index/llms/ollama/base.py` & `llama_index_llms_ollama-0.1.5/llama_index/llms/ollama/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
                 timeout=Timeout(self.request_timeout)
             ) as client:
                 async with client.stream(
                     method="POST",
                     url=f"{self.base_url}/api/generate",
                     json=payload,
                 ) as response:
-                    async for line in response.aiter_text():
+                    async for line in response.aiter_lines():
                         if line:
                             chunk = json.loads(line)
                             delta = chunk.get("response")
                             yield CompletionResponse(
                                 delta=delta,
                                 text=delta,
                                 raw=chunk,
```

### Comparing `llama_index_llms_ollama-0.1.4/pyproject.toml` & `llama_index_llms_ollama-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms ollama integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-ollama"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_llms_ollama-0.1.4/PKG-INFO` & `llama_index_llms_ollama-0.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-ollama
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index llms ollama integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

