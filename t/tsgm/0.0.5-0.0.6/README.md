# Comparing `tmp/tsgm-0.0.5.tar.gz` & `tmp/tsgm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsgm-0.0.5.tar", last modified: Sun Mar 24 18:06:03 2024, max compression
+gzip compressed data, was "tsgm-0.0.6.tar", last modified: Fri May 24 09:39:56 2024, max compression
```

## Comparing `tsgm-0.0.5.tar` & `tsgm-0.0.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-03-24 18:06:03.381103 tsgm-0.0.5/
--rw-r--r--   0 nikitia3   (502) staff       (20)    11357 2023-10-23 09:26:15.000000 tsgm-0.0.5/LICENSE
--rw-r--r--   0 nikitia3   (502) staff       (20)     7480 2024-03-24 18:06:03.380613 tsgm-0.0.5/PKG-INFO
--rw-r--r--   0 nikitia3   (502) staff       (20)     6647 2024-03-21 10:00:43.000000 tsgm-0.0.5/README.md
--rw-r--r--   0 nikitia3   (502) staff       (20)      339 2024-03-24 18:06:03.383470 tsgm-0.0.5/setup.cfg
--rw-r--r--   0 nikitia3   (502) staff       (20)     2302 2024-03-24 18:05:13.000000 tsgm-0.0.5/setup.py
-drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-03-24 18:06:03.198666 tsgm-0.0.5/tests/
--rw-r--r--   0 nikitia3   (502) staff       (20)     2365 2023-12-15 07:17:14.000000 tsgm-0.0.5/tests/test_abc.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     3578 2023-10-23 09:26:15.000000 tsgm-0.0.5/tests/test_augmentations.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     8975 2023-12-15 06:44:08.000000 tsgm-0.0.5/tests/test_cgan.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     1304 2024-03-14 13:28:15.000000 tsgm-0.0.5/tests/test_dataset.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     3609 2023-12-14 18:48:53.000000 tsgm-0.0.5/tests/test_downstream_models.py
--rw-r--r--   0 nikitia3   (502) staff       (20)    10107 2024-02-27 12:41:48.000000 tsgm-0.0.5/tests/test_metrics.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     2009 2023-12-14 18:50:26.000000 tsgm-0.0.5/tests/test_monitors.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     1311 2023-11-17 19:38:09.000000 tsgm-0.0.5/tests/test_simulator.py
--rw-r--r--   0 nikitia3   (502) staff       (20)      382 2023-12-15 07:16:34.000000 tsgm-0.0.5/tests/test_sts.py
--rw-r--r--   0 nikitia3   (502) staff       (20)    11667 2023-12-15 06:47:15.000000 tsgm-0.0.5/tests/test_timegan.py
--rw-r--r--   0 nikitia3   (502) staff       (20)    11626 2024-03-14 14:50:07.000000 tsgm-0.0.5/tests/test_utils.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     3118 2023-12-14 18:08:42.000000 tsgm-0.0.5/tests/test_vae.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     2401 2023-11-17 19:19:01.000000 tsgm-0.0.5/tests/test_visualizations.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     2761 2023-11-19 12:55:17.000000 tsgm-0.0.5/tests/test_zoo.py
-drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-03-24 18:06:03.210995 tsgm-0.0.5/tsgm/
--rw-r--r--   0 nikitia3   (502) staff       (20)      180 2024-03-14 14:48:53.000000 tsgm-0.0.5/tsgm/__init__.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     5284 2023-12-14 13:40:58.000000 tsgm-0.0.5/tsgm/dataset.py
-drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-03-24 18:06:03.234941 tsgm-0.0.5/tsgm/metrics/
--rw-r--r--   0 nikitia3   (502) staff       (20)      275 2024-02-27 12:12:07.000000 tsgm-0.0.5/tsgm/metrics/__init__.py
--rw-r--r--   0 nikitia3   (502) staff       (20)    16267 2024-03-14 14:41:08.000000 tsgm-0.0.5/tsgm/metrics/metrics.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     2368 2023-11-26 12:05:04.000000 tsgm-0.0.5/tsgm/metrics/statistics.py
-drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-03-24 18:06:03.308349 tsgm-0.0.5/tsgm/models/
--rw-r--r--   0 nikitia3   (502) staff       (20)      235 2023-10-23 09:26:15.000000 tsgm-0.0.5/tsgm/models/__init__.py
-drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-03-24 18:06:03.328521 tsgm-0.0.5/tsgm/models/architectures/
--rw-r--r--   0 nikitia3   (502) staff       (20)       58 2024-03-21 10:00:43.000000 tsgm-0.0.5/tsgm/models/architectures/__init__.py
--rw-r--r--   0 nikitia3   (502) staff       (20)    32146 2024-03-21 10:00:43.000000 tsgm-0.0.5/tsgm/models/architectures/zoo.py
--rw-r--r--   0 nikitia3   (502) staff       (20)    18204 2024-03-14 17:32:03.000000 tsgm-0.0.5/tsgm/models/augmentations.py
--rw-r--r--   0 nikitia3   (502) staff       (20)    13076 2024-03-14 18:07:01.000000 tsgm-0.0.5/tsgm/models/cgan.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     9007 2024-03-14 17:54:47.000000 tsgm-0.0.5/tsgm/models/cvae.py
--rw-r--r--   0 nikitia3   (502) staff       (20)       67 2023-10-23 09:26:15.000000 tsgm-0.0.5/tsgm/models/gp.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     6348 2024-03-15 09:14:54.000000 tsgm-0.0.5/tsgm/models/monitors.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     2731 2024-03-15 09:06:52.000000 tsgm-0.0.5/tsgm/models/sts.py
--rw-r--r--   0 nikitia3   (502) staff       (20)    22084 2024-03-21 10:00:43.000000 tsgm-0.0.5/tsgm/models/timeGAN.py
-drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-03-24 18:06:03.338168 tsgm-0.0.5/tsgm/optimization/
--rw-r--r--   0 nikitia3   (502) staff       (20)       29 2023-10-23 09:26:15.000000 tsgm-0.0.5/tsgm/optimization/__init__.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     3870 2024-03-14 18:06:17.000000 tsgm-0.0.5/tsgm/optimization/abc.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     3409 2023-11-26 14:44:23.000000 tsgm-0.0.5/tsgm/simulator.py
--rw-r--r--   0 nikitia3   (502) staff       (20)      190 2023-11-26 14:44:31.000000 tsgm-0.0.5/tsgm/types.py
-drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-03-24 18:06:03.377714 tsgm-0.0.5/tsgm/utils/
--rw-r--r--   0 nikitia3   (502) staff       (20)      310 2024-03-14 14:48:31.000000 tsgm-0.0.5/tsgm/utils/__init__.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     7999 2023-11-26 14:19:55.000000 tsgm-0.0.5/tsgm/utils/covid19_data_utils.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     4005 2024-03-15 09:08:19.000000 tsgm-0.0.5/tsgm/utils/data_processing.py
--rw-r--r--   0 nikitia3   (502) staff       (20)    22434 2024-03-15 09:03:42.000000 tsgm-0.0.5/tsgm/utils/datasets.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     2883 2023-11-26 14:33:42.000000 tsgm-0.0.5/tsgm/utils/file_utils.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     4866 2023-11-26 14:35:20.000000 tsgm-0.0.5/tsgm/utils/mmd.py
--rw-r--r--   0 nikitia3   (502) staff       (20)     2793 2023-11-26 14:35:58.000000 tsgm-0.0.5/tsgm/utils/utils.py
--rw-r--r--   0 nikitia3   (502) staff       (20)    12671 2024-03-15 09:14:46.000000 tsgm-0.0.5/tsgm/utils/visualization.py
--rw-r--r--   0 nikitia3   (502) staff       (20)       22 2024-03-24 18:01:28.000000 tsgm-0.0.5/tsgm/version.py
-drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-03-24 18:06:03.378970 tsgm-0.0.5/tsgm.egg-info/
--rw-r--r--   0 nikitia3   (502) staff       (20)     7480 2024-03-24 18:06:02.000000 tsgm-0.0.5/tsgm.egg-info/PKG-INFO
--rw-r--r--   0 nikitia3   (502) staff       (20)     1179 2024-03-24 18:06:02.000000 tsgm-0.0.5/tsgm.egg-info/SOURCES.txt
--rw-r--r--   0 nikitia3   (502) staff       (20)        1 2024-03-24 18:06:02.000000 tsgm-0.0.5/tsgm.egg-info/dependency_links.txt
--rw-r--r--   0 nikitia3   (502) staff       (20)       66 2024-03-24 18:06:02.000000 tsgm-0.0.5/tsgm.egg-info/entry_points.txt
--rw-r--r--   0 nikitia3   (502) staff       (20)      170 2024-03-24 18:06:02.000000 tsgm-0.0.5/tsgm.egg-info/requires.txt
--rw-r--r--   0 nikitia3   (502) staff       (20)        5 2024-03-24 18:06:02.000000 tsgm-0.0.5/tsgm.egg-info/top_level.txt
+drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-05-24 09:39:56.263019 tsgm-0.0.6/
+-rw-r--r--   0 nikitia3   (502) staff       (20)    11357 2023-10-23 09:26:15.000000 tsgm-0.0.6/LICENSE
+-rw-r--r--   0 nikitia3   (502) staff       (20)     7716 2024-05-24 09:39:56.262530 tsgm-0.0.6/PKG-INFO
+-rw-r--r--   0 nikitia3   (502) staff       (20)     6883 2024-05-24 09:23:07.000000 tsgm-0.0.6/README.md
+-rw-r--r--   0 nikitia3   (502) staff       (20)      339 2024-05-24 09:39:56.264991 tsgm-0.0.6/setup.cfg
+-rw-r--r--   0 nikitia3   (502) staff       (20)     2302 2024-05-24 09:23:07.000000 tsgm-0.0.6/setup.py
+drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-05-24 09:39:56.230498 tsgm-0.0.6/tests/
+-rw-r--r--   0 nikitia3   (502) staff       (20)     2365 2023-12-15 07:17:14.000000 tsgm-0.0.6/tests/test_abc.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     3578 2023-10-23 09:26:15.000000 tsgm-0.0.6/tests/test_augmentations.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     8975 2023-12-15 06:44:08.000000 tsgm-0.0.6/tests/test_cgan.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     1304 2024-03-14 13:28:15.000000 tsgm-0.0.6/tests/test_dataset.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     3609 2024-05-24 09:23:07.000000 tsgm-0.0.6/tests/test_downstream_models.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)    10171 2024-05-24 09:30:36.000000 tsgm-0.0.6/tests/test_metrics.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     2009 2024-05-24 09:23:07.000000 tsgm-0.0.6/tests/test_monitors.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     1311 2023-11-17 19:38:09.000000 tsgm-0.0.6/tests/test_simulator.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)      382 2023-12-15 07:16:34.000000 tsgm-0.0.6/tests/test_sts.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)    11667 2024-05-24 09:23:07.000000 tsgm-0.0.6/tests/test_timegan.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)    11626 2024-03-14 14:50:07.000000 tsgm-0.0.6/tests/test_utils.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     3118 2023-12-14 18:08:42.000000 tsgm-0.0.6/tests/test_vae.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     2401 2023-11-17 19:19:01.000000 tsgm-0.0.6/tests/test_visualizations.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     2761 2023-11-19 12:55:17.000000 tsgm-0.0.6/tests/test_zoo.py
+drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-05-24 09:39:56.234149 tsgm-0.0.6/tsgm/
+-rw-r--r--   0 nikitia3   (502) staff       (20)      180 2024-03-14 14:48:53.000000 tsgm-0.0.6/tsgm/__init__.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     5284 2023-12-14 13:40:58.000000 tsgm-0.0.6/tsgm/dataset.py
+drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-05-24 09:39:56.244493 tsgm-0.0.6/tsgm/metrics/
+-rw-r--r--   0 nikitia3   (502) staff       (20)      275 2024-02-27 12:12:07.000000 tsgm-0.0.6/tsgm/metrics/__init__.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)    16546 2024-05-24 09:30:36.000000 tsgm-0.0.6/tsgm/metrics/metrics.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     2368 2023-11-26 12:05:04.000000 tsgm-0.0.6/tsgm/metrics/statistics.py
+drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-05-24 09:39:56.251189 tsgm-0.0.6/tsgm/models/
+-rw-r--r--   0 nikitia3   (502) staff       (20)      235 2023-10-23 09:26:15.000000 tsgm-0.0.6/tsgm/models/__init__.py
+drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-05-24 09:39:56.252674 tsgm-0.0.6/tsgm/models/architectures/
+-rw-r--r--   0 nikitia3   (502) staff       (20)       58 2024-05-24 09:23:07.000000 tsgm-0.0.6/tsgm/models/architectures/__init__.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)    32146 2024-05-24 09:23:07.000000 tsgm-0.0.6/tsgm/models/architectures/zoo.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)    18287 2024-05-24 09:23:07.000000 tsgm-0.0.6/tsgm/models/augmentations.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)    13076 2024-03-14 18:07:01.000000 tsgm-0.0.6/tsgm/models/cgan.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     9007 2024-03-14 17:54:47.000000 tsgm-0.0.6/tsgm/models/cvae.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)       67 2023-10-23 09:26:15.000000 tsgm-0.0.6/tsgm/models/gp.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     6348 2024-03-27 09:28:27.000000 tsgm-0.0.6/tsgm/models/monitors.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     2731 2024-03-15 09:06:52.000000 tsgm-0.0.6/tsgm/models/sts.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)    22084 2024-05-24 09:23:07.000000 tsgm-0.0.6/tsgm/models/timeGAN.py
+drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-05-24 09:39:56.253971 tsgm-0.0.6/tsgm/optimization/
+-rw-r--r--   0 nikitia3   (502) staff       (20)       29 2023-10-23 09:26:15.000000 tsgm-0.0.6/tsgm/optimization/__init__.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     3870 2024-03-14 18:06:17.000000 tsgm-0.0.6/tsgm/optimization/abc.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     3409 2023-11-26 14:44:23.000000 tsgm-0.0.6/tsgm/simulator.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)      190 2023-11-26 14:44:31.000000 tsgm-0.0.6/tsgm/types.py
+drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-05-24 09:39:56.260967 tsgm-0.0.6/tsgm/utils/
+-rw-r--r--   0 nikitia3   (502) staff       (20)      310 2024-03-14 14:48:31.000000 tsgm-0.0.6/tsgm/utils/__init__.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     7999 2023-11-26 14:19:55.000000 tsgm-0.0.6/tsgm/utils/covid19_data_utils.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     4005 2024-03-15 09:08:19.000000 tsgm-0.0.6/tsgm/utils/data_processing.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)    22434 2024-03-15 09:03:42.000000 tsgm-0.0.6/tsgm/utils/datasets.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     2883 2023-11-26 14:33:42.000000 tsgm-0.0.6/tsgm/utils/file_utils.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     4866 2023-11-26 14:35:20.000000 tsgm-0.0.6/tsgm/utils/mmd.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)     2793 2024-05-24 09:23:07.000000 tsgm-0.0.6/tsgm/utils/utils.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)    12671 2024-03-15 09:14:46.000000 tsgm-0.0.6/tsgm/utils/visualization.py
+-rw-r--r--   0 nikitia3   (502) staff       (20)       22 2024-05-24 09:39:02.000000 tsgm-0.0.6/tsgm/version.py
+drwxr-xr-x   0 nikitia3   (502) staff       (20)        0 2024-05-24 09:39:56.242309 tsgm-0.0.6/tsgm.egg-info/
+-rw-r--r--   0 nikitia3   (502) staff       (20)     7716 2024-05-24 09:39:56.000000 tsgm-0.0.6/tsgm.egg-info/PKG-INFO
+-rw-r--r--   0 nikitia3   (502) staff       (20)     1179 2024-05-24 09:39:56.000000 tsgm-0.0.6/tsgm.egg-info/SOURCES.txt
+-rw-r--r--   0 nikitia3   (502) staff       (20)        1 2024-05-24 09:39:56.000000 tsgm-0.0.6/tsgm.egg-info/dependency_links.txt
+-rw-r--r--   0 nikitia3   (502) staff       (20)       66 2024-05-24 09:39:56.000000 tsgm-0.0.6/tsgm.egg-info/entry_points.txt
+-rw-r--r--   0 nikitia3   (502) staff       (20)      170 2024-05-24 09:39:56.000000 tsgm-0.0.6/tsgm.egg-info/requires.txt
+-rw-r--r--   0 nikitia3   (502) staff       (20)        5 2024-05-24 09:39:56.000000 tsgm-0.0.6/tsgm.egg-info/top_level.txt
```

### Comparing `tsgm-0.0.5/LICENSE` & `tsgm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/PKG-INFO` & `tsgm-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsgm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Time Series Generative Modelling Framework
 Home-page: https://github.com/AlexanderVNikitin/tsgm
 Download-URL: 
 Author: Alexander Nikitin
 Author-email: 
 Maintainer: Alexander Nikitin
 Maintainer-email: 
