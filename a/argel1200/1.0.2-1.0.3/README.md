# Comparing `tmp/argel1200-1.0.2.tar.gz` & `tmp/argel1200-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argel1200-1.0.2.tar", last modified: Sat Mar 23 02:18:34 2024, max compression
+gzip compressed data, was "argel1200-1.0.3.tar", last modified: Fri May 24 17:24:52 2024, max compression
```

## Comparing `argel1200-1.0.2.tar` & `argel1200-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 02:18:34.230784 argel1200-1.0.2/
--rw-rw-rw-   0        0        0     1695 2024-03-23 02:18:34.229784 argel1200-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1355 2024-03-23 02:18:21.000000 argel1200-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-23 02:18:34.216277 argel1200-1.0.2/argel1200/
--rw-rw-rw-   0        0        0        0 2022-10-12 00:05:40.000000 argel1200-1.0.2/argel1200/__init__.py
--rw-rw-rw-   0        0        0     7550 2024-03-23 02:18:21.000000 argel1200-1.0.2/argel1200/utilities.py
-drwxrwxrwx   0        0        0        0 2024-03-23 02:18:34.227255 argel1200-1.0.2/argel1200.egg-info/
--rw-rw-rw-   0        0        0     1695 2024-03-23 02:18:34.000000 argel1200-1.0.2/argel1200.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2024-03-23 02:18:34.000000 argel1200-1.0.2/argel1200.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 02:18:34.000000 argel1200-1.0.2/argel1200.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-03-23 02:18:34.000000 argel1200-1.0.2/argel1200.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-23 02:18:34.000000 argel1200-1.0.2/argel1200.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-23 02:18:34.231809 argel1200-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      515 2024-03-23 02:18:21.000000 argel1200-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:24:52.744404 argel1200-1.0.3/
+-rw-rw-rw-   0        0        0     1695 2024-05-24 17:24:52.743123 argel1200-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1355 2024-03-23 02:18:21.000000 argel1200-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 17:24:52.737843 argel1200-1.0.3/argel1200/
+-rw-rw-rw-   0        0        0        0 2022-10-12 00:05:40.000000 argel1200-1.0.3/argel1200/__init__.py
+-rw-rw-rw-   0        0        0     8045 2024-05-24 17:22:23.000000 argel1200-1.0.3/argel1200/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:24:52.743123 argel1200-1.0.3/argel1200.egg-info/
+-rw-rw-rw-   0        0        0     1695 2024-05-24 17:24:52.000000 argel1200-1.0.3/argel1200.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2024-05-24 17:24:52.000000 argel1200-1.0.3/argel1200.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 17:24:52.000000 argel1200-1.0.3/argel1200.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 17:24:52.000000 argel1200-1.0.3/argel1200.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 17:24:52.000000 argel1200-1.0.3/argel1200.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 17:24:52.744404 argel1200-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      515 2024-05-24 17:10:12.000000 argel1200-1.0.3/setup.py
```

### Comparing `argel1200-1.0.2/PKG-INFO` & `argel1200-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argel1200
-Version: 1.0.2
+Version: 1.0.3
 Summary: My utility functions
 Home-page: https://github.com/argel1200/argel1200-python
 Author: argel1200
 Author-email: argel@msn.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: click>=7.1.2
```

### Comparing `argel1200-1.0.2/README.md` & `argel1200-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `argel1200-1.0.2/argel1200/utilities.py` & `argel1200-1.0.3/argel1200/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import dataclasses
 import errno
 import click
 import dumper
 import haggis.logs
 import logging
 import os
 import re
 import sys
 import traceback
-
+from dataclasses import dataclass
+from typing import Optional
 
 def get_variable_name(stack_back=-2):
     """
     Called by dumps()
 
     Pulls the variable names from the function that called this function
 
@@ -197,7 +199,18 @@
         print(f"Type: {exc_type}; Value: {exc_value}; Traceback: {exc_traceback}")
         print(f"Try running the program with -h or --help.")
         exit(10)
 
     if click_invoke_rc == 0:  # Catch if -h, --help, --version, or something unknown was specified
         exit(1)
 
+# Intent is, in your script, to import this and create a dataclass like below:
+#    @dataclass
+#       class Config(argel1200.utilties.Config_Base):
+#       csv_in_file: str = foo.csv
+#   my_cfg=Config()
+# This way you can do a my_cfg.log_level  without having to remember to add it to your Config class
+
+@dataclass
+class ConfigBase:
+    logger_out_filename: Optional[str]
+    log_level: str = 'debug'
```

### Comparing `argel1200-1.0.2/argel1200.egg-info/PKG-INFO` & `argel1200-1.0.3/argel1200.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argel1200
-Version: 1.0.2
+Version: 1.0.3
 Summary: My utility functions
 Home-page: https://github.com/argel1200/argel1200-python
 Author: argel1200
 Author-email: argel@msn.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: click>=7.1.2
```

### Comparing `argel1200-1.0.2/setup.py` & `argel1200-1.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='argel1200',
-    version='1.0.2',
+    version='1.0.3',
     packages=['argel1200'],
     url='https://github.com/argel1200/argel1200-python',
     license='MIT',
     author='argel1200',
     author_email='argel@msn.com',
     description='My utility functions',
     long_description=open('README.md').read(),
```

