# Comparing `tmp/contacts_assistant-0.0.1.tar.gz` & `tmp/contacts_assistant-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contacts_assistant-0.0.1.tar", last modified: Fri May 24 14:31:15 2024, max compression
+gzip compressed data, was "contacts_assistant-0.0.2.tar", last modified: Fri May 24 15:15:05 2024, max compression
```

## Comparing `contacts_assistant-0.0.1.tar` & `contacts_assistant-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 14:31:15.178914 contacts_assistant-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-24 14:31:15.142903 contacts_assistant-0.0.1/ContactsAssistant/
--rw-rw-rw-   0        0        0     1330 2024-05-24 14:13:23.000000 contacts_assistant-0.0.1/ContactsAssistant/Birthday.py
--rw-rw-rw-   0        0        0     1217 2024-05-24 07:04:24.000000 contacts_assistant-0.0.1/ContactsAssistant/Email.py
--rw-rw-rw-   0        0        0      853 2024-05-22 16:29:48.000000 contacts_assistant-0.0.1/ContactsAssistant/Field.py
--rw-rw-rw-   0        0        0      591 2024-05-22 16:29:48.000000 contacts_assistant-0.0.1/ContactsAssistant/Name.py
--rw-rw-rw-   0        0        0     1504 2024-05-22 16:29:48.000000 contacts_assistant-0.0.1/ContactsAssistant/Phone.py
--rw-rw-rw-   0        0        0     6498 2024-05-24 07:04:24.000000 contacts_assistant-0.0.1/ContactsAssistant/Record.py
--rw-rw-rw-   0        0        0        0 2024-05-24 13:51:21.000000 contacts_assistant-0.0.1/ContactsAssistant/__init__.py
--rw-rw-rw-   0        0        0     2248 2024-05-24 09:53:13.000000 contacts_assistant-0.0.1/ContactsAssistant/__main__.py
--rw-rw-rw-   0        0        0     2140 2024-05-24 08:47:43.000000 contacts_assistant-0.0.1/ContactsAssistant/address.py
--rw-rw-rw-   0        0        0     1201 2024-05-24 07:04:24.000000 contacts_assistant-0.0.1/ContactsAssistant/command_completer.py
--rw-rw-rw-   0        0        0      834 2024-05-24 11:34:46.000000 contacts_assistant-0.0.1/ContactsAssistant/constants.py
--rw-rw-rw-   0        0        0     8535 2024-05-24 11:34:46.000000 contacts_assistant-0.0.1/ContactsAssistant/contactsBook.py
--rw-rw-rw-   0        0        0     1983 2024-05-24 06:37:57.000000 contacts_assistant-0.0.1/ContactsAssistant/datehelper.py
--rw-rw-rw-   0        0        0    16904 2024-05-24 11:34:46.000000 contacts_assistant-0.0.1/ContactsAssistant/handler.py
--rw-rw-rw-   0        0        0     6995 2024-05-24 11:34:46.000000 contacts_assistant-0.0.1/ContactsAssistant/menu.py
--rw-rw-rw-   0        0        0     3280 2024-05-24 06:37:57.000000 contacts_assistant-0.0.1/ContactsAssistant/note.py
--rw-rw-rw-   0        0        0     8394 2024-05-24 06:37:57.000000 contacts_assistant-0.0.1/ContactsAssistant/notebook.py
--rw-rw-rw-   0        0        0      549 2024-05-22 16:32:08.000000 contacts_assistant-0.0.1/ContactsAssistant/utils.py
--rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4080 2024-05-24 14:31:15.177903 contacts_assistant-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3313 2024-05-24 13:50:38.000000 contacts_assistant-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 14:31:15.176905 contacts_assistant-0.0.1/contacts_assistant.egg-info/
--rw-rw-rw-   0        0        0     4080 2024-05-24 14:31:15.000000 contacts_assistant-0.0.1/contacts_assistant.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2024-05-24 14:31:15.000000 contacts_assistant-0.0.1/contacts_assistant.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 14:31:15.000000 contacts_assistant-0.0.1/contacts_assistant.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-24 14:31:15.000000 contacts_assistant-0.0.1/contacts_assistant.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-24 14:31:15.000000 contacts_assistant-0.0.1/contacts_assistant.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 14:31:15.178914 contacts_assistant-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1420 2024-05-24 14:31:10.000000 contacts_assistant-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:15:05.386419 contacts_assistant-0.0.2/
+-rw-rw-rw-   0        0        0     1095 2024-05-22 08:53:23.000000 contacts_assistant-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4080 2024-05-24 15:15:05.385420 contacts_assistant-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3313 2024-05-24 13:50:38.000000 contacts_assistant-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 15:15:05.378420 contacts_assistant-0.0.2/contacts_assistant/
+-rw-rw-rw-   0        0        0     1330 2024-05-24 14:13:23.000000 contacts_assistant-0.0.2/contacts_assistant/Birthday.py
+-rw-rw-rw-   0        0        0     1217 2024-05-24 07:04:24.000000 contacts_assistant-0.0.2/contacts_assistant/Email.py
+-rw-rw-rw-   0        0        0      853 2024-05-22 16:29:48.000000 contacts_assistant-0.0.2/contacts_assistant/Field.py
+-rw-rw-rw-   0        0        0      591 2024-05-22 16:29:48.000000 contacts_assistant-0.0.2/contacts_assistant/Name.py
+-rw-rw-rw-   0        0        0     1504 2024-05-22 16:29:48.000000 contacts_assistant-0.0.2/contacts_assistant/Phone.py
+-rw-rw-rw-   0        0        0     6498 2024-05-24 07:04:24.000000 contacts_assistant-0.0.2/contacts_assistant/Record.py
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:51:21.000000 contacts_assistant-0.0.2/contacts_assistant/__init__.py
+-rw-rw-rw-   0        0        0     2248 2024-05-24 09:53:13.000000 contacts_assistant-0.0.2/contacts_assistant/__main__.py
+-rw-rw-rw-   0        0        0     2140 2024-05-24 08:47:43.000000 contacts_assistant-0.0.2/contacts_assistant/address.py
+-rw-rw-rw-   0        0        0     1201 2024-05-24 07:04:24.000000 contacts_assistant-0.0.2/contacts_assistant/command_completer.py
+-rw-rw-rw-   0        0        0      834 2024-05-24 11:34:46.000000 contacts_assistant-0.0.2/contacts_assistant/constants.py
+-rw-rw-rw-   0        0        0     8535 2024-05-24 11:34:46.000000 contacts_assistant-0.0.2/contacts_assistant/contactsBook.py
+-rw-rw-rw-   0        0        0     1983 2024-05-24 06:37:57.000000 contacts_assistant-0.0.2/contacts_assistant/datehelper.py
+-rw-rw-rw-   0        0        0    16904 2024-05-24 11:34:46.000000 contacts_assistant-0.0.2/contacts_assistant/handler.py
+-rw-rw-rw-   0        0        0     6995 2024-05-24 11:34:46.000000 contacts_assistant-0.0.2/contacts_assistant/menu.py
+-rw-rw-rw-   0        0        0     3280 2024-05-24 06:37:57.000000 contacts_assistant-0.0.2/contacts_assistant/note.py
+-rw-rw-rw-   0        0        0     8394 2024-05-24 06:37:57.000000 contacts_assistant-0.0.2/contacts_assistant/notebook.py
+-rw-rw-rw-   0        0        0      549 2024-05-22 16:32:08.000000 contacts_assistant-0.0.2/contacts_assistant/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:15:05.385420 contacts_assistant-0.0.2/contacts_assistant.egg-info/
+-rw-rw-rw-   0        0        0     4080 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      826 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-24 15:15:05.000000 contacts_assistant-0.0.2/contacts_assistant.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 15:15:05.386419 contacts_assistant-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1555 2024-05-24 15:05:05.000000 contacts_assistant-0.0.2/setup.py
```

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/Birthday.py` & `contacts_assistant-0.0.2/contacts_assistant/Birthday.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/Email.py` & `contacts_assistant-0.0.2/contacts_assistant/Email.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/Field.py` & `contacts_assistant-0.0.2/contacts_assistant/Field.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/Name.py` & `contacts_assistant-0.0.2/contacts_assistant/Name.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/Phone.py` & `contacts_assistant-0.0.2/contacts_assistant/Phone.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/Record.py` & `contacts_assistant-0.0.2/contacts_assistant/Record.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/__main__.py` & `contacts_assistant-0.0.2/contacts_assistant/__main__.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/address.py` & `contacts_assistant-0.0.2/contacts_assistant/address.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/command_completer.py` & `contacts_assistant-0.0.2/contacts_assistant/command_completer.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/constants.py` & `contacts_assistant-0.0.2/contacts_assistant/constants.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/contactsBook.py` & `contacts_assistant-0.0.2/contacts_assistant/contactsBook.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/datehelper.py` & `contacts_assistant-0.0.2/contacts_assistant/datehelper.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/handler.py` & `contacts_assistant-0.0.2/contacts_assistant/handler.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/menu.py` & `contacts_assistant-0.0.2/contacts_assistant/menu.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/note.py` & `contacts_assistant-0.0.2/contacts_assistant/note.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/notebook.py` & `contacts_assistant-0.0.2/contacts_assistant/notebook.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/ContactsAssistant/utils.py` & `contacts_assistant-0.0.2/contacts_assistant/utils.py`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/LICENSE` & `contacts_assistant-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/PKG-INFO` & `contacts_assistant-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.1
+Version: 0.0.2
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samiolenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `contacts_assistant-0.0.1/README.md` & `contacts_assistant-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `contacts_assistant-0.0.1/contacts_assistant.egg-info/PKG-INFO` & `contacts_assistant-0.0.2/contacts_assistant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contacts_assistant
-Version: 0.0.1
+Version: 0.0.2
 Summary: Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.
 Home-page: https://github.com/Bignichok/Python-ContactsAssistant
 Author: Mykyta Samiolenko
 Author-email: inikita546@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `contacts_assistant-0.0.1/contacts_assistant.egg-info/SOURCES.txt` & `contacts_assistant-0.0.2/contacts_assistant.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 LICENSE
 README.md
 setup.py
-ContactsAssistant/Birthday.py
-ContactsAssistant/Email.py
-ContactsAssistant/Field.py
-ContactsAssistant/Name.py
-ContactsAssistant/Phone.py
-ContactsAssistant/Record.py
-ContactsAssistant/__init__.py
-ContactsAssistant/__main__.py
-ContactsAssistant/address.py
-ContactsAssistant/command_completer.py
-ContactsAssistant/constants.py
-ContactsAssistant/contactsBook.py
-ContactsAssistant/datehelper.py
-ContactsAssistant/handler.py
-ContactsAssistant/menu.py
-ContactsAssistant/note.py
-ContactsAssistant/notebook.py
-ContactsAssistant/utils.py
+contacts_assistant/Birthday.py
+contacts_assistant/Email.py
+contacts_assistant/Field.py
+contacts_assistant/Name.py
+contacts_assistant/Phone.py
+contacts_assistant/Record.py
+contacts_assistant/__init__.py
+contacts_assistant/__main__.py
+contacts_assistant/address.py
+contacts_assistant/command_completer.py
+contacts_assistant/constants.py
+contacts_assistant/contactsBook.py
+contacts_assistant/datehelper.py
+contacts_assistant/handler.py
+contacts_assistant/menu.py
+contacts_assistant/note.py
+contacts_assistant/notebook.py
+contacts_assistant/utils.py
 contacts_assistant.egg-info/PKG-INFO
 contacts_assistant.egg-info/SOURCES.txt
 contacts_assistant.egg-info/dependency_links.txt
+contacts_assistant.egg-info/entry_points.txt
 contacts_assistant.egg-info/requires.txt
 contacts_assistant.egg-info/top_level.txt
```

### Comparing `contacts_assistant-0.0.1/setup.py` & `contacts_assistant-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,23 +17,28 @@
     encoding = result['encoding']
 
 with open("requirements.txt", "r", encoding=encoding) as fh:
     requirements = fh.read().splitlines()
 
 setuptools.setup(
     name="contacts_assistant",
-    version="0.0.1",
+    version="0.0.2",
     author="Mykyta Samiolenko",
     author_email="inikita546@gmail.com",
     description="Contacts Assistant is a bot designed to help you manage your address book efficiently. Below is a list of available commands, their functions, and required arguments. Additionally, you can add your notes to our notebook.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Bignichok/Python-ContactsAssistant",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
+    entry_points={
+        'console_scripts': [
+            'contacts-assistant=contacts_assistant.__main__:main'
+        ]
+    }
 )
```

