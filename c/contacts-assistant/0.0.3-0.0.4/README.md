# Comparing `tmp/contacts_assistant-0.0.3.tar.gz` & `tmp/contacts_assistant-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contacts_assistant-0.0.3.tar", last modified: Fri May 24 16:52:15 2024, max compression
+gzip compressed data, was "contacts_assistant-0.0.4.tar", last modified: Fri May 24 20:36:30 2024, max compression
```

## Comparing `contacts_assistant-0.0.3.tar` & `contacts_assistant-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 16:52:15.691677 contacts_assistant-0.0.3/
--rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4080 2024-05-24 16:52:15.689675 contacts_assistant-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3313 2024-05-24 13:50:38.000000 contacts_assistant-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 16:52:15.650607 contacts_assistant-0.0.3/contacts_assistant/
--rw-rw-rw-   0        0        0     1330 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/Birthday.py
--rw-rw-rw-   0        0        0     1217 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/Email.py
--rw-rw-rw-   0        0        0      853 2024-05-22 16:29:48.000000 contacts_assistant-0.0.3/contacts_assistant/Field.py
--rw-rw-rw-   0        0        0      591 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/Name.py
--rw-rw-rw-   0        0        0     1504 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/Phone.py
--rw-rw-rw-   0        0        0     6498 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/Record.py
--rw-rw-rw-   0        0        0        0 2024-05-24 13:51:21.000000 contacts_assistant-0.0.3/contacts_assistant/__init__.py
--rw-rw-rw-   0        0        0     2248 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/__main__.py
--rw-rw-rw-   0        0        0     2140 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/address.py
--rw-rw-rw-   0        0        0     1199 2024-05-24 16:46:36.000000 contacts_assistant-0.0.3/contacts_assistant/command_completer.py
--rw-rw-rw-   0        0        0      834 2024-05-24 11:34:46.000000 contacts_assistant-0.0.3/contacts_assistant/constants.py
--rw-rw-rw-   0        0        0     8535 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/contactsBook.py
--rw-rw-rw-   0        0        0     1983 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/datehelper.py
--rw-rw-rw-   0        0        0    16904 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/handler.py
--rw-rw-rw-   0        0        0     6995 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/menu.py
--rw-rw-rw-   0        0        0     3280 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/note.py
--rw-rw-rw-   0        0        0     8394 2024-05-24 16:50:28.000000 contacts_assistant-0.0.3/contacts_assistant/notebook.py
--rw-rw-rw-   0        0        0      549 2024-05-22 16:32:08.000000 contacts_assistant-0.0.3/contacts_assistant/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-24 16:52:15.688677 contacts_assistant-0.0.3/contacts_assistant.egg-info/
--rw-rw-rw-   0        0        0     4080 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      826 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-24 16:52:15.000000 contacts_assistant-0.0.3/contacts_assistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 16:52:15.691677 contacts_assistant-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1536 2024-05-24 16:51:47.000000 contacts_assistant-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:36:30.054384 contacts_assistant-0.0.4/
+-rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4080 2024-05-24 20:36:30.053385 contacts_assistant-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3313 2024-05-24 13:50:38.000000 contacts_assistant-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 20:36:30.052384 contacts_assistant-0.0.4/contacts_assistant.egg-info/
+-rw-rw-rw-   0        0        0     4080 2024-05-24 20:36:29.000000 contacts_assistant-0.0.4/contacts_assistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2024-05-24 20:36:29.000000 contacts_assistant-0.0.4/contacts_assistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 20:36:29.000000 contacts_assistant-0.0.4/contacts_assistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-24 20:36:29.000000 contacts_assistant-0.0.4/contacts_assistant.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-05-24 20:36:29.000000 contacts_assistant-0.0.4/contacts_assistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-24 20:36:29.000000 contacts_assistant-0.0.4/contacts_assistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 20:36:30.054384 contacts_assistant-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1536 2024-05-24 20:36:23.000000 contacts_assistant-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:36:30.043384 contacts_assistant-0.0.4/src/
+-rw-rw-rw-   0        0        0        0 2024-05-24 20:35:08.000000 contacts_assistant-0.0.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:36:30.052384 contacts_assistant-0.0.4/src/contacts_assistant/
+-rw-rw-rw-   0        0        0     1330 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/Birthday.py
+-rw-rw-rw-   0        0        0     1217 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/Email.py
+-rw-rw-rw-   0        0        0      853 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/Field.py
+-rw-rw-rw-   0        0        0      591 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/Name.py
+-rw-rw-rw-   0        0        0     1504 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/Phone.py
+-rw-rw-rw-   0        0        0     6498 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/Record.py
+-rw-rw-rw-   0        0        0        0 2024-05-24 20:13:39.000000 contacts_assistant-0.0.4/src/contacts_assistant/__init__.py
+-rw-rw-rw-   0        0        0     2248 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/__main__.py
+-rw-rw-rw-   0        0        0     2140 2024-05-24 20:18:37.000000 contacts_assistant-0.0.4/src/contacts_assistant/address.py
+-rw-rw-rw-   0        0        0     1201 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/command_completer.py
+-rw-rw-rw-   0        0        0      834 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/constants.py
+-rw-rw-rw-   0        0        0     8535 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/contactsBook.py
+-rw-rw-rw-   0        0        0     1983 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/datehelper.py
+-rw-rw-rw-   0        0        0    16904 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/handler.py
+-rw-rw-rw-   0        0        0     6995 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/menu.py
+-rw-rw-rw-   0        0        0     3280 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/note.py
+-rw-rw-rw-   0        0        0     8394 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/notebook.py
+-rw-rw-rw-   0        0        0      549 2024-05-24 20:10:40.000000 contacts_assistant-0.0.4/src/contacts_assistant/utils.py
```

### Comparing `contacts_assistant-0.0.3/LICENSE` & `contacts_assistant-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/PKG-INFO` & `contacts_assistant-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.3
+Version: 0.0.4
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samiolenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `contacts_assistant-0.0.3/README.md` & `contacts_assistant-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/Birthday.py` & `contacts_assistant-0.0.4/src/contacts_assistant/Birthday.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/Email.py` & `contacts_assistant-0.0.4/src/contacts_assistant/Email.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/Field.py` & `contacts_assistant-0.0.4/src/contacts_assistant/Field.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/Name.py` & `contacts_assistant-0.0.4/src/contacts_assistant/Name.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/Phone.py` & `contacts_assistant-0.0.4/src/contacts_assistant/Phone.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/Record.py` & `contacts_assistant-0.0.4/src/contacts_assistant/Record.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/__main__.py` & `contacts_assistant-0.0.4/src/contacts_assistant/__main__.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/address.py` & `contacts_assistant-0.0.4/src/contacts_assistant/address.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/command_completer.py` & `contacts_assistant-0.0.4/src/contacts_assistant/command_completer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from prompt_toolkit.completion import Completer, Completion
 
+
 class CommandCompleter(Completer):
     def __init__(self, command_args, book):
         super().__init__()
         self.command_args = command_args
         self.book = book
 
     def get_completions(self, document, complete_event):
```

