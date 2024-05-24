# Comparing `tmp/neural-commons-0.3.4.tar.gz` & `tmp/neural-commons-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-commons-0.3.4.tar", last modified: Thu May 23 17:18:06 2024, max compression
+gzip compressed data, was "neural-commons-0.3.5.tar", last modified: Fri May 24 00:49:01 2024, max compression
```

## Comparing `neural-commons-0.3.4.tar` & `neural-commons-0.3.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.296209 neural-commons-0.3.4/
--rw-rw-rw-   0        0        0      622 2024-05-23 17:18:06.280586 neural-commons-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-05-23 13:58:37.000000 neural-commons-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.238306 neural-commons-0.3.4/neural_commons/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.249332 neural-commons-0.3.4/neural_commons/cf_nn/
--rw-rw-rw-   0        0        0     3314 2024-05-23 14:04:53.000000 neural-commons-0.3.4/neural_commons/cf_nn/CFConv2d.py
--rw-rw-rw-   0        0        0     1575 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/cf_nn/CFLinear.py
--rw-rw-rw-   0        0        0     1228 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/cf_nn/CFModule.py
--rw-rw-rw-   0        0        0    10584 2024-05-20 01:06:32.000000 neural-commons-0.3.4/neural_commons/cf_nn/CFOptimizer.py
--rw-rw-rw-   0        0        0      363 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/cf_nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.249332 neural-commons-0.3.4/neural_commons/cf_nn/tests/
--rw-rw-rw-   0        0        0        0 2024-05-18 16:33:26.000000 neural-commons-0.3.4/neural_commons/cf_nn/tests/__init__.py
--rw-rw-rw-   0        0        0     7761 2024-05-23 16:35:09.000000 neural-commons-0.3.4/neural_commons/cf_nn/tests/test_cf_optimizer.py
--rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/cf_nn/tests/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.249332 neural-commons-0.3.4/neural_commons/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/helpers/__init__.py
--rw-rw-rw-   0        0        0     5844 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.280586 neural-commons-0.3.4/neural_commons/modules/
--rw-rw-rw-   0        0        0      699 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/AdaptiveSimpleNorm.py
--rw-rw-rw-   0        0        0      288 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/modules/ArgMax.py
--rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.3.4/neural_commons/modules/ConvMixer2d.py
--rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/GTanh.py
--rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/GaELU.py
--rw-rw-rw-   0        0        0      312 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/modules/GaussianNoise.py
--rw-rw-rw-   0        0        0     1266 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/InputEncoder.py
--rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/LogShape.py
--rw-rw-rw-   0        0        0      203 2024-05-02 14:19:58.000000 neural-commons-0.3.4/neural_commons/modules/MAELoss.py
--rw-rw-rw-   0        0        0     2188 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/NeuralLayer.py
--rw-rw-rw-   0        0        0      842 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/NeuralLayer2d.py
--rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/ParametricReLU.py
--rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.3.4/neural_commons/modules/Permute.py
--rw-rw-rw-   0        0        0      286 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/modules/Plus.py
--rw-rw-rw-   0        0        0      472 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/Quadratic.py
--rw-rw-rw-   0        0        0      235 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/RMSELoss.py
--rw-rw-rw-   0        0        0      470 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/RndNonLinearFunction.py
--rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/RndProjection.py
--rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.3.4/neural_commons/modules/SMoE.py
--rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/SMoEMixIn.py
--rw-rw-rw-   0        0        0      232 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/modules/View.py
--rw-rw-rw-   0        0        0      714 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.280586 neural-commons-0.3.4/neural_commons/opt/
--rw-rw-rw-   0        0        0     1909 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/opt/CosineScheduleOptimizer.py
--rw-rw-rw-   0        0        0     1428 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/opt/CosineScheduler.py
--rw-rw-rw-   0        0        0     2066 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/opt/TBCosineScheduleOptimizer.py
--rw-rw-rw-   0        0        0      174 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/opt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.280586 neural-commons-0.3.4/neural_commons/q_nn/
--rw-rw-rw-   0        0        0     2157 2024-05-23 13:56:40.000000 neural-commons-0.3.4/neural_commons/q_nn/ParamModule.py
--rw-rw-rw-   0        0        0     1911 2024-05-23 16:24:52.000000 neural-commons-0.3.4/neural_commons/q_nn/QConv2d.py
--rw-rw-rw-   0        0        0     7468 2024-05-23 13:53:33.000000 neural-commons-0.3.4/neural_commons/q_nn/QGRFOptimizer.py
--rw-rw-rw-   0        0        0     1207 2024-05-22 19:47:30.000000 neural-commons-0.3.4/neural_commons/q_nn/QLinear.py
--rw-rw-rw-   0        0        0      372 2024-05-23 17:17:36.000000 neural-commons-0.3.4/neural_commons/q_nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.280586 neural-commons-0.3.4/neural_commons/q_nn/tests/
--rw-rw-rw-   0        0        0        0 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/q_nn/tests/__init__.py
--rw-rw-rw-   0        0        0     7951 2024-05-23 17:17:44.000000 neural-commons-0.3.4/neural_commons/q_nn/tests/test_qgrf_optimizer.py
--rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/q_nn/tests/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.243299 neural-commons-0.3.4/neural_commons.egg-info/
--rw-rw-rw-   0        0        0      622 2024-05-23 17:18:06.000000 neural-commons-0.3.4/neural_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1853 2024-05-23 17:18:06.000000 neural-commons-0.3.4/neural_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 17:18:06.000000 neural-commons-0.3.4/neural_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-23 17:18:06.000000 neural-commons-0.3.4/neural_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-23 17:18:06.000000 neural-commons-0.3.4/neural_commons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 17:18:06.296209 neural-commons-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      969 2024-05-23 17:17:54.000000 neural-commons-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:01.232774 neural-commons-0.3.5/
+-rw-rw-rw-   0        0        0      622 2024-05-24 00:49:01.232774 neural-commons-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-05-23 13:58:37.000000 neural-commons-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:01.185888 neural-commons-0.3.5/neural_commons/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.5/neural_commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:01.185888 neural-commons-0.3.5/neural_commons/cf_nn/
+-rw-rw-rw-   0        0        0     3314 2024-05-23 14:04:53.000000 neural-commons-0.3.5/neural_commons/cf_nn/CFConv2d.py
+-rw-rw-rw-   0        0        0     1575 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/cf_nn/CFLinear.py
+-rw-rw-rw-   0        0        0     1228 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/cf_nn/CFModule.py
+-rw-rw-rw-   0        0        0    10551 2024-05-24 00:47:04.000000 neural-commons-0.3.5/neural_commons/cf_nn/CFOptimizer.py
+-rw-rw-rw-   0        0        0      363 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/cf_nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:01.201525 neural-commons-0.3.5/neural_commons/cf_nn/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-18 16:33:26.000000 neural-commons-0.3.5/neural_commons/cf_nn/tests/__init__.py
+-rw-rw-rw-   0        0        0     7751 2024-05-24 00:45:30.000000 neural-commons-0.3.5/neural_commons/cf_nn/tests/test_cf_optimizer.py
+-rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/cf_nn/tests/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:01.201525 neural-commons-0.3.5/neural_commons/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.5/neural_commons/helpers/__init__.py
+-rw-rw-rw-   0        0        0     5844 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:01.217152 neural-commons-0.3.5/neural_commons/modules/
+-rw-rw-rw-   0        0        0      699 2024-04-28 15:00:31.000000 neural-commons-0.3.5/neural_commons/modules/AdaptiveSimpleNorm.py
+-rw-rw-rw-   0        0        0      288 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/modules/ArgMax.py
+-rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.3.5/neural_commons/modules/ConvMixer2d.py
+-rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.3.5/neural_commons/modules/GTanh.py
+-rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.3.5/neural_commons/modules/GaELU.py
+-rw-rw-rw-   0        0        0      312 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/modules/GaussianNoise.py
+-rw-rw-rw-   0        0        0     1266 2024-04-28 15:00:31.000000 neural-commons-0.3.5/neural_commons/modules/InputEncoder.py
+-rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.3.5/neural_commons/modules/LogShape.py
+-rw-rw-rw-   0        0        0      203 2024-05-02 14:19:58.000000 neural-commons-0.3.5/neural_commons/modules/MAELoss.py
+-rw-rw-rw-   0        0        0     2188 2024-04-28 15:00:31.000000 neural-commons-0.3.5/neural_commons/modules/NeuralLayer.py
+-rw-rw-rw-   0        0        0      842 2024-04-28 15:00:31.000000 neural-commons-0.3.5/neural_commons/modules/NeuralLayer2d.py
+-rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.3.5/neural_commons/modules/ParametricReLU.py
+-rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.3.5/neural_commons/modules/Permute.py
+-rw-rw-rw-   0        0        0      286 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/modules/Plus.py
+-rw-rw-rw-   0        0        0      472 2024-04-28 15:00:31.000000 neural-commons-0.3.5/neural_commons/modules/Quadratic.py
+-rw-rw-rw-   0        0        0      235 2024-04-28 15:00:31.000000 neural-commons-0.3.5/neural_commons/modules/RMSELoss.py
+-rw-rw-rw-   0        0        0      470 2024-04-28 15:00:31.000000 neural-commons-0.3.5/neural_commons/modules/RndNonLinearFunction.py
+-rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.3.5/neural_commons/modules/RndProjection.py
+-rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.3.5/neural_commons/modules/SMoE.py
+-rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.3.5/neural_commons/modules/SMoEMixIn.py
+-rw-rw-rw-   0        0        0      232 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/modules/View.py
+-rw-rw-rw-   0        0        0      714 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:01.217152 neural-commons-0.3.5/neural_commons/opt/
+-rw-rw-rw-   0        0        0     1909 2024-04-28 15:00:31.000000 neural-commons-0.3.5/neural_commons/opt/CosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0     1428 2024-04-28 15:00:31.000000 neural-commons-0.3.5/neural_commons/opt/CosineScheduler.py
+-rw-rw-rw-   0        0        0     2066 2024-04-28 15:00:31.000000 neural-commons-0.3.5/neural_commons/opt/TBCosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0      174 2024-04-28 15:00:31.000000 neural-commons-0.3.5/neural_commons/opt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:01.232774 neural-commons-0.3.5/neural_commons/q_nn/
+-rw-rw-rw-   0        0        0     2157 2024-05-23 13:56:40.000000 neural-commons-0.3.5/neural_commons/q_nn/ParamModule.py
+-rw-rw-rw-   0        0        0     1911 2024-05-23 16:24:52.000000 neural-commons-0.3.5/neural_commons/q_nn/QConv2d.py
+-rw-rw-rw-   0        0        0     7468 2024-05-23 13:53:33.000000 neural-commons-0.3.5/neural_commons/q_nn/QGRFOptimizer.py
+-rw-rw-rw-   0        0        0     1207 2024-05-22 19:47:30.000000 neural-commons-0.3.5/neural_commons/q_nn/QLinear.py
+-rw-rw-rw-   0        0        0      372 2024-05-23 17:17:36.000000 neural-commons-0.3.5/neural_commons/q_nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:01.232774 neural-commons-0.3.5/neural_commons/q_nn/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/q_nn/tests/__init__.py
+-rw-rw-rw-   0        0        0     7951 2024-05-23 17:17:44.000000 neural-commons-0.3.5/neural_commons/q_nn/tests/test_qgrf_optimizer.py
+-rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.5/neural_commons/q_nn/tests/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:49:01.185888 neural-commons-0.3.5/neural_commons.egg-info/
+-rw-rw-rw-   0        0        0      622 2024-05-24 00:49:01.000000 neural-commons-0.3.5/neural_commons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1853 2024-05-24 00:49:01.000000 neural-commons-0.3.5/neural_commons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 00:49:01.000000 neural-commons-0.3.5/neural_commons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-24 00:49:01.000000 neural-commons-0.3.5/neural_commons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-24 00:49:01.000000 neural-commons-0.3.5/neural_commons.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 00:49:01.232774 neural-commons-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      969 2024-05-24 00:48:54.000000 neural-commons-0.3.5/setup.py
```

### Comparing `neural-commons-0.3.4/PKG-INFO` & `neural-commons-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-commons
-Version: 0.3.4
+Version: 0.3.5
 Summary: A neural network utility library for PyTorch.
 Author: Jose Solorzano
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.23
```

### Comparing `neural-commons-0.3.4/neural_commons/cf_nn/CFConv2d.py` & `neural-commons-0.3.5/neural_commons/cf_nn/CFConv2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/cf_nn/CFLinear.py` & `neural-commons-0.3.5/neural_commons/cf_nn/CFLinear.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/cf_nn/CFModule.py` & `neural-commons-0.3.5/neural_commons/cf_nn/CFModule.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/cf_nn/CFOptimizer.py` & `neural-commons-0.3.5/neural_commons/cf_nn/CFOptimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,36 +202,36 @@
                 self.data_queue.append((inputs, output, residual,))
         return loss
 
     @property
     def queued_batch_size(self) -> int:
         return sum(output.size(0) for _, output, _ in self.data_queue)
 
