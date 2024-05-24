# Comparing `tmp/naturalexperiments-0.0.8.tar.gz` & `tmp/naturalexperiments-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalexperiments-0.0.8.tar", last modified: Fri May 24 15:00:21 2024, max compression
+gzip compressed data, was "naturalexperiments-0.0.9.tar", last modified: Fri May 24 15:11:30 2024, max compression
```

## Comparing `naturalexperiments-0.0.8.tar` & `naturalexperiments-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.306275 naturalexperiments-0.0.8/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.8/LICENSE
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 15:00:21.306090 naturalexperiments-0.0.8/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.8/README.md
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.300422 naturalexperiments-0.0.8/naturalexperiments/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    12240 2024-05-24 14:54:01.000000 naturalexperiments-0.0.8/naturalexperiments/benchmark.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.301116 naturalexperiments-0.0.8/naturalexperiments/data/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      391 2024-05-24 13:38:10.000000 naturalexperiments-0.0.8/naturalexperiments/data/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.301380 naturalexperiments-0.0.8/naturalexperiments/data/acic/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.8/naturalexperiments/data/acic/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.301648 naturalexperiments-0.0.8/naturalexperiments/data/ihdp/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.8/naturalexperiments/data/ihdp/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.301886 naturalexperiments-0.0.8/naturalexperiments/data/jobs/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.8/naturalexperiments/data/jobs/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.302154 naturalexperiments-0.0.8/naturalexperiments/data/news/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.0.8/naturalexperiments/data/news/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.302698 naturalexperiments-0.0.8/naturalexperiments/data/rorco/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     2253 2024-05-24 13:38:42.000000 naturalexperiments-0.0.8/naturalexperiments/data/rorco/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.8/naturalexperiments/data/rorco/rorco_preprocess.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.302963 naturalexperiments-0.0.8/naturalexperiments/data/twins/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1810 2024-05-23 12:04:17.000000 naturalexperiments-0.0.8/naturalexperiments/data/twins/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     6151 2024-05-24 13:47:10.000000 naturalexperiments-0.0.8/naturalexperiments/data_summary.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.305655 naturalexperiments-0.0.8/naturalexperiments/estimators/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-23 17:30:11.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/catenet.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/direct_difference.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/direct_prediction.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/double_double.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/doubly_robust.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/horvitz_thompson.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/learned_direct.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/off_policy.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/propensity_stratification.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/regression_discontinuity.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.8/naturalexperiments/estimators/tmle.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     3546 2024-05-24 13:44:37.000000 naturalexperiments-0.0.8/naturalexperiments/model.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     2185 2024-05-24 13:19:39.000000 naturalexperiments-0.0.8/naturalexperiments/utils.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:00:21.305852 naturalexperiments-0.0.8/naturalexperiments.egg-info/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 15:00:21.000000 naturalexperiments-0.0.8/naturalexperiments.egg-info/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-24 15:00:21.000000 naturalexperiments-0.0.8/naturalexperiments.egg-info/SOURCES.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-24 15:00:21.000000 naturalexperiments-0.0.8/naturalexperiments.egg-info/dependency_links.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-24 15:00:21.000000 naturalexperiments-0.0.8/naturalexperiments.egg-info/top_level.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-24 15:00:21.306316 naturalexperiments-0.0.8/setup.cfg
--rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-24 14:59:57.000000 naturalexperiments-0.0.8/setup.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:11:30.543063 naturalexperiments-0.0.9/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.9/LICENSE
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 15:11:30.542870 naturalexperiments-0.0.9/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.9/README.md
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:11:30.536886 naturalexperiments-0.0.9/naturalexperiments/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    12052 2024-05-24 15:10:46.000000 naturalexperiments-0.0.9/naturalexperiments/benchmark.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:11:30.537614 naturalexperiments-0.0.9/naturalexperiments/data/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      391 2024-05-24 13:38:10.000000 naturalexperiments-0.0.9/naturalexperiments/data/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:11:30.537842 naturalexperiments-0.0.9/naturalexperiments/data/acic/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.9/naturalexperiments/data/acic/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:11:30.538056 naturalexperiments-0.0.9/naturalexperiments/data/ihdp/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.9/naturalexperiments/data/ihdp/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:11:30.538279 naturalexperiments-0.0.9/naturalexperiments/data/jobs/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.9/naturalexperiments/data/jobs/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:11:30.538515 naturalexperiments-0.0.9/naturalexperiments/data/news/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.0.9/naturalexperiments/data/news/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:11:30.539067 naturalexperiments-0.0.9/naturalexperiments/data/rorco/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2253 2024-05-24 13:38:42.000000 naturalexperiments-0.0.9/naturalexperiments/data/rorco/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.9/naturalexperiments/data/rorco/rorco_preprocess.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:11:30.539374 naturalexperiments-0.0.9/naturalexperiments/data/twins/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1810 2024-05-23 12:04:17.000000 naturalexperiments-0.0.9/naturalexperiments/data/twins/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     6151 2024-05-24 13:47:10.000000 naturalexperiments-0.0.9/naturalexperiments/data_summary.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:11:30.542338 naturalexperiments-0.0.9/naturalexperiments/estimators/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-23 17:30:11.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/catenet.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/direct_difference.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/direct_prediction.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/double_double.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/doubly_robust.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/horvitz_thompson.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/learned_direct.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/off_policy.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/propensity_stratification.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/regression_discontinuity.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.9/naturalexperiments/estimators/tmle.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     3546 2024-05-24 13:44:37.000000 naturalexperiments-0.0.9/naturalexperiments/model.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     2185 2024-05-24 13:19:39.000000 naturalexperiments-0.0.9/naturalexperiments/utils.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-24 15:11:30.542553 naturalexperiments-0.0.9/naturalexperiments.egg-info/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-24 15:11:30.000000 naturalexperiments-0.0.9/naturalexperiments.egg-info/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-24 15:11:30.000000 naturalexperiments-0.0.9/naturalexperiments.egg-info/SOURCES.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-24 15:11:30.000000 naturalexperiments-0.0.9/naturalexperiments.egg-info/dependency_links.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-24 15:11:30.000000 naturalexperiments-0.0.9/naturalexperiments.egg-info/top_level.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-24 15:11:30.543107 naturalexperiments-0.0.9/setup.cfg
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-24 15:11:02.000000 naturalexperiments-0.0.9/setup.py
```

### Comparing `naturalexperiments-0.0.8/LICENSE` & `naturalexperiments-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/PKG-INFO` & `naturalexperiments-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.8
+Version: 0.0.9
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.8/naturalexperiments/benchmark.py` & `naturalexperiments-0.0.9/naturalexperiments/benchmark.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,16 +141,15 @@
         X, y, z = subsample(X, y, z, limit)
         p_estimated = estimate_propensity(X, z)
         true_effect = (y['y1'] - y['y0']).mean()
  
         saved = {}
         for method, get_estimate in methods.items():
             time_start = time.time()
