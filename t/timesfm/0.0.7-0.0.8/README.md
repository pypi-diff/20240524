# Comparing `tmp/timesfm-0.0.7.tar.gz` & `tmp/timesfm-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timesfm-0.0.7.tar", max compression
+gzip compressed data, was "timesfm-0.0.8.tar", max compression
```

## Comparing `timesfm-0.0.7.tar` & `timesfm-0.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11358 2024-05-24 11:50:27.805024 timesfm-0.0.7/LICENSE
--rw-r--r--   0        0        0     6210 2024-05-24 11:50:27.805024 timesfm-0.0.7/README.md
--rw-r--r--   0        0        0     1178 2024-05-24 11:50:38.309054 timesfm-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      734 2024-05-24 11:50:27.813024 timesfm-0.0.7/src/__init__.py
--rw-r--r--   0        0        0    15225 2024-05-24 11:50:27.813024 timesfm-0.0.7/src/patched_decoder.py
--rw-r--r--   0        0        0    20999 2024-05-24 11:50:27.813024 timesfm-0.0.7/src/timesfm.py
--rw-r--r--   0        0        0     7237 1970-01-01 00:00:00.000000 timesfm-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-24 11:55:25.725356 timesfm-0.0.8/LICENSE
+-rw-r--r--   0        0        0     6210 2024-05-24 11:55:25.725356 timesfm-0.0.8/README.md
+-rw-r--r--   0        0        0     1204 2024-05-24 11:55:34.953386 timesfm-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      734 2024-05-24 11:55:25.733356 timesfm-0.0.8/src/__init__.py
+-rw-r--r--   0        0        0    15225 2024-05-24 11:55:25.733356 timesfm-0.0.8/src/patched_decoder.py
+-rw-r--r--   0        0        0    20999 2024-05-24 11:55:25.733356 timesfm-0.0.8/src/timesfm.py
+-rw-r--r--   0        0        0     7284 1970-01-01 00:00:00.000000 timesfm-0.0.8/PKG-INFO
```

### Comparing `timesfm-0.0.7/LICENSE` & `timesfm-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.7/README.md` & `timesfm-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.7/pyproject.toml` & `timesfm-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "timesfm"
 packages = [
     { include = "*", from = "src" },
 ]
-version = "0.0.7"
+version = "0.0.8"
 description = "Open weights time-series foundation model from Google Research."
 authors = [
     "Rajat Sen <senrajat@google.com>",
     "Yichen Zhou <yichenzhou@google.com>",
     "Abhimanyu Das <abhidas@google.com>",
     "Petros Mol <pmol@google.com>",
     "Justin Güse <guese.justin@gmail.com>",
@@ -32,12 +32,13 @@
 python = ">=3.10,<3.11"
 einshape = ">=1.0.0"
 numpy = ">=1.26.4"
 pandas = ">=2.1.4"
 paxml = "1.4.0"
 jax = "0.4.26"
 jaxlib = "0.4.26"
+utilsforecast = "^0.1.10"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `timesfm-0.0.7/src/__init__.py` & `timesfm-0.0.8/src/__init__.py`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.7/src/patched_decoder.py` & `timesfm-0.0.8/src/patched_decoder.py`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.7/src/timesfm.py` & `timesfm-0.0.8/src/timesfm.py`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.7/PKG-INFO` & `timesfm-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timesfm
-Version: 0.0.7
+Version: 0.0.8
 Summary: Open weights time-series foundation model from Google Research.
 Home-page: https://github.com/google-research/timesfm
 Keywords: time series,timesfm,forecast,time series model
 Author: Rajat Sen
 Author-email: senrajat@google.com
 Requires-Python: >=3.10,<3.11
 Classifier: Environment :: Console
@@ -17,14 +17,15 @@
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: einshape (>=1.0.0)
 Requires-Dist: jax (==0.4.26)
 Requires-Dist: jaxlib (==0.4.26)
 Requires-Dist: numpy (>=1.26.4)
 Requires-Dist: pandas (>=2.1.4)
 Requires-Dist: paxml (==1.4.0)
+Requires-Dist: utilsforecast (>=0.1.10,<0.2.0)
 Project-URL: Repository, https://github.com/google-research/timesfm
 Description-Content-Type: text/markdown
 
 # TimesFM
 
 TimesFM  (Time Series Foundation Model) is a pretrained time-series foundation model developed by Google
 Research for time-series forecasting.
```

