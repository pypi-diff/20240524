# Comparing `tmp/timesfm-0.0.5.tar.gz` & `tmp/timesfm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timesfm-0.0.5.tar", max compression
+gzip compressed data, was "timesfm-0.0.6.tar", max compression
```

## Comparing `timesfm-0.0.5.tar` & `timesfm-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    11358 2024-05-24 11:45:39.859973 timesfm-0.0.5/LICENSE
--rw-r--r--   0        0        0     6210 2024-05-24 11:45:39.859973 timesfm-0.0.5/README.md
--rw-r--r--   0        0        0     1160 2024-05-24 11:45:51.036089 timesfm-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    15225 2024-05-24 11:45:39.867973 timesfm-0.0.5/src/patched_decoder.py
--rw-r--r--   0        0        0    20999 2024-05-24 11:45:39.867973 timesfm-0.0.5/src/timesfm.py
--rw-r--r--   0        0        0     7204 1970-01-01 00:00:00.000000 timesfm-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-24 11:47:36.668726 timesfm-0.0.6/LICENSE
+-rw-r--r--   0        0        0     6210 2024-05-24 11:47:36.668726 timesfm-0.0.6/README.md
+-rw-r--r--   0        0        0     1160 2024-05-24 11:47:48.100872 timesfm-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      734 2024-05-24 11:47:36.676726 timesfm-0.0.6/src/__init__.py
+-rw-r--r--   0        0        0    15225 2024-05-24 11:47:36.676726 timesfm-0.0.6/src/patched_decoder.py
+-rw-r--r--   0        0        0    20999 2024-05-24 11:47:36.676726 timesfm-0.0.6/src/timesfm.py
+-rw-r--r--   0        0        0     7204 1970-01-01 00:00:00.000000 timesfm-0.0.6/PKG-INFO
```

### Comparing `timesfm-0.0.5/LICENSE` & `timesfm-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.5/README.md` & `timesfm-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.5/pyproject.toml` & `timesfm-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "timesfm"
 packages = [
     { include = "*", from = "src" },
 ]
-version = "0.0.5"
+version = "0.0.6"
 description = "Open weights time-series foundation model from Google Research."
 authors = [
     "Rajat Sen <senrajat@google.com>",
     "Yichen Zhou <yichenzhou@google.com>",
     "Abhimanyu Das <abhidas@google.com>",
     "Petros Mol <pmol@google.com>",
     "Justin Güse <guese.justin@gmail.com>",
```

### Comparing `timesfm-0.0.5/src/patched_decoder.py` & `timesfm-0.0.6/src/patched_decoder.py`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.5/src/timesfm.py` & `timesfm-0.0.6/src/timesfm.py`

 * *Files identical despite different names*

### Comparing `timesfm-0.0.5/PKG-INFO` & `timesfm-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timesfm
-Version: 0.0.5
+Version: 0.0.6
 Summary: Open weights time-series foundation model from Google Research.
 Home-page: https://github.com/google-research/timesfm
 Keywords: time series,timesfm,forecast,time series model
 Author: Rajat Sen
 Author-email: senrajat@google.com
 Requires-Python: >=3.10,<3.11
 Classifier: Environment :: Console
```

