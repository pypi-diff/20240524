# Comparing `tmp/neural-commons-0.3.3.tar.gz` & `tmp/neural-commons-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-commons-0.3.3.tar", last modified: Thu May 23 17:04:45 2024, max compression
+gzip compressed data, was "neural-commons-0.3.4.tar", last modified: Thu May 23 17:18:06 2024, max compression
```

## Comparing `neural-commons-0.3.3.tar` & `neural-commons-0.3.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 17:04:45.993059 neural-commons-0.3.3/
--rw-rw-rw-   0        0        0      622 2024-05-23 17:04:45.993059 neural-commons-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      155 2024-05-23 13:58:37.000000 neural-commons-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 17:04:45.946175 neural-commons-0.3.3/neural_commons/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.3/neural_commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:04:45.946175 neural-commons-0.3.3/neural_commons/cf_nn/
--rw-rw-rw-   0        0        0     3314 2024-05-23 14:04:53.000000 neural-commons-0.3.3/neural_commons/cf_nn/CFConv2d.py
--rw-rw-rw-   0        0        0     1575 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/cf_nn/CFLinear.py
--rw-rw-rw-   0        0        0     1228 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/cf_nn/CFModule.py
--rw-rw-rw-   0        0        0    10584 2024-05-20 01:06:32.000000 neural-commons-0.3.3/neural_commons/cf_nn/CFOptimizer.py
--rw-rw-rw-   0        0        0      363 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/cf_nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:04:45.961809 neural-commons-0.3.3/neural_commons/cf_nn/tests/
--rw-rw-rw-   0        0        0        0 2024-05-18 16:33:26.000000 neural-commons-0.3.3/neural_commons/cf_nn/tests/__init__.py
--rw-rw-rw-   0        0        0     7761 2024-05-23 16:35:09.000000 neural-commons-0.3.3/neural_commons/cf_nn/tests/test_cf_optimizer.py
--rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/cf_nn/tests/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:04:45.961809 neural-commons-0.3.3/neural_commons/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.3/neural_commons/helpers/__init__.py
--rw-rw-rw-   0        0        0     5844 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/helpers/torch_helper.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:04:45.977441 neural-commons-0.3.3/neural_commons/modules/
--rw-rw-rw-   0        0        0      699 2024-04-28 15:00:31.000000 neural-commons-0.3.3/neural_commons/modules/AdaptiveSimpleNorm.py
--rw-rw-rw-   0        0        0      288 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/modules/ArgMax.py
--rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.3.3/neural_commons/modules/ConvMixer2d.py
--rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.3.3/neural_commons/modules/GTanh.py
--rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.3.3/neural_commons/modules/GaELU.py
--rw-rw-rw-   0        0        0      312 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/modules/GaussianNoise.py
--rw-rw-rw-   0        0        0     1266 2024-04-28 15:00:31.000000 neural-commons-0.3.3/neural_commons/modules/InputEncoder.py
--rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.3.3/neural_commons/modules/LogShape.py
--rw-rw-rw-   0        0        0      203 2024-05-02 14:19:58.000000 neural-commons-0.3.3/neural_commons/modules/MAELoss.py
--rw-rw-rw-   0        0        0     2188 2024-04-28 15:00:31.000000 neural-commons-0.3.3/neural_commons/modules/NeuralLayer.py
--rw-rw-rw-   0        0        0      842 2024-04-28 15:00:31.000000 neural-commons-0.3.3/neural_commons/modules/NeuralLayer2d.py
--rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.3.3/neural_commons/modules/ParametricReLU.py
--rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.3.3/neural_commons/modules/Permute.py
--rw-rw-rw-   0        0        0      286 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/modules/Plus.py
--rw-rw-rw-   0        0        0      472 2024-04-28 15:00:31.000000 neural-commons-0.3.3/neural_commons/modules/Quadratic.py
--rw-rw-rw-   0        0        0      235 2024-04-28 15:00:31.000000 neural-commons-0.3.3/neural_commons/modules/RMSELoss.py
--rw-rw-rw-   0        0        0      470 2024-04-28 15:00:31.000000 neural-commons-0.3.3/neural_commons/modules/RndNonLinearFunction.py
--rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.3.3/neural_commons/modules/RndProjection.py
--rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.3.3/neural_commons/modules/SMoE.py
--rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.3.3/neural_commons/modules/SMoEMixIn.py
--rw-rw-rw-   0        0        0      232 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/modules/View.py
--rw-rw-rw-   0        0        0      714 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:04:45.977441 neural-commons-0.3.3/neural_commons/opt/
--rw-rw-rw-   0        0        0     1909 2024-04-28 15:00:31.000000 neural-commons-0.3.3/neural_commons/opt/CosineScheduleOptimizer.py
--rw-rw-rw-   0        0        0     1428 2024-04-28 15:00:31.000000 neural-commons-0.3.3/neural_commons/opt/CosineScheduler.py
--rw-rw-rw-   0        0        0     2066 2024-04-28 15:00:31.000000 neural-commons-0.3.3/neural_commons/opt/TBCosineScheduleOptimizer.py
--rw-rw-rw-   0        0        0      174 2024-04-28 15:00:31.000000 neural-commons-0.3.3/neural_commons/opt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:04:45.993059 neural-commons-0.3.3/neural_commons/q_nn/
--rw-rw-rw-   0        0        0     2157 2024-05-23 13:56:40.000000 neural-commons-0.3.3/neural_commons/q_nn/ParamModule.py
--rw-rw-rw-   0        0        0     1911 2024-05-23 16:24:52.000000 neural-commons-0.3.3/neural_commons/q_nn/QConv2d.py
--rw-rw-rw-   0        0        0     7468 2024-05-23 13:53:33.000000 neural-commons-0.3.3/neural_commons/q_nn/QGRFOptimizer.py
--rw-rw-rw-   0        0        0     1207 2024-05-22 19:47:30.000000 neural-commons-0.3.3/neural_commons/q_nn/QLinear.py
--rw-rw-rw-   0        0        0      342 2024-05-22 19:46:27.000000 neural-commons-0.3.3/neural_commons/q_nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:04:45.993059 neural-commons-0.3.3/neural_commons/q_nn/tests/
--rw-rw-rw-   0        0        0        0 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/q_nn/tests/__init__.py
--rw-rw-rw-   0        0        0     7991 2024-05-23 16:35:34.000000 neural-commons-0.3.3/neural_commons/q_nn/tests/test_qgrf_optimizer.py
--rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.3/neural_commons/q_nn/tests/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:04:45.946175 neural-commons-0.3.3/neural_commons.egg-info/
--rw-rw-rw-   0        0        0      622 2024-05-23 17:04:45.000000 neural-commons-0.3.3/neural_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1853 2024-05-23 17:04:45.000000 neural-commons-0.3.3/neural_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 17:04:45.000000 neural-commons-0.3.3/neural_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-23 17:04:45.000000 neural-commons-0.3.3/neural_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-23 17:04:45.000000 neural-commons-0.3.3/neural_commons.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 17:04:45.993059 neural-commons-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      969 2024-05-23 17:04:34.000000 neural-commons-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.296209 neural-commons-0.3.4/
+-rw-rw-rw-   0        0        0      622 2024-05-23 17:18:06.280586 neural-commons-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2024-05-23 13:58:37.000000 neural-commons-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.238306 neural-commons-0.3.4/neural_commons/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.249332 neural-commons-0.3.4/neural_commons/cf_nn/
+-rw-rw-rw-   0        0        0     3314 2024-05-23 14:04:53.000000 neural-commons-0.3.4/neural_commons/cf_nn/CFConv2d.py
+-rw-rw-rw-   0        0        0     1575 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/cf_nn/CFLinear.py
+-rw-rw-rw-   0        0        0     1228 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/cf_nn/CFModule.py
+-rw-rw-rw-   0        0        0    10584 2024-05-20 01:06:32.000000 neural-commons-0.3.4/neural_commons/cf_nn/CFOptimizer.py
+-rw-rw-rw-   0        0        0      363 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/cf_nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.249332 neural-commons-0.3.4/neural_commons/cf_nn/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-18 16:33:26.000000 neural-commons-0.3.4/neural_commons/cf_nn/tests/__init__.py
+-rw-rw-rw-   0        0        0     7761 2024-05-23 16:35:09.000000 neural-commons-0.3.4/neural_commons/cf_nn/tests/test_cf_optimizer.py
+-rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/cf_nn/tests/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.249332 neural-commons-0.3.4/neural_commons/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/helpers/__init__.py
+-rw-rw-rw-   0        0        0     5844 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/helpers/torch_helper.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.280586 neural-commons-0.3.4/neural_commons/modules/
+-rw-rw-rw-   0        0        0      699 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/AdaptiveSimpleNorm.py
+-rw-rw-rw-   0        0        0      288 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/modules/ArgMax.py
+-rw-rw-rw-   0        0        0     1791 2024-04-10 19:02:18.000000 neural-commons-0.3.4/neural_commons/modules/ConvMixer2d.py
+-rw-rw-rw-   0        0        0      248 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/GTanh.py
+-rw-rw-rw-   0        0        0      283 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/GaELU.py
+-rw-rw-rw-   0        0        0      312 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/modules/GaussianNoise.py
+-rw-rw-rw-   0        0        0     1266 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/InputEncoder.py
+-rw-rw-rw-   0        0        0      463 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/LogShape.py
+-rw-rw-rw-   0        0        0      203 2024-05-02 14:19:58.000000 neural-commons-0.3.4/neural_commons/modules/MAELoss.py
+-rw-rw-rw-   0        0        0     2188 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/NeuralLayer.py
+-rw-rw-rw-   0        0        0      842 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/NeuralLayer2d.py
+-rw-rw-rw-   0        0        0      477 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/ParametricReLU.py
+-rw-rw-rw-   0        0        0      225 2024-04-10 19:01:12.000000 neural-commons-0.3.4/neural_commons/modules/Permute.py
+-rw-rw-rw-   0        0        0      286 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/modules/Plus.py
+-rw-rw-rw-   0        0        0      472 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/Quadratic.py
+-rw-rw-rw-   0        0        0      235 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/RMSELoss.py
+-rw-rw-rw-   0        0        0      470 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/modules/RndNonLinearFunction.py
+-rw-rw-rw-   0        0        0     1708 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/RndProjection.py
+-rw-rw-rw-   0        0        0     2952 2024-04-08 16:14:56.000000 neural-commons-0.3.4/neural_commons/modules/SMoE.py
+-rw-rw-rw-   0        0        0      750 2024-04-07 23:57:05.000000 neural-commons-0.3.4/neural_commons/modules/SMoEMixIn.py
+-rw-rw-rw-   0        0        0      232 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/modules/View.py
+-rw-rw-rw-   0        0        0      714 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.280586 neural-commons-0.3.4/neural_commons/opt/
+-rw-rw-rw-   0        0        0     1909 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/opt/CosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0     1428 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/opt/CosineScheduler.py
+-rw-rw-rw-   0        0        0     2066 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/opt/TBCosineScheduleOptimizer.py
+-rw-rw-rw-   0        0        0      174 2024-04-28 15:00:31.000000 neural-commons-0.3.4/neural_commons/opt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.280586 neural-commons-0.3.4/neural_commons/q_nn/
+-rw-rw-rw-   0        0        0     2157 2024-05-23 13:56:40.000000 neural-commons-0.3.4/neural_commons/q_nn/ParamModule.py
+-rw-rw-rw-   0        0        0     1911 2024-05-23 16:24:52.000000 neural-commons-0.3.4/neural_commons/q_nn/QConv2d.py
+-rw-rw-rw-   0        0        0     7468 2024-05-23 13:53:33.000000 neural-commons-0.3.4/neural_commons/q_nn/QGRFOptimizer.py
+-rw-rw-rw-   0        0        0     1207 2024-05-22 19:47:30.000000 neural-commons-0.3.4/neural_commons/q_nn/QLinear.py
+-rw-rw-rw-   0        0        0      372 2024-05-23 17:17:36.000000 neural-commons-0.3.4/neural_commons/q_nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.280586 neural-commons-0.3.4/neural_commons/q_nn/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/q_nn/tests/__init__.py
+-rw-rw-rw-   0        0        0     7951 2024-05-23 17:17:44.000000 neural-commons-0.3.4/neural_commons/q_nn/tests/test_qgrf_optimizer.py
+-rw-rw-rw-   0        0        0     1073 2024-05-19 22:28:27.000000 neural-commons-0.3.4/neural_commons/q_nn/tests/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:18:06.243299 neural-commons-0.3.4/neural_commons.egg-info/
+-rw-rw-rw-   0        0        0      622 2024-05-23 17:18:06.000000 neural-commons-0.3.4/neural_commons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1853 2024-05-23 17:18:06.000000 neural-commons-0.3.4/neural_commons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:18:06.000000 neural-commons-0.3.4/neural_commons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-23 17:18:06.000000 neural-commons-0.3.4/neural_commons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 17:18:06.000000 neural-commons-0.3.4/neural_commons.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 17:18:06.296209 neural-commons-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      969 2024-05-23 17:17:54.000000 neural-commons-0.3.4/setup.py
```

### Comparing `neural-commons-0.3.3/PKG-INFO` & `neural-commons-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-commons
-Version: 0.3.3
+Version: 0.3.4
 Summary: A neural network utility library for PyTorch.
 Author: Jose Solorzano
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.23
```

### Comparing `neural-commons-0.3.3/neural_commons/cf_nn/CFConv2d.py` & `neural-commons-0.3.4/neural_commons/cf_nn/CFConv2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/cf_nn/CFLinear.py` & `neural-commons-0.3.4/neural_commons/cf_nn/CFLinear.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/cf_nn/CFModule.py` & `neural-commons-0.3.4/neural_commons/cf_nn/CFModule.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/cf_nn/CFOptimizer.py` & `neural-commons-0.3.4/neural_commons/cf_nn/CFOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/cf_nn/tests/test_cf_optimizer.py` & `neural-commons-0.3.4/neural_commons/cf_nn/tests/test_cf_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/cf_nn/tests/utils.py` & `neural-commons-0.3.4/neural_commons/cf_nn/tests/utils.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/helpers/torch_helper.py` & `neural-commons-0.3.4/neural_commons/helpers/torch_helper.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/modules/AdaptiveSimpleNorm.py` & `neural-commons-0.3.4/neural_commons/modules/AdaptiveSimpleNorm.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/modules/ConvMixer2d.py` & `neural-commons-0.3.4/neural_commons/modules/ConvMixer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/modules/InputEncoder.py` & `neural-commons-0.3.4/neural_commons/modules/InputEncoder.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/modules/NeuralLayer.py` & `neural-commons-0.3.4/neural_commons/modules/NeuralLayer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/modules/NeuralLayer2d.py` & `neural-commons-0.3.4/neural_commons/modules/NeuralLayer2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/modules/RndProjection.py` & `neural-commons-0.3.4/neural_commons/modules/RndProjection.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/modules/SMoE.py` & `neural-commons-0.3.4/neural_commons/modules/SMoE.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/modules/SMoEMixIn.py` & `neural-commons-0.3.4/neural_commons/modules/SMoEMixIn.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/modules/__init__.py` & `neural-commons-0.3.4/neural_commons/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/opt/CosineScheduleOptimizer.py` & `neural-commons-0.3.4/neural_commons/opt/CosineScheduleOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/opt/CosineScheduler.py` & `neural-commons-0.3.4/neural_commons/opt/CosineScheduler.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/opt/TBCosineScheduleOptimizer.py` & `neural-commons-0.3.4/neural_commons/opt/TBCosineScheduleOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/q_nn/ParamModule.py` & `neural-commons-0.3.4/neural_commons/q_nn/ParamModule.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/q_nn/QConv2d.py` & `neural-commons-0.3.4/neural_commons/q_nn/QConv2d.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/q_nn/QGRFOptimizer.py` & `neural-commons-0.3.4/neural_commons/q_nn/QGRFOptimizer.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/q_nn/QLinear.py` & `neural-commons-0.3.4/neural_commons/q_nn/QLinear.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons/q_nn/tests/test_qgrf_optimizer.py` & `neural-commons-0.3.4/neural_commons/q_nn/tests/test_qgrf_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import unittest
 import torch
 from torch import nn
 from neural_commons.modules import RndProjection, ArgMax, MAELoss, View
 from neural_commons.modules.Plus import Plus
