# Comparing `tmp/gf180_hdl21-6.0.0.tar.gz` & `tmp/gf180_hdl21-6.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gf180_hdl21-6.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gf180_hdl21-6.0.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gf180_hdl21-6.0.0.tar` & `gf180_hdl21-6.0.0rc0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1524 2024-05-24 16:13:54.035789 gf180_hdl21-6.0.0/LICENSE
--rw-r--r--   0        0        0      333 2023-07-11 14:50:48.444133 gf180_hdl21-6.0.0/gf180_hdl21/__init__.py
--rw-r--r--   0        0        0       51 2023-07-11 14:50:48.430997 gf180_hdl21-6.0.0/gf180_hdl21/digital_cells/__init__.py
--rw-r--r--   0        0        0    31678 2023-08-25 22:51:16.178369 gf180_hdl21-6.0.0/gf180_hdl21/digital_cells/nine_track.py
--rw-r--r--   0        0        0    31913 2023-08-25 22:51:16.178684 gf180_hdl21-6.0.0/gf180_hdl21/digital_cells/seven_track.py
--rw-r--r--   0        0        0     7628 2023-09-05 17:20:37.568737 gf180_hdl21-6.0.0/gf180_hdl21/pdk_data.py
--rw-r--r--   0        0        0    10993 2024-04-19 00:12:11.469581 gf180_hdl21-6.0.0/gf180_hdl21/pdk_logic.py
--rw-r--r--   0        0        0       26 2023-07-11 14:50:48.431754 gf180_hdl21-6.0.0/gf180_hdl21/primitives/__init__.py
--rw-r--r--   0        0        0     5717 2023-07-11 14:50:48.431827 gf180_hdl21-6.0.0/gf180_hdl21/primitives/prim_dicts.py
--rw-r--r--   0        0        0     2656 2023-07-11 14:50:48.431897 gf180_hdl21-6.0.0/gf180_hdl21/primitives/primitives.py
--rw-r--r--   0        0        0     1090 2023-07-11 14:50:48.432011 gf180_hdl21-6.0.0/gf180_hdl21/scripts/parse_digital_cells.py
--rw-r--r--   0        0        0     6353 2023-09-05 17:20:37.569069 gf180_hdl21-6.0.0/gf180_hdl21/test_netlists.py
--rw-r--r--   0        0        0     9468 2024-04-19 00:12:11.469925 gf180_hdl21-6.0.0/gf180_hdl21/test_pdk.py
--rw-r--r--   0        0        0     9984 2023-09-05 17:20:37.569231 gf180_hdl21-6.0.0/gf180_hdl21/test_site_sims.py
--rw-r--r--   0        0        0     1324 2024-05-24 17:12:01.381086 gf180_hdl21-6.0.0/pyproject.toml
--rw-r--r--   0        0        0    10487 2023-09-05 17:20:37.569565 gf180_hdl21-6.0.0/readme.md
--rw-r--r--   0        0        0    11630 1970-01-01 00:00:00.000000 gf180_hdl21-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2024-05-24 16:13:54.035789 gf180_hdl21-6.0.0rc0/LICENSE
+-rw-r--r--   0        0        0      333 2023-07-11 14:50:48.444133 gf180_hdl21-6.0.0rc0/gf180_hdl21/__init__.py
+-rw-r--r--   0        0        0       51 2023-07-11 14:50:48.430997 gf180_hdl21-6.0.0rc0/gf180_hdl21/digital_cells/__init__.py
+-rw-r--r--   0        0        0    31678 2023-08-25 22:51:16.178369 gf180_hdl21-6.0.0rc0/gf180_hdl21/digital_cells/nine_track.py
+-rw-r--r--   0        0        0    31913 2023-08-25 22:51:16.178684 gf180_hdl21-6.0.0rc0/gf180_hdl21/digital_cells/seven_track.py
+-rw-r--r--   0        0        0     7628 2023-09-05 17:20:37.568737 gf180_hdl21-6.0.0rc0/gf180_hdl21/pdk_data.py
+-rw-r--r--   0        0        0    10993 2024-04-19 00:12:11.469581 gf180_hdl21-6.0.0rc0/gf180_hdl21/pdk_logic.py
+-rw-r--r--   0        0        0       26 2023-07-11 14:50:48.431754 gf180_hdl21-6.0.0rc0/gf180_hdl21/primitives/__init__.py
+-rw-r--r--   0        0        0     5717 2023-07-11 14:50:48.431827 gf180_hdl21-6.0.0rc0/gf180_hdl21/primitives/prim_dicts.py
+-rw-r--r--   0        0        0     2656 2023-07-11 14:50:48.431897 gf180_hdl21-6.0.0rc0/gf180_hdl21/primitives/primitives.py
+-rw-r--r--   0        0        0     1090 2023-07-11 14:50:48.432011 gf180_hdl21-6.0.0rc0/gf180_hdl21/scripts/parse_digital_cells.py
+-rw-r--r--   0        0        0     6353 2023-09-05 17:20:37.569069 gf180_hdl21-6.0.0rc0/gf180_hdl21/test_netlists.py
+-rw-r--r--   0        0        0     9468 2024-04-19 00:12:11.469925 gf180_hdl21-6.0.0rc0/gf180_hdl21/test_pdk.py
+-rw-r--r--   0        0        0     9984 2023-09-05 17:20:37.569231 gf180_hdl21-6.0.0rc0/gf180_hdl21/test_site_sims.py
+-rw-r--r--   0        0        0     1330 2024-05-24 16:19:17.640385 gf180_hdl21-6.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    10487 2023-09-05 17:20:37.569565 gf180_hdl21-6.0.0rc0/readme.md
+-rw-r--r--   0        0        0    11636 1970-01-01 00:00:00.000000 gf180_hdl21-6.0.0rc0/PKG-INFO
```

### Comparing `gf180_hdl21-6.0.0/LICENSE` & `gf180_hdl21-6.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/gf180_hdl21/digital_cells/nine_track.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/digital_cells/nine_track.py`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/gf180_hdl21/digital_cells/seven_track.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/digital_cells/seven_track.py`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/gf180_hdl21/pdk_data.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/pdk_data.py`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/gf180_hdl21/pdk_logic.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/pdk_logic.py`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/gf180_hdl21/primitives/prim_dicts.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/primitives/prim_dicts.py`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/gf180_hdl21/primitives/primitives.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/primitives/primitives.py`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/gf180_hdl21/scripts/parse_digital_cells.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/scripts/parse_digital_cells.py`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/gf180_hdl21/test_netlists.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/test_netlists.py`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/gf180_hdl21/test_pdk.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/test_pdk.py`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/gf180_hdl21/test_site_sims.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/test_site_sims.py`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/pyproject.toml` & `gf180_hdl21-6.0.0rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "gf180-hdl21"
 description="Global Foundries 180nm MCU PDK Package for Hdl21"
