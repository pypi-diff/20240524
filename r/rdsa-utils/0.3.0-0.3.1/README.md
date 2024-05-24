# Comparing `tmp/rdsa_utils-0.3.0.tar.gz` & `tmp/rdsa_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdsa_utils-0.3.0.tar", last modified: Mon May 20 11:40:17 2024, max compression
+gzip compressed data, was "rdsa_utils-0.3.1.tar", last modified: Fri May 24 12:47:38 2024, max compression
```

## Comparing `rdsa_utils-0.3.0.tar` & `rdsa_utils-0.3.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.775625 rdsa_utils-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-20 11:40:17.775625 rdsa_utils-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.771625 rdsa_utils-0.3.0/rdsa_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.771625 rdsa_utils-0.3.0/rdsa_utils/cdp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/cdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.771625 rdsa_utils-0.3.0/rdsa_utils/cdp/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/cdp/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/cdp/helpers/hdfs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/cdp/helpers/impala.py
--rw-r--r--   0 runner    (1001) docker     (127)    23213 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/cdp/helpers/s3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.771625 rdsa_utils-0.3.0/rdsa_utils/cdp/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/cdp/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/cdp/io/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/cdp/io/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/cdp/io/pipeline_runlog.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.771625 rdsa_utils-0.3.0/rdsa_utils/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/gcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.771625 rdsa_utils-0.3.0/rdsa_utils/gcp/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/gcp/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/gcp/helpers/gcp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.771625 rdsa_utils-0.3.0/rdsa_utils/gcp/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/gcp/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/gcp/io/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/gcp/io/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.775625 rdsa_utils-0.3.0/rdsa_utils/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/helpers/pyspark.py
--rw-r--r--   0 runner    (1001) docker     (127)     9545 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/helpers/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.775625 rdsa_utils-0.3.0/rdsa_utils/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/io/input.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/io/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.775625 rdsa_utils-0.3.0/rdsa_utils/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/methods/averaging_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/rdsa_utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.775625 rdsa_utils-0.3.0/rdsa_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-20 11:40:17.000000 rdsa_utils-0.3.0/rdsa_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 11:40:17.000000 rdsa_utils-0.3.0/rdsa_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:40:17.000000 rdsa_utils-0.3.0/rdsa_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-20 11:40:17.000000 rdsa_utils-0.3.0/rdsa_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 11:40:17.000000 rdsa_utils-0.3.0/rdsa_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-20 11:40:17.775625 rdsa_utils-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:40:17.775625 rdsa_utils-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-20 11:40:13.000000 rdsa_utils-0.3.0/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.178097 rdsa_utils-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-24 12:47:38.178097 rdsa_utils-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.174097 rdsa_utils-0.3.1/rdsa_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.174097 rdsa_utils-0.3.1/rdsa_utils/cdp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/cdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.174097 rdsa_utils-0.3.1/rdsa_utils/cdp/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/cdp/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11615 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/cdp/helpers/hdfs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/cdp/helpers/impala.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23213 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/cdp/helpers/s3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.174097 rdsa_utils-0.3.1/rdsa_utils/cdp/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/cdp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/cdp/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/cdp/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/cdp/io/pipeline_runlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.174097 rdsa_utils-0.3.1/rdsa_utils/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/gcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.174097 rdsa_utils-0.3.1/rdsa_utils/gcp/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/gcp/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23081 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/gcp/helpers/gcp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.174097 rdsa_utils-0.3.1/rdsa_utils/gcp/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/gcp/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/gcp/io/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/gcp/io/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.174097 rdsa_utils-0.3.1/rdsa_utils/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/helpers/pyspark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9545 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/helpers/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.178097 rdsa_utils-0.3.1/rdsa_utils/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.178097 rdsa_utils-0.3.1/rdsa_utils/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/methods/averaging_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/rdsa_utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.178097 rdsa_utils-0.3.1/rdsa_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-24 12:47:38.000000 rdsa_utils-0.3.1/rdsa_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-24 12:47:38.000000 rdsa_utils-0.3.1/rdsa_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:47:38.000000 rdsa_utils-0.3.1/rdsa_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-24 12:47:38.000000 rdsa_utils-0.3.1/rdsa_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 12:47:38.000000 rdsa_utils-0.3.1/rdsa_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-24 12:47:38.178097 rdsa_utils-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:47:38.178097 rdsa_utils-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-24 12:47:32.000000 rdsa_utils-0.3.1/tests/test_validation.py
```

### Comparing `rdsa_utils-0.3.0/LICENSE` & `rdsa_utils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/PKG-INFO` & `rdsa_utils-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdsa-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: A suite of PySpark, Pandas, and general pipeline utils for Reproducible Data Science and Analysis (RDSA) projects.
 Home-page: https://github.com/ONSdigital/rdsa-utils
 Author: Reproducible Data Science & Analysis, ONS
 Author-email: Diego.Lara.De.Andres@ons.gov.uk, Meg.Scammell@ons.gov.uk, Dominic.Bean@ons.gov.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rdsa_utils-0.3.0/README.md` & `rdsa_utils-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/cdp/helpers/hdfs_utils.py` & `rdsa_utils-0.3.1/rdsa_utils/cdp/helpers/hdfs_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/cdp/helpers/impala.py` & `rdsa_utils-0.3.1/rdsa_utils/cdp/helpers/impala.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/cdp/helpers/s3_utils.py` & `rdsa_utils-0.3.1/rdsa_utils/cdp/helpers/s3_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/cdp/io/input.py` & `rdsa_utils-0.3.1/rdsa_utils/cdp/io/input.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/cdp/io/output.py` & `rdsa_utils-0.3.1/rdsa_utils/cdp/io/output.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/cdp/io/pipeline_runlog.py` & `rdsa_utils-0.3.1/rdsa_utils/cdp/io/pipeline_runlog.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/exceptions.py` & `rdsa_utils-0.3.1/rdsa_utils/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,10 +33,10 @@
 class TableNotFoundError(Exception):
     """Custom exception to raise when a table to be read is not found."""
 
     pass
 
 
 class InvalidBucketNameError(Exception):
