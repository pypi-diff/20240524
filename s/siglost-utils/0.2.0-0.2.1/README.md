# Comparing `tmp/siglost_utils-0.2.0.tar.gz` & `tmp/siglost_utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siglost_utils-0.2.0.tar", last modified: Fri May 24 03:25:58 2024, max compression
+gzip compressed data, was "siglost_utils-0.2.1.tar", last modified: Fri May 24 03:33:43 2024, max compression
```

## Comparing `siglost_utils-0.2.0.tar` & `siglost_utils-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.934724 siglost_utils-0.2.0/siglost_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.934724 siglost_utils-0.2.0/siglost_utils/api/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.934724 siglost_utils-0.2.0/siglost_utils/display/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/display/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/siglost_utils/inference/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16528 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/inference/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/siglost_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/utils/extras.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/utils/log_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/siglost_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 03:25:58.000000 siglost_utils-0.2.0/siglost_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-24 03:25:58.000000 siglost_utils-0.2.0/siglost_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:25:58.000000 siglost_utils-0.2.0/siglost_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 03:25:58.000000 siglost_utils-0.2.0/siglost_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/tests/test_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:33:43.792829 siglost_utils-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 03:33:43.792829 siglost_utils-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 03:33:43.792829 siglost_utils-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:33:43.788829 siglost_utils-0.2.1/siglost_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/siglost_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:33:43.788829 siglost_utils-0.2.1/siglost_utils/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/siglost_utils/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/siglost_utils/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:33:43.788829 siglost_utils-0.2.1/siglost_utils/display/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/siglost_utils/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/siglost_utils/display/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:33:43.788829 siglost_utils-0.2.1/siglost_utils/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/siglost_utils/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16528 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/siglost_utils/inference/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:33:43.788829 siglost_utils-0.2.1/siglost_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/siglost_utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/siglost_utils/utils/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/siglost_utils/utils/log_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:33:43.788829 siglost_utils-0.2.1/siglost_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 03:33:43.000000 siglost_utils-0.2.1/siglost_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-24 03:33:43.000000 siglost_utils-0.2.1/siglost_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:33:43.000000 siglost_utils-0.2.1/siglost_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 03:33:43.000000 siglost_utils-0.2.1/siglost_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:33:43.788829 siglost_utils-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 03:33:31.000000 siglost_utils-0.2.1/tests/test_display.py
```

### Comparing `siglost_utils-0.2.0/LICENSE` & `siglost_utils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.2.0/PKG-INFO` & `siglost_utils-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `siglost_utils-0.2.0/setup.cfg` & `siglost_utils-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.2.0/siglost_utils/display/display.py` & `siglost_utils-0.2.1/siglost_utils/display/display.py`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.2.0/siglost_utils/inference/inference.py` & `siglost_utils-0.2.1/siglost_utils/inference/inference.py`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.2.0/siglost_utils/utils/extras.py` & `siglost_utils-0.2.1/siglost_utils/utils/extras.py`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.2.0/siglost_utils/utils/log_events.py` & `siglost_utils-0.2.1/siglost_utils/utils/log_events.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,7 +46,19 @@
         LogEvents.log_event("debug", "deployment.debug.node", f"{node_id} : {object_to_log}")
 
 
     @staticmethod
     def conditional_debug_log(object_to_log, condition, node_id=""):
         if condition:
             print("{} : {}".format(node_id, object_to_log))
+
+
+# Expose methods at the module level
+#     This is necessary if you want to import these methods directly from log_events.py without referencing the LogEvents class.
+#     This setup allows you to re-export these methods in the __init__.py file of the utils module, making them directly
+#     accessible when importing from lumeo.utils.
+log_event = LogEvents.log_event
+error_log = LogEvents.error_log
+warning_log = LogEvents.warning_log
+info_log = LogEvents.info_log
+debug_log = LogEvents.debug_log
+conditional_debug_log = LogEvents.conditional_debug_log
```

### Comparing `siglost_utils-0.2.0/siglost_utils.egg-info/PKG-INFO` & `siglost_utils-0.2.1/siglost_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `siglost_utils-0.2.0/siglost_utils.egg-info/SOURCES.txt` & `siglost_utils-0.2.1/siglost_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.2.0/tests/test_display.py` & `siglost_utils-0.2.1/tests/test_display.py`

 * *Files identical despite different names*

