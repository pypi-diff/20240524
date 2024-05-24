# Comparing `tmp/goit-phone-book-bot-0.0.2.tar.gz` & `tmp/goit-phone-book-bot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goit-phone-book-bot-0.0.2.tar", last modified: Fri May 24 11:43:05 2024, max compression
+gzip compressed data, was "goit-phone-book-bot-0.0.3.tar", last modified: Fri May 24 12:02:12 2024, max compression
```

## Comparing `goit-phone-book-bot-0.0.2.tar` & `goit-phone-book-bot-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 11:43:05.410385 goit-phone-book-bot-0.0.2/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit-phone-book-bot-0.0.2/LICENSE
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 11:43:05.410256 goit-phone-book-bot-0.0.2/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-23 10:25:17.000000 goit-phone-book-bot-0.0.2/README.md
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 11:43:05.409828 goit-phone-book-bot-0.0.2/goit_phone_book_bot.egg-info/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 11:43:05.000000 goit-phone-book-bot-0.0.2/goit_phone_book_bot.egg-info/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      314 2024-05-24 11:43:05.000000 goit-phone-book-bot-0.0.2/goit_phone_book_bot.egg-info/SOURCES.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-24 11:43:05.000000 goit-phone-book-bot-0.0.2/goit_phone_book_bot.egg-info/dependency_links.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       52 2024-05-24 11:43:05.000000 goit-phone-book-bot-0.0.2/goit_phone_book_bot.egg-info/entry_points.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-24 11:43:05.000000 goit-phone-book-bot-0.0.2/goit_phone_book_bot.egg-info/requires.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-24 11:43:05.000000 goit-phone-book-bot-0.0.2/goit_phone_book_bot.egg-info/top_level.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-24 11:43:05.410433 goit-phone-book-bot-0.0.2/setup.cfg
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      819 2024-05-24 11:42:06.000000 goit-phone-book-bot-0.0.2/setup.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 11:43:05.410055 goit-phone-book-bot-0.0.2/src/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       55 2024-05-24 11:27:09.000000 goit-phone-book-bot-0.0.2/src/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     5461 2024-05-24 08:05:45.000000 goit-phone-book-bot-0.0.2/src/main.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:02:12.842395 goit-phone-book-bot-0.0.3/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit-phone-book-bot-0.0.3/LICENSE
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 12:02:12.842275 goit-phone-book-bot-0.0.3/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-23 10:25:17.000000 goit-phone-book-bot-0.0.3/README.md
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:02:12.841689 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      314 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       45 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/entry_points.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/requires.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/top_level.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-24 12:02:12.842444 goit-phone-book-bot-0.0.3/setup.cfg
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      812 2024-05-24 12:01:50.000000 goit-phone-book-bot-0.0.3/setup.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:02:12.841994 goit-phone-book-bot-0.0.3/src/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       55 2024-05-24 11:27:09.000000 goit-phone-book-bot-0.0.3/src/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     5461 2024-05-24 08:05:45.000000 goit-phone-book-bot-0.0.3/src/main.py
```

### Comparing `goit-phone-book-bot-0.0.2/LICENSE` & `goit-phone-book-bot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `goit-phone-book-bot-0.0.2/PKG-INFO` & `goit-phone-book-bot-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `goit-phone-book-bot-0.0.2/goit_phone_book_bot.egg-info/PKG-INFO` & `goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.0.2
+Version: 0.0.3
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `goit-phone-book-bot-0.0.2/setup.py` & `goit-phone-book-bot-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='goit-phone-book-bot',
-    version='0.0.2',
+    version='0.0.3',
     author='Vasyl Martyniv',
     author_email='doc.people97@gmail.com',
     description='Phone Book bot developed by team #5 - CREATORS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VasylMartyniv/GoIT_Phone_Book_bot',
     packages=find_packages(),
@@ -18,11 +18,11 @@
     python_requires='>=3.6',
     install_requires=[
         'pyreadline3',
         'tabulate',
     ],
     entry_points={
         'console_scripts': [
-            'start_bot=my_package.main:main',
+            'start_bot=src.main:main',
         ],
     },
 )
```

### Comparing `goit-phone-book-bot-0.0.2/src/main.py` & `goit-phone-book-bot-0.0.3/src/main.py`

 * *Files identical despite different names*

