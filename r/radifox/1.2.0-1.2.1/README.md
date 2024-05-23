# Comparing `tmp/radifox-1.2.0.tar.gz` & `tmp/radifox-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radifox-1.2.0.tar", last modified: Thu May 23 13:31:05 2024, max compression
+gzip compressed data, was "radifox-1.2.1.tar", last modified: Thu May 23 21:06:05 2024, max compression
```

## Comparing `radifox-1.2.0.tar` & `radifox-1.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:05.421316 radifox-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-23 13:31:01.000000 radifox-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46961 2024-05-23 13:31:05.421316 radifox-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    45907 2024-05-23 13:31:01.000000 radifox-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:05.421316 radifox-1.2.0/radifox/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 13:31:05.421316 radifox-1.2.0/radifox/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:05.417316 radifox-1.2.0/radifox/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/dicom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/lut.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    55768 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/nib_parrec_fork.py
--rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/parrec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:05.417316 radifox-1.2.0/radifox/conversion/parrec_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/parrec_templates/gen_info.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/parrec_templates/pixel_values.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/parrec_templates/top_header.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/parrec_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/conversion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:05.417316 radifox-1.2.0/radifox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16756 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/modules/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:05.417316 radifox-1.2.0/radifox/naming/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/naming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/naming/imagefile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:05.417316 radifox-1.2.0/radifox/qa/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/qa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    13265 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/qa/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/qa/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:05.417316 radifox-1.2.0/radifox/qa/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    25968 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/qa/templates/conversion.html
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/qa/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/qa/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)    22900 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/qa/templates/processing.html
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/qa/templates/project.html
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/qa/templates/subject.html
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/qa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:05.417316 radifox-1.2.0/radifox/records/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/records/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-23 13:31:01.000000 radifox-1.2.0/radifox/records/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:31:05.421316 radifox-1.2.0/radifox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46961 2024-05-23 13:31:05.000000 radifox-1.2.0/radifox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-23 13:31:05.000000 radifox-1.2.0/radifox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:31:05.000000 radifox-1.2.0/radifox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-23 13:31:05.000000 radifox-1.2.0/radifox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-23 13:31:05.000000 radifox-1.2.0/radifox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 13:31:05.000000 radifox-1.2.0/radifox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:31:05.421316 radifox-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-23 13:31:01.000000 radifox-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:05.111457 radifox-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-23 21:06:01.000000 radifox-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46961 2024-05-23 21:06:05.111457 radifox-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    45907 2024-05-23 21:06:01.000000 radifox-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:05.111457 radifox-1.2.1/radifox/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 21:06:05.111457 radifox-1.2.1/radifox/_static_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:05.107457 radifox-1.2.1/radifox/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/dicom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/lut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55768 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/nib_parrec_fork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/parrec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:05.107457 radifox-1.2.1/radifox/conversion/parrec_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/parrec_templates/gen_info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/parrec_templates/pixel_values.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/parrec_templates/top_header.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/parrec_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/conversion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:05.107457 radifox-1.2.1/radifox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16756 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/modules/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:05.107457 radifox-1.2.1/radifox/naming/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/naming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/naming/imagefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:05.107457 radifox-1.2.1/radifox/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15980 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/qa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13482 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/qa/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/qa/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:05.111457 radifox-1.2.1/radifox/qa/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    25968 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/qa/templates/conversion.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/qa/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/qa/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22900 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/qa/templates/processing.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/qa/templates/project.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/qa/templates/subject.html
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/qa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:05.111457 radifox-1.2.1/radifox/records/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/records/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-23 21:06:01.000000 radifox-1.2.1/radifox/records/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:06:05.111457 radifox-1.2.1/radifox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46961 2024-05-23 21:06:05.000000 radifox-1.2.1/radifox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-23 21:06:05.000000 radifox-1.2.1/radifox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:06:05.000000 radifox-1.2.1/radifox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-23 21:06:05.000000 radifox-1.2.1/radifox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-23 21:06:05.000000 radifox-1.2.1/radifox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 21:06:05.000000 radifox-1.2.1/radifox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:06:05.111457 radifox-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-23 21:06:01.000000 radifox-1.2.1/setup.py
```

### Comparing `radifox-1.2.0/LICENSE` & `radifox-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/PKG-INFO` & `radifox-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radifox
-Version: 1.2.0
+Version: 1.2.1
 Summary: RADIFOX is the RADiological Image File Ontology eXtension, a Python package for the organization and management of medical images.
 Home-page: https://github.com/jh-mipc/radifox
 Author: Blake Dewey
 Author-email: blake.dewey@jhu.edu
 License: Apache License, 2.0
 Keywords: mri conversion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `radifox-1.2.0/README.md` & `radifox-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/_version.py` & `radifox-1.2.1/radifox/_version.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/base.py` & `radifox-1.2.1/radifox/conversion/base.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/cli.py` & `radifox-1.2.1/radifox/conversion/cli.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/dicom.py` & `radifox-1.2.1/radifox/conversion/dicom.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/exec.py` & `radifox-1.2.1/radifox/conversion/exec.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/json.py` & `radifox-1.2.1/radifox/conversion/json.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/logging.py` & `radifox-1.2.1/radifox/conversion/logging.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/lut.py` & `radifox-1.2.1/radifox/conversion/lut.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/metadata.py` & `radifox-1.2.1/radifox/conversion/metadata.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/nib_parrec_fork.py` & `radifox-1.2.1/radifox/conversion/nib_parrec_fork.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/parrec.py` & `radifox-1.2.1/radifox/conversion/parrec.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/parrec_templates/gen_info.txt` & `radifox-1.2.1/radifox/conversion/parrec_templates/gen_info.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/parrec_templates/pixel_values.txt` & `radifox-1.2.1/radifox/conversion/parrec_templates/pixel_values.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/parrec_writer.py` & `radifox-1.2.1/radifox/conversion/parrec_writer.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/conversion/utils.py` & `radifox-1.2.1/radifox/conversion/utils.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/modules/staging.py` & `radifox-1.2.1/radifox/modules/staging.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/naming/imagefile.py` & `radifox-1.2.1/radifox/naming/imagefile.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/qa/app.py` & `radifox-1.2.1/radifox/qa/app.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/qa/create.py` & `radifox-1.2.1/radifox/qa/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,19 +288,27 @@
         return sel_slice if tuple(dirs) == self.inplane_dirs[plane][0] else sel_slice.T
 
 
 def create_surface_qa_image(
     surf_file,
     img_file,
     output_file,
+    color="red",
     axial_slices=(0.3, 0.35, 0.4, 0.45, 0.5, 0.55, 0.6, 0.65, 0.7),
     coronal_slices=(0.3, 0.35, 0.4, 0.45, 0.5, 0.55, 0.6, 0.65, 0.7),
     sagittal_slices=(0.3, 0.35, 0.4, 0.45, 0.5, 0.55, 0.6, 0.65, 0.7),
-    color="red",
 ):
+    linewidth = 0.5
+    if color == "binary":
+        linecolor = "red"
+    if isinstance(color, (list, tuple)):
+        linecolor = color[0]
+        linewidth = color[1]
+    else:
+        linecolor = color
     img_obj = nib.Nifti1Image.load(img_file)
     img_data = img_obj.get_fdata()
     # noinspection PyUnresolvedReferences
     tk = get_tkr_matrix(img_obj.shape, img_obj.header.get_zooms())
 
     surf_obj = nib.GiftiImage.load(surf_file)
     mesh = trimesh.Trimesh(*surf_obj.agg_data(("pointset", "triangle")))
@@ -377,15 +385,15 @@
                     if direction in ["sagittal", "coronal"]:
                         points = points[:, ::-1]
                         points[:, 1] = img_data.shape[2] - points[:, 1] + 16
                         if direction == "coronal":
                             points[:, 0] = img_data.shape[0] - points[:, 0]
                     else:
                         points[:, 1] = img_data.shape[1] - points[:, 1]
-                    ax.plot(*points.T, color=color, linewidth=0.5)
+                    ax.plot(*points.T, color=linecolor, linewidth=linewidth)
             buf = io.BytesIO()
             fig.savefig(buf, format="png")
             buf.seek(0)
             imgs[d].append(np.array(Image.open(buf)))
             buf.close()
             plt.close(fig)
     montage = np.concatenate([np.concatenate(img_dir, 1) for img_dir in imgs], 0)
```

