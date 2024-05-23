# Comparing `tmp/embedme-0.1.2.tar.gz` & `tmp/embedme-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedme-0.1.2.tar", max compression
+gzip compressed data, was "embedme-0.1.3.tar", max compression
```

## Comparing `embedme-0.1.2.tar` & `embedme-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1574 2024-05-23 21:02:03.943084 embedme-0.1.2/LICENSE
--rw-r--r--   0        0        0     2534 2024-05-23 21:02:03.943188 embedme-0.1.2/README.md
--rw-r--r--   0        0        0      152 2024-05-23 21:02:03.944141 embedme-0.1.2/embedme/__init__.py
--rw-r--r--   0        0        0     2056 2024-05-23 21:04:35.478183 embedme-0.1.2/embedme/embedme.py
--rw-r--r--   0        0        0      729 2024-05-23 21:14:29.860983 embedme-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 embedme-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1574 2024-05-23 22:01:30.316373 embedme-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2534 2024-05-23 22:01:30.316485 embedme-0.1.3/README.md
+-rw-r--r--   0        0        0      152 2024-05-23 22:01:30.317539 embedme-0.1.3/embedme/__init__.py
+-rw-r--r--   0        0        0     2056 2024-05-23 22:01:30.317645 embedme-0.1.3/embedme/embedme.py
+-rw-r--r--   0        0        0      729 2024-05-23 22:03:06.357126 embedme-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3513 1970-01-01 00:00:00.000000 embedme-0.1.3/PKG-INFO
```

### Comparing `embedme-0.1.2/LICENSE` & `embedme-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `embedme-0.1.2/README.md` & `embedme-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `embedme-0.1.2/embedme/embedme.py` & `embedme-0.1.3/embedme/embedme.py`

 * *Files identical despite different names*

### Comparing `embedme-0.1.2/pyproject.toml` & `embedme-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "embedme"
-version = "0.1.2"
+version = "0.1.3"
 description = "Easily create and search text embeddings using OpenAI's API using json for local storage. Just add dicts of info and search! Built for rapid prototyping."
 authors = ["John Partee"]
 repository = "https://github.com/morganpartee/embedme"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 keywords = ["nlp", "embeddings", "search", "openai", "gpt3", "AI", "machine learning"]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.13"
+python = ">=3.8,<3.13"
 openai = "^0.26.1"
 numpy = "^1.24.1"
-nltk = "^3.8.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
+nltk = "^3.8.1"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.4"
 
 [build-system]
 requires = ["poetry>=1.0"]
 build-backend = "poetry.masonry.api"
```

### Comparing `embedme-0.1.2/PKG-INFO` & `embedme-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: embedme
-Version: 0.1.2
+Version: 0.1.3
 Summary: Easily create and search text embeddings using OpenAI's API using json for local storage. Just add dicts of info and search! Built for rapid prototyping.
 Home-page: https://github.com/morganpartee/embedme
 License: GPL-3.0-or-later
 Keywords: nlp,embeddings,search,openai,gpt3,AI,machine learning
 Author: John Partee
-Requires-Python: >=3.7,<3.13
+Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: openai (>=0.26.1,<0.27.0)
 Project-URL: Repository, https://github.com/morganpartee/embedme
 Description-Content-Type: text/markdown
 
 # Embedme
```

