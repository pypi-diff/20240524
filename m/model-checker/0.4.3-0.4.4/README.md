# Comparing `tmp/model_checker-0.4.3.tar.gz` & `tmp/model_checker-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_checker-0.4.3.tar", last modified: Fri May 24 20:07:50 2024, max compression
+gzip compressed data, was "model_checker-0.4.4.tar", last modified: Fri May 24 20:33:28 2024, max compression
```

## Comparing `model_checker-0.4.3.tar` & `model_checker-0.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:07:50.690985 model_checker-0.4.3/
--rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.4.3/LICENCE
--rw-r--r--   0 benjamin  (1000) users      (100)     9566 2024-05-24 20:07:50.690985 model_checker-0.4.3/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)     8781 2024-05-23 21:42:24.000000 model_checker-0.4.3/README.md
--rw-r--r--   0 benjamin  (1000) users      (100)     1007 2024-05-24 20:07:47.000000 model_checker-0.4.3/pyproject.toml
--rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-24 20:07:50.690985 model_checker-0.4.3/setup.cfg
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:07:50.688985 model_checker-0.4.3/src/
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:07:50.689985 model_checker-0.4.3/src/model_checker/
--rw-r--r--   0 benjamin  (1000) users      (100)      124 2024-05-24 20:07:47.000000 model_checker-0.4.3/src/model_checker/__init__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    13625 2024-05-23 17:20:26.000000 model_checker-0.4.3/src/model_checker/__main__.py
--rw-r--r--   0 benjamin  (1000) users      (100)    22895 2024-05-24 19:48:40.000000 model_checker-0.4.3/src/model_checker/model_definitions.py
--rw-r--r--   0 benjamin  (1000) users      (100)    26524 2024-05-24 17:55:48.000000 model_checker-0.4.3/src/model_checker/model_structure.py
--rw-r--r--   0 benjamin  (1000) users      (100)    28404 2024-05-24 17:38:50.000000 model_checker-0.4.3/src/model_checker/semantics.py
--rw-r--r--   0 benjamin  (1000) users      (100)     7836 2024-05-23 18:38:27.000000 model_checker-0.4.3/src/model_checker/syntax.py
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:07:50.690985 model_checker-0.4.3/src/model_checker.egg-info/
--rw-r--r--   0 benjamin  (1000) users      (100)     9566 2024-05-24 20:07:50.000000 model_checker-0.4.3/src/model_checker.egg-info/PKG-INFO
--rw-r--r--   0 benjamin  (1000) users      (100)      510 2024-05-24 20:07:50.000000 model_checker-0.4.3/src/model_checker.egg-info/SOURCES.txt
--rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-24 20:07:50.000000 model_checker-0.4.3/src/model_checker.egg-info/dependency_links.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-24 20:07:50.000000 model_checker-0.4.3/src/model_checker.egg-info/entry_points.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-24 20:07:50.000000 model_checker-0.4.3/src/model_checker.egg-info/requires.txt
--rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-24 20:07:50.000000 model_checker-0.4.3/src/model_checker.egg-info/top_level.txt
-drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:07:50.690985 model_checker-0.4.3/test/
--rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-23 04:07:12.000000 model_checker-0.4.3/test/test.py
--rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-23 04:07:12.000000 model_checker-0.4.3/test/test_examples.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:33:28.075412 model_checker-0.4.4/
+-rw-r--r--   0 benjamin  (1000) users      (100)     1064 2024-05-08 20:11:06.000000 model_checker-0.4.4/LICENCE
+-rw-r--r--   0 benjamin  (1000) users      (100)     9566 2024-05-24 20:33:28.075412 model_checker-0.4.4/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)     8781 2024-05-23 21:42:24.000000 model_checker-0.4.4/README.md
+-rw-r--r--   0 benjamin  (1000) users      (100)     1007 2024-05-24 20:33:24.000000 model_checker-0.4.4/pyproject.toml
+-rw-r--r--   0 benjamin  (1000) users      (100)       38 2024-05-24 20:33:28.075412 model_checker-0.4.4/setup.cfg
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:33:28.074412 model_checker-0.4.4/src/
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:33:28.075412 model_checker-0.4.4/src/model_checker/
+-rw-r--r--   0 benjamin  (1000) users      (100)      124 2024-05-24 20:33:24.000000 model_checker-0.4.4/src/model_checker/__init__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    13625 2024-05-23 17:20:26.000000 model_checker-0.4.4/src/model_checker/__main__.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    22895 2024-05-24 19:48:40.000000 model_checker-0.4.4/src/model_checker/model_definitions.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    26524 2024-05-24 17:55:48.000000 model_checker-0.4.4/src/model_checker/model_structure.py
+-rw-r--r--   0 benjamin  (1000) users      (100)    28404 2024-05-24 17:38:50.000000 model_checker-0.4.4/src/model_checker/semantics.py
+-rw-r--r--   0 benjamin  (1000) users      (100)     7836 2024-05-23 18:38:27.000000 model_checker-0.4.4/src/model_checker/syntax.py
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:33:28.075412 model_checker-0.4.4/src/model_checker.egg-info/
+-rw-r--r--   0 benjamin  (1000) users      (100)     9566 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/PKG-INFO
+-rw-r--r--   0 benjamin  (1000) users      (100)      510 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)        1 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       62 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/entry_points.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       10 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/requires.txt
+-rw-r--r--   0 benjamin  (1000) users      (100)       14 2024-05-24 20:33:28.000000 model_checker-0.4.4/src/model_checker.egg-info/top_level.txt
+drwxr-xr-x   0 benjamin  (1000) users      (100)        0 2024-05-24 20:33:28.075412 model_checker-0.4.4/test/
+-rw-r--r--   0 benjamin  (1000) users      (100)     2985 2024-05-23 04:07:12.000000 model_checker-0.4.4/test/test.py
+-rw-r--r--   0 benjamin  (1000) users      (100)      330 2024-05-23 04:07:12.000000 model_checker-0.4.4/test/test_examples.py
```

### Comparing `model_checker-0.4.3/LICENCE` & `model_checker-0.4.4/LICENCE`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.3/PKG-INFO` & `model_checker-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.4.3
+Version: 0.4.4
 Summary: A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,logic,counterfactuals,modality,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.4.3/README.md` & `model_checker-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.3/pyproject.toml` & `model_checker-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-checker"
-version = "0.4.3"
+version = "0.4.4"
 description = "A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators."
 authors = [
     { name = "Benjamin Brast-McKie", email = "benbrastmckie@gmail.com" },
     { name = "Miguel Buitrago", email = "mbuit82@gmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
```

