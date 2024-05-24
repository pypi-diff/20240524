# Comparing `tmp/naturalexperiments-0.0.6.tar.gz` & `tmp/naturalexperiments-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalexperiments-0.0.6.tar", last modified: Thu May 23 12:24:04 2024, max compression
+gzip compressed data, was "naturalexperiments-0.0.7.tar", last modified: Thu May 23 21:04:45 2024, max compression
```

## Comparing `naturalexperiments-0.0.6.tar` & `naturalexperiments-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.846246 naturalexperiments-0.0.6/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.6/LICENSE
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 12:24:04.846032 naturalexperiments-0.0.6/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.6/README.md
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.842299 naturalexperiments-0.0.6/naturalexperiments/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    11440 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/benchmark.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843003 naturalexperiments-0.0.6/naturalexperiments/data/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      338 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/data/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843142 naturalexperiments-0.0.6/naturalexperiments/data/acic/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.6/naturalexperiments/data/acic/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843273 naturalexperiments-0.0.6/naturalexperiments/data/ihdp/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.6/naturalexperiments/data/ihdp/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843403 naturalexperiments-0.0.6/naturalexperiments/data/jobs/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.6/naturalexperiments/data/jobs/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843526 naturalexperiments-0.0.6/naturalexperiments/data/news/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.0.6/naturalexperiments/data/news/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843781 naturalexperiments-0.0.6/naturalexperiments/data/rorco/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1215 2024-05-22 21:42:52.000000 naturalexperiments-0.0.6/naturalexperiments/data/rorco/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.6/naturalexperiments/data/rorco/rorco_preprocess.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.844030 naturalexperiments-0.0.6/naturalexperiments/data/twins/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1810 2024-05-23 12:04:17.000000 naturalexperiments-0.0.6/naturalexperiments/data/twins/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     6139 2024-05-23 12:21:06.000000 naturalexperiments-0.0.6/naturalexperiments/data_summary.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.845664 naturalexperiments-0.0.6/naturalexperiments/estimators/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/catenet.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/direct_difference.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/direct_prediction.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/double_double.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/doubly_robust.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/horvitz_thompson.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/learned_direct.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/off_policy.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/propensity_stratification.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/regression_discontinuity.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/tmle.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     3438 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/model.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/utils.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.845834 naturalexperiments-0.0.6/naturalexperiments.egg-info/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 12:24:04.000000 naturalexperiments-0.0.6/naturalexperiments.egg-info/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-23 12:24:04.000000 naturalexperiments-0.0.6/naturalexperiments.egg-info/SOURCES.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-23 12:24:04.000000 naturalexperiments-0.0.6/naturalexperiments.egg-info/dependency_links.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-23 12:24:04.000000 naturalexperiments-0.0.6/naturalexperiments.egg-info/top_level.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-23 12:24:04.846289 naturalexperiments-0.0.6/setup.cfg
--rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-23 12:23:25.000000 naturalexperiments-0.0.6/setup.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.935469 naturalexperiments-0.0.7/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.7/LICENSE
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 21:04:45.935284 naturalexperiments-0.0.7/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.7/README.md
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.928974 naturalexperiments-0.0.7/naturalexperiments/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    11440 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/benchmark.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.929649 naturalexperiments-0.0.7/naturalexperiments/data/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      338 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/data/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.929853 naturalexperiments-0.0.7/naturalexperiments/data/acic/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.7/naturalexperiments/data/acic/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.930048 naturalexperiments-0.0.7/naturalexperiments/data/ihdp/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.7/naturalexperiments/data/ihdp/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.930236 naturalexperiments-0.0.7/naturalexperiments/data/jobs/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.7/naturalexperiments/data/jobs/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.930471 naturalexperiments-0.0.7/naturalexperiments/data/news/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.0.7/naturalexperiments/data/news/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.930917 naturalexperiments-0.0.7/naturalexperiments/data/rorco/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-23 21:01:42.000000 naturalexperiments-0.0.7/naturalexperiments/data/rorco/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.7/naturalexperiments/data/rorco/rorco_preprocess.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.931156 naturalexperiments-0.0.7/naturalexperiments/data/twins/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1810 2024-05-23 12:04:17.000000 naturalexperiments-0.0.7/naturalexperiments/data/twins/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     6139 2024-05-23 12:21:06.000000 naturalexperiments-0.0.7/naturalexperiments/data_summary.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.934793 naturalexperiments-0.0.7/naturalexperiments/estimators/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-23 17:30:11.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/catenet.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/direct_difference.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/direct_prediction.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/double_double.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/doubly_robust.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/horvitz_thompson.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/learned_direct.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/off_policy.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/propensity_stratification.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/regression_discontinuity.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/estimators/tmle.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     3551 2024-05-23 20:59:16.000000 naturalexperiments-0.0.7/naturalexperiments/model.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.7/naturalexperiments/utils.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 21:04:45.935100 naturalexperiments-0.0.7/naturalexperiments.egg-info/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 21:04:45.000000 naturalexperiments-0.0.7/naturalexperiments.egg-info/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-23 21:04:45.000000 naturalexperiments-0.0.7/naturalexperiments.egg-info/SOURCES.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-23 21:04:45.000000 naturalexperiments-0.0.7/naturalexperiments.egg-info/dependency_links.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-23 21:04:45.000000 naturalexperiments-0.0.7/naturalexperiments.egg-info/top_level.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-23 21:04:45.935510 naturalexperiments-0.0.7/setup.cfg
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-23 21:03:05.000000 naturalexperiments-0.0.7/setup.py
```

### Comparing `naturalexperiments-0.0.6/LICENSE` & `naturalexperiments-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/PKG-INFO` & `naturalexperiments-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.6
+Version: 0.0.7
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.6/naturalexperiments/benchmark.py` & `naturalexperiments-0.0.7/naturalexperiments/benchmark.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/data/acic/__init__.py` & `naturalexperiments-0.0.7/naturalexperiments/data/acic/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/data/ihdp/__init__.py` & `naturalexperiments-0.0.7/naturalexperiments/data/ihdp/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/data/jobs/__init__.py` & `naturalexperiments-0.0.7/naturalexperiments/data/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/data/news/__init__.py` & `naturalexperiments-0.0.7/naturalexperiments/data/news/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/data/rorco/__init__.py` & `naturalexperiments-0.0.7/naturalexperiments/data/rorco/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,17 +21,19 @@
     # Restrict to rural schools
     data = data[data['is_rural'] == 1]
 
     outcome_variable = 'Mean Scale Score'
     treatment_variable = 'is_RORCO'
 
     z = data[treatment_variable].values
