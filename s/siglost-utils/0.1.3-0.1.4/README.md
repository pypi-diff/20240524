# Comparing `tmp/siglost_utils-0.1.3.tar.gz` & `tmp/siglost_utils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siglost_utils-0.1.3.tar", last modified: Fri May 24 02:11:50 2024, max compression
+gzip compressed data, was "siglost_utils-0.1.4.tar", last modified: Fri May 24 02:52:03 2024, max compression
```

## Comparing `siglost_utils-0.1.3.tar` & `siglost_utils-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils/api/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils/display/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/display/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils/inference/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/inference/inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/siglost_utils/utils/log_events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/siglost_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 02:11:50.000000 siglost_utils-0.1.3/siglost_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-24 02:11:50.000000 siglost_utils-0.1.3/siglost_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:11:50.000000 siglost_utils-0.1.3/siglost_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 02:11:50.000000 siglost_utils-0.1.3/siglost_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:50.591858 siglost_utils-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 02:11:39.000000 siglost_utils-0.1.3/tests/test_display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-24 02:52:03.277471 siglost_utils-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils/display/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/display/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/inference/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/siglost_utils/utils/log_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/siglost_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-24 02:52:03.000000 siglost_utils-0.1.4/siglost_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-24 02:52:03.000000 siglost_utils-0.1.4/siglost_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 02:52:03.000000 siglost_utils-0.1.4/siglost_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 02:52:03.000000 siglost_utils-0.1.4/siglost_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 02:52:03.273471 siglost_utils-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-24 02:51:52.000000 siglost_utils-0.1.4/tests/test_display.py
```

### Comparing `siglost_utils-0.1.3/LICENSE` & `siglost_utils-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.3/PKG-INFO` & `siglost_utils-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `siglost_utils-0.1.3/setup.cfg` & `siglost_utils-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.3/siglost_utils/display/display.py` & `siglost_utils-0.1.4/siglost_utils/display/display.py`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.3/siglost_utils/inference/inference.py` & `siglost_utils-0.1.4/siglost_utils/inference/inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 
     self.unique_key = f"{deployment_id}_{node_id}.{self.model_name}"
     self.url = url
     self.node_id = node_id
     self.auto_manage = auto_manage
     self.input_max_dims = input_max_dims
     self.output_max_dims = output_max_dims
+    self.enable_debug_logs = enable_debug_logs
     self.compare_outputs = compare_outputs
     self.unload_unused_model = unload_unused_model
 
     # Choose the Triton client based on the communication scheme
     # Ref : https://github.com/triton-inference-server/client/blob/main/src/python/library/tritonclient/http/_client.py
     import tritonclient.http as client  # noqa
     self.triton_client = client.InferenceServerClient(url=url, verbose=False, ssl=False, concurrency=5)
@@ -151,15 +152,15 @@
 
   def load_model(self):
     is_loaded, is_loading = self.get_model_state()
     if not (is_loaded or is_loading):
       with contextlib.suppress(Exception):
         self.triton_client.load_model(self.model_name)
     while not self.triton_client.is_model_ready(self.model_name):
-      conditional_debug_log(f"Waiting for Triton model {self.model_name} to be ready.", enable_debug_logs, self.node_id)
+      conditional_debug_log(f"Waiting for Triton model {self.model_name} to be ready.", self.enable_debug_logs, self.node_id)
       time.sleep(10)
 
     is_loaded, is_loading = self.get_model_state()
     if is_loaded:
       config = self.triton_client.get_model_config(self.model_name)
 
       # Sort output names alphabetically, i.e. 'output0', 'output1', etc.
@@ -205,15 +206,15 @@
         deployments_using_model = set()
         triton_shms = self.triton_client.get_system_shared_memory_status()
         for triton_shm in triton_shms:
           if self.model_name in triton_shm['name']:
             deployments_using_model.add(triton_shm['name'].split('.')[1].split('_')[0])
 
         if len(deployments_using_model) == 0:
