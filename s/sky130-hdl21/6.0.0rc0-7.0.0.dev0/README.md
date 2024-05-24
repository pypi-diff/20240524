# Comparing `tmp/sky130_hdl21-6.0.0rc0.tar.gz` & `tmp/sky130_hdl21-7.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sky130_hdl21-6.0.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sky130_hdl21-7.0.0.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sky130_hdl21-6.0.0rc0.tar` & `sky130_hdl21-7.0.0.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1524 2024-05-24 16:13:54.035862 sky130_hdl21-6.0.0rc0/LICENSE
--rw-r--r--   0        0        0     1321 2024-05-24 16:20:26.505731 sky130_hdl21-6.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0    20435 2023-09-05 17:20:37.569826 sky130_hdl21-6.0.0rc0/readme.md
--rw-r--r--   0        0        0      333 2023-07-11 14:50:48.432908 sky130_hdl21-6.0.0rc0/sky130_hdl21/__init__.py
--rw-r--r--   0        0        0      153 2023-07-11 14:50:48.433006 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/__init__.py
--rw-r--r--   0        0        0    61602 2023-08-25 22:51:16.179401 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/high_density.py
--rw-r--r--   0        0        0    53672 2023-08-25 22:51:16.179861 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/high_speed.py
--rw-r--r--   0        0        0    50419 2023-08-25 22:51:16.180189 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_leakage.py
--rw-r--r--   0        0        0   101450 2023-08-25 22:51:16.180523 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_power.py
--rw-r--r--   0        0        0    54196 2023-08-25 22:51:16.180834 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_speed.py
--rw-r--r--   0        0        0    54623 2023-08-25 22:51:16.181132 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/medium_speed.py
--rw-r--r--   0        0        0    16083 2024-04-19 00:12:11.470278 sky130_hdl21-6.0.0rc0/sky130_hdl21/pdk_data.py
--rw-r--r--   0        0        0    13536 2024-04-19 00:12:11.470616 sky130_hdl21-6.0.0rc0/sky130_hdl21/pdk_logic.py
--rw-r--r--   0        0        0       26 2023-07-11 14:50:48.434932 sky130_hdl21-6.0.0rc0/sky130_hdl21/primitives/__init__.py
--rw-r--r--   0        0        0    15069 2024-04-19 00:12:11.470940 sky130_hdl21-6.0.0rc0/sky130_hdl21/primitives/prim_dicts.py
--rw-r--r--   0        0        0     7888 2024-04-19 00:12:11.471254 sky130_hdl21-6.0.0rc0/sky130_hdl21/primitives/primitives.py
--rw-r--r--   0        0        0     7190 2023-09-05 17:20:37.570542 sky130_hdl21-6.0.0rc0/sky130_hdl21/test_netlists.py
--rw-r--r--   0        0        0    13614 2023-07-11 14:50:48.443513 sky130_hdl21-6.0.0rc0/sky130_hdl21/test_pdk.py
--rw-r--r--   0        0        0    21806 2023-07-11 14:50:48.443308 sky130_hdl21-6.0.0rc0/sky130_hdl21/test_site_sims.py
--rw-r--r--   0        0        0    21574 1970-01-01 00:00:00.000000 sky130_hdl21-6.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2024-05-24 16:13:54.035862 sky130_hdl21-7.0.0.dev0/LICENSE
+-rw-r--r--   0        0        0     1325 2024-05-24 17:33:41.212601 sky130_hdl21-7.0.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    20435 2023-09-05 17:20:37.569826 sky130_hdl21-7.0.0.dev0/readme.md
+-rw-r--r--   0        0        0      333 2023-07-11 14:50:48.432908 sky130_hdl21-7.0.0.dev0/sky130_hdl21/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-11 14:50:48.433006 sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/__init__.py
+-rw-r--r--   0        0        0    61602 2023-08-25 22:51:16.179401 sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/high_density.py
+-rw-r--r--   0        0        0    53672 2023-08-25 22:51:16.179861 sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/high_speed.py
+-rw-r--r--   0        0        0    50419 2023-08-25 22:51:16.180189 sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/low_leakage.py
+-rw-r--r--   0        0        0   101450 2023-08-25 22:51:16.180523 sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/low_power.py
+-rw-r--r--   0        0        0    54196 2023-08-25 22:51:16.180834 sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/low_speed.py
+-rw-r--r--   0        0        0    54623 2023-08-25 22:51:16.181132 sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/medium_speed.py
+-rw-r--r--   0        0        0    16083 2024-04-19 00:12:11.470278 sky130_hdl21-7.0.0.dev0/sky130_hdl21/pdk_data.py
+-rw-r--r--   0        0        0    13536 2024-04-19 00:12:11.470616 sky130_hdl21-7.0.0.dev0/sky130_hdl21/pdk_logic.py
+-rw-r--r--   0        0        0       26 2023-07-11 14:50:48.434932 sky130_hdl21-7.0.0.dev0/sky130_hdl21/primitives/__init__.py
+-rw-r--r--   0        0        0    15069 2024-04-19 00:12:11.470940 sky130_hdl21-7.0.0.dev0/sky130_hdl21/primitives/prim_dicts.py
+-rw-r--r--   0        0        0     7888 2024-04-19 00:12:11.471254 sky130_hdl21-7.0.0.dev0/sky130_hdl21/primitives/primitives.py
+-rw-r--r--   0        0        0     7190 2023-09-05 17:20:37.570542 sky130_hdl21-7.0.0.dev0/sky130_hdl21/test_netlists.py
+-rw-r--r--   0        0        0    13614 2023-07-11 14:50:48.443513 sky130_hdl21-7.0.0.dev0/sky130_hdl21/test_pdk.py
+-rw-r--r--   0        0        0    21806 2023-07-11 14:50:48.443308 sky130_hdl21-7.0.0.dev0/sky130_hdl21/test_site_sims.py
+-rw-r--r--   0        0        0    21578 1970-01-01 00:00:00.000000 sky130_hdl21-7.0.0.dev0/PKG-INFO
```

### Comparing `sky130_hdl21-6.0.0rc0/LICENSE` & `sky130_hdl21-7.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/pyproject.toml` & `sky130_hdl21-7.0.0.dev0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "sky130-hdl21"
 description="SkyWater 130nm PDK Package for Hdl21"
