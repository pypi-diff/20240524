# Comparing `tmp/smartpredict-0.7.2.tar.gz` & `tmp/smartpredict-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartpredict-0.7.2.tar", last modified: Thu May 23 09:30:17 2024, max compression
+gzip compressed data, was "smartpredict-0.7.3.tar", last modified: Fri May 24 08:58:17 2024, max compression
```

## Comparing `smartpredict-0.7.2.tar` & `smartpredict-0.7.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:30:17.220639 smartpredict-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-23 09:30:13.000000 smartpredict-0.7.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 09:30:13.000000 smartpredict-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-23 09:30:17.220639 smartpredict-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-23 09:30:13.000000 smartpredict-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 09:30:13.000000 smartpredict-0.7.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:30:17.220639 smartpredict-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-23 09:30:13.000000 smartpredict-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:30:17.220639 smartpredict-0.7.2/smartpredict/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-23 09:30:13.000000 smartpredict-0.7.2/smartpredict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 09:30:13.000000 smartpredict-0.7.2/smartpredict/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 09:30:13.000000 smartpredict-0.7.2/smartpredict/ensemble_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-23 09:30:13.000000 smartpredict-0.7.2/smartpredict/explainability.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-23 09:30:13.000000 smartpredict-0.7.2/smartpredict/feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-23 09:30:13.000000 smartpredict-0.7.2/smartpredict/hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-23 09:30:13.000000 smartpredict-0.7.2/smartpredict/model_assessment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-23 09:30:13.000000 smartpredict-0.7.2/smartpredict/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-23 09:30:13.000000 smartpredict-0.7.2/smartpredict/supervised.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:30:13.000000 smartpredict-0.7.2/smartpredict/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:30:17.220639 smartpredict-0.7.2/smartpredict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-05-23 09:30:17.000000 smartpredict-0.7.2/smartpredict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-23 09:30:17.000000 smartpredict-0.7.2/smartpredict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:30:17.000000 smartpredict-0.7.2/smartpredict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 09:30:17.000000 smartpredict-0.7.2/smartpredict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 09:30:17.000000 smartpredict-0.7.2/smartpredict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:30:17.220639 smartpredict-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:30:13.000000 smartpredict-0.7.2/tests/test_smartpredict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:58:17.908413 smartpredict-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-24 08:58:10.000000 smartpredict-0.7.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-24 08:58:10.000000 smartpredict-0.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-24 08:58:17.908413 smartpredict-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-24 08:58:10.000000 smartpredict-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-24 08:58:10.000000 smartpredict-0.7.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 08:58:17.908413 smartpredict-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-24 08:58:10.000000 smartpredict-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:58:17.904413 smartpredict-0.7.3/smartpredict/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-24 08:58:10.000000 smartpredict-0.7.3/smartpredict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-24 08:58:10.000000 smartpredict-0.7.3/smartpredict/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-24 08:58:10.000000 smartpredict-0.7.3/smartpredict/ensemble_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-24 08:58:10.000000 smartpredict-0.7.3/smartpredict/explainability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-24 08:58:10.000000 smartpredict-0.7.3/smartpredict/feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-24 08:58:10.000000 smartpredict-0.7.3/smartpredict/hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-24 08:58:10.000000 smartpredict-0.7.3/smartpredict/model_assessment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-24 08:58:10.000000 smartpredict-0.7.3/smartpredict/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-24 08:58:10.000000 smartpredict-0.7.3/smartpredict/supervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:58:10.000000 smartpredict-0.7.3/smartpredict/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:58:17.904413 smartpredict-0.7.3/smartpredict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-24 08:58:17.000000 smartpredict-0.7.3/smartpredict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-24 08:58:17.000000 smartpredict-0.7.3/smartpredict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:58:17.000000 smartpredict-0.7.3/smartpredict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-24 08:58:17.000000 smartpredict-0.7.3/smartpredict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 08:58:17.000000 smartpredict-0.7.3/smartpredict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:58:17.904413 smartpredict-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:58:10.000000 smartpredict-0.7.3/tests/test_smartpredict.py
```

### Comparing `smartpredict-0.7.2/CHANGELOG.md` & `smartpredict-0.7.3/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Changelog
 