### Comparing `contacts_assistant-0.0.3/contacts_assistant/constants.py` & `contacts_assistant-0.0.4/src/contacts_assistant/constants.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/contactsBook.py` & `contacts_assistant-0.0.4/src/contacts_assistant/contactsBook.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/datehelper.py` & `contacts_assistant-0.0.4/src/contacts_assistant/datehelper.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/handler.py` & `contacts_assistant-0.0.4/src/contacts_assistant/handler.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/menu.py` & `contacts_assistant-0.0.4/src/contacts_assistant/menu.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/note.py` & `contacts_assistant-0.0.4/src/contacts_assistant/note.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/notebook.py` & `contacts_assistant-0.0.4/src/contacts_assistant/notebook.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant/utils.py` & `contacts_assistant-0.0.4/src/contacts_assistant/utils.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.3/contacts_assistant.egg-info/PKG-INFO` & `contacts_assistant-0.0.4/contacts_assistant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.3
+Version: 0.0.4
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samiolenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `contacts_assistant-0.0.3/contacts_assistant.egg-info/SOURCES.txt` & `contacts_assistant-0.0.4/contacts_assistant.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 LICENSE
 README.md
 setup.py
-contacts_assistant/Birthday.py
-contacts_assistant/Email.py
-contacts_assistant/Field.py
-contacts_assistant/Name.py
-contacts_assistant/Phone.py
-contacts_assistant/Record.py
-contacts_assistant/__init__.py
-contacts_assistant/__main__.py
-contacts_assistant/address.py
-contacts_assistant/command_completer.py
-contacts_assistant/constants.py
-contacts_assistant/contactsBook.py
-contacts_assistant/datehelper.py
-contacts_assistant/handler.py
-contacts_assistant/menu.py
-contacts_assistant/note.py
-contacts_assistant/notebook.py
-contacts_assistant/utils.py
 contacts_assistant.egg-info/PKG-INFO
 contacts_assistant.egg-info/SOURCES.txt
 contacts_assistant.egg-info/dependency_links.txt
 contacts_assistant.egg-info/entry_points.txt
 contacts_assistant.egg-info/requires.txt
-contacts_assistant.egg-info/top_level.txt
+contacts_assistant.egg-info/top_level.txt
+src/__init__.py
+src/contacts_assistant/Birthday.py
+src/contacts_assistant/Email.py
+src/contacts_assistant/Field.py
+src/contacts_assistant/Name.py
+src/contacts_assistant/Phone.py
+src/contacts_assistant/Record.py
+src/contacts_assistant/__init__.py
+src/contacts_assistant/__main__.py
+src/contacts_assistant/address.py
+src/contacts_assistant/command_completer.py
+src/contacts_assistant/constants.py
+src/contacts_assistant/contactsBook.py
+src/contacts_assistant/datehelper.py
+src/contacts_assistant/handler.py
+src/contacts_assistant/menu.py
+src/contacts_assistant/note.py
+src/contacts_assistant/notebook.py
+src/contacts_assistant/utils.py
```

### Comparing `contacts_assistant-0.0.3/setup.py` & `contacts_assistant-0.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     encoding = result['encoding']
 
 with open("requirements.txt", "r", encoding=encoding) as fh:
     requirements = fh.read().splitlines()
 
 setuptools.setup(
     name="contacts_assistant",
-    version="0.0.3",
+    version="0.0.4",
     author="Mykyta Samiolenko",
     author_email="inikita546@gmail.com",
     description="Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bignichok/Python-ContactsAssistant",
     packages=setuptools.find_packages(),
```