-          conditional_debug_log(f"Unloading Triton model {self.model_name} as it is not being used by any deployment.", enable_debug_logs, self.node_id)
+          conditional_debug_log(f"Unloading Triton model {self.model_name} as it is not being used by any deployment.", self.enable_debug_logs, self.node_id)
           self.triton_client.unload_model(self.model_name)
           return True
 
     return self
 
   def setup_shared_memory(self):
     """
@@ -248,15 +249,15 @@
       with contextlib.suppress(Exception):
         self.triton_client.unregister_system_shared_memory(f'output_data.{self.unique_key}')
       with contextlib.suppress(Exception):
         shm.destroy_shared_memory_region(f"input_data.{self.unique_key}")
       with contextlib.suppress(Exception):
         shm.destroy_shared_memory_region(f"output_data.{self.unique_key}")
       self.is_shm_setup = False
-      conditional_debug_log(f"Unregistered shared memory regions with Triton server.", enable_debug_logs, self.node_id)
+      conditional_debug_log(f"Unregistered shared memory regions with Triton server.", self.enable_debug_logs, self.node_id)
     return self
 
   def __del__(self):
     # To make sure no shared memory regions are registered with the
     # server.
     if self.auto_manage or self.unload_unused_model:
       self.unregister_shared_memory()
@@ -304,15 +305,15 @@
     outputs = self.triton_client.infer(model_name=self.model_name, inputs=infer_inputs, outputs=infer_outputs)
 
     # Read results from the outputs and create a dictionary
     output_data = {}
     for output_name in self.output_names:
       output_data[output_name] = outputs.as_numpy(output_name).astype(input_format)
 
-    # conditional_debug_log(f"Time taken for predict_noshm() inference: {time.time() - tick:.3f}s", enable_debug_logs, self.node_id)
+    # conditional_debug_log(f"Time taken for predict_noshm() inference: {time.time() - tick:.3f}s", self.enable_debug_logs, self.node_id)
     return output_data
 
 
   def predict_shm(self, *inputs: np.ndarray) -> dict:
     """
     Call the model with the given inputs.
     Args:
@@ -356,26 +357,26 @@
           tritonclient.utils.triton_to_np_dtype(output["datatype"]),
           output["shape"],
           offset=offset,
         )
         output_data[output_name] = output_data_np
         offset += output_data_np.size * output_data_np.itemsize
       else:
-        conditional_debug_log(f"{output_name} is missing in the response.", enable_debug_logs, self.node_id)
+        conditional_debug_log(f"{output_name} is missing in the response.", self.enable_debug_logs, self.node_id)
 
-    # conditional_debug_log(f"Time taken for predict_shm() inference: {time.time() - tick:.3f}s", enable_debug_logs, self.node_id)
+    # conditional_debug_log(f"Time taken for predict_shm() inference: {time.time() - tick:.3f}s", self.enable_debug_logs, self.node_id)
     return output_data
 
   def compare_shm_noshm_outputs(self, output_shm, output_noshm):
-    conditional_debug_log(f"output_shm: {output_shm}", enable_debug_logs, self.node_id)
-    conditional_debug_log(f"output_noshm: {output_noshm}", enable_debug_logs, self.node_id)
+    conditional_debug_log(f"output_shm: {output_shm}", self.enable_debug_logs, self.node_id)
+    conditional_debug_log(f"output_noshm: {output_noshm}", self.enable_debug_logs, self.node_id)
 
-    conditional_debug_log(f"output_shm shape: {output_shm.shape}", enable_debug_logs, self.node_id)
-    conditional_debug_log(f"output_shm numpy type: {output_shm.dtype}", enable_debug_logs, self.node_id)
+    conditional_debug_log(f"output_shm shape: {output_shm.shape}", self.enable_debug_logs, self.node_id)
+    conditional_debug_log(f"output_shm numpy type: {output_shm.dtype}", self.enable_debug_logs, self.node_id)
 
-    conditional_debug_log(f"output_noshm shape: {output_noshm.shape}", enable_debug_logs, self.node_id)
-    conditional_debug_log(f"output_noshm numpy type: {output_noshm.dtype}", enable_debug_logs, self.node_id)
+    conditional_debug_log(f"output_noshm shape: {output_noshm.shape}", self.enable_debug_logs, self.node_id)
+    conditional_debug_log(f"output_noshm numpy type: {output_noshm.dtype}", self.enable_debug_logs, self.node_id)
 
     if output_shm.shape != output_noshm.shape:
       return False
 
     return np.array_equal(output_shm, output_noshm)
```

### Comparing `siglost_utils-0.1.3/siglost_utils/utils/log_events.py` & `siglost_utils-0.1.4/siglost_utils/utils/log_events.py`

 * *Files identical despite different names*

### Comparing `siglost_utils-0.1.3/siglost_utils.egg-info/PKG-INFO` & `siglost_utils-0.1.4/siglost_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siglost_utils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python utility package
 Home-page: https://github.com/siglost/python_utils
 Author: SIGLOST
 Author-email: SIGLOST@email.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `siglost_utils-0.1.3/tests/test_display.py` & `siglost_utils-0.1.4/tests/test_display.py`

 * *Files identical despite different names*

