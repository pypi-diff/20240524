# Comparing `tmp/soda_core_trino-3.3.4.tar.gz` & `tmp/soda_core_trino-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_trino-3.3.4.tar", last modified: Tue May  7 23:40:54 2024, max compression
+gzip compressed data, was "soda_core_trino-3.3.5.tar", last modified: Thu May 23 22:51:21 2024, max compression
```

## Comparing `soda_core_trino-3.3.4.tar` & `soda_core_trino-3.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:54.280027 soda_core_trino-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 23:39:42.000000 soda_core_trino-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 23:40:54.280027 soda_core_trino-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:40:54.280027 soda_core_trino-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 23:39:42.000000 soda_core_trino-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:54.276027 soda_core_trino-3.3.4/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:54.276027 soda_core_trino-3.3.4/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-07 23:39:42.000000 soda_core_trino-3.3.4/soda/data_sources/trino_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:54.280027 soda_core_trino-3.3.4/soda_core_trino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-07 23:40:54.000000 soda_core_trino-3.3.4/soda_core_trino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-07 23:40:54.000000 soda_core_trino-3.3.4/soda_core_trino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:40:54.000000 soda_core_trino-3.3.4/soda_core_trino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-07 23:40:54.000000 soda_core_trino-3.3.4/soda_core_trino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 23:40:54.000000 soda_core_trino-3.3.4/soda_core_trino.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:54.280027 soda_core_trino-3.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 23:39:42.000000 soda_core_trino-3.3.4/tests/test_trino.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:21.874581 soda_core_trino-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 22:50:11.000000 soda_core_trino-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 22:51:21.874581 soda_core_trino-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:51:21.874581 soda_core_trino-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-23 22:50:11.000000 soda_core_trino-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:21.874581 soda_core_trino-3.3.5/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:21.874581 soda_core_trino-3.3.5/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-23 22:50:11.000000 soda_core_trino-3.3.5/soda/data_sources/trino_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:21.874581 soda_core_trino-3.3.5/soda_core_trino.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 22:51:21.000000 soda_core_trino-3.3.5/soda_core_trino.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-23 22:51:21.000000 soda_core_trino-3.3.5/soda_core_trino.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:51:21.000000 soda_core_trino-3.3.5/soda_core_trino.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 22:51:21.000000 soda_core_trino-3.3.5/soda_core_trino.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 22:51:21.000000 soda_core_trino-3.3.5/soda_core_trino.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:21.874581 soda_core_trino-3.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-23 22:50:11.000000 soda_core_trino-3.3.5/tests/test_trino.py
```

### Comparing `soda_core_trino-3.3.4/LICENSE` & `soda_core_trino-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core_trino-3.3.4/soda/data_sources/trino_data_source.py` & `soda_core_trino-3.3.5/soda/data_sources/trino_data_source.py`

 * *Files identical despite different names*

