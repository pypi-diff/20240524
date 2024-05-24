# Comparing `tmp/naturalexperiments-0.1.1.tar.gz` & `tmp/naturalexperiments-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalexperiments-0.1.1.tar", last modified: Fri May 24 16:22:57 2024, max compression
+gzip compressed data, was "naturalexperiments-0.1.2.tar", last modified: Fri May 24 20:50:31 2024, max compression
```

## Comparing `naturalexperiments-0.1.1.tar` & `naturalexperiments-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 16:22:57.889116 naturalexperiments-0.1.1/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.1.1/LICENSE
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 16:22:57.888967 naturalexperiments-0.1.1/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.1.1/README.md
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 16:22:57.883541 naturalexperiments-0.1.1/naturalexperiments/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-24 16:16:52.000000 naturalexperiments-0.1.1/naturalexperiments/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    12052 2024-05-24 15:10:46.000000 naturalexperiments-0.1.1/naturalexperiments/benchmark.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 16:22:57.884240 naturalexperiments-0.1.1/naturalexperiments/data/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      391 2024-05-24 13:38:10.000000 naturalexperiments-0.1.1/naturalexperiments/data/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 16:22:57.884526 naturalexperiments-0.1.1/naturalexperiments/data/acic/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.1.1/naturalexperiments/data/acic/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 16:22:57.884753 naturalexperiments-0.1.1/naturalexperiments/data/ihdp/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.1.1/naturalexperiments/data/ihdp/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 16:22:57.884961 naturalexperiments-0.1.1/naturalexperiments/data/jobs/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.1.1/naturalexperiments/data/jobs/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 16:22:57.885206 naturalexperiments-0.1.1/naturalexperiments/data/news/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.1.1/naturalexperiments/data/news/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 16:22:57.885719 naturalexperiments-0.1.1/naturalexperiments/data/rorco/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     2253 2024-05-24 13:38:42.000000 naturalexperiments-0.1.1/naturalexperiments/data/rorco/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.1.1/naturalexperiments/data/rorco/rorco_preprocess.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 16:22:57.885993 naturalexperiments-0.1.1/naturalexperiments/data/twins/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1810 2024-05-23 12:04:17.000000 naturalexperiments-0.1.1/naturalexperiments/data/twins/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     6151 2024-05-24 13:47:10.000000 naturalexperiments-0.1.1/naturalexperiments/data_summary.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 16:22:57.888757 naturalexperiments-0.1.1/naturalexperiments/estimators/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-23 17:30:11.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/catenet.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/direct_difference.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/direct_prediction.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/double_double.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/doubly_robust.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/horvitz_thompson.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/learned_direct.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/off_policy.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/propensity_stratification.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/regression_discontinuity.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.1.1/naturalexperiments/estimators/tmle.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     3546 2024-05-24 13:44:37.000000 naturalexperiments-0.1.1/naturalexperiments/model.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     2185 2024-05-24 13:19:39.000000 naturalexperiments-0.1.1/naturalexperiments/utils.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 16:22:57.884131 naturalexperiments-0.1.1/naturalexperiments.egg-info/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 16:22:57.000000 naturalexperiments-0.1.1/naturalexperiments.egg-info/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-24 16:22:57.000000 naturalexperiments-0.1.1/naturalexperiments.egg-info/SOURCES.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-24 16:22:57.000000 naturalexperiments-0.1.1/naturalexperiments.egg-info/dependency_links.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-24 16:22:57.000000 naturalexperiments-0.1.1/naturalexperiments.egg-info/top_level.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-24 16:22:57.889158 naturalexperiments-0.1.1/setup.cfg
--rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-24 16:22:55.000000 naturalexperiments-0.1.1/setup.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 20:50:31.901913 naturalexperiments-0.1.2/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.1.2/LICENSE
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 20:50:31.901736 naturalexperiments-0.1.2/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.1.2/README.md
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 20:50:31.895376 naturalexperiments-0.1.2/naturalexperiments/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-24 16:16:52.000000 naturalexperiments-0.1.2/naturalexperiments/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    12639 2024-05-24 20:41:03.000000 naturalexperiments-0.1.2/naturalexperiments/benchmark.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 20:50:31.896243 naturalexperiments-0.1.2/naturalexperiments/data/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      391 2024-05-24 13:38:10.000000 naturalexperiments-0.1.2/naturalexperiments/data/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 20:50:31.896511 naturalexperiments-0.1.2/naturalexperiments/data/acic/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.1.2/naturalexperiments/data/acic/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 20:50:31.896744 naturalexperiments-0.1.2/naturalexperiments/data/ihdp/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.1.2/naturalexperiments/data/ihdp/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 20:50:31.896957 naturalexperiments-0.1.2/naturalexperiments/data/jobs/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.1.2/naturalexperiments/data/jobs/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 20:50:31.897197 naturalexperiments-0.1.2/naturalexperiments/data/news/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.1.2/naturalexperiments/data/news/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 20:50:31.897723 naturalexperiments-0.1.2/naturalexperiments/data/rorco/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2253 2024-05-24 13:38:42.000000 naturalexperiments-0.1.2/naturalexperiments/data/rorco/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.1.2/naturalexperiments/data/rorco/rorco_preprocess.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 20:50:31.898010 naturalexperiments-0.1.2/naturalexperiments/data/twins/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1810 2024-05-23 12:04:17.000000 naturalexperiments-0.1.2/naturalexperiments/data/twins/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     6151 2024-05-24 13:47:10.000000 naturalexperiments-0.1.2/naturalexperiments/data_summary.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 20:50:31.901319 naturalexperiments-0.1.2/naturalexperiments/estimators/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-23 17:30:11.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      690 2024-05-24 20:42:56.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/catenet.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/direct_difference.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/direct_prediction.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/double_double.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/doubly_robust.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/horvitz_thompson.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/learned_direct.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/off_policy.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/propensity_stratification.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/regression_discontinuity.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.1.2/naturalexperiments/estimators/tmle.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     3546 2024-05-24 13:44:37.000000 naturalexperiments-0.1.2/naturalexperiments/model.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2185 2024-05-24 13:19:39.000000 naturalexperiments-0.1.2/naturalexperiments/utils.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 20:50:31.901517 naturalexperiments-0.1.2/naturalexperiments.egg-info/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 20:50:31.000000 naturalexperiments-0.1.2/naturalexperiments.egg-info/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-24 20:50:31.000000 naturalexperiments-0.1.2/naturalexperiments.egg-info/SOURCES.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-24 20:50:31.000000 naturalexperiments-0.1.2/naturalexperiments.egg-info/dependency_links.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-24 20:50:31.000000 naturalexperiments-0.1.2/naturalexperiments.egg-info/top_level.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-24 20:50:31.901964 naturalexperiments-0.1.2/setup.cfg
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-24 20:50:02.000000 naturalexperiments-0.1.2/setup.py
```

### Comparing `naturalexperiments-0.1.1/LICENSE` & `naturalexperiments-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/PKG-INFO` & `naturalexperiments-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.1.1
+Version: 0.1.2
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.1.1/naturalexperiments/benchmark.py` & `naturalexperiments-0.1.2/naturalexperiments/benchmark.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 from tqdm import tqdm
 import time
 from .model import estimate_propensity, train
 from .data import dataloaders