-from neural_commons.q_nn import QLinear, QGRFOptimizer
-from neural_commons.q_nn.QConv2d import QConv2d
+from neural_commons.q_nn import QLinear, QGRFOptimizer, QConv2d
 from neural_commons.q_nn.tests.utils import InvGaussianLoss, IrregularLoss
 
 
 class TestQGRFOptimizer(unittest.TestCase):
     def test_regression_with_bias(self):
         in_features = 32
         out_features = 24
```

### Comparing `neural-commons-0.3.3/neural_commons/q_nn/tests/utils.py` & `neural-commons-0.3.4/neural_commons/q_nn/tests/utils.py`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/neural_commons.egg-info/PKG-INFO` & `neural-commons-0.3.4/neural_commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-commons
-Version: 0.3.3
+Version: 0.3.4
 Summary: A neural network utility library for PyTorch.
 Author: Jose Solorzano
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.23
```

### Comparing `neural-commons-0.3.3/neural_commons.egg-info/SOURCES.txt` & `neural-commons-0.3.4/neural_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural-commons-0.3.3/setup.py` & `neural-commons-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 
 from setuptools import setup, find_packages
 
 # Define project metadata
 NAME = 'neural-commons'
-VERSION = '0.3.3'
+VERSION = '0.3.4'
 DESCRIPTION = 'A neural network utility library for PyTorch.'
 AUTHOR = 'Jose Solorzano'
 
 REQUIRES = [
     'numpy>=1.23',
     'tqdm>=4.0.0',
     'torch>=2.1.0',
```

