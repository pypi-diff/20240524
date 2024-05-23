# Comparing `tmp/embedme-0.1.4.tar.gz` & `tmp/embedme-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedme-0.1.4.tar", max compression
+gzip compressed data, was "embedme-0.1.5.tar", max compression
```

## Comparing `embedme-0.1.4.tar` & `embedme-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1574 2024-05-23 22:01:30.316373 embedme-0.1.4/LICENSE
--rw-r--r--   0        0        0     2534 2024-05-23 22:01:30.316485 embedme-0.1.4/README.md
--rw-r--r--   0        0        0      152 2024-05-23 22:01:30.317539 embedme-0.1.4/embedme/__init__.py
--rw-r--r--   0        0        0     2056 2024-05-23 22:01:30.317645 embedme-0.1.4/embedme/embedme.py
--rw-r--r--   0        0        0      729 2024-05-23 22:09:42.979534 embedme-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 embedme-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1574 2024-05-23 22:01:30.316373 embedme-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2534 2024-05-23 22:01:30.316485 embedme-0.1.5/README.md
+-rw-r--r--   0        0        0      152 2024-05-23 22:01:30.317539 embedme-0.1.5/embedme/__init__.py
+-rw-r--r--   0        0        0     2088 2024-05-23 22:19:32.332978 embedme-0.1.5/embedme/embedme.py
+-rw-r--r--   0        0        0      729 2024-05-23 22:21:56.584435 embedme-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 embedme-0.1.5/PKG-INFO
```

### Comparing `embedme-0.1.4/LICENSE` & `embedme-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `embedme-0.1.4/README.md` & `embedme-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `embedme-0.1.4/embedme/embedme.py` & `embedme-0.1.5/embedme/embedme.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
 import json
 import numpy as np
-import openai
+from openai import OpenAI
 
 
+client = OpenAI()
+
 class Embedme:
     def __init__(self, data_folder=".embedme", model="text-embedding-3-small"):
         self.data_folder = data_folder
         if not os.path.exists(self.data_folder):
             os.makedirs(self.data_folder)
         self.data = {}  # store the data here
         self.vectors = None
         self.model = model
 
     def get_embedding(self, text):
         text = text.replace("\n", " ")
-        return openai.Embedding.create(input=[text], model=self.model)["data"][0][
+        return client.embeddings.create(input=[text], model=self.model)["data"][0][
             "embedding"
         ]
 
     def add(self, data, save=True):
         name = data["name"]
         embeddings = self.get_embedding(data["text"])
```

### Comparing `embedme-0.1.4/pyproject.toml` & `embedme-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "embedme"
-version = "0.1.4"
+version = "0.1.5"
 description = "Easily create and search text embeddings using OpenAI's API using json for local storage. Just add dicts of info and search! Built for rapid prototyping."
 authors = ["John Partee"]
 repository = "https://github.com/morganpartee/embedme"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 keywords = ["nlp", "embeddings", "search", "openai", "gpt3", "AI", "machine learning"]
```

### Comparing `embedme-0.1.4/PKG-INFO` & `embedme-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedme
-Version: 0.1.4
+Version: 0.1.5
 Summary: Easily create and search text embeddings using OpenAI's API using json for local storage. Just add dicts of info and search! Built for rapid prototyping.
 Home-page: https://github.com/morganpartee/embedme
 License: GPL-3.0-or-later
 Keywords: nlp,embeddings,search,openai,gpt3,AI,machine learning
 Author: John Partee
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

