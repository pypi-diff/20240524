# Comparing `tmp/gf180-hdl21-5.0.0.tar.gz` & `tmp/gf180_hdl21-6.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gf180-hdl21-5.0.0.tar", last modified: Tue Nov 14 18:40:51 2023, max compression
+gzip compressed data, was "gf180_hdl21-6.0.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gf180-hdl21-5.0.0.tar` & `gf180_hdl21-6.0.0rc0.tar`

### file list

```diff
@@ -1,25 +1,17 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:51.521659 gf180-hdl21-5.0.0/
--rw-r--r--   0 dan        (501) staff       (20)    10771 2023-11-14 18:40:51.521460 gf180-hdl21-5.0.0/PKG-INFO
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:51.519305 gf180-hdl21-5.0.0/gf180_hdl21/
--rw-r--r--   0 dan        (501) staff       (20)      333 2023-07-11 14:50:48.000000 gf180-hdl21-5.0.0/gf180_hdl21/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:51.520726 gf180-hdl21-5.0.0/gf180_hdl21/digital_cells/
--rw-r--r--   0 dan        (501) staff       (20)       51 2023-07-11 14:50:48.000000 gf180-hdl21-5.0.0/gf180_hdl21/digital_cells/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    31678 2023-08-25 22:51:16.000000 gf180-hdl21-5.0.0/gf180_hdl21/digital_cells/nine_track.py
--rw-r--r--   0 dan        (501) staff       (20)    31913 2023-08-25 22:51:16.000000 gf180-hdl21-5.0.0/gf180_hdl21/digital_cells/seven_track.py
--rw-r--r--   0 dan        (501) staff       (20)     7628 2023-09-05 17:20:37.000000 gf180-hdl21-5.0.0/gf180_hdl21/pdk_data.py
--rw-r--r--   0 dan        (501) staff       (20)    11045 2023-10-11 16:45:30.000000 gf180-hdl21-5.0.0/gf180_hdl21/pdk_logic.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:51.521230 gf180-hdl21-5.0.0/gf180_hdl21/primitives/
--rw-r--r--   0 dan        (501) staff       (20)       26 2023-07-11 14:50:48.000000 gf180-hdl21-5.0.0/gf180_hdl21/primitives/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     5717 2023-07-11 14:50:48.000000 gf180-hdl21-5.0.0/gf180_hdl21/primitives/prim_dicts.py
--rw-r--r--   0 dan        (501) staff       (20)     2656 2023-07-11 14:50:48.000000 gf180-hdl21-5.0.0/gf180_hdl21/primitives/primitives.py
--rw-r--r--   0 dan        (501) staff       (20)     6353 2023-09-05 17:20:37.000000 gf180-hdl21-5.0.0/gf180_hdl21/test_netlists.py
--rw-r--r--   0 dan        (501) staff       (20)     9472 2023-07-11 14:50:48.000000 gf180-hdl21-5.0.0/gf180_hdl21/test_pdk.py
--rw-r--r--   0 dan        (501) staff       (20)     9984 2023-09-05 17:20:37.000000 gf180-hdl21-5.0.0/gf180_hdl21/test_site_sims.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:51.520200 gf180-hdl21-5.0.0/gf180_hdl21.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)    10771 2023-11-14 18:40:51.000000 gf180-hdl21-5.0.0/gf180_hdl21.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      566 2023-11-14 18:40:51.000000 gf180-hdl21-5.0.0/gf180_hdl21.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-11-14 18:40:51.000000 gf180-hdl21-5.0.0/gf180_hdl21.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       58 2023-11-14 18:40:51.000000 gf180-hdl21-5.0.0/gf180_hdl21.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       12 2023-11-14 18:40:51.000000 gf180-hdl21-5.0.0/gf180_hdl21.egg-info/top_level.txt
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-11-14 18:40:51.521710 gf180-hdl21-5.0.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      951 2023-11-14 18:31:59.000000 gf180-hdl21-5.0.0/setup.py
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

### Comparing `gf180-hdl21-5.0.0/PKG-INFO` & `gf180_hdl21-6.0.0rc0/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: gf180-hdl21
-Version: 5.0.0
-Summary: Global Foundries 180nm MCU PDK Package for Hdl21
-Home-page: https://github.com/dan-fritchman/Hdl21
-Author: Dan Fritchman, Thomas Pluck
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 
 # GF 180 MCU - Hdl21 PDK Module
 
 Hdl21 PDK package for the open-source Global Foundries 180nm MCU PDK.  
 https://pypi.org/project/gf180-hdl21/
 
 ## About This Technology 
@@ -272,8 +262,8 @@
 
 ```python
 from gf180_hdl21.digital_cells.seven_track as d7
 from gf180_hdl21 import GF180LogicParams as p
 simple_and_gate = d7.and2_1(p())
 ```
 
