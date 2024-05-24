# Comparing `tmp/pazok-0.1.2.tar.gz` & `tmp/pazok-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pazok-0.1.2.tar", last modified: Fri May 24 00:01:59 2024, max compression
+gzip compressed data, was "pazok-0.1.4.tar", last modified: Fri May 24 12:09:35 2024, max compression
```

## Comparing `pazok-0.1.2.tar` & `pazok-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 00:01:59.216487 pazok-0.1.2/
--rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1141 2024-05-24 00:01:59.215492 pazok-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 00:01:59.201528 pazok-0.1.2/pazok/
--rw-rw-rw-   0        0        0      723 2024-05-23 23:50:04.000000 pazok-0.1.2/pazok/__init__.py
--rw-rw-rw-   0        0        0    44226 2024-05-23 23:59:46.000000 pazok-0.1.2/pazok/pazok.py
-drwxrwxrwx   0        0        0        0 2024-05-24 00:01:59.213497 pazok-0.1.2/pazok.egg-info/
--rw-rw-rw-   0        0        0     1141 2024-05-24 00:01:59.000000 pazok-0.1.2/pazok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-24 00:01:59.000000 pazok-0.1.2/pazok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 00:01:59.000000 pazok-0.1.2/pazok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-24 00:01:59.000000 pazok-0.1.2/pazok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 00:01:59.216487 pazok-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      552 2024-05-24 00:01:50.000000 pazok-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 12:09:35.506591 pazok-0.1.4/
+-rw-rw-rw-   0        0        0       29 2024-05-23 23:30:01.000000 pazok-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1141 2024-05-24 12:09:35.503599 pazok-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-05-23 23:29:46.000000 pazok-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 12:09:35.472683 pazok-0.1.4/pazok/
+-rw-rw-rw-   0        0        0      723 2024-05-24 12:03:21.000000 pazok-0.1.4/pazok/__init__.py
+-rw-rw-rw-   0        0        0    44251 2024-05-24 12:03:19.000000 pazok-0.1.4/pazok/pazok.py
+drwxrwxrwx   0        0        0        0 2024-05-24 12:09:35.499613 pazok-0.1.4/pazok.egg-info/
+-rw-rw-rw-   0        0        0     1141 2024-05-24 12:09:35.000000 pazok-0.1.4/pazok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-24 12:09:35.000000 pazok-0.1.4/pazok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 12:09:35.000000 pazok-0.1.4/pazok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 12:09:35.000000 pazok-0.1.4/pazok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 12:09:35.506591 pazok-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      552 2024-05-24 12:09:20.000000 pazok-0.1.4/setup.py
```

### Comparing `pazok-0.1.2/PKG-INFO` & `pazok-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pazok
-Version: 0.1.2
+Version: 0.1.4
 Summary: A short description of my package
 Author: b_azo
 Author-email: husseun.selt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pazok Version: 0.1.2 Summary: A short description
+Metadata-Version: 2.1 Name: pazok Version: 0.1.4 Summary: A short description
 of my package Author: b_azo Author-email: husseun.selt@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt
                               ************ ppaazzookk ************
 ### What is pazok? It is a python library that contains a set of ready-made
 codes that enable you to create the most wonderful designs and animations on
```

### Comparing `pazok-0.1.2/README.md` & `pazok-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pazok-0.1.2/pazok/__init__.py` & `pazok-0.1.4/pazok/__init__.py`

 * *Files identical despite different names*

### Comparing `pazok-0.1.2/pazok/pazok.py` & `pazok-0.1.4/pazok/pazok.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 try:
-
+    import requests
     import argparse
     import json
     import locale
     import re
     import shlex
     from collections import OrderedDict
     from urllib.parse import unquote, urlparse
@@ -32,14 +32,15 @@
     os.system("pip install python-cfonts")
     os.system("pip install pyTelegramBotAPI")
     os.system("pip install colorama")
     os.system("pip install requests")
     os.system("pip install threading")
     os.system("pip install random")
     os.system("pip install time")
+    
 
 #- - - - - - - - - - - - - - -- - - - - - -- - - - - #
 #لوكو
 def logo():
     o = "\u001b[38;5;208m"  # برتقالي
     e = "\u001b[38;5;242m"  # رمادي داكن
     logo=f"""
```

### Comparing `pazok-0.1.2/pazok.egg-info/PKG-INFO` & `pazok-0.1.4/pazok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pazok
-Version: 0.1.2
+Version: 0.1.4
 Summary: A short description of my package
 Author: b_azo
 Author-email: husseun.selt@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pazok Version: 0.1.2 Summary: A short description
+Metadata-Version: 2.1 Name: pazok Version: 0.1.4 Summary: A short description
 of my package Author: b_azo Author-email: husseun.selt@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt
                               ************ ppaazzookk ************
 ### What is pazok? It is a python library that contains a set of ready-made
 codes that enable you to create the most wonderful designs and animations on
```

### Comparing `pazok-0.1.2/setup.py` & `pazok-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pazok',
-    version='0.1.2',
+    version='0.1.4',
     author='b_azo',
     author_email='husseun.selt@gmail.com',
     description='A short description of my package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

