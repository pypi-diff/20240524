# Comparing `tmp/xtalx-1.1.4.tar.gz` & `tmp/xtalx-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtalx-1.1.4.tar", last modified: Thu May 23 05:45:09 2024, max compression
+gzip compressed data, was "xtalx-1.1.5.tar", last modified: Thu May 23 20:13:04 2024, max compression
```

## Comparing `xtalx-1.1.4.tar` & `xtalx-1.1.5.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.330386 xtalx-1.1.4/
--rw-r--r--   0 greent7    (502) staff       (20)     1092 2023-07-27 00:41:10.000000 xtalx-1.1.4/LICENSE
--rw-r--r--   0 greent7    (502) staff       (20)     5401 2024-05-23 05:45:09.330327 xtalx-1.1.4/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)     4704 2023-09-12 00:58:41.000000 xtalx-1.1.4/README.rst
--rw-r--r--   0 greent7    (502) staff       (20)     1338 2024-05-23 05:45:09.330617 xtalx-1.1.4/setup.cfg
--rw-r--r--   0 greent7    (502) staff       (20)       38 2023-07-27 00:41:10.000000 xtalx-1.1.4/setup.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.324666 xtalx-1.1.4/xtalx/
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.326306 xtalx-1.1.4/xtalx/p_sensor/
--rw-r--r--   0 greent7    (502) staff       (20)      718 2023-08-04 23:44:45.000000 xtalx-1.1.4/xtalx/p_sensor/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      109 2023-08-04 23:44:45.000000 xtalx-1.1.4/xtalx/p_sensor/exception.py
--rw-r--r--   0 greent7    (502) staff       (20)    21608 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/p_sensor/xti.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.324615 xtalx-1.1.4/xtalx/tools/
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.326567 xtalx-1.1.4/xtalx/tools/config/
--rw-r--r--   0 greent7    (502) staff       (20)      203 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/tools/config/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      835 2024-04-03 23:21:00.000000 xtalx-1.1.4/xtalx/tools/config/config.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.326786 xtalx-1.1.4/xtalx/tools/csv/
--rw-r--r--   0 greent7    (502) staff       (20)      143 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/csv/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     1554 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/csv/decoder.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.326997 xtalx-1.1.4/xtalx/tools/influxdb/
--rw-r--r--   0 greent7    (502) staff       (20)       89 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/tools/influxdb/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     3405 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/influxdb/push_queue.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.327301 xtalx-1.1.4/xtalx/tools/math/
--rw-r--r--   0 greent7    (502) staff       (20)      215 2023-11-16 00:10:23.000000 xtalx-1.1.4/xtalx/tools/math/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     1273 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/tools/math/lorentz.py
--rw-r--r--   0 greent7    (502) staff       (20)     2667 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/math/xy_series.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.328030 xtalx-1.1.4/xtalx/tools/p_sensor/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2023-08-04 23:44:45.000000 xtalx-1.1.4/xtalx/tools/p_sensor/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     1597 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/p_sensor/csv_resample.py
--rw-r--r--   0 greent7    (502) staff       (20)      520 2023-08-04 23:44:45.000000 xtalx-1.1.4/xtalx/tools/p_sensor/discover.py
--rw-r--r--   0 greent7    (502) staff       (20)     8038 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/tools/p_sensor/gl_track_mode.py
--rw-r--r--   0 greent7    (502) staff       (20)      632 2024-04-03 23:28:49.000000 xtalx-1.1.4/xtalx/tools/p_sensor/xtalx_test_read.py
--rw-r--r--   0 greent7    (502) staff       (20)      789 2024-04-03 23:28:49.000000 xtalx-1.1.4/xtalx/tools/p_sensor/xtalx_test_read_async.py
--rw-r--r--   0 greent7    (502) staff       (20)     2687 2023-08-04 23:44:45.000000 xtalx-1.1.4/xtalx/tools/p_sensor/xtalx_test_yield.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.328136 xtalx-1.1.4/xtalx/tools/usb/
--rw-r--r--   0 greent7    (502) staff       (20)      977 2023-08-04 23:59:51.000000 xtalx-1.1.4/xtalx/tools/usb/__init__.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.329088 xtalx-1.1.4/xtalx/tools/z_sensor/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/tools/z_sensor/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)     1086 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/tools/z_sensor/cli_track_mode.py
--rw-r--r--   0 greent7    (502) staff       (20)      476 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/tools/z_sensor/discover.py
--rw-r--r--   0 greent7    (502) staff       (20)     3166 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/tools/z_sensor/get_info.py
--rw-r--r--   0 greent7    (502) staff       (20)     5345 2024-01-30 23:28:20.000000 xtalx-1.1.4/xtalx/tools/z_sensor/gl_scope_mode.py
--rw-r--r--   0 greent7    (502) staff       (20)     7231 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/tools/z_sensor/gl_sweep_mode.py
--rw-r--r--   0 greent7    (502) staff       (20)    16101 2024-05-21 22:41:40.000000 xtalx-1.1.4/xtalx/tools/z_sensor/gl_track_mode.py
--rw-r--r--   0 greent7    (502) staff       (20)    10119 2024-05-23 05:44:38.000000 xtalx-1.1.4/xtalx/tools/z_sensor/gl_wat_mode.py
--rw-r--r--   0 greent7    (502) staff       (20)     7162 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/tools/z_sensor/z_common.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.329958 xtalx-1.1.4/xtalx/z_sensor/
--rw-r--r--   0 greent7    (502) staff       (20)      976 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/z_sensor/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)    11028 2024-05-23 05:43:44.000000 xtalx-1.1.4/xtalx/z_sensor/peak_tracker.py
--rw-r--r--   0 greent7    (502) staff       (20)     5448 2023-09-12 00:58:41.000000 xtalx-1.1.4/xtalx/z_sensor/predicate_queue.py
--rw-r--r--   0 greent7    (502) staff       (20)      861 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/z_sensor/scope_data.py
--rw-r--r--   0 greent7    (502) staff       (20)     3588 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/z_sensor/sweeper.py
--rw-r--r--   0 greent7    (502) staff       (20)    21964 2024-03-25 22:34:49.000000 xtalx-1.1.4/xtalx/z_sensor/tcsc.py
--rw-r--r--   0 greent7    (502) staff       (20)      205 2023-08-04 23:45:01.000000 xtalx-1.1.4/xtalx/z_sensor/tcsc_u5.py
--rw-r--r--   0 greent7    (502) staff       (20)     1819 2023-09-13 20:20:19.000000 xtalx-1.1.4/xtalx/z_sensor/tincan.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 05:45:09.330112 xtalx-1.1.4/xtalx.egg-info/
--rw-r--r--   0 greent7    (502) staff       (20)     5401 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)     1398 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/SOURCES.txt
--rw-r--r--   0 greent7    (502) staff       (20)        1 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/dependency_links.txt
--rw-r--r--   0 greent7    (502) staff       (20)      434 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/entry_points.txt
--rw-r--r--   0 greent7    (502) staff       (20)       87 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/requires.txt
--rw-r--r--   0 greent7    (502) staff       (20)        6 2024-05-23 05:45:09.000000 xtalx-1.1.4/xtalx.egg-info/top_level.txt
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.432236 xtalx-1.1.5/
+-rw-r--r--   0 greent7    (502) staff       (20)     1092 2023-07-27 00:41:10.000000 xtalx-1.1.5/LICENSE
+-rw-r--r--   0 greent7    (502) staff       (20)     5401 2024-05-23 20:13:04.432165 xtalx-1.1.5/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)     4704 2023-09-12 00:58:41.000000 xtalx-1.1.5/README.rst
+-rw-r--r--   0 greent7    (502) staff       (20)     1338 2024-05-23 20:13:04.432468 xtalx-1.1.5/setup.cfg
+-rw-r--r--   0 greent7    (502) staff       (20)       38 2023-07-27 00:41:10.000000 xtalx-1.1.5/setup.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.426306 xtalx-1.1.5/xtalx/
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.427875 xtalx-1.1.5/xtalx/p_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)      718 2023-08-04 23:44:45.000000 xtalx-1.1.5/xtalx/p_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      109 2023-08-04 23:44:45.000000 xtalx-1.1.5/xtalx/p_sensor/exception.py
+-rw-r--r--   0 greent7    (502) staff       (20)    21608 2024-03-25 22:34:49.000000 xtalx-1.1.5/xtalx/p_sensor/xti.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.426254 xtalx-1.1.5/xtalx/tools/
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.428209 xtalx-1.1.5/xtalx/tools/config/
+-rw-r--r--   0 greent7    (502) staff       (20)      203 2023-09-12 00:58:41.000000 xtalx-1.1.5/xtalx/tools/config/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      835 2024-04-03 23:21:00.000000 xtalx-1.1.5/xtalx/tools/config/config.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.428428 xtalx-1.1.5/xtalx/tools/csv/
+-rw-r--r--   0 greent7    (502) staff       (20)      143 2024-03-25 22:34:49.000000 xtalx-1.1.5/xtalx/tools/csv/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1554 2024-03-25 22:34:49.000000 xtalx-1.1.5/xtalx/tools/csv/decoder.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.428635 xtalx-1.1.5/xtalx/tools/influxdb/
+-rw-r--r--   0 greent7    (502) staff       (20)       89 2023-09-12 00:58:41.000000 xtalx-1.1.5/xtalx/tools/influxdb/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3405 2024-03-25 22:34:49.000000 xtalx-1.1.5/xtalx/tools/influxdb/push_queue.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.428952 xtalx-1.1.5/xtalx/tools/math/
+-rw-r--r--   0 greent7    (502) staff       (20)      215 2023-11-16 00:10:23.000000 xtalx-1.1.5/xtalx/tools/math/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1273 2023-08-04 23:45:01.000000 xtalx-1.1.5/xtalx/tools/math/lorentz.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2667 2024-03-25 22:34:49.000000 xtalx-1.1.5/xtalx/tools/math/xy_series.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.429702 xtalx-1.1.5/xtalx/tools/p_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-08-04 23:44:45.000000 xtalx-1.1.5/xtalx/tools/p_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1597 2024-03-25 22:34:49.000000 xtalx-1.1.5/xtalx/tools/p_sensor/csv_resample.py
+-rw-r--r--   0 greent7    (502) staff       (20)      520 2023-08-04 23:44:45.000000 xtalx-1.1.5/xtalx/tools/p_sensor/discover.py
+-rw-r--r--   0 greent7    (502) staff       (20)     8038 2024-03-25 22:34:49.000000 xtalx-1.1.5/xtalx/tools/p_sensor/gl_track_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)      632 2024-04-03 23:28:49.000000 xtalx-1.1.5/xtalx/tools/p_sensor/xtalx_test_read.py
+-rw-r--r--   0 greent7    (502) staff       (20)      789 2024-04-03 23:28:49.000000 xtalx-1.1.5/xtalx/tools/p_sensor/xtalx_test_read_async.py
+-rw-r--r--   0 greent7    (502) staff       (20)     2687 2023-08-04 23:44:45.000000 xtalx-1.1.5/xtalx/tools/p_sensor/xtalx_test_yield.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.429808 xtalx-1.1.5/xtalx/tools/usb/
+-rw-r--r--   0 greent7    (502) staff       (20)      977 2023-08-04 23:59:51.000000 xtalx-1.1.5/xtalx/tools/usb/__init__.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.430937 xtalx-1.1.5/xtalx/tools/z_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-08-04 23:45:01.000000 xtalx-1.1.5/xtalx/tools/z_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1086 2023-09-12 00:58:41.000000 xtalx-1.1.5/xtalx/tools/z_sensor/cli_track_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)      476 2023-08-04 23:45:01.000000 xtalx-1.1.5/xtalx/tools/z_sensor/discover.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3166 2023-09-12 00:58:41.000000 xtalx-1.1.5/xtalx/tools/z_sensor/get_info.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5345 2024-01-30 23:28:20.000000 xtalx-1.1.5/xtalx/tools/z_sensor/gl_scope_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7231 2023-08-04 23:45:01.000000 xtalx-1.1.5/xtalx/tools/z_sensor/gl_sweep_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)    16101 2024-05-21 22:41:40.000000 xtalx-1.1.5/xtalx/tools/z_sensor/gl_track_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)    10186 2024-05-23 20:12:40.000000 xtalx-1.1.5/xtalx/tools/z_sensor/gl_wat_mode.py
+-rw-r--r--   0 greent7    (502) staff       (20)      523 2024-05-23 20:12:40.000000 xtalx-1.1.5/xtalx/tools/z_sensor/stop_crystal.py
+-rw-r--r--   0 greent7    (502) staff       (20)     7162 2023-09-12 00:58:41.000000 xtalx-1.1.5/xtalx/tools/z_sensor/z_common.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.431784 xtalx-1.1.5/xtalx/z_sensor/
+-rw-r--r--   0 greent7    (502) staff       (20)      976 2023-09-12 00:58:41.000000 xtalx-1.1.5/xtalx/z_sensor/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)    11056 2024-05-23 20:12:40.000000 xtalx-1.1.5/xtalx/z_sensor/peak_tracker.py
+-rw-r--r--   0 greent7    (502) staff       (20)     5448 2023-09-12 00:58:41.000000 xtalx-1.1.5/xtalx/z_sensor/predicate_queue.py
+-rw-r--r--   0 greent7    (502) staff       (20)      861 2023-08-04 23:45:01.000000 xtalx-1.1.5/xtalx/z_sensor/scope_data.py
+-rw-r--r--   0 greent7    (502) staff       (20)     3588 2023-08-04 23:45:01.000000 xtalx-1.1.5/xtalx/z_sensor/sweeper.py
+-rw-r--r--   0 greent7    (502) staff       (20)    21964 2024-03-25 22:34:49.000000 xtalx-1.1.5/xtalx/z_sensor/tcsc.py
+-rw-r--r--   0 greent7    (502) staff       (20)      205 2023-08-04 23:45:01.000000 xtalx-1.1.5/xtalx/z_sensor/tcsc_u5.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1819 2023-09-13 20:20:19.000000 xtalx-1.1.5/xtalx/z_sensor/tincan.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2024-05-23 20:13:04.431958 xtalx-1.1.5/xtalx.egg-info/
+-rw-r--r--   0 greent7    (502) staff       (20)     5401 2024-05-23 20:13:04.000000 xtalx-1.1.5/xtalx.egg-info/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)     1435 2024-05-23 20:13:04.000000 xtalx-1.1.5/xtalx.egg-info/SOURCES.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        1 2024-05-23 20:13:04.000000 xtalx-1.1.5/xtalx.egg-info/dependency_links.txt
+-rw-r--r--   0 greent7    (502) staff       (20)      434 2024-05-23 20:13:04.000000 xtalx-1.1.5/xtalx.egg-info/entry_points.txt
+-rw-r--r--   0 greent7    (502) staff       (20)       87 2024-05-23 20:13:04.000000 xtalx-1.1.5/xtalx.egg-info/requires.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        6 2024-05-23 20:13:04.000000 xtalx-1.1.5/xtalx.egg-info/top_level.txt
```

### Comparing `xtalx-1.1.4/LICENSE` & `xtalx-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/PKG-INFO` & `xtalx-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtalx
-Version: 1.1.4
+Version: 1.1.5
 Summary: Drivers and tools for the XtalX sensor family.
 Home-page: https://github.com/phasesensors/xtalx_python
 Author: Phase Advanced Sensor Systems Corp.
 Author-email: tgreeniaus@phasesensors.com
 License: MIT
 Keywords: xtalx
 Classifier: Operating System :: OS Independent
