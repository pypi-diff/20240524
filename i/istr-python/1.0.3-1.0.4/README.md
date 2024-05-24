# Comparing `tmp/istr_python-1.0.3.tar.gz` & `tmp/istr_python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-1.0.3.tar", last modified: Fri May 24 09:19:41 2024, max compression
+gzip compressed data, was "istr_python-1.0.4.tar", last modified: Fri May 24 09:21:42 2024, max compression
```

## Comparing `istr_python-1.0.3.tar` & `istr_python-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 09:19:41.950298 istr_python-1.0.3/
--rw-rw-rw-   0        0        0    16546 2024-05-24 09:19:41.942880 istr_python-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    15382 2024-05-20 18:51:02.000000 istr_python-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 09:19:41.892674 istr_python-1.0.3/istr/
--rw-rw-rw-   0        0        0     1100 2024-05-14 13:17:20.000000 istr_python-1.0.3/istr/LICENSE.txt
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-1.0.3/istr/__init__.py
--rw-rw-rw-   0        0        0    18685 2024-05-24 09:15:55.000000 istr_python-1.0.3/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-05-24 09:19:41.937298 istr_python-1.0.3/istr_python.egg-info/
--rw-rw-rw-   0        0        0    16546 2024-05-24 09:19:41.000000 istr_python-1.0.3/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-05-24 09:19:41.000000 istr_python-1.0.3/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 09:19:41.000000 istr_python-1.0.3/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-24 09:19:41.000000 istr_python-1.0.3/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      711 2024-05-24 09:19:32.000000 istr_python-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-24 09:19:41.951300 istr_python-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-24 09:19:41.930235 istr_python-1.0.3/tests/
--rw-rw-rw-   0        0        0    17265 2024-05-24 09:16:04.000000 istr_python-1.0.3/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:21:42.674208 istr_python-1.0.4/
+-rw-rw-rw-   0        0        0    16546 2024-05-24 09:21:42.670570 istr_python-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    15382 2024-05-20 18:51:02.000000 istr_python-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 09:21:42.614698 istr_python-1.0.4/istr/
+-rw-rw-rw-   0        0        0     1100 2024-05-14 13:17:20.000000 istr_python-1.0.4/istr/LICENSE.txt
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-1.0.4/istr/__init__.py
+-rw-rw-rw-   0        0        0    18685 2024-05-24 09:20:38.000000 istr_python-1.0.4/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-05-24 09:21:42.667568 istr_python-1.0.4/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    16546 2024-05-24 09:21:42.000000 istr_python-1.0.4/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-05-24 09:21:42.000000 istr_python-1.0.4/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 09:21:42.000000 istr_python-1.0.4/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-24 09:21:42.000000 istr_python-1.0.4/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      711 2024-05-24 09:21:36.000000 istr_python-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 09:21:42.674208 istr_python-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 09:21:42.663524 istr_python-1.0.4/tests/
+-rw-rw-rw-   0        0        0    17265 2024-05-24 09:16:04.000000 istr_python-1.0.4/tests/test_istr.py
```

### Comparing `istr_python-1.0.3/PKG-INFO` & `istr_python-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `istr_python-1.0.3/README.md` & `istr_python-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `istr_python-1.0.3/istr/LICENSE.txt` & `istr_python-1.0.4/istr/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `istr_python-1.0.3/istr/istr.py` & `istr_python-1.0.4/istr/istr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #     _       _
 #    (_) ___ | |_  _ __
 #    | |/ __|| __|| '__|
 #    | |\__ \| |_ | |
 #    |_||___/ \__||_|
 # strings you can count on
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 import functools
 import math
 import copy
 
 """
 Note: the changelog is now in changelog.md
```

### Comparing `istr_python-1.0.3/istr_python.egg-info/PKG-INFO` & `istr_python-1.0.4/istr_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 1.0.3
+Version: 1.0.4
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `istr_python-1.0.3/pyproject.toml` & `istr_python-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "1.0.3"
+version = "1.0.4"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `istr_python-1.0.3/tests/test_istr.py` & `istr_python-1.0.4/tests/test_istr.py`

 * *Files identical despite different names*

