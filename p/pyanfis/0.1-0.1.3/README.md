# Comparing `tmp/pyanfis-0.1.tar.gz` & `tmp/pyanfis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanfis-0.1.tar", last modified: Mon May 20 13:08:10 2024, max compression
+gzip compressed data, was "pyanfis-0.1.3.tar", last modified: Wed May 22 17:42:26 2024, max compression
```

## Comparing `pyanfis-0.1.tar` & `pyanfis-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-20 13:08:10.963667 pyanfis-0.1/
--rw-r--r--   0 vicente    (501) staff       (20)     1073 2024-05-20 13:06:33.000000 pyanfis-0.1/LICENSE
--rw-r--r--   0 vicente    (501) staff       (20)     1658 2024-05-20 13:08:10.963491 pyanfis-0.1/PKG-INFO
--rw-r--r--   0 vicente    (501) staff       (20)     1193 2024-05-13 09:31:46.000000 pyanfis-0.1/README.md
--rw-r--r--   0 vicente    (501) staff       (20)      455 2024-05-20 13:05:51.000000 pyanfis-0.1/pyproject.toml
--rw-r--r--   0 vicente    (501) staff       (20)       38 2024-05-20 13:08:10.963707 pyanfis-0.1/setup.cfg
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-20 13:08:10.958025 pyanfis-0.1/src/
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-20 13:08:10.959015 pyanfis-0.1/src/pyanfis/
--rw-r--r--   0 vicente    (501) staff       (20)       43 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/__init__.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-20 13:08:10.959831 pyanfis-0.1/src/pyanfis/algorithms/
--rw-r--r--   0 vicente    (501) staff       (20)     1136 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/algorithms/LSTSQ.py
--rw-r--r--   0 vicente    (501) staff       (20)     1207 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/algorithms/RLSE.py
--rw-r--r--   0 vicente    (501) staff       (20)       76 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/algorithms/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)    19952 2024-05-20 07:41:00.000000 pyanfis-0.1/src/pyanfis/anfis.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-20 13:08:10.960088 pyanfis-0.1/src/pyanfis/antecedents/
--rwxr-xr-x   0 vicente    (501) staff       (20)       63 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/antecedents/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)     1752 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/antecedents/antecedents.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-20 13:08:10.960368 pyanfis-0.1/src/pyanfis/consequents/
--rwxr-xr-x   0 vicente    (501) staff       (20)      212 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/consequents/__init__.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     1668 2024-05-13 17:29:36.000000 pyanfis-0.1/src/pyanfis/consequents/consequents.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-20 13:08:10.960900 pyanfis-0.1/src/pyanfis/consequents/types/
--rwxr-xr-x   0 vicente    (501) staff       (20)     1077 2024-05-13 17:42:35.000000 pyanfis-0.1/src/pyanfis/consequents/types/algorithm.py
--rw-r--r--   0 vicente    (501) staff       (20)      833 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/consequents/types/lee.py
--rw-r--r--   0 vicente    (501) staff       (20)     1593 2024-05-17 18:35:06.000000 pyanfis-0.1/src/pyanfis/consequents/types/takagi_sugeno.py
--rw-r--r--   0 vicente    (501) staff       (20)     2148 2024-05-17 18:35:18.000000 pyanfis-0.1/src/pyanfis/consequents/types/tsukamoto.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-20 13:08:10.961921 pyanfis-0.1/src/pyanfis/functions/
--rw-r--r--   0 vicente    (501) staff       (20)      287 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/functions/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)      979 2024-05-17 09:25:31.000000 pyanfis-0.1/src/pyanfis/functions/bell.py
--rw-r--r--   0 vicente    (501) staff       (20)     1524 2024-05-17 10:25:03.000000 pyanfis-0.1/src/pyanfis/functions/gauss.py
--rw-r--r--   0 vicente    (501) staff       (20)     1567 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/functions/heaviside.py
--rw-r--r--   0 vicente    (501) staff       (20)     1164 2024-05-17 09:21:58.000000 pyanfis-0.1/src/pyanfis/functions/linear_s.py
--rw-r--r--   0 vicente    (501) staff       (20)     1186 2024-05-17 09:22:02.000000 pyanfis-0.1/src/pyanfis/functions/linear_z.py
--rw-r--r--   0 vicente    (501) staff       (20)      837 2024-05-17 09:22:06.000000 pyanfis-0.1/src/pyanfis/functions/sigmoid.py
--rw-r--r--   0 vicente    (501) staff       (20)     3461 2024-05-13 17:43:56.000000 pyanfis-0.1/src/pyanfis/functions/universe.py
--rw-r--r--   0 vicente    (501) staff       (20)      293 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/functions/utils.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-20 13:08:10.962188 pyanfis-0.1/src/pyanfis/optimizers/
--rw-r--r--   0 vicente    (501) staff       (20)       54 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/optimizers/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)     6877 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/optimizers/fuzzySGD.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-20 13:08:10.962780 pyanfis-0.1/src/pyanfis/rules/
--rwxr-xr-x   0 vicente    (501) staff       (20)       46 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/rules/__init__.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     2904 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/rules/intersection_algorithms.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     1527 2024-05-13 09:31:46.000000 pyanfis-0.1/src/pyanfis/rules/relation_algorithms.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     1976 2024-05-13 17:14:57.000000 pyanfis-0.1/src/pyanfis/rules/rules.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-20 13:08:10.963302 pyanfis-0.1/src/pyanfis.egg-info/
--rw-r--r--   0 vicente    (501) staff       (20)     1658 2024-05-20 13:08:10.000000 pyanfis-0.1/src/pyanfis.egg-info/PKG-INFO
--rw-r--r--   0 vicente    (501) staff       (20)     1144 2024-05-20 13:08:10.000000 pyanfis-0.1/src/pyanfis.egg-info/SOURCES.txt
--rw-r--r--   0 vicente    (501) staff       (20)        1 2024-05-20 13:08:10.000000 pyanfis-0.1/src/pyanfis.egg-info/dependency_links.txt
--rw-r--r--   0 vicente    (501) staff       (20)        8 2024-05-20 13:08:10.000000 pyanfis-0.1/src/pyanfis.egg-info/top_level.txt
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.509207 pyanfis-0.1.3/
+-rw-r--r--   0 vicente    (501) staff       (20)     1073 2024-05-20 13:06:33.000000 pyanfis-0.1.3/LICENSE
+-rw-r--r--   0 vicente    (501) staff       (20)     1659 2024-05-22 17:42:26.509029 pyanfis-0.1.3/PKG-INFO
+-rw-r--r--   0 vicente    (501) staff       (20)     1193 2024-05-13 09:31:46.000000 pyanfis-0.1.3/README.md
+-rw-r--r--   0 vicente    (501) staff       (20)      456 2024-05-22 16:50:37.000000 pyanfis-0.1.3/pyproject.toml
+-rw-r--r--   0 vicente    (501) staff       (20)       38 2024-05-22 17:42:26.509248 pyanfis-0.1.3/setup.cfg
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.503501 pyanfis-0.1.3/src/
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.504475 pyanfis-0.1.3/src/pyanfis/
+-rw-r--r--   0 vicente    (501) staff       (20)       45 2024-05-22 16:48:25.000000 pyanfis-0.1.3/src/pyanfis/__init__.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.505306 pyanfis-0.1.3/src/pyanfis/algorithms/
+-rw-r--r--   0 vicente    (501) staff       (20)     1136 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/algorithms/LSTSQ.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1207 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/algorithms/RLSE.py
+-rw-r--r--   0 vicente    (501) staff       (20)       76 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/algorithms/__init__.py
+-rw-r--r--   0 vicente    (501) staff       (20)    20053 2024-05-22 17:39:05.000000 pyanfis-0.1.3/src/pyanfis/anfis.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.505555 pyanfis-0.1.3/src/pyanfis/antecedents/
+-rwxr-xr-x   0 vicente    (501) staff       (20)       63 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/antecedents/__init__.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1760 2024-05-22 17:02:39.000000 pyanfis-0.1.3/src/pyanfis/antecedents/antecedents.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.505803 pyanfis-0.1.3/src/pyanfis/consequents/
+-rwxr-xr-x   0 vicente    (501) staff       (20)      212 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/consequents/__init__.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1725 2024-05-22 17:06:13.000000 pyanfis-0.1.3/src/pyanfis/consequents/consequents.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.506312 pyanfis-0.1.3/src/pyanfis/consequents/types/
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1085 2024-05-22 17:06:25.000000 pyanfis-0.1.3/src/pyanfis/consequents/types/algorithm.py
+-rw-r--r--   0 vicente    (501) staff       (20)      841 2024-05-22 17:06:33.000000 pyanfis-0.1.3/src/pyanfis/consequents/types/lee.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1600 2024-05-22 17:42:19.000000 pyanfis-0.1.3/src/pyanfis/consequents/types/takagi_sugeno.py
+-rw-r--r--   0 vicente    (501) staff       (20)     2156 2024-05-22 17:07:01.000000 pyanfis-0.1.3/src/pyanfis/consequents/types/tsukamoto.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.507499 pyanfis-0.1.3/src/pyanfis/functions/
+-rw-r--r--   0 vicente    (501) staff       (20)      287 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/functions/__init__.py
+-rw-r--r--   0 vicente    (501) staff       (20)      979 2024-05-17 09:25:31.000000 pyanfis-0.1.3/src/pyanfis/functions/bell.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1524 2024-05-17 10:25:03.000000 pyanfis-0.1.3/src/pyanfis/functions/gauss.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1567 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/functions/heaviside.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1164 2024-05-17 09:21:58.000000 pyanfis-0.1.3/src/pyanfis/functions/linear_s.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1186 2024-05-17 09:22:02.000000 pyanfis-0.1.3/src/pyanfis/functions/linear_z.py
+-rw-r--r--   0 vicente    (501) staff       (20)      837 2024-05-17 09:22:06.000000 pyanfis-0.1.3/src/pyanfis/functions/sigmoid.py
+-rw-r--r--   0 vicente    (501) staff       (20)     3461 2024-05-13 17:43:56.000000 pyanfis-0.1.3/src/pyanfis/functions/universe.py
+-rw-r--r--   0 vicente    (501) staff       (20)      293 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/functions/utils.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.507806 pyanfis-0.1.3/src/pyanfis/optimizers/
+-rw-r--r--   0 vicente    (501) staff       (20)       54 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/optimizers/__init__.py
+-rw-r--r--   0 vicente    (501) staff       (20)     6877 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/optimizers/fuzzySGD.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.508396 pyanfis-0.1.3/src/pyanfis/rules/
+-rwxr-xr-x   0 vicente    (501) staff       (20)       46 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/rules/__init__.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     2904 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/rules/intersection_algorithms.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1527 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/rules/relation_algorithms.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1917 2024-05-22 17:05:40.000000 pyanfis-0.1.3/src/pyanfis/rules/rules.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.508845 pyanfis-0.1.3/src/pyanfis.egg-info/
+-rw-r--r--   0 vicente    (501) staff       (20)     1659 2024-05-22 17:42:26.000000 pyanfis-0.1.3/src/pyanfis.egg-info/PKG-INFO
+-rw-r--r--   0 vicente    (501) staff       (20)     1144 2024-05-22 17:42:26.000000 pyanfis-0.1.3/src/pyanfis.egg-info/SOURCES.txt
+-rw-r--r--   0 vicente    (501) staff       (20)        1 2024-05-22 17:42:26.000000 pyanfis-0.1.3/src/pyanfis.egg-info/dependency_links.txt
+-rw-r--r--   0 vicente    (501) staff       (20)        8 2024-05-22 17:42:26.000000 pyanfis-0.1.3/src/pyanfis.egg-info/top_level.txt
```

### Comparing `pyanfis-0.1/LICENSE` & `pyanfis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/PKG-INFO` & `pyanfis-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyanfis
-Version: 0.1
-Summary: An pytorch-based package to use ANFIS for AI
+Version: 0.1.3
+Summary: A pytorch-based package to use ANFIS for AI
 Author-email: Vicente Feced Mas <vicente.feced.mas@gmail.com>
 Project-URL: Homepage, https://github.com/VicenteFecedMas/pyanfis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyANFIS
 
 Welcome to pyANFIS! here you will be able to find a framework that will allow you to use **Fuzzy Logic** with usual pytorch layers.
 This framework is based on [Jang's](https://www.researchgate.net/publication/3113825_ANFIS_Adaptive-Network-based_Fuzzy_Inference_System?enrichId=rgreq-15825cac70a3ae795992310484420cab-XXX&enrichSource=Y292ZXJQYWdlOzMxMTM4MjU7QVM6MTU5MDc1MDY1MTQ3MzkyQDE0MTQ5Mzc4NTk3MzI%3D&el=1_x_2&_esc=publicationCoverPdf) original paper, although it is going to implement several more things (listed below).
```

### Comparing `pyanfis-0.1/README.md` & `pyanfis-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/algorithms/LSTSQ.py` & `pyanfis-0.1.3/src/pyanfis/algorithms/LSTSQ.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/algorithms/RLSE.py` & `pyanfis-0.1.3/src/pyanfis/algorithms/RLSE.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/anfis.py` & `pyanfis-0.1.3/src/pyanfis/anfis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import torch
 import math
 
-from antecedents import Antecedents
-from rules import Rules
-from consequents import Consequents
+from pyanfis.antecedents import Antecedents
+from pyanfis.rules import Rules
+from pyanfis.consequents import Consequents
 
 class ANFIS(torch.nn.Module):
-    def __init__(self, num_inputs:int, num_outputs:int, system_type:str="Takagi-Sugeno", consequents_parameters_update:str = 'backward',):
+    def __init__(self, num_inputs:int, num_outputs:int, system_type:str="Takagi-Sugeno", parameters_update:str = 'backward',):
         super().__init__()
         self.num_inputs = num_inputs
         self.num_outputs = num_outputs
         self.system_type = system_type
 
-        self.params_update = consequents_parameters_update
+        self.parameters_update = parameters_update
 
         self.antecedents = Antecedents(num_inputs)
         self.rules = Rules()
         self.normalisation = torch.nn.functional.normalize
-        self.consequents = Consequents(num_inputs=num_inputs, num_outputs=num_outputs, parameters_update=self.params_update, system_type=self.system_type)
+        self.consequents = Consequents(num_inputs=num_inputs, num_outputs=num_outputs, parameters_update=self.parameters_update, system_type=self.system_type)
 
         self.active_rules = None
         self.active_rules_consequents = None
         self.rules_relevancy = None
         self.erase_irrelevant_rules = None
 
 
@@ -114,15 +114,15 @@
         # Antecedents parameters
         for universe in self.antecedents.universes.values():
             for function in universe.functions.values():
                 for param in function.parameters():
                     parameters.append(param)
 
         # Consequent parameters
-        if self.params_update == "backward":
+        if self.parameters_update == "backward":
             for universe in self.consequents.consequents.universes.values():
                 if self.system_type == "Takagi-Sugeno":
                     parameters.append(universe.theta)
                 else:
                     for function in universe.functions.values():
                         for param in function.parameters():
                             parameters.append(param)
@@ -139,25 +139,23 @@
         elif dimensions == 1:
             return tensor_list.view(1,shape[0],-1)
         elif dimensions == 2:
             return tensor_list.view(shape[0], shape[1],-1)
         elif dimensions == 3:
             return tensor_list.view(shape[0], shape[1] * shape[2] , -1) 
         
-    def _prepare_input_matrices(self, **kwargs):
-        if len(kwargs) != len(self.antecedents.universes.items()):
-            
+    def _prepare_keywords_matrices(self, **kwargs):
         antecedents_tensor = []
         for universe in self.antecedents.universes.values():
             if universe.name not in list(kwargs.keys()):
                 raise ValueError(f"Universe name {universe.name} not present in input variables {list(kwargs.keys())}")
             antecedents_tensor.append(kwargs[universe.name])
             del kwargs[universe.name]
         
-        if not kwargs and self.system_type == "Takagi-Sugeno" and self.training is True and self.params_update != "backward":
+        if not kwargs and self.system_type == "Takagi-Sugeno" and self.training is True and self.parameters_update != "backward":
             raise ValueError(f"If you use a {self.system_type} and do not update the system using backpropagation you need to feed the output values to train the system.")
         elif not kwargs:
             return self.smart_concat(antecedents_tensor), None
          
         consequents_tensor = []
         for universe in self.consequents.consequents.universes.values():
             if universe.name not in list(kwargs.keys()):
@@ -166,15 +164,15 @@
             consequents_tensor.append(kwargs[universe.name])
             del kwargs[universe.name]
 
         return self.smart_concat(antecedents_tensor), self.smart_concat(consequents_tensor)
 
     def get_fired_rules(self, **kwargs):
         self.training = False
-        X, _ = self._prepare_input_matrices(**kwargs)
+        X, _ = self._prepare_keywords_matrices(**kwargs)
         if X.size(1) != 1:
             raise ValueError(f"Only one row can be evaluated at a time")
 
         f = self.antecedents(X)
 
         self.rules.active_rules = self.active_rules
         f, _ = self.rules(f) # col_indexes = rule place on each col
@@ -187,15 +185,15 @@
         params = {}
 
         # Main
         params["main"] = {}
         params["main"]["num_inputs"] = self.num_inputs
         params["main"]["num_outputs"] = self.num_outputs
         params["main"]["system_type"] = self.system_type
-        params["main"]["params_update"] = self.params_update
+        params["main"]["parameters_update"] = self.parameters_update
         params["main"]["active_rules"] = self.active_rules
         params["main"]["rules_relevancy"] = self.rules_relevancy
         params["main"]["active_rules_consequents"] = self.active_rules_consequents
         params["main"]["erase_irrelevant_rules"] = self.erase_irrelevant_rules
         params["main"]["firing_strength"] = self.firing_strength
 
         # Antecedents
@@ -256,20 +254,20 @@
         if self.num_inputs != state_dict["main"]["num_inputs"]:
             raise ImportError(f"Atempting to import a system with {state_dict['main']['num_inputs']} inputs into a created system of {self.num_inputs} inputs.")
         
         if self.num_outputs != state_dict["main"]["num_outputs"]:
             raise ImportError(f"Atempting to import a system with {state_dict['main']['num_outputs']} outputs into a created system of {self.num_outputs} outputs.")
         
         self.system_type = state_dict["main"]["system_type"]
-        self.params_update = state_dict["main"]["params_update"]
+        self.parameters_update = state_dict["main"]["parameters_update"]
 
         self.antecedents = Antecedents(self.num_inputs)
         self.rules = Rules()
         self.normalisation = torch.nn.functional.normalize
-        self.consequents = Consequents(num_inputs=self.num_inputs, num_outputs=self.num_outputs, parameters_update=self.params_update, system_type=self.system_type)
+        self.consequents = Consequents(num_inputs=self.num_inputs, num_outputs=self.num_outputs, parameters_update=self.parameters_update, system_type=self.system_type)
 
         self.active_rules = state_dict["main"]["active_rules"]
         self.active_rules_consequents = state_dict["main"]["active_rules_consequents"]
         self.rules_relevancy = state_dict["main"]["rules_relevancy"]
         self.erase_irrelevant_rules = state_dict["main"]["erase_irrelevant_rules"]
 
         self.firing_strength = state_dict["main"]["firing_strength"]
@@ -334,23 +332,28 @@
         if self.rules_relevancy is None:
             self.rules_relevancy = relevancy
         else:
             self.rules_relevancy += relevancy
 
         self.rules_relevancy = torch.nn.functional.normalize(self.rules_relevancy, dim=0, p=1)
 
-    def get_conversion_number(self, x):
-        if x == 0:
-            return 1.0
-        
-        x = math.floor(math.log10(abs(x)))
-        if x > 0:
-            return float("1" + "0" * x)
-        else:
-            return float("0." + "0" * abs(x) + "1")
+    def _sanity_check(self, matrix):
+        '''
+        Will check if a matrice is batched
+        '''
+        if matrix is None:
+            return None
+        
+        if matrix.dim() == 2:
+            return matrix[None, :, :]
+        elif matrix.dim() == 3:
+            return matrix
+        elif matrix.dim() > 3 or matrix.dim() < 2:
+            raise ValueError(f"Expected a matrix with 2 or 3 dimensions but got one with {matrix.dim()}")
+        
 
     def forward(self, X, Y):
         f = self.antecedents(X)
 
         self.rules.active_rules = self.active_rules
         f = self.rules(f)
         
@@ -367,50 +370,29 @@
         In the call step I will preprocess the data and discern if 
         I am being asked a control/regression or a classification task.
         '''
 
         if args and kwargs:
             raise ValueError("All the arguments must be either arguments or keyword arguments, but you cannot mix between both")
 
-        # I NEED TO DISCOVER HOW THE DATA ENTERS
+        if args and not isinstance(args[0], torch.Tensor):
+            raise ValueError(f"Expected torch.Tensor as input but recived {type(args)}")
+        
         if kwargs:
-            X, Y = self._prepare_input_matrices(**kwargs)
+            X, Y = self._prepare_keywords_matrices(**kwargs)
         
         else:
             if len(args) > 2:
-                raise ValueError("Please provide as input either a matrix with the X arguments or two matrices, one with X arguments and one with Y arguments")
-            X, Y = args
+                raise ValueError("Please provide as input either a matrix with the input arguments or two matrices, one with input arguments and one with objective arguments")
 
-        print(X, Y)
-        return self.forward(X, Y)
-        
+            if self.parameters_update == "backward" and len(args) >= 2:
+                raise ValueError(f"The selected propagation is {self.parameters_update} but you provided more than one tensor as input. Please, join all the input tensors before feeding them into the system.") 
 
-from functions import LinearS, LinearZ
-import torch
-
-anfis = ANFIS(num_inputs=2, num_outputs=1)
+            if self.parameters_update == "backward":
+                X, Y = args[0], None
+            else:
+                X, Y = args
+        X, Y = self._sanity_check(X), self._sanity_check(Y)
 
-anfis.inputs['Input 1'].range = 0, 10
-anfis.inputs['Input 1'].name = 'X'
-anfis.inputs['Input 1'].functions["Token1"] = LinearS(0, 10)
-
-anfis.inputs['Input 2'].range = 0, 10
-anfis.inputs['Input 2'].name = 'Y'
-anfis.inputs['Input 2'].functions["Token2"] = LinearZ(0, 10)
-
-anfis.create_rules_base([
-    "If Token1",
-    "If Token2"
-])
-
-X = torch.rand(1, 1)
-Y = torch.rand(1, 1)
-print(' ')
-print('Pasando argumentos posicionales')
-anfis(X=X, Y=Y)
-print(' ')
-print('Pasando argumentos no posicionales')
-anfis(X, Y)
-print(' ')
-print('Pasando argumentos mix')
-anfis(X, Y, X)
+        # NEEDS TO GET TESTED FOR DIFFERENT USECASES
 
+        return self.forward(X, Y)
```

### Comparing `pyanfis-0.1/src/pyanfis/antecedents/antecedents.py` & `pyanfis-0.1.3/src/pyanfis/antecedents/antecedents.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from functions import Universe
+from pyanfis.functions import Universe
 
 class Antecedents(torch.nn.Module):
     """
     This class is used to define the range in which a variable
     is going to be defined in a fuzzy way, it is composed of
     several functions used to describe it.
```

### Comparing `pyanfis-0.1/src/pyanfis/consequents/consequents.py` & `pyanfis-0.1.3/src/pyanfis/consequents/consequents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 
-from .types.takagi_sugeno import TakagiSugeno
-from .types.tsukamoto import Tsukamoto
-from .types.lee import Lee
+from pyanfis.consequents.types.takagi_sugeno import TakagiSugeno
+from pyanfis.consequents.types.tsukamoto import Tsukamoto
+from pyanfis.consequents.types.lee import Lee
 
 
 
 CONSEQUENTS = {
     "Takagi-Sugeno": lambda num_inputs, num_outputs, parameters_update: TakagiSugeno(num_inputs, num_outputs, parameters_update),
     "Tsukamoto": lambda num_inputs, num_outputs, parameters_update: Tsukamoto(num_inputs, num_outputs, parameters_update),
     "Lee": lambda num_inputs, num_outputs, parameters_update: Lee(num_inputs, num_outputs, parameters_update),
```

### Comparing `pyanfis-0.1/src/pyanfis/consequents/types/algorithm.py` & `pyanfis-0.1.3/src/pyanfis/consequents/types/algorithm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from algorithms import LSTSQ, RLSE
+from pyanfis.algorithms import LSTSQ, RLSE
 
 ALGORITHMS = {
     "LSTSQ": lambda n_vars: LSTSQ(n_vars),
     "RLSE":  lambda n_vars: RLSE(n_vars),
 }
 
 class TakagiSugenoAlgorithm(torch.nn.Module):
```

### Comparing `pyanfis-0.1/src/pyanfis/consequents/types/lee.py` & `pyanfis-0.1.3/src/pyanfis/consequents/types/lee.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from functions import Sigmoid
+from pyanfis.functions import Sigmoid
 
 
 class Lee(torch.nn.Module):
     """
     This class will compute the learnable parameters using the Lee approach.
 
     Attributes
```

### Comparing `pyanfis-0.1/src/pyanfis/consequents/types/takagi_sugeno.py` & `pyanfis-0.1.3/src/pyanfis/consequents/types/takagi_sugeno.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,11 +37,10 @@
         #output = {f"Output {i+1}": torch.zeros((x_b, x_i , 1)) for i in range(self.num_outputs)}
         outputs = torch.zeros(f.size(0), f.size(1), self.num_outputs)
         X = torch.einsum('bri, brj -> brij', f, X).view(x_b, x_i, -1)
 
         for i, (algorithm) in enumerate(self.universes.values()):
             if Y is not None:
                 algorithm(X, Y[:, :, i:i+1])
-
-            outputs[:, :, i] = outputs[:, :, i] + torch.einsum('bij, jk -> bik', X, algorithm.theta)
+            outputs[:, :, i:i+1] = outputs[:, :, i:i+1] + torch.einsum('bij, jk -> bik', X, algorithm.theta)
    
         return outputs
```

### Comparing `pyanfis-0.1/src/pyanfis/consequents/types/tsukamoto.py` & `pyanfis-0.1.3/src/pyanfis/consequents/types/tsukamoto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from functions import Universe
+from pyanfis.functions import Universe
 
 
 class Tsukamoto(torch.nn.Module):
     """
     This class will compute the learnable parameters using the Tsukamoto approach.
 
     Attributes
```

### Comparing `pyanfis-0.1/src/pyanfis/functions/bell.py` & `pyanfis-0.1.3/src/pyanfis/functions/bell.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/functions/gauss.py` & `pyanfis-0.1.3/src/pyanfis/functions/gauss.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/functions/heaviside.py` & `pyanfis-0.1.3/src/pyanfis/functions/heaviside.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/functions/linear_s.py` & `pyanfis-0.1.3/src/pyanfis/functions/linear_s.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/functions/linear_z.py` & `pyanfis-0.1.3/src/pyanfis/functions/linear_z.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/functions/sigmoid.py` & `pyanfis-0.1.3/src/pyanfis/functions/sigmoid.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/functions/universe.py` & `pyanfis-0.1.3/src/pyanfis/functions/universe.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/optimizers/fuzzySGD.py` & `pyanfis-0.1.3/src/pyanfis/optimizers/fuzzySGD.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/rules/intersection_algorithms.py` & `pyanfis-0.1.3/src/pyanfis/rules/intersection_algorithms.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/rules/relation_algorithms.py` & `pyanfis-0.1.3/src/pyanfis/rules/relation_algorithms.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1/src/pyanfis/rules/rules.py` & `pyanfis-0.1.3/src/pyanfis/rules/rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import torch
 
-from consequents import TakagiSugeno
-
-from .intersection_algorithms import *
-from .relation_algorithms import *
+from .intersection_algorithms import larsen, mamdani
 
 INTERSECTIONS = {
     'larsen': larsen,
     'mamdani': mamdani,
 }
```

### Comparing `pyanfis-0.1/src/pyanfis.egg-info/PKG-INFO` & `pyanfis-0.1.3/src/pyanfis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyanfis
-Version: 0.1
-Summary: An pytorch-based package to use ANFIS for AI
+Version: 0.1.3
+Summary: A pytorch-based package to use ANFIS for AI
 Author-email: Vicente Feced Mas <vicente.feced.mas@gmail.com>
 Project-URL: Homepage, https://github.com/VicenteFecedMas/pyanfis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyANFIS
 
 Welcome to pyANFIS! here you will be able to find a framework that will allow you to use **Fuzzy Logic** with usual pytorch layers.
 This framework is based on [Jang's](https://www.researchgate.net/publication/3113825_ANFIS_Adaptive-Network-based_Fuzzy_Inference_System?enrichId=rgreq-15825cac70a3ae795992310484420cab-XXX&enrichSource=Y292ZXJQYWdlOzMxMTM4MjU7QVM6MTU5MDc1MDY1MTQ3MzkyQDE0MTQ5Mzc4NTk3MzI%3D&el=1_x_2&_esc=publicationCoverPdf) original paper, although it is going to implement several more things (listed below).
```

### Comparing `pyanfis-0.1/src/pyanfis.egg-info/SOURCES.txt` & `pyanfis-0.1.3/src/pyanfis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