-    def _step(self, update_rate: float, max_residual_rel_rms: float, **kwargs):
+    def _step(self, update_rate: float, max_change: float, **kwargs):
         if len(self.data_queue) == 0:
             raise InvalidCFStateException("No data has been queued. Call enqueue_data() before calling step().")
         inputs_list = [i for i, _, _ in self.data_queue]
         output_list = [out for _, out, _ in self.data_queue]
         residual_list = [res for _, _, res in self.data_queue]
         self.data_queue = list()
         with torch.no_grad():
             inputs = concatenate_tensors(inputs_list, dim=0)
             del inputs_list
             output = torch.cat(output_list, dim=0)
             del output_list
             residual = torch.cat(residual_list, dim=0)
             del residual_list
             residual *= update_rate
-            max_res_rms = rms(output) * max_residual_rel_rms
+            max_res_rms = rms(output) * max_change
             res_rms = rms(residual)
             if res_rms > max_res_rms:
                 residual *= max_res_rms / res_rms
             self.selected_module.cf_learn(inputs, output, residual, **kwargs)
 
-    def step(self, update_rate: float = 1.0, max_residual_rel_rms = 1.0, **kwargs):
+    def step(self, update_rate: float = 1.0, max_change: float = 1.0, **kwargs):
         if update_rate <= 0 or update_rate > 1.0:
             raise ValueError("update_rate expected to be in ]0, 1].")
         try:
