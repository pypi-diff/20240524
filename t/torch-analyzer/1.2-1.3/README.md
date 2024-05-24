# Comparing `tmp/torch_analyzer-1.2.tar.gz` & `tmp/torch_analyzer-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_analyzer-1.2.tar", last modified: Fri May 24 06:48:41 2024, max compression
+gzip compressed data, was "torch_analyzer-1.3.tar", last modified: Fri May 24 08:03:51 2024, max compression
```

## Comparing `torch_analyzer-1.2.tar` & `torch_analyzer-1.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:48:41.350983 torch_analyzer-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 06:48:37.000000 torch_analyzer-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-24 06:48:41.350983 torch_analyzer-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-24 06:48:37.000000 torch_analyzer-1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 06:48:41.350983 torch_analyzer-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-24 06:48:37.000000 torch_analyzer-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:48:41.346982 torch_analyzer-1.2/torch_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-24 06:48:41.000000 torch_analyzer-1.2/torch_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-24 06:48:41.000000 torch_analyzer-1.2/torch_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 06:48:41.000000 torch_analyzer-1.2/torch_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 06:48:41.000000 torch_analyzer-1.2/torch_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 06:48:41.000000 torch_analyzer-1.2/torch_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 06:48:41.346982 torch_analyzer-1.2/torchanalyzer/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-24 06:48:37.000000 torch_analyzer-1.2/torchanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-24 06:48:37.000000 torch_analyzer-1.2/torchanalyzer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-24 06:48:37.000000 torch_analyzer-1.2/torchanalyzer/flops.py
--rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-05-24 06:48:37.000000 torch_analyzer-1.2/torchanalyzer/flops_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-24 06:48:37.000000 torch_analyzer-1.2/torchanalyzer/in_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-24 06:48:37.000000 torch_analyzer-1.2/torchanalyzer/time_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 06:48:37.000000 torch_analyzer-1.2/torchanalyzer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-24 06:48:37.000000 torch_analyzer-1.2/torchanalyzer/viser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:03:51.852543 torch_analyzer-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 08:03:46.000000 torch_analyzer-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-24 08:03:51.852543 torch_analyzer-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-24 08:03:46.000000 torch_analyzer-1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 08:03:51.852543 torch_analyzer-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-24 08:03:46.000000 torch_analyzer-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:03:51.852543 torch_analyzer-1.3/torch_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-24 08:03:51.000000 torch_analyzer-1.3/torch_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-24 08:03:51.000000 torch_analyzer-1.3/torch_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:03:51.000000 torch_analyzer-1.3/torch_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 08:03:51.000000 torch_analyzer-1.3/torch_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 08:03:51.000000 torch_analyzer-1.3/torch_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:03:51.852543 torch_analyzer-1.3/torchanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/flops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/flops_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/in_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/memops_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/time_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/viser.py
```

### Comparing `torch_analyzer-1.2/LICENSE` & `torch_analyzer-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.2/PKG-INFO` & `torch_analyzer-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-analyzer
-Version: 1.2
+Version: 1.3
 Summary: A torch model analyzer
 Home-page: https://github.com/IrisRainbowNeko/torch-analyzer
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_analyzer-1.2/README.md` & `torch_analyzer-1.3/README.md`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.2/setup.py` & `torch_analyzer-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     for x in f.readlines():
         requires.append(f'{x.strip()}')
 
 
 setuptools.setup(
     name="torch-analyzer",
     py_modules=["torch-analyzer"],
-    version="1.2",
+    version="1.3",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A torch model analyzer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IrisRainbowNeko/torch-analyzer",
     packages=setuptools.find_packages(),
```

### Comparing `torch_analyzer-1.2/torch_analyzer.egg-info/PKG-INFO` & `torch_analyzer-1.3/torch_analyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-analyzer
-Version: 1.2
+Version: 1.3
 Summary: A torch model analyzer
 Home-page: https://github.com/IrisRainbowNeko/torch-analyzer
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_analyzer-1.2/torchanalyzer/base.py` & `torch_analyzer-1.3/torchanalyzer/base.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.2/torchanalyzer/flops.py` & `torch_analyzer-1.3/torchanalyzer/flops.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List, Tuple
 
 from torch import nn
 from torch.profiler import profile, record_function
 
 from .base import ModelAnalyzer, RecordFlowContext
-from .flops_kernel import op_map
+from .flops_kernel import flops_op_map
+from .memops_kernel import memops_op_map
 from .utils import Color, format_flops, format_percent
 
 
 class ProfContext:
     def __init__(self, model, prefix='layer:'):
         self.model = model
         self.prefix = prefix