-The devices in all are too numerous to cover here, but are covered in great detail in the [official PDK documentation](https://gf180mcu-pdk.readthedocs.io/en/latest/digital/Digital.html).
+The devices in all are too numerous to cover here, but are covered in great detail in the [official PDK documentation](https://gf180mcu-pdk.readthedocs.io/en/latest/digital/Digital.html).
```

### Comparing `gf180-hdl21-5.0.0/gf180_hdl21/digital_cells/nine_track.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/digital_cells/nine_track.py`

 * *Files identical despite different names*

### Comparing `gf180-hdl21-5.0.0/gf180_hdl21/digital_cells/seven_track.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/digital_cells/seven_track.py`

 * *Files identical despite different names*

### Comparing `gf180-hdl21-5.0.0/gf180_hdl21/pdk_data.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/pdk_data.py`

 * *Files identical despite different names*

### Comparing `gf180-hdl21-5.0.0/gf180_hdl21/pdk_logic.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/pdk_logic.py`

 * *Files 3% similar despite different names*

```diff
@@ -281,21 +281,18 @@
         return modcall
 
     def scale_param(self, orig: Optional[h.Scalar], default: h.Prefixed) -> h.Scalar:
         """Replace device size parameter-value `orig`.
         Primarily type-dispatches across the need to scale to microns for this PDK."""
         if orig is None:
             return default
-        if not isinstance(orig, h.Scalar):
-            orig = h.scalar.to_scalar(orig)
-
         if isinstance(orig, h.Prefixed):
-            return orig
+            return orig  # FIXME: where's the scaling?
         if isinstance(orig, h.Literal):
-            return h.Literal(f"({orig} * 1e6)")
+            return h.Literal(f"({orig.text} * 1e6)")
         raise TypeError(f"Param Value {orig}")
 
     def use_defaults(self, params: h.paramclass, modname: str, defaults: dict):
         w, l = None, None
 
         if params.w is None:
             w = defaults[modname][0]
```

### Comparing `gf180-hdl21-5.0.0/gf180_hdl21/primitives/prim_dicts.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/primitives/prim_dicts.py`

 * *Files identical despite different names*

### Comparing `gf180-hdl21-5.0.0/gf180_hdl21/primitives/primitives.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/primitives/primitives.py`

 * *Files identical despite different names*

### Comparing `gf180-hdl21-5.0.0/gf180_hdl21/test_netlists.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/test_netlists.py`

 * *Files identical despite different names*

### Comparing `gf180-hdl21-5.0.0/gf180_hdl21/test_pdk.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/test_pdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 def _compile_and_test(prims: h.Module, paramtype: h.Param):
 
     # Compile
     gf180_hdl21.compile(prims)
 
     # ... and Test
     for k in prims.namespace:
-        if k is not "z":
+        if k != "z":
 
             assert isinstance(prims.namespace[k], h.Instance)
             assert isinstance(prims.namespace[k].of, h.ExternalModuleCall)
             assert isinstance(prims.namespace[k].of.params, paramtype)
 
 
 def test_compile():
```

### Comparing `gf180-hdl21-5.0.0/gf180_hdl21/test_site_sims.py` & `gf180_hdl21-6.0.0rc0/gf180_hdl21/test_site_sims.py`

 * *Files identical despite different names*

### Comparing `gf180-hdl21-5.0.0/gf180_hdl21.egg-info/PKG-INFO` & `gf180_hdl21-6.0.0rc0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 Metadata-Version: 2.1
 Name: gf180-hdl21
-Version: 5.0.0
+Version: 6.0.0rc0
 Summary: Global Foundries 180nm MCU PDK Package for Hdl21
-Home-page: https://github.com/dan-fritchman/Hdl21
-Author: Dan Fritchman, Thomas Pluck
-Requires-Python: >=3.7
+Keywords: PDK,EDA,analog,circuit
+Author: Thomas Pluck
+Author-email: Dan Fritchman <dan@fritch.mn>, Curtis Mayberry <Curtisma3@gmail.com>
+Maintainer-email: Dan Fritchman <dan@fritch.mn>
+Requires-Python: >=3.7, <3.13
 Description-Content-Type: text/markdown
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Requires-Dist: hdl21>=6.0.0rc0,<7
+Requires-Dist: pytest==7.1 ; extra == "dev"
+Requires-Dist: coverage ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: pre-commit==2.20 ; extra == "dev"
+Requires-Dist: black==22.6 ; extra == "dev"
+Requires-Dist: flit ; extra == "dev"
+Project-URL: Bug Tracker, https://github.com/dan-fritchman/Hdl21/issues
+Project-URL: Documentation, https://github.com/dan-fritchman/Hdl21/blob/main/pdks/Gf180/readme.md
+Project-URL: Homepage, https://github.com/dan-fritchman/Hdl21
+Project-URL: Repository, https://github.com/dan-fritchman/Hdl21
 Provides-Extra: dev
 
 
 # GF 180 MCU - Hdl21 PDK Module
 
 Hdl21 PDK package for the open-source Global Foundries 180nm MCU PDK.  
 https://pypi.org/project/gf180-hdl21/
```

