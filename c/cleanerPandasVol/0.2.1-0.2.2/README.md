# Comparing `tmp/cleanerpandasvol-0.2.1.tar.gz` & `tmp/cleanerpandasvol-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanerpandasvol-0.2.1.tar", last modified: Fri May 24 11:11:39 2024, max compression
+gzip compressed data, was "cleanerpandasvol-0.2.2.tar", last modified: Fri May 24 11:25:10 2024, max compression
```

## Comparing `cleanerpandasvol-0.2.1.tar` & `cleanerpandasvol-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 11:11:39.783670 cleanerpandasvol-0.2.1/
--rw-rw-rw-   0        0        0     1082 2024-05-21 11:41:29.000000 cleanerpandasvol-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      595 2024-05-24 11:11:39.781608 cleanerpandasvol-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-24 11:11:39.734563 cleanerpandasvol-0.2.1/cleanerPandasVol/
--rw-rw-rw-   0        0        0      579 2024-05-22 12:28:48.000000 cleanerpandasvol-0.2.1/cleanerPandasVol/__init__.py
--rw-rw-rw-   0        0        0      694 2024-05-21 08:54:01.000000 cleanerpandasvol-0.2.1/cleanerPandasVol/categorical_encoder.py
--rw-rw-rw-   0        0        0      433 2024-05-21 08:54:44.000000 cleanerpandasvol-0.2.1/cleanerPandasVol/data_type_converter.py
--rw-rw-rw-   0        0        0      618 2024-05-24 11:11:06.000000 cleanerpandasvol-0.2.1/cleanerPandasVol/date_time_handler.py
--rw-rw-rw-   0        0        0      433 2024-05-21 08:56:02.000000 cleanerpandasvol-0.2.1/cleanerPandasVol/feature_engineer.py
--rw-rw-rw-   0        0        0      847 2024-05-21 08:56:30.000000 cleanerpandasvol-0.2.1/cleanerPandasVol/missing_value_handler.py
--rw-rw-rw-   0        0        0     1364 2024-05-21 08:56:56.000000 cleanerpandasvol-0.2.1/cleanerPandasVol/outlier_handler.py
--rw-rw-rw-   0        0        0      419 2024-05-21 08:57:27.000000 cleanerpandasvol-0.2.1/cleanerPandasVol/scaler.py
--rw-rw-rw-   0        0        0     1202 2024-05-23 17:52:43.000000 cleanerpandasvol-0.2.1/cleanerPandasVol/text_cleaner.py
-drwxrwxrwx   0        0        0        0 2024-05-24 11:11:39.777834 cleanerpandasvol-0.2.1/cleanerPandasVol.egg-info/
--rw-rw-rw-   0        0        0      595 2024-05-24 11:11:39.000000 cleanerpandasvol-0.2.1/cleanerPandasVol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2024-05-24 11:11:39.000000 cleanerpandasvol-0.2.1/cleanerPandasVol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 11:11:39.000000 cleanerpandasvol-0.2.1/cleanerPandasVol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-24 11:11:39.000000 cleanerpandasvol-0.2.1/cleanerPandasVol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-24 11:11:39.000000 cleanerpandasvol-0.2.1/cleanerPandasVol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 11:11:39.784668 cleanerpandasvol-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      716 2024-05-24 11:11:31.000000 cleanerpandasvol-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 11:11:39.773840 cleanerpandasvol-0.2.1/test/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:03:34.000000 cleanerpandasvol-0.2.1/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:25:10.489009 cleanerpandasvol-0.2.2/
+-rw-rw-rw-   0        0        0     1082 2024-05-21 11:41:29.000000 cleanerpandasvol-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      595 2024-05-24 11:25:10.485655 cleanerpandasvol-0.2.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 11:25:10.443647 cleanerpandasvol-0.2.2/cleanerPandasVol/
+-rw-rw-rw-   0        0        0      579 2024-05-22 12:28:48.000000 cleanerpandasvol-0.2.2/cleanerPandasVol/__init__.py
+-rw-rw-rw-   0        0        0      694 2024-05-21 08:54:01.000000 cleanerpandasvol-0.2.2/cleanerPandasVol/categorical_encoder.py
+-rw-rw-rw-   0        0        0      433 2024-05-21 08:54:44.000000 cleanerpandasvol-0.2.2/cleanerPandasVol/data_type_converter.py
+-rw-rw-rw-   0        0        0      524 2024-05-24 11:25:03.000000 cleanerpandasvol-0.2.2/cleanerPandasVol/date_time_handler.py
+-rw-rw-rw-   0        0        0      433 2024-05-21 08:56:02.000000 cleanerpandasvol-0.2.2/cleanerPandasVol/feature_engineer.py
+-rw-rw-rw-   0        0        0      847 2024-05-21 08:56:30.000000 cleanerpandasvol-0.2.2/cleanerPandasVol/missing_value_handler.py
+-rw-rw-rw-   0        0        0     1364 2024-05-21 08:56:56.000000 cleanerpandasvol-0.2.2/cleanerPandasVol/outlier_handler.py
+-rw-rw-rw-   0        0        0      419 2024-05-21 08:57:27.000000 cleanerpandasvol-0.2.2/cleanerPandasVol/scaler.py
+-rw-rw-rw-   0        0        0     1202 2024-05-23 17:52:43.000000 cleanerpandasvol-0.2.2/cleanerPandasVol/text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:25:10.484336 cleanerpandasvol-0.2.2/cleanerPandasVol.egg-info/
+-rw-rw-rw-   0        0        0      595 2024-05-24 11:25:10.000000 cleanerpandasvol-0.2.2/cleanerPandasVol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2024-05-24 11:25:10.000000 cleanerpandasvol-0.2.2/cleanerPandasVol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 11:25:10.000000 cleanerpandasvol-0.2.2/cleanerPandasVol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-24 11:25:10.000000 cleanerpandasvol-0.2.2/cleanerPandasVol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-24 11:25:10.000000 cleanerpandasvol-0.2.2/cleanerPandasVol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 11:25:10.489230 cleanerpandasvol-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      716 2024-05-24 11:24:38.000000 cleanerpandasvol-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 11:25:10.482184 cleanerpandasvol-0.2.2/test/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:03:34.000000 cleanerpandasvol-0.2.2/test/__init__.py
```

### Comparing `cleanerpandasvol-0.2.1/LICENSE` & `cleanerpandasvol-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.2.1/PKG-INFO` & `cleanerpandasvol-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanerPandasVol
-Version: 0.2.1
+Version: 0.2.2
 Summary: A comprehensive Python library for data preprocessing and cleaning
 Home-page: https://github.com/MuratKeskin0/Python_Data_Project_Vol
 Author: Murat Keskin & Ahmet Bagbakan & Cagla Ilhani
 Author-email: eng.murat.keskin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cleanerpandasvol-0.2.1/cleanerPandasVol/__init__.py` & `cleanerpandasvol-0.2.2/cleanerPandasVol/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.2.1/cleanerPandasVol/categorical_encoder.py` & `cleanerpandasvol-0.2.2/cleanerPandasVol/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.2.1/cleanerPandasVol/missing_value_handler.py` & `cleanerpandasvol-0.2.2/cleanerPandasVol/missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.2.1/cleanerPandasVol/outlier_handler.py` & `cleanerpandasvol-0.2.2/cleanerPandasVol/outlier_handler.py`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.2.1/cleanerPandasVol/text_cleaner.py` & `cleanerpandasvol-0.2.2/cleanerPandasVol/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.2.1/cleanerPandasVol.egg-info/PKG-INFO` & `cleanerpandasvol-0.2.2/cleanerPandasVol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanerPandasVol
-Version: 0.2.1
+Version: 0.2.2
 Summary: A comprehensive Python library for data preprocessing and cleaning
 Home-page: https://github.com/MuratKeskin0/Python_Data_Project_Vol
 Author: Murat Keskin & Ahmet Bagbakan & Cagla Ilhani
 Author-email: eng.murat.keskin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cleanerpandasvol-0.2.1/cleanerPandasVol.egg-info/SOURCES.txt` & `cleanerpandasvol-0.2.2/cleanerPandasVol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.2.1/setup.py` & `cleanerpandasvol-0.2.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cleanerPandasVol',
-    version='0.2.1',
+    version='0.2.2',
     author='Murat Keskin & Ahmet Bagbakan & Cagla Ilhani',
     author_email='eng.murat.keskin@gmail.com',
     description='A comprehensive Python library for data preprocessing and cleaning',
     url='https://github.com/MuratKeskin0/Python_Data_Project_Vol',
     packages=find_packages(),
     install_requires=[
         'pandas',
```

