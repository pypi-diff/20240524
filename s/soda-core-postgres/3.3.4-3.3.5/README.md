# Comparing `tmp/soda_core_postgres-3.3.4.tar.gz` & `tmp/soda_core_postgres-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_postgres-3.3.4.tar", last modified: Tue May  7 23:40:30 2024, max compression
+gzip compressed data, was "soda_core_postgres-3.3.5.tar", last modified: Thu May 23 22:50:56 2024, max compression
```

## Comparing `soda_core_postgres-3.3.4.tar` & `soda_core_postgres-3.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:30.311992 soda_core_postgres-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 23:39:42.000000 soda_core_postgres-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 23:40:30.311992 soda_core_postgres-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:40:30.311992 soda_core_postgres-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-07 23:39:42.000000 soda_core_postgres-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:30.311992 soda_core_postgres-3.3.4/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:30.311992 soda_core_postgres-3.3.4/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-05-07 23:39:42.000000 soda_core_postgres-3.3.4/soda/data_sources/postgres_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:30.311992 soda_core_postgres-3.3.4/soda_core_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-07 23:40:30.000000 soda_core_postgres-3.3.4/soda_core_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-07 23:40:30.000000 soda_core_postgres-3.3.4/soda_core_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:40:30.000000 soda_core_postgres-3.3.4/soda_core_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-07 23:40:30.000000 soda_core_postgres-3.3.4/soda_core_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 23:40:30.000000 soda_core_postgres-3.3.4/soda_core_postgres.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:30.311992 soda_core_postgres-3.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-07 23:39:42.000000 soda_core_postgres-3.3.4/tests/test_postgres_connection_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-07 23:39:42.000000 soda_core_postgres-3.3.4/tests/test_postgres_specific_stuff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:56.050284 soda_core_postgres-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 22:50:11.000000 soda_core_postgres-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-23 22:50:56.050284 soda_core_postgres-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:50:56.050284 soda_core_postgres-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-23 22:50:11.000000 soda_core_postgres-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:56.046284 soda_core_postgres-3.3.5/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:56.046284 soda_core_postgres-3.3.5/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-05-23 22:50:11.000000 soda_core_postgres-3.3.5/soda/data_sources/postgres_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:56.050284 soda_core_postgres-3.3.5/soda_core_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-23 22:50:56.000000 soda_core_postgres-3.3.5/soda_core_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-23 22:50:56.000000 soda_core_postgres-3.3.5/soda_core_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:50:56.000000 soda_core_postgres-3.3.5/soda_core_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 22:50:56.000000 soda_core_postgres-3.3.5/soda_core_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 22:50:56.000000 soda_core_postgres-3.3.5/soda_core_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:56.050284 soda_core_postgres-3.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-23 22:50:11.000000 soda_core_postgres-3.3.5/tests/test_postgres_connection_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-23 22:50:11.000000 soda_core_postgres-3.3.5/tests/test_postgres_specific_stuff.py
```

### Comparing `soda_core_postgres-3.3.4/LICENSE` & `soda_core_postgres-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core_postgres-3.3.4/soda/data_sources/postgres_data_source.py` & `soda_core_postgres-3.3.5/soda/data_sources/postgres_data_source.py`

 * *Files identical despite different names*

### Comparing `soda_core_postgres-3.3.4/tests/test_postgres_connection_validation.py` & `soda_core_postgres-3.3.5/tests/test_postgres_connection_validation.py`

 * *Files identical despite different names*

### Comparing `soda_core_postgres-3.3.4/tests/test_postgres_specific_stuff.py` & `soda_core_postgres-3.3.5/tests/test_postgres_specific_stuff.py`

 * *Files identical despite different names*