-    """Custom exception to raise when an AWS S3 bucket name is invalid."""
+    """Custom exception to raise when an AWS S3 or GCS bucket name is invalid."""
 
     pass
```

### Comparing `rdsa_utils-0.3.0/rdsa_utils/gcp/io/inputs.py` & `rdsa_utils-0.3.1/rdsa_utils/gcp/io/inputs.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/gcp/io/outputs.py` & `rdsa_utils-0.3.1/rdsa_utils/gcp/io/outputs.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/helpers/pyspark.py` & `rdsa_utils-0.3.1/rdsa_utils/helpers/pyspark.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/helpers/python.py` & `rdsa_utils-0.3.1/rdsa_utils/helpers/python.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/io/config.py` & `rdsa_utils-0.3.1/rdsa_utils/io/config.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/io/input.py` & `rdsa_utils-0.3.1/rdsa_utils/io/input.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/logging.py` & `rdsa_utils-0.3.1/rdsa_utils/logging.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/methods/averaging_methods.py` & `rdsa_utils-0.3.1/rdsa_utils/methods/averaging_methods.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/test_utils.py` & `rdsa_utils-0.3.1/rdsa_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/typing.py` & `rdsa_utils-0.3.1/rdsa_utils/typing.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils/validation.py` & `rdsa_utils-0.3.1/rdsa_utils/validation.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils.egg-info/PKG-INFO` & `rdsa_utils-0.3.1/rdsa_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdsa-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: A suite of PySpark, Pandas, and general pipeline utils for Reproducible Data Science and Analysis (RDSA) projects.
 Home-page: https://github.com/ONSdigital/rdsa-utils
 Author: Reproducible Data Science & Analysis, ONS
 Author-email: Diego.Lara.De.Andres@ons.gov.uk, Meg.Scammell@ons.gov.uk, Dominic.Bean@ons.gov.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `rdsa_utils-0.3.0/rdsa_utils.egg-info/SOURCES.txt` & `rdsa_utils-0.3.1/rdsa_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/rdsa_utils.egg-info/requires.txt` & `rdsa_utils-0.3.1/rdsa_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/setup.cfg` & `rdsa_utils-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/tests/test_logging.py` & `rdsa_utils-0.3.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `rdsa_utils-0.3.0/tests/test_validation.py` & `rdsa_utils-0.3.1/tests/test_validation.py`

 * *Files identical despite different names*

