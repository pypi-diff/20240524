# Comparing `tmp/visionai_data_format-1.3.4.tar.gz` & `tmp/visionai_data_format-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai_data_format-1.3.4.tar", last modified: Tue May 21 02:25:14 2024, max compression
+gzip compressed data, was "visionai_data_format-1.3.5.tar", last modified: Fri May 24 01:50:00 2024, max compression
```

## Comparing `visionai_data_format-1.3.4.tar` & `visionai_data_format-1.3.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:25:14.585808 visionai_data_format-1.3.4/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    25808 2024-05-21 02:25:14.585607 visionai_data_format-1.3.4/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    25408 2024-05-20 06:25:16.000000 visionai_data_format-1.3.4/README.md
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-05-21 02:25:14.585851 visionai_data_format-1.3.4/setup.cfg
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      763 2024-05-21 02:24:51.000000 visionai_data_format-1.3.4/setup.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:25:14.575997 visionai_data_format-1.3.4/tests/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2176 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/tests/test_schemas.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     8449 2024-02-06 03:21:26.000000 visionai_data_format-1.3.4/tests/test_validators.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:25:14.577011 visionai_data_format-1.3.4/visionai_data_format/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     7698 2024-05-20 06:25:16.000000 visionai_data_format-1.3.4/visionai_data_format/convert_dataset.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:25:14.579569 visionai_data_format-1.3.4/visionai_data_format/converters/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      206 2024-05-20 06:25:16.000000 visionai_data_format-1.3.4/visionai_data_format/converters/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1729 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/converters/base.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    16423 2024-03-19 09:51:26.000000 visionai_data_format-1.3.4/visionai_data_format/converters/bdd_to_vai.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     9405 2024-05-20 06:25:16.000000 visionai_data_format-1.3.4/visionai_data_format/converters/coco_to_vai.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    16685 2024-03-19 08:30:06.000000 visionai_data_format-1.3.4/visionai_data_format/converters/kitti_to_vai.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     9965 2024-05-21 02:24:51.000000 visionai_data_format-1.3.4/visionai_data_format/converters/vai_to_coco.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    10099 2024-05-20 06:25:16.000000 visionai_data_format-1.3.4/visionai_data_format/converters/yolo_to_vai.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:25:14.580577 visionai_data_format-1.3.4/visionai_data_format/exceptions/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      156 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/exceptions/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1405 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/exceptions/constants.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5564 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/exceptions/error_messages.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1322 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/exceptions/visionai.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:25:14.581760 visionai_data_format-1.3.4/visionai_data_format/schemas/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/schemas/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2586 2024-04-16 07:37:46.000000 visionai_data_format-1.3.4/visionai_data_format/schemas/bdd_schema.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      679 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/schemas/coco_schema.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1745 2024-05-20 06:25:16.000000 visionai_data_format-1.3.4/visionai_data_format/schemas/common.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      994 2024-04-16 08:33:06.000000 visionai_data_format-1.3.4/visionai_data_format/schemas/ontology.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:25:14.582341 visionai_data_format-1.3.4/visionai_data_format/schemas/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/schemas/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    50408 2024-04-16 07:40:00.000000 visionai_data_format-1.3.4/visionai_data_format/schemas/utils/validators.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    32093 2024-04-16 08:33:06.000000 visionai_data_format-1.3.4/visionai_data_format/schemas/visionai_schema.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:25:14.584901 visionai_data_format-1.3.4/visionai_data_format/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1692 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/utils/calculation.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    10506 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/utils/checker.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      761 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/utils/classes.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      593 2024-05-20 06:25:16.000000 visionai_data_format-1.3.4/visionai_data_format/utils/common.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     4571 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/utils/converter.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     4059 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/utils/resize.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     4588 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/utils/validator.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     2308 2023-12-21 03:02:35.000000 visionai_data_format-1.3.4/visionai_data_format/vai_to_bdd.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5917 2023-07-06 06:50:32.000000 visionai_data_format-1.3.4/visionai_data_format/vai_to_bdd_v2.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:25:14.585158 visionai_data_format-1.3.4/visionai_data_format.egg-info/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    25808 2024-05-21 02:25:14.000000 visionai_data_format-1.3.4/visionai_data_format.egg-info/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1595 2024-05-21 02:25:14.000000 visionai_data_format-1.3.4/visionai_data_format.egg-info/SOURCES.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-05-21 02:25:14.000000 visionai_data_format-1.3.4/visionai_data_format.egg-info/dependency_links.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       52 2024-05-21 02:25:14.000000 visionai_data_format-1.3.4/visionai_data_format.egg-info/requires.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       21 2024-05-21 02:25:14.000000 visionai_data_format-1.3.4/visionai_data_format.egg-info/top_level.txt
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-24 01:50:00.577090 visionai_data_format-1.3.5/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    25808 2024-05-24 01:50:00.576902 visionai_data_format-1.3.5/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    25408 2024-05-20 06:25:16.000000 visionai_data_format-1.3.5/README.md
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-05-24 01:50:00.577133 visionai_data_format-1.3.5/setup.cfg
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      763 2024-05-24 01:49:30.000000 visionai_data_format-1.3.5/setup.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-24 01:50:00.567384 visionai_data_format-1.3.5/tests/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     2176 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/tests/test_schemas.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     8449 2024-02-06 03:21:26.000000 visionai_data_format-1.3.5/tests/test_validators.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-24 01:50:00.568392 visionai_data_format-1.3.5/visionai_data_format/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     7698 2024-05-20 06:25:16.000000 visionai_data_format-1.3.5/visionai_data_format/convert_dataset.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-24 01:50:00.571066 visionai_data_format-1.3.5/visionai_data_format/converters/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      206 2024-05-20 06:25:16.000000 visionai_data_format-1.3.5/visionai_data_format/converters/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1729 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/converters/base.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    16423 2024-03-19 09:51:26.000000 visionai_data_format-1.3.5/visionai_data_format/converters/bdd_to_vai.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     9405 2024-05-20 06:25:16.000000 visionai_data_format-1.3.5/visionai_data_format/converters/coco_to_vai.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    16685 2024-03-19 08:30:06.000000 visionai_data_format-1.3.5/visionai_data_format/converters/kitti_to_vai.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     9995 2024-05-24 01:49:30.000000 visionai_data_format-1.3.5/visionai_data_format/converters/vai_to_coco.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    10099 2024-05-20 06:25:16.000000 visionai_data_format-1.3.5/visionai_data_format/converters/yolo_to_vai.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-24 01:50:00.572875 visionai_data_format-1.3.5/visionai_data_format/exceptions/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      156 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/exceptions/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1405 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/exceptions/constants.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5564 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/exceptions/error_messages.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1322 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/exceptions/visionai.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-24 01:50:00.574004 visionai_data_format-1.3.5/visionai_data_format/schemas/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/schemas/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     2586 2024-04-16 07:37:46.000000 visionai_data_format-1.3.5/visionai_data_format/schemas/bdd_schema.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      679 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/schemas/coco_schema.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1745 2024-05-20 06:25:16.000000 visionai_data_format-1.3.5/visionai_data_format/schemas/common.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      994 2024-04-16 08:33:06.000000 visionai_data_format-1.3.5/visionai_data_format/schemas/ontology.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-24 01:50:00.574653 visionai_data_format-1.3.5/visionai_data_format/schemas/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/schemas/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    50408 2024-04-16 07:40:00.000000 visionai_data_format-1.3.5/visionai_data_format/schemas/utils/validators.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    32093 2024-04-16 08:33:06.000000 visionai_data_format-1.3.5/visionai_data_format/schemas/visionai_schema.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-24 01:50:00.576235 visionai_data_format-1.3.5/visionai_data_format/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1692 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/utils/calculation.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    10506 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/utils/checker.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      761 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/utils/classes.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      593 2024-05-20 06:25:16.000000 visionai_data_format-1.3.5/visionai_data_format/utils/common.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     4571 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/utils/converter.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     4059 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/utils/resize.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     4588 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/utils/validator.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     2308 2023-12-21 03:02:35.000000 visionai_data_format-1.3.5/visionai_data_format/vai_to_bdd.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5917 2023-07-06 06:50:32.000000 visionai_data_format-1.3.5/visionai_data_format/vai_to_bdd_v2.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-24 01:50:00.576471 visionai_data_format-1.3.5/visionai_data_format.egg-info/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    25808 2024-05-24 01:50:00.000000 visionai_data_format-1.3.5/visionai_data_format.egg-info/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1595 2024-05-24 01:50:00.000000 visionai_data_format-1.3.5/visionai_data_format.egg-info/SOURCES.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-05-24 01:50:00.000000 visionai_data_format-1.3.5/visionai_data_format.egg-info/dependency_links.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       52 2024-05-24 01:50:00.000000 visionai_data_format-1.3.5/visionai_data_format.egg-info/requires.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       21 2024-05-24 01:50:00.000000 visionai_data_format-1.3.5/visionai_data_format.egg-info/top_level.txt
```

### Comparing `visionai_data_format-1.3.4/PKG-INFO` & `visionai_data_format-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai-data-format
-Version: 1.3.4
+Version: 1.3.5
 Summary: converter tool for visionai format
 Home-page: 
 Author: LinkerVision
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==1.*
 Requires-Dist: pillow
