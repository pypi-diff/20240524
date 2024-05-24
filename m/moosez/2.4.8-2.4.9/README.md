# Comparing `tmp/moosez-2.4.8.tar.gz` & `tmp/moosez-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moosez-2.4.8.tar", last modified: Mon May  6 19:52:34 2024, max compression
+gzip compressed data, was "moosez-2.4.9.tar", last modified: Tue May  7 14:26:48 2024, max compression
```

## Comparing `moosez-2.4.8.tar` & `moosez-2.4.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:52:34.550170 moosez-2.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-06 19:52:30.000000 moosez-2.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-06 19:52:34.550170 moosez-2.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21366 2024-05-06 19:52:30.000000 moosez-2.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:52:34.546170 moosez-2.4.8/moosez/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/image_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    25528 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/input_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/moosez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:52:34.550170 moosez-2.4.8/moosez/nnUNet_custom_trainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/nnUNet_custom_trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/nnUNet_custom_trainer/utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    15482 2024-05-06 19:52:30.000000 moosez-2.4.8/moosez/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:52:34.550170 moosez-2.4.8/moosez.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-06 19:52:34.000000 moosez-2.4.8/moosez.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 19:52:34.550170 moosez-2.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-06 19:52:30.000000 moosez-2.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:48.285507 moosez-2.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 14:26:44.000000 moosez-2.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-07 14:26:48.285507 moosez-2.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21366 2024-05-07 14:26:44.000000 moosez-2.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:48.285507 moosez-2.4.9/moosez/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/image_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25528 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/moosez.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:48.285507 moosez-2.4.9/moosez/nnUNet_custom_trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/nnUNet_custom_trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/nnUNet_custom_trainer/utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15482 2024-05-07 14:26:44.000000 moosez-2.4.9/moosez/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:26:48.285507 moosez-2.4.9/moosez.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 14:26:48.000000 moosez-2.4.9/moosez.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:26:48.285507 moosez-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-07 14:26:44.000000 moosez-2.4.9/setup.py
```

### Comparing `moosez-2.4.8/LICENSE` & `moosez-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/PKG-INFO` & `moosez-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.8
+Version: 2.4.9
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/ENHANCE-PET/MOOSE
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.4.8/README.md` & `moosez-2.4.9/README.md`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez/constants.py` & `moosez-2.4.9/moosez/constants.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez/display.py` & `moosez-2.4.9/moosez/display.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez/download.py` & `moosez-2.4.9/moosez/download.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez/file_utilities.py` & `moosez-2.4.9/moosez/file_utilities.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez/image_conversion.py` & `moosez-2.4.9/moosez/image_conversion.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez/image_processing.py` & `moosez-2.4.9/moosez/image_processing.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez/input_validation.py` & `moosez-2.4.9/moosez/input_validation.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez/moosez.py` & `moosez-2.4.9/moosez/moosez.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                 os.path.isdir(os.path.join(parent_folder, d))]
     moose_compliant_subjects = input_validation.select_moose_compliant_subjects(subjects, modalities)
 
     num_subjects = len(moose_compliant_subjects)
 
     if num_subjects < 1:
         print(
-            f'{constants.ANSI_RED} {emoji.emojize(":cross_mark:")} No moose compliant subject found to continue!{constants.ANSI_RESET} {emoji.emojize(":light_bulb:")} See: https://github.com/QIMP-Team/MOOSE#directory-structure-and-naming-conventions-for-moose-%EF%B8%8F')
+            f'{constants.ANSI_RED} {emoji.emojize(":cross_mark:")} No moose compliant subject found to continue!{constants.ANSI_RESET} {emoji.emojize(":light_bulb:")} See: https://github.com/ENHANCE-PET/MOOSE#directory-structure-and-naming-conventions-for-moose-%EF%B8%8F')
         return
 
     # -------------------------------------------------
     # RUN PREDICTION ONLY FOR MOOSE COMPLIANT SUBJECTS
     # -------------------------------------------------
 
     print('')
```

### Comparing `moosez-2.4.8/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py` & `moosez-2.4.9/moosez/nnUNet_custom_trainer/MOOSE_custom_trainers.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez/nnUNet_custom_trainer/utility.py` & `moosez-2.4.9/moosez/nnUNet_custom_trainer/utility.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez/predict.py` & `moosez-2.4.9/moosez/predict.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez/resources.py` & `moosez-2.4.9/moosez/resources.py`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/moosez.egg-info/PKG-INFO` & `moosez-2.4.9/moosez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moosez
-Version: 2.4.8
+Version: 2.4.9
 Summary: An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks
 Home-page: https://github.com/ENHANCE-PET/MOOSE
 Author: Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer
 Author-email: Lalith.shiyamsundar@meduniwien.ac.at
 License: GPLv3
 Keywords: moosez model-zoo nnUNet medical-imaging tumor-segmentation organ-segmentation bone-segmentation lung-segmentation muscle-segmentation fat-segmentation vessel-segmentation vertebral-segmentation rib-segmentation preclinical-segmentation clinical-segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moosez-2.4.8/moosez.egg-info/SOURCES.txt` & `moosez-2.4.9/moosez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moosez-2.4.8/setup.py` & `moosez-2.4.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='moosez',
-    version='2.4.8',
+    version='2.4.9',
     author='Lalith Kumar Shiyam Sundar | Sebastian Gutschmayer',
     author_email='Lalith.shiyamsundar@meduniwien.ac.at',
     description='An AI-inference engine for 3D clinical and preclinical whole-body segmentation tasks',
     python_requires='>=3.10',
     long_description='mooseZ is an AI-inference engine based on nnUNet, designed for 3D clinical and preclinical'
                      ' whole-body segmentation tasks. It serves models tailored towards different modalities such'
                      ' as PET, CT, and MR. mooseZ provides fast and accurate segmentation results, making it a '
```

