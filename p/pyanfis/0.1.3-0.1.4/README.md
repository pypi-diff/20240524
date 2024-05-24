# Comparing `tmp/pyanfis-0.1.3.tar.gz` & `tmp/pyanfis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanfis-0.1.3.tar", last modified: Wed May 22 17:42:26 2024, max compression
+gzip compressed data, was "pyanfis-0.1.4.tar", last modified: Fri May 24 11:43:12 2024, max compression
```

## Comparing `pyanfis-0.1.3.tar` & `pyanfis-0.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.509207 pyanfis-0.1.3/
--rw-r--r--   0 vicente    (501) staff       (20)     1073 2024-05-20 13:06:33.000000 pyanfis-0.1.3/LICENSE
--rw-r--r--   0 vicente    (501) staff       (20)     1659 2024-05-22 17:42:26.509029 pyanfis-0.1.3/PKG-INFO
--rw-r--r--   0 vicente    (501) staff       (20)     1193 2024-05-13 09:31:46.000000 pyanfis-0.1.3/README.md
--rw-r--r--   0 vicente    (501) staff       (20)      456 2024-05-22 16:50:37.000000 pyanfis-0.1.3/pyproject.toml
--rw-r--r--   0 vicente    (501) staff       (20)       38 2024-05-22 17:42:26.509248 pyanfis-0.1.3/setup.cfg
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.503501 pyanfis-0.1.3/src/
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.504475 pyanfis-0.1.3/src/pyanfis/
--rw-r--r--   0 vicente    (501) staff       (20)       45 2024-05-22 16:48:25.000000 pyanfis-0.1.3/src/pyanfis/__init__.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.505306 pyanfis-0.1.3/src/pyanfis/algorithms/
--rw-r--r--   0 vicente    (501) staff       (20)     1136 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/algorithms/LSTSQ.py
--rw-r--r--   0 vicente    (501) staff       (20)     1207 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/algorithms/RLSE.py
--rw-r--r--   0 vicente    (501) staff       (20)       76 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/algorithms/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)    20053 2024-05-22 17:39:05.000000 pyanfis-0.1.3/src/pyanfis/anfis.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.505555 pyanfis-0.1.3/src/pyanfis/antecedents/
--rwxr-xr-x   0 vicente    (501) staff       (20)       63 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/antecedents/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)     1760 2024-05-22 17:02:39.000000 pyanfis-0.1.3/src/pyanfis/antecedents/antecedents.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.505803 pyanfis-0.1.3/src/pyanfis/consequents/
--rwxr-xr-x   0 vicente    (501) staff       (20)      212 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/consequents/__init__.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     1725 2024-05-22 17:06:13.000000 pyanfis-0.1.3/src/pyanfis/consequents/consequents.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.506312 pyanfis-0.1.3/src/pyanfis/consequents/types/
--rwxr-xr-x   0 vicente    (501) staff       (20)     1085 2024-05-22 17:06:25.000000 pyanfis-0.1.3/src/pyanfis/consequents/types/algorithm.py
--rw-r--r--   0 vicente    (501) staff       (20)      841 2024-05-22 17:06:33.000000 pyanfis-0.1.3/src/pyanfis/consequents/types/lee.py
--rw-r--r--   0 vicente    (501) staff       (20)     1600 2024-05-22 17:42:19.000000 pyanfis-0.1.3/src/pyanfis/consequents/types/takagi_sugeno.py
--rw-r--r--   0 vicente    (501) staff       (20)     2156 2024-05-22 17:07:01.000000 pyanfis-0.1.3/src/pyanfis/consequents/types/tsukamoto.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.507499 pyanfis-0.1.3/src/pyanfis/functions/
--rw-r--r--   0 vicente    (501) staff       (20)      287 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/functions/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)      979 2024-05-17 09:25:31.000000 pyanfis-0.1.3/src/pyanfis/functions/bell.py
--rw-r--r--   0 vicente    (501) staff       (20)     1524 2024-05-17 10:25:03.000000 pyanfis-0.1.3/src/pyanfis/functions/gauss.py
--rw-r--r--   0 vicente    (501) staff       (20)     1567 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/functions/heaviside.py
--rw-r--r--   0 vicente    (501) staff       (20)     1164 2024-05-17 09:21:58.000000 pyanfis-0.1.3/src/pyanfis/functions/linear_s.py
--rw-r--r--   0 vicente    (501) staff       (20)     1186 2024-05-17 09:22:02.000000 pyanfis-0.1.3/src/pyanfis/functions/linear_z.py
--rw-r--r--   0 vicente    (501) staff       (20)      837 2024-05-17 09:22:06.000000 pyanfis-0.1.3/src/pyanfis/functions/sigmoid.py
--rw-r--r--   0 vicente    (501) staff       (20)     3461 2024-05-13 17:43:56.000000 pyanfis-0.1.3/src/pyanfis/functions/universe.py
--rw-r--r--   0 vicente    (501) staff       (20)      293 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/functions/utils.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.507806 pyanfis-0.1.3/src/pyanfis/optimizers/
--rw-r--r--   0 vicente    (501) staff       (20)       54 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/optimizers/__init__.py
--rw-r--r--   0 vicente    (501) staff       (20)     6877 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/optimizers/fuzzySGD.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.508396 pyanfis-0.1.3/src/pyanfis/rules/
--rwxr-xr-x   0 vicente    (501) staff       (20)       46 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/rules/__init__.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     2904 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/rules/intersection_algorithms.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     1527 2024-05-13 09:31:46.000000 pyanfis-0.1.3/src/pyanfis/rules/relation_algorithms.py
--rwxr-xr-x   0 vicente    (501) staff       (20)     1917 2024-05-22 17:05:40.000000 pyanfis-0.1.3/src/pyanfis/rules/rules.py
-drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-22 17:42:26.508845 pyanfis-0.1.3/src/pyanfis.egg-info/
--rw-r--r--   0 vicente    (501) staff       (20)     1659 2024-05-22 17:42:26.000000 pyanfis-0.1.3/src/pyanfis.egg-info/PKG-INFO
--rw-r--r--   0 vicente    (501) staff       (20)     1144 2024-05-22 17:42:26.000000 pyanfis-0.1.3/src/pyanfis.egg-info/SOURCES.txt
--rw-r--r--   0 vicente    (501) staff       (20)        1 2024-05-22 17:42:26.000000 pyanfis-0.1.3/src/pyanfis.egg-info/dependency_links.txt
--rw-r--r--   0 vicente    (501) staff       (20)        8 2024-05-22 17:42:26.000000 pyanfis-0.1.3/src/pyanfis.egg-info/top_level.txt
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 11:43:12.613642 pyanfis-0.1.4/
+-rw-r--r--   0 vicente    (501) staff       (20)     1073 2024-05-20 13:06:33.000000 pyanfis-0.1.4/LICENSE
+-rw-r--r--   0 vicente    (501) staff       (20)     1659 2024-05-24 11:43:12.613454 pyanfis-0.1.4/PKG-INFO
+-rw-r--r--   0 vicente    (501) staff       (20)     1193 2024-05-13 09:31:46.000000 pyanfis-0.1.4/README.md
+-rw-r--r--   0 vicente    (501) staff       (20)      456 2024-05-24 11:43:02.000000 pyanfis-0.1.4/pyproject.toml
+-rw-r--r--   0 vicente    (501) staff       (20)       38 2024-05-24 11:43:12.613685 pyanfis-0.1.4/setup.cfg
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 11:43:12.607576 pyanfis-0.1.4/src/
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 11:43:12.608603 pyanfis-0.1.4/src/pyanfis/
+-rw-r--r--   0 vicente    (501) staff       (20)       45 2024-05-22 16:48:25.000000 pyanfis-0.1.4/src/pyanfis/__init__.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 11:43:12.609520 pyanfis-0.1.4/src/pyanfis/algorithms/
+-rw-r--r--   0 vicente    (501) staff       (20)     1136 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/algorithms/LSTSQ.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1207 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/algorithms/RLSE.py
+-rw-r--r--   0 vicente    (501) staff       (20)       76 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/algorithms/__init__.py
+-rw-r--r--   0 vicente    (501) staff       (20)    20053 2024-05-22 17:39:05.000000 pyanfis-0.1.4/src/pyanfis/anfis.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 11:43:12.609784 pyanfis-0.1.4/src/pyanfis/antecedents/
+-rwxr-xr-x   0 vicente    (501) staff       (20)       63 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/antecedents/__init__.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1760 2024-05-22 17:02:39.000000 pyanfis-0.1.4/src/pyanfis/antecedents/antecedents.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 11:43:12.610080 pyanfis-0.1.4/src/pyanfis/consequents/
+-rwxr-xr-x   0 vicente    (501) staff       (20)      212 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/consequents/__init__.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1725 2024-05-22 17:06:13.000000 pyanfis-0.1.4/src/pyanfis/consequents/consequents.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 11:43:12.610645 pyanfis-0.1.4/src/pyanfis/consequents/types/
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1085 2024-05-22 17:06:25.000000 pyanfis-0.1.4/src/pyanfis/consequents/types/algorithm.py
+-rw-r--r--   0 vicente    (501) staff       (20)      841 2024-05-22 17:06:33.000000 pyanfis-0.1.4/src/pyanfis/consequents/types/lee.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1600 2024-05-22 17:42:19.000000 pyanfis-0.1.4/src/pyanfis/consequents/types/takagi_sugeno.py
+-rw-r--r--   0 vicente    (501) staff       (20)     2156 2024-05-22 17:07:01.000000 pyanfis-0.1.4/src/pyanfis/consequents/types/tsukamoto.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 11:43:12.611805 pyanfis-0.1.4/src/pyanfis/functions/
+-rw-r--r--   0 vicente    (501) staff       (20)      287 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/functions/__init__.py
+-rw-r--r--   0 vicente    (501) staff       (20)      979 2024-05-17 09:25:31.000000 pyanfis-0.1.4/src/pyanfis/functions/bell.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1462 2024-05-24 11:41:24.000000 pyanfis-0.1.4/src/pyanfis/functions/gauss.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1567 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/functions/heaviside.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1164 2024-05-17 09:21:58.000000 pyanfis-0.1.4/src/pyanfis/functions/linear_s.py
+-rw-r--r--   0 vicente    (501) staff       (20)     1186 2024-05-17 09:22:02.000000 pyanfis-0.1.4/src/pyanfis/functions/linear_z.py
+-rw-r--r--   0 vicente    (501) staff       (20)      837 2024-05-17 09:22:06.000000 pyanfis-0.1.4/src/pyanfis/functions/sigmoid.py
+-rw-r--r--   0 vicente    (501) staff       (20)     3461 2024-05-13 17:43:56.000000 pyanfis-0.1.4/src/pyanfis/functions/universe.py
+-rw-r--r--   0 vicente    (501) staff       (20)      293 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/functions/utils.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 11:43:12.612149 pyanfis-0.1.4/src/pyanfis/optimizers/
+-rw-r--r--   0 vicente    (501) staff       (20)       54 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/optimizers/__init__.py
+-rw-r--r--   0 vicente    (501) staff       (20)     6877 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/optimizers/fuzzySGD.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 11:43:12.612701 pyanfis-0.1.4/src/pyanfis/rules/
+-rwxr-xr-x   0 vicente    (501) staff       (20)       46 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/rules/__init__.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     2904 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/rules/intersection_algorithms.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1527 2024-05-13 09:31:46.000000 pyanfis-0.1.4/src/pyanfis/rules/relation_algorithms.py
+-rwxr-xr-x   0 vicente    (501) staff       (20)     1917 2024-05-22 17:05:40.000000 pyanfis-0.1.4/src/pyanfis/rules/rules.py
+drwxr-xr-x   0 vicente    (501) staff       (20)        0 2024-05-24 11:43:12.613256 pyanfis-0.1.4/src/pyanfis.egg-info/
+-rw-r--r--   0 vicente    (501) staff       (20)     1659 2024-05-24 11:43:12.000000 pyanfis-0.1.4/src/pyanfis.egg-info/PKG-INFO
+-rw-r--r--   0 vicente    (501) staff       (20)     1144 2024-05-24 11:43:12.000000 pyanfis-0.1.4/src/pyanfis.egg-info/SOURCES.txt
+-rw-r--r--   0 vicente    (501) staff       (20)        1 2024-05-24 11:43:12.000000 pyanfis-0.1.4/src/pyanfis.egg-info/dependency_links.txt
+-rw-r--r--   0 vicente    (501) staff       (20)        8 2024-05-24 11:43:12.000000 pyanfis-0.1.4/src/pyanfis.egg-info/top_level.txt
```

### Comparing `pyanfis-0.1.3/LICENSE` & `pyanfis-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/PKG-INFO` & `pyanfis-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanfis
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pytorch-based package to use ANFIS for AI
 Author-email: Vicente Feced Mas <vicente.feced.mas@gmail.com>
 Project-URL: Homepage, https://github.com/VicenteFecedMas/pyanfis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyanfis-0.1.3/README.md` & `pyanfis-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/algorithms/LSTSQ.py` & `pyanfis-0.1.4/src/pyanfis/algorithms/LSTSQ.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/algorithms/RLSE.py` & `pyanfis-0.1.4/src/pyanfis/algorithms/RLSE.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/anfis.py` & `pyanfis-0.1.4/src/pyanfis/anfis.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/antecedents/antecedents.py` & `pyanfis-0.1.4/src/pyanfis/antecedents/antecedents.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/consequents/consequents.py` & `pyanfis-0.1.4/src/pyanfis/consequents/consequents.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/consequents/types/algorithm.py` & `pyanfis-0.1.4/src/pyanfis/consequents/types/algorithm.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/consequents/types/lee.py` & `pyanfis-0.1.4/src/pyanfis/consequents/types/lee.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/consequents/types/takagi_sugeno.py` & `pyanfis-0.1.4/src/pyanfis/consequents/types/takagi_sugeno.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/consequents/types/tsukamoto.py` & `pyanfis-0.1.4/src/pyanfis/consequents/types/tsukamoto.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/functions/bell.py` & `pyanfis-0.1.4/src/pyanfis/functions/bell.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/functions/gauss.py` & `pyanfis-0.1.4/src/pyanfis/functions/gauss.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,32 +17,32 @@
     torch.tensor
         a tensor of equal size to the input tensor
     """
     def __init__(self, mean:float = None, std:float = None) -> None:
         super().__init__()
         
         
-        if not isinstance(std, float) and not isinstance(std, None):
-            raise ValueError(f"Expected std to be a float number but got {type(std)} instead")
-        elif std <= 0.0:
-            raise ValueError(f"std value must be greater than 0.0 but got {std}")
+        #if not std and not isinstance(std, float):
+        #    raise ValueError(f"Expected std to be a float number but got {type(std)} instead")
+        #elif std <= 0.0:
+        #    raise ValueError(f"std value must be greater than 0.0 but got {std}")
     
-        if not isinstance(mean, float) and not isinstance(mean, None):
-            raise ValueError(f"Expected mean to be a float number but got {type(std)} instead")
+        #if not mean and not isinstance(mean, float):
+        #    raise ValueError(f"Expected mean to be a float number but got {type(std)} instead")
         
         self.mean = init_parameter(mean)
         self.std = init_parameter(std)
     
     def get_center(self) -> torch.Tensor:
         return self.mean
     
     def forward(self, x) -> torch.Tensor:
-        if not isinstance(self.mean, None):
-            raise RuntimeError(r"Expected mean to be a number but got None")
-        if not isinstance(self.std, None):
-            raise RuntimeError(r"Expected std to have a number but got None")
+        #if not self.mean:
+        #    raise RuntimeError(r"Expected mean to be a number but got None")
+        #if not self.std:
+        #    raise RuntimeError(r"Expected std to have a number but got None")
         
         x = x - self.mean
         x = (x)** 2
         x = -(x)/ (2 * (self.std ** 2))
         x = torch.exp(x)
         return x
```

### Comparing `pyanfis-0.1.3/src/pyanfis/functions/heaviside.py` & `pyanfis-0.1.4/src/pyanfis/functions/heaviside.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/functions/linear_s.py` & `pyanfis-0.1.4/src/pyanfis/functions/linear_s.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/functions/linear_z.py` & `pyanfis-0.1.4/src/pyanfis/functions/linear_z.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/functions/sigmoid.py` & `pyanfis-0.1.4/src/pyanfis/functions/sigmoid.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/functions/universe.py` & `pyanfis-0.1.4/src/pyanfis/functions/universe.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/optimizers/fuzzySGD.py` & `pyanfis-0.1.4/src/pyanfis/optimizers/fuzzySGD.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/rules/intersection_algorithms.py` & `pyanfis-0.1.4/src/pyanfis/rules/intersection_algorithms.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/rules/relation_algorithms.py` & `pyanfis-0.1.4/src/pyanfis/rules/relation_algorithms.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis/rules/rules.py` & `pyanfis-0.1.4/src/pyanfis/rules/rules.py`

 * *Files identical despite different names*

### Comparing `pyanfis-0.1.3/src/pyanfis.egg-info/PKG-INFO` & `pyanfis-0.1.4/src/pyanfis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanfis
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pytorch-based package to use ANFIS for AI
 Author-email: Vicente Feced Mas <vicente.feced.mas@gmail.com>
 Project-URL: Homepage, https://github.com/VicenteFecedMas/pyanfis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `pyanfis-0.1.3/src/pyanfis.egg-info/SOURCES.txt` & `pyanfis-0.1.4/src/pyanfis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

