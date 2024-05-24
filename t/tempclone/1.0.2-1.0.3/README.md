# Comparing `tmp/tempclone-1.0.2.tar.gz` & `tmp/tempclone-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempclone-1.0.2.tar", last modified: Mon May 20 19:37:07 2024, max compression
+gzip compressed data, was "tempclone-1.0.3.tar", last modified: Fri May 24 13:11:44 2024, max compression
```

## Comparing `tempclone-1.0.2.tar` & `tempclone-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:37:07.718315 tempclone-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 19:36:52.000000 tempclone-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 19:37:07.718315 tempclone-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-20 19:36:52.000000 tempclone-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:37:07.718315 tempclone-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-20 19:36:52.000000 tempclone-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:37:07.714315 tempclone-1.0.2/tempclone/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:36:52.000000 tempclone-1.0.2/tempclone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-05-20 19:36:52.000000 tempclone-1.0.2/tempclone/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:37:07.714315 tempclone-1.0.2/tempclone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-20 19:37:07.000000 tempclone-1.0.2/tempclone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 19:37:07.000000 tempclone-1.0.2/tempclone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:37:07.000000 tempclone-1.0.2/tempclone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 19:37:07.000000 tempclone-1.0.2/tempclone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 19:37:07.000000 tempclone-1.0.2/tempclone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 19:37:07.000000 tempclone-1.0.2/tempclone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:37:07.718315 tempclone-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:36:52.000000 tempclone-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-20 19:36:52.000000 tempclone-1.0.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:11:44.450882 tempclone-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-24 13:11:26.000000 tempclone-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 13:11:44.450882 tempclone-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-24 13:11:26.000000 tempclone-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:11:44.450882 tempclone-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-24 13:11:26.000000 tempclone-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:11:44.450882 tempclone-1.0.3/tempclone/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:11:26.000000 tempclone-1.0.3/tempclone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-24 13:11:26.000000 tempclone-1.0.3/tempclone/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:11:44.450882 tempclone-1.0.3/tempclone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 13:11:44.000000 tempclone-1.0.3/tempclone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-24 13:11:44.000000 tempclone-1.0.3/tempclone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:11:44.000000 tempclone-1.0.3/tempclone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 13:11:44.000000 tempclone-1.0.3/tempclone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-24 13:11:44.000000 tempclone-1.0.3/tempclone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 13:11:44.000000 tempclone-1.0.3/tempclone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:11:44.450882 tempclone-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:11:26.000000 tempclone-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-24 13:11:26.000000 tempclone-1.0.3/tests/test_cli.py
```

### Comparing `tempclone-1.0.2/LICENSE` & `tempclone-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tempclone-1.0.2/PKG-INFO` & `tempclone-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempclone
-Version: 1.0.2
+Version: 1.0.3
 Summary: CLI to automate the creation of new projects from GitHub templates
 Home-page: https://github.com/yourusername/tempclone
 Author: Matheus
 Author-email: matheusmlfg@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tempclone-1.0.2/README.md` & `tempclone-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tempclone-1.0.2/setup.py` & `tempclone-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tempclone",
-    version="1.0.2",
+    version="1.0.3",
     author="Matheus",
     author_email="matheusmlfg@gmail.com",
     description="CLI to automate the creation of new projects from GitHub templates",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yourusername/tempclone",  # URL do repositório do seu projeto
     packages=find_packages(),
```

### Comparing `tempclone-1.0.2/tempclone/cli.py` & `tempclone-1.0.3/tempclone/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import subprocess
 import os
 import json
 from pathlib import Path
 import time
 
 GITHUB_API_URL = "https://api.github.com"
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 CONFIG_FILE = Path.home() / ".tempclone_config"
 
 ASCII_ART = r"""
- /$$$$$$$$ /$$$$$$ /$$     /$$ /$$$$$$      /$$$$  /$$      /$$$$$  /$$  /$$ /$$$$$$
-|__  $$__/| $$___/| $$$   /$$$| $$_  $$    /$$_ $$| $$     /$$_  $$| $$ | $$| $$___/
-   | $$   | $$    | $$$$  $$$$| $$ \ $$   | $$ \_/| $$    | $$ \ $$| $$$| $$| $$    
-   | $$   | $$$$  | $$ $$/$ $$| $$$$$$/   | $$    | $$    | $$ | $$| $$$$ $$| $$$$  
-   | $$   | $$_/  | $$  $$| $$| $$___/    | $$    | $$    | $$ | $$| $$ $$$$| $$_/  
-   | $$   | $$$$$$| $$ \/ | $$| $$        |  $$$$/| $$$$$$|  $$$$$/| $$\  $$| $$$$$$
-   |__/   |______/|__/    |__/|__/         \____/ |______/ \_____/ |__/ \__/|______/
+ /$$$$$$$ /$$$$$$ /$$      /|/$$$$$$      /$$$$  /$$     /$$$$$  /$$  /$$ /$$$$$$
+|__  $$_/| $$___/| $$$    /$| $$_  $$    /$$_ $$| $$    /$$_  $$| $$ | $$| $$___/
+   | $$  | $$    | $$$$  /$$| $$ \ $$   | $$ \_/| $$   | $$ \ $$| $$$| $$| $$    
+   | $$  | $$$$  | $$ $$/$ $| $$$$$$/   | $$    | $$   | $$ | $$| $$$$ $$| $$$$  
+   | $$  | $$_/  | $$  $$| $| $$___/    | $$    | $$   | $$ | $$| $$ $$$$| $$_/  
+   | $$  | $$$$$$| $$ \/ | $| $$        |  $$$$/| $$$$$|  $$$$$/| $$\  $$| $$$$$$
+   |__/  |______/|__/    |_/|__/         \____/ |_____/ \_____/ |__/ \__/|______/
 """
 
 def get_config():
     if CONFIG_FILE.exists():
         try:
             with open(CONFIG_FILE, "r") as file:
                 return json.load(file)
```

### Comparing `tempclone-1.0.2/tempclone.egg-info/PKG-INFO` & `tempclone-1.0.3/tempclone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempclone
-Version: 1.0.2
+Version: 1.0.3
 Summary: CLI to automate the creation of new projects from GitHub templates
 Home-page: https://github.com/yourusername/tempclone
 Author: Matheus
 Author-email: matheusmlfg@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tempclone-1.0.2/tests/test_cli.py` & `tempclone-1.0.3/tests/test_cli.py`

 * *Files identical despite different names*

