# Comparing `tmp/naturalexperiments-0.0.7.tar.gz` & `tmp/naturalexperiments-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalexperiments-0.0.7.tar", last modified: Thu May 23 21:04:45 2024, max compression
+gzip compressed data, was "naturalexperiments-0.0.8.tar", last modified: Fri May 24 15:00:21 2024, max compression
```

## Comparing `naturalexperiments-0.0.7.tar` & `naturalexperiments-0.0.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.935469 naturalexperiments-0.0.7/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.7/LICENSE
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 21:04:45.935284 naturalexperiments-0.0.7/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.7/README.md
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.928974 naturalexperiments-0.0.7/naturalexperiments/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    11440 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/benchmark.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.929649 naturalexperiments-0.0.7/naturalexperiments/data/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      338 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/data/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.929853 naturalexperiments-0.0.7/naturalexperiments/data/acic/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.7/naturalexperiments/data/acic/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.930048 naturalexperiments-0.0.7/naturalexperiments/data/ihdp/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.7/naturalexperiments/data/ihdp/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.930236 naturalexperiments-0.0.7/naturalexperiments/data/jobs/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.7/naturalexperiments/data/jobs/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.930471 naturalexperiments-0.0.7/naturalexperiments/data/news/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.0.7/naturalexperiments/data/news/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.930917 naturalexperiments-0.0.7/naturalexperiments/data/rorco/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-23 21:01:42.000000 naturalexperiments-0.0.7/naturalexperiments/data/rorco/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.7/naturalexperiments/data/rorco/rorco_preprocess.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.931156 naturalexperiments-0.0.7/naturalexperiments/data/twins/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1810 2024-05-23 12:04:17.000000 naturalexperiments-0.0.7/naturalexperiments/data/twins/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     6139 2024-05-23 12:21:06.000000 naturalexperiments-0.0.7/naturalexperiments/data_summary.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.934793 naturalexperiments-0.0.7/naturalexperiments/estimators/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-23 17:30:11.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/catenet.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/direct_difference.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/direct_prediction.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/double_double.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/doubly_robust.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/horvitz_thompson.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/learned_direct.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/off_policy.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/propensity_stratification.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/regression_discontinuity.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/tmle.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     3551 2024-05-23 20:59:16.000000 naturalexperiments-0.0.7/naturalexperiments/model.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/utils.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.935100 naturalexperiments-0.0.7/naturalexperiments.egg-info/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 21:04:45.000000 naturalexperiments-0.0.7/naturalexperiments.egg-info/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-23 21:04:45.000000 naturalexperiments-0.0.7/naturalexperiments.egg-info/SOURCES.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-23 21:04:45.000000 naturalexperiments-0.0.7/naturalexperiments.egg-info/dependency_links.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-23 21:04:45.000000 naturalexperiments-0.0.7/naturalexperiments.egg-info/top_level.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-23 21:04:45.935510 naturalexperiments-0.0.7/setup.cfg
--rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-23 21:03:05.000000 naturalexperiments-0.0.7/setup.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.306275 naturalexperiments-0.0.8/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.8/LICENSE
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 15:00:21.306090 naturalexperiments-0.0.8/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.8/README.md
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.300422 naturalexperiments-0.0.8/naturalexperiments/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    12240 2024-05-24 14:54:01.000000 naturalexperiments-0.0.8/naturalexperiments/benchmark.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.301116 naturalexperiments-0.0.8/naturalexperiments/data/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      391 2024-05-24 13:38:10.000000 naturalexperiments-0.0.8/naturalexperiments/data/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.301380 naturalexperiments-0.0.8/naturalexperiments/data/acic/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.8/naturalexperiments/data/acic/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.301648 naturalexperiments-0.0.8/naturalexperiments/data/ihdp/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.8/naturalexperiments/data/ihdp/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.301886 naturalexperiments-0.0.8/naturalexperiments/data/jobs/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.8/naturalexperiments/data/jobs/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.302154 naturalexperiments-0.0.8/naturalexperiments/data/news/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.0.8/naturalexperiments/data/news/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.302698 naturalexperiments-0.0.8/naturalexperiments/data/rorco/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2253 2024-05-24 13:38:42.000000 naturalexperiments-0.0.8/naturalexperiments/data/rorco/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.8/naturalexperiments/data/rorco/rorco_preprocess.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.302963 naturalexperiments-0.0.8/naturalexperiments/data/twins/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1810 2024-05-23 12:04:17.000000 naturalexperiments-0.0.8/naturalexperiments/data/twins/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     6151 2024-05-24 13:47:10.000000 naturalexperiments-0.0.8/naturalexperiments/data_summary.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.305655 naturalexperiments-0.0.8/naturalexperiments/estimators/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-23 17:30:11.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/catenet.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/direct_difference.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/direct_prediction.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/double_double.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/doubly_robust.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/horvitz_thompson.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/learned_direct.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/off_policy.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/propensity_stratification.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/regression_discontinuity.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/tmle.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     3546 2024-05-24 13:44:37.000000 naturalexperiments-0.0.8/naturalexperiments/model.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2185 2024-05-24 13:19:39.000000 naturalexperiments-0.0.8/naturalexperiments/utils.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.305852 naturalexperiments-0.0.8/naturalexperiments.egg-info/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 15:00:21.000000 naturalexperiments-0.0.8/naturalexperiments.egg-info/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-24 15:00:21.000000 naturalexperiments-0.0.8/naturalexperiments.egg-info/SOURCES.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-24 15:00:21.000000 naturalexperiments-0.0.8/naturalexperiments.egg-info/dependency_links.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-24 15:00:21.000000 naturalexperiments-0.0.8/naturalexperiments.egg-info/top_level.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-24 15:00:21.306316 naturalexperiments-0.0.8/setup.cfg
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-24 14:59:57.000000 naturalexperiments-0.0.8/setup.py
```

### Comparing `naturalexperiments-0.0.7/LICENSE` & `naturalexperiments-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/PKG-INFO` & `naturalexperiments-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.7
+Version: 0.0.8
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.7/naturalexperiments/benchmark.py` & `naturalexperiments-0.0.8/naturalexperiments/benchmark.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from tqdm import tqdm
 import time
 from .model import estimate_propensity, train
 from .data import dataloaders
