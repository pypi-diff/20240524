# Comparing `tmp/array_api_compat-1.6.tar.gz` & `tmp/array_api_compat-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "array_api_compat-1.6.tar", last modified: Sat Mar 30 02:51:47 2024, max compression
+gzip compressed data, was "array_api_compat-1.7.tar", last modified: Fri May 24 20:33:44 2024, max compression
```

## Comparing `array_api_compat-1.6.tar` & `array_api_compat-1.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 02:51:47.947678 array_api_compat-1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-30 02:51:35.000000 array_api_compat-1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-30 02:51:47.947678 array_api_compat-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-30 02:51:35.000000 array_api_compat-1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 02:51:47.939678 array_api_compat-1.6/array_api_compat/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/_internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 02:51:47.943678 array_api_compat-1.6/array_api_compat/common/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/common/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/common/_fft.py
--rw-r--r--   0 runner    (1001) docker     (127)    16752 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/common/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/common/_linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/common/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 02:51:47.943678 array_api_compat-1.6/array_api_compat/cupy/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/cupy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/cupy/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/cupy/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/cupy/fft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/cupy/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 02:51:47.943678 array_api_compat-1.6/array_api_compat/dask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/dask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 02:51:47.943678 array_api_compat-1.6/array_api_compat/dask/array/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/dask/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/dask/array/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/dask/array/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 02:51:47.943678 array_api_compat-1.6/array_api_compat/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/numpy/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/numpy/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/numpy/fft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/numpy/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 02:51:47.943678 array_api_compat-1.6/array_api_compat/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27220 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/torch/_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/torch/fft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-03-30 02:51:35.000000 array_api_compat-1.6/array_api_compat/torch/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 02:51:47.947678 array_api_compat-1.6/array_api_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-30 02:51:47.000000 array_api_compat-1.6/array_api_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-30 02:51:47.000000 array_api_compat-1.6/array_api_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 02:51:47.000000 array_api_compat-1.6/array_api_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-30 02:51:47.000000 array_api_compat-1.6/array_api_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-30 02:51:47.000000 array_api_compat-1.6/array_api_compat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 02:51:47.947678 array_api_compat-1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-30 02:51:35.000000 array_api_compat-1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 02:51:47.947678 array_api_compat-1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-30 02:51:35.000000 array_api_compat-1.6/tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-03-30 02:51:35.000000 array_api_compat-1.6/tests/test_array_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-03-30 02:51:35.000000 array_api_compat-1.6/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-03-30 02:51:35.000000 array_api_compat-1.6/tests/test_isdtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-30 02:51:35.000000 array_api_compat-1.6/tests/test_no_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-03-30 02:51:35.000000 array_api_compat-1.6/tests/test_vendoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.251219 array_api_compat-1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-24 20:33:33.000000 array_api_compat-1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-24 20:33:44.251219 array_api_compat-1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-24 20:33:33.000000 array_api_compat-1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.243219 array_api_compat-1.7/array_api_compat/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/_internal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.243219 array_api_compat-1.7/array_api_compat/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14199 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/_fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19149 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/common/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat/cupy/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/cupy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/cupy/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/cupy/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/cupy/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/cupy/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat/dask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/dask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat/dask/array/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/dask/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/dask/array/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/dask/array/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/numpy/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/numpy/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/numpy/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/numpy/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27220 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/torch/_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/torch/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-24 20:33:33.000000 array_api_compat-1.7/array_api_compat/torch/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/array_api_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-24 20:33:44.000000 array_api_compat-1.7/array_api_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-24 20:33:44.000000 array_api_compat-1.7/array_api_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:33:44.000000 array_api_compat-1.7/array_api_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-24 20:33:44.000000 array_api_compat-1.7/array_api_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 20:33:44.000000 array_api_compat-1.7/array_api_compat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 20:33:44.251219 array_api_compat-1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-24 20:33:33.000000 array_api_compat-1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:33:44.247219 array_api_compat-1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_array_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_isdtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_no_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-24 20:33:33.000000 array_api_compat-1.7/tests/test_vendoring.py
```

### Comparing `array_api_compat-1.6/LICENSE` & `array_api_compat-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/PKG-INFO` & `array_api_compat-1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: array_api_compat
-Version: 1.6
+Version: 1.7
 Summary: A wrapper around NumPy and other array libraries to make them compatible with the Array API standard
 Home-page: https://data-apis.org/array-api-compat/
 Author: Consortium for Python Data API Standards
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,17 +19,19 @@
 Requires-Dist: cupy; extra == "cupy"
 Provides-Extra: jax
 Requires-Dist: jax; extra == "jax"
 Provides-Extra: pytorch
 Requires-Dist: pytorch; extra == "pytorch"
 Provides-Extra: dask
 Requires-Dist: dask; extra == "dask"
