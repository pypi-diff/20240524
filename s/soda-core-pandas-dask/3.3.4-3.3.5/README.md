# Comparing `tmp/soda_core_pandas_dask-3.3.4.tar.gz` & `tmp/soda_core_pandas_dask-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_pandas_dask-3.3.4.tar", last modified: Tue May  7 23:40:05 2024, max compression
+gzip compressed data, was "soda_core_pandas_dask-3.3.5.tar", last modified: Thu May 23 22:50:33 2024, max compression
```

## Comparing `soda_core_pandas_dask-3.3.4.tar` & `soda_core_pandas_dask-3.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:05.835965 soda_core_pandas_dask-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 23:39:42.000000 soda_core_pandas_dask-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 23:40:05.835965 soda_core_pandas_dask-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:40:05.835965 soda_core_pandas_dask-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-07 23:39:42.000000 soda_core_pandas_dask-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:05.831965 soda_core_pandas_dask-3.3.4/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:05.831965 soda_core_pandas_dask-3.3.4/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 23:39:42.000000 soda_core_pandas_dask-3.3.4/soda/data_sources/dask_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-07 23:39:42.000000 soda_core_pandas_dask-3.3.4/soda/data_sources/dask_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-07 23:39:42.000000 soda_core_pandas_dask-3.3.4/soda/data_sources/dask_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:05.831965 soda_core_pandas_dask-3.3.4/soda_core_pandas_dask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-07 23:40:05.000000 soda_core_pandas_dask-3.3.4/soda_core_pandas_dask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-07 23:40:05.000000 soda_core_pandas_dask-3.3.4/soda_core_pandas_dask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:40:05.000000 soda_core_pandas_dask-3.3.4/soda_core_pandas_dask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 23:40:05.000000 soda_core_pandas_dask-3.3.4/soda_core_pandas_dask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 23:40:05.000000 soda_core_pandas_dask-3.3.4/soda_core_pandas_dask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:05.831965 soda_core_pandas_dask-3.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:39:42.000000 soda_core_pandas_dask-3.3.4/tests/test_dask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:33.134011 soda_core_pandas_dask-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 22:50:11.000000 soda_core_pandas_dask-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-23 22:50:33.134011 soda_core_pandas_dask-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:50:33.134011 soda_core_pandas_dask-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-23 22:50:11.000000 soda_core_pandas_dask-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:33.134011 soda_core_pandas_dask-3.3.5/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:33.134011 soda_core_pandas_dask-3.3.5/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-23 22:50:11.000000 soda_core_pandas_dask-3.3.5/soda/data_sources/dask_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-23 22:50:11.000000 soda_core_pandas_dask-3.3.5/soda/data_sources/dask_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-23 22:50:11.000000 soda_core_pandas_dask-3.3.5/soda/data_sources/dask_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:33.134011 soda_core_pandas_dask-3.3.5/soda_core_pandas_dask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-23 22:50:33.000000 soda_core_pandas_dask-3.3.5/soda_core_pandas_dask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-23 22:50:33.000000 soda_core_pandas_dask-3.3.5/soda_core_pandas_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:50:33.000000 soda_core_pandas_dask-3.3.5/soda_core_pandas_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 22:50:33.000000 soda_core_pandas_dask-3.3.5/soda_core_pandas_dask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 22:50:33.000000 soda_core_pandas_dask-3.3.5/soda_core_pandas_dask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:33.134011 soda_core_pandas_dask-3.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:50:11.000000 soda_core_pandas_dask-3.3.5/tests/test_dask.py
```

### Comparing `soda_core_pandas_dask-3.3.4/LICENSE` & `soda_core_pandas_dask-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core_pandas_dask-3.3.4/setup.py` & `soda_core_pandas_dask-3.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import find_namespace_packages, setup
 
 package_name = "soda-core-pandas-dask"
-package_version = "3.3.4"
+package_version = "3.3.5"
 description = "Soda Core Dask Package"
 
 # 2023.10 or its subdependencies introduces breaking changes in how rows are counted, so we stay away from it for now.
 requires = [f"soda-core=={package_version}", "dask>=2022.10.0", "dask-sql>=2022.12.0,<2023.10.0"]
 
 
 setup(
```

### Comparing `soda_core_pandas_dask-3.3.4/soda/data_sources/dask_cursor.py` & `soda_core_pandas_dask-3.3.5/soda/data_sources/dask_cursor.py`

 * *Files identical despite different names*

### Comparing `soda_core_pandas_dask-3.3.4/soda/data_sources/dask_data_source.py` & `soda_core_pandas_dask-3.3.5/soda/data_sources/dask_data_source.py`

 * *Files identical despite different names*