```

### Comparing `visionai_data_format-1.3.4/README.md` & `visionai_data_format-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/setup.py` & `visionai_data_format-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "visionai-data-format"
-PACKAGE_VERSION = "1.3.4"
+PACKAGE_VERSION = "1.3.5"
 DESC = "converter tool for visionai format"
 REQUIRED = ["pydantic==1.*", "pillow"]
 REQUIRES_PYTHON = ">=3.7, <4"
 EXTRAS = {
     "test": [
         "pytest",
         "mock",
```

### Comparing `visionai_data_format-1.3.4/tests/test_schemas.py` & `visionai_data_format-1.3.5/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/tests/test_validators.py` & `visionai_data_format-1.3.5/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/convert_dataset.py` & `visionai_data_format-1.3.5/visionai_data_format/convert_dataset.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/converters/base.py` & `visionai_data_format-1.3.5/visionai_data_format/converters/base.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/converters/bdd_to_vai.py` & `visionai_data_format-1.3.5/visionai_data_format/converters/bdd_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/converters/coco_to_vai.py` & `visionai_data_format-1.3.5/visionai_data_format/converters/coco_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/converters/kitti_to_vai.py` & `visionai_data_format-1.3.5/visionai_data_format/converters/kitti_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/converters/vai_to_coco.py` & `visionai_data_format-1.3.5/visionai_data_format/converters/vai_to_coco.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,16 +189,16 @@
                 height=img_height,
                 file_name=f"{image_id:012d}{IMAGE_EXT}",
                 coco_url=dest_coco_url
                 # assume there is only one sensor, so there is only one img url per frame
             )
             images.append(image)
 
-            image_id += 1
             if not frame_data.get("objects", None):
+                image_id += 1
                 continue
 
             for object_id, object_v in frame_data["objects"].items():
                 # from [center x, center y, width, height] to [top left x, top left y, width, height]
                 center_x, center_y, width, height = object_v["object_data"]["bbox"][0][
                     "val"
                 ]
@@ -218,14 +218,15 @@
                     category_id=category_map[category],
                     bbox=bbox,
                     area=width * height,
                     iscrowd=0,
                 )
                 annotations.append(annotation)
                 anno_id += 1