-            self._step(update_rate, max_residual_rel_rms, **kwargs)
+            self._step(update_rate, max_change, **kwargs)
         finally:
             self.data_queue = list()
             self._select_next()
```

### Comparing `neural-commons-0.3.4/neural_commons/cf_nn/tests/test_cf_optimizer.py` & `neural-commons-0.3.5/neural_commons/cf_nn/tests/test_cf_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,12 +176,12 @@
             def _fn() -> torch.Tensor:
                 y = opt_m(x)
                 _loss = loss_fn(y, label)
                 return _loss
 
             optimizer.enqueue_data(_fn)
             if optimizer.queued_batch_size >= 1:
-                optimizer.step(max_residual_rel_rms=10.0)
+                optimizer.step(max_change=10.0)
         pred_y_2 = opt_m(x)
         loss = loss_fn(pred_y_2, label)
         loss_value_2 = torch.mean(loss).item()
         return loss_value_1, loss_value_2,
```

### Comparing `neural-commons-0.3.4/neural_commons/cf_nn/tests/utils.py` & `neural-commons-0.3.5/neural_commons/cf_nn/tests/utils.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/helpers/torch_helper.py` & `neural-commons-0.3.5/neural_commons/helpers/torch_helper.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/modules/AdaptiveSimpleNorm.py` & `neural-commons-0.3.5/neural_commons/modules/AdaptiveSimpleNorm.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/modules/ConvMixer2d.py` & `neural-commons-0.3.5/neural_commons/modules/ConvMixer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/modules/InputEncoder.py` & `neural-commons-0.3.5/neural_commons/modules/InputEncoder.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/modules/NeuralLayer.py` & `neural-commons-0.3.5/neural_commons/modules/NeuralLayer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/modules/NeuralLayer2d.py` & `neural-commons-0.3.5/neural_commons/modules/NeuralLayer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/modules/RndProjection.py` & `neural-commons-0.3.5/neural_commons/modules/RndProjection.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/modules/SMoE.py` & `neural-commons-0.3.5/neural_commons/modules/SMoE.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/modules/SMoEMixIn.py` & `neural-commons-0.3.5/neural_commons/modules/SMoEMixIn.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/modules/__init__.py` & `neural-commons-0.3.5/neural_commons/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/opt/CosineScheduleOptimizer.py` & `neural-commons-0.3.5/neural_commons/opt/CosineScheduleOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/opt/CosineScheduler.py` & `neural-commons-0.3.5/neural_commons/opt/CosineScheduler.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/opt/TBCosineScheduleOptimizer.py` & `neural-commons-0.3.5/neural_commons/opt/TBCosineScheduleOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/q_nn/ParamModule.py` & `neural-commons-0.3.5/neural_commons/q_nn/ParamModule.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/q_nn/QConv2d.py` & `neural-commons-0.3.5/neural_commons/q_nn/QConv2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/q_nn/QGRFOptimizer.py` & `neural-commons-0.3.5/neural_commons/q_nn/QGRFOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/q_nn/QLinear.py` & `neural-commons-0.3.5/neural_commons/q_nn/QLinear.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/q_nn/tests/test_qgrf_optimizer.py` & `neural-commons-0.3.5/neural_commons/q_nn/tests/test_qgrf_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons/q_nn/tests/utils.py` & `neural-commons-0.3.5/neural_commons/q_nn/tests/utils.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/neural_commons.egg-info/PKG-INFO` & `neural-commons-0.3.5/neural_commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-commons
-Version: 0.3.4
+Version: 0.3.5
 Summary: A neural network utility library for PyTorch.
 Author: Jose Solorzano
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.23
```

### Comparing `neural-commons-0.3.4/neural_commons.egg-info/SOURCES.txt` & `neural-commons-0.3.5/neural_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.4/setup.py` & `neural-commons-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 
 from setuptools import setup, find_packages
 
 # Define project metadata
 NAME = 'neural-commons'
-VERSION = '0.3.4'
+VERSION = '0.3.5'
 DESCRIPTION = 'A neural network utility library for PyTorch.'
 AUTHOR = 'Jose Solorzano'
 
 REQUIRES = [
     'numpy>=1.23',
     'tqdm>=4.0.0',
     'torch>=2.1.0',
```

