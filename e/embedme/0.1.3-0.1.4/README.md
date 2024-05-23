# Comparing `tmp/embedme-0.1.3.tar.gz` & `tmp/embedme-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedme-0.1.3.tar", max compression
+gzip compressed data, was "embedme-0.1.4.tar", max compression
```

## Comparing `embedme-0.1.3.tar` & `embedme-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1574 2024-05-23 22:01:30.316373 embedme-0.1.3/LICENSE
--rw-r--r--   0        0        0     2534 2024-05-23 22:01:30.316485 embedme-0.1.3/README.md
--rw-r--r--   0        0        0      152 2024-05-23 22:01:30.317539 embedme-0.1.3/embedme/__init__.py
--rw-r--r--   0        0        0     2056 2024-05-23 22:01:30.317645 embedme-0.1.3/embedme/embedme.py
--rw-r--r--   0        0        0      729 2024-05-23 22:03:06.357126 embedme-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3513 1970-01-01 00:00:00.000000 embedme-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1574 2024-05-23 22:01:30.316373 embedme-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2534 2024-05-23 22:01:30.316485 embedme-0.1.4/README.md
+-rw-r--r--   0        0        0      152 2024-05-23 22:01:30.317539 embedme-0.1.4/embedme/__init__.py
+-rw-r--r--   0        0        0     2056 2024-05-23 22:01:30.317645 embedme-0.1.4/embedme/embedme.py
+-rw-r--r--   0        0        0      729 2024-05-23 22:09:42.979534 embedme-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 embedme-0.1.4/PKG-INFO
```

### Comparing `embedme-0.1.3/LICENSE` & `embedme-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `embedme-0.1.3/README.md` & `embedme-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `embedme-0.1.3/embedme/embedme.py` & `embedme-0.1.4/embedme/embedme.py`

 * *Files identical despite different names*

### Comparing `embedme-0.1.3/pyproject.toml` & `embedme-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "embedme"
-version = "0.1.3"
+version = "0.1.4"
 description = "Easily create and search text embeddings using OpenAI's API using json for local storage. Just add dicts of info and search! Built for rapid prototyping."
 authors = ["John Partee"]
 repository = "https://github.com/morganpartee/embedme"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 keywords = ["nlp", "embeddings", "search", "openai", "gpt3", "AI", "machine learning"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
-openai = "^0.26.1"
+openai = "^1.30.2"
 numpy = "^1.24.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 nltk = "^3.8.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `embedme-0.1.3/PKG-INFO` & `embedme-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: embedme
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easily create and search text embeddings using OpenAI's API using json for local storage. Just add dicts of info and search! Built for rapid prototyping.
 Home-page: https://github.com/morganpartee/embedme
 License: GPL-3.0-or-later
 Keywords: nlp,embeddings,search,openai,gpt3,AI,machine learning
 Author: John Partee
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
-Requires-Dist: openai (>=0.26.1,<0.27.0)
+Requires-Dist: openai (>=1.30.2,<2.0.0)
 Project-URL: Repository, https://github.com/morganpartee/embedme
 Description-Content-Type: text/markdown
 
 # Embedme
 
 Embedme is a python module that allows you to easily use embeddings from text fields with OpenAI's Embedding API and store them in a local folder.
```