@@ -38,21 +39,24 @@
 class ModelFlopsAnalyzer(ModelAnalyzer):
 
     def analyze(self, inputs) -> List[Tuple[str, str, nn.Module, List]]:
         with (RecordFlowContext(self.model) as module_flow, ProfContext(self.model, prefix=''),
               profile(record_shapes=True, use_cuda=True) as prof):
             out = self.model(inputs)
 
-        self.flops_dict = self.summary_events(prof.events())
+        self.flops_dict = self.summary_events(prof.events(), flops_op_map)
         self.flops_all = self.flops_dict['']
 
+        self.memops_dict = self.summary_events(prof.events(), memops_op_map)
+        self.memops_all = self.memops_dict['']
+
         flow = self.add_info_to_flow(module_flow.module_record)
         return flow
 
-    def summary_events(self, events):
+    def summary_events(self, events, op_map):
         flops_dict = {}
         blocks = []
         for event in events:
             if event.name.endswith('$i'):
                 blocks.append([event.name[:-2], 0])
             elif event.name.endswith('$o'):
                 block = blocks.pop()
@@ -75,14 +79,16 @@
         return new_flow
 
     def get_flops(self, name, module):
         '''
         :return: [(name:str, info, color:str)]
         '''
         flops = self.flops_dict[name]
+        memops = self.memops_dict[name]
 
         info_list = [
             # ('Layer', f'{format_time(event.cpu_time)}, {format_percent(event.cpu_time / self.cpu_time_all)}', None, Color.CYAN),
             ('FLOPs', f'{format_flops(flops)}, {format_percent(flops / self.flops_all)}', Color.CYAN),
+            ('MemOPs', f'{format_flops(memops)}, {format_percent(memops / self.memops_all)}', Color.MAGENTA),
         ]
 
         return {'_one_': info_list}
```

### Comparing `torch_analyzer-1.2/torchanalyzer/flops_kernel.py` & `torch_analyzer-1.3/torchanalyzer/flops_kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import torch
 from torch.nn import functional as F
 from torch.profiler import profile
 
 
 def tensor_context(func):
     def wrapper(*args, **kwargs):
-        args = [(np.array(x) if isinstance(x, list) else x) for x in args]
-        kwargs = {k: (np.array(v) if isinstance(v, list) else v) for k, v in kwargs}
+        args = [(np.array(x, dtype=np.int64) if isinstance(x, list) else x) for x in args]
+        kwargs = {k: (np.array(v, dtype=np.int64) if isinstance(v, list) else v) for k, v in kwargs}
         return func(*args, **kwargs)
 
     return wrapper
 
 
 # -----------------------model ops-----------------------
 def flops_convnd(input_shapes, concrete_inputs):
@@ -116,15 +116,15 @@
 
 def flops_std(input_shapes, concrete_inputs):
     return 5*np.prod(input_shapes[0])
 
 # -----------------------memory ops-----------------------
 
 
-op_map = {
+flops_op_map = {
     # model ops
     'aten::conv2d': flops_convnd,
     'aten::relu': flops_single_ops,
     'aten::relu_': flops_single_ops,
     'aten::gelu': flops_gelu,
     'aten::gelu_': flops_gelu,
     'aten::silu': flops_silu,
@@ -251,23 +251,23 @@
             x = self.fc(x)
             return x
 
     import timm
 
     device = 'cpu'
     #model = SimpleCNN().to(device)
-    model = MNISTClassifier().to(device)
+    #model = MNISTClassifier().to(device)
     #model = models.resnet18().cuda()
-    #model = timm.create_model('vit_base_patch16_224').to(device)
+    model = timm.create_model('vit_base_patch16_224').to(device)
     inputs = torch.randn(1, 3, 224, 224).to(device)
 
     with profile(record_shapes=True, use_cuda=True) as prof:
         model(inputs)
 
     # 遍历每个事件
     for event in prof.events():
         if event.name.startswith('cuda'):
             continue
         print(
             f"{event.name} - CUDA time: {event.cuda_time}, Input shapes: {event.input_shapes}, input:{event.concrete_inputs}")
-        if event.name in op_map:
-            print(f"{event.name} - FLOPs: {op_map[event.name](event.input_shapes, event.concrete_inputs)}")
+        if event.name in flops_op_map:
+            print(f"{event.name} - FLOPs: {flops_op_map[event.name](event.input_shapes, event.concrete_inputs)}")
```

### Comparing `torch_analyzer-1.2/torchanalyzer/in_out.py` & `torch_analyzer-1.3/torchanalyzer/in_out.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.2/torchanalyzer/time_mem.py` & `torch_analyzer-1.3/torchanalyzer/time_mem.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.2/torchanalyzer/utils.py` & `torch_analyzer-1.3/torchanalyzer/utils.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.2/torchanalyzer/viser.py` & `torch_analyzer-1.3/torchanalyzer/viser.py`

 * *Files identical despite different names*