+Provides-Extra: sprase
+Requires-Dist: sparse>=0.15.1; extra == "sprase"
 
 # Array API compatibility library
 
 This is a small wrapper around common array libraries that is compatible with
 the [Array API standard](https://data-apis.org/array-api/latest/). Currently,
-NumPy, CuPy, PyTorch, Dask, and JAX are supported. If you want support for other array
-libraries, or if you encounter any issues, please [open an
+NumPy, CuPy, PyTorch, Dask, JAX and `sparse` are supported. If you want support
+for other array libraries, or if you encounter any issues, please [open an
 issue](https://github.com/data-apis/array-api-compat/issues).
 
 See the documentation for more details https://data-apis.org/array-api-compat/
```

### Comparing `array_api_compat-1.6/array_api_compat/_internal.py` & `array_api_compat-1.7/array_api_compat/_internal.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/common/_aliases.py` & `array_api_compat-1.7/array_api_compat/common/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/common/_fft.py` & `array_api_compat-1.7/array_api_compat/common/_fft.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/common/_helpers.py` & `array_api_compat-1.7/array_api_compat/common/_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,28 @@
     from ._typing import Array, Device
 
 import sys
 import math
 import inspect
 import warnings
 
+def _is_jax_zero_gradient_array(x):
+    """Return True if `x` is a zero-gradient array.
+
+    These arrays are a design quirk of Jax that may one day be removed.
+    See https://github.com/google/jax/issues/20620.
+    """
+    if 'numpy' not in sys.modules or 'jax' not in sys.modules:
+        return False
+
+    import numpy as np
+    import jax
+
+    return isinstance(x, np.ndarray) and x.dtype == jax.float0
+
 def is_numpy_array(x):
     """
     Return True if `x` is a NumPy array.
 
     This function does not import NumPy if it has not already been imported
     and is therefore cheap to use.
 
@@ -32,23 +46,25 @@
 
     array_namespace
     is_array_api_obj
     is_cupy_array
     is_torch_array
     is_dask_array
     is_jax_array
+    is_pydata_sparse_array
     """
     # Avoid importing NumPy if it isn't already
     if 'numpy' not in sys.modules:
         return False
 
     import numpy as np
 
     # TODO: Should we reject ndarray subclasses?
-    return isinstance(x, (np.ndarray, np.generic))
+    return (isinstance(x, (np.ndarray, np.generic))
+            and not _is_jax_zero_gradient_array(x))
 
 def is_cupy_array(x):
     """
     Return True if `x` is a CuPy array.
 
     This function does not import CuPy if it has not already been imported
     and is therefore cheap to use.
@@ -60,14 +76,15 @@
 
     array_namespace
     is_array_api_obj
     is_numpy_array
     is_torch_array
     is_dask_array
     is_jax_array
+    is_pydata_sparse_array
     """
     # Avoid importing NumPy if it isn't already
     if 'cupy' not in sys.modules:
         return False
 
     import cupy as cp
 
@@ -86,14 +103,15 @@
 
     array_namespace
     is_array_api_obj
     is_numpy_array
     is_cupy_array
     is_dask_array
     is_jax_array
+    is_pydata_sparse_array
     """
     # Avoid importing torch if it isn't already
     if 'torch' not in sys.modules:
         return False
 
     import torch
 
@@ -112,14 +130,15 @@
 
     array_namespace
     is_array_api_obj
     is_numpy_array
     is_cupy_array
     is_torch_array
     is_jax_array
+    is_pydata_sparse_array
     """
     # Avoid importing dask if it isn't already
     if 'dask.array' not in sys.modules:
         return False
 
     import dask.array
 
@@ -138,22 +157,52 @@
 
     array_namespace
     is_array_api_obj
     is_numpy_array
     is_cupy_array
     is_torch_array
     is_dask_array
+    is_pydata_sparse_array
     """
     # Avoid importing jax if it isn't already
     if 'jax' not in sys.modules:
         return False
 
     import jax
 
-    return isinstance(x, jax.Array)
+    return isinstance(x, jax.Array) or _is_jax_zero_gradient_array(x)
+
+
+def is_pydata_sparse_array(x) -> bool:
+    """
+    Return True if `x` is an array from the `sparse` package.
+
+    This function does not import `sparse` if it has not already been imported
+    and is therefore cheap to use.
+
+
+    See Also
+    --------
+
+    array_namespace
+    is_array_api_obj
+    is_numpy_array
+    is_cupy_array
+    is_torch_array
+    is_dask_array
+    is_jax_array
+    """
+    # Avoid importing jax if it isn't already
+    if 'sparse' not in sys.modules:
+        return False
+
+    import sparse
+
+    # TODO: Account for other backends.
+    return isinstance(x, sparse.SparseArray)
 
 def is_array_api_obj(x):
     """
     Return True if `x` is an array API compatible array object.
 
     See Also
     --------
@@ -166,14 +215,15 @@
     is_jax_array
     """
     return is_numpy_array(x) \
         or is_cupy_array(x) \
         or is_torch_array(x) \
         or is_dask_array(x) \
         or is_jax_array(x) \
+        or is_pydata_sparse_array(x) \
         or hasattr(x, '__array_namespace__')
 
 def _check_api_version(api_version):
     if api_version == '2021.12':
         warnings.warn("The 2021.12 version of the array API specification was requested but the returned namespace is actually version 2022.12")
     elif api_version is not None and api_version != '2022.12':
         raise ValueError("Only the 2022.12 version of the array API specification is currently supported")
@@ -234,14 +284,15 @@
 
     is_array_api_obj
     is_numpy_array
     is_cupy_array
     is_torch_array
     is_dask_array
     is_jax_array
+    is_pydata_sparse_array
 
     """
     if use_compat not in [None, True, False]:
         raise ValueError("use_compat must be None, True, or False")
 
     _use_compat = use_compat in [None, True]
 
@@ -293,14 +344,23 @@
             elif use_compat is False:
                 import jax.numpy as jnp
             else:
                 # jax.experimental.array_api is already an array namespace. We do
                 # not have a wrapper submodule for it.
                 import jax.experimental.array_api as jnp
             namespaces.add(jnp)
+        elif is_pydata_sparse_array(x):
+            if use_compat is True:
+                _check_api_version(api_version)
+                raise ValueError("`sparse` does not have an array-api-compat wrapper")
+            else:
+                import sparse
+            # `sparse` is already an array namespace. We do not have a wrapper
+            # submodule for it.
+            namespaces.add(sparse)
         elif hasattr(x, '__array_namespace__'):
             if use_compat is True:
                 raise ValueError("The given array does not have an array-api-compat wrapper")
             namespaces.add(x.__array_namespace__(api_version=api_version))
         else:
             # TODO: Support Python scalars?
             raise TypeError(f"{type(x).__name__} is not a supported array type")
@@ -387,16 +447,31 @@
         # can become a property, in accordance with the standard. In order for
         # this function to not break when JAX makes the flip, we check for
         # both here.
         if inspect.ismethod(x.device):
             return x.device()
         else:
             return x.device
+    elif is_pydata_sparse_array(x):
+        # `sparse` will gain `.device`, so check for this first.
+        x_device = getattr(x, 'device', None)
+        if x_device is not None:
+            return x_device
+        # Everything but DOK has this attr.
+        try:
+            inner = x.data
+        except AttributeError:
+            return "cpu"
+        # Return the device of the constituent array
+        return device(inner)
     return x.device
 
+# Prevent shadowing, used below
+_device = device
+
 # Based on cupy.array_api.Array.to_device
 def _cupy_to_device(x, device, /, stream=None):
     import cupy as cp
     from cupy.cuda import Device as _Device
     from cupy.cuda import stream as stream_module
     from cupy_backends.cuda.api import runtime
 
@@ -504,14 +579,18 @@
         if device == 'cpu':
             return x
         raise ValueError(f"Unsupported device {device!r}")
     elif is_jax_array(x):
         # This import adds to_device to x
         import jax.experimental.array_api # noqa: F401
         return x.to_device(device, stream=stream)
+    elif is_pydata_sparse_array(x) and device == _device(x):
+        # Perform trivial check to return the same array if
+        # device is same instead of err-ing.
+        return x
     return x.to_device(device, stream=stream)
 
 def size(x):
     """
     Return the total number of elements of x.
 
     This is equivalent to `x.size` according to the `standard
@@ -530,12 +609,13 @@
     "get_namespace",
     "is_array_api_obj",
     "is_cupy_array",
     "is_dask_array",
     "is_jax_array",
     "is_numpy_array",
     "is_torch_array",
+    "is_pydata_sparse_array",
     "size",
     "to_device",
 ]
 
 _all_ignore = ['sys', 'math', 'inspect', 'warnings']
```

### Comparing `array_api_compat-1.6/array_api_compat/common/_linalg.py` & `array_api_compat-1.7/array_api_compat/common/_linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/cupy/_aliases.py` & `array_api_compat-1.7/array_api_compat/cupy/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/cupy/_typing.py` & `array_api_compat-1.7/array_api_compat/cupy/_typing.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/cupy/fft.py` & `array_api_compat-1.7/array_api_compat/cupy/fft.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/cupy/linalg.py` & `array_api_compat-1.7/array_api_compat/cupy/linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/dask/array/_aliases.py` & `array_api_compat-1.7/array_api_compat/dask/array/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/dask/array/linalg.py` & `array_api_compat-1.7/array_api_compat/dask/array/linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/numpy/__init__.py` & `array_api_compat-1.7/array_api_compat/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/numpy/_aliases.py` & `array_api_compat-1.7/array_api_compat/numpy/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/numpy/_typing.py` & `array_api_compat-1.7/array_api_compat/numpy/_typing.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/numpy/fft.py` & `array_api_compat-1.7/array_api_compat/numpy/fft.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/numpy/linalg.py` & `array_api_compat-1.7/array_api_compat/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/torch/__init__.py` & `array_api_compat-1.7/array_api_compat/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/torch/_aliases.py` & `array_api_compat-1.7/array_api_compat/torch/_aliases.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/torch/fft.py` & `array_api_compat-1.7/array_api_compat/torch/fft.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/array_api_compat/torch/linalg.py` & `array_api_compat-1.7/array_api_compat/torch/linalg.py`

 * *Files 24% similar despite different names*

```diff
@@ -56,14 +56,30 @@
 
         res = x1_[..., None, :] @ x2_[..., None]
         return res[..., 0, 0]
     return torch.linalg.vecdot(x1, x2, dim=axis, **kwargs)
 
 def solve(x1: array, x2: array, /, **kwargs) -> array:
     x1, x2 = _fix_promotion(x1, x2, only_scalar=False)
+    # Torch tries to emulate NumPy 1 solve behavior by using batched 1-D solve
+    # whenever
+    # 1. x1.ndim - 1 == x2.ndim
+    # 2. x1.shape[:-1] == x2.shape
+    #
+    # See linalg_solve_is_vector_rhs in
+    # aten/src/ATen/native/LinearAlgebraUtils.h and
+    # TORCH_META_FUNC(_linalg_solve_ex) in
+    # aten/src/ATen/native/BatchLinearAlgebra.cpp in the PyTorch source code.
+    #
+    # The easiest way to work around this is to prepend a size 1 dimension to
+    # x2, since x2 is already one dimension less than x1.
+    #
+    # See https://github.com/pytorch/pytorch/issues/52915
+    if x2.ndim != 1 and x1.ndim - 1 == x2.ndim and x1.shape[:-1] == x2.shape:
+        x2 = x2[None]
     return torch.linalg.solve(x1, x2, **kwargs)
 
 # torch.trace doesn't support the offset argument and doesn't support stacking
 def trace(x: array, /, *, offset: int = 0, dtype: Optional[Dtype] = None) -> array:
     # Use our wrapped sum to make sure it does upcasting correctly
     return sum(torch.diagonal(x, offset=offset, dim1=-2, dim2=-1), axis=-1, dtype=dtype)
 
@@ -74,15 +90,31 @@
     axis: Optional[Union[int, Tuple[int, ...]]] = None,
     keepdims: bool = False,
     ord: Union[int, float, Literal[inf, -inf]] = 2,
     **kwargs,
 ) -> array:
     # torch.vector_norm incorrectly treats axis=() the same as axis=None
     if axis == ():
-        keepdims = True
+        out = kwargs.get('out')
+        if out is None:
+            dtype = None
+            if x.dtype == torch.complex64:
+                dtype = torch.float32
+            elif x.dtype == torch.complex128:
+                dtype = torch.float64
+
+            out = torch.zeros_like(x, dtype=dtype)
+
+        # The norm of a single scalar works out to abs(x) in every case except
+        # for ord=0, which is x != 0.
+        if ord == 0:
+            out[:] = (x != 0)
+        else:
+            out[:] = torch.abs(x)
+        return out
     return torch.linalg.vector_norm(x, ord=ord, axis=axis, keepdim=keepdims, **kwargs)
 
 __all__ = linalg_all + ['outer', 'matmul', 'matrix_transpose', 'tensordot',
                         'cross', 'vecdot', 'solve', 'trace', 'vector_norm']
 
 _all_ignore = ['torch_linalg', 'sum']
```

### Comparing `array_api_compat-1.6/array_api_compat.egg-info/PKG-INFO` & `array_api_compat-1.7/array_api_compat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: array_api_compat
-Version: 1.6
+Version: 1.7
 Summary: A wrapper around NumPy and other array libraries to make them compatible with the Array API standard
 Home-page: https://data-apis.org/array-api-compat/
 Author: Consortium for Python Data API Standards
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,17 +19,19 @@
 Requires-Dist: cupy; extra == "cupy"
 Provides-Extra: jax
 Requires-Dist: jax; extra == "jax"
 Provides-Extra: pytorch
 Requires-Dist: pytorch; extra == "pytorch"
 Provides-Extra: dask
 Requires-Dist: dask; extra == "dask"
+Provides-Extra: sprase
+Requires-Dist: sparse>=0.15.1; extra == "sprase"
 
 # Array API compatibility library
 
 This is a small wrapper around common array libraries that is compatible with
 the [Array API standard](https://data-apis.org/array-api/latest/). Currently,
-NumPy, CuPy, PyTorch, Dask, and JAX are supported. If you want support for other array
-libraries, or if you encounter any issues, please [open an
+NumPy, CuPy, PyTorch, Dask, JAX and `sparse` are supported. If you want support
+for other array libraries, or if you encounter any issues, please [open an
 issue](https://github.com/data-apis/array-api-compat/issues).
 
 See the documentation for more details https://data-apis.org/array-api-compat/
```

### Comparing `array_api_compat-1.6/array_api_compat.egg-info/SOURCES.txt` & `array_api_compat-1.7/array_api_compat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/setup.py` & `array_api_compat-1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     license="MIT",
     extras_require={
         "numpy": "numpy",
         "cupy": "cupy",
         "jax": "jax",
         "pytorch": "pytorch",
         "dask": "dask",
+        "sprase": "sparse >=0.15.1",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
```

### Comparing `array_api_compat-1.6/tests/test_all.py` & `array_api_compat-1.7/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/tests/test_array_namespace.py` & `array_api_compat-1.7/tests/test_array_namespace.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import subprocess
 import sys
 import warnings
 
+import jax
 import numpy as np
 import pytest
 import torch
 
 import array_api_compat
 from array_api_compat import array_namespace
 
@@ -14,15 +15,15 @@
 @pytest.mark.parametrize("use_compat", [True, False, None])
 @pytest.mark.parametrize("api_version", [None, "2021.12", "2022.12"])
 @pytest.mark.parametrize("library", all_libraries + ['array_api_strict'])
 def test_array_namespace(library, api_version, use_compat):
     xp = import_(library)
 
     array = xp.asarray([1.0, 2.0, 3.0])
-    if use_compat is True and library in ['array_api_strict', 'jax.numpy']:
+    if use_compat is True and library in {'array_api_strict', 'jax.numpy', 'sparse'}:
         pytest.raises(ValueError, lambda: array_namespace(array, use_compat=use_compat))
         return
     namespace = array_api_compat.array_namespace(array, api_version=api_version, use_compat=use_compat)
 
     if use_compat is False or use_compat is None and library not in wrapped_libraries:
         if library == "jax.numpy" and use_compat is None:
             import jax.experimental.array_api
@@ -51,14 +52,20 @@
 namespace = array_api_compat.array_namespace(array, api_version={api_version!r})
 
 import jax.experimental.array_api
 assert namespace == jax.experimental.array_api
 """
         subprocess.run([sys.executable, "-c", code], check=True)
 
+def test_jax_zero_gradient():
+    jx = jax.numpy.arange(4)
+    jax_zero = jax.vmap(jax.grad(jax.numpy.float32, allow_int=True))(jx)
+    assert (array_api_compat.get_namespace(jax_zero) is
+            array_api_compat.get_namespace(jx))
+
 def test_array_namespace_errors():
     pytest.raises(TypeError, lambda: array_namespace([1]))
     pytest.raises(TypeError, lambda: array_namespace())
 
     x = np.asarray([1, 2])
     pytest.raises(TypeError, lambda: array_namespace((x, x)))
     pytest.raises(TypeError, lambda: array_namespace(x, (x, x)))
```

### Comparing `array_api_compat-1.6/tests/test_common.py` & `array_api_compat-1.7/tests/test_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from array_api_compat import (is_numpy_array, is_cupy_array, is_torch_array, # noqa: F401
-                              is_dask_array, is_jax_array)
+                              is_dask_array, is_jax_array, is_pydata_sparse_array)
 
 from array_api_compat import is_array_api_obj, device, to_device
 
 from ._helpers import import_, wrapped_libraries, all_libraries
 
 import pytest
 import numpy as np
@@ -12,14 +12,15 @@
 
 is_functions = {
     'numpy': 'is_numpy_array',
     'cupy': 'is_cupy_array',
     'torch': 'is_torch_array',
     'dask.array': 'is_dask_array',
     'jax.numpy': 'is_jax_array',
+    'sparse': 'is_pydata_sparse_array',
 }
 
 @pytest.mark.parametrize('library', is_functions.keys())
 @pytest.mark.parametrize('func', is_functions.values())
 def test_is_xp_array(library, func):
     lib = import_(library)
     is_func = globals()[func]
@@ -72,14 +73,16 @@
 
         # TODO: remove xfail once
         # https://github.com/dask/dask/issues/8260 is resolved
         request.node.add_marker(pytest.mark.xfail(reason="Bug in dask raising error on conversion"))
     if source_library == "cupy" and target_library != "cupy":
         # cupy explicitly disallows implicit conversions to CPU
         pytest.skip(reason="cupy does not support implicit conversion to CPU")
+    elif source_library == "sparse" and target_library != "sparse":
+        pytest.skip(reason="`sparse` does not allow implicit densification")
     src_lib = import_(source_library, wrapper=True)
     tgt_lib = import_(target_library, wrapper=True)
     is_tgt_type = globals()[is_functions[target_library]]
 
     a = src_lib.asarray([1, 2, 3])
     b = tgt_lib.asarray(a)
```

### Comparing `array_api_compat-1.6/tests/test_isdtype.py` & `array_api_compat-1.7/tests/test_isdtype.py`

 * *Files identical despite different names*

### Comparing `array_api_compat-1.6/tests/test_no_dependencies.py` & `array_api_compat-1.7/tests/test_no_dependencies.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     import array_api_compat
     assert mod not in sys.modules
 
     a = Array()
 
     # array-api-strict is an example of an array API library that isn't
     # wrapped by array-api-compat.
-    if "strict" not in mod:
+    if "strict" not in mod and mod != "sparse":
         is_mod_array = getattr(array_api_compat, f"is_{mod.split('.')[0]}_array")
         assert not is_mod_array(a)
         assert mod not in sys.modules
 
     is_array_api_obj = getattr(array_api_compat, "is_array_api_obj")
     assert is_array_api_obj(a)
     assert mod not in sys.modules
@@ -46,15 +46,15 @@
     array_namespace(Array())
     assert mod not in sys.modules
 
 # TODO: Test that wrapper for library X doesn't depend on wrappers for library
 # Y (except most array libraries actually do themselves depend on numpy).
 
 @pytest.mark.parametrize("library", ["cupy", "numpy", "torch", "dask.array",
-                                     "jax.numpy", "array_api_strict"])
+                                     "jax.numpy", "sparse", "array_api_strict"])
 def test_numpy_dependency(library):
     # This import is here because it imports numpy
     from ._helpers import import_
 
     # This unfortunately won't go through any of the pytest machinery. We
     # reraise the exception as an AssertionError so that pytest will show it
     # in a semi-reasonable way
```

