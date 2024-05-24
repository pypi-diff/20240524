# Comparing `tmp/ollama_chat-0.9.2.tar.gz` & `tmp/ollama_chat-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama_chat-0.9.2.tar", last modified: Thu May 23 22:31:14 2024, max compression
+gzip compressed data, was "ollama_chat-0.9.3.tar", last modified: Fri May 24 00:04:39 2024, max compression
```

## Comparing `ollama_chat-0.9.2.tar` & `ollama_chat-0.9.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 22:31:14.126561 ollama_chat-0.9.2/
--rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-05-02 18:06:38.000000 ollama_chat-0.9.2/LICENSE
--rw-r--r--   0 craighobbs   (501) staff       (20)     2709 2024-05-23 22:31:14.126493 ollama_chat-0.9.2/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)     1851 2024-05-23 21:31:11.000000 ollama_chat-0.9.2/README.md
--rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-05-02 18:06:38.000000 ollama_chat-0.9.2/pyproject.toml
--rw-r--r--   0 craighobbs   (501) staff       (20)     1039 2024-05-23 22:31:14.126819 ollama_chat-0.9.2/setup.cfg
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 22:31:14.123995 ollama_chat-0.9.2/src/
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 22:31:14.125093 ollama_chat-0.9.2/src/ollama_chat/
--rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-02 18:06:38.000000 ollama_chat-0.9.2/src/ollama_chat/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)      229 2024-05-02 18:06:38.000000 ollama_chat-0.9.2/src/ollama_chat/__main__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     9552 2024-05-23 20:21:45.000000 ollama_chat-0.9.2/src/ollama_chat/app.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     2125 2024-05-21 19:56:51.000000 ollama_chat-0.9.2/src/ollama_chat/main.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     2659 2024-05-22 20:43:32.000000 ollama_chat-0.9.2/src/ollama_chat/ollama.py
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 22:31:14.126083 ollama_chat-0.9.2/src/ollama_chat/static/
--rw-r--r--   0 craighobbs   (501) staff       (20)     3774 2024-05-09 17:20:22.000000 ollama_chat-0.9.2/src/ollama_chat/static/index.html
--rw-r--r--   0 craighobbs   (501) staff       (20)    17342 2024-05-23 21:09:36.000000 ollama_chat-0.9.2/src/ollama_chat/static/ollamaChat.bare
--rw-r--r--   0 craighobbs   (501) staff       (20)     3506 2024-05-23 17:06:52.000000 ollama_chat-0.9.2/src/ollama_chat/static/ollamaChat.smd
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-23 22:31:14.126236 ollama_chat-0.9.2/src/ollama_chat.egg-info/
--rw-r--r--   0 craighobbs   (501) staff       (20)     2709 2024-05-23 22:31:14.000000 ollama_chat-0.9.2/src/ollama_chat.egg-info/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)      518 2024-05-23 22:31:14.000000 ollama_chat-0.9.2/src/ollama_chat.egg-info/SOURCES.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-05-23 22:31:14.000000 ollama_chat-0.9.2/src/ollama_chat.egg-info/dependency_links.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-05-23 22:31:14.000000 ollama_chat-0.9.2/src/ollama_chat.egg-info/entry_points.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       44 2024-05-23 22:31:14.000000 ollama_chat-0.9.2/src/ollama_chat.egg-info/requires.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-05-23 22:31:14.000000 ollama_chat-0.9.2/src/ollama_chat.egg-info/top_level.txt
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-24 00:04:39.319512 ollama_chat-0.9.3/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-05-02 18:06:38.000000 ollama_chat-0.9.3/LICENSE
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2709 2024-05-24 00:04:39.319449 ollama_chat-0.9.3/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1851 2024-05-23 21:31:11.000000 ollama_chat-0.9.3/README.md
+-rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-05-02 18:06:38.000000 ollama_chat-0.9.3/pyproject.toml
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1039 2024-05-24 00:04:39.319765 ollama_chat-0.9.3/setup.cfg
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-24 00:04:39.316873 ollama_chat-0.9.3/src/
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-24 00:04:39.318000 ollama_chat-0.9.3/src/ollama_chat/
+-rw-r--r--   0 craighobbs   (501) staff       (20)        0 2024-05-02 18:06:38.000000 ollama_chat-0.9.3/src/ollama_chat/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)      229 2024-05-02 18:06:38.000000 ollama_chat-0.9.3/src/ollama_chat/__main__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     9552 2024-05-23 20:21:45.000000 ollama_chat-0.9.3/src/ollama_chat/app.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2125 2024-05-21 19:56:51.000000 ollama_chat-0.9.3/src/ollama_chat/main.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2659 2024-05-22 20:43:32.000000 ollama_chat-0.9.3/src/ollama_chat/ollama.py
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-24 00:04:39.318982 ollama_chat-0.9.3/src/ollama_chat/static/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3774 2024-05-09 17:20:22.000000 ollama_chat-0.9.3/src/ollama_chat/static/index.html
+-rw-r--r--   0 craighobbs   (501) staff       (20)    17415 2024-05-24 00:00:30.000000 ollama_chat-0.9.3/src/ollama_chat/static/ollamaChat.bare
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3506 2024-05-23 17:06:52.000000 ollama_chat-0.9.3/src/ollama_chat/static/ollamaChat.smd
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-05-24 00:04:39.319135 ollama_chat-0.9.3/src/ollama_chat.egg-info/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     2709 2024-05-24 00:04:39.000000 ollama_chat-0.9.3/src/ollama_chat.egg-info/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)      518 2024-05-24 00:04:39.000000 ollama_chat-0.9.3/src/ollama_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-05-24 00:04:39.000000 ollama_chat-0.9.3/src/ollama_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       54 2024-05-24 00:04:39.000000 ollama_chat-0.9.3/src/ollama_chat.egg-info/entry_points.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       44 2024-05-24 00:04:39.000000 ollama_chat-0.9.3/src/ollama_chat.egg-info/requires.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       12 2024-05-24 00:04:39.000000 ollama_chat-0.9.3/src/ollama_chat.egg-info/top_level.txt
```

### Comparing `ollama_chat-0.9.2/LICENSE` & `ollama_chat-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.2/PKG-INFO` & `ollama_chat-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-chat
-Version: 0.9.2
+Version: 0.9.3
 Summary: ollama-chat
 Home-page: https://github.com/craigahobbs/ollama-chat
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: ollama-chat
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ollama_chat-0.9.2/README.md` & `ollama_chat-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.2/setup.cfg` & `ollama_chat-0.9.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ollama-chat
-version = 0.9.2
+version = 0.9.3
 url = https://github.com/craigahobbs/ollama-chat
 author = Craig A. Hobbs
 author_email = craigahobbs@gmail.com
 license = MIT
 description = ollama-chat
 long_description = file:README.md
 long_description_content_type = text/markdown
