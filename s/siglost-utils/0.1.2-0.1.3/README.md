# Comparing `tmp/siglost_utils-0.1.2.tar.gz` & `tmp/siglost_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siglost_utils-0.1.2.tar", last modified: Wed May  8 01:09:32 2024, max compression
+gzip compressed data, was "siglost_utils-0.1.3.tar", last modified: Fri May 24 02:11:50 2024, max compression
```

## Comparing `siglost_utils-0.1.2.tar` & `siglost_utils-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:09:32.131605 siglost_utils-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 01:09:19.000000 siglost_utils-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 01:09:32.131605 siglost_utils-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 01:09:19.000000 siglost_utils-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-08 01:09:32.131605 siglost_utils-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-08 01:09:19.000000 siglost_utils-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:09:32.127606 siglost_utils-0.1.2/siglost_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 01:09:19.000000 siglost_utils-0.1.2/siglost_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 01:09:19.000000 siglost_utils-0.1.2/siglost_utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:09:32.131605 siglost_utils-0.1.2/siglost_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-08 01:09:32.000000 siglost_utils-0.1.2/siglost_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-08 01:09:32.000000 siglost_utils-0.1.2/siglost_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:09:32.000000 siglost_utils-0.1.2/siglost_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 01:09:32.000000 siglost_utils-0.1.2/siglost_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:09:32.131605 siglost_utils-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 01:09:19.000000 siglost_utils-0.1.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils/display/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/display/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/inference/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/utils/log_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 02:11:50.000000 siglost_utils-0.1.3/siglost_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-24 02:11:50.000000 siglost_utils-0.1.3/siglost_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:11:50.000000 siglost_utils-0.1.3/siglost_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 02:11:50.000000 siglost_utils-0.1.3/siglost_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/tests/test_display.py
```

### Comparing `siglost_utils-0.1.2/LICENSE` & `siglost_utils-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.2/PKG-INFO` & `siglost_utils-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `siglost_utils-0.1.2/setup.cfg` & `siglost_utils-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.2/siglost_utils.egg-info/PKG-INFO` & `siglost_utils-0.1.3/siglost_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

