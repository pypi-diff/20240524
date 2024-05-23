# Comparing `tmp/neuroweave-0.0.6.tar.gz` & `tmp/neuroweave-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroweave-0.0.6.tar", last modified: Thu May 23 18:15:23 2024, max compression
+gzip compressed data, was "neuroweave-0.0.7.tar", last modified: Thu May 23 20:26:40 2024, max compression
```

## Comparing `neuroweave-0.0.6.tar` & `neuroweave-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.688299 neuroweave-0.0.6/
--rw-rw-rw-   0        0        0     1088 2024-04-25 14:13:00.000000 neuroweave-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5677 2024-05-23 18:15:23.687299 neuroweave-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4339 2024-05-23 11:36:09.000000 neuroweave-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.686298 neuroweave-0.0.6/neuroweave.egg-info/
--rw-rw-rw-   0        0        0     5677 2024-05-23 18:15:23.000000 neuroweave-0.0.6/neuroweave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2024-05-23 18:15:23.000000 neuroweave-0.0.6/neuroweave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 18:15:23.000000 neuroweave-0.0.6/neuroweave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2024-05-23 18:15:23.000000 neuroweave-0.0.6/neuroweave.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-23 18:15:23.000000 neuroweave-0.0.6/neuroweave.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 18:15:23.688299 neuroweave-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1785 2024-05-23 18:15:17.000000 neuroweave-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.675783 neuroweave-0.0.6/weave/
--rw-rw-rw-   0        0        0      896 2024-05-23 11:36:09.000000 neuroweave-0.0.6/weave/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.676783 neuroweave-0.0.6/weave/_utils/
--rw-rw-rw-   0        0        0       42 2024-05-23 06:31:49.000000 neuroweave-0.0.6/weave/_utils/__init__.py
--rw-rw-rw-   0        0        0     4941 2024-05-23 06:32:37.000000 neuroweave-0.0.6/weave/_utils/core.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.677782 neuroweave-0.0.6/weave/cuda/
--rw-rw-rw-   0        0        0     1839 2024-05-23 06:31:49.000000 neuroweave-0.0.6/weave/cuda/__init__.py
--rw-rw-rw-   0        0        0     5708 2024-05-23 11:36:09.000000 neuroweave-0.0.6/weave/cuda/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.678785 neuroweave-0.0.6/weave/neuro_dataset/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.6/weave/neuro_dataset/__init__.py
--rw-rw-rw-   0        0        0    23302 2024-05-23 18:06:55.000000 neuroweave-0.0.6/weave/neuro_dataset/main.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.679783 neuroweave-0.0.6/weave/neuro_functions/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.6/weave/neuro_functions/__init__.py
--rw-rw-rw-   0        0        0    28120 2024-05-23 11:30:14.000000 neuroweave-0.0.6/weave/neuro_functions/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.681295 neuroweave-0.0.6/weave/neuro_storage/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.6/weave/neuro_storage/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-05-23 06:32:37.000000 neuroweave-0.0.6/weave/neuro_storage/loader.py
--rw-rw-rw-   0        0        0     2795 2024-05-23 06:32:37.000000 neuroweave-0.0.6/weave/neuro_storage/saver.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.681295 neuroweave-0.0.6/weave/nn/
--rw-rw-rw-   0        0        0       46 2024-05-23 06:31:49.000000 neuroweave-0.0.6/weave/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.684299 neuroweave-0.0.6/weave/nn/modules/
--rw-rw-rw-   0        0        0      239 2024-05-23 06:31:49.000000 neuroweave-0.0.6/weave/nn/modules/__init__.py
--rw-rw-rw-   0        0        0    10512 2024-05-23 11:30:14.000000 neuroweave-0.0.6/weave/nn/modules/activations.py
--rw-rw-rw-   0        0        0     3392 2024-05-23 11:36:09.000000 neuroweave-0.0.6/weave/nn/modules/layer.py
--rw-rw-rw-   0        0        0     5209 2024-05-23 11:30:14.000000 neuroweave-0.0.6/weave/nn/modules/losses.py
--rw-rw-rw-   0        0        0     4637 2024-05-23 11:30:14.000000 neuroweave-0.0.6/weave/nn/modules/model.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.685299 neuroweave-0.0.6/weave/nn/optim/
--rw-rw-rw-   0        0        0       55 2024-05-23 06:31:49.000000 neuroweave-0.0.6/weave/nn/optim/__init__.py
--rw-rw-rw-   0        0        0     5637 2024-05-23 11:30:14.000000 neuroweave-0.0.6/weave/nn/optim/optimizers.py
--rw-rw-rw-   0        0        0    46181 2024-05-23 17:55:40.000000 neuroweave-0.0.6/weave/tensor.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:15:23.686298 neuroweave-0.0.6/weave/visualization/
--rw-rw-rw-   0        0        0       71 2024-05-23 06:31:49.000000 neuroweave-0.0.6/weave/visualization/__init__.py
--rw-rw-rw-   0        0        0     2003 2024-05-23 18:14:59.000000 neuroweave-0.0.6/weave/visualization/weave_weights.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.280876 neuroweave-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2024-04-25 14:13:00.000000 neuroweave-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5677 2024-05-23 20:26:40.279628 neuroweave-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4339 2024-05-23 11:36:09.000000 neuroweave-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.278281 neuroweave-0.0.7/neuroweave.egg-info/
+-rw-rw-rw-   0        0        0     5677 2024-05-23 20:26:40.000000 neuroweave-0.0.7/neuroweave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2024-05-23 20:26:40.000000 neuroweave-0.0.7/neuroweave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 20:26:40.000000 neuroweave-0.0.7/neuroweave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2024-05-23 20:26:40.000000 neuroweave-0.0.7/neuroweave.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-23 20:26:40.000000 neuroweave-0.0.7/neuroweave.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 20:26:40.280876 neuroweave-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1785 2024-05-23 20:26:06.000000 neuroweave-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.251433 neuroweave-0.0.7/weave/
+-rw-rw-rw-   0        0        0      896 2024-05-23 11:36:09.000000 neuroweave-0.0.7/weave/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.253877 neuroweave-0.0.7/weave/_utils/
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:31:49.000000 neuroweave-0.0.7/weave/_utils/__init__.py
+-rw-rw-rw-   0        0        0     5029 2024-05-23 20:12:45.000000 neuroweave-0.0.7/weave/_utils/core.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.255096 neuroweave-0.0.7/weave/cuda/
+-rw-rw-rw-   0        0        0     1839 2024-05-23 06:31:49.000000 neuroweave-0.0.7/weave/cuda/__init__.py
+-rw-rw-rw-   0        0        0     5708 2024-05-23 11:36:09.000000 neuroweave-0.0.7/weave/cuda/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.257561 neuroweave-0.0.7/weave/neuro_dataset/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.7/weave/neuro_dataset/__init__.py
+-rw-rw-rw-   0        0        0    23302 2024-05-23 18:06:55.000000 neuroweave-0.0.7/weave/neuro_dataset/main.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.259968 neuroweave-0.0.7/weave/neuro_functions/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.7/weave/neuro_functions/__init__.py
+-rw-rw-rw-   0        0        0    28120 2024-05-23 11:30:14.000000 neuroweave-0.0.7/weave/neuro_functions/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.263698 neuroweave-0.0.7/weave/neuro_storage/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.7/weave/neuro_storage/__init__.py
+-rw-rw-rw-   0        0        0     2381 2024-05-23 06:32:37.000000 neuroweave-0.0.7/weave/neuro_storage/loader.py
+-rw-rw-rw-   0        0        0     2795 2024-05-23 06:32:37.000000 neuroweave-0.0.7/weave/neuro_storage/saver.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.264941 neuroweave-0.0.7/weave/nn/
+-rw-rw-rw-   0        0        0       46 2024-05-23 06:31:49.000000 neuroweave-0.0.7/weave/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.271004 neuroweave-0.0.7/weave/nn/modules/
+-rw-rw-rw-   0        0        0      239 2024-05-23 06:31:49.000000 neuroweave-0.0.7/weave/nn/modules/__init__.py
+-rw-rw-rw-   0        0        0    10594 2024-05-23 20:04:58.000000 neuroweave-0.0.7/weave/nn/modules/activations.py
+-rw-rw-rw-   0        0        0     3392 2024-05-23 11:36:09.000000 neuroweave-0.0.7/weave/nn/modules/layer.py
+-rw-rw-rw-   0        0        0     5209 2024-05-23 11:30:14.000000 neuroweave-0.0.7/weave/nn/modules/losses.py
+-rw-rw-rw-   0        0        0     4637 2024-05-23 11:30:14.000000 neuroweave-0.0.7/weave/nn/modules/model.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.273441 neuroweave-0.0.7/weave/nn/optim/
+-rw-rw-rw-   0        0        0       55 2024-05-23 06:31:49.000000 neuroweave-0.0.7/weave/nn/optim/__init__.py
+-rw-rw-rw-   0        0        0     5637 2024-05-23 11:30:14.000000 neuroweave-0.0.7/weave/nn/optim/optimizers.py
+-rw-rw-rw-   0        0        0    46533 2024-05-23 20:09:22.000000 neuroweave-0.0.7/weave/tensor.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:26:40.275918 neuroweave-0.0.7/weave/visualization/
+-rw-rw-rw-   0        0        0       71 2024-05-23 06:31:49.000000 neuroweave-0.0.7/weave/visualization/__init__.py
+-rw-rw-rw-   0        0        0     2003 2024-05-23 18:14:59.000000 neuroweave-0.0.7/weave/visualization/weave_weights.py
```

### Comparing `neuroweave-0.0.6/LICENSE` & `neuroweave-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/PKG-INFO` & `neuroweave-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroweave
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small machine learning library.
 Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin, Patricia Pérez, Hugo Urbán
 Author-email: gabriellichu@gmail.com, info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com, hugourmaz@gmail.com
 Keywords: Python,Machine Learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neuroweave Version: 0.0.6 Summary: A small machine
