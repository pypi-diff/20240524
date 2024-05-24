# Comparing `tmp/goit-phone-book-bot-0.0.6.tar.gz` & `tmp/goit-phone-book-bot-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goit-phone-book-bot-0.0.6.tar", last modified: Fri May 24 16:06:14 2024, max compression
+gzip compressed data, was "goit-phone-book-bot-0.0.7.tar", last modified: Fri May 24 16:43:09 2024, max compression
```

## Comparing `goit-phone-book-bot-0.0.6.tar` & `goit-phone-book-bot-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:06:14.243149 goit-phone-book-bot-0.0.6/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit-phone-book-bot-0.0.6/LICENSE
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 16:06:14.242887 goit-phone-book-bot-0.0.6/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-23 10:25:17.000000 goit-phone-book-bot-0.0.6/README.md
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:06:14.239266 goit-phone-book-bot-0.0.6/goit_phone_book_bot.egg-info/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 16:06:14.000000 goit-phone-book-bot-0.0.6/goit_phone_book_bot.egg-info/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      634 2024-05-24 16:06:14.000000 goit-phone-book-bot-0.0.6/goit_phone_book_bot.egg-info/SOURCES.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-24 16:06:14.000000 goit-phone-book-bot-0.0.6/goit_phone_book_bot.egg-info/dependency_links.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       55 2024-05-24 16:06:14.000000 goit-phone-book-bot-0.0.6/goit_phone_book_bot.egg-info/entry_points.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-24 16:06:14.000000 goit-phone-book-bot-0.0.6/goit_phone_book_bot.egg-info/requires.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-24 16:06:14.000000 goit-phone-book-bot-0.0.6/goit_phone_book_bot.egg-info/top_level.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-24 16:06:14.243365 goit-phone-book-bot-0.0.6/setup.cfg
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      822 2024-05-24 16:06:06.000000 goit-phone-book-bot-0.0.6/setup.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:06:14.239759 goit-phone-book-bot-0.0.6/src/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       55 2024-05-24 11:27:09.000000 goit-phone-book-bot-0.0.6/src/__init__.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:06:14.241681 goit-phone-book-bot-0.0.6/src/classes/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:46:43.000000 goit-phone-book-bot-0.0.6/src/classes/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 17:28:11.000000 goit-phone-book-bot-0.0.6/src/classes/address_book.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:06:18.000000 goit-phone-book-bot-0.0.6/src/classes/birthday.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 17:29:59.000000 goit-phone-book-bot-0.0.6/src/classes/email.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      126 2024-05-23 18:06:25.000000 goit-phone-book-bot-0.0.6/src/classes/field.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 19:15:04.000000 goit-phone-book-bot-0.0.6/src/classes/misc.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      251 2024-05-23 17:44:13.000000 goit-phone-book-bot-0.0.6/src/classes/note.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     2936 2024-05-23 17:54:38.000000 goit-phone-book-bot-0.0.6/src/classes/notes_book.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 17:28:25.000000 goit-phone-book-bot-0.0.6/src/classes/phone.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:06:18.000000 goit-phone-book-bot-0.0.6/src/classes/record.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:06:14.241911 goit-phone-book-bot-0.0.6/src/constants/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:46:43.000000 goit-phone-book-bot-0.0.6/src/constants/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1178 2024-05-23 17:42:37.000000 goit-phone-book-bot-0.0.6/src/constants/commands.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4755 2024-05-24 16:05:12.000000 goit-phone-book-bot-0.0.6/src/main.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:06:14.242453 goit-phone-book-bot-0.0.6/src/utils/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:46:43.000000 goit-phone-book-bot-0.0.6/src/utils/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1304 2024-05-24 12:10:41.000000 goit-phone-book-bot-0.0.6/src/utils/utils.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:43:09.380225 goit-phone-book-bot-0.0.7/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit-phone-book-bot-0.0.7/LICENSE
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 16:43:09.380104 goit-phone-book-bot-0.0.7/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-23 10:25:17.000000 goit-phone-book-bot-0.0.7/README.md
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:43:09.376964 goit-phone-book-bot-0.0.7/goit_phone_book_bot.egg-info/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 16:43:09.000000 goit-phone-book-bot-0.0.7/goit_phone_book_bot.egg-info/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      634 2024-05-24 16:43:09.000000 goit-phone-book-bot-0.0.7/goit_phone_book_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-24 16:43:09.000000 goit-phone-book-bot-0.0.7/goit_phone_book_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       55 2024-05-24 16:43:09.000000 goit-phone-book-bot-0.0.7/goit_phone_book_bot.egg-info/entry_points.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-24 16:43:09.000000 goit-phone-book-bot-0.0.7/goit_phone_book_bot.egg-info/requires.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-24 16:43:09.000000 goit-phone-book-bot-0.0.7/goit_phone_book_bot.egg-info/top_level.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-24 16:43:09.380268 goit-phone-book-bot-0.0.7/setup.cfg
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      822 2024-05-24 16:40:36.000000 goit-phone-book-bot-0.0.7/setup.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:43:09.377320 goit-phone-book-bot-0.0.7/src/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       93 2024-05-24 16:34:51.000000 goit-phone-book-bot-0.0.7/src/__init__.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:43:09.379176 goit-phone-book-bot-0.0.7/src/classes/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:46:43.000000 goit-phone-book-bot-0.0.7/src/classes/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 17:28:11.000000 goit-phone-book-bot-0.0.7/src/classes/address_book.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:06:18.000000 goit-phone-book-bot-0.0.7/src/classes/birthday.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 17:29:59.000000 goit-phone-book-bot-0.0.7/src/classes/email.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      126 2024-05-23 18:06:25.000000 goit-phone-book-bot-0.0.7/src/classes/field.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 19:15:04.000000 goit-phone-book-bot-0.0.7/src/classes/misc.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      251 2024-05-23 17:44:13.000000 goit-phone-book-bot-0.0.7/src/classes/note.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     2936 2024-05-23 17:54:38.000000 goit-phone-book-bot-0.0.7/src/classes/notes_book.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-23 17:28:25.000000 goit-phone-book-bot-0.0.7/src/classes/phone.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:06:18.000000 goit-phone-book-bot-0.0.7/src/classes/record.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:43:09.379442 goit-phone-book-bot-0.0.7/src/constants/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:46:43.000000 goit-phone-book-bot-0.0.7/src/constants/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1178 2024-05-23 17:42:37.000000 goit-phone-book-bot-0.0.7/src/constants/commands.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4759 2024-05-24 16:16:30.000000 goit-phone-book-bot-0.0.7/src/main.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 16:43:09.379828 goit-phone-book-bot-0.0.7/src/utils/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 15:46:43.000000 goit-phone-book-bot-0.0.7/src/utils/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1304 2024-05-24 12:10:41.000000 goit-phone-book-bot-0.0.7/src/utils/utils.py
```

### Comparing `goit-phone-book-bot-0.0.6/LICENSE` & `goit-phone-book-bot-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `goit-phone-book-bot-0.0.6/PKG-INFO` & `goit-phone-book-bot-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.0.6
+Version: 0.0.7
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `goit-phone-book-bot-0.0.6/goit_phone_book_bot.egg-info/PKG-INFO` & `goit-phone-book-bot-0.0.7/goit_phone_book_bot.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.0.6
+Version: 0.0.7
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `goit-phone-book-bot-0.0.6/goit_phone_book_bot.egg-info/SOURCES.txt` & `goit-phone-book-bot-0.0.7/goit_phone_book_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goit-phone-book-bot-0.0.6/setup.py` & `goit-phone-book-bot-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='goit-phone-book-bot',
-    version='0.0.6',
+    version='0.0.7',
     author='Vasyl Martyniv',
     author_email='doc.people97@gmail.com',
     description='Phone Book bot developed by team #5 - CREATORS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VasylMartyniv/GoIT_Phone_Book_bot',
     packages=find_packages(),
```

### Comparing `goit-phone-book-bot-0.0.6/src/classes/notes_book.py` & `goit-phone-book-bot-0.0.7/src/classes/notes_book.py`

 * *Files identical despite different names*

### Comparing `goit-phone-book-bot-0.0.6/src/constants/commands.py` & `goit-phone-book-bot-0.0.7/src/constants/commands.py`

 * *Files identical despite different names*

### Comparing `goit-phone-book-bot-0.0.6/src/main.py` & `goit-phone-book-bot-0.0.7/src/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import readline
 
-from constants.commands import commands
 from src.classes.notes_book import NotesBook
+from src.constants.commands import commands
 from src.utils.utils import *
 
 
 # Функція для автодоповнення команд
 def completer(text, state):
     options = [cmd for cmd in commands.keys() if cmd.startswith(text)]
     if state < len(options):
```

### Comparing `goit-phone-book-bot-0.0.6/src/utils/utils.py` & `goit-phone-book-bot-0.0.7/src/utils/utils.py`

 * *Files identical despite different names*

