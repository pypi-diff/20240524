# Comparing `tmp/radifox-1.2.2.tar.gz` & `tmp/radifox-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radifox-1.2.2.tar", last modified: Thu May 23 22:52:38 2024, max compression
+gzip compressed data, was "radifox-1.2.3.tar", last modified: Thu May 23 22:59:15 2024, max compression
```

## Comparing `radifox-1.2.2.tar` & `radifox-1.2.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:52:38.035576 radifox-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-23 22:52:34.000000 radifox-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46961 2024-05-23 22:52:38.035576 radifox-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    45907 2024-05-23 22:52:34.000000 radifox-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:52:38.035576 radifox-1.2.2/radifox/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 22:52:38.035576 radifox-1.2.2/radifox/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:52:38.031576 radifox-1.2.2/radifox/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/dicom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/lut.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    55768 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/nib_parrec_fork.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/parrec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:52:38.031576 radifox-1.2.2/radifox/conversion/parrec_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/parrec_templates/gen_info.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/parrec_templates/pixel_values.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/parrec_templates/top_header.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/parrec_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/conversion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:52:38.031576 radifox-1.2.2/radifox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16756 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/modules/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:52:38.031576 radifox-1.2.2/radifox/naming/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/naming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/naming/imagefile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:52:38.031576 radifox-1.2.2/radifox/qa/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/qa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/qa/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/qa/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:52:38.031576 radifox-1.2.2/radifox/qa/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    25968 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/qa/templates/conversion.html
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/qa/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/qa/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)    22900 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/qa/templates/processing.html
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/qa/templates/project.html
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/qa/templates/subject.html
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/qa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:52:38.035576 radifox-1.2.2/radifox/records/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/records/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-23 22:52:34.000000 radifox-1.2.2/radifox/records/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:52:38.035576 radifox-1.2.2/radifox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46961 2024-05-23 22:52:38.000000 radifox-1.2.2/radifox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-23 22:52:38.000000 radifox-1.2.2/radifox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:52:38.000000 radifox-1.2.2/radifox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-23 22:52:38.000000 radifox-1.2.2/radifox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-23 22:52:38.000000 radifox-1.2.2/radifox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 22:52:38.000000 radifox-1.2.2/radifox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:52:38.035576 radifox-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-23 22:52:34.000000 radifox-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:15.271862 radifox-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-23 22:59:11.000000 radifox-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46961 2024-05-23 22:59:15.271862 radifox-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    45907 2024-05-23 22:59:11.000000 radifox-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:15.271862 radifox-1.2.3/radifox/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 22:59:15.271862 radifox-1.2.3/radifox/_static_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:15.267862 radifox-1.2.3/radifox/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/lut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55768 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/nib_parrec_fork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/parrec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:15.267862 radifox-1.2.3/radifox/conversion/parrec_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/parrec_templates/gen_info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/parrec_templates/pixel_values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/parrec_templates/top_header.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/parrec_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/conversion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:15.267862 radifox-1.2.3/radifox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16756 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/modules/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:15.267862 radifox-1.2.3/radifox/naming/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/naming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/naming/imagefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:15.271862 radifox-1.2.3/radifox/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15965 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/qa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/qa/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/qa/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:15.271862 radifox-1.2.3/radifox/qa/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    25968 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/qa/templates/conversion.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/qa/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/qa/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22900 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/qa/templates/processing.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/qa/templates/project.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/qa/templates/subject.html
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/qa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:15.271862 radifox-1.2.3/radifox/records/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/records/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-23 22:59:11.000000 radifox-1.2.3/radifox/records/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:15.271862 radifox-1.2.3/radifox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46961 2024-05-23 22:59:15.000000 radifox-1.2.3/radifox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-23 22:59:15.000000 radifox-1.2.3/radifox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:59:15.000000 radifox-1.2.3/radifox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-23 22:59:15.000000 radifox-1.2.3/radifox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-23 22:59:15.000000 radifox-1.2.3/radifox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 22:59:15.000000 radifox-1.2.3/radifox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:59:15.271862 radifox-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-23 22:59:11.000000 radifox-1.2.3/setup.py
```

### Comparing `radifox-1.2.2/LICENSE` & `radifox-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/PKG-INFO` & `radifox-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radifox
-Version: 1.2.2
+Version: 1.2.3
 Summary: RADIFOX is the RADiological Image File Ontology eXtension, a Python package for the organization and management of medical images.
 Home-page: https://github.com/jh-mipc/radifox
 Author: Blake Dewey
 Author-email: blake.dewey@jhu.edu
 License: Apache License, 2.0
 Keywords: mri conversion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `radifox-1.2.2/README.md` & `radifox-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/_version.py` & `radifox-1.2.3/radifox/_version.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/base.py` & `radifox-1.2.3/radifox/conversion/base.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/cli.py` & `radifox-1.2.3/radifox/conversion/cli.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/dicom.py` & `radifox-1.2.3/radifox/conversion/dicom.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/exec.py` & `radifox-1.2.3/radifox/conversion/exec.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/json.py` & `radifox-1.2.3/radifox/conversion/json.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/logging.py` & `radifox-1.2.3/radifox/conversion/logging.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/lut.py` & `radifox-1.2.3/radifox/conversion/lut.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/metadata.py` & `radifox-1.2.3/radifox/conversion/metadata.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/nib_parrec_fork.py` & `radifox-1.2.3/radifox/conversion/nib_parrec_fork.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/parrec.py` & `radifox-1.2.3/radifox/conversion/parrec.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/parrec_templates/gen_info.txt` & `radifox-1.2.3/radifox/conversion/parrec_templates/gen_info.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/parrec_templates/pixel_values.txt` & `radifox-1.2.3/radifox/conversion/parrec_templates/pixel_values.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/parrec_writer.py` & `radifox-1.2.3/radifox/conversion/parrec_writer.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/conversion/utils.py` & `radifox-1.2.3/radifox/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/modules/staging.py` & `radifox-1.2.3/radifox/modules/staging.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/naming/imagefile.py` & `radifox-1.2.3/radifox/naming/imagefile.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/qa/app.py` & `radifox-1.2.3/radifox/qa/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,24 +290,24 @@
             prov_obj["OutputQA"] = {}
             for key, val in prov_obj["Outputs"].items():
                 prov_obj["OutputQA"][key] = {}
                 if not isinstance(val, list):
                     val = [val]
                 for v in val:
                     filestr = v.split(":")[0]
-                    if not (filestr.endswith(".nii.gz") or filestr.endswith(".gii")):
-                        continue
                     existing_qa = qa_dict.get(filestr, "")
                     filepath = session_dir.parent.parent / filestr
                     qa_path = (
                         filepath.parent.parent
                         / "qa"
                         / module_str.split(":")[0]
-                        / (filepath.name.replace(".nii.gz", ".png").replace(".gii", ".png"))
+                        / (filepath.name.split('.')[0] + '.png')
                     )
+                    if not qa_path.exists():
+                        continue
                     display_name = (
                         filestr.split("_")[2]
                         + "_"
                         + " / ".join(filestr.split(".")[0].split("_")[3:])
                     )
                     prov_obj["OutputQA"][key][filestr] = (
                         (
```