+            image_id += 1
         if n_frame != -1:
             n_frame -= len(images)
         return (category_map, images, annotations, image_id, anno_id, n_frame)
 
     @classmethod
     def _visionai_to_coco(
         cls,
```

### Comparing `visionai_data_format-1.3.4/visionai_data_format/converters/yolo_to_vai.py` & `visionai_data_format-1.3.5/visionai_data_format/converters/yolo_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/exceptions/constants.py` & `visionai_data_format-1.3.5/visionai_data_format/exceptions/constants.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/exceptions/error_messages.py` & `visionai_data_format-1.3.5/visionai_data_format/exceptions/error_messages.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/exceptions/visionai.py` & `visionai_data_format-1.3.5/visionai_data_format/exceptions/visionai.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/schemas/bdd_schema.py` & `visionai_data_format-1.3.5/visionai_data_format/schemas/bdd_schema.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/schemas/coco_schema.py` & `visionai_data_format-1.3.5/visionai_data_format/schemas/coco_schema.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/schemas/common.py` & `visionai_data_format-1.3.5/visionai_data_format/schemas/common.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/schemas/ontology.py` & `visionai_data_format-1.3.5/visionai_data_format/schemas/ontology.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/schemas/utils/validators.py` & `visionai_data_format-1.3.5/visionai_data_format/schemas/utils/validators.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/schemas/visionai_schema.py` & `visionai_data_format-1.3.5/visionai_data_format/schemas/visionai_schema.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/utils/calculation.py` & `visionai_data_format-1.3.5/visionai_data_format/utils/calculation.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/utils/checker.py` & `visionai_data_format-1.3.5/visionai_data_format/utils/checker.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/utils/classes.py` & `visionai_data_format-1.3.5/visionai_data_format/utils/classes.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/utils/common.py` & `visionai_data_format-1.3.5/visionai_data_format/utils/common.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/utils/converter.py` & `visionai_data_format-1.3.5/visionai_data_format/utils/converter.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/utils/resize.py` & `visionai_data_format-1.3.5/visionai_data_format/utils/resize.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/utils/validator.py` & `visionai_data_format-1.3.5/visionai_data_format/utils/validator.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/vai_to_bdd.py` & `visionai_data_format-1.3.5/visionai_data_format/vai_to_bdd.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format/vai_to_bdd_v2.py` & `visionai_data_format-1.3.5/visionai_data_format/vai_to_bdd_v2.py`

 * *Files identical despite different names*

### Comparing `visionai_data_format-1.3.4/visionai_data_format.egg-info/PKG-INFO` & `visionai_data_format-1.3.5/visionai_data_format.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai-data-format
-Version: 1.3.4
+Version: 1.3.5
 Summary: converter tool for visionai format
 Home-page: 
 Author: LinkerVision
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==1.*
 Requires-Dist: pillow
```

### Comparing `visionai_data_format-1.3.4/visionai_data_format.egg-info/SOURCES.txt` & `visionai_data_format-1.3.5/visionai_data_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

