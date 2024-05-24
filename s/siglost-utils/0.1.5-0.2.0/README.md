# Comparing `tmp/siglost_utils-0.1.5.tar.gz` & `tmp/siglost_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siglost_utils-0.1.5.tar", last modified: Fri May 24 03:03:06 2024, max compression
+gzip compressed data, was "siglost_utils-0.2.0.tar", last modified: Fri May 24 03:25:58 2024, max compression
```

## Comparing `siglost_utils-0.1.5.tar` & `siglost_utils-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.045586 siglost_utils-0.1.5/siglost_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/siglost_utils/api/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/siglost_utils/display/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/display/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/siglost_utils/inference/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/inference/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/siglost_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/siglost_utils/utils/log_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/siglost_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 03:03:06.000000 siglost_utils-0.1.5/siglost_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-24 03:03:06.000000 siglost_utils-0.1.5/siglost_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:03:06.000000 siglost_utils-0.1.5/siglost_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 03:03:06.000000 siglost_utils-0.1.5/siglost_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:06.049586 siglost_utils-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 03:02:55.000000 siglost_utils-0.1.5/tests/test_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.934724 siglost_utils-0.2.0/siglost_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.934724 siglost_utils-0.2.0/siglost_utils/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.934724 siglost_utils-0.2.0/siglost_utils/display/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/display/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/siglost_utils/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16528 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/inference/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/siglost_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/utils/extras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/siglost_utils/utils/log_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/siglost_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 03:25:58.000000 siglost_utils-0.2.0/siglost_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-24 03:25:58.000000 siglost_utils-0.2.0/siglost_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:25:58.000000 siglost_utils-0.2.0/siglost_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 03:25:58.000000 siglost_utils-0.2.0/siglost_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:58.938724 siglost_utils-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 03:25:45.000000 siglost_utils-0.2.0/tests/test_display.py
```

### Comparing `siglost_utils-0.1.5/LICENSE` & `siglost_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.5/PKG-INFO` & `siglost_utils-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.1.5
+Version: 0.2.0
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `siglost_utils-0.1.5/setup.cfg` & `siglost_utils-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.5/siglost_utils/display/display.py` & `siglost_utils-0.2.0/siglost_utils/display/display.py`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.5/siglost_utils/inference/inference.py` & `siglost_utils-0.2.0/siglost_utils/inference/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from lumeopipeline import Utils
 import os
 import time
 import numpy as np
 import contextlib
 from urllib.parse import urlsplit
 
-from siglost_utils.utils.log_events import conditional_debug_log, error_log
-from siglost_utils.utils.command_utils import run_command
+from siglost_utils.utils import conditional_debug_log, error_log
+from siglost_utils.utils import run_command
 
 tritonclient = Utils.install_import('tritonclient[http]', version='2.33')
 import tritonclient.utils.shared_memory as shm
 
 
 class TritonRemoteModelUsingSHM:
   """
@@ -87,30 +87,30 @@
 
     triton_model_file = f"/var/lib/lumeo/models/triton_model_repo/{self.model_name}/1/{self.model_name}.onnx"
     return os.path.exists(triton_model_file)
 
   def clear_cache(self):
     triton_cache_path = f"/var/lib/lumeo/models/triton_model_cache/{self.model_name}"
     triton_model_path = f"/var/lib/lumeo/models/triton_model_repo/{self.model_name}"
-    run_command(f"rm -rf {triton_cache_path}", None, 'Clearing Triton cache')
-    run_command(f"rm -rf {triton_model_path}", None, 'Clearing Triton model')
+    run_command(f"rm -rf {triton_cache_path}", None, 'Clearing Triton cache', node_id=self.node_id)
+    run_command(f"rm -rf {triton_model_path}", None, 'Clearing Triton model', node_id=self.node_id)
 
   def install_model(self, onnx_file, enable_trt=False):
 
     # Ref : https://github.com/triton-inference-server/tutorials/blob/main/Conceptual_Guide/Part_4-inference_acceleration/README.md
 
     triton_model_file = f"/var/lib/lumeo/models/triton_model_repo/{self.model_name}/1/{self.model_name}.onnx"
     triton_model_config = f"/var/lib/lumeo/models/triton_model_repo/{self.model_name}/config.pbtxt"
     triton_cache_path = f"/var/lib/lumeo/models/triton_model_cache/{self.model_name}"
 
     # make directory
     os.makedirs(os.path.dirname(triton_model_file), exist_ok=True)
     os.makedirs(triton_cache_path, exist_ok=True)
 
-    run_command(f"mv -f {onnx_file} {triton_model_file}", None, 'Moving ONNX file to triton model directory')
+    run_command(f"mv -f {onnx_file} {triton_model_file}", None, 'Moving ONNX file to triton model directory', node_id=self.node_id)
 
     # TRT execution provider for ONNX runtime will create TRT engine, and
     # cache it to the specified directory.
     # Ref : https://github.com/triton-inference-server/onnxruntime_backend
     model_config = (f"name: \"{self.model_name}\"\n"
                     "platform: \"onnxruntime_onnx\"\n"
                     "max_batch_size: 1\n"
```

### Comparing `siglost_utils-0.1.5/siglost_utils/utils/log_events.py` & `siglost_utils-0.2.0/siglost_utils/utils/log_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,34 +19,34 @@
         event_sender.send(severity, event_type, payload)
 
         if print_to_console:
             print(f"Event: {severity} - {event_type} - {payload}")
 
 
     @staticmethod
-    def error_log(object_to_log, node_id):
+    def error_log(object_to_log, node_id=""):
         print("{} Error : {}".format(node_id, object_to_log))
         LogEvents.log_event("error", "deployment.error.node", f"{node_id} Error : {object_to_log}")
 
 
     @staticmethod
-    def warning_log(object_to_log, node_id):
+    def warning_log(object_to_log, node_id=""):
         print("{} Warning : {}".format(node_id, object_to_log))
         LogEvents.log_event("warning", "deployment.warning.node", f"{node_id} Warning : {object_to_log}")
 
 
     @staticmethod
-    def info_log(object_to_log, node_id):
+    def info_log(object_to_log, node_id=""):
         print("{} Info : {}".format(node_id, object_to_log))
         LogEvents.log_event("info", "deployment.info.node", f"{node_id} : {object_to_log}")
 
 
     @staticmethod
-    def debug_log(object_to_log, node_id):
+    def debug_log(object_to_log, node_id=""):
         print("{} : {}".format(node_id, object_to_log))
         LogEvents.log_event("debug", "deployment.debug.node", f"{node_id} : {object_to_log}")
 
 
     @staticmethod
-    def conditional_debug_log(object_to_log, condition, node_id):
+    def conditional_debug_log(object_to_log, condition, node_id=""):
         if condition:
             print("{} : {}".format(node_id, object_to_log))
```

### Comparing `siglost_utils-0.1.5/siglost_utils.egg-info/PKG-INFO` & `siglost_utils-0.2.0/siglost_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.1.5
+Version: 0.2.0
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `siglost_utils-0.1.5/tests/test_display.py` & `siglost_utils-0.2.0/tests/test_display.py`

 * *Files identical despite different names*

