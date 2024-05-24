# Comparing `tmp/skope_rules_temp-0.2.4.tar.gz` & `tmp/skope_rules_temp-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skope_rules_temp-0.2.4.tar", max compression
+gzip compressed data, was "skope_rules_temp-0.2.5.tar", max compression
```

## Comparing `skope_rules_temp-0.2.4.tar` & `skope_rules_temp-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      428 2024-03-05 21:27:15.152010 skope_rules_temp-0.2.4/AUTHORS.rst
--rw-r--r--   0        0        0     1551 2024-03-05 21:27:15.152121 skope_rules_temp-0.2.4/COPYING
--rw-r--r--   0        0        0     5465 2024-03-05 21:27:15.152351 skope_rules_temp-0.2.4/README.md
--rw-r--r--   0        0        0      485 2024-04-25 13:55:18.381102 skope_rules_temp-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      115 2024-03-05 21:27:15.158029 skope_rules_temp-0.2.4/src/skope_rules_temp/__init__.py
--rw-r--r--   0        0        0       74 2024-03-05 21:27:15.158175 skope_rules_temp-0.2.4/src/skope_rules_temp/datasets/__init__.py
--rw-r--r--   0        0        0     1435 2024-03-05 21:27:15.158300 skope_rules_temp-0.2.4/src/skope_rules_temp/datasets/credit_data.py
--rw-r--r--   0        0        0     2352 2024-03-05 21:27:15.158409 skope_rules_temp-0.2.4/src/skope_rules_temp/rule.py
--rw-r--r--   0        0        0    27240 2024-03-05 21:27:15.158638 skope_rules_temp-0.2.4/src/skope_rules_temp/skope_rules.py
--rw-r--r--   0        0        0        0 2024-03-05 21:27:15.158776 skope_rules_temp-0.2.4/src/skope_rules_temp/tests/__init__.py
--rw-r--r--   0        0        0      277 2024-03-05 21:27:15.158910 skope_rules_temp-0.2.4/src/skope_rules_temp/tests/test_common.py
--rw-r--r--   0        0        0     1872 2024-03-05 21:27:15.159076 skope_rules_temp-0.2.4/src/skope_rules_temp/tests/test_rule.py
--rw-r--r--   0        0        0     8074 2024-03-05 21:27:15.159227 skope_rules_temp-0.2.4/src/skope_rules_temp/tests/test_skope_rules.py
--rw-r--r--   0        0        0     6205 1970-01-01 00:00:00.000000 skope_rules_temp-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      428 2024-03-05 21:27:15.152010 skope_rules_temp-0.2.5/AUTHORS.rst
+-rw-r--r--   0        0        0     1551 2024-03-05 21:27:15.152121 skope_rules_temp-0.2.5/COPYING
+-rw-r--r--   0        0        0     5465 2024-03-05 21:27:15.152351 skope_rules_temp-0.2.5/README.md
+-rw-r--r--   0        0        0      485 2024-05-24 11:17:46.355645 skope_rules_temp-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      115 2024-03-05 21:27:15.158029 skope_rules_temp-0.2.5/src/skope_rules_temp/__init__.py
+-rw-r--r--   0        0        0       74 2024-03-05 21:27:15.158175 skope_rules_temp-0.2.5/src/skope_rules_temp/datasets/__init__.py
+-rw-r--r--   0        0        0     1435 2024-03-05 21:27:15.158300 skope_rules_temp-0.2.5/src/skope_rules_temp/datasets/credit_data.py
+-rw-r--r--   0        0        0     2352 2024-03-05 21:27:15.158409 skope_rules_temp-0.2.5/src/skope_rules_temp/rule.py
+-rw-r--r--   0        0        0    27233 2024-05-24 11:15:23.243436 skope_rules_temp-0.2.5/src/skope_rules_temp/skope_rules.py
+-rw-r--r--   0        0        0        0 2024-03-05 21:27:15.158776 skope_rules_temp-0.2.5/src/skope_rules_temp/tests/__init__.py
+-rw-r--r--   0        0        0      277 2024-03-05 21:27:15.158910 skope_rules_temp-0.2.5/src/skope_rules_temp/tests/test_common.py
+-rw-r--r--   0        0        0     1872 2024-03-05 21:27:15.159076 skope_rules_temp-0.2.5/src/skope_rules_temp/tests/test_rule.py
+-rw-r--r--   0        0        0     8074 2024-03-05 21:27:15.159227 skope_rules_temp-0.2.5/src/skope_rules_temp/tests/test_skope_rules.py
+-rw-r--r--   0        0        0      849 2024-05-24 11:15:23.246200 skope_rules_temp-0.2.5/src/skope_rules_temp/utils.py
+-rw-r--r--   0        0        0     6205 1970-01-01 00:00:00.000000 skope_rules_temp-0.2.5/PKG-INFO
```

### Comparing `skope_rules_temp-0.2.4/COPYING` & `skope_rules_temp-0.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.4/README.md` & `skope_rules_temp-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.4/src/skope_rules_temp/datasets/credit_data.py` & `skope_rules_temp-0.2.5/src/skope_rules_temp/datasets/credit_data.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.4/src/skope_rules_temp/rule.py` & `skope_rules_temp-0.2.5/src/skope_rules_temp/rule.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.4/src/skope_rules_temp/skope_rules.py` & `skope_rules_temp-0.2.5/src/skope_rules_temp/skope_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import pandas
 import numbers
 from warnings import warn
 
 from sklearn.base import BaseEstimator
 from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
 from sklearn.utils.multiclass import check_classification_targets
-from sklearn.utils import indices_to_mask
 from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 from sklearn.ensemble import BaggingClassifier, BaggingRegressor
 from sklearn.tree import _tree
 
+from .utils import indices_to_mask
 from .rule import Rule, replace_feature_name
 
 INTEGER_TYPES = (numbers.Integral, np.integer)
 BASE_FEATURE_NAME = "__C__"
 
 
 class SkopeRules(BaseEstimator):
```

### Comparing `skope_rules_temp-0.2.4/src/skope_rules_temp/tests/test_rule.py` & `skope_rules_temp-0.2.5/src/skope_rules_temp/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.4/src/skope_rules_temp/tests/test_skope_rules.py` & `skope_rules_temp-0.2.5/src/skope_rules_temp/tests/test_skope_rules.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.4/PKG-INFO` & `skope_rules_temp-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skope-rules-temp
-Version: 0.2.4
+Version: 0.2.5
 Summary: Fork of https://github.com/scikit-learn-contrib/skope-rules
 Author: Pierre Hulot
 Author-email: pierre@ai-vidence.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

