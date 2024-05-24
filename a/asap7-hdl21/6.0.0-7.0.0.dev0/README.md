# Comparing `tmp/asap7_hdl21-6.0.0.tar.gz` & `tmp/asap7_hdl21-7.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asap7_hdl21-6.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "asap7_hdl21-7.0.0.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `asap7_hdl21-6.0.0.tar` & `asap7_hdl21-7.0.0.dev0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1524 2024-05-24 16:13:54.035628 asap7_hdl21-6.0.0/LICENSE
--rw-r--r--   0        0        0      315 2023-07-11 14:50:48.444752 asap7_hdl21-6.0.0/asap7_hdl21/__init__.py
--rw-r--r--   0        0        0     3985 2023-07-11 14:50:48.444618 asap7_hdl21-6.0.0/asap7_hdl21/pdk.py
--rw-r--r--   0        0        0      180 2023-07-11 14:50:48.444416 asap7_hdl21-6.0.0/asap7_hdl21/test_pdk.py
--rw-r--r--   0        0        0     1298 2024-05-24 17:12:01.379907 asap7_hdl21-6.0.0/pyproject.toml
--rw-r--r--   0        0        0       19 2024-05-24 17:18:05.507739 asap7_hdl21-6.0.0/readme.md
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 asap7_hdl21-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2024-05-24 16:13:54.035628 asap7_hdl21-7.0.0.dev0/LICENSE
+-rw-r--r--   0        0        0      315 2023-07-11 14:50:48.444752 asap7_hdl21-7.0.0.dev0/asap7_hdl21/__init__.py
+-rw-r--r--   0        0        0     3985 2023-07-11 14:50:48.444618 asap7_hdl21-7.0.0.dev0/asap7_hdl21/pdk.py
+-rw-r--r--   0        0        0      180 2023-07-11 14:50:48.444416 asap7_hdl21-7.0.0.dev0/asap7_hdl21/test_pdk.py
+-rw-r--r--   0        0        0     1308 2024-05-24 17:33:41.212550 asap7_hdl21-7.0.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0       19 2024-05-24 17:18:05.507739 asap7_hdl21-7.0.0.dev0/readme.md
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 asap7_hdl21-7.0.0.dev0/PKG-INFO
```

### Comparing `asap7_hdl21-6.0.0/LICENSE` & `asap7_hdl21-7.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `asap7_hdl21-6.0.0/asap7_hdl21/pdk.py` & `asap7_hdl21-7.0.0.dev0/asap7_hdl21/pdk.py`

 * *Files identical despite different names*

### Comparing `asap7_hdl21-6.0.0/pyproject.toml` & `asap7_hdl21-7.0.0.dev0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "asap7-hdl21"
 description = "ASAP7 PDK Package for Hdl21"
-version = "6.0.0" # VLSIR_VERSION
+version = "7.0.0.dev0" # VLSIR_VERSION
 dependencies = [
-  "hdl21>=6.0.0,<7", # VLSIR_VERSION
+  "hdl21>=7.0.0.dev0,<7", # VLSIR_VERSION
 ]
 requires-python = ">=3.7, <3.13"
 maintainers = [{ name = "Dan Fritchman", email = "dan@fritch.mn" }]
 authors = [
   { name = "Dan Fritchman", email = "dan@fritch.mn" },
   { name = "Thomas Pluck" },
   { name = "Curtis Mayberry", email = "Curtisma3@gmail.com" },
```

### Comparing `asap7_hdl21-6.0.0/PKG-INFO` & `asap7_hdl21-7.0.0.dev0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: asap7-hdl21
-Version: 6.0.0
+Version: 7.0.0.dev0
 Summary: ASAP7 PDK Package for Hdl21
 Keywords: PDK,EDA,analog,circuit
 Author: Thomas Pluck
 Author-email: Dan Fritchman <dan@fritch.mn>, Curtis Mayberry <Curtisma3@gmail.com>
 Maintainer-email: Dan Fritchman <dan@fritch.mn>
 Requires-Python: >=3.7, <3.13
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Requires-Dist: hdl21>=6.0.0,<7
+Requires-Dist: hdl21>=7.0.0.dev0,<7
 Requires-Dist: pytest==7.1 ; extra == "dev"
 Requires-Dist: coverage ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pre-commit==2.20 ; extra == "dev"
 Requires-Dist: black==22.6 ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Project-URL: Bug Tracker, https://github.com/dan-fritchman/Hdl21/issues
```

