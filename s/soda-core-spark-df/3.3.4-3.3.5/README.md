# Comparing `tmp/soda_core_spark_df-3.3.4.tar.gz` & `tmp/soda_core_spark_df-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_spark_df-3.3.4.tar", last modified: Tue May  7 23:40:46 2024, max compression
+gzip compressed data, was "soda_core_spark_df-3.3.5.tar", last modified: Thu May 23 22:51:12 2024, max compression
```

## Comparing `soda_core_spark_df-3.3.4.tar` & `soda_core_spark_df-3.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:46.496015 soda_core_spark_df-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 23:39:42.000000 soda_core_spark_df-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 23:40:46.496015 soda_core_spark_df-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:40:46.496015 soda_core_spark_df-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 23:39:42.000000 soda_core_spark_df-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:46.492015 soda_core_spark_df-3.3.4/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:46.496015 soda_core_spark_df-3.3.4/soda/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-07 23:39:42.000000 soda_core_spark_df-3.3.4/soda/data_sources/spark_df_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-07 23:39:42.000000 soda_core_spark_df-3.3.4/soda/data_sources/spark_df_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-07 23:39:42.000000 soda_core_spark_df-3.3.4/soda/data_sources/spark_df_data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:46.496015 soda_core_spark_df-3.3.4/soda_core_spark_df.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 23:40:46.000000 soda_core_spark_df-3.3.4/soda_core_spark_df.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-07 23:40:46.000000 soda_core_spark_df-3.3.4/soda_core_spark_df.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:40:46.000000 soda_core_spark_df-3.3.4/soda_core_spark_df.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 23:40:46.000000 soda_core_spark_df-3.3.4/soda_core_spark_df.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 23:40:46.000000 soda_core_spark_df-3.3.4/soda_core_spark_df.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:46.496015 soda_core_spark_df-3.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-07 23:39:42.000000 soda_core_spark_df-3.3.4/tests/test_spark_df.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:12.910478 soda_core_spark_df-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 22:50:11.000000 soda_core_spark_df-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-23 22:51:12.910478 soda_core_spark_df-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:51:12.910478 soda_core_spark_df-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-23 22:50:11.000000 soda_core_spark_df-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:12.906479 soda_core_spark_df-3.3.5/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:12.906479 soda_core_spark_df-3.3.5/soda/data_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-23 22:50:11.000000 soda_core_spark_df-3.3.5/soda/data_sources/spark_df_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-23 22:50:11.000000 soda_core_spark_df-3.3.5/soda/data_sources/spark_df_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-23 22:50:11.000000 soda_core_spark_df-3.3.5/soda/data_sources/spark_df_data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:12.910478 soda_core_spark_df-3.3.5/soda_core_spark_df.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-23 22:51:12.000000 soda_core_spark_df-3.3.5/soda_core_spark_df.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-23 22:51:12.000000 soda_core_spark_df-3.3.5/soda_core_spark_df.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:51:12.000000 soda_core_spark_df-3.3.5/soda_core_spark_df.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 22:51:12.000000 soda_core_spark_df-3.3.5/soda_core_spark_df.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 22:51:12.000000 soda_core_spark_df-3.3.5/soda_core_spark_df.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:51:12.910478 soda_core_spark_df-3.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-23 22:50:11.000000 soda_core_spark_df-3.3.5/tests/test_spark_df.py
```

### Comparing `soda_core_spark_df-3.3.4/LICENSE` & `soda_core_spark_df-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core_spark_df-3.3.4/soda/data_sources/spark_df_cursor.py` & `soda_core_spark_df-3.3.5/soda/data_sources/spark_df_cursor.py`

 * *Files identical despite different names*

### Comparing `soda_core_spark_df-3.3.4/soda/data_sources/spark_df_data_source.py` & `soda_core_spark_df-3.3.5/soda/data_sources/spark_df_data_source.py`

 * *Files identical despite different names*

### Comparing `soda_core_spark_df-3.3.4/tests/test_spark_df.py` & `soda_core_spark_df-3.3.5/tests/test_spark_df.py`

 * *Files identical despite different names*

