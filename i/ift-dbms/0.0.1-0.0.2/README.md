# Comparing `tmp/ift-dbms-0.0.1.tar.gz` & `tmp/ift-dbms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ift-dbms-0.0.1.tar", last modified: Fri May 24 14:41:48 2024, max compression
+gzip compressed data, was "ift-dbms-0.0.2.tar", last modified: Fri May 24 16:00:45 2024, max compression
```

## Comparing `ift-dbms-0.0.1.tar` & `ift-dbms-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 14:41:48.404738 ift-dbms-0.0.1/
--rw-rw-rw-   0        0        0        0 2024-05-24 07:35:28.000000 ift-dbms-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      122 2024-05-24 07:35:28.000000 ift-dbms-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2263 2024-05-24 14:41:48.404738 ift-dbms-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1760 2024-05-24 07:35:28.000000 ift-dbms-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 14:41:48.329486 ift-dbms-0.0.1/ift-dbms/
--rw-rw-rw-   0        0        0    12047 2024-05-24 14:36:30.000000 ift-dbms-0.0.1/ift-dbms/IFTBOM.py
--rw-rw-rw-   0        0        0    20118 2024-05-24 07:35:36.000000 ift-dbms-0.0.1/ift-dbms/IFTBase.py
--rw-rw-rw-   0        0        0     6631 2024-05-24 14:36:32.000000 ift-dbms-0.0.1/ift-dbms/IFTMachine.py
--rw-rw-rw-   0        0        0     6297 2024-05-24 14:36:33.000000 ift-dbms-0.0.1/ift-dbms/IFTMachiningFeature.py
--rw-rw-rw-   0        0        0     7842 2024-05-24 14:36:34.000000 ift-dbms-0.0.1/ift-dbms/IFTMachiningPart.py
--rw-rw-rw-   0        0        0    61388 2024-05-24 14:36:59.000000 ift-dbms-0.0.1/ift-dbms/IFTOperation.py
--rw-rw-rw-   0        0        0     8309 2024-05-24 14:37:23.000000 ift-dbms-0.0.1/ift-dbms/IFTPDF.py
--rw-rw-rw-   0        0        0     9555 2024-05-24 14:37:37.000000 ift-dbms-0.0.1/ift-dbms/IFTPmi.py
--rw-rw-rw-   0        0        0    12473 2024-05-24 14:37:43.000000 ift-dbms-0.0.1/ift-dbms/IFTTool.py
--rw-rw-rw-   0        0        0      259 2024-05-24 07:35:36.000000 ift-dbms-0.0.1/ift-dbms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 14:41:48.350618 ift-dbms-0.0.1/ift-dbms/build/
--rw-rw-rw-   0        0        0      119 2024-05-24 07:35:36.000000 ift-dbms-0.0.1/ift-dbms/build/cut_number_0.csv
--rw-rw-rw-   0        0        0      495 2024-05-24 07:35:36.000000 ift-dbms-0.0.1/ift-dbms/build/intersection_points_0.csv
--rw-rw-rw-   0        0        0     3522 2024-05-24 07:35:36.000000 ift-dbms-0.0.1/ift-dbms/build/points_of_ipw_0.csv
--rw-rw-rw-   0        0        0      990 2024-05-24 07:35:36.000000 ift-dbms-0.0.1/ift-dbms/build/toolpath_points_0.csv
-drwxrwxrwx   0        0        0        0 2024-05-24 14:41:48.377757 ift-dbms-0.0.1/ift-dbms/static/
--rw-rw-rw-   0        0        0   461745 2024-05-24 07:35:36.000000 ift-dbms-0.0.1/ift-dbms/static/A4_template_cam_setup.prt
--rw-rw-rw-   0        0        0   469819 2024-05-24 07:35:36.000000 ift-dbms-0.0.1/ift-dbms/static/A4_template_part.prt
--rw-rw-rw-   0        0        0      180 2024-05-24 07:35:36.000000 ift-dbms-0.0.1/ift-dbms/static/configuration.json
--rw-rw-rw-   0        0        0     1938 2024-05-24 07:35:36.000000 ift-dbms-0.0.1/ift-dbms/static/featuretypes.txt
--rw-rw-rw-   0        0        0      192 2024-05-24 07:35:36.000000 ift-dbms-0.0.1/ift-dbms/static/tool_ug_type_map.json
-drwxrwxrwx   0        0        0        0 2024-05-24 14:41:48.402737 ift-dbms-0.0.1/ift_dbms.egg-info/
--rw-rw-rw-   0        0        0     2263 2024-05-24 14:41:48.000000 ift-dbms-0.0.1/ift_dbms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      754 2024-05-24 14:41:48.000000 ift-dbms-0.0.1/ift_dbms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 14:41:48.000000 ift-dbms-0.0.1/ift_dbms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-24 14:41:48.000000 ift-dbms-0.0.1/ift_dbms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-24 14:41:48.000000 ift-dbms-0.0.1/ift_dbms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 14:41:48.404738 ift-dbms-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      973 2024-05-24 14:38:51.000000 ift-dbms-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:00:45.953924 ift-dbms-0.0.2/
+-rw-rw-rw-   0        0        0        0 2024-05-24 07:35:28.000000 ift-dbms-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      122 2024-05-24 07:35:28.000000 ift-dbms-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2263 2024-05-24 16:00:45.953924 ift-dbms-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1760 2024-05-24 07:35:28.000000 ift-dbms-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 16:00:45.882002 ift-dbms-0.0.2/ift-dbms/
+-rw-rw-rw-   0        0        0    12047 2024-05-24 14:36:30.000000 ift-dbms-0.0.2/ift-dbms/IFTBOM.py
+-rw-rw-rw-   0        0        0    20118 2024-05-24 07:35:36.000000 ift-dbms-0.0.2/ift-dbms/IFTBase.py
+-rw-rw-rw-   0        0        0     6631 2024-05-24 14:36:32.000000 ift-dbms-0.0.2/ift-dbms/IFTMachine.py
+-rw-rw-rw-   0        0        0     6297 2024-05-24 14:36:33.000000 ift-dbms-0.0.2/ift-dbms/IFTMachiningFeature.py
+-rw-rw-rw-   0        0        0     7842 2024-05-24 14:36:34.000000 ift-dbms-0.0.2/ift-dbms/IFTMachiningPart.py
+-rw-rw-rw-   0        0        0    61388 2024-05-24 14:36:59.000000 ift-dbms-0.0.2/ift-dbms/IFTOperation.py
+-rw-rw-rw-   0        0        0     8309 2024-05-24 14:37:23.000000 ift-dbms-0.0.2/ift-dbms/IFTPDF.py
+-rw-rw-rw-   0        0        0     9555 2024-05-24 14:37:37.000000 ift-dbms-0.0.2/ift-dbms/IFTPmi.py
+-rw-rw-rw-   0        0        0    12473 2024-05-24 14:37:43.000000 ift-dbms-0.0.2/ift-dbms/IFTTool.py
+-rw-rw-rw-   0        0        0      259 2024-05-24 07:35:36.000000 ift-dbms-0.0.2/ift-dbms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 16:00:45.902414 ift-dbms-0.0.2/ift-dbms/build/
+-rw-rw-rw-   0        0        0      119 2024-05-24 07:35:36.000000 ift-dbms-0.0.2/ift-dbms/build/cut_number_0.csv
+-rw-rw-rw-   0        0        0      495 2024-05-24 07:35:36.000000 ift-dbms-0.0.2/ift-dbms/build/intersection_points_0.csv
+-rw-rw-rw-   0        0        0     3522 2024-05-24 07:35:36.000000 ift-dbms-0.0.2/ift-dbms/build/points_of_ipw_0.csv
+-rw-rw-rw-   0        0        0      990 2024-05-24 07:35:36.000000 ift-dbms-0.0.2/ift-dbms/build/toolpath_points_0.csv
+drwxrwxrwx   0        0        0        0 2024-05-24 16:00:45.931270 ift-dbms-0.0.2/ift-dbms/static/
+-rw-rw-rw-   0        0        0   461745 2024-05-24 07:35:36.000000 ift-dbms-0.0.2/ift-dbms/static/A4_template_cam_setup.prt
+-rw-rw-rw-   0        0        0   469819 2024-05-24 07:35:36.000000 ift-dbms-0.0.2/ift-dbms/static/A4_template_part.prt
+-rw-rw-rw-   0        0        0      180 2024-05-24 07:35:36.000000 ift-dbms-0.0.2/ift-dbms/static/configuration.json
+-rw-rw-rw-   0        0        0     1938 2024-05-24 07:35:36.000000 ift-dbms-0.0.2/ift-dbms/static/featuretypes.txt
+-rw-rw-rw-   0        0        0      192 2024-05-24 07:35:36.000000 ift-dbms-0.0.2/ift-dbms/static/tool_ug_type_map.json
+drwxrwxrwx   0        0        0        0 2024-05-24 16:00:45.952012 ift-dbms-0.0.2/ift_dbms.egg-info/
+-rw-rw-rw-   0        0        0     2263 2024-05-24 16:00:45.000000 ift-dbms-0.0.2/ift_dbms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      754 2024-05-24 16:00:45.000000 ift-dbms-0.0.2/ift_dbms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 16:00:45.000000 ift-dbms-0.0.2/ift_dbms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-24 16:00:45.000000 ift-dbms-0.0.2/ift_dbms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 16:00:45.000000 ift-dbms-0.0.2/ift_dbms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 16:00:45.953924 ift-dbms-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      910 2024-05-24 16:00:25.000000 ift-dbms-0.0.2/setup.py
```

### Comparing `ift-dbms-0.0.1/PKG-INFO` & `ift-dbms-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ift-dbms
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