+Metadata-Version: 2.1 Name: neuroweave Version: 0.0.7 Summary: A small machine
 learning library. Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin,
 Patricia PÃ©rez, Hugo UrbÃ¡n Author-email: gabriellichu@gmail.com,
 info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com,
 hugourmaz@gmail.com Keywords: Python,Machine Learning Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Microsoft :: Windows Classifier:
```

### Comparing `neuroweave-0.0.6/README.md` & `neuroweave-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/neuroweave.egg-info/PKG-INFO` & `neuroweave-0.0.7/neuroweave.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroweave
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small machine learning library.
 Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin, Patricia Pérez, Hugo Urbán
 Author-email: gabriellichu@gmail.com, info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com, hugourmaz@gmail.com
 Keywords: Python,Machine Learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neuroweave Version: 0.0.6 Summary: A small machine
+Metadata-Version: 2.1 Name: neuroweave Version: 0.0.7 Summary: A small machine
 learning library. Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin,
 Patricia PÃ©rez, Hugo UrbÃ¡n Author-email: gabriellichu@gmail.com,
 info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com,
 hugourmaz@gmail.com Keywords: Python,Machine Learning Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Microsoft :: Windows Classifier:
```

### Comparing `neuroweave-0.0.6/neuroweave.egg-info/SOURCES.txt` & `neuroweave-0.0.7/neuroweave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/setup.py` & `neuroweave-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as fh:
     long_description = fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'A small machine learning library.'
 LONG_DESCRIPTION = ('A Machine Learning library with the basic components necessary for building basic '
                     'Neural Network Models')
 
 setup(
     name='neuroweave',
     version=VERSION,
```

### Comparing `neuroweave-0.0.6/weave/__init__.py` & `neuroweave-0.0.7/weave/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/weave/_utils/core.py` & `neuroweave-0.0.7/weave/_utils/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,39 +44,42 @@
         the RAM with older, no more useful, variables.
     """
     this_global = globals()
 
     _iadd_hooks = 0
     _isub_hooks = 0
     _imul_hooks = 0
+    _idiv_hooks = 0
     _log_hooks = 0
     _softmax_hooks = 0
     _relu_hooks = 0
 
     @classmethod
     def create_hooks(cls, hook_tensor, op: str, alter: bool = False, other=None):
         match op:   # We select a base hook name based on the operation
             case '+':
                 name = '_iadd_hooks'
             case '-':
                 name = '_isub_hooks'
             case '*':
                 name = '_imul_hooks'
+            case '/':
+                name = '_idiv_hooks'
             case 'log':
                 name = '_log_hooks'
             case 'softmax':
                 name = '_softmax_hooks'
             case 'relu':
                 name = '_relu_hooks'
             case _:
                 raise ValueError('Unsupported hook.')
         globals()[f'{name}{getattr(cls, name)}'] = hook_tensor.copy()  # We store a copy of the tenor in the hook
         if alter:
             # We change the children of the 'hook_tensor' in case we are doing an immediate operation with grad enabled
-            if isinstance(other, (np.ndarray, list)) or issubclass(other, np.ndarray):
+            if isinstance(other, (np.ndarray, list)) or issubclass(type(other), np.ndarray):
                 hook_tensor._prev = {id(globals()[f'{name}{getattr(cls, name)}']), id(other)}
             else:
                 hook_tensor._prev = {globals()[f'{name}{getattr(cls, name)}']}
         setattr(cls, name, getattr(cls, name) + 1)
 
     @classmethod
     def delete_hooks(cls):
```

### Comparing `neuroweave-0.0.6/weave/cuda/__init__.py` & `neuroweave-0.0.7/weave/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/weave/cuda/tools.py` & `neuroweave-0.0.7/weave/cuda/tools.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/weave/neuro_dataset/main.py` & `neuroweave-0.0.7/weave/neuro_dataset/main.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/weave/neuro_functions/functions.py` & `neuroweave-0.0.7/weave/neuro_functions/functions.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/weave/neuro_storage/loader.py` & `neuroweave-0.0.7/weave/neuro_storage/loader.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/weave/neuro_storage/saver.py` & `neuroweave-0.0.7/weave/neuro_storage/saver.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/weave/nn/modules/activations.py` & `neuroweave-0.0.7/weave/nn/modules/activations.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,16 @@
         def _backward():
             out._grad_enabled = False
             if len(out.shape) > 1:
                 derivative = []
                 for i in range(out.shape[0]):
                     d = out.grad @ (diag(out[i].squeeze(), device=self.device) - outer(out[i], out[i],
                                                                                        device=self.device))
+                    if d.shape[0] == 1:
+                        d = d.squeeze()
                     derivative.append(d[i])
                 x.grad += vstack(tuple(derivative), device=self.device)
             else:
                 x.grad += out.grad @ (diag(out.squeeze(), device=self.device) - outer(out, out, device=self.device))
             out._grad_enabled = True
 
         if x.grad_enabled:
```

### Comparing `neuroweave-0.0.6/weave/nn/modules/layer.py` & `neuroweave-0.0.7/weave/nn/modules/layer.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/weave/nn/modules/losses.py` & `neuroweave-0.0.7/weave/nn/modules/losses.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/weave/nn/modules/model.py` & `neuroweave-0.0.7/weave/nn/modules/model.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/weave/nn/optim/optimizers.py` & `neuroweave-0.0.7/weave/nn/optim/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.6/weave/tensor.py` & `neuroweave-0.0.7/weave/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     def __neg__(self):
         return self * -1
 
     def __radd__(self, other: Any) -> "Tensor":
         return self + other
 
     def __iadd__(self, other: Any) -> "Tensor":
-        enable_grad = self._grad_enabled and other.grad_enabled
+        enable_grad = (self._grad_enabled and other.grad_enabled) if isinstance(other, Tensor) else self._grad_enabled
         out = self + other
         if enable_grad:
             HookManager.create_hooks(self, '+', alter=True, other=other)
         self._op = out._op
         self.grad = out.grad
         self.data = out.data
         self._populate(out.data)
@@ -159,15 +159,15 @@
     def __sub__(self, other: Any) -> "Tensor":
         return self + (-other)
 
     def __rsub__(self, other: Any) -> "Tensor":
         return (-self) + other
 
     def __isub__(self, other: Any) -> "Tensor":
-        enable_grad = self._grad_enabled and other.grad_enabled
+        enable_grad = (self._grad_enabled and other.grad_enabled) if isinstance(other, Tensor) else self._grad_enabled
         out = self + (-other)
         if enable_grad:
             HookManager.create_hooks(self, '-', alter=True, other=other)
         self._op = out._op
         self.grad = out.grad
         self._data = out.data
         self._populate(out.data)
@@ -211,15 +211,15 @@
             out._backward = _backward
         return out
 
     def __rmul__(self, other: Any) -> "Tensor":
         return self * other
 
     def __imul__(self, other: Any) -> "Tensor":
-        enable_grad = self._grad_enabled and other.grad_enabled
+        enable_grad = (self._grad_enabled and other.grad_enabled) if isinstance(other, Tensor) else self._grad_enabled
         out = self * other
         if enable_grad:
             HookManager.create_hooks(self, '*', alter=True, other=other)
         self._op = out._op
         self.grad = out.grad
         self.data = out.data
         self._populate(out.data)
@@ -328,20 +328,22 @@
             return other / self
         elif isinstance(other, (int, float)):
             return (self ** -1) * other
         else:
             raise TypeError(f"Cannot divide Tensor by object of type {type(other)}.")
 
     def __itruediv__(self, other: Any) -> "Tensor":
+        enable_grad = (self._grad_enabled and other.grad_enabled) if isinstance(other, Tensor) else self._grad_enabled
         out = self / other
+        if enable_grad:
+            HookManager.create_hooks(self, '/', alter=True, other=other)
+        self._op = out._op
         self.grad = out.grad
         self.data = out.data
         self._populate(out.data)
-        self._prev = out._prev
-        self._op = out._op
         return self
 
     def __floordiv__(self, other: Any) -> "Tensor":
         raise NotImplementedError("Floor division not implemented for tensors.")
 
     def __rfloordiv__(self, other: Any) -> "Tensor":
         raise NotImplementedError("Floor division not implemented for tensors.")
```

### Comparing `neuroweave-0.0.6/weave/visualization/weave_weights.py` & `neuroweave-0.0.7/weave/visualization/weave_weights.py`

 * *Files identical despite different names*