-            #estimate = get_estimate(X, y, z, p_estimated, train_fn)
-            estimate = np.random.uniform()
+            estimate = get_estimate(X, y, z, p_estimated, train_fn)
             square_difference = (estimate - true_effect)**2
             run_time = time.time() - time_start            
             if return_error:
                 saved[method] = (square_difference, run_time)
             else:
                 saved[method] = (estimate, run_time)
         with open(filename, 'a') as f:
@@ -181,16 +180,15 @@
             X, y, z = subsample(X, y, z, n)
 
             p_estimated = estimate_propensity(X, z)
             true_effect = (y['y1'] - y['y0']).mean()
     
             saved = {'n':n}
             for method, get_estimate in methods.items():
-                #estimate = get_estimate(X, y, z, p_estimated, train_fn)
-                estimate = np.random.uniform()
+                estimate = get_estimate(X, y, z, p_estimated, train_fn)
                 square_difference = (estimate - true_effect)**2
                 saved[method] = square_difference
             with open(filename, 'a') as f:
                 f.write(str(saved) + '\n')
     
     output = {}
     with open(filename, 'r') as f:
@@ -226,16 +224,15 @@
 
             cross_entropy = np.round(cross_entropy / increment) * increment
 
             true_effect = (y['y1'] - y['y0']).mean()
     
             saved = {'cross_entropy':cross_entropy}
             for method, get_estimate in methods.items():
