# Comparing `tmp/mcd_stitcher-0.1.0.tar.gz` & `tmp/mcd_stitcher-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcd_stitcher-0.1.0.tar", last modified: Fri May 24 08:15:15 2024, max compression
+gzip compressed data, was "mcd_stitcher-0.1.1.tar", last modified: Fri May 24 17:07:54 2024, max compression
```

## Comparing `mcd_stitcher-0.1.0.tar` & `mcd_stitcher-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:15:15.410264 mcd_stitcher-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-24 08:15:15.410264 mcd_stitcher-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:15:15.406264 mcd_stitcher-0.1.0/mcd_stitcher/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/mcd_stitcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/mcd_stitcher/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:15:15.410264 mcd_stitcher-0.1.0/mcd_stitcher/imclib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/mcd_stitcher/imclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/mcd_stitcher/imclib/imcdataparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/mcd_stitcher/imclib/imcraw.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/mcd_stitcher/imclib/mcdmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/mcd_stitcher/imclib/mcdutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/mcd_stitcher/imclib/mcdxmlparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/mcd_stitcher/imclib/metadefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/mcd_stitcher/stitcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:15:15.410264 mcd_stitcher-0.1.0/mcd_stitcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-24 08:15:15.000000 mcd_stitcher-0.1.0/mcd_stitcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-24 08:15:15.000000 mcd_stitcher-0.1.0/mcd_stitcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:15:15.000000 mcd_stitcher-0.1.0/mcd_stitcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-24 08:15:15.000000 mcd_stitcher-0.1.0/mcd_stitcher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 08:15:15.000000 mcd_stitcher-0.1.0/mcd_stitcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 08:15:15.000000 mcd_stitcher-0.1.0/mcd_stitcher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 08:15:10.000000 mcd_stitcher-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-24 08:15:15.410264 mcd_stitcher-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/mcd_stitcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/mcd_stitcher/imclib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/imcdataparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/imcraw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdxmlparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/imclib/metadefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/mcd_stitcher/stitcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 17:07:54.000000 mcd_stitcher-0.1.1/mcd_stitcher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 17:07:54.688343 mcd_stitcher-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-24 17:07:45.000000 mcd_stitcher-0.1.1/setup.py
```

### Comparing `mcd_stitcher-0.1.0/LICENSE` & `mcd_stitcher-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.0/PKG-INFO` & `mcd_stitcher-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: mcd_stitcher
-Version: 0.1.0
+Version: 0.1.1
 Summary: MCD to Zarr conversion and stitching
 Home-page: https://github.com/PawanChaurasia/mcd_stitcher
 Author: Pawan Chaurasia
-Author-email: "pchaurasia98@gmail.com"
+Author-email: pchaurasia98@gmail.com
 Project-URL: Bug Tracker, https://github.com/PawanChaurasia/mcd_stitcher/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: python_dateutil
 Requires-Dist: xarray
 Requires-Dist: zarr
+Requires-Dist: scikit-image
 
 # MCD STITCHER
 
 Stitch rois from MCD files into OME-TIFFS.
 
 ## Install
 
@@ -33,28 +34,28 @@
 
 * click
 * numpy
 * pandas
 * python_dateutil
 * xarray
 * zarr
+* scikit-image
 
 ## Command line usage
 
 *MCD to Zarr converter
-]
+
 imc2zarr <mcd_folder> <zarr_folder>
 
 *Zarr dataset stitcher
 
 zarr_stitch <zarr_folder>
 
 *Composite MCD to Zarr to Stitch function
 
 mcd_stitch <mcd_folder> <zarr_folder>
 
 ### Arguments
 * mcd_folder:
-  * the root folder of the IMC scan containing a single and/or multiple mcd files.
-  
+  * The root folder of the IMC scan containing a single and/or multiple mcd files.
 * zarr_folder: 
-	*Storage location of converted MCD files in Zarr format and the starting point for stitching zarr files.
+  * Storage location of converted MCD files in Zarr format and the starting point for stitching zarr files.
```

### Comparing `mcd_stitcher-0.1.0/mcd_stitcher/__init__.py` & `mcd_stitcher-0.1.1/mcd_stitcher/__init__.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.0/mcd_stitcher/converter.py` & `mcd_stitcher-0.1.1/mcd_stitcher/converter.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.0/mcd_stitcher/imclib/imcdataparser.py` & `mcd_stitcher-0.1.1/mcd_stitcher/imclib/imcdataparser.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.0/mcd_stitcher/imclib/imcraw.py` & `mcd_stitcher-0.1.1/mcd_stitcher/imclib/imcraw.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.0/mcd_stitcher/imclib/mcdmeta.py` & `mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdmeta.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.0/mcd_stitcher/imclib/mcdutils.py` & `mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdutils.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.0/mcd_stitcher/imclib/mcdxmlparser.py` & `mcd_stitcher-0.1.1/mcd_stitcher/imclib/mcdxmlparser.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.0/mcd_stitcher/imclib/metadefs.py` & `mcd_stitcher-0.1.1/mcd_stitcher/imclib/metadefs.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.0/mcd_stitcher/stitcher.py` & `mcd_stitcher-0.1.1/mcd_stitcher/stitcher.py`

 * *Files identical despite different names*

### Comparing `mcd_stitcher-0.1.0/mcd_stitcher.egg-info/PKG-INFO` & `mcd_stitcher-0.1.1/mcd_stitcher.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: mcd_stitcher
-Version: 0.1.0
+Version: 0.1.1
 Summary: MCD to Zarr conversion and stitching
 Home-page: https://github.com/PawanChaurasia/mcd_stitcher
 Author: Pawan Chaurasia
-Author-email: "pchaurasia98@gmail.com"
+Author-email: pchaurasia98@gmail.com
 Project-URL: Bug Tracker, https://github.com/PawanChaurasia/mcd_stitcher/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: python_dateutil
 Requires-Dist: xarray
 Requires-Dist: zarr
+Requires-Dist: scikit-image
 
 # MCD STITCHER
 
 Stitch rois from MCD files into OME-TIFFS.
 
 ## Install
 
@@ -33,28 +34,28 @@
 
 * click
 * numpy
 * pandas
 * python_dateutil
 * xarray
 * zarr
+* scikit-image
 
 ## Command line usage
 
 *MCD to Zarr converter
-]
+
 imc2zarr <mcd_folder> <zarr_folder>
 
 *Zarr dataset stitcher
 
 zarr_stitch <zarr_folder>
 
 *Composite MCD to Zarr to Stitch function
 
 mcd_stitch <mcd_folder> <zarr_folder>
 
 ### Arguments
 * mcd_folder:
-  * the root folder of the IMC scan containing a single and/or multiple mcd files.
-  
+  * The root folder of the IMC scan containing a single and/or multiple mcd files.
 * zarr_folder: 
-	*Storage location of converted MCD files in Zarr format and the starting point for stitching zarr files.
+  * Storage location of converted MCD files in Zarr format and the starting point for stitching zarr files.
```

### Comparing `mcd_stitcher-0.1.0/mcd_stitcher.egg-info/SOURCES.txt` & `mcd_stitcher-0.1.1/mcd_stitcher.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
+setup.py
 mcd_stitcher/__init__.py
 mcd_stitcher/converter.py
 mcd_stitcher/stitcher.py
 mcd_stitcher.egg-info/PKG-INFO
 mcd_stitcher.egg-info/SOURCES.txt
 mcd_stitcher.egg-info/dependency_links.txt
 mcd_stitcher.egg-info/entry_points.txt
```

