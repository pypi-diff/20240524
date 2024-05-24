# Comparing `tmp/mcd_stitcher-0.1.1.tar.gz` & `tmp/mcd_stitcher-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcd_stitcher-0.1.1.tar", last modified: Fri May 24 17:07:54 2024, max compression
+gzip compressed data, was "mcd_stitcher-0.1.2.tar", last modified: Fri May 24 17:29:14 2024, max compression
```

## Comparing `mcd_stitcher-0.1.1.tar` & `mcd_stitcher-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/mcd_stitcher/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/mcd_stitcher/imclib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/imcdataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/imcraw.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdxmlparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/metadefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/stitcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:29:14.869933 mcd_stitcher-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-24 17:29:14.869933 mcd_stitcher-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:29:14.865934 mcd_stitcher-0.1.2/mcd_stitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/mcd_stitcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/mcd_stitcher/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:29:14.869933 mcd_stitcher-0.1.2/mcd_stitcher/imclib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/mcd_stitcher/imclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/mcd_stitcher/imclib/imcdataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/mcd_stitcher/imclib/imcraw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/mcd_stitcher/imclib/mcdmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/mcd_stitcher/imclib/mcdutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/mcd_stitcher/imclib/mcdxmlparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/mcd_stitcher/imclib/metadefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/mcd_stitcher/stitcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:29:14.869933 mcd_stitcher-0.1.2/mcd_stitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-24 17:29:14.000000 mcd_stitcher-0.1.2/mcd_stitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-24 17:29:14.000000 mcd_stitcher-0.1.2/mcd_stitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:29:14.000000 mcd_stitcher-0.1.2/mcd_stitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-24 17:29:14.000000 mcd_stitcher-0.1.2/mcd_stitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 17:29:14.000000 mcd_stitcher-0.1.2/mcd_stitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 17:29:14.000000 mcd_stitcher-0.1.2/mcd_stitcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-24 17:29:14.869933 mcd_stitcher-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-24 17:29:04.000000 mcd_stitcher-0.1.2/setup.py
```

### Comparing `mcd_stitcher-0.1.1/LICENSE` & `mcd_stitcher-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.1/PKG-INFO` & `mcd_stitcher-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcd_stitcher
-Version: 0.1.1
+Version: 0.1.2
 Summary: MCD to Zarr conversion and stitching
 Home-page: https://github.com/PawanChaurasia/mcd_stitcher
 Author: Pawan Chaurasia
 Author-email: pchaurasia98@gmail.com
 Project-URL: Bug Tracker, https://github.com/PawanChaurasia/mcd_stitcher/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mcd_stitcher-0.1.1/README.md` & `mcd_stitcher-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.1/mcd_stitcher/__init__.py` & `mcd_stitcher-0.1.2/mcd_stitcher/__init__.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.1/mcd_stitcher/converter.py` & `mcd_stitcher-0.1.2/mcd_stitcher/converter.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.1/mcd_stitcher/imclib/imcdataparser.py` & `mcd_stitcher-0.1.2/mcd_stitcher/imclib/imcdataparser.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.1/mcd_stitcher/imclib/imcraw.py` & `mcd_stitcher-0.1.2/mcd_stitcher/imclib/imcraw.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdmeta.py` & `mcd_stitcher-0.1.2/mcd_stitcher/imclib/mcdmeta.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdutils.py` & `mcd_stitcher-0.1.2/mcd_stitcher/imclib/mcdutils.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdxmlparser.py` & `mcd_stitcher-0.1.2/mcd_stitcher/imclib/mcdxmlparser.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.1/mcd_stitcher/imclib/metadefs.py` & `mcd_stitcher-0.1.2/mcd_stitcher/imclib/metadefs.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.1/mcd_stitcher/stitcher.py` & `mcd_stitcher-0.1.2/mcd_stitcher/stitcher.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.1/mcd_stitcher.egg-info/PKG-INFO` & `mcd_stitcher-0.1.2/mcd_stitcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcd_stitcher
-Version: 0.1.1
+Version: 0.1.2
 Summary: MCD to Zarr conversion and stitching
 Home-page: https://github.com/PawanChaurasia/mcd_stitcher
 Author: Pawan Chaurasia
 Author-email: pchaurasia98@gmail.com
 Project-URL: Bug Tracker, https://github.com/PawanChaurasia/mcd_stitcher/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mcd_stitcher-0.1.1/mcd_stitcher.egg-info/SOURCES.txt` & `mcd_stitcher-0.1.2/mcd_stitcher.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 setup.py
 mcd_stitcher/__init__.py
 mcd_stitcher/converter.py
 mcd_stitcher/stitcher.py
 mcd_stitcher.egg-info/PKG-INFO
 mcd_stitcher.egg-info/SOURCES.txt
 mcd_stitcher.egg-info/dependency_links.txt
```

### Comparing `mcd_stitcher-0.1.1/setup.py` & `mcd_stitcher-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mcd_stitcher',
-    version='0.1.1',
+    version='0.1.2',
     author='Pawan Chaurasia',
     author_email='pchaurasia98@gmail.com',
     description='MCD to Zarr conversion and stitching',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/PawanChaurasia/mcd_stitcher',
     project_urls={
```