### Comparing `radifox-1.2.0/radifox/qa/run.py` & `radifox-1.2.1/radifox/qa/run.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/qa/templates/conversion.html` & `radifox-1.2.1/radifox/qa/templates/conversion.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/qa/templates/index.html` & `radifox-1.2.1/radifox/qa/templates/index.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/qa/templates/login.html` & `radifox-1.2.1/radifox/qa/templates/login.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/qa/templates/processing.html` & `radifox-1.2.1/radifox/qa/templates/processing.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/qa/templates/project.html` & `radifox-1.2.1/radifox/qa/templates/project.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/qa/templates/subject.html` & `radifox-1.2.1/radifox/qa/templates/subject.html`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox/records/processing.py` & `radifox-1.2.1/radifox/records/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,16 @@
             if overlay is not None and overlay.name.endswith(".gii"):
                 if len(nib.GiftiImage.load(overlay).agg_data('pointset')) == 0 \
                         or len(nib.GiftiImage.load(overlay).agg_data('triangle')) == 0:
                     continue
                 create_surface_qa_image(
                     overlay,
                     bg_image,
-                    out_dir / out_name
+                    out_dir / out_name,
+                    color=lut,
                 )
             else:
                 create_qa_image(
                     str(bg_image),
                     out_dir / out_name,
                     str(overlay) if overlay is not None else None,
                     lut,
```

### Comparing `radifox-1.2.0/radifox/records/utils.py` & `radifox-1.2.1/radifox/records/utils.py`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/radifox.egg-info/PKG-INFO` & `radifox-1.2.1/radifox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radifox
-Version: 1.2.0
+Version: 1.2.1
 Summary: RADIFOX is the RADiological Image File Ontology eXtension, a Python package for the organization and management of medical images.
 Home-page: https://github.com/jh-mipc/radifox
 Author: Blake Dewey
 Author-email: blake.dewey@jhu.edu
 License: Apache License, 2.0
 Keywords: mri conversion
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `radifox-1.2.0/radifox.egg-info/SOURCES.txt` & `radifox-1.2.1/radifox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radifox-1.2.0/setup.py` & `radifox-1.2.1/setup.py`

 * *Files identical despite different names*

