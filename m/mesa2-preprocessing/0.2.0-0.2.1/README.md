# Comparing `tmp/mesa2_preprocessing-0.2.0.tar.gz` & `tmp/mesa2_preprocessing-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mesa2_preprocessing-0.2.0.tar", last modified: Thu May  9 08:53:26 2024, max compression
+gzip compressed data, was "mesa2_preprocessing-0.2.1.tar", last modified: Thu May  9 09:30:57 2024, max compression
```

## Comparing `mesa2_preprocessing-0.2.0.tar` & `mesa2_preprocessing-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 08:53:26.799644 mesa2_preprocessing-0.2.0/
--rw-rw-rw-   0        0        0     1091 2024-05-08 20:04:06.000000 mesa2_preprocessing-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1972 2024-05-09 08:53:26.796638 mesa2_preprocessing-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1107 2024-05-09 08:39:03.000000 mesa2_preprocessing-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 08:53:26.753004 mesa2_preprocessing-0.2.0/mesa2_preprocessing/
--rw-rw-rw-   0        0        0      165 2024-05-09 08:39:03.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing/__init__.py
--rw-rw-rw-   0        0        0    12019 2024-05-09 08:39:03.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing/operations.py
-drwxrwxrwx   0        0        0        0 2024-05-09 08:53:26.793626 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/
--rw-rw-rw-   0        0        0     1972 2024-05-09 08:53:26.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-05-09 08:53:26.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 08:53:26.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-09 08:53:26.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-09 08:53:26.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 08:53:26.800637 mesa2_preprocessing-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1081 2024-05-09 08:53:15.000000 mesa2_preprocessing-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:30:57.766041 mesa2_preprocessing-0.2.1/
+-rw-rw-rw-   0        0        0     1091 2024-05-08 20:04:06.000000 mesa2_preprocessing-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2060 2024-05-09 09:30:57.763041 mesa2_preprocessing-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1133 2024-05-09 09:29:06.000000 mesa2_preprocessing-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 09:30:57.724961 mesa2_preprocessing-0.2.1/mesa2_preprocessing/
+-rw-rw-rw-   0        0        0      165 2024-05-09 08:39:03.000000 mesa2_preprocessing-0.2.1/mesa2_preprocessing/__init__.py
+-rw-rw-rw-   0        0        0    12019 2024-05-09 08:39:03.000000 mesa2_preprocessing-0.2.1/mesa2_preprocessing/operations.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:30:57.760013 mesa2_preprocessing-0.2.1/mesa2_preprocessing.egg-info/
+-rw-rw-rw-   0        0        0     2060 2024-05-09 09:30:57.000000 mesa2_preprocessing-0.2.1/mesa2_preprocessing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-09 09:30:57.000000 mesa2_preprocessing-0.2.1/mesa2_preprocessing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 09:30:57.000000 mesa2_preprocessing-0.2.1/mesa2_preprocessing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-09 09:30:57.000000 mesa2_preprocessing-0.2.1/mesa2_preprocessing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-09 09:30:57.000000 mesa2_preprocessing-0.2.1/mesa2_preprocessing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 09:30:57.766041 mesa2_preprocessing-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2024-05-09 09:29:06.000000 mesa2_preprocessing-0.2.1/setup.py
```

### Comparing `mesa2_preprocessing-0.2.0/LICENSE` & `mesa2_preprocessing-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mesa2_preprocessing-0.2.0/PKG-INFO` & `mesa2_preprocessing-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mesa2_preprocessing
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool for pre-processing MESA2.0 measurement data
 Author: Nadir Nadirov
 Author-email: nadirnadirov1999@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -16,14 +16,16 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.0
 Requires-Dist: numpy>=1.18
 Requires-Dist: nptdms>=0.25
+Requires-Dist: pyarrow>=4.0
+Requires-Dist: fastparquet>=0.6
 
 # MESA2.0 Preprocessing Tool
 
 This package provides a set of tools designed for pre-processing MESA2.0 measurement data. It includes functionality to read, merge, and process measurement data efficiently.
 
 ## Features
 - Read data from `.dat` and associated binary files.
@@ -50,12 +52,14 @@
 # Create a merged TDMS file from DAT and TDMS sources
 create_merged_tdms('path_to_your_tdms_file.tdms', 'path_to_your_dat_file.dat', 'output_directory')
 ```
 ## Dependencies
 
 - Python >= 3.8
 - pandas
+- pyarrow
+- fastparquet
 - numpy
 - nptdms
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `mesa2_preprocessing-0.2.0/README.md` & `mesa2_preprocessing-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,12 +27,14 @@
 # Create a merged TDMS file from DAT and TDMS sources
 create_merged_tdms('path_to_your_tdms_file.tdms', 'path_to_your_dat_file.dat', 'output_directory')
 ```
 ## Dependencies
 
 - Python >= 3.8
 - pandas
+- pyarrow
+- fastparquet
 - numpy
 - nptdms
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `mesa2_preprocessing-0.2.0/mesa2_preprocessing/operations.py` & `mesa2_preprocessing-0.2.1/mesa2_preprocessing/operations.py`

 * *Files identical despite different names*

### Comparing `mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/PKG-INFO` & `mesa2_preprocessing-0.2.1/mesa2_preprocessing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mesa2-preprocessing
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool for pre-processing MESA2.0 measurement data
 Author: Nadir Nadirov
 Author-email: nadirnadirov1999@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -16,14 +16,16 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.0
 Requires-Dist: numpy>=1.18
 Requires-Dist: nptdms>=0.25
+Requires-Dist: pyarrow>=4.0
+Requires-Dist: fastparquet>=0.6
 
 # MESA2.0 Preprocessing Tool
 
 This package provides a set of tools designed for pre-processing MESA2.0 measurement data. It includes functionality to read, merge, and process measurement data efficiently.
 
 ## Features
 - Read data from `.dat` and associated binary files.
@@ -50,12 +52,14 @@
 # Create a merged TDMS file from DAT and TDMS sources
 create_merged_tdms('path_to_your_tdms_file.tdms', 'path_to_your_dat_file.dat', 'output_directory')
 ```
 ## Dependencies
 
 - Python >= 3.8
 - pandas
+- pyarrow
+- fastparquet
 - numpy
 - nptdms
 
 ## License
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `mesa2_preprocessing-0.2.0/setup.py` & `mesa2_preprocessing-0.2.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mesa2_preprocessing',
-    version='0.2.0',
+    version='0.2.1',
     author='Nadir Nadirov',
     author_email='nadirnadirov1999@gmail.com',
     description='A tool for pre-processing MESA2.0 measurement data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'pandas>=1.0',
         'numpy>=1.18',
-        'nptdms>=0.25'
+        'nptdms>=0.25',
+        'pyarrow>=4.0',
+        'fastparquet>=0.6'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',  # Ensure this matches your chosen license
+        'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering :: Visualization'
```

