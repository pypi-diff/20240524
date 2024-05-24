# Comparing `tmp/samar-0.0.2.tar.gz` & `tmp/samar-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samar-0.0.2.tar", max compression
+gzip compressed data, was "samar-0.0.3.tar", max compression
```

## Comparing `samar-0.0.2.tar` & `samar-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-12-09 16:03:34.747571 samar-0.0.2/LICENSE
--rw-r--r--   0        0        0      868 2023-12-09 16:03:34.747571 samar-0.0.2/README.md
--rw-r--r--   0        0        0     1353 2023-12-09 16:03:34.747571 samar-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-09 16:03:34.747571 samar-0.0.2/samar/__init__.py
--rw-r--r--   0        0        0     1841 2023-12-09 16:03:34.747571 samar-0.0.2/samar/analyse.py
--rw-r--r--   0        0        0     4602 2023-12-09 16:03:34.747571 samar-0.0.2/samar/compute.py
--rw-r--r--   0        0        0      570 2023-12-09 16:03:34.747571 samar-0.0.2/samar/config.yaml
--rw-r--r--   0        0        0      726 2023-12-09 16:03:34.747571 samar-0.0.2/samar/draw.py
--rw-r--r--   0        0        0     2523 2023-12-09 16:03:34.747571 samar-0.0.2/samar/util.py
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 samar-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-24 13:41:10.455828 samar-0.0.3/LICENSE
+-rw-r--r--   0        0        0      922 2024-05-24 13:41:10.455828 samar-0.0.3/README.md
+-rw-r--r--   0        0        0     1367 2024-05-24 13:41:10.455828 samar-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-24 13:41:10.455828 samar-0.0.3/samar/__init__.py
+-rw-r--r--   0        0        0     3281 2024-05-24 13:41:10.455828 samar-0.0.3/samar/analyse.py
+-rw-r--r--   0        0        0     6562 2024-05-24 13:41:10.455828 samar-0.0.3/samar/compute.py
+-rw-r--r--   0        0        0      940 2024-05-24 13:41:10.455828 samar-0.0.3/samar/config.yaml
+-rw-r--r--   0        0        0      726 2024-05-24 13:41:10.455828 samar-0.0.3/samar/draw.py
+-rw-r--r--   0        0        0     2877 2024-05-24 13:41:10.455828 samar-0.0.3/samar/util.py
+-rw-r--r--   0        0        0     1665 1970-01-01 00:00:00.000000 samar-0.0.3/PKG-INFO
```

### Comparing `samar-0.0.2/LICENSE` & `samar-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `samar-0.0.2/README.md` & `samar-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 ## Features
 
 - ✅ Straight forward from **.xlsx file** to **charts and tables**.
 - ✅ Robust comparison and prediction of multiple methods.
 - ✅ Feature importance analysis with RandomForest.
 - ✅ Robust comparison in independent verification dataset.
+- ✅ Both support classification and regression task.
 
 
 ## Quick start
 
 1. Install the samar via pip.
 
 ```sh
 pip install samar
 ```
 
 2. Use samar like [examples.py](https://github.com/LMH0066/samar/blob/main/examples.py)
 
 Once the package is installed, the main ways of use are in examples.py.
-
```

### Comparing `samar-0.0.2/pyproject.toml` & `samar-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "samar"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Minghong Li <lmh0066@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9 <3.12"
 scikit-learn = "^1.3.2"
-fancyimpute = "^0.7.0"
 matplotlib = "^3.8.2"
-pandas = "^2.1.3"
+pandas = ">=1.1.5"
 openpyxl = "^3.1.2"
-seaborn = "^0.13.0"
+seaborn = ">=0.12.2"
 pyyaml = "^6.0.1"
+shap = ">=0.42.1"
+xlrd = ">=2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.1.0"
 black = "^23.11.0"
 flake8-black = "^0.3.6"
 isort = "^5.12.0"
 flake8-isort = "^6.1.1"
```

### Comparing `samar-0.0.2/samar/draw.py` & `samar-0.0.3/samar/draw.py`

 * *Files identical despite different names*

### Comparing `samar-0.0.2/samar/util.py` & `samar-0.0.3/samar/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import importlib
+import inspect
 import os
+from typing import Tuple
 
 import numpy as np
 import pandas as pd
 import yaml
-from fancyimpute import KNN
+from sklearn.impute import KNNImputer
 
 """
 config.yaml related code
 """
 
 
 def load_config(path: str) -> dict:
