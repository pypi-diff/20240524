# Comparing `tmp/torch_analyzer-1.0.tar.gz` & `tmp/torch_analyzer-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_analyzer-1.0.tar", last modified: Thu May 23 09:45:51 2024, max compression
+gzip compressed data, was "torch_analyzer-1.1.tar", last modified: Fri May 24 04:58:17 2024, max compression
```

## Comparing `torch_analyzer-1.0.tar` & `torch_analyzer-1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:45:51.192186 torch_analyzer-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 09:45:46.000000 torch_analyzer-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-23 09:45:51.192186 torch_analyzer-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-23 09:45:46.000000 torch_analyzer-1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:45:51.192186 torch_analyzer-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-23 09:45:46.000000 torch_analyzer-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:45:51.192186 torch_analyzer-1.0/torch_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-23 09:45:51.000000 torch_analyzer-1.0/torch_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-23 09:45:51.000000 torch_analyzer-1.0/torch_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:45:51.000000 torch_analyzer-1.0/torch_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 09:45:51.000000 torch_analyzer-1.0/torch_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 09:45:51.000000 torch_analyzer-1.0/torch_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:45:51.192186 torch_analyzer-1.0/torchanalyzer/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/flops.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/flops_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/in_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/time_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/viser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:58:17.719143 torch_analyzer-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 04:58:14.000000 torch_analyzer-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-24 04:58:17.719143 torch_analyzer-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-24 04:58:14.000000 torch_analyzer-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 04:58:17.719143 torch_analyzer-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-24 04:58:14.000000 torch_analyzer-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:58:17.719143 torch_analyzer-1.1/torch_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-24 04:58:17.000000 torch_analyzer-1.1/torch_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-24 04:58:17.000000 torch_analyzer-1.1/torch_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 04:58:17.000000 torch_analyzer-1.1/torch_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 04:58:17.000000 torch_analyzer-1.1/torch_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 04:58:17.000000 torch_analyzer-1.1/torch_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 04:58:17.719143 torch_analyzer-1.1/torchanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-24 04:58:14.000000 torch_analyzer-1.1/torchanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-24 04:58:14.000000 torch_analyzer-1.1/torchanalyzer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-24 04:58:14.000000 torch_analyzer-1.1/torchanalyzer/flops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-05-24 04:58:14.000000 torch_analyzer-1.1/torchanalyzer/flops_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-24 04:58:14.000000 torch_analyzer-1.1/torchanalyzer/in_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-24 04:58:14.000000 torch_analyzer-1.1/torchanalyzer/time_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 04:58:14.000000 torch_analyzer-1.1/torchanalyzer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-05-24 04:58:14.000000 torch_analyzer-1.1/torchanalyzer/viser.py
```

### Comparing `torch_analyzer-1.0/LICENSE` & `torch_analyzer-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.0/PKG-INFO` & `torch_analyzer-1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-analyzer
-Version: 1.0
+Version: 1.1
 Summary: A torch model analyzer
 Home-page: https://github.com/IrisRainbowNeko/torch-analyzer
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -94,7 +94,16 @@
 ```
 
 Show with flow style:
 ```python
 from torchanalyzer import FlowViser
 FlowViser().show(model, info)
 ```
+
+### Backward Analyze
+Analyze run time and memory of each layer in backward:
+```python
+from torchanalyzer import ModelTimeMemAnalyzer
+
+analyzer = ModelTimeMemAnalyzer(model)
+info = analyzer.analyze(inputs, with_backward=True)
+```
```

### Comparing `torch_analyzer-1.0/README.md` & `torch_analyzer-1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -72,8 +72,17 @@
 TableViser().show(model, info)
 ```
 
 Show with flow style:
 ```python
 from torchanalyzer import FlowViser
 FlowViser().show(model, info)
+```
+
+### Backward Analyze
+Analyze run time and memory of each layer in backward:
+```python
+from torchanalyzer import ModelTimeMemAnalyzer
+
+analyzer = ModelTimeMemAnalyzer(model)
+info = analyzer.analyze(inputs, with_backward=True)
 ```
```