+    y_all = data[outcome_variable].values
+    y_all = (y_all - y_all.mean()) / y_all.std()
     y = pd.DataFrame({
-        'y1' : data[outcome_variable].values * z,
-        'y0' : data[outcome_variable].values * (1-z)
+        'y1' : y_all * z,
+        'y0' : y_all * (1-z)
     }, dtype=float)
 
     X = data.drop(columns = [treatment_variable, outcome_variable, 'num_from_RORCO'])
 
     X = X.select_dtypes(include = ['int16', 'int32', 'int64', 'float16', 'float32', 'float64'])
     X.replace(np.nan, 0, inplace=True)
```

### Comparing `naturalexperiments-0.0.6/naturalexperiments/data/rorco/rorco_preprocess.py` & `naturalexperiments-0.0.7/naturalexperiments/data/rorco/rorco_preprocess.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/data/twins/__init__.py` & `naturalexperiments-0.0.7/naturalexperiments/data/twins/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/data_summary.py` & `naturalexperiments-0.0.7/naturalexperiments/data_summary.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/estimators/__init__.py` & `naturalexperiments-0.0.7/naturalexperiments/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/estimators/catenet.py` & `naturalexperiments-0.0.7/naturalexperiments/estimators/catenet.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/estimators/double_double.py` & `naturalexperiments-0.0.7/naturalexperiments/estimators/double_double.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/estimators/doubly_robust.py` & `naturalexperiments-0.0.7/naturalexperiments/estimators/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/estimators/off_policy.py` & `naturalexperiments-0.0.7/naturalexperiments/estimators/off_policy.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/estimators/tmle.py` & `naturalexperiments-0.0.7/naturalexperiments/estimators/tmle.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments/model.py` & `naturalexperiments-0.0.7/naturalexperiments/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,44 +32,47 @@
     def __len__(self):
         return len(self.X)
 
     def __getitem__(self, idx):
         return self.X[idx], self.y[idx], self.weights[idx]
 
 class Model(torch.nn.Module):