-from .utils import compute_cross_entropy, compute_distance_correlation
+from .utils import compute_cross_entropy, compute_distance_correlation, build_synthetic_outcomes, biased_treatment_effect, sigmoid
 import numpy as np
 import sklearn.preprocessing
 import pandas as pd
 from tabulate import tabulate
 import matplotlib.pyplot as plt
 
 # # # VARIANCE BENCHMARK TABLE # # #
@@ -107,122 +107,116 @@
     if save:
         plt.savefig(f'{folder}{figure_name}.pdf', dpi=500)
     if show:
         plt.show()
 
 # # # SYNTHETIC OUTCOMES # # #
 
-def biased_treatment_effect(x, scaling=1):
-    # No effect on first half
-    # Second half has effect of sqrt(x) * scaling
-    adjustment = .5 - np.sqrt(.5) * scaling
-    line = x * (x<.5).astype(int) + (x>=.5).astype(int) * (scaling * np.sqrt(x) + adjustment)
-    return line
-
-def sigmoid(x):
-    return 1 / (1 + np.exp(-x))
-
-# Build problem where treatment and outcome are correlated
-def build_synthetic_outcomes(X, scale=True):
-    if scale:
-        X = sklearn.preprocessing.StandardScaler().fit(X).transform(X)
-
-    b = np.random.normal(size=X.shape[1])
-    important_variable = X @ b
-    p = sigmoid(important_variable)
-    p = np.clip(p, 0.01, .99) # regularize
-
-    y = pd.DataFrame({
-        'y0' : 1-p,
-        'y1' : 1-biased_treatment_effect(p)
-    }, dtype=float)
-    return X, y, p
-
 def wrap_dataloader(dataset, num):
     if dataset == 'IHDP':
         X, y, z = dataloaders['IHDP'](num % 10 + 1)
     if dataset == 'NEWS':
         X, y, z = dataloaders['NEWS'](num % 50 + 1)
     else: # For datasets where outcomes only known for treatment or control but not both
         X, _, _ = dataloaders[dataset]()
         X, y, p = build_synthetic_outcomes(X)
         uniform = np.random.random_sample(X.shape[0])
         z = (uniform < p).astype(int)
     return X, y, z
 
 # # # VARIANCE BENCHMARK # # #
 