```

### Comparing `ollama_chat-0.9.2/src/ollama_chat/app.py` & `ollama_chat-0.9.3/src/ollama_chat/app.py`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.2/src/ollama_chat/main.py` & `ollama_chat-0.9.3/src/ollama_chat/main.py`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.2/src/ollama_chat/ollama.py` & `ollama_chat-0.9.3/src/ollama_chat/ollama.py`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.2/src/ollama_chat/static/index.html` & `ollama_chat-0.9.3/src/ollama_chat/static/index.html`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.2/src/ollama_chat/static/ollamaChat.bare` & `ollama_chat-0.9.3/src/ollama_chat/static/ollamaChat.bare`

 * *Files 0% similar despite different names*

```diff
@@ -379,30 +379,32 @@
                 'padding: 10px', \
                 'position: fixed', \
                 'top: 10px' \
             ), '; ') \
         ), \
         'elem', arrayNew( \
             formsLinkElements('Back', argsURL(ollamaChatArguments, null, true)), \
-            objectNew('text', separator), \
-            formsLinkElements('Top', argsURL(ollamaChatArguments, null, false, '_top')), \
-            objectNew('text', separator), \
-            formsLinkElements('Bottom', argsURL(ollamaChatArguments, null, false, ollamaChatBottomID)) \
+            if(!generating, arrayNew( \
+                objectNew('text', separator), \
+                formsLinkElements('Top', argsURL(ollamaChatArguments, null, false, '_top')), \
+                objectNew('text', separator), \
+                formsLinkElements('Bottom', argsURL(ollamaChatArguments, null, false, ollamaChatBottomID)) \
+            )) \
         ) \
     ))
 
     # The prompt controls
     arrayPush(elements, objectNew( \
         'html', 'div', \
         'attr', objectNew( \
             'style', arrayJoin(arrayNew( \
                 'align-items: center', \
                 'background-color: #c0c0c0', \
                 'border-radius: 10px', \
-                'bottom: 10px', \
+                'bottom: 30px', \
                 'display: flex', \
                 'left: 50px', \
                 'padding: 15px', \
                 'position: fixed', \
                 'right: 50px' \
             ), '; ') \
         ), \
@@ -463,15 +465,15 @@
 
 
 # The Ollama chat pages floating controls bottom-of-the-window space div element model
 function ollamaChatPageFloatingBottomElements():
     elements = arrayNew()
 
     # Add the bottom space
-    arrayPush(elements, objectNew('html', 'div', 'attr', objectNew('style', 'height: 80px')))
+    arrayPush(elements, objectNew('html', 'div', 'attr', objectNew('style', 'height: 90px')))
 
     # Add the bottom document ID
     bottomElementId = stringSlice(argsURL(ollamaChatArguments, null, false, ollamaChatBottomID), 1)
     arrayPush(elements, objectNew('html', 'div', 'attr', objectNew('id', bottomElementId)))
 
     return elements
 endfunction
```

### Comparing `ollama_chat-0.9.2/src/ollama_chat/static/ollamaChat.smd` & `ollama_chat-0.9.3/src/ollama_chat/static/ollamaChat.smd`

 * *Files identical despite different names*

### Comparing `ollama_chat-0.9.2/src/ollama_chat.egg-info/PKG-INFO` & `ollama_chat-0.9.3/src/ollama_chat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-chat
-Version: 0.9.2
+Version: 0.9.3
 Summary: ollama-chat
 Home-page: https://github.com/craigahobbs/ollama-chat
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: ollama-chat
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ollama_chat-0.9.2/src/ollama_chat.egg-info/SOURCES.txt` & `ollama_chat-0.9.3/src/ollama_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