```

### Comparing `xtalx-1.1.4/README.rst` & `xtalx-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/setup.cfg` & `xtalx-1.1.5/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xtalx
-version = 1.1.4
+version = 1.1.5
 author = Phase Advanced Sensor Systems Corp.
 author_email = tgreeniaus@phasesensors.com
 description = Drivers and tools for the XtalX sensor family.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = xtalx
 url = https://github.com/phasesensors/xtalx_python
```

### Comparing `xtalx-1.1.4/xtalx/p_sensor/__init__.py` & `xtalx-1.1.5/xtalx/p_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/p_sensor/xti.py` & `xtalx-1.1.5/xtalx/p_sensor/xti.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/config/config.py` & `xtalx-1.1.5/xtalx/tools/config/config.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/csv/decoder.py` & `xtalx-1.1.5/xtalx/tools/csv/decoder.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/influxdb/push_queue.py` & `xtalx-1.1.5/xtalx/tools/influxdb/push_queue.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/math/lorentz.py` & `xtalx-1.1.5/xtalx/tools/math/lorentz.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/math/xy_series.py` & `xtalx-1.1.5/xtalx/tools/math/xy_series.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/p_sensor/csv_resample.py` & `xtalx-1.1.5/xtalx/tools/p_sensor/csv_resample.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/p_sensor/discover.py` & `xtalx-1.1.5/xtalx/tools/p_sensor/discover.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/p_sensor/gl_track_mode.py` & `xtalx-1.1.5/xtalx/tools/p_sensor/gl_track_mode.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/p_sensor/xtalx_test_read.py` & `xtalx-1.1.5/xtalx/tools/p_sensor/xtalx_test_read.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/p_sensor/xtalx_test_read_async.py` & `xtalx-1.1.5/xtalx/tools/p_sensor/xtalx_test_read_async.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/p_sensor/xtalx_test_yield.py` & `xtalx-1.1.5/xtalx/tools/p_sensor/xtalx_test_yield.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/usb/__init__.py` & `xtalx-1.1.5/xtalx/tools/usb/__init__.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/z_sensor/cli_track_mode.py` & `xtalx-1.1.5/xtalx/tools/z_sensor/cli_track_mode.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/z_sensor/get_info.py` & `xtalx-1.1.5/xtalx/tools/z_sensor/get_info.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/z_sensor/gl_scope_mode.py` & `xtalx-1.1.5/xtalx/tools/z_sensor/gl_scope_mode.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/z_sensor/gl_sweep_mode.py` & `xtalx-1.1.5/xtalx/tools/z_sensor/gl_sweep_mode.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/z_sensor/gl_track_mode.py` & `xtalx-1.1.5/xtalx/tools/z_sensor/gl_track_mode.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/tools/z_sensor/gl_wat_mode.py` & `xtalx-1.1.5/xtalx/tools/z_sensor/gl_wat_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         csv = open(  # pylint: disable=R1732
                 args.output_csv, 'a', encoding='utf8')
         csv.write('time_ns,dt,temp_c,peak_hz\n')
         csv.flush()
     else:
         csv = None
 
