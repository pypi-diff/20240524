# Comparing `tmp/pyperclip_plus-0.1.2.tar.gz` & `tmp/pyperclip-plus-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyperclip_plus-0.1.2.tar", last modified: Fri May 24 10:12:02 2024, max compression
+gzip compressed data, was "pyperclip-plus-0.1.3.tar", last modified: Fri May 24 10:20:22 2024, max compression
```

## Comparing `pyperclip_plus-0.1.2.tar` & `pyperclip-plus-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-24 10:12:02.073812 pyperclip_plus-0.1.2/
--rw-r--r--   0 akitashowhey   (501) staff       (20)     5418 2024-05-24 10:12:02.073672 pyperclip_plus-0.1.2/PKG-INFO
--rw-r--r--   0 akitashowhey   (501) staff       (20)     4684 2024-05-24 09:59:11.000000 pyperclip_plus-0.1.2/README.md
-drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-24 10:12:02.072684 pyperclip_plus-0.1.2/pyperclip_plus/
--rw-r--r--   0 akitashowhey   (501) staff       (20)       78 2024-05-24 10:10:16.000000 pyperclip_plus-0.1.2/pyperclip_plus/__init__.py
--rw-r--r--   0 akitashowhey   (501) staff       (20)     1422 2024-05-24 09:23:05.000000 pyperclip_plus-0.1.2/pyperclip_plus/clipboard_manager.py
-drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-24 10:12:02.073446 pyperclip_plus-0.1.2/pyperclip_plus.egg-info/
--rw-r--r--   0 akitashowhey   (501) staff       (20)     5418 2024-05-24 10:12:02.000000 pyperclip_plus-0.1.2/pyperclip_plus.egg-info/PKG-INFO
--rw-r--r--   0 akitashowhey   (501) staff       (20)      233 2024-05-24 10:12:02.000000 pyperclip_plus-0.1.2/pyperclip_plus.egg-info/SOURCES.txt
--rw-r--r--   0 akitashowhey   (501) staff       (20)        1 2024-05-24 10:12:02.000000 pyperclip_plus-0.1.2/pyperclip_plus.egg-info/dependency_links.txt
--rw-r--r--   0 akitashowhey   (501) staff       (20)       15 2024-05-24 10:12:02.000000 pyperclip_plus-0.1.2/pyperclip_plus.egg-info/top_level.txt
--rw-r--r--   0 akitashowhey   (501) staff       (20)       38 2024-05-24 10:12:02.073869 pyperclip_plus-0.1.2/setup.cfg
--rw-r--r--   0 akitashowhey   (501) staff       (20)     1025 2024-05-24 09:45:13.000000 pyperclip_plus-0.1.2/setup.py
+drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-24 10:20:22.301374 pyperclip-plus-0.1.3/
+-rw-r--r--   0 akitashowhey   (501) staff       (20)     5418 2024-05-24 10:20:22.301248 pyperclip-plus-0.1.3/PKG-INFO
+-rw-r--r--   0 akitashowhey   (501) staff       (20)     4684 2024-05-24 09:59:11.000000 pyperclip-plus-0.1.3/README.md
+drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-24 10:20:22.300370 pyperclip-plus-0.1.3/pyperclip-plus/
+-rw-r--r--   0 akitashowhey   (501) staff       (20)       78 2024-05-24 10:10:16.000000 pyperclip-plus-0.1.3/pyperclip-plus/__init__.py
+-rw-r--r--   0 akitashowhey   (501) staff       (20)     1422 2024-05-24 09:23:05.000000 pyperclip-plus-0.1.3/pyperclip-plus/clipboard_manager.py
+drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-24 10:20:22.301020 pyperclip-plus-0.1.3/pyperclip_plus.egg-info/
+-rw-r--r--   0 akitashowhey   (501) staff       (20)     5418 2024-05-24 10:20:22.000000 pyperclip-plus-0.1.3/pyperclip_plus.egg-info/PKG-INFO
+-rw-r--r--   0 akitashowhey   (501) staff       (20)      233 2024-05-24 10:20:22.000000 pyperclip-plus-0.1.3/pyperclip_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 akitashowhey   (501) staff       (20)        1 2024-05-24 10:20:22.000000 pyperclip-plus-0.1.3/pyperclip_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 akitashowhey   (501) staff       (20)       15 2024-05-24 10:20:22.000000 pyperclip-plus-0.1.3/pyperclip_plus.egg-info/top_level.txt
+-rw-r--r--   0 akitashowhey   (501) staff       (20)       38 2024-05-24 10:20:22.301419 pyperclip-plus-0.1.3/setup.cfg
+-rw-r--r--   0 akitashowhey   (501) staff       (20)     1025 2024-05-24 10:19:59.000000 pyperclip-plus-0.1.3/setup.py
```

### Comparing `pyperclip_plus-0.1.2/PKG-INFO` & `pyperclip-plus-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyperclip_plus
-Version: 0.1.2
+Name: pyperclip-plus
+Version: 0.1.3
 Summary: An enhanced clipboard management tool
 Home-page: https://github.com/yourusername/pyperclip_plus
 Author: Your Name
 Author-email: your.email@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyperclip_plus-0.1.2/README.md` & `pyperclip-plus-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyperclip_plus-0.1.2/pyperclip_plus/clipboard_manager.py` & `pyperclip-plus-0.1.3/pyperclip-plus/clipboard_manager.py`

 * *Files identical despite different names*

### Comparing `pyperclip_plus-0.1.2/pyperclip_plus.egg-info/PKG-INFO` & `pyperclip-plus-0.1.3/pyperclip_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperclip-plus
-Version: 0.1.2
+Version: 0.1.3
 Summary: An enhanced clipboard management tool
 Home-page: https://github.com/yourusername/pyperclip_plus
 Author: Your Name
 Author-email: your.email@example.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyperclip_plus-0.1.2/setup.py` & `pyperclip-plus-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # setup.py
 from setuptools import setup, find_packages
 import pathlib
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 setup(
-    name='pyperclip_plus',
-    version='0.1.2',
+    name='pyperclip-plus',
+    version='0.1.3',
     packages=find_packages(),
     description='An enhanced clipboard management tool',
     author='Your Name',
     author_email='your.email@example.com',
     url='https://github.com/yourusername/pyperclip_plus',  # プロジェクトのURLを設定
     long_description=long_description,
     long_description_content_type="text/markdown",
```

