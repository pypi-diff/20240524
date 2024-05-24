# Comparing `tmp/siglost_utils-0.1.4.tar.gz` & `tmp/siglost_utils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siglost_utils-0.1.4.tar", last modified: Fri May 24 02:52:03 2024, max compression
+gzip compressed data, was "siglost_utils-0.1.5.tar", last modified: Fri May 24 03:03:06 2024, max compression
```

## Comparing `siglost_utils-0.1.4.tar` & `siglost_utils-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 02:52:03.277471 siglost_utils-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils/api/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils/display/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/display/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils/inference/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/inference/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/utils/log_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 02:52:03.000000 siglost_utils-0.1.4/siglost_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-24 02:52:03.000000 siglost_utils-0.1.4/siglost_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:52:03.000000 siglost_utils-0.1.4/siglost_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 02:52:03.000000 siglost_utils-0.1.4/siglost_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/tests/test_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.045586 siglost_utils-0.1.5/siglost_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/siglost_utils/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/siglost_utils/display/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/display/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/siglost_utils/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/inference/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/siglost_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/utils/log_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/siglost_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 03:03:06.000000 siglost_utils-0.1.5/siglost_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-24 03:03:06.000000 siglost_utils-0.1.5/siglost_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:03:06.000000 siglost_utils-0.1.5/siglost_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 03:03:06.000000 siglost_utils-0.1.5/siglost_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/tests/test_display.py
```

### Comparing `siglost_utils-0.1.4/LICENSE` & `siglost_utils-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.4/PKG-INFO` & `siglost_utils-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `siglost_utils-0.1.4/setup.cfg` & `siglost_utils-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.4/siglost_utils/display/display.py` & `siglost_utils-0.1.5/siglost_utils/display/display.py`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.4/siglost_utils/inference/inference.py` & `siglost_utils-0.1.5/siglost_utils/inference/inference.py`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.4/siglost_utils/utils/log_events.py` & `siglost_utils-0.1.5/siglost_utils/utils/log_events.py`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.4/siglost_utils.egg-info/PKG-INFO` & `siglost_utils-0.1.5/siglost_utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `siglost_utils-0.1.4/tests/test_display.py` & `siglost_utils-0.1.5/tests/test_display.py`

 * *Files identical despite different names*