-from .utils import compute_cross_entropy, compute_distance_correlation, build_synthetic_outcomes, biased_treatment_effect, sigmoid
+from .utils import compute_cross_entropy, compute_distance_correlation, build_synthetic_outcomes, biased_treatment_effect, sigmoid, sig_round
 import numpy as np
 import sklearn.preprocessing
 import pandas as pd
 from tabulate import tabulate
 import matplotlib.pyplot as plt
 
 # # # VARIANCE BENCHMARK TABLE # # #
 
 def benchmark_table(variance, times, print_md=True, print_latex=False):
     table = []
     for method in variance:
         # Sometimes NaNs from one of the CATENet methods
         # Remove NaNs from variance[method]
         variance[method] = [x for x in variance[method] if not np.isnan(x)]
-        mean = round(np.mean(variance[method]))
-        median = round(np.median(variance[method]))
-        upper = round(np.percentile(variance[method], 75))
-        lower = round(np.percentile(variance[method], 25))
-        times_mean = round(np.mean(times[method]))
-        table.append([method, mean, lower, median, upper, times_mean])
+        row = [method]
+        mean = np.mean(variance[method])
+        median = np.median(variance[method])
+        upper = np.percentile(variance[method], 75)
+        lower = np.percentile(variance[method], 25)
+        times_mean = np.mean(times[method])
+        to_add = [mean, lower, median, upper, times_mean]
+        row += [sig_round(x) for x in to_add]
+        table.append(row)
 
     if print_md:
         print(tabulate(table, headers=['Method', 'Mean', '1st Quartile', '2nd Quartile', '3rd Quartile', 'Time (s)'], tablefmt="github"))    
 
     cols = []
