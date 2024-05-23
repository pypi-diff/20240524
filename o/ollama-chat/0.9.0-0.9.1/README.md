# Comparing `tmp/ollama_chat-0.9.0.tar.gz` & `tmp/ollama_chat-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama_chat-0.9.0.tar", last modified: Thu May 23 21:35:28 2024, max compression
+gzip compressed data, was "ollama_chat-0.9.1.tar", last modified: Thu May 23 22:05:37 2024, max compression
```

## Comparing `ollama_chat-0.9.0.tar` & `ollama_chat-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 21:35:28.188538 ollama_chat-0.9.0/
--rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-05-02 18:06:38.000000 ollama_chat-0.9.0/LICENSE
--rw-r--r--   0 craighobbs   (501) staff       (20)     2709 2024-05-23 21:35:28.188475 ollama_chat-0.9.0/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)     1851 2024-05-23 21:31:11.000000 ollama_chat-0.9.0/README.md
--rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-05-02 18:06:38.000000 ollama_chat-0.9.0/pyproject.toml
--rw-r--r--   0 craighobbs   (501) staff       (20)     1045 2024-05-23 21:35:28.188799 ollama_chat-0.9.0/setup.cfg
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 21:35:28.185833 ollama_chat-0.9.0/src/
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 21:35:28.187011 ollama_chat-0.9.0/src/ollama_chat/
--rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-02 18:06:38.000000 ollama_chat-0.9.0/src/ollama_chat/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)      229 2024-05-02 18:06:38.000000 ollama_chat-0.9.0/src/ollama_chat/__main__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     9552 2024-05-23 20:21:45.000000 ollama_chat-0.9.0/src/ollama_chat/app.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     2125 2024-05-21 19:56:51.000000 ollama_chat-0.9.0/src/ollama_chat/main.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     2659 2024-05-22 20:43:32.000000 ollama_chat-0.9.0/src/ollama_chat/ollama.py
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 21:35:28.187772 ollama_chat-0.9.0/src/ollama_chat/static/
--rw-r--r--   0 craighobbs   (501) staff       (20)     3506 2024-05-23 17:06:52.000000 ollama_chat-0.9.0/src/ollama_chat/static/ollamaChat.smd
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 21:35:28.188184 ollama_chat-0.9.0/src/ollama_chat.egg-info/
--rw-r--r--   0 craighobbs   (501) staff       (20)     2709 2024-05-23 21:35:28.000000 ollama_chat-0.9.0/src/ollama_chat.egg-info/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)      445 2024-05-23 21:35:28.000000 ollama_chat-0.9.0/src/ollama_chat.egg-info/SOURCES.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-05-23 21:35:28.000000 ollama_chat-0.9.0/src/ollama_chat.egg-info/dependency_links.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-05-23 21:35:28.000000 ollama_chat-0.9.0/src/ollama_chat.egg-info/entry_points.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       44 2024-05-23 21:35:28.000000 ollama_chat-0.9.0/src/ollama_chat.egg-info/requires.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-05-23 21:35:28.000000 ollama_chat-0.9.0/src/ollama_chat.egg-info/top_level.txt
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 22:05:37.096566 ollama_chat-0.9.1/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-05-02 18:06:38.000000 ollama_chat-0.9.1/LICENSE
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2709 2024-05-23 22:05:37.096506 ollama_chat-0.9.1/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1851 2024-05-23 21:31:11.000000 ollama_chat-0.9.1/README.md
+-rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-05-02 18:06:38.000000 ollama_chat-0.9.1/pyproject.toml
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1046 2024-05-23 22:05:37.096820 ollama_chat-0.9.1/setup.cfg
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 22:05:37.093972 ollama_chat-0.9.1/src/
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 22:05:37.095100 ollama_chat-0.9.1/src/ollama_chat/
+-rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-02 18:06:38.000000 ollama_chat-0.9.1/src/ollama_chat/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)      229 2024-05-02 18:06:38.000000 ollama_chat-0.9.1/src/ollama_chat/__main__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     9552 2024-05-23 20:21:45.000000 ollama_chat-0.9.1/src/ollama_chat/app.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2125 2024-05-21 19:56:51.000000 ollama_chat-0.9.1/src/ollama_chat/main.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2659 2024-05-22 20:43:32.000000 ollama_chat-0.9.1/src/ollama_chat/ollama.py
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 22:05:37.096107 ollama_chat-0.9.1/src/ollama_chat/static/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3774 2024-05-09 17:20:22.000000 ollama_chat-0.9.1/src/ollama_chat/static/index.html
+-rw-r--r--   0 craighobbs   (501) staff       (20)    17342 2024-05-23 21:09:36.000000 ollama_chat-0.9.1/src/ollama_chat/static/ollamaChat.bare
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3506 2024-05-23 17:06:52.000000 ollama_chat-0.9.1/src/ollama_chat/static/ollamaChat.smd
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 22:05:37.096265 ollama_chat-0.9.1/src/ollama_chat.egg-info/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2709 2024-05-23 22:05:37.000000 ollama_chat-0.9.1/src/ollama_chat.egg-info/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)      518 2024-05-23 22:05:37.000000 ollama_chat-0.9.1/src/ollama_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-05-23 22:05:37.000000 ollama_chat-0.9.1/src/ollama_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-05-23 22:05:37.000000 ollama_chat-0.9.1/src/ollama_chat.egg-info/entry_points.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       44 2024-05-23 22:05:37.000000 ollama_chat-0.9.1/src/ollama_chat.egg-info/requires.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-05-23 22:05:37.000000 ollama_chat-0.9.1/src/ollama_chat.egg-info/top_level.txt
```

### Comparing `ollama_chat-0.9.0/LICENSE` & `ollama_chat-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.0/PKG-INFO` & `ollama_chat-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-chat
-Version: 0.9.0
+Version: 0.9.1
 Summary: ollama-chat
 Home-page: https://github.com/craigahobbs/ollama-chat
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: ollama-chat
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ollama_chat-0.9.0/README.md` & `ollama_chat-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.0/setup.cfg` & `ollama_chat-0.9.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ollama-chat
-version = 0.9.0
+version = 0.9.1
 url = https://github.com/craigahobbs/ollama-chat
 author = Craig A. Hobbs
 author_email = craigahobbs@gmail.com
 license = MIT
 description = ollama-chat
 long_description = file:README.md
 long_description_content_type = text/markdown
@@ -33,14 +33,14 @@
 [options.entry_points]
 console_scripts = 
 	ollama-chat = ollama_chat.main:main
 
 [options.package_data]
 ollama_chat = \
 	static/index.html, \
-	static/ollamaChat.mds, \
+	static/ollamaChat.bare, \
 	static/ollamaChat.smd
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ollama_chat-0.9.0/src/ollama_chat/app.py` & `ollama_chat-0.9.1/src/ollama_chat/app.py`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.0/src/ollama_chat/main.py` & `ollama_chat-0.9.1/src/ollama_chat/main.py`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.0/src/ollama_chat/ollama.py` & `ollama_chat-0.9.1/src/ollama_chat/ollama.py`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.0/src/ollama_chat/static/ollamaChat.smd` & `ollama_chat-0.9.1/src/ollama_chat/static/ollamaChat.smd`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.0/src/ollama_chat.egg-info/PKG-INFO` & `ollama_chat-0.9.1/src/ollama_chat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-chat
-Version: 0.9.0
+Version: 0.9.1
 Summary: ollama-chat
 Home-page: https://github.com/craigahobbs/ollama-chat
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: ollama-chat
 Classifier: Development Status :: 5 - Production/Stable
```