-                #estimate = get_estimate(X, y, z, noised_p, train_fn)
-                estimate = np.random.uniform()
+                estimate = get_estimate(X, y, z, noised_p, train_fn)
                 square_difference = (estimate - true_effect)**2
                 saved[method] = square_difference
             with open(filename, 'a') as f:
                 f.write(str(saved) + '\n')
 
     output = {}
     with open(filename, 'r') as f:
@@ -281,16 +278,15 @@
             p_estimated = estimate_propensity(X, z)
 
             true_effect = (y['y1'] - y['y0']).mean()
     
             correlation = np.round(correlation / increment) * increment
             saved = {'correlation':correlation}
             for method, get_estimate in methods.items():
-                #estimate = get_estimate(X, y, z, p_estimated, train_fn)
-                estimate = np.random.uniform()
+                estimate = get_estimate(X, y, z, p_estimated, train_fn)
                 square_difference = (estimate - true_effect)**2
                 estimate
                 saved[method] = square_difference
             with open(filename, 'a') as f:
                 f.write(str(saved) + '\n')
     
     output = {}
```

### Comparing `naturalexperiments-0.0.8/naturalexperiments/data/acic/__init__.py` & `naturalexperiments-0.0.9/naturalexperiments/data/acic/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/data/ihdp/__init__.py` & `naturalexperiments-0.0.9/naturalexperiments/data/ihdp/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/data/jobs/__init__.py` & `naturalexperiments-0.0.9/naturalexperiments/data/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/data/news/__init__.py` & `naturalexperiments-0.0.9/naturalexperiments/data/news/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/data/rorco/__init__.py` & `naturalexperiments-0.0.9/naturalexperiments/data/rorco/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/data/rorco/rorco_preprocess.py` & `naturalexperiments-0.0.9/naturalexperiments/data/rorco/rorco_preprocess.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/data/twins/__init__.py` & `naturalexperiments-0.0.9/naturalexperiments/data/twins/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/data_summary.py` & `naturalexperiments-0.0.9/naturalexperiments/data_summary.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/estimators/__init__.py` & `naturalexperiments-0.0.9/naturalexperiments/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/estimators/catenet.py` & `naturalexperiments-0.0.9/naturalexperiments/estimators/catenet.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/estimators/double_double.py` & `naturalexperiments-0.0.9/naturalexperiments/estimators/double_double.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/estimators/doubly_robust.py` & `naturalexperiments-0.0.9/naturalexperiments/estimators/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/estimators/off_policy.py` & `naturalexperiments-0.0.9/naturalexperiments/estimators/off_policy.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/estimators/tmle.py` & `naturalexperiments-0.0.9/naturalexperiments/estimators/tmle.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/model.py` & `naturalexperiments-0.0.9/naturalexperiments/model.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments/utils.py` & `naturalexperiments-0.0.9/naturalexperiments/utils.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/naturalexperiments.egg-info/PKG-INFO` & `naturalexperiments-0.0.9/naturalexperiments.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.8
+Version: 0.0.9
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.8/naturalexperiments.egg-info/SOURCES.txt` & `naturalexperiments-0.0.9/naturalexperiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.8/setup.py` & `naturalexperiments-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="naturalexperiments",
-    version="0.0.8",
+    version="0.0.9",
     author="R. Teal Witter",
     author_email="rtealwitter@gmail.com",
     description="Estimators and datasets for treatment effect estimation in natural experiments.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rtealwitter/naturalexperiments",
     packages=setuptools.find_packages(),
```