-    for i in range(len(table[0])-1):
-        vals = [row[i+1] for row in table]
+    for i in range(1,len(table[0])):
+        vals = [row[i] for row in table]
         cols += [sorted(vals)]
     for row in table:
         print_row = [row[0]]
         for idx in range(1, len(row)):
             if row[idx] == cols[idx-1][0]:
-                print_row.append(r'\textbf{'+row[idx]+'}')
+                print_row.append(r'\textbf{'+str(row[idx])+'}')
             elif row[idx] == cols[idx-1][1]:
-                print_row.append(r'\textit{\textbf{'+row[idx]+'}}')
+                print_row.append(r'\textit{\textbf{'+str(row[idx])+'}}')
             elif row[idx] == cols[idx-1][2]:
-                print_row.append(r'\underline{\textbf{'+row[idx]+'}}')
+                print_row.append(r'\underline{\textbf{'+str(row[idx])+'}}')
             else:
                 print_row.append(row[idx])
         if print_latex:
             print(' & '.join(print_row) + '\\\\ \hline')
 
 # # # VARIANCE PLOTS # # #
 
@@ -154,21 +157,23 @@
                 saved[method] = (estimate, run_time)
         with open(filename, 'a') as f:
             f.write(str(saved) + '\n')
     
     
     output, times = {}, {}
     with open(filename, 'r') as f:
-        saved = eval(f.readline())
-        for method in saved:
-            if method not in output:
-                output[method] = []
-                times[method] = []
-            output[method] += [saved[method][0]]
-            times[method] += [saved[method][1]]
+        for line in f:
+            line = line.replace('Array(', '').replace(', dtype=float32)', '')
+            saved = eval(line)
+            for method in saved:
+                if method not in output:
+                    output[method] = []
+                    times[method] = []
+                output[method] += [float(saved[method][0])]
+                times[method] += [saved[method][1]]
 
     return output, times
 
 def compute_variance(methods, dataset, num_runs=10, train_fn=train, folder='', limit=5000):
     return compute_estimates(methods, dataset, num_runs=num_runs, train_fn=train_fn, folder=folder, return_error=True, limit=limit)
 
 def compute_variance_by_n(methods, dataset, ns, num_runs=10, train_fn=train, folder='', limit=5000):
@@ -188,22 +193,24 @@
                 square_difference = (estimate - true_effect)**2
                 saved[method] = square_difference
             with open(filename, 'a') as f:
                 f.write(str(saved) + '\n')
     
     output = {}
     with open(filename, 'r') as f:
-        saved = eval(f.readline())
-        for method in saved:
-            if method not in output:
-                output[method] = {}
-            n = saved['n']
-            if n not in output[method]:
-                output[method][n] = []
-            output[method][n] += [saved[method]]
+        for line in f:
+            line = line.replace('Array(', '').replace(', dtype=float32)', '')
+            saved = eval(line)
+            for method in saved:
+                if method not in output:
+                    output[method] = {}
+                n = saved['n']
+                if n not in output[method]:
+                    output[method][n] = []
+                output[method][n] += [float(saved[method])]
 
     return output
 
 def compute_variance_by_entropy(methods, dataset, noise_levels=[0, .2, .3, .4, .5], increment=.1, num_runs=10, train_fn = train, folder='', limit=5000):
 
     filename = folder + f'/variance_by_entropy_{dataset}.csv'
 
@@ -232,22 +239,24 @@
                 square_difference = (estimate - true_effect)**2
                 saved[method] = square_difference
             with open(filename, 'a') as f:
                 f.write(str(saved) + '\n')
 
     output = {}
     with open(filename, 'r') as f:
