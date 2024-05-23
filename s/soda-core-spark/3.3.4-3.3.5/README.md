# Comparing `tmp/soda_core_spark-3.3.4.tar.gz` & `tmp/soda_core_spark-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_spark-3.3.4.tar", last modified: Tue May  7 23:40:43 2024, max compression
+gzip compressed data, was "soda_core_spark-3.3.5.tar", last modified: Thu May 23 22:51:10 2024, max compression
```

## Comparing `soda_core_spark-3.3.4.tar` & `soda_core_spark-3.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:43.328010 soda_core_spark-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 23:39:42.000000 soda_core_spark-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-07 23:40:43.328010 soda_core_spark-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:40:43.328010 soda_core_spark-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-07 23:39:42.000000 soda_core_spark-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:43.324010 soda_core_spark-3.3.4/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:43.328010 soda_core_spark-3.3.4/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)    17855 2024-05-07 23:39:42.000000 soda_core_spark-3.3.4/soda/data_sources/spark_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:43.328010 soda_core_spark-3.3.4/soda_core_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-07 23:40:43.000000 soda_core_spark-3.3.4/soda_core_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-07 23:40:43.000000 soda_core_spark-3.3.4/soda_core_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:40:43.000000 soda_core_spark-3.3.4/soda_core_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-07 23:40:43.000000 soda_core_spark-3.3.4/soda_core_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 23:40:43.000000 soda_core_spark-3.3.4/soda_core_spark.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:43.328010 soda_core_spark-3.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-07 23:39:42.000000 soda_core_spark-3.3.4/tests/test_table_name_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:10.174447 soda_core_spark-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 22:50:11.000000 soda_core_spark-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-23 22:51:10.174447 soda_core_spark-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:51:10.174447 soda_core_spark-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-23 22:50:11.000000 soda_core_spark-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:10.170446 soda_core_spark-3.3.5/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:10.174447 soda_core_spark-3.3.5/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)    17855 2024-05-23 22:50:11.000000 soda_core_spark-3.3.5/soda/data_sources/spark_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:10.174447 soda_core_spark-3.3.5/soda_core_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-23 22:51:10.000000 soda_core_spark-3.3.5/soda_core_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 22:51:10.000000 soda_core_spark-3.3.5/soda_core_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:51:10.000000 soda_core_spark-3.3.5/soda_core_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-23 22:51:10.000000 soda_core_spark-3.3.5/soda_core_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 22:51:10.000000 soda_core_spark-3.3.5/soda_core_spark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:10.174447 soda_core_spark-3.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-23 22:50:11.000000 soda_core_spark-3.3.5/tests/test_table_name_filtering.py
```

### Comparing `soda_core_spark-3.3.4/LICENSE` & `soda_core_spark-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core_spark-3.3.4/setup.py` & `soda_core_spark-3.3.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import find_namespace_packages, setup
 
 package_name = "soda-core-spark"
-package_version = "3.3.4"
+package_version = "3.3.5"
 description = "Soda Core Spark Package"
 
 requires = [f"soda-core=={package_version}"]
 
 extras = {
     "hive": [
         "PyHive[hive]",
```

### Comparing `soda_core_spark-3.3.4/soda/data_sources/spark_data_source.py` & `soda_core_spark-3.3.5/soda/data_sources/spark_data_source.py`

 * *Files identical despite different names*

### Comparing `soda_core_spark-3.3.4/tests/test_table_name_filtering.py` & `soda_core_spark-3.3.5/tests/test_table_name_filtering.py`

 * *Files identical despite different names*