@@ -18,36 +20,47 @@
 DEFAULT_CONFIG = load_config(os.path.join(os.path.dirname(__file__), "config.yaml"))
 
 
 def get_funcs_name(funcs: dict):
     return funcs.keys()
 
 
-def get_clf(funcs, func_name, random_state):
+def get_clf(funcs: dict, func_name: str, task: str, random_state: int):
     def _import(class_path: str):
         module_name, class_name = class_path.rsplit(".", 1)
         return getattr(importlib.import_module(module_name), class_name)
 
-    func = funcs[func_name]
-    return _import(func["class_path"])(**func["kwargs"], random_state=random_state)
+    def _filter_args(obj, args):
+        accepted_args = inspect.signature(obj).parameters
+        filtered_args = {
+            key: value for key, value in args.items() if key in accepted_args
+        }
+        return filtered_args
+
+    func = funcs[func_name].copy()
+    func["kwargs"].update(dict(random_state=random_state))
+
+    obj = _import(func["class_path"][task])
+    args = _filter_args(obj, func["kwargs"])
+    return obj(**args)
 
 
 """
 compute related code
 """
 
 
 def load_xlsx(
     path: str, preprocess_func: str, result_col: str = "efficacy evaluation"
-) -> (np.array, np.array, pd.DataFrame):
+) -> Tuple[np.array, np.array, pd.DataFrame]:
     data = pd.read_excel(path, index_col=0, header=[0])
 
     data = data.dropna(subset=[result_col])
     y = data[result_col].copy()
-    data = data.drop(["efficacy evaluation"], axis=1)
+    data = data.drop([result_col], axis=1)
 
     filter_data = Preprocess().do(data, preprocess_func)
     X = np.array(filter_data)
     y = np.array(y[filter_data.index])
     return X, y, filter_data
 
 
@@ -76,22 +89,22 @@
 
         filter_data = filter_data.dropna()
         return filter_data
 
     def KNN(self, data: pd.DataFrame) -> pd.DataFrame:
         filter_data = data.copy()
 
-        filled_data = KNN(k=10).fit_transform(filter_data)
+        filled_data = KNNImputer(n_neighbors=10).fit_transform(filter_data)
         filter_data[:] = filled_data
 
         return filter_data
 
 
-def write_stable_test_result(path: str, accs: dict, rocs: dict):
+def write_stable_test_result(path: str, scores: dict):
     if not path.endswith(".npy"):
         path += ".npy"
-    np.save(path, {"accs": accs, "rocs": rocs})
+    np.save(path, scores)
 
 
-def read_stable_test_result(path: str) -> (dict, dict):
-    result = np.load(path, allow_pickle=True).item()
-    return result["accs"], result["rocs"]
+def read_stable_test_result(path: str) -> dict:
+    scores = np.load(path, allow_pickle=True).item()
+    return scores
```

### Comparing `samar-0.0.2/PKG-INFO` & `samar-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: samar
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: MIT
 Author: Minghong Li
 Author-email: lmh0066@outlook.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fancyimpute (>=0.7.0,<0.8.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
-Requires-Dist: pandas (>=2.1.3,<3.0.0)
+Requires-Dist: pandas (>=1.1.5)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
-Requires-Dist: seaborn (>=0.13.0,<0.14.0)
+Requires-Dist: seaborn (>=0.12.2)
+Requires-Dist: shap (>=0.42.1)
+Requires-Dist: xlrd (>=2.0.1)
 Description-Content-Type: text/markdown
 
 # samar
 [![PyPI version](https://img.shields.io/pypi/pyversions/samar.svg)](https://pypi.org/project/samar/)
 [![PyPI version](https://img.shields.io/pypi/v/samar.svg)](https://pypi.org/project/samar/)
 [![PyPI version](https://img.shields.io/pypi/l/ansicolortags.svg)](https://github.com/LMH0066/samar/blob/main/LICENSE)
 
@@ -29,22 +30,22 @@
 
 ## Features
 
 - ✅ Straight forward from **.xlsx file** to **charts and tables**.
 - ✅ Robust comparison and prediction of multiple methods.
 - ✅ Feature importance analysis with RandomForest.
 - ✅ Robust comparison in independent verification dataset.
+- ✅ Both support classification and regression task.
 
 
 ## Quick start
 
 1. Install the samar via pip.
 
 ```sh
 pip install samar
 ```
 
 2. Use samar like [examples.py](https://github.com/LMH0066/samar/blob/main/examples.py)
 
 Once the package is installed, the main ways of use are in examples.py.
 
-
```

