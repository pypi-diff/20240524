# Comparing `tmp/goit-phone-book-bot-0.0.4.tar.gz` & `tmp/goit-phone-book-bot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goit-phone-book-bot-0.0.4.tar", last modified: Fri May 24 12:07:42 2024, max compression
+gzip compressed data, was "goit-phone-book-bot-0.0.5.tar", last modified: Fri May 24 15:47:26 2024, max compression
```

## Comparing `goit-phone-book-bot-0.0.4.tar` & `goit-phone-book-bot-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,33 @@
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:07:42.393097 goit-phone-book-bot-0.0.4/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit-phone-book-bot-0.0.4/LICENSE
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 12:07:42.392959 goit-phone-book-bot-0.0.4/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-23 10:25:17.000000 goit-phone-book-bot-0.0.4/README.md
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:07:42.392180 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      314 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/SOURCES.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/dependency_links.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       45 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/entry_points.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/requires.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/top_level.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-24 12:07:42.393156 goit-phone-book-bot-0.0.4/setup.cfg
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      812 2024-05-24 12:06:57.000000 goit-phone-book-bot-0.0.4/setup.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:07:42.392654 goit-phone-book-bot-0.0.4/src/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       55 2024-05-24 11:27:09.000000 goit-phone-book-bot-0.0.4/src/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4715 2024-05-24 12:06:18.000000 goit-phone-book-bot-0.0.4/src/main.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:47:26.374111 goit-phone-book-bot-0.0.5/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit-phone-book-bot-0.0.5/LICENSE
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 15:47:26.373987 goit-phone-book-bot-0.0.5/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-23 10:25:17.000000 goit-phone-book-bot-0.0.5/README.md
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:47:26.372057 goit-phone-book-bot-0.0.5/goit_phone_book_bot.egg-info/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 15:47:26.000000 goit-phone-book-bot-0.0.5/goit_phone_book_bot.egg-info/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      634 2024-05-24 15:47:26.000000 goit-phone-book-bot-0.0.5/goit_phone_book_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-24 15:47:26.000000 goit-phone-book-bot-0.0.5/goit_phone_book_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       45 2024-05-24 15:47:26.000000 goit-phone-book-bot-0.0.5/goit_phone_book_bot.egg-info/entry_points.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-24 15:47:26.000000 goit-phone-book-bot-0.0.5/goit_phone_book_bot.egg-info/requires.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-24 15:47:26.000000 goit-phone-book-bot-0.0.5/goit_phone_book_bot.egg-info/top_level.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-24 15:47:26.374163 goit-phone-book-bot-0.0.5/setup.cfg
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      812 2024-05-24 15:47:10.000000 goit-phone-book-bot-0.0.5/setup.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:47:26.372407 goit-phone-book-bot-0.0.5/src/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       55 2024-05-24 11:27:09.000000 goit-phone-book-bot-0.0.5/src/__init__.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:47:26.373435 goit-phone-book-bot-0.0.5/src/classes/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:46:43.000000 goit-phone-book-bot-0.0.5/src/classes/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 17:28:11.000000 goit-phone-book-bot-0.0.5/src/classes/address_book.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:06:18.000000 goit-phone-book-bot-0.0.5/src/classes/birthday.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 17:29:59.000000 goit-phone-book-bot-0.0.5/src/classes/email.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      126 2024-05-23 18:06:25.000000 goit-phone-book-bot-0.0.5/src/classes/field.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 19:15:04.000000 goit-phone-book-bot-0.0.5/src/classes/misc.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      251 2024-05-23 17:44:13.000000 goit-phone-book-bot-0.0.5/src/classes/note.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     2936 2024-05-23 17:54:38.000000 goit-phone-book-bot-0.0.5/src/classes/notes_book.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 17:28:25.000000 goit-phone-book-bot-0.0.5/src/classes/phone.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:06:18.000000 goit-phone-book-bot-0.0.5/src/classes/record.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:47:26.373615 goit-phone-book-bot-0.0.5/src/constants/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:46:43.000000 goit-phone-book-bot-0.0.5/src/constants/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1178 2024-05-23 17:42:37.000000 goit-phone-book-bot-0.0.5/src/constants/commands.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4751 2024-05-24 12:11:28.000000 goit-phone-book-bot-0.0.5/src/main.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:47:26.373823 goit-phone-book-bot-0.0.5/src/utils/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:46:43.000000 goit-phone-book-bot-0.0.5/src/utils/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1304 2024-05-24 12:10:41.000000 goit-phone-book-bot-0.0.5/src/utils/utils.py
```

### Comparing `goit-phone-book-bot-0.0.4/LICENSE` & `goit-phone-book-bot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `goit-phone-book-bot-0.0.4/PKG-INFO` & `goit-phone-book-bot-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/PKG-INFO` & `goit-phone-book-bot-0.0.5/goit_phone_book_bot.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `goit-phone-book-bot-0.0.4/setup.py` & `goit-phone-book-bot-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='goit-phone-book-bot',
-    version='0.0.4',
+    version='0.0.5',
     author='Vasyl Martyniv',
     author_email='doc.people97@gmail.com',
     description='Phone Book bot developed by team #5 - CREATORS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VasylMartyniv/GoIT_Phone_Book_bot',
     packages=find_packages(),
```

### Comparing `goit-phone-book-bot-0.0.4/src/main.py` & `goit-phone-book-bot-0.0.5/src/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import readline
 
-from src.classes.notes_book import NotesBook
-from src.utils.utils import *
+from classes.notes_book import NotesBook
+from src.constants.commands import commands
+from utils.utils import *
 
 
 # Функція для автодоповнення команд
 def completer(text, state):
     options = [cmd for cmd in commands.keys() if cmd.startswith(text)]
     if state < len(options):
         return options[state]
```

