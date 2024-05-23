# Comparing `tmp/embedme-0.1.1.tar.gz` & `tmp/embedme-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedme-0.1.1.tar", max compression
+gzip compressed data, was "embedme-0.1.2.tar", max compression
```

## Comparing `embedme-0.1.1.tar` & `embedme-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      159 2023-01-22 14:38:16.031071 embedme-0.1.1/embedme/__init__.py
--rw-r--r--   0        0        0     2121 2023-01-22 19:00:16.797023 embedme-0.1.1/embedme/embedme.py
--rw-r--r--   0        0        0     1607 2023-01-22 13:46:41.917356 embedme-0.1.1/LICENSE
--rw-r--r--   0        0        0      668 2023-01-22 19:56:37.483471 embedme-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2605 2023-01-22 19:08:58.038941 embedme-0.1.1/README.md
--rw-r--r--   0        0        0     3406 2023-01-22 19:56:44.203013 embedme-0.1.1/setup.py
--rw-r--r--   0        0        0     3311 2023-01-22 19:56:44.203013 embedme-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1574 2024-05-23 21:02:03.943084 embedme-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2534 2024-05-23 21:02:03.943188 embedme-0.1.2/README.md
+-rw-r--r--   0        0        0      152 2024-05-23 21:02:03.944141 embedme-0.1.2/embedme/__init__.py
+-rw-r--r--   0        0        0     2056 2024-05-23 21:04:35.478183 embedme-0.1.2/embedme/embedme.py
+-rw-r--r--   0        0        0      729 2024-05-23 21:14:29.860983 embedme-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 embedme-0.1.2/PKG-INFO
```

### Comparing `embedme-0.1.1/LICENSE` & `embedme-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-GNU GENERAL PUBLIC LICENSE
-                      Version 3, 29 June 2007
-
-    A quick bit of code to allow folks to use embeddings easier.
-    Copyright (C) 2023  John Partee
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
-
+GNU GENERAL PUBLIC LICENSE
+                      Version 3, 29 June 2007
+
+    A quick bit of code to allow folks to use embeddings easier.
+    Copyright (C) 2023  John Partee
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+
```

### Comparing `embedme-0.1.1/pyproject.toml` & `embedme-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-[tool.poetry]
-name = "embedme"
-version = "0.1.1"
-description = "Easily create and search text embeddings using OpenAI's API using json for local storage. Just add dicts of info and search! Built for rapid prototyping."
-authors = ["John Partee"]
-repository = "https://github.com/morganpartee/embedme"
-readme = "README.md"
-license = "GPL-3.0-or-later"
-keywords = ["nlp", "embeddings", "search", "openai", "gpt3", "AI", "machine learning"]
-
-[tool.poetry.dependencies]
-python = "^3.10"
-openai = "^0.26.1"
-numpy = "^1.24.1"
-
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-
-[build-system]
-requires = ["poetry>=1.0"]
-build-backend = "poetry.masonry.api"
+[tool.poetry]
+name = "embedme"
+version = "0.1.2"
+description = "Easily create and search text embeddings using OpenAI's API using json for local storage. Just add dicts of info and search! Built for rapid prototyping."
+authors = ["John Partee"]
+repository = "https://github.com/morganpartee/embedme"
+readme = "README.md"
+license = "GPL-3.0-or-later"
+keywords = ["nlp", "embeddings", "search", "openai", "gpt3", "AI", "machine learning"]
+
+[tool.poetry.dependencies]
+python = ">=3.7,<3.13"
+openai = "^0.26.1"
+numpy = "^1.24.1"
+nltk = "^3.8.1"
+
+[tool.poetry.dev-dependencies]
+pytest = "^5.2"
+
+[tool.poetry.group.dev.dependencies]
+ipykernel = "^6.29.4"
+
+[build-system]
+requires = ["poetry>=1.0"]
+build-backend = "poetry.masonry.api"
```

### Comparing `embedme-0.1.1/README.md` & `embedme-0.1.2/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# Embedme
-
-Embedme is a python module that allows you to easily use embeddings from text fields with OpenAI's Embedding API and store them in a local folder.
-
-It's like a lazy version of pinecone - Numpy is actually pretty fast for embeddings stuff at smaller scale, why overthink stuff? We store the data and vectors as json and build the numpy array before you search (and store it until you add more)
-
-## Installation
-
-To install Embedme, you can use pip:
-
-```sh
-pip install embedme
-```
-
-## Setup
-
-The only thing you _must_ do before you use `embedme` is setup auth with OpenAI. We use it to embed your items and search queries, so it is required. I don't want to touch **any** of that code - just sign in how they tell you to, either in the script via a file for the key, or an environment variable for your key.
-
-[OpenAI Python Module (With Auth Instructions)](https://github.com/openai/openai-python)
-
-## Usage
-
-Embedme provides a simple interface to use embeddings from text fields with OpenAI's Embedding API and store them in a local folder.
-
-Check out the example notebook for a better example, but useage is something like:
-
-```py
-import openai
-import nltk
-from more_itertools import chunked
-from embedme import Embedme
-from tqdm import tqdm
-
-# Downloading the NLTK corpus
-nltk.download('gutenberg')
-
-# Creating an instance of the Embedme class
-embedme = Embedme(data_folder='.embedme', model="text-embedding-ada-002")
-
-# Getting the text
-text = nltk.corpus.gutenberg.raw('melville-moby_dick.txt')
-
-# Splitting the text into sentences
-sentences = nltk.sent_tokenize(text)
-
-input("Hey this call will cost you money and take a minute. Like, a few cents probably, but wanted to warn you.")
-
-for i, chunk in enumerate(tqdm(chunked(sentences, 20))):
-    data = {'name': f'moby_dick_chunk_{i}', 'text': ' '.join(chunk)}
-    embedme.add(data, save=False)
-
-embedme.save()
-```
-
-And to search:
-
-```py
-embedme.search("lessons")
-```
-
-You can do anything you would want to with `.vectors` after you call `.prepare_search()` (or... search something, it's automatic mostly), like plot clusters, etc.
-
-## Follow Us
-
-Some friends and I are writing about large language model stuff at [SensibleDefaults.io](https://sensibledefaults.io), honest to god free. Follow us (or star this repo!) if this helps you!
-
-## Note
-
-Embedme uses OpenAI's Embedding API to get embeddings for text fields, so an API key is required to use it. You can get one from https://beta.openai.com/signup/
-
-The token limit today is about 8k, so... you're probably fine
+# Embedme
+
+Embedme is a python module that allows you to easily use embeddings from text fields with OpenAI's Embedding API and store them in a local folder.
+
+It's like a lazy version of pinecone - Numpy is actually pretty fast for embeddings stuff at smaller scale, why overthink stuff? We store the data and vectors as json and build the numpy array before you search (and store it until you add more)
+
+## Installation
+
+To install Embedme, you can use pip:
+
+```sh
+pip install embedme
+```
+
+## Setup
+
+The only thing you _must_ do before you use `embedme` is setup auth with OpenAI. We use it to embed your items and search queries, so it is required. I don't want to touch **any** of that code - just sign in how they tell you to, either in the script via a file for the key, or an environment variable for your key.
+
+[OpenAI Python Module (With Auth Instructions)](https://github.com/openai/openai-python)
+
+## Usage
+
+Embedme provides a simple interface to use embeddings from text fields with OpenAI's Embedding API and store them in a local folder.
+
+Check out the example notebook for a better example, but useage is something like:
+
+```py
+import openai
+import nltk
+from more_itertools import chunked
+from embedme import Embedme
+from tqdm import tqdm
+
+# Downloading the NLTK corpus
+nltk.download('gutenberg')
+
+# Creating an instance of the Embedme class
+embedme = Embedme(data_folder='.embedme', model="text-embedding-ada-002")
+
+# Getting the text
+text = nltk.corpus.gutenberg.raw('melville-moby_dick.txt')
+
+# Splitting the text into sentences
+sentences = nltk.sent_tokenize(text)
+
+input("Hey this call will cost you money and take a minute. Like, a few cents probably, but wanted to warn you.")
+
+for i, chunk in enumerate(tqdm(chunked(sentences, 20))):
+    data = {'name': f'moby_dick_chunk_{i}', 'text': ' '.join(chunk)}
+    embedme.add(data, save=False)
+
+embedme.save()
+```
+
+And to search:
+
+```py
+embedme.search("lessons")
+```
+
+You can do anything you would want to with `.vectors` after you call `.prepare_search()` (or... search something, it's automatic mostly), like plot clusters, etc.
+
+## Follow Us
+
+Some friends and I are writing about large language model stuff at [SensibleDefaults.io](https://sensibledefaults.io), honest to god free. Follow us (or star this repo!) if this helps you!
+
+## Note
+
+Embedme uses OpenAI's Embedding API to get embeddings for text fields, so an API key is required to use it. You can get one from https://beta.openai.com/signup/
+
+The token limit today is about 8k, so... you're probably fine
```

### Comparing `embedme-0.1.1/PKG-INFO` & `embedme-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: embedme
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easily create and search text embeddings using OpenAI's API using json for local storage. Just add dicts of info and search! Built for rapid prototyping.
 Home-page: https://github.com/morganpartee/embedme
 License: GPL-3.0-or-later
 Keywords: nlp,embeddings,search,openai,gpt3,AI,machine learning
 Author: John Partee
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.7,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: openai (>=0.26.1,<0.27.0)
 Project-URL: Repository, https://github.com/morganpartee/embedme
 Description-Content-Type: text/markdown
 
 # Embedme
```

