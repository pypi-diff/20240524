# Comparing `tmp/torch_analyzer-0.2.tar.gz` & `tmp/torch_analyzer-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_analyzer-0.2.tar", last modified: Fri Apr 26 04:36:58 2024, max compression
+gzip compressed data, was "torch_analyzer-1.0.tar", last modified: Thu May 23 09:45:51 2024, max compression
```

## Comparing `torch_analyzer-0.2.tar` & `torch_analyzer-1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:36:58.381704 torch_analyzer-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 04:36:54.000000 torch_analyzer-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-26 04:36:58.381704 torch_analyzer-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-26 04:36:54.000000 torch_analyzer-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 04:36:58.381704 torch_analyzer-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-26 04:36:54.000000 torch_analyzer-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:36:58.381704 torch_analyzer-0.2/torch_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-26 04:36:58.000000 torch_analyzer-0.2/torch_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-26 04:36:58.000000 torch_analyzer-0.2/torch_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 04:36:58.000000 torch_analyzer-0.2/torch_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 04:36:58.000000 torch_analyzer-0.2/torch_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-26 04:36:58.000000 torch_analyzer-0.2/torch_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 04:36:58.381704 torch_analyzer-0.2/torchanalyzer/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-26 04:36:54.000000 torch_analyzer-0.2/torchanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-26 04:36:54.000000 torch_analyzer-0.2/torchanalyzer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-26 04:36:54.000000 torch_analyzer-0.2/torchanalyzer/flops.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-04-26 04:36:54.000000 torch_analyzer-0.2/torchanalyzer/flops_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-26 04:36:54.000000 torch_analyzer-0.2/torchanalyzer/in_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-26 04:36:54.000000 torch_analyzer-0.2/torchanalyzer/time_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-26 04:36:54.000000 torch_analyzer-0.2/torchanalyzer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-26 04:36:54.000000 torch_analyzer-0.2/torchanalyzer/viser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:45:51.192186 torch_analyzer-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 09:45:46.000000 torch_analyzer-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-23 09:45:51.192186 torch_analyzer-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-23 09:45:46.000000 torch_analyzer-1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:45:51.192186 torch_analyzer-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-23 09:45:46.000000 torch_analyzer-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:45:51.192186 torch_analyzer-1.0/torch_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-23 09:45:51.000000 torch_analyzer-1.0/torch_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-23 09:45:51.000000 torch_analyzer-1.0/torch_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:45:51.000000 torch_analyzer-1.0/torch_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 09:45:51.000000 torch_analyzer-1.0/torch_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 09:45:51.000000 torch_analyzer-1.0/torch_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:45:51.192186 torch_analyzer-1.0/torchanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/flops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/flops_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/in_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/time_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-05-23 09:45:46.000000 torch_analyzer-1.0/torchanalyzer/viser.py
```

### Comparing `torch_analyzer-0.2/LICENSE` & `torch_analyzer-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_analyzer-0.2/PKG-INFO` & `torch_analyzer-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-analyzer
-Version: 0.2
+Version: 1.0
 Summary: A torch model analyzer
 Home-page: https://github.com/IrisRainbowNeko/torch-analyzer
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_analyzer-0.2/README.md` & `torch_analyzer-1.0/README.md`

 * *Files identical despite different names*

### Comparing `torch_analyzer-0.2/setup.py` & `torch_analyzer-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     for x in f.readlines():
         requires.append(f'{x.strip()}')
 
 
 setuptools.setup(
     name="torch-analyzer",
     py_modules=["torch-analyzer"],
-    version="0.2",
+    version="1.0",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A torch model analyzer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IrisRainbowNeko/torch-analyzer",
     packages=setuptools.find_packages(),
```

### Comparing `torch_analyzer-0.2/torch_analyzer.egg-info/PKG-INFO` & `torch_analyzer-1.0/torch_analyzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-analyzer
-Version: 0.2
+Version: 1.0
 Summary: A torch model analyzer
 Home-page: https://github.com/IrisRainbowNeko/torch-analyzer
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_analyzer-0.2/torchanalyzer/base.py` & `torch_analyzer-1.0/torchanalyzer/base.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-0.2/torchanalyzer/flops.py` & `torch_analyzer-1.0/torchanalyzer/flops.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,21 +38,21 @@
 class ModelFlopsAnalyzer(ModelAnalyzer):
 
     def analyze(self, inputs) -> List[Tuple[str, str, nn.Module, List]]:
         with (RecordFlowContext(self.model) as module_flow, ProfContext(self.model, prefix=''),
               profile(record_shapes=True, use_cuda=True) as prof):
             out = self.model(inputs)
 
-        self.flops_dict = self.summary_event(prof.events())
+        self.flops_dict = self.summary_events(prof.events())
         self.flops_all = self.flops_dict['']
 
         flow = self.add_info_to_flow(module_flow.module_record)
         return flow
 
-    def summary_event(self, events):
+    def summary_events(self, events):
         flops_dict = {}
         blocks = []
         for event in events:
             if event.name.endswith('$i'):
                 blocks.append([event.name[:-2], 0])
             elif event.name.endswith('$o'):
                 block = blocks.pop()
```

### Comparing `torch_analyzer-0.2/torchanalyzer/flops_kernel.py` & `torch_analyzer-1.0/torchanalyzer/flops_kernel.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-0.2/torchanalyzer/in_out.py` & `torch_analyzer-1.0/torchanalyzer/in_out.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-0.2/torchanalyzer/utils.py` & `torch_analyzer-1.0/torchanalyzer/utils.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-0.2/torchanalyzer/viser.py` & `torch_analyzer-1.0/torchanalyzer/viser.py`

 * *Files identical despite different names*

