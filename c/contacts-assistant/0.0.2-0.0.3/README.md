# Comparing `tmp/contacts_assistant-0.0.2.tar.gz` & `tmp/contacts_assistant-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contacts_assistant-0.0.2.tar", last modified: Fri May 24 15:15:05 2024, max compression
+gzip compressed data, was "contacts_assistant-0.0.3.tar", last modified: Fri May 24 16:52:15 2024, max compression
```

## Comparing `contacts_assistant-0.0.2.tar` & `contacts_assistant-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 15:15:05.386419 contacts_assistant-0.0.2/
--rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4080 2024-05-24 15:15:05.385420 contacts_assistant-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3313 2024-05-24 13:50:38.000000 contacts_assistant-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 15:15:05.378420 contacts_assistant-0.0.2/contacts_assistant/
--rw-rw-rw-   0        0        0     1330 2024-05-24 14:13:23.000000 contacts_assistant-0.0.2/contacts_assistant/Birthday.py
--rw-rw-rw-   0        0        0     1217 2024-05-24 07:04:24.000000 contacts_assistant-0.0.2/contacts_assistant/Email.py
--rw-rw-rw-   0        0        0      853 2024-05-22 16:29:48.000000 contacts_assistant-0.0.2/contacts_assistant/Field.py
--rw-rw-rw-   0        0        0      591 2024-05-22 16:29:48.000000 contacts_assistant-0.0.2/contacts_assistant/Name.py
--rw-rw-rw-   0        0        0     1504 2024-05-22 16:29:48.000000 contacts_assistant-0.0.2/contacts_assistant/Phone.py
--rw-rw-rw-   0        0        0     6498 2024-05-24 07:04:24.000000 contacts_assistant-0.0.2/contacts_assistant/Record.py
--rw-rw-rw-   0        0        0        0 2024-05-24 13:51:21.000000 contacts_assistant-0.0.2/contacts_assistant/__init__.py
--rw-rw-rw-   0        0        0     2248 2024-05-24 09:53:13.000000 contacts_assistant-0.0.2/contacts_assistant/__main__.py
--rw-rw-rw-   0        0        0     2140 2024-05-24 08:47:43.000000 contacts_assistant-0.0.2/contacts_assistant/address.py
--rw-rw-rw-   0        0        0     1201 2024-05-24 07:04:24.000000 contacts_assistant-0.0.2/contacts_assistant/command_completer.py
--rw-rw-rw-   0        0        0      834 2024-05-24 11:34:46.000000 contacts_assistant-0.0.2/contacts_assistant/constants.py
--rw-rw-rw-   0        0        0     8535 2024-05-24 11:34:46.000000 contacts_assistant-0.0.2/contacts_assistant/contactsBook.py
--rw-rw-rw-   0        0        0     1983 2024-05-24 06:37:57.000000 contacts_assistant-0.0.2/contacts_assistant/datehelper.py
--rw-rw-rw-   0        0        0    16904 2024-05-24 11:34:46.000000 contacts_assistant-0.0.2/contacts_assistant/handler.py
--rw-rw-rw-   0        0        0     6995 2024-05-24 11:34:46.000000 contacts_assistant-0.0.2/contacts_assistant/menu.py
--rw-rw-rw-   0        0        0     3280 2024-05-24 06:37:57.000000 contacts_assistant-0.0.2/contacts_assistant/note.py
--rw-rw-rw-   0        0        0     8394 2024-05-24 06:37:57.000000 contacts_assistant-0.0.2/contacts_assistant/notebook.py
--rw-rw-rw-   0        0        0      549 2024-05-22 16:32:08.000000 contacts_assistant-0.0.2/contacts_assistant/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:15:05.385420 contacts_assistant-0.0.2/contacts_assistant.egg-info/
--rw-rw-rw-   0        0        0     4080 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 15:15:05.386419 contacts_assistant-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1555 2024-05-24 15:05:05.000000 contacts_assistant-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:52:15.691677 contacts_assistant-0.0.3/
+-rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4080 2024-05-24 16:52:15.689675 contacts_assistant-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3313 2024-05-24 13:50:38.000000 contacts_assistant-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 16:52:15.650607 contacts_assistant-0.0.3/contacts_assistant/
+-rw-rw-rw-   0        0        0     1330 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/Birthday.py
+-rw-rw-rw-   0        0        0     1217 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/Email.py
+-rw-rw-rw-   0        0        0      853 2024-05-22 16:29:48.000000 contacts_assistant-0.0.3/contacts_assistant/Field.py
+-rw-rw-rw-   0        0        0      591 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/Name.py
+-rw-rw-rw-   0        0        0     1504 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/Phone.py
+-rw-rw-rw-   0        0        0     6498 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/Record.py
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:51:21.000000 contacts_assistant-0.0.3/contacts_assistant/__init__.py
+-rw-rw-rw-   0        0        0     2248 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/__main__.py
+-rw-rw-rw-   0        0        0     2140 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/address.py
+-rw-rw-rw-   0        0        0     1199 2024-05-24 16:46:36.000000 contacts_assistant-0.0.3/contacts_assistant/command_completer.py
+-rw-rw-rw-   0        0        0      834 2024-05-24 11:34:46.000000 contacts_assistant-0.0.3/contacts_assistant/constants.py
+-rw-rw-rw-   0        0        0     8535 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/contactsBook.py
+-rw-rw-rw-   0        0        0     1983 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/datehelper.py
+-rw-rw-rw-   0        0        0    16904 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/handler.py
+-rw-rw-rw-   0        0        0     6995 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/menu.py
+-rw-rw-rw-   0        0        0     3280 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/note.py
+-rw-rw-rw-   0        0        0     8394 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/notebook.py
+-rw-rw-rw-   0        0        0      549 2024-05-22 16:32:08.000000 contacts_assistant-0.0.3/contacts_assistant/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:52:15.688677 contacts_assistant-0.0.3/contacts_assistant.egg-info/
+-rw-rw-rw-   0        0        0     4080 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 16:52:15.691677 contacts_assistant-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1536 2024-05-24 16:51:47.000000 contacts_assistant-0.0.3/setup.py
```

### Comparing `contacts_assistant-0.0.2/LICENSE` & `contacts_assistant-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/PKG-INFO` & `contacts_assistant-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.2
+Version: 0.0.3
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samiolenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `contacts_assistant-0.0.2/README.md` & `contacts_assistant-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/Birthday.py` & `contacts_assistant-0.0.3/contacts_assistant/Birthday.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/Email.py` & `contacts_assistant-0.0.3/contacts_assistant/Email.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/Field.py` & `contacts_assistant-0.0.3/contacts_assistant/Field.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/Name.py` & `contacts_assistant-0.0.3/contacts_assistant/Name.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/Phone.py` & `contacts_assistant-0.0.3/contacts_assistant/Phone.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/Record.py` & `contacts_assistant-0.0.3/contacts_assistant/Record.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/__main__.py` & `contacts_assistant-0.0.3/contacts_assistant/__main__.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/address.py` & `contacts_assistant-0.0.3/contacts_assistant/address.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/command_completer.py` & `contacts_assistant-0.0.3/contacts_assistant/command_completer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from prompt_toolkit.completion import Completer, Completion
 
-
 class CommandCompleter(Completer):
     def __init__(self, command_args, book):
         super().__init__()
         self.command_args = command_args
         self.book = book
 
     def get_completions(self, document, complete_event):
```