### Comparing `model_checker-0.4.3/src/model_checker/__main__.py` & `model_checker-0.4.4/src/model_checker/__main__.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.3/src/model_checker/model_definitions.py` & `model_checker-0.4.4/src/model_checker/model_definitions.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.3/src/model_checker/model_structure.py` & `model_checker-0.4.4/src/model_checker/model_structure.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.3/src/model_checker/semantics.py` & `model_checker-0.4.4/src/model_checker/semantics.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.3/src/model_checker/syntax.py` & `model_checker-0.4.4/src/model_checker/syntax.py`

 * *Files identical despite different names*

### Comparing `model_checker-0.4.3/src/model_checker.egg-info/PKG-INFO` & `model_checker-0.4.4/src/model_checker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-checker
-Version: 0.4.3
+Version: 0.4.4
 Summary: A hyperintensional theorem prover for modal, counterfactual conditional, constitutive explanatory, and extensional operators.
 Author-email: Benjamin Brast-McKie <benbrastmckie@gmail.com>, Miguel Buitrago <mbuit82@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/benbrastmckie/ModelChecker
 Project-URL: Issues, https://github.com/benbrastmckie/ModelChecker/issues
 Keywords: semantics,Z3,logic,counterfactuals,modality,model checker,theorem prover,hyperintensionality
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `model_checker-0.4.3/test/test.py` & `model_checker-0.4.4/test/test.py`

 * *Files identical despite different names*