-version = "6.0.0rc0" # VLSIR_VERSION
+version = "7.0.0.dev0" # VLSIR_VERSION
 dependencies = [
-  "hdl21>=6.0.0rc0,<7", # VLSIR_VERSION
+  "hdl21>=7.0.0.dev0,<7", # VLSIR_VERSION
 ]
 requires-python = ">=3.7, <3.13"
 maintainers = [
   {name = "Dan Fritchman", email = "dan@fritch.mn"},
 ]
 authors = [
   {name = "Dan Fritchman", email = "dan@fritch.mn"},
```

### Comparing `sky130_hdl21-6.0.0rc0/readme.md` & `sky130_hdl21-7.0.0.dev0/readme.md`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/high_density.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/high_density.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/high_speed.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/high_speed.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_leakage.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/low_leakage.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_power.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/low_power.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_speed.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/low_speed.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/medium_speed.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/digital_cells/medium_speed.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/pdk_data.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/pdk_data.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/pdk_logic.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/pdk_logic.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/primitives/prim_dicts.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/primitives/prim_dicts.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/primitives/primitives.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/primitives/primitives.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/test_netlists.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/test_netlists.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/test_pdk.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/test_pdk.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/sky130_hdl21/test_site_sims.py` & `sky130_hdl21-7.0.0.dev0/sky130_hdl21/test_site_sims.py`

 * *Files identical despite different names*

### Comparing `sky130_hdl21-6.0.0rc0/PKG-INFO` & `sky130_hdl21-7.0.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: sky130-hdl21
-Version: 6.0.0rc0
+Version: 7.0.0.dev0
 Summary: SkyWater 130nm PDK Package for Hdl21
 Keywords: PDK,EDA,analog,circuit
 Author: Thomas Pluck
 Author-email: Dan Fritchman <dan@fritch.mn>, Curtis Mayberry <Curtisma3@gmail.com>
 Maintainer-email: Dan Fritchman <dan@fritch.mn>
 Requires-Python: >=3.7, <3.13
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Requires-Dist: hdl21>=6.0.0rc0,<7
+Requires-Dist: hdl21>=7.0.0.dev0,<7
 Requires-Dist: pytest==7.1 ; extra == "dev"
 Requires-Dist: coverage ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pre-commit==2.20 ; extra == "dev"
 Requires-Dist: black==22.6 ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Project-URL: Bug Tracker, https://github.com/dan-fritchman/Hdl21/issues
```