-def compute_variance(methods, dataset, num_runs=10, train_fn=train, variance=None, times=None):
-    if variance is None: 
-        variance = {method: [] for method in methods}
-        times = {method: [] for method in methods}
-
-    for method in methods:
-        if method not in variance:
-            variance[method] = []
-            times[method] = []    
+def subsample(X, y, z, n):
+    # Some methods are slow so we subsample
+    sample_indices = np.random.choice(X.shape[0], n, replace=False)
+    return X[sample_indices], y.iloc[sample_indices].reset_index(drop=True), z[sample_indices]
+
+def compute_estimates(methods, dataset, num_runs=10, train_fn=train, folder='', return_error=False, limit=5000):
+    if return_error:
+        filename = folder + f'/variance_{dataset}.csv'
+    else: 
+        filename = folder + f'/estimates_{dataset}.csv'
 
     for num in tqdm(range(num_runs)): 
         X, y, z = wrap_dataloader(dataset, num)
+        X, y, z = subsample(X, y, z, limit)
         p_estimated = estimate_propensity(X, z)
         true_effect = (y['y1'] - y['y0']).mean()
  
+        saved = {}
         for method, get_estimate in methods.items():
-            if len(variance[method]) < num_runs:
-                time_start = time.time()
-                estimate = get_estimate(X, y, z, p_estimated, train_fn)
-                square_difference = (estimate - true_effect)**2
-                run_time = time.time() - time_start            
-                variance[method].append(square_difference) 
-                times[method].append(run_time)
-                print(f'{method} variance: {square_difference} time: {run_time}')
-
-    return variance, times
-
-def compute_variance_by_n(methods, dataset, ns, num_runs=10, train_fn=train, variance=None):
-    if variance is None: 
-        variance = {}
-
-    for method in methods:
-        if method not in variance:
-            variance[method] = {n : [] for n in ns} 
-        for n in ns:
-            if n not in variance[method]:
-                variance[method][n] = []
+            time_start = time.time()
+            #estimate = get_estimate(X, y, z, p_estimated, train_fn)
+            estimate = np.random.uniform()
+            square_difference = (estimate - true_effect)**2
+            run_time = time.time() - time_start            
+            if return_error:
+                saved[method] = (square_difference, run_time)
+            else:
+                saved[method] = (estimate, run_time)
+        with open(filename, 'a') as f:
+            f.write(str(saved) + '\n')
+    
+    
+    output, times = {}, {}
+    with open(filename, 'r') as f:
+        saved = eval(f.readline())
+        for method in saved:
+            if method not in output:
+                output[method] = []
+                times[method] = []
+            output[method] += [saved[method][0]]
+            times[method] += [saved[method][1]]
+
+    return output, times
+
+def compute_variance(methods, dataset, num_runs=10, train_fn=train, folder='', limit=5000):
+    return compute_estimates(methods, dataset, num_runs=num_runs, train_fn=train_fn, folder=folder, return_error=True, limit=limit)
+
+def compute_variance_by_n(methods, dataset, ns, num_runs=10, train_fn=train, folder='', limit=5000):
+    filename = folder + f'/variance_by_n_{dataset}.csv'
 
     for num in tqdm(range(num_runs)): 
         for i, n in enumerate(ns):
             X, y, z = wrap_dataloader(dataset, num + i*len(ns))
-            sample_indices = np.random.choice(X.shape[0], n, replace=False)
-            X, y, z = X[sample_indices], y.iloc[sample_indices], z[sample_indices]
-            # Reset index for y
-            y = y.reset_index(drop=True)
+            X, y, z = subsample(X, y, z, n)
 
             p_estimated = estimate_propensity(X, z)
             true_effect = (y['y1'] - y['y0']).mean()
     
+            saved = {'n':n}
             for method, get_estimate in methods.items():
