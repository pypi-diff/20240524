# Comparing `tmp/timesfm-0.0.1.tar.gz` & `tmp/timesfm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timesfm-0.0.1.tar", max compression
+gzip compressed data, was "timesfm-0.0.3.tar", max compression
```

## Comparing `timesfm-0.0.1.tar` & `timesfm-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11358 2024-05-24 10:40:26.588397 timesfm-0.0.1/LICENSE
--rw-r--r--   0        0        0     6210 2024-05-24 10:40:26.588554 timesfm-0.0.1/README.md
--rw-r--r--   0        0        0     1092 2024-05-24 10:52:49.376855 timesfm-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    20999 2024-05-24 10:40:26.594212 timesfm-0.0.1/src/timesfm.py
--rw-r--r--   0        0        0     7173 1970-01-01 00:00:00.000000 timesfm-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-24 11:39:36.925411 timesfm-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6210 2024-05-24 11:39:36.925411 timesfm-0.0.3/README.md
+-rw-r--r--   0        0        0     1108 2024-05-24 11:39:52.193625 timesfm-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    20999 2024-05-24 11:39:36.929411 timesfm-0.0.3/src/timesfm.py
+-rw-r--r--   0        0        0     7204 1970-01-01 00:00:00.000000 timesfm-0.0.3/PKG-INFO
```

### Comparing `timesfm-0.0.1/LICENSE` & `timesfm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.1/README.md` & `timesfm-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.1/pyproject.toml` & `timesfm-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "timesfm"
-version = "0.0.1"
+version = "0.0.3"
 description = "Open weights time-series foundation model from Google Research."
 authors = [
     "Rajat Sen <senrajat@google.com>",
     "Yichen Zhou <yichenzhou@google.com>",
     "Abhimanyu Das <abhidas@google.com>",
     "Petros Mol <pmol@google.com>",
     "Justin Güse <guese.justin@gmail.com>",
@@ -24,15 +24,16 @@
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 einshape = ">=1.0.0"
-jax = "0.4.26"
 numpy = ">=1.26.4"
 pandas = ">=2.1.4"
+paxml = "1.4.0"
+jax = "0.4.26"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `timesfm-0.0.1/src/timesfm.py` & `timesfm-0.0.3/src/timesfm.py`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.1/PKG-INFO` & `timesfm-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timesfm
-Version: 0.0.1
+Version: 0.0.3
 Summary: Open weights time-series foundation model from Google Research.
 Home-page: https://github.com/google-research/timesfm
 Keywords: time series,timesfm,forecast,time series model
 Author: Rajat Sen
 Author-email: senrajat@google.com
 Requires-Python: >=3.10,<3.11
 Classifier: Environment :: Console
@@ -15,14 +15,15 @@
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: einshape (>=1.0.0)
 Requires-Dist: jax (==0.4.26)
 Requires-Dist: numpy (>=1.26.4)
 Requires-Dist: pandas (>=2.1.4)
+Requires-Dist: paxml (==1.4.0)
 Project-URL: Repository, https://github.com/google-research/timesfm
 Description-Content-Type: text/markdown
 
 # TimesFM
 
 TimesFM  (Time Series Foundation Model) is a pretrained time-series foundation model developed by Google
 Research for time-series forecasting.
```