### Comparing `radifox-1.2.2/radifox/qa/create.py` & `radifox-1.2.3/radifox/qa/create.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/qa/run.py` & `radifox-1.2.3/radifox/qa/run.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/qa/templates/conversion.html` & `radifox-1.2.3/radifox/qa/templates/conversion.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/qa/templates/index.html` & `radifox-1.2.3/radifox/qa/templates/index.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/qa/templates/login.html` & `radifox-1.2.3/radifox/qa/templates/login.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/qa/templates/processing.html` & `radifox-1.2.3/radifox/qa/templates/processing.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/qa/templates/project.html` & `radifox-1.2.3/radifox/qa/templates/project.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/qa/templates/subject.html` & `radifox-1.2.3/radifox/qa/templates/subject.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/records/processing.py` & `radifox-1.2.3/radifox/records/processing.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox/records/utils.py` & `radifox-1.2.3/radifox/records/utils.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/radifox.egg-info/PKG-INFO` & `radifox-1.2.3/radifox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radifox
-Version: 1.2.2
+Version: 1.2.3
 Summary: RADIFOX is the RADiological Image File Ontology eXtension, a Python package for the organization and management of medical images.
 Home-page: https://github.com/jh-mipc/radifox
 Author: Blake Dewey
 Author-email: blake.dewey@jhu.edu
 License: Apache License, 2.0
 Keywords: mri conversion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `radifox-1.2.2/radifox.egg-info/SOURCES.txt` & `radifox-1.2.3/radifox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.2.2/setup.py` & `radifox-1.2.3/setup.py`

 * *Files identical despite different names*

