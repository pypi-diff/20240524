# Comparing `tmp/iftaixpath-0.0.1.tar.gz` & `tmp/iftaixpath-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iftaixpath-0.0.1.tar", last modified: Fri May 24 16:45:36 2024, max compression
+gzip compressed data, was "iftaixpath-0.0.2.tar", last modified: Fri May 24 16:47:08 2024, max compression
```

## Comparing `iftaixpath-0.0.1.tar` & `iftaixpath-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 16:45:36.715439 iftaixpath-0.0.1/
--rw-rw-rw-   0        0        0        0 2024-05-24 07:35:28.000000 iftaixpath-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      122 2024-05-24 07:35:28.000000 iftaixpath-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2265 2024-05-24 16:45:36.714438 iftaixpath-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1760 2024-05-24 07:35:28.000000 iftaixpath-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 16:45:36.689338 iftaixpath-0.0.1/ift4aixpath/
--rw-rw-rw-   0        0        0    12049 2024-05-24 16:44:43.000000 iftaixpath-0.0.1/ift4aixpath/IFTBOM.py
--rw-rw-rw-   0        0        0    20118 2024-05-24 07:35:36.000000 iftaixpath-0.0.1/ift4aixpath/IFTBase.py
--rw-rw-rw-   0        0        0     6638 2024-05-24 16:44:41.000000 iftaixpath-0.0.1/ift4aixpath/IFTMachine.py
--rw-rw-rw-   0        0        0     6299 2024-05-24 16:44:40.000000 iftaixpath-0.0.1/ift4aixpath/IFTMachiningFeature.py
--rw-rw-rw-   0        0        0     7844 2024-05-24 16:44:39.000000 iftaixpath-0.0.1/ift4aixpath/IFTMachiningPart.py
--rw-rw-rw-   0        0        0    61394 2024-05-24 16:44:38.000000 iftaixpath-0.0.1/ift4aixpath/IFTOperation.py
--rw-rw-rw-   0        0        0     8315 2024-05-24 16:44:37.000000 iftaixpath-0.0.1/ift4aixpath/IFTPDF.py
--rw-rw-rw-   0        0        0     9559 2024-05-24 16:44:36.000000 iftaixpath-0.0.1/ift4aixpath/IFTPmi.py
--rw-rw-rw-   0        0        0    12475 2024-05-24 16:44:34.000000 iftaixpath-0.0.1/ift4aixpath/IFTTool.py
--rw-rw-rw-   0        0        0      259 2024-05-24 07:35:36.000000 iftaixpath-0.0.1/ift4aixpath/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 16:45:36.693436 iftaixpath-0.0.1/ift4aixpath/build/
--rw-rw-rw-   0        0        0      119 2024-05-24 07:35:36.000000 iftaixpath-0.0.1/ift4aixpath/build/cut_number_0.csv
--rw-rw-rw-   0        0        0      495 2024-05-24 07:35:36.000000 iftaixpath-0.0.1/ift4aixpath/build/intersection_points_0.csv
--rw-rw-rw-   0        0        0     3522 2024-05-24 07:35:36.000000 iftaixpath-0.0.1/ift4aixpath/build/points_of_ipw_0.csv
--rw-rw-rw-   0        0        0      990 2024-05-24 07:35:36.000000 iftaixpath-0.0.1/ift4aixpath/build/toolpath_points_0.csv
-drwxrwxrwx   0        0        0        0 2024-05-24 16:45:36.698437 iftaixpath-0.0.1/ift4aixpath/static/
--rw-rw-rw-   0        0        0   461745 2024-05-24 07:35:36.000000 iftaixpath-0.0.1/ift4aixpath/static/A4_template_cam_setup.prt
--rw-rw-rw-   0        0        0   469819 2024-05-24 07:35:36.000000 iftaixpath-0.0.1/ift4aixpath/static/A4_template_part.prt
--rw-rw-rw-   0        0        0      180 2024-05-24 07:35:36.000000 iftaixpath-0.0.1/ift4aixpath/static/configuration.json
--rw-rw-rw-   0        0        0     1938 2024-05-24 07:35:36.000000 iftaixpath-0.0.1/ift4aixpath/static/featuretypes.txt
--rw-rw-rw-   0        0        0      192 2024-05-24 07:35:36.000000 iftaixpath-0.0.1/ift4aixpath/static/tool_ug_type_map.json
-drwxrwxrwx   0        0        0        0 2024-05-24 16:45:36.714438 iftaixpath-0.0.1/iftaixpath.egg-info/
--rw-rw-rw-   0        0        0     2265 2024-05-24 16:45:36.000000 iftaixpath-0.0.1/iftaixpath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2024-05-24 16:45:36.000000 iftaixpath-0.0.1/iftaixpath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 16:45:36.000000 iftaixpath-0.0.1/iftaixpath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-24 16:45:36.000000 iftaixpath-0.0.1/iftaixpath.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-24 16:45:36.000000 iftaixpath-0.0.1/iftaixpath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 16:45:36.715439 iftaixpath-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      912 2024-05-24 16:43:17.000000 iftaixpath-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:47:08.667797 iftaixpath-0.0.2/
+-rw-rw-rw-   0        0        0        0 2024-05-24 07:35:28.000000 iftaixpath-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      122 2024-05-24 07:35:28.000000 iftaixpath-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2265 2024-05-24 16:47:08.666801 iftaixpath-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1760 2024-05-24 07:35:28.000000 iftaixpath-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 16:47:08.638796 iftaixpath-0.0.2/iftaixpath/
+-rw-rw-rw-   0        0        0    12049 2024-05-24 16:44:43.000000 iftaixpath-0.0.2/iftaixpath/IFTBOM.py
+-rw-rw-rw-   0        0        0    20118 2024-05-24 07:35:36.000000 iftaixpath-0.0.2/iftaixpath/IFTBase.py
+-rw-rw-rw-   0        0        0     6638 2024-05-24 16:44:41.000000 iftaixpath-0.0.2/iftaixpath/IFTMachine.py
+-rw-rw-rw-   0        0        0     6299 2024-05-24 16:44:40.000000 iftaixpath-0.0.2/iftaixpath/IFTMachiningFeature.py
+-rw-rw-rw-   0        0        0     7844 2024-05-24 16:44:39.000000 iftaixpath-0.0.2/iftaixpath/IFTMachiningPart.py
+-rw-rw-rw-   0        0        0    61394 2024-05-24 16:44:38.000000 iftaixpath-0.0.2/iftaixpath/IFTOperation.py
+-rw-rw-rw-   0        0        0     8315 2024-05-24 16:44:37.000000 iftaixpath-0.0.2/iftaixpath/IFTPDF.py
+-rw-rw-rw-   0        0        0     9559 2024-05-24 16:44:36.000000 iftaixpath-0.0.2/iftaixpath/IFTPmi.py
+-rw-rw-rw-   0        0        0    12475 2024-05-24 16:44:34.000000 iftaixpath-0.0.2/iftaixpath/IFTTool.py
+-rw-rw-rw-   0        0        0      259 2024-05-24 07:35:36.000000 iftaixpath-0.0.2/iftaixpath/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:47:08.660798 iftaixpath-0.0.2/iftaixpath/build/
+-rw-rw-rw-   0        0        0      119 2024-05-24 07:35:36.000000 iftaixpath-0.0.2/iftaixpath/build/cut_number_0.csv
+-rw-rw-rw-   0        0        0      495 2024-05-24 07:35:36.000000 iftaixpath-0.0.2/iftaixpath/build/intersection_points_0.csv
+-rw-rw-rw-   0        0        0     3522 2024-05-24 07:35:36.000000 iftaixpath-0.0.2/iftaixpath/build/points_of_ipw_0.csv
+-rw-rw-rw-   0        0        0      990 2024-05-24 07:35:36.000000 iftaixpath-0.0.2/iftaixpath/build/toolpath_points_0.csv
+drwxrwxrwx   0        0        0        0 2024-05-24 16:47:08.665799 iftaixpath-0.0.2/iftaixpath/static/
+-rw-rw-rw-   0        0        0   461745 2024-05-24 07:35:36.000000 iftaixpath-0.0.2/iftaixpath/static/A4_template_cam_setup.prt
+-rw-rw-rw-   0        0        0   469819 2024-05-24 07:35:36.000000 iftaixpath-0.0.2/iftaixpath/static/A4_template_part.prt
+-rw-rw-rw-   0        0        0      180 2024-05-24 07:35:36.000000 iftaixpath-0.0.2/iftaixpath/static/configuration.json
+-rw-rw-rw-   0        0        0     1938 2024-05-24 07:35:36.000000 iftaixpath-0.0.2/iftaixpath/static/featuretypes.txt
+-rw-rw-rw-   0        0        0      192 2024-05-24 07:35:36.000000 iftaixpath-0.0.2/iftaixpath/static/tool_ug_type_map.json
+drwxrwxrwx   0        0        0        0 2024-05-24 16:47:08.657885 iftaixpath-0.0.2/iftaixpath.egg-info/
+-rw-rw-rw-   0        0        0     2265 2024-05-24 16:47:08.000000 iftaixpath-0.0.2/iftaixpath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      802 2024-05-24 16:47:08.000000 iftaixpath-0.0.2/iftaixpath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 16:47:08.000000 iftaixpath-0.0.2/iftaixpath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-24 16:47:08.000000 iftaixpath-0.0.2/iftaixpath.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-24 16:47:08.000000 iftaixpath-0.0.2/iftaixpath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 16:47:08.667797 iftaixpath-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      912 2024-05-24 16:46:47.000000 iftaixpath-0.0.2/setup.py
```

### Comparing `iftaixpath-0.0.1/PKG-INFO` & `iftaixpath-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iftaixpath
-Version: 0.0.1
+Version: 0.0.2
 Summary: IFT-DBMS PyPi Version
 Home-page: https://git.ift.tuwien.ac.at/lab/ift/sis/data-science/nxopen-export/-/tree/lea?ref_type=heads
 Author-email: julian.zulehner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `iftaixpath-0.0.1/README.md` & `iftaixpath-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/IFTBOM.py` & `iftaixpath-0.0.2/iftaixpath/IFTBOM.py`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/IFTBase.py` & `iftaixpath-0.0.2/iftaixpath/IFTBase.py`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/IFTMachine.py` & `iftaixpath-0.0.2/iftaixpath/IFTMachine.py`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/IFTMachiningFeature.py` & `iftaixpath-0.0.2/iftaixpath/IFTMachiningFeature.py`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/IFTMachiningPart.py` & `iftaixpath-0.0.2/iftaixpath/IFTMachiningPart.py`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/IFTOperation.py` & `iftaixpath-0.0.2/iftaixpath/IFTOperation.py`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/IFTPDF.py` & `iftaixpath-0.0.2/iftaixpath/IFTPDF.py`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/IFTPmi.py` & `iftaixpath-0.0.2/iftaixpath/IFTPmi.py`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/IFTTool.py` & `iftaixpath-0.0.2/iftaixpath/IFTTool.py`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/build/points_of_ipw_0.csv` & `iftaixpath-0.0.2/iftaixpath/build/points_of_ipw_0.csv`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/build/toolpath_points_0.csv` & `iftaixpath-0.0.2/iftaixpath/build/toolpath_points_0.csv`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/static/A4_template_cam_setup.prt` & `iftaixpath-0.0.2/iftaixpath/static/A4_template_cam_setup.prt`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/static/A4_template_part.prt` & `iftaixpath-0.0.2/iftaixpath/static/A4_template_part.prt`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/ift4aixpath/static/featuretypes.txt` & `iftaixpath-0.0.2/iftaixpath/static/featuretypes.txt`

 * *Files identical despite different names*

### Comparing `iftaixpath-0.0.1/iftaixpath.egg-info/PKG-INFO` & `iftaixpath-0.0.2/iftaixpath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iftaixpath
-Version: 0.0.1
+Version: 0.0.2
 Summary: IFT-DBMS PyPi Version
 Home-page: https://git.ift.tuwien.ac.at/lab/ift/sis/data-science/nxopen-export/-/tree/lea?ref_type=heads
 Author-email: julian.zulehner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `iftaixpath-0.0.1/setup.py` & `iftaixpath-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="iftaixpath",
-    version="0.0.1",
+    version="0.0.2",
     authors="Lea Tonejca, Julian Zulehner",
     author_email="julian.zulehner@gmail.com",
     description="IFT-DBMS PyPi Version",
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     url="https://git.ift.tuwien.ac.at/lab/ift/sis/data-science/nxopen-export/-/tree/lea?ref_type=heads",
     packages=find_packages(),
```