-        saved = eval(f.readline())
-        for method in saved:
-            if method not in output:
-                output[method] = {}
-            cross_entropy = saved['cross_entropy']
-            if cross_entropy not in output[method]:
-                output[method][cross_entropy] = []
-            output[method][cross_entropy] += [saved[method]]        
+        for line in f:
+            line = line.replace('Array(', '').replace(', dtype=float32)', '')
+            saved = eval(line)
+            for method in saved:
+                if method not in output:
+                    output[method] = {}
+                cross_entropy = saved['cross_entropy']
+                if cross_entropy not in output[method]:
+                    output[method][cross_entropy] = []
+                output[method][cross_entropy] += [float(saved[method])]
 
     return output
 
 def compute_variance_by_correlation(methods, dataset, alphas=[0, .15, .2, .25, .35, .5], increment=.1, num_runs=10, train_fn = train, folder='', limit=5000):
 
     filename = folder + f'/variance_by_correlation_{dataset}.csv'
 
@@ -287,17 +296,19 @@
                 estimate
                 saved[method] = square_difference
             with open(filename, 'a') as f:
                 f.write(str(saved) + '\n')
     
     output = {}
     with open(filename, 'r') as f:
-        saved = eval(f.readline())
-        for method in saved:
-            if method not in output:
-                output[method] = {}
-            correlation = saved['correlation']
-            if correlation not in output[method]:
-                output[method][correlation] = []
-            output[method][correlation] += [saved[method]]
+        for line in f:
+            line = line.replace('Array(', '').replace(', dtype=float32)', '')
+            saved = eval(line)
+            for method in saved:
+                if method not in output:
+                    output[method] = {}
+                correlation = saved['correlation']
+                if correlation not in output[method]:
+                    output[method][correlation] = []
+                output[method][correlation] += [float(saved[method])]
 
     return output
```

### Comparing `naturalexperiments-0.1.1/naturalexperiments/data/acic/__init__.py` & `naturalexperiments-0.1.2/naturalexperiments/data/acic/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/data/ihdp/__init__.py` & `naturalexperiments-0.1.2/naturalexperiments/data/ihdp/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/data/jobs/__init__.py` & `naturalexperiments-0.1.2/naturalexperiments/data/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/data/news/__init__.py` & `naturalexperiments-0.1.2/naturalexperiments/data/news/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/data/rorco/__init__.py` & `naturalexperiments-0.1.2/naturalexperiments/data/rorco/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/data/rorco/rorco_preprocess.py` & `naturalexperiments-0.1.2/naturalexperiments/data/rorco/rorco_preprocess.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/data/twins/__init__.py` & `naturalexperiments-0.1.2/naturalexperiments/data/twins/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/data_summary.py` & `naturalexperiments-0.1.2/naturalexperiments/data_summary.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/estimators/__init__.py` & `naturalexperiments-0.1.2/naturalexperiments/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/estimators/catenet.py` & `naturalexperiments-0.1.2/naturalexperiments/estimators/catenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     def get_catenet_estimate(X, y, z, p, train_fn):
         y = y['y0']*(1-z) + y['y1'] * z
         y = y.values
         w = z
         t = catenet_models[model_name]()
         t.fit(X, y, w)
         cate_pred = t.predict(X)
-        return cate_pred.mean()
+        return float(cate_pred.mean())
     return get_catenet_estimate
```

### Comparing `naturalexperiments-0.1.1/naturalexperiments/estimators/double_double.py` & `naturalexperiments-0.1.2/naturalexperiments/estimators/double_double.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/estimators/doubly_robust.py` & `naturalexperiments-0.1.2/naturalexperiments/estimators/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/estimators/off_policy.py` & `naturalexperiments-0.1.2/naturalexperiments/estimators/off_policy.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/estimators/tmle.py` & `naturalexperiments-0.1.2/naturalexperiments/estimators/tmle.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/model.py` & `naturalexperiments-0.1.2/naturalexperiments/model.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments/utils.py` & `naturalexperiments-0.1.2/naturalexperiments/utils.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/naturalexperiments.egg-info/PKG-INFO` & `naturalexperiments-0.1.2/naturalexperiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.1.1
+Version: 0.1.2
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.1.1/naturalexperiments.egg-info/SOURCES.txt` & `naturalexperiments-0.1.2/naturalexperiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.1.1/setup.py` & `naturalexperiments-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="naturalexperiments",
-    version="0.1.1",
+    version="0.1.2",
     author="R. Teal Witter",
     author_email="rtealwitter@gmail.com",
     description="Estimators and datasets for treatment effect estimation in natural experiments.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rtealwitter/naturalexperiments",
     packages=setuptools.find_packages(),
```