@@ -149,17 +149,18 @@
 ## Augmentations
 TSGM provides a number of time series augmentations.
 
 | Augmentation  | Class in TSGM | Reference     |
 | ------------- | ------------- | ------------- |
 | Gaussian Noise / Jittering  | `tsgm.augmentations.GaussianNoise` | -  |        
 | Slice-And-Shuffle  | `tsgm.augmentations.SliceAndShuffle` | - |
-| Shuffle features  | `tsgm.augmentations.Shuffle` | - |
-| Magnitude warping  | `tsgm.augmentations.MagnitudeWarping` | [Data Augmentation of Wearable Sensor Data for Parkinson’s Disease Monitoring using Convolutional Neural Networks](https://dl.acm.org/doi/pdf/10.1145/3136755.3136817) |
-| Window warping  | `tsgm.augmentations.WindowWarping` | [Data Augmentation for Time Series Classification using Convolutional Neural Networks](https://shs.hal.science/halshs-01357973/document) |
+| Shuffle Features  | `tsgm.augmentations.Shuffle` | - |
+| Magnitude Warping  | `tsgm.augmentations.MagnitudeWarping` | [Data Augmentation of Wearable Sensor Data for Parkinson’s Disease Monitoring using Convolutional Neural Networks](https://dl.acm.org/doi/pdf/10.1145/3136755.3136817) |
+| Window Warping  | `tsgm.augmentations.WindowWarping` | [Data Augmentation for Time Series Classification using Convolutional Neural Networks](https://shs.hal.science/halshs-01357973/document) |
+| DTW Barycentric Averaging  | `tsgm.augmentations.DTWBarycentricAveraging` | [A global averaging method for dynamic time warping, with applications to clustering.](https://www.sciencedirect.com/science/article/pii/S003132031000453X) |
 
 
 ## Contributing
 We appreciate all contributions. To learn more, please check [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Citing
 If you find this repo useful, please consider citing our paper:
```

### Comparing `tsgm-0.0.5/README.md` & `tsgm-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -121,17 +121,18 @@
 ## Augmentations
 TSGM provides a number of time series augmentations.
 
 | Augmentation  | Class in TSGM | Reference     |
 | ------------- | ------------- | ------------- |
 | Gaussian Noise / Jittering  | `tsgm.augmentations.GaussianNoise` | -  |        
 | Slice-And-Shuffle  | `tsgm.augmentations.SliceAndShuffle` | - |
-| Shuffle features  | `tsgm.augmentations.Shuffle` | - |
-| Magnitude warping  | `tsgm.augmentations.MagnitudeWarping` | [Data Augmentation of Wearable Sensor Data for Parkinson’s Disease Monitoring using Convolutional Neural Networks](https://dl.acm.org/doi/pdf/10.1145/3136755.3136817) |
-| Window warping  | `tsgm.augmentations.WindowWarping` | [Data Augmentation for Time Series Classification using Convolutional Neural Networks](https://shs.hal.science/halshs-01357973/document) |
+| Shuffle Features  | `tsgm.augmentations.Shuffle` | - |
+| Magnitude Warping  | `tsgm.augmentations.MagnitudeWarping` | [Data Augmentation of Wearable Sensor Data for Parkinson’s Disease Monitoring using Convolutional Neural Networks](https://dl.acm.org/doi/pdf/10.1145/3136755.3136817) |
+| Window Warping  | `tsgm.augmentations.WindowWarping` | [Data Augmentation for Time Series Classification using Convolutional Neural Networks](https://shs.hal.science/halshs-01357973/document) |
+| DTW Barycentric Averaging  | `tsgm.augmentations.DTWBarycentricAveraging` | [A global averaging method for dynamic time warping, with applications to clustering.](https://www.sciencedirect.com/science/article/pii/S003132031000453X) |
 
 
 ## Contributing
 We appreciate all contributions. To learn more, please check [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Citing
 If you find this repo useful, please consider citing our paper:
```

### Comparing `tsgm-0.0.5/setup.py` & `tsgm-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_abc.py` & `tsgm-0.0.6/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_augmentations.py` & `tsgm-0.0.6/tests/test_augmentations.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_cgan.py` & `tsgm-0.0.6/tests/test_cgan.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_dataset.py` & `tsgm-0.0.6/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_downstream_models.py` & `tsgm-0.0.6/tests/test_downstream_models.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_metrics.py` & `tsgm-0.0.6/tests/test_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,26 +187,27 @@
     assert mmd_metric(ts, ts) == 0 and mmd_metric(diff_ts, diff_ts) == 0
 
     assert mmd_metric(D1, D2) == mmd_metric(ts, diff_ts)
     assert mmd_metric(D1, D1) == 0 and mmd_metric(D2, D2) == 0
 
 
 def test_discriminative_metric():
-    ts = np.array([[[0, 2], [11, -11], [1, 2]], [[10, 21], [1, -1], [6, 8]]]).astype(np.float32)
+    ts = np.sin(np.arange(10)[:, None, None] + np.arange(6)[None, :, None])  # sin_sequence, [10, 6, 3]
     D1 = tsgm.dataset.Dataset(ts, y=None)
 
-    diff_ts = np.array([[[12, 13], [10, 10], [-1, -2]], [[-1, 32], [2, 1], [10, 8]]]).astype(np.float32)
+    diff_ts = np.sin(np.arange(10)[:, None, None] + np.arange(6)[None, :, None]) + 1000  # sin_sequence, [10, 6, 3]
     D2 = tsgm.dataset.Dataset(diff_ts, y=None)
 
-    model = tsgm.models.zoo["clf_cl_n"](seq_len=ts.shape[1], feat_dim=ts.shape[2], output_dim=1).model
+    model = tsgm.models.zoo["clf_cl_n"](seq_len=ts.shape[1], feat_dim=ts.shape[2], output_dim=2).model
     model.compile(
         tf.keras.optimizers.Adam(),
-        tf.keras.losses.CategoricalCrossentropy(from_logits=True)
+        tf.keras.losses.SparseCategoricalCrossentropy(from_logits=False)
     )
     discr_metric = tsgm.metrics.DiscriminativeMetric()
+    # should be easy to be classified 
     assert discr_metric(d_hist=D1, d_syn=D2, model=model, test_size=0.2, random_seed=42, n_epochs=5) == 1.0
     assert discr_metric(d_hist=D1, d_syn=D2, model=model, metric=sklearn.metrics.precision_score, test_size=0.2, random_seed=42, n_epochs=5) == 1.0
 
 
 def test_entropy_metric():
     ts = np.array([[[0, 2], [11, -11], [1, 2]], [[10, 21], [1, -1], [6, 8]]]).astype(np.float32)
     D1 = tsgm.dataset.Dataset(ts, y=None)
```

### Comparing `tsgm-0.0.5/tests/test_monitors.py` & `tsgm-0.0.6/tests/test_monitors.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_simulator.py` & `tsgm-0.0.6/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_timegan.py` & `tsgm-0.0.6/tests/test_timegan.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_utils.py` & `tsgm-0.0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_vae.py` & `tsgm-0.0.6/tests/test_vae.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_visualizations.py` & `tsgm-0.0.6/tests/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tests/test_zoo.py` & `tsgm-0.0.6/tests/test_zoo.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/dataset.py` & `tsgm-0.0.6/tsgm/dataset.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/metrics/metrics.py` & `tsgm-0.0.6/tsgm/metrics/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,20 @@
     >>> print(result)
     """
     def __call__(self, d_hist: tsgm.dataset.DatasetOrTensor, d_syn: tsgm.dataset.DatasetOrTensor, model: T.Callable, test_size: T.Union[float, int], n_epochs: int, metric: T.Optional[T.Callable] = None, random_seed: T.Optional[int] = None) -> float:
         X_hist, X_syn = _dataset_or_tensor_to_tensor(d_hist), _dataset_or_tensor_to_tensor(d_syn)
         X_all, y_all = np.concatenate([X_hist, X_syn]), np.concatenate([[1] * len(d_hist), [0] * len(d_syn)])
         X_train, X_test, y_train, y_test = sklearn.model_selection.train_test_split(X_all, y_all, test_size=test_size, random_state=random_seed)
         model.fit(X_train, y_train, epochs=n_epochs)
-        y_pred = (model.predict(X_test) > 0.5).astype(int)
+        pred = model.predict(X_test)
+        # check the shape, 1D array or N-D arrary
+        if len(pred.shape) == 1:  # binary classification with sigmoid activation
+            y_pred = (pred > 0.5).astype(int)
+        else:  # multiple classification with softmax activation
+            y_pred = np.argmax(pred, axis=-1).astype(int)
         if metric is None:
             return sklearn.metrics.accuracy_score(y_test, y_pred)
         else:
             return metric(y_test, y_pred)
 
 
 def _spectral_entropy_per_feature(X: TensorLike) -> TensorLike:
```

### Comparing `tsgm-0.0.5/tsgm/metrics/statistics.py` & `tsgm-0.0.6/tsgm/metrics/statistics.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/models/architectures/zoo.py` & `tsgm-0.0.6/tsgm/models/architectures/zoo.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/models/augmentations.py` & `tsgm-0.0.6/tsgm/models/augmentations.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,16 @@
                 start_idx = 0
                 for j in sorted(idxs):
                     s = sequence[start_idx:j]
                     start_idx = j
                     slices.append(s)
                 slices.append(sequence[start_idx:])
                 np.random.shuffle(slices)
+            # concatenate the slices
+            sequence = np.concatenate(slices)
             synthetic_data.append(sequence)
             if has_labels:
                 new_labels.append(y[i])
         if has_labels:
             return np.array(synthetic_data), np.array(new_labels)
         else:
             return np.array(synthetic_data)
```

### Comparing `tsgm-0.0.5/tsgm/models/cgan.py` & `tsgm-0.0.6/tsgm/models/cgan.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/models/cvae.py` & `tsgm-0.0.6/tsgm/models/cvae.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/models/monitors.py` & `tsgm-0.0.6/tsgm/models/monitors.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/models/sts.py` & `tsgm-0.0.6/tsgm/models/sts.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/models/timeGAN.py` & `tsgm-0.0.6/tsgm/models/timeGAN.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/optimization/abc.py` & `tsgm-0.0.6/tsgm/optimization/abc.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/simulator.py` & `tsgm-0.0.6/tsgm/simulator.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/utils/covid19_data_utils.py` & `tsgm-0.0.6/tsgm/utils/covid19_data_utils.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/utils/data_processing.py` & `tsgm-0.0.6/tsgm/utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/utils/datasets.py` & `tsgm-0.0.6/tsgm/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/utils/file_utils.py` & `tsgm-0.0.6/tsgm/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/utils/mmd.py` & `tsgm-0.0.6/tsgm/utils/mmd.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/utils/utils.py` & `tsgm-0.0.6/tsgm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm/utils/visualization.py` & `tsgm-0.0.6/tsgm/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `tsgm-0.0.5/tsgm.egg-info/PKG-INFO` & `tsgm-0.0.6/tsgm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsgm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Time Series Generative Modelling Framework
 Home-page: https://github.com/AlexanderVNikitin/tsgm
 Download-URL: 
 Author: Alexander Nikitin
 Author-email: 
 Maintainer: Alexander Nikitin
 Maintainer-email: 
@@ -149,17 +149,18 @@
 ## Augmentations
 TSGM provides a number of time series augmentations.
 
 | Augmentation  | Class in TSGM | Reference     |
 | ------------- | ------------- | ------------- |
 | Gaussian Noise / Jittering  | `tsgm.augmentations.GaussianNoise` | -  |        
 | Slice-And-Shuffle  | `tsgm.augmentations.SliceAndShuffle` | - |
-| Shuffle features  | `tsgm.augmentations.Shuffle` | - |
-| Magnitude warping  | `tsgm.augmentations.MagnitudeWarping` | [Data Augmentation of Wearable Sensor Data for Parkinson’s Disease Monitoring using Convolutional Neural Networks](https://dl.acm.org/doi/pdf/10.1145/3136755.3136817) |
-| Window warping  | `tsgm.augmentations.WindowWarping` | [Data Augmentation for Time Series Classification using Convolutional Neural Networks](https://shs.hal.science/halshs-01357973/document) |
+| Shuffle Features  | `tsgm.augmentations.Shuffle` | - |
+| Magnitude Warping  | `tsgm.augmentations.MagnitudeWarping` | [Data Augmentation of Wearable Sensor Data for Parkinson’s Disease Monitoring using Convolutional Neural Networks](https://dl.acm.org/doi/pdf/10.1145/3136755.3136817) |
+| Window Warping  | `tsgm.augmentations.WindowWarping` | [Data Augmentation for Time Series Classification using Convolutional Neural Networks](https://shs.hal.science/halshs-01357973/document) |
+| DTW Barycentric Averaging  | `tsgm.augmentations.DTWBarycentricAveraging` | [A global averaging method for dynamic time warping, with applications to clustering.](https://www.sciencedirect.com/science/article/pii/S003132031000453X) |
 
 
 ## Contributing
 We appreciate all contributions. To learn more, please check [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Citing
 If you find this repo useful, please consider citing our paper:
```

### Comparing `tsgm-0.0.5/tsgm.egg-info/SOURCES.txt` & `tsgm-0.0.6/tsgm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