### Comparing `ift-dbms-0.0.1/README.md` & `ift-dbms-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/IFTBOM.py` & `ift-dbms-0.0.2/ift-dbms/IFTBOM.py`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/IFTBase.py` & `ift-dbms-0.0.2/ift-dbms/IFTBase.py`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/IFTMachine.py` & `ift-dbms-0.0.2/ift-dbms/IFTMachine.py`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/IFTMachiningFeature.py` & `ift-dbms-0.0.2/ift-dbms/IFTMachiningFeature.py`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/IFTMachiningPart.py` & `ift-dbms-0.0.2/ift-dbms/IFTMachiningPart.py`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/IFTOperation.py` & `ift-dbms-0.0.2/ift-dbms/IFTOperation.py`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/IFTPDF.py` & `ift-dbms-0.0.2/ift-dbms/IFTPDF.py`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/IFTPmi.py` & `ift-dbms-0.0.2/ift-dbms/IFTPmi.py`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/IFTTool.py` & `ift-dbms-0.0.2/ift-dbms/IFTTool.py`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/build/points_of_ipw_0.csv` & `ift-dbms-0.0.2/ift-dbms/build/points_of_ipw_0.csv`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/build/toolpath_points_0.csv` & `ift-dbms-0.0.2/ift-dbms/build/toolpath_points_0.csv`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/static/A4_template_cam_setup.prt` & `ift-dbms-0.0.2/ift-dbms/static/A4_template_cam_setup.prt`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/static/A4_template_part.prt` & `ift-dbms-0.0.2/ift-dbms/static/A4_template_part.prt`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift-dbms/static/featuretypes.txt` & `ift-dbms-0.0.2/ift-dbms/static/featuretypes.txt`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/ift_dbms.egg-info/PKG-INFO` & `ift-dbms-0.0.2/ift_dbms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ift-dbms
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

### Comparing `ift-dbms-0.0.1/ift_dbms.egg-info/SOURCES.txt` & `ift-dbms-0.0.2/ift_dbms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ift-dbms-0.0.1/setup.py` & `ift-dbms-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="ift-dbms",
-    version="0.0.1",
+    version="0.0.2",
     authors="Lea Tonejca, Julian Zulehner",
     author_email="julian.zulehner@gmail.com",
     description="IFT-DBMS PyPi Version",
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     url="https://git.ift.tuwien.ac.at/lab/ift/sis/data-science/nxopen-export/-/tree/lea?ref_type=heads",
     packages=find_packages(),
     install_requires=[
-        'NXOpen',
-        'inspect',
-        'pathlib',
-        'statistics'
+        'NXOpen'
     ],        
     include_package_data=True,
     package_data={
         'ift-test': ['static/*.prt', 'static/*.csv', 'static/*.txt', 'static/*.json', 'build/*.csv']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