-version = "6.0.0" # VLSIR_VERSION
+version = "6.0.0rc0" # VLSIR_VERSION
 dependencies = [
-  "hdl21>=6.0.0,<7", # VLSIR_VERSION
+  "hdl21>=6.0.0rc0,<7", # VLSIR_VERSION
 ]
 requires-python = ">=3.7, <3.13"
 maintainers = [
   {name = "Dan Fritchman", email = "dan@fritch.mn"},
 ]
 authors = [
   {name = "Dan Fritchman", email = "dan@fritch.mn"},
```

### Comparing `gf180_hdl21-6.0.0/readme.md` & `gf180_hdl21-6.0.0rc0/readme.md`

 * *Files identical despite different names*

### Comparing `gf180_hdl21-6.0.0/PKG-INFO` & `gf180_hdl21-6.0.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: gf180-hdl21
-Version: 6.0.0
+Version: 6.0.0rc0
 Summary: Global Foundries 180nm MCU PDK Package for Hdl21
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
+Requires-Dist: hdl21>=6.0.0rc0,<7
 Requires-Dist: pytest==7.1 ; extra == "dev"
 Requires-Dist: coverage ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pre-commit==2.20 ; extra == "dev"
 Requires-Dist: black==22.6 ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Project-URL: Bug Tracker, https://github.com/dan-fritchman/Hdl21/issues
```