-                if len(variance[method][n]) < num_runs:
-                    estimate = get_estimate(X, y, z, p_estimated, train_fn)
-                    square_difference = (estimate - true_effect)**2
-                    variance[method][n].append(square_difference) 
-
-    return variance
-
-def compute_variance_by_entropy(methods, dataset, noise_levels=[0, .2, .3, .4, .5], increment=.1, num_runs=10, train_fn = train, variance=None):
-    if variance is None: 
-        variance = {}
-
-    for method in methods:
-        if method not in variance:
-            variance[method] = {}
+                #estimate = get_estimate(X, y, z, p_estimated, train_fn)
+                estimate = np.random.uniform()
+                square_difference = (estimate - true_effect)**2
+                saved[method] = square_difference
+            with open(filename, 'a') as f:
+                f.write(str(saved) + '\n')
+    
+    output = {}
+    with open(filename, 'r') as f:
+        saved = eval(f.readline())
+        for method in saved:
+            if method not in output:
+                output[method] = {}
+            n = saved['n']
+            if n not in output[method]:
+                output[method][n] = []
+            output[method][n] += [saved[method]]
+
+    return output
+
+def compute_variance_by_entropy(methods, dataset, noise_levels=[0, .2, .3, .4, .5], increment=.1, num_runs=10, train_fn = train, folder='', limit=5000):
+
+    filename = folder + f'/variance_by_entropy_{dataset}.csv'
 
     for _ in tqdm(range(num_runs)): 
         for noise_level in noise_levels:
-            X, _, _ = dataloaders[dataset]()
+            X, y, z = dataloaders[dataset]()
+            X, _, _ = subsample(X, y, z, limit)
 
             # Need to know propensity to add noise
             X, y, p = build_synthetic_outcomes(X)
             uniform = np.random.random_sample(X.shape[0])
             z = (uniform < p).astype(int)
 
             noised_p = p + np.random.normal(0, noise_level, size=p.shape)
@@ -230,35 +224,44 @@
 
             cross_entropy = compute_cross_entropy(noised_p, z)
 
             cross_entropy = np.round(cross_entropy / increment) * increment
 
             true_effect = (y['y1'] - y['y0']).mean()
     
+            saved = {'cross_entropy':cross_entropy}
             for method, get_estimate in methods.items():
-                if cross_entropy not in variance[method]:
-                    variance[method][cross_entropy] = []
-                if len(variance[method][cross_entropy]) < num_runs:
-                    estimate = get_estimate(X, y, z, noised_p, train_fn)
-                    square_difference = (estimate - true_effect)**2
-                    variance[method][cross_entropy].append(square_difference) 
-
-    return variance
-
-def compute_variance_by_correlation(methods, dataset, alphas=[0, .15, .2, .25, .35, .5], increment=.1, num_runs=10, train_fn = train, variance=None):
-    if variance is None: 
-        variance = {}
-
-    for method in methods:
-        if method not in variance:
-            variance[method] = {}
+                #estimate = get_estimate(X, y, z, noised_p, train_fn)
+                estimate = np.random.uniform()
+                square_difference = (estimate - true_effect)**2
+                saved[method] = square_difference
+            with open(filename, 'a') as f:
+                f.write(str(saved) + '\n')
+
+    output = {}
+    with open(filename, 'r') as f:
+        saved = eval(f.readline())
+        for method in saved:
+            if method not in output:
+                output[method] = {}
+            cross_entropy = saved['cross_entropy']
+            if cross_entropy not in output[method]:
+                output[method][cross_entropy] = []
+            output[method][cross_entropy] += [saved[method]]        
+
+    return output
+
+def compute_variance_by_correlation(methods, dataset, alphas=[0, .15, .2, .25, .35, .5], increment=.1, num_runs=10, train_fn = train, folder='', limit=5000):
+
+    filename = folder + f'/variance_by_correlation_{dataset}.csv'
 
     for _ in tqdm(range(num_runs)): 
         for alpha in alphas:
-            X, _, _ = dataloaders[dataset]()
+            X, y, z = dataloaders[dataset]()
+            X, _, _ = subsample(X, y, z, limit)
 
             b = np.random.normal(size=X.shape[1])
             important_variable = X @ b
             p = sigmoid(important_variable)
             p = np.clip(p, 0.01, .99) # regularize
 
             random_vector = np.random.normal(size=X.shape[0])
@@ -267,27 +270,38 @@
                 'y0' : (1-p) * (1-alpha) + random_vector * alpha,
                 'y1' : 1-biased_treatment_effect(p) * (1-alpha) + random_vector * alpha
             }, dtype=float)
 
             uniform = np.random.random_sample(X.shape[0])
             z = (uniform < p).astype(int)
 
