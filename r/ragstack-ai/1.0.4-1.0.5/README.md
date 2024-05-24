# Comparing `tmp/ragstack_ai-1.0.4.tar.gz` & `tmp/ragstack_ai-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai-1.0.4.tar", max compression
+gzip compressed data, was "ragstack_ai-1.0.5.tar", max compression
```

## Comparing `ragstack_ai-1.0.4.tar` & `ragstack_ai-1.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3781 2024-05-21 20:21:58.965071 ragstack_ai-1.0.4/LICENSE.md
--rw-r--r--   0        0        0     2395 2024-05-21 20:21:58.965071 ragstack_ai-1.0.4/PACKAGE_README.md
--rw-r--r--   0        0        0     1796 2024-05-21 20:21:58.993070 ragstack_ai-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      271 2024-05-21 20:21:58.993070 ragstack_ai-1.0.4/ragstack/__init__.py
--rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 ragstack_ai-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3781 2024-05-24 13:07:00.512500 ragstack_ai-1.0.5/LICENSE.md
+-rw-r--r--   0        0        0     2395 2024-05-24 13:07:00.512500 ragstack_ai-1.0.5/PACKAGE_README.md
+-rw-r--r--   0        0        0     1798 2024-05-24 13:07:00.560501 ragstack_ai-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-05-24 13:07:00.560501 ragstack_ai-1.0.5/ragstack/__init__.py
+-rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 ragstack_ai-1.0.5/PKG-INFO
```

### Comparing `ragstack_ai-1.0.4/LICENSE.md` & `ragstack_ai-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai-1.0.4/PACKAGE_README.md` & `ragstack_ai-1.0.5/PACKAGE_README.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai-1.0.4/pyproject.toml` & `ragstack_ai-1.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "ragstack-ai"
-version = "1.0.4"
+version = "1.0.5"
 description = "DataStax RAGStack"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "PACKAGE_README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-ragstack-ai-langchain = { version = "1.0.4", extras = ["colbert", "google", "nvidia"] }
-ragstack-ai-llamaindex = { version = "1.0.3", extras = ["colbert", "google", "azure", "bedrock"] }
-ragstack-ai-colbert = "1.0.3"
+ragstack-ai-langchain = { version = "1.0.5", extras = ["colbert", "google", "nvidia"] }
+ragstack-ai-llamaindex = { version = "1.0.4", extras = ["colbert", "google", "azure", "bedrock"] }
+ragstack-ai-colbert = "1.0.4"
 
 [tool.poetry.group.test.dependencies]
 ragstack-ai-langchain = { path = "libs/langchain", develop = true, extras = ["colbert", "google", "nvidia"] }
 ragstack-ai-llamaindex = { path = "libs/llamaindex", develop = true, extras = ["colbert", "google", "azure", "bedrock"] }
 ragstack-ai-colbert = { path = "libs/colbert", develop = true }
 
 pytest = "^7.3.0"
@@ -51,17 +51,19 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 
 
 
+
 [tool.poetry.group.dev.dependencies]
 yamllint = "^1.34.0"
 
 
 
 
 
+
 [tool.poetry.group.notebooks.dependencies]
 nbmake = "*"
 astrapy = "*"
```

### Comparing `ragstack_ai-1.0.4/PKG-INFO` & `ragstack_ai-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ragstack-ai
-Version: 1.0.4
+Version: 1.0.5
 Summary: DataStax RAGStack
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ragstack-ai-colbert (==1.0.3)
-Requires-Dist: ragstack-ai-langchain[colbert,google,nvidia] (==1.0.4)
-Requires-Dist: ragstack-ai-llamaindex[azure,bedrock,colbert,google] (==1.0.3)
+Requires-Dist: ragstack-ai-colbert (==1.0.4)
+Requires-Dist: ragstack-ai-langchain[colbert,google,nvidia] (==1.0.5)
+Requires-Dist: ragstack-ai-llamaindex[azure,bedrock,colbert,google] (==1.0.4)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack
 [![Release Notes](https://img.shields.io/github/v/release/datastax/ragstack-ai.svg)](https://github.com/datastax/ragstack-ai/releases)
 [![Downloads](https://static.pepy.tech/badge/ragstack-ai/month)](https://www.pepy.tech/projects/ragstack-ai)
```