### Comparing `contacts_assistant-0.0.2/contacts_assistant/constants.py` & `contacts_assistant-0.0.3/contacts_assistant/constants.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/contactsBook.py` & `contacts_assistant-0.0.3/contacts_assistant/contactsBook.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/datehelper.py` & `contacts_assistant-0.0.3/contacts_assistant/datehelper.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/handler.py` & `contacts_assistant-0.0.3/contacts_assistant/handler.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/menu.py` & `contacts_assistant-0.0.3/contacts_assistant/menu.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/note.py` & `contacts_assistant-0.0.3/contacts_assistant/note.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/notebook.py` & `contacts_assistant-0.0.3/contacts_assistant/notebook.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant/utils.py` & `contacts_assistant-0.0.3/contacts_assistant/utils.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/contacts_assistant.egg-info/PKG-INFO` & `contacts_assistant-0.0.3/contacts_assistant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.2
+Version: 0.0.3
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samiolenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `contacts_assistant-0.0.2/contacts_assistant.egg-info/SOURCES.txt` & `contacts_assistant-0.0.3/contacts_assistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.2/setup.py` & `contacts_assistant-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     encoding = result['encoding']
 
 with open("requirements.txt", "r", encoding=encoding) as fh:
     requirements = fh.read().splitlines()
 
 setuptools.setup(
     name="contacts_assistant",
-    version="0.0.2",
+    version="0.0.3",
     author="Mykyta Samiolenko",
     author_email="inikita546@gmail.com",
     description="Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bignichok/Python-ContactsAssistant",
     packages=setuptools.find_packages(),
@@ -34,11 +34,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     entry_points={
         'console_scripts': [
-            'contacts-assistant=contacts_assistant.__main__:main'
+            'contacts-assistant=__main__:main'
         ]
     }
 )
```