-            correlation = (
-                compute_distance_correlation(y['y0'][z==0], p[z==0]) + \
-                compute_distance_correlation(y['y1'][z==1], p[z==1])
-            )
+            correlation = (np.abs(np.corrcoef(y['y1'], p)[0,1]) + np.abs(np.corrcoef(y['y0'], p)[0,1]))/2
 
             correlation = np.round(correlation / increment) * increment
 
             p_estimated = estimate_propensity(X, z)
 
             true_effect = (y['y1'] - y['y0']).mean()
     
+            correlation = np.round(correlation / increment) * increment
+            saved = {'correlation':correlation}
             for method, get_estimate in methods.items():
-                if correlation not in variance[method]:
-                    variance[method][correlation] = []
-                if len(variance[method][correlation]) < num_runs:
-                    estimate = get_estimate(X, y, z, p_estimated, train_fn)
-                    square_difference = (estimate - true_effect)**2
-                    variance[method][correlation].append(square_difference) 
+                #estimate = get_estimate(X, y, z, p_estimated, train_fn)
+                estimate = np.random.uniform()
+                square_difference = (estimate - true_effect)**2
+                estimate
+                saved[method] = square_difference
+            with open(filename, 'a') as f:
+                f.write(str(saved) + '\n')
+    
+    output = {}
+    with open(filename, 'r') as f:
+        saved = eval(f.readline())
+        for method in saved:
+            if method not in output:
+                output[method] = {}
+            correlation = saved['correlation']
+            if correlation not in output[method]:
+                output[method][correlation] = []
+            output[method][correlation] += [saved[method]]
 
-    return variance
+    return output
```

### Comparing `naturalexperiments-0.0.7/naturalexperiments/data/acic/__init__.py` & `naturalexperiments-0.0.8/naturalexperiments/data/acic/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/data/ihdp/__init__.py` & `naturalexperiments-0.0.8/naturalexperiments/data/ihdp/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/data/jobs/__init__.py` & `naturalexperiments-0.0.8/naturalexperiments/data/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/data/news/__init__.py` & `naturalexperiments-0.0.8/naturalexperiments/data/news/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/data/rorco/__init__.py` & `naturalexperiments-0.0.8/naturalexperiments/data/rorco/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pandas as pd
-import pickle as pkl
 import sklearn.preprocessing
+from ...utils import build_synthetic_outcomes
 import os
 import requests
 
-def load_rorco():
+def load_rorco_real():
     filename = __file__.replace('__init__.py', 'rorco_data.csv')
 
     if not os.path.exists(filename):
         print('Downloading RORCO data...')
         # Download the data 
         url = 'https://raw.githubusercontent.com/rtealwitter/naturalexperiments/main/naturalexperiments/data/rorco/rorco_data.csv'
 
@@ -37,7 +37,34 @@
     X = X.select_dtypes(include = ['int16', 'int32', 'int64', 'float16', 'float32', 'float64'])
     X.replace(np.nan, 0, inplace=True)
 
     X = sklearn.preprocessing.StandardScaler().fit(X.values).transform(X.values)
 
     return X, y, z
 
+def load_rorco():
+    filename = __file__.replace('__init__.py', 'rorco_data.csv')
+
+    if not os.path.exists(filename):
+        print('Downloading RORCO data...')
+        # Download the data 
+        url = 'https://raw.githubusercontent.com/rtealwitter/naturalexperiments/main/naturalexperiments/data/rorco/rorco_data.csv'
+
+        r = requests.get(url)
+        open(filename, 'wb').write(r.content)
+
+    data = pd.read_csv(filename)
+
+    outcome_variable = 'Mean Scale Score'
+    treatment_variable = 'is_RORCO'
+
+    X = data.drop(columns = [treatment_variable, outcome_variable, 'num_from_RORCO'])
+
+    X = X.select_dtypes(include = ['int16', 'int32', 'int64', 'float16', 'float32', 'float64'])
+    X.replace(np.nan, 0, inplace=True)
+
+    X = sklearn.preprocessing.StandardScaler().fit(X.values).transform(X.values)
+
+    X, y, p = build_synthetic_outcomes(X)
+    uniform = np.random.random_sample(X.shape[0])
+    z = (uniform < p).astype(int)
+    return X, y, z
```

### Comparing `naturalexperiments-0.0.7/naturalexperiments/data/rorco/rorco_preprocess.py` & `naturalexperiments-0.0.8/naturalexperiments/data/rorco/rorco_preprocess.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/data/twins/__init__.py` & `naturalexperiments-0.0.8/naturalexperiments/data/twins/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/data_summary.py` & `naturalexperiments-0.0.8/naturalexperiments/data_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,18 +49,18 @@
     plot_percentiles = (percentiles[1:] + percentiles[:-1]) / 2
     treatment_outcomes, treatment_sizes = [], []
     control_outcomes, control_sizes = [], []
     total_size = len(propensity)
     for i in range(num_buckets):
         bucket = (propensity >= percentiles[i]) & (propensity < percentiles[i+1])
         treatment_in_bucket = np.sum(z * bucket)