-    dev    = xtalx.z_sensor.find_one()
+    dev    = xtalx.z_sensor.find_one(serial_number=args.sensor)
     tc     = xtalx.z_sensor.make(dev, yield_Y=True)
     ww     = WATWindow(tc, csv)
     a      = tc.parse_amplitude(None)
     pt     = xtalx.z_sensor.PeakTracker(tc, a, PT_F0, PT_F1, PT_DF, PT_NFREQS,
                                         PT_SEARCH_TIME_SEC, PT_SWEEP_TIME_SEC,
                                         settle_ms=PT_SETTLE_TIME_MS,
                                         delegate=ww, enable_chirp=ENABLE_CHIRP)
@@ -269,13 +269,14 @@
     finally:
         pt.stop_threaded()
 
 
 def _main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--output-csv', '-o')
+    parser.add_argument('--sensor', '-s')
     args = parser.parse_args()
     main(args)
 
 
 if __name__ == '__main__':
     _main()
```

### Comparing `xtalx-1.1.4/xtalx/tools/z_sensor/z_common.py` & `xtalx-1.1.5/xtalx/tools/z_sensor/z_common.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/z_sensor/__init__.py` & `xtalx-1.1.5/xtalx/z_sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/z_sensor/peak_tracker.py` & `xtalx-1.1.5/xtalx/z_sensor/peak_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
         Start chirping and refine the data as it comes in.
         '''
         self.tc.info('Chirping from %f to %f...' % (CHIRP_F0, CHIRP_F1))
         self.tc.send_auto_chirp_cmd(CHIRP_F0, CHIRP_F1,
                                     round(self.tc.a_to_dac(CHIRP_A)))
         self._transition(State.CHIRP_WAIT_DATA)
         self.t_timeout = time.time() + CHIRP_DT
+        self.sweep_iter = 0
 
     def _start_peak_search(self, min_f, max_f, df):
         '''
         Do a fast sweep of the full frequency range to try and find the peak.
         '''
         min_f       = math.floor(min_f / df) * df
         max_f       = math.ceil(max_f / df) * df
```

### Comparing `xtalx-1.1.4/xtalx/z_sensor/predicate_queue.py` & `xtalx-1.1.5/xtalx/z_sensor/predicate_queue.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/z_sensor/scope_data.py` & `xtalx-1.1.5/xtalx/z_sensor/scope_data.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/z_sensor/sweeper.py` & `xtalx-1.1.5/xtalx/z_sensor/sweeper.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/z_sensor/tcsc.py` & `xtalx-1.1.5/xtalx/z_sensor/tcsc.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx/z_sensor/tincan.py` & `xtalx-1.1.5/xtalx/z_sensor/tincan.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.1.4/xtalx.egg-info/PKG-INFO` & `xtalx-1.1.5/xtalx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtalx
-Version: 1.1.4
+Version: 1.1.5
 Summary: Drivers and tools for the XtalX sensor family.
 Home-page: https://github.com/phasesensors/xtalx_python
 Author: Phase Advanced Sensor Systems Corp.
 Author-email: tgreeniaus@phasesensors.com
 License: MIT
 Keywords: xtalx
 Classifier: Operating System :: OS Independent
```

### Comparing `xtalx-1.1.4/xtalx.egg-info/SOURCES.txt` & `xtalx-1.1.5/xtalx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 xtalx/tools/z_sensor/cli_track_mode.py
 xtalx/tools/z_sensor/discover.py
 xtalx/tools/z_sensor/get_info.py
 xtalx/tools/z_sensor/gl_scope_mode.py
 xtalx/tools/z_sensor/gl_sweep_mode.py
 xtalx/tools/z_sensor/gl_track_mode.py
 xtalx/tools/z_sensor/gl_wat_mode.py
+xtalx/tools/z_sensor/stop_crystal.py
 xtalx/tools/z_sensor/z_common.py
 xtalx/z_sensor/__init__.py
 xtalx/z_sensor/peak_tracker.py
 xtalx/z_sensor/predicate_queue.py
 xtalx/z_sensor/scope_data.py
 xtalx/z_sensor/sweeper.py
 xtalx/z_sensor/tcsc.py
```

