# Comparing `tmp/lavague_contexts_openai-0.1.2.tar.gz` & `tmp/lavague_contexts_openai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_contexts_openai-0.1.2.tar", max compression
+gzip compressed data, was "lavague_contexts_openai-0.1.3.tar", max compression
```

## Comparing `lavague_contexts_openai-0.1.2.tar` & `lavague_contexts_openai-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       32 2024-05-15 22:13:36.166566 lavague_contexts_openai-0.1.2/README.md
--rw-r--r--   0        0        0       75 2024-05-15 22:13:36.166566 lavague_contexts_openai-0.1.2/lavague/contexts/openai/__init__.py
--rw-r--r--   0        0        0     2193 2024-05-21 21:06:53.305594 lavague_contexts_openai-0.1.2/lavague/contexts/openai/base.py
--rw-r--r--   0        0        0     1171 2024-05-21 23:05:42.411752 lavague_contexts_openai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 lavague_contexts_openai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       32 2024-05-22 18:18:44.473928 lavague_contexts_openai-0.1.3/README.md
+-rw-r--r--   0        0        0       75 2024-05-22 18:18:44.474112 lavague_contexts_openai-0.1.3/lavague/contexts/openai/__init__.py
+-rw-r--r--   0        0        0     2186 2024-05-24 06:43:44.648233 lavague_contexts_openai-0.1.3/lavague/contexts/openai/base.py
+-rw-r--r--   0        0        0     1171 2024-05-24 11:05:35.199763 lavague_contexts_openai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 lavague_contexts_openai-0.1.3/PKG-INFO
```

### Comparing `lavague_contexts_openai-0.1.2/lavague/contexts/openai/base.py` & `lavague_contexts_openai-0.1.3/lavague/contexts/openai/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from lavague.core.context import Context, DEFAULT_MAX_TOKENS, DEFAULT_TEMPERATURE
 
 
 class OpenaiContext(Context):
     def __init__(
         self,
         api_key: Optional[str] = None,
-        llm: str = "gpt-3.5-turbo",
+        llm: str = "gpt-4o",
         mm_llm: str = "gpt-4o",
         embedding: str = "text-embedding-3-large",
     ) -> Context:
         if api_key is None:
             api_key = os.getenv("OPENAI_API_KEY")
             if api_key is None:
                 raise ValueError("OPENAI_API_KEY is not set")
```

### Comparing `lavague_contexts_openai-0.1.2/pyproject.toml` & `lavague_contexts_openai-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-contexts-openai"
-version = "0.1.2"
+version = "0.1.3"
 description = "Openai integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_contexts_openai-0.1.2/PKG-INFO` & `lavague_contexts_openai-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-contexts-openai
-Version: 0.1.2
+Version: 0.1.3
 Summary: Openai integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