-        treatment_outcomes.append(np.sum(y['y1'][bucket]) / treatment_in_bucket)
+        treatment_outcomes.append(np.sum((y['y1']*z)[bucket]) / treatment_in_bucket)
         treatment_sizes.append(treatment_in_bucket/total_size * 500)
         control_in_bucket = np.sum((1-z) * bucket)
-        control_outcomes.append(np.sum(y['y0'][bucket]) / control_in_bucket)
+        control_outcomes.append(np.sum((y['y0']*(1-z))[bucket]) / control_in_bucket)
         control_sizes.append(control_in_bucket / total_size * 500)
     plt.scatter(plot_percentiles, treatment_outcomes, s=treatment_sizes, color='teal')
     plt.plot(plot_percentiles, treatment_outcomes, label='Treatment', color='teal', linewidth=3)
 
     plt.scatter(plot_percentiles, control_outcomes, s=control_sizes, color='purple')
     plt.plot(plot_percentiles, control_outcomes, label='Control', color='purple', linestyle='dashed', linewidth=3)
 
@@ -125,19 +125,19 @@
         # Number of variables
         m = X.shape[1]
         # Percent treated 
         rate_treated = sig_round(np.mean(z) * 100)
         # Cross entropy of propensity score and z
         cross_entropy = sig_round(compute_cross_entropy(propensity, z))
         # Correlation between propensity and y1
-        #corr_y1 = sig_round(np.corrcoef(propensity[z==1], y['y1'][z==1])[0,1])
-        corr_y1 = sig_round(compute_distance_correlation(propensity[z==1], y['y1'][z==1].values))
+        corr_y1 = sig_round(np.corrcoef(propensity[z==1], y['y1'][z==1])[0,1])
+        #corr_y1 = sig_round(compute_distance_correlation(propensity[z==1], y['y1'][z==1].values))
         # Correlation between propensity and y0
-        #corr_y0 = sig_round(np.corrcoef(propensity[z==0], y['y0'][z==0])[0,1])
-        corr_y0 = sig_round(compute_distance_correlation(propensity[z==0], y['y0'][z==0].values))
+        corr_y0 = sig_round(np.corrcoef(propensity[z==0], y['y0'][z==0])[0,1])
+        #corr_y0 = sig_round(compute_distance_correlation(propensity[z==0], y['y0'][z==0].values))
 
         table += [[dataname, n, m, rate_treated, cross_entropy, corr_y1, corr_y0]]
 
     headers = ['Dataset', 'Size', 'Variables', '% Treated', 'Cross Entropy', 'Corr(y1, p)', 'Corr(y0, p)']
 
     if print_md:
         print(tabulate(table, headers=headers))
```

### Comparing `naturalexperiments-0.0.7/naturalexperiments/estimators/__init__.py` & `naturalexperiments-0.0.8/naturalexperiments/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/estimators/catenet.py` & `naturalexperiments-0.0.8/naturalexperiments/estimators/catenet.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/estimators/double_double.py` & `naturalexperiments-0.0.8/naturalexperiments/estimators/double_double.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/estimators/doubly_robust.py` & `naturalexperiments-0.0.8/naturalexperiments/estimators/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/estimators/off_policy.py` & `naturalexperiments-0.0.8/naturalexperiments/estimators/off_policy.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/estimators/tmle.py` & `naturalexperiments-0.0.8/naturalexperiments/estimators/tmle.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/naturalexperiments/model.py` & `naturalexperiments-0.0.8/naturalexperiments/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,25 +34,24 @@
 
     def __getitem__(self, idx):
         return self.X[idx], self.y[idx], self.weights[idx]
 
 class Model(torch.nn.Module):
     def __init__(self, input_size, hidden_dim=100, num_layers=3, output_logits=False):
         super(Model, self).__init__()