-    def __init__(self, input_size, hidden_dim=100, num_layers=3):
+    def __init__(self, input_size, hidden_dim=100, num_layers=3, output_logits=False):
         super(Model, self).__init__()
         activation = torch.nn.Sigmoid
+        activation = torch.nn.ReLU
         layers = []
         layers.append(torch.nn.Linear(input_size, hidden_dim))
         layers.append(activation())
         for _ in range(num_layers-2):
             layers.append(torch.nn.Linear(hidden_dim, hidden_dim))
             layers.append(activation())            
         layers.append(torch.nn.Linear(hidden_dim, 1))    
-        layers.append(activation())
+        if output_logits:
+            layers.append(torch.nn.Sigmoid())
         self.layers = torch.nn.Sequential(*layers)
 
     def forward(self, x):
         return self.layers(x)
 
-def train(X_train, y_train, X_test=None, weights=None, lr=.001, epochs=200, return_model=False, clip_value=None, noise_multiplier=None, loss=None):
+def train(X_train, y_train, X_test=None, weights=None, lr=.001, epochs=200, return_model=False, clip_value=None, noise_multiplier=None, is_bce=False):
 
     device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
     if weights is None:
         weights = np.ones(X_train.shape[0])
 
     dataset = CustomDataset(X_train, y_train, weights)
     dataloader = DataLoader(dataset, batch_size=1000, shuffle=True)
 
-    if loss is None:
-        loss = lambda y_true, y_pred, weights: ((y_true - y_pred) ** 2 * weights).mean()
+    loss = lambda y_true, y_pred, weights: ((y_true - y_pred) ** 2 * weights).mean()
+    if is_bce:
+        loss = lambda y_true, y_pred, weights: torch.nn.BCELoss()(y_pred, y_true)
 
-    model = Model(X_train.shape[1], hidden_dim=100).to(device)
+    model = Model(X_train.shape[1], hidden_dim=100, output_logits=is_bce).to(device)
 
     for p in model.parameters():
         if clip_value is not None:
             p.register_hook(lambda grad: torch.clamp(grad, -clip_value, clip_value))
         if noise_multiplier is not None:
             p.register_hook(lambda grad: add_noise(grad, noise_multiplier, secure_mode=True))
 
@@ -85,11 +88,10 @@
 
     easy_model = lambda X : model(to_torch(X).to(device)).detach().squeeze().cpu().numpy()
     if return_model:
         return easy_model
     return easy_model(X_test)
 
 def estimate_propensity(X, treatment):
-    loss = lambda y_true, y_pred, weights: torch.nn.BCELoss()(y_pred, y_true)
-    propensity = train(X, treatment, X, loss=loss)
+    propensity = train(X, treatment, X, is_bce=True)
     # Clip propensity to avoid numerical instability
     return propensity.clip(.01, .99)
```

### Comparing `naturalexperiments-0.0.6/naturalexperiments/utils.py` & `naturalexperiments-0.0.7/naturalexperiments/utils.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/naturalexperiments.egg-info/PKG-INFO` & `naturalexperiments-0.0.7/naturalexperiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.6
+Version: 0.0.7
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.6/naturalexperiments.egg-info/SOURCES.txt` & `naturalexperiments-0.0.7/naturalexperiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.6/setup.py` & `naturalexperiments-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="naturalexperiments",
-    version="0.0.6",
+    version="0.0.7",
     author="R. Teal Witter",
     author_email="rtealwitter@gmail.com",
     description="Estimators and datasets for treatment effect estimation in natural experiments.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rtealwitter/naturalexperiments",
     packages=setuptools.find_packages(),
```

