# Comparing `tmp/soda_core_dbt-3.3.4.tar.gz` & `tmp/soda_core_dbt-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda_core_dbt-3.3.4.tar", last modified: Tue May  7 23:40:12 2024, max compression
+gzip compressed data, was "soda_core_dbt-3.3.5.tar", last modified: Thu May 23 22:50:39 2024, max compression
```

## Comparing `soda_core_dbt-3.3.4.tar` & `soda_core_dbt-3.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:12.703968 soda_core_dbt-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 23:39:42.000000 soda_core_dbt-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-07 23:40:12.703968 soda_core_dbt-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:40:12.703968 soda_core_dbt-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-07 23:39:42.000000 soda_core_dbt-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:12.699968 soda_core_dbt-3.3.4/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:12.703968 soda_core_dbt-3.3.4/soda/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-05-07 23:39:42.000000 soda_core_dbt-3.3.4/soda/cloud/dbt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:12.699968 soda_core_dbt-3.3.4/soda/execution/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:12.703968 soda_core_dbt-3.3.4/soda/execution/check/
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-07 23:39:42.000000 soda_core_dbt-3.3.4/soda/execution/check/dbt_check.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:12.703968 soda_core_dbt-3.3.4/soda/sodacl/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-07 23:39:42.000000 soda_core_dbt-3.3.4/soda/sodacl/dbt_check_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:12.703968 soda_core_dbt-3.3.4/soda_core_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-07 23:40:12.000000 soda_core_dbt-3.3.4/soda_core_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-07 23:40:12.000000 soda_core_dbt-3.3.4/soda_core_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:40:12.000000 soda_core_dbt-3.3.4/soda_core_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 23:40:12.000000 soda_core_dbt-3.3.4/soda_core_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 23:40:12.000000 soda_core_dbt-3.3.4/soda_core_dbt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:40:12.703968 soda_core_dbt-3.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 23:39:42.000000 soda_core_dbt-3.3.4/tests/test_dbt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.602090 soda_core_dbt-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 22:50:11.000000 soda_core_dbt-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-23 22:50:39.602090 soda_core_dbt-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:50:39.602090 soda_core_dbt-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-23 22:50:11.000000 soda_core_dbt-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.602090 soda_core_dbt-3.3.5/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.602090 soda_core_dbt-3.3.5/soda/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-05-23 22:50:11.000000 soda_core_dbt-3.3.5/soda/cloud/dbt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.602090 soda_core_dbt-3.3.5/soda/execution/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.602090 soda_core_dbt-3.3.5/soda/execution/check/
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-23 22:50:11.000000 soda_core_dbt-3.3.5/soda/execution/check/dbt_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.602090 soda_core_dbt-3.3.5/soda/sodacl/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 22:50:11.000000 soda_core_dbt-3.3.5/soda/sodacl/dbt_check_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.602090 soda_core_dbt-3.3.5/soda_core_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-23 22:50:39.000000 soda_core_dbt-3.3.5/soda_core_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-23 22:50:39.000000 soda_core_dbt-3.3.5/soda_core_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:50:39.000000 soda_core_dbt-3.3.5/soda_core_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 22:50:39.000000 soda_core_dbt-3.3.5/soda_core_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 22:50:39.000000 soda_core_dbt-3.3.5/soda_core_dbt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.602090 soda_core_dbt-3.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-23 22:50:11.000000 soda_core_dbt-3.3.5/tests/test_dbt.py
```

### Comparing `soda_core_dbt-3.3.4/LICENSE` & `soda_core_dbt-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soda_core_dbt-3.3.4/soda/cloud/dbt.py` & `soda_core_dbt-3.3.5/soda/cloud/dbt.py`

 * *Files identical despite different names*

### Comparing `soda_core_dbt-3.3.4/soda/execution/check/dbt_check.py` & `soda_core_dbt-3.3.5/soda/execution/check/dbt_check.py`

 * *Files identical despite different names*

### Comparing `soda_core_dbt-3.3.4/tests/test_dbt.py` & `soda_core_dbt-3.3.5/tests/test_dbt.py`

 * *Files identical despite different names*