-        activation = torch.nn.Sigmoid
-        activation = torch.nn.ReLU
+        activation = torch.nn.Sigmoid if output_logits else torch.nn.ReLU
         layers = []
         layers.append(torch.nn.Linear(input_size, hidden_dim))
         layers.append(activation())
         for _ in range(num_layers-2):
             layers.append(torch.nn.Linear(hidden_dim, hidden_dim))
             layers.append(activation())            
         layers.append(torch.nn.Linear(hidden_dim, 1))    
         if output_logits:
-            layers.append(torch.nn.Sigmoid())
+            layers.append(activation())
         self.layers = torch.nn.Sequential(*layers)
 
     def forward(self, x):
         return self.layers(x)
 
 def train(X_train, y_train, X_test=None, weights=None, lr=.001, epochs=200, return_model=False, clip_value=None, noise_multiplier=None, is_bce=False):
```

### Comparing `naturalexperiments-0.0.7/naturalexperiments/utils.py` & `naturalexperiments-0.0.8/naturalexperiments/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 import sklearn
-import warnings
+import pandas as pd
 
 def center_distance_matrix(x):
     x = np.expand_dims(x, axis=1)
     X = sklearn.metrics.pairwise_distances(x)
     n = X.shape[0]
     row_means = np.tile(X.mean(axis=0), (n,1))
     col_means = np.tile(X.mean(axis=1), (n,1)).T
@@ -27,16 +27,35 @@
     distance_variance_Y = np.sum(centered_Y**2) / (n**2)
 
     return distance_covariance / np.sqrt(distance_variance_X * distance_variance_Y)
 
 def compute_cross_entropy(p, treatment):
     return - np.mean(treatment * np.log(p) + (1-treatment) * np.log(1-p))
 
+def sig_round(x, precision=3):
+    return np.format_float_positional(x, precision=precision, unique=False, fractional=False, trim='k')
+
 def biased_treatment_effect(x, scaling=1):
     # No effect on first half
     # Second half has effect of sqrt(x) * scaling
     adjustment = .5 - np.sqrt(.5) * scaling
     line = x * (x<.5).astype(int) + (x>=.5).astype(int) * (scaling * np.sqrt(x) + adjustment)
     return line
 
-def sig_round(x, precision=3):
-    return np.format_float_positional(x, precision=precision, unique=False, fractional=False, trim='k')
+def sigmoid(x):
+    return 1 / (1 + np.exp(-x))
+
+# Build problem where treatment and outcome are correlated
+def build_synthetic_outcomes(X, scale=True):
+    if scale:
+        X = sklearn.preprocessing.StandardScaler().fit(X).transform(X)
+
+    b = np.random.normal(size=X.shape[1])
+    important_variable = X @ b
+    p = sigmoid(important_variable)
+    p = np.clip(p, 0.01, .99) # regularize
+
+    y = pd.DataFrame({
+        'y0' : 1-p,
+        'y1' : 1-biased_treatment_effect(p)
+    }, dtype=float)
+    return X, y, p
```

### Comparing `naturalexperiments-0.0.7/naturalexperiments.egg-info/PKG-INFO` & `naturalexperiments-0.0.8/naturalexperiments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.7
+Version: 0.0.8
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.7/naturalexperiments.egg-info/SOURCES.txt` & `naturalexperiments-0.0.8/naturalexperiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.7/setup.py` & `naturalexperiments-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="naturalexperiments",
-    version="0.0.7",
+    version="0.0.8",
     author="R. Teal Witter",
     author_email="rtealwitter@gmail.com",
     description="Estimators and datasets for treatment effect estimation in natural experiments.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rtealwitter/naturalexperiments",
     packages=setuptools.find_packages(),
```

