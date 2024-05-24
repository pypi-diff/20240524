# Comparing `tmp/goit-phone-book-bot-0.0.3.tar.gz` & `tmp/goit-phone-book-bot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goit-phone-book-bot-0.0.3.tar", last modified: Fri May 24 12:02:12 2024, max compression
+gzip compressed data, was "goit-phone-book-bot-0.0.4.tar", last modified: Fri May 24 12:07:42 2024, max compression
```

## Comparing `goit-phone-book-bot-0.0.3.tar` & `goit-phone-book-bot-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:02:12.842395 goit-phone-book-bot-0.0.3/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit-phone-book-bot-0.0.3/LICENSE
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 12:02:12.842275 goit-phone-book-bot-0.0.3/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-23 10:25:17.000000 goit-phone-book-bot-0.0.3/README.md
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:02:12.841689 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/PKG-INFO
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      314 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/SOURCES.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/dependency_links.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       45 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/entry_points.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/requires.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-24 12:02:12.000000 goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/top_level.txt
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-24 12:02:12.842444 goit-phone-book-bot-0.0.3/setup.cfg
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)      812 2024-05-24 12:01:50.000000 goit-phone-book-bot-0.0.3/setup.py
-drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:02:12.841994 goit-phone-book-bot-0.0.3/src/
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)       55 2024-05-24 11:27:09.000000 goit-phone-book-bot-0.0.3/src/__init__.py
--rw-r--r--   0 vasylmartyniv   (501) staff       (20)     5461 2024-05-24 08:05:45.000000 goit-phone-book-bot-0.0.3/src/main.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:07:42.393097 goit-phone-book-bot-0.0.4/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     1070 2024-05-23 18:00:36.000000 goit-phone-book-bot-0.0.4/LICENSE
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 12:07:42.392959 goit-phone-book-bot-0.0.4/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      214 2024-05-23 10:25:17.000000 goit-phone-book-bot-0.0.4/README.md
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:07:42.392180 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      726 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/PKG-INFO
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      314 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        1 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       45 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/entry_points.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       21 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/requires.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)        4 2024-05-24 12:07:42.000000 goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/top_level.txt
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       38 2024-05-24 12:07:42.393156 goit-phone-book-bot-0.0.4/setup.cfg
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)      812 2024-05-24 12:06:57.000000 goit-phone-book-bot-0.0.4/setup.py
+drwxr-xr-x   0 vasylmartyniv   (501) staff       (20)        0 2024-05-24 12:07:42.392654 goit-phone-book-bot-0.0.4/src/
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)       55 2024-05-24 11:27:09.000000 goit-phone-book-bot-0.0.4/src/__init__.py
+-rw-r--r--   0 vasylmartyniv   (501) staff       (20)     4715 2024-05-24 12:06:18.000000 goit-phone-book-bot-0.0.4/src/main.py
```

### Comparing `goit-phone-book-bot-0.0.3/LICENSE` & `goit-phone-book-bot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goit-phone-book-bot-0.0.3/PKG-INFO` & `goit-phone-book-bot-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `goit-phone-book-bot-0.0.3/goit_phone_book_bot.egg-info/PKG-INFO` & `goit-phone-book-bot-0.0.4/goit_phone_book_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goit-phone-book-bot
-Version: 0.0.3
+Version: 0.0.4
 Summary: Phone Book bot developed by team #5 - CREATORS
 Home-page: https://github.com/VasylMartyniv/GoIT_Phone_Book_bot
 Author: Vasyl Martyniv
 Author-email: doc.people97@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `goit-phone-book-bot-0.0.3/setup.py` & `goit-phone-book-bot-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='goit-phone-book-bot',
-    version='0.0.3',
+    version='0.0.4',
     author='Vasyl Martyniv',
     author_email='doc.people97@gmail.com',
     description='Phone Book bot developed by team #5 - CREATORS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VasylMartyniv/GoIT_Phone_Book_bot',
     packages=find_packages(),
```

### Comparing `goit-phone-book-bot-0.0.3/src/main.py` & `goit-phone-book-bot-0.0.4/src/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import readline
 
 from src.classes.notes_book import NotesBook
 from src.utils.utils import *
-from src.classes.birthday import add_birthday, show_birthday, show_all_birthdays, search_by_date_birthday
 
 
 # Функція для автодоповнення команд
 def completer(text, state):
     options = [cmd for cmd in commands.keys() if cmd.startswith(text)]
     if state < len(options):
         return options[state]
@@ -62,38 +61,25 @@
         elif command == "all_contact":
             all_contact()
 
         elif command == "delete_contact":
             delete_contact()
 
         elif command == "add_birthday":
-            name = input("Enter name: ")
-            birthday = input("Enter birthday (DD.MM.YYYY): ")
-            print(add_birthday([name, birthday], book))
+            add_birthday()
 
         elif command == "show_birthday":
-            name = input("Enter name: ")
-            print(show_birthday([name], book))
+            show_birthday()
 
         elif command == "show_all_birthdays":
-            print(show_all_birthdays(book))
+            show_all_birthdays()
 
         elif command == "search_by_date_birthday":
-            date = input("Enter date (DD.MM.YYYY): ")
-            print(search_by_date_birthday([date], book))
+            search_by_date_birthday()
 
-        elif command == "change_birthday":
-            name = input("Enter name: ")
-            new_birthday = input("Enter new birthday (DD.MM.YYYY): ")
-            print(change_birthday([name, new_birthday], book))
-
-        elif command == "delete_birthday":
-            name = input("Enter name: ")
-            print(delete_birthday([name], book))
-            
         elif command == "add_note":
             text = input("Enter note text: ")
             tags = input("Enter tags separated by comma: ").split(",")
             db.add_note(text, tags)
             print("Note added.")
             all_notes = (
                 db.get_all_notes()
```