### Comparing `torch_analyzer-1.0/setup.py` & `torch_analyzer-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     for x in f.readlines():
         requires.append(f'{x.strip()}')
 
 
 setuptools.setup(
     name="torch-analyzer",
     py_modules=["torch-analyzer"],
-    version="1.0",
+    version="1.1",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A torch model analyzer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IrisRainbowNeko/torch-analyzer",
     packages=setuptools.find_packages(),
```

### Comparing `torch_analyzer-1.0/torch_analyzer.egg-info/PKG-INFO` & `torch_analyzer-1.1/torch_analyzer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-analyzer
-Version: 1.0
+Version: 1.1
 Summary: A torch model analyzer
 Home-page: https://github.com/IrisRainbowNeko/torch-analyzer
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -94,7 +94,16 @@
 ```
 
 Show with flow style:
 ```python
 from torchanalyzer import FlowViser
 FlowViser().show(model, info)
 ```
+
+### Backward Analyze
+Analyze run time and memory of each layer in backward:
+```python
+from torchanalyzer import ModelTimeMemAnalyzer
+
+analyzer = ModelTimeMemAnalyzer(model)
+info = analyzer.analyze(inputs, with_backward=True)
+```
```

### Comparing `torch_analyzer-1.0/torchanalyzer/base.py` & `torch_analyzer-1.1/torchanalyzer/base.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.0/torchanalyzer/flops.py` & `torch_analyzer-1.1/torchanalyzer/flops.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.0/torchanalyzer/flops_kernel.py` & `torch_analyzer-1.1/torchanalyzer/flops_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,17 @@
 def flops_gelu(input_shapes, concrete_inputs):
     # tanh take 7 flops
     return (4+7+3)*np.prod(input_shapes[0])
 
 def flops_silu(input_shapes, concrete_inputs):
     return 5*np.prod(input_shapes[0])
 
+def flops_tanh(input_shapes, concrete_inputs):
+    return 8*np.prod(input_shapes[0])
+
 # -----------------------tensor ops-----------------------
 def flops_sum(input_shapes, concrete_inputs):
     s_in = np.array(input_shapes[0])
     s_in[concrete_inputs[1]] -= 1
     return s_in.prod()
 
 def flops_var(input_shapes, concrete_inputs):
@@ -120,16 +123,18 @@
 op_map = {
     # model ops
     'aten::conv2d': flops_convnd,
     'aten::relu': flops_single_ops,
     'aten::relu_': flops_single_ops,
     'aten::gelu': flops_gelu,
     'aten::gelu_': flops_gelu,
-    'aten::silu': flops_gelu,
-    'aten::silu_': flops_gelu,
+    'aten::silu': flops_silu,
+    'aten::silu_': flops_silu,
+    'aten::tanh': flops_tanh,
+    'aten::tanh_': flops_tanh,
     'aten::max_pool2d': flops_pool,
     'aten::batch_norm': flops_batch_norm,
     'aten::layer_norm': flops_batch_norm,
 
     'aten::scaled_dot_product_attention': flops_attention,
     # mat ops
     'aten::addmm': flops_addmm,
```

### Comparing `torch_analyzer-1.0/torchanalyzer/in_out.py` & `torch_analyzer-1.1/torchanalyzer/in_out.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.0/torchanalyzer/time_mem.py` & `torch_analyzer-1.1/torchanalyzer/time_mem.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,23 +85,23 @@
             with profile(activities=[ProfilerActivity.CPU, ProfilerActivity.CUDA], profile_memory=True) as prof_back:
                 out.backward()
             # for event in prof_back.events():
             #     print(event.name, format_memory(abs(event.cuda_memory_usage)), format_time(event.cuda_time))
             self.events_back = self.summary_events(prof_back.events())
 
             events_back_all = self.events_back['']
-            self.back_cpu_time_all = events_back_all[0]
-            self.back_cuda_time_all = events_back_all[1]
-            self.back_cpu_mem_all = events_back_all[2]
-            self.back_cuda_mem_all = events_back_all[3]
+            self.back_cpu_time_all = max(1, events_back_all[0])
+            self.back_cuda_time_all = max(1, events_back_all[1])
+            self.back_cpu_mem_all = max(1, events_back_all[2])
+            self.back_cuda_mem_all = max(1, events_back_all[3])
 
         self.filtered_events = {event.key[len(prefix):]: event for event in prof.key_averages() if
                                 event.key.startswith(prefix)}
-        self.cpu_time_all = self.filtered_events[''].cpu_time
-        self.cuda_time_all = self.filtered_events[''].cuda_time
+        self.cpu_time_all = max(1, self.filtered_events[''].cpu_time)
+        self.cuda_time_all = max(1, self.filtered_events[''].cuda_time)
         self.cpu_mem_all = max(1, self.filtered_events[''].cpu_memory_usage)
         self.cuda_mem_all = max(1, self.filtered_events[''].cuda_memory_usage)
 
         flow = self.add_info_to_flow(module_flow.module_record)
         return flow
 
     def summary_events(self, events: Iterable, start_key='$o', end_key='$i', prefix='layer:',
```

### Comparing `torch_analyzer-1.0/torchanalyzer/utils.py` & `torch_analyzer-1.1/torchanalyzer/utils.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.0/torchanalyzer/viser.py` & `torch_analyzer-1.1/torchanalyzer/viser.py`

 * *Files identical despite different names*