-## [0.6.13] - 2024-05-24
+## [0.7.3] - 2024-05-24
+### Added
+- KernelExplainer in place of Explainer
+- Added .shape_values in place of .values
+
+## [0.6.13] - 2024-05-23
 ### Added
 - Added comprehensive model assessment metrics to evaluate machine learning models.
   - Accuracy
   - Precision
   - Recall
   - F1 Score
   - Confusion Matrix
```

### Comparing `smartpredict-0.7.2/PKG-INFO` & `smartpredict-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpredict
-Version: 0.7.2
+Version: 0.7.3
 Summary: An advanced machine learning library for effortless model training, evaluation, and selection.
 Home-page: https://github.com/SubaashNair/SmartPredict
 Author: Subashanan Nair
 Author-email: subaashnair12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -183,15 +183,20 @@
 ## License
 
 SmartPredict is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 
 # Changelog
 
-## [0.6.13] - 2024-05-24
+## [0.7.3] - 2024-05-24
+### Added
+- KernelExplainer in place of Explainer
+- Added .shape_values in place of .values
+
+## [0.6.13] - 2024-05-23
 ### Added
 - Added comprehensive model assessment metrics to evaluate machine learning models.
   - Accuracy
   - Precision
   - Recall
   - F1 Score
   - Confusion Matrix
```

### Comparing `smartpredict-0.7.2/README.md` & `smartpredict-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.2/setup.py` & `smartpredict-0.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 if readme_path.exists():
     long_description += readme_path.read_text(encoding='utf-8')
 if changelog_path.exists():
     long_description += "\n\n" + changelog_path.read_text(encoding='utf-8')
 
 setup(
     name="smartpredict",
-    version="0.7.2",  # Update the version number
+    version="0.7.3",  # Update the version number
     description="An advanced machine learning library for effortless model training, evaluation, and selection.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Subashanan Nair",
     author_email="subaashnair12@gmail.com",
     url="https://github.com/SubaashNair/SmartPredict",
     packages=find_packages(),
```

### Comparing `smartpredict-0.7.2/smartpredict/base.py` & `smartpredict-0.7.3/smartpredict/base.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.2/smartpredict/ensemble_methods.py` & `smartpredict-0.7.3/smartpredict/ensemble_methods.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.2/smartpredict/explainability.py` & `smartpredict-0.7.3/smartpredict/explainability.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,10 +14,10 @@
     model (estimator): The trained machine learning model.
     X_test (array-like): Testing features.
     y_test (array-like): Testing labels.
 
     Returns:
     None
     """
-    explainer = shap.Explainer(model)
-    shap_values = explainer(X_test)
+    explainer = shap.KernelExplainer(model)
+    shap_values = explainer.shap_values(X_test)
     shap.summary_plot(shap_values, X_test)
```

### Comparing `smartpredict-0.7.2/smartpredict/feature_engineering.py` & `smartpredict-0.7.3/smartpredict/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.2/smartpredict/hyperparameter_tuning.py` & `smartpredict-0.7.3/smartpredict/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.2/smartpredict/model_assessment.py` & `smartpredict-0.7.3/smartpredict/model_assessment.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.2/smartpredict/model_selection.py` & `smartpredict-0.7.3/smartpredict/model_selection.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.2/smartpredict/supervised.py` & `smartpredict-0.7.3/smartpredict/supervised.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.2/smartpredict.egg-info/PKG-INFO` & `smartpredict-0.7.3/smartpredict.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpredict
-Version: 0.7.2
+Version: 0.7.3
 Summary: An advanced machine learning library for effortless model training, evaluation, and selection.
 Home-page: https://github.com/SubaashNair/SmartPredict
 Author: Subashanan Nair
 Author-email: subaashnair12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -183,15 +183,20 @@
 ## License
 
 SmartPredict is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
 
 
 # Changelog
 
-## [0.6.13] - 2024-05-24
+## [0.7.3] - 2024-05-24
+### Added
+- KernelExplainer in place of Explainer
+- Added .shape_values in place of .values
+
+## [0.6.13] - 2024-05-23
 ### Added
 - Added comprehensive model assessment metrics to evaluate machine learning models.
   - Accuracy
   - Precision
   - Recall
   - F1 Score
   - Confusion Matrix
```

### Comparing `smartpredict-0.7.2/smartpredict.egg-info/SOURCES.txt` & `smartpredict-0.7.3/smartpredict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

