# Comparing `tmp/soda_core_athena-3.3.4.tar.gz` & `tmp/soda_core_athena-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_athena-3.3.4.tar", last modified: Tue May  7 23:39:48 2024, max compression
+gzip compressed data, was "soda_core_athena-3.3.5.tar", last modified: Thu May 23 22:50:18 2024, max compression
```

## Comparing `soda_core_athena-3.3.4.tar` & `soda_core_athena-3.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:48.295930 soda_core_athena-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 23:39:42.000000 soda_core_athena-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 23:39:48.295930 soda_core_athena-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:39:48.295930 soda_core_athena-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-07 23:39:42.000000 soda_core_athena-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:48.295930 soda_core_athena-3.3.4/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:48.295930 soda_core_athena-3.3.4/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-07 23:39:42.000000 soda_core_athena-3.3.4/soda/data_sources/athena_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:48.295930 soda_core_athena-3.3.4/soda_core_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-07 23:39:48.000000 soda_core_athena-3.3.4/soda_core_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-07 23:39:48.000000 soda_core_athena-3.3.4/soda_core_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:39:48.000000 soda_core_athena-3.3.4/soda_core_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:39:48.000000 soda_core_athena-3.3.4/soda_core_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 23:39:48.000000 soda_core_athena-3.3.4/soda_core_athena.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:39:48.295930 soda_core_athena-3.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-07 23:39:42.000000 soda_core_athena-3.3.4/tests/test_athena.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:18.597848 soda_core_athena-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 22:50:11.000000 soda_core_athena-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-23 22:50:18.597848 soda_core_athena-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:50:18.597848 soda_core_athena-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-23 22:50:11.000000 soda_core_athena-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:18.597848 soda_core_athena-3.3.5/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:18.597848 soda_core_athena-3.3.5/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-23 22:50:11.000000 soda_core_athena-3.3.5/soda/data_sources/athena_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:18.597848 soda_core_athena-3.3.5/soda_core_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-23 22:50:18.000000 soda_core_athena-3.3.5/soda_core_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-23 22:50:18.000000 soda_core_athena-3.3.5/soda_core_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:50:18.000000 soda_core_athena-3.3.5/soda_core_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:50:18.000000 soda_core_athena-3.3.5/soda_core_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 22:50:18.000000 soda_core_athena-3.3.5/soda_core_athena.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:18.597848 soda_core_athena-3.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 22:50:11.000000 soda_core_athena-3.3.5/tests/test_athena.py
```

### Comparing `soda_core_athena-3.3.4/LICENSE` & `soda_core_athena-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core_athena-3.3.4/soda/data_sources/athena_data_source.py` & `soda_core_athena-3.3.5/soda/data_sources/athena_data_source.py`

 * *Files identical despite different names*

