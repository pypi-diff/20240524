# Comparing `tmp/pinscrape-3.2.0.tar.gz` & `tmp/pinscrape-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinscrape-3.2.0.tar", last modified: Tue May 21 08:47:23 2024, max compression
+gzip compressed data, was "pinscrape-3.2.1.tar", last modified: Fri May 24 10:32:50 2024, max compression
```

## Comparing `pinscrape-3.2.0.tar` & `pinscrape-3.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:47:23.188009 pinscrape-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-21 08:47:09.000000 pinscrape-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 08:47:23.184009 pinscrape-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 08:47:09.000000 pinscrape-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:47:23.184009 pinscrape-3.2.0/pinscrape/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-21 08:47:09.000000 pinscrape-3.2.0/pinscrape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 08:47:09.000000 pinscrape-3.2.0/pinscrape/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-05-21 08:47:09.000000 pinscrape-3.2.0/pinscrape/pinscrape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:47:23.184009 pinscrape-3.2.0/pinscrape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 08:47:23.000000 pinscrape-3.2.0/pinscrape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-21 08:47:23.000000 pinscrape-3.2.0/pinscrape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:47:23.000000 pinscrape-3.2.0/pinscrape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-21 08:47:23.000000 pinscrape-3.2.0/pinscrape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 08:47:23.000000 pinscrape-3.2.0/pinscrape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:47:23.188009 pinscrape-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-21 08:47:09.000000 pinscrape-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:32:50.147877 pinscrape-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-24 10:32:36.000000 pinscrape-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-24 10:32:50.147877 pinscrape-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-24 10:32:36.000000 pinscrape-3.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:32:50.143877 pinscrape-3.2.1/pinscrape/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-24 10:32:36.000000 pinscrape-3.2.1/pinscrape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 10:32:36.000000 pinscrape-3.2.1/pinscrape/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-05-24 10:32:36.000000 pinscrape-3.2.1/pinscrape/pinscrape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:32:50.147877 pinscrape-3.2.1/pinscrape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-24 10:32:50.000000 pinscrape-3.2.1/pinscrape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-24 10:32:50.000000 pinscrape-3.2.1/pinscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 10:32:50.000000 pinscrape-3.2.1/pinscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-24 10:32:50.000000 pinscrape-3.2.1/pinscrape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 10:32:50.000000 pinscrape-3.2.1/pinscrape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 10:32:50.147877 pinscrape-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-24 10:32:36.000000 pinscrape-3.2.1/setup.py
```

### Comparing `pinscrape-3.2.0/LICENSE` & `pinscrape-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pinscrape-3.2.0/PKG-INFO` & `pinscrape-3.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 3.2.0
+Version: 3.2.1
 Summary: Pinterest | a simple data scraper for pinterest
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.32.0
 Requires-Dist: beautifulsoup4==4.11.1
-Requires-Dist: tqdm==4.66.3
 Requires-Dist: pydotmap
 Requires-Dist: opencv-python
 Requires-Dist: pytest==7.2.0
 
 # pinscrape
 [![built with Python3](https://img.shields.io/badge/built%20with-Python3.6+-red.svg)](https://www.python.org/)
```

### Comparing `pinscrape-3.2.0/README.md` & `pinscrape-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pinscrape-3.2.0/pinscrape/pinscrape.py` & `pinscrape-3.2.1/pinscrape/pinscrape.py`

 * *Files identical despite different names*

### Comparing `pinscrape-3.2.0/pinscrape.egg-info/PKG-INFO` & `pinscrape-3.2.1/pinscrape.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: pinscrape
-Version: 3.2.0
+Version: 3.2.1
 Summary: Pinterest | a simple data scraper for pinterest
 Home-page: https://github.com/iamatulsingh/pinscrape
 Author: Atul Singh
 Author-email: atulsingh0401@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.32.0
 Requires-Dist: beautifulsoup4==4.11.1
-Requires-Dist: tqdm==4.66.3
 Requires-Dist: pydotmap
 Requires-Dist: opencv-python
 Requires-Dist: pytest==7.2.0
 
 # pinscrape
 [![built with Python3](https://img.shields.io/badge/built%20with-Python3.6+-red.svg)](https://www.python.org/)
```

### Comparing `pinscrape-3.2.0/setup.py` & `pinscrape-3.2.1/setup.py`

 * *Files identical despite different names*

