# Comparing `tmp/smartpredict-0.7.5.tar.gz` & `tmp/smartpredict-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartpredict-0.7.5.tar", last modified: Fri May 24 09:29:02 2024, max compression
+gzip compressed data, was "smartpredict-0.7.6.tar", last modified: Fri May 24 09:36:53 2024, max compression
```

## Comparing `smartpredict-0.7.5.tar` & `smartpredict-0.7.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:29:02.189566 smartpredict-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-24 09:28:58.000000 smartpredict-0.7.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-24 09:28:58.000000 smartpredict-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-24 09:29:02.189566 smartpredict-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-24 09:28:58.000000 smartpredict-0.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-24 09:28:58.000000 smartpredict-0.7.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 09:29:02.189566 smartpredict-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-24 09:28:58.000000 smartpredict-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:29:02.189566 smartpredict-0.7.5/smartpredict/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-24 09:28:58.000000 smartpredict-0.7.5/smartpredict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-24 09:28:58.000000 smartpredict-0.7.5/smartpredict/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-24 09:28:58.000000 smartpredict-0.7.5/smartpredict/ensemble_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-24 09:28:58.000000 smartpredict-0.7.5/smartpredict/explainability.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-24 09:28:58.000000 smartpredict-0.7.5/smartpredict/feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-24 09:28:58.000000 smartpredict-0.7.5/smartpredict/hyperparameter_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-24 09:28:58.000000 smartpredict-0.7.5/smartpredict/model_assessment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-24 09:28:58.000000 smartpredict-0.7.5/smartpredict/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-24 09:28:58.000000 smartpredict-0.7.5/smartpredict/supervised.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:28:58.000000 smartpredict-0.7.5/smartpredict/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:29:02.189566 smartpredict-0.7.5/smartpredict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-24 09:29:02.000000 smartpredict-0.7.5/smartpredict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-24 09:29:02.000000 smartpredict-0.7.5/smartpredict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:29:02.000000 smartpredict-0.7.5/smartpredict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-24 09:29:02.000000 smartpredict-0.7.5/smartpredict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 09:29:02.000000 smartpredict-0.7.5/smartpredict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:29:02.189566 smartpredict-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:28:58.000000 smartpredict-0.7.5/tests/test_smartpredict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:36:53.636915 smartpredict-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-24 09:36:50.000000 smartpredict-0.7.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-24 09:36:50.000000 smartpredict-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-24 09:36:53.636915 smartpredict-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-24 09:36:50.000000 smartpredict-0.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-24 09:36:50.000000 smartpredict-0.7.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 09:36:53.640915 smartpredict-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-24 09:36:50.000000 smartpredict-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:36:53.636915 smartpredict-0.7.6/smartpredict/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-24 09:36:50.000000 smartpredict-0.7.6/smartpredict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-24 09:36:50.000000 smartpredict-0.7.6/smartpredict/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-24 09:36:50.000000 smartpredict-0.7.6/smartpredict/ensemble_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-24 09:36:50.000000 smartpredict-0.7.6/smartpredict/explainability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-24 09:36:50.000000 smartpredict-0.7.6/smartpredict/feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-24 09:36:50.000000 smartpredict-0.7.6/smartpredict/hyperparameter_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-24 09:36:50.000000 smartpredict-0.7.6/smartpredict/model_assessment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-24 09:36:50.000000 smartpredict-0.7.6/smartpredict/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-24 09:36:50.000000 smartpredict-0.7.6/smartpredict/supervised.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:36:50.000000 smartpredict-0.7.6/smartpredict/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:36:53.636915 smartpredict-0.7.6/smartpredict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-24 09:36:53.000000 smartpredict-0.7.6/smartpredict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-24 09:36:53.000000 smartpredict-0.7.6/smartpredict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:36:53.000000 smartpredict-0.7.6/smartpredict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-24 09:36:53.000000 smartpredict-0.7.6/smartpredict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 09:36:53.000000 smartpredict-0.7.6/smartpredict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:36:53.636915 smartpredict-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:36:50.000000 smartpredict-0.7.6/tests/test_smartpredict.py
```

### Comparing `smartpredict-0.7.5/CHANGELOG.md` & `smartpredict-0.7.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.5/PKG-INFO` & `smartpredict-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpredict
-Version: 0.7.5
+Version: 0.7.6
 Summary: An advanced machine learning library for effortless model training, evaluation, and selection.
 Home-page: https://github.com/SubaashNair/SmartPredict
 Author: Subashanan Nair
 Author-email: subaashnair12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smartpredict-0.7.5/README.md` & `smartpredict-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.5/setup.py` & `smartpredict-0.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 if readme_path.exists():
     long_description += readme_path.read_text(encoding='utf-8')
 if changelog_path.exists():
     long_description += "\n\n" + changelog_path.read_text(encoding='utf-8')
 
 setup(
     name="smartpredict",
-    version="0.7.5",  # Update the version number
+    version="0.7.6",  # Update the version number
     description="An advanced machine learning library for effortless model training, evaluation, and selection.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Subashanan Nair",
     author_email="subaashnair12@gmail.com",
     url="https://github.com/SubaashNair/SmartPredict",
     packages=find_packages(),
```

### Comparing `smartpredict-0.7.5/smartpredict/base.py` & `smartpredict-0.7.6/smartpredict/base.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.5/smartpredict/ensemble_methods.py` & `smartpredict-0.7.6/smartpredict/ensemble_methods.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.5/smartpredict/explainability.py` & `smartpredict-0.7.6/smartpredict/explainability.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.5/smartpredict/feature_engineering.py` & `smartpredict-0.7.6/smartpredict/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.5/smartpredict/hyperparameter_tuning.py` & `smartpredict-0.7.6/smartpredict/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.5/smartpredict/model_assessment.py` & `smartpredict-0.7.6/smartpredict/model_assessment.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.5/smartpredict/model_selection.py` & `smartpredict-0.7.6/smartpredict/model_selection.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.5/smartpredict/supervised.py` & `smartpredict-0.7.6/smartpredict/supervised.py`

 * *Files identical despite different names*

### Comparing `smartpredict-0.7.5/smartpredict.egg-info/PKG-INFO` & `smartpredict-0.7.6/smartpredict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpredict
-Version: 0.7.5
+Version: 0.7.6
 Summary: An advanced machine learning library for effortless model training, evaluation, and selection.
 Home-page: https://github.com/SubaashNair/SmartPredict
 Author: Subashanan Nair
 Author-email: subaashnair12@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `smartpredict-0.7.5/smartpredict.egg-info/SOURCES.txt` & `smartpredict-0.7.6/smartpredict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

