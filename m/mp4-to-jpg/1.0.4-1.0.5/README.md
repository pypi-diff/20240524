# Comparing `tmp/mp4_to_jpg-1.0.4.tar.gz` & `tmp/mp4_to_jpg-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mp4_to_jpg-1.0.4.tar", last modified: Wed May 22 11:42:41 2024, max compression
+gzip compressed data, was "mp4_to_jpg-1.0.5.tar", last modified: Fri May 24 14:35:08 2024, max compression
```

## Comparing `mp4_to_jpg-1.0.4.tar` & `mp4_to_jpg-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-22 11:42:41.444969 mp4_to_jpg-1.0.4/
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4648 2024-05-22 11:42:41.444707 mp4_to_jpg-1.0.4/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4065 2024-05-16 13:42:55.000000 mp4_to_jpg-1.0.4/README.md
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-22 11:42:41.443310 mp4_to_jpg-1.0.4/mp4_to_jpg/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-16 13:47:00.000000 mp4_to_jpg-1.0.4/mp4_to_jpg/__init__.py
--rw-r--r--   0 tadeasfort   (501) staff       (20)    11373 2024-05-22 11:40:31.000000 mp4_to_jpg-1.0.4/mp4_to_jpg/mp4_to_jpg.py
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-22 11:42:41.444286 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4648 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)      272 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/SOURCES.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/dependency_links.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       58 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/entry_points.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       46 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/requires.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       11 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/top_level.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-22 11:42:41.445024 mp4_to_jpg-1.0.4/setup.cfg
--rw-r--r--   0 tadeasfort   (501) staff       (20)      891 2024-05-22 11:42:38.000000 mp4_to_jpg-1.0.4/setup.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 14:35:08.651393 mp4_to_jpg-1.0.5/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4653 2024-05-24 14:35:08.651177 mp4_to_jpg-1.0.5/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4065 2024-05-16 13:42:55.000000 mp4_to_jpg-1.0.5/README.md
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 14:35:08.649556 mp4_to_jpg-1.0.5/mp4_to_jpg/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-16 13:47:00.000000 mp4_to_jpg-1.0.5/mp4_to_jpg/__init__.py
+-rw-r--r--   0 tadeasfort   (501) staff       (20)    11389 2024-05-24 14:33:54.000000 mp4_to_jpg-1.0.5/mp4_to_jpg/mp4_to_jpg.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-24 14:35:08.650733 mp4_to_jpg-1.0.5/mp4_to_jpg.egg-info/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4653 2024-05-24 14:35:08.000000 mp4_to_jpg-1.0.5/mp4_to_jpg.egg-info/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      272 2024-05-24 14:35:08.000000 mp4_to_jpg-1.0.5/mp4_to_jpg.egg-info/SOURCES.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-24 14:35:08.000000 mp4_to_jpg-1.0.5/mp4_to_jpg.egg-info/dependency_links.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       58 2024-05-24 14:35:08.000000 mp4_to_jpg-1.0.5/mp4_to_jpg.egg-info/entry_points.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       51 2024-05-24 14:35:08.000000 mp4_to_jpg-1.0.5/mp4_to_jpg.egg-info/requires.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       11 2024-05-24 14:35:08.000000 mp4_to_jpg-1.0.5/mp4_to_jpg.egg-info/top_level.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-24 14:35:08.651438 mp4_to_jpg-1.0.5/setup.cfg
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      896 2024-05-24 14:34:50.000000 mp4_to_jpg-1.0.5/setup.py
```

### Comparing `mp4_to_jpg-1.0.4/PKG-INFO` & `mp4_to_jpg-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mp4_to_jpg
-Version: 1.0.4
+Version: 1.0.5
 Summary: A tool to extract frames from MP4 videos and remove duplicates
 Home-page: https://github.com/tadeasf/mp4-to-jpg_click
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: click
+Requires-Dist: rich-click
 Requires-Dist: opencv-python
 Requires-Dist: tk
 Requires-Dist: tqdm
 Requires-Dist: loguru
 Requires-Dist: imagededup
 
 # Video Frame Extraction Tool
```

### Comparing `mp4_to_jpg-1.0.4/README.md` & `mp4_to_jpg-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mp4_to_jpg-1.0.4/mp4_to_jpg/mp4_to_jpg.py` & `mp4_to_jpg-1.0.5/mp4_to_jpg/mp4_to_jpg.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import shutil
 import tempfile
 import concurrent.futures
 from pathlib import Path
 import tkinter as tk
 from tkinter import filedialog
-import click
+from rich_click import click
 from tqdm import tqdm
 from loguru import logger
 from imagededup.methods import CNN
 import math
 
 # Setup loguru for logging
 logger.add("file_{time}.log", rotation="1 MB", backtrace=True, diagnose=True)
```

### Comparing `mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/PKG-INFO` & `mp4_to_jpg-1.0.5/mp4_to_jpg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mp4_to_jpg
-Version: 1.0.4
+Version: 1.0.5
 Summary: A tool to extract frames from MP4 videos and remove duplicates
 Home-page: https://github.com/tadeasf/mp4-to-jpg_click
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: click
+Requires-Dist: rich-click
 Requires-Dist: opencv-python
 Requires-Dist: tk
 Requires-Dist: tqdm
 Requires-Dist: loguru
 Requires-Dist: imagededup
 
 # Video Frame Extraction Tool
```

### Comparing `mp4_to_jpg-1.0.4/setup.py` & `mp4_to_jpg-1.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mp4_to_jpg",
-    version="1.0.4",
+    version="1.0.5",
     author="Tadeas Fort",
     author_email="taddy.fort@gmail.com",
     description="A tool to extract frames from MP4 videos and remove duplicates",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tadeasf/mp4-to-jpg_click",
     packages=find_packages(),
     install_requires=[
-        "click",
+        "rich-click",
         "opencv-python",
         "tk",
         "tqdm",
         "loguru",
         "imagededup",
     ],
     entry_points={
```

