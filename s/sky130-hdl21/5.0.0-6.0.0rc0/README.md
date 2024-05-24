# Comparing `tmp/sky130-hdl21-5.0.0.tar.gz` & `tmp/sky130_hdl21-6.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sky130-hdl21-5.0.0.tar", last modified: Tue Nov 14 18:40:38 2023, max compression
+gzip compressed data, was "sky130_hdl21-6.0.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sky130-hdl21-5.0.0.tar` & `sky130_hdl21-6.0.0rc0.tar`

### file list

```diff
@@ -1,29 +1,20 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:38.481609 sky130-hdl21-5.0.0/
--rw-r--r--   0 dan        (501) staff       (20)    20707 2023-11-14 18:40:38.481393 sky130-hdl21-5.0.0/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-11-14 18:40:38.481663 sky130-hdl21-5.0.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      912 2023-11-14 18:31:59.000000 sky130-hdl21-5.0.0/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:38.478326 sky130-hdl21-5.0.0/sky130_hdl21/
--rw-r--r--   0 dan        (501) staff       (20)      333 2023-07-11 14:50:48.000000 sky130-hdl21-5.0.0/sky130_hdl21/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:38.480440 sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/
--rw-r--r--   0 dan        (501) staff       (20)      153 2023-07-11 14:50:48.000000 sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    61602 2023-08-25 22:51:16.000000 sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/high_density.py
--rw-r--r--   0 dan        (501) staff       (20)    53672 2023-08-25 22:51:16.000000 sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/high_speed.py
--rw-r--r--   0 dan        (501) staff       (20)    50419 2023-08-25 22:51:16.000000 sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/low_leakage.py
--rw-r--r--   0 dan        (501) staff       (20)   101450 2023-08-25 22:51:16.000000 sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/low_power.py
--rw-r--r--   0 dan        (501) staff       (20)    54196 2023-08-25 22:51:16.000000 sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/low_speed.py
--rw-r--r--   0 dan        (501) staff       (20)    54623 2023-08-25 22:51:16.000000 sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/medium_speed.py
--rw-r--r--   0 dan        (501) staff       (20)    16281 2023-09-05 17:20:37.000000 sky130-hdl21-5.0.0/sky130_hdl21/pdk_data.py
--rw-r--r--   0 dan        (501) staff       (20)    13588 2023-10-11 16:45:30.000000 sky130-hdl21-5.0.0/sky130_hdl21/pdk_logic.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:38.481132 sky130-hdl21-5.0.0/sky130_hdl21/primitives/
--rw-r--r--   0 dan        (501) staff       (20)       26 2023-07-11 14:50:48.000000 sky130-hdl21-5.0.0/sky130_hdl21/primitives/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    14933 2023-07-11 14:50:48.000000 sky130-hdl21-5.0.0/sky130_hdl21/primitives/prim_dicts.py
--rw-r--r--   0 dan        (501) staff       (20)     7888 2023-07-11 14:50:48.000000 sky130-hdl21-5.0.0/sky130_hdl21/primitives/primitives.py
--rw-r--r--   0 dan        (501) staff       (20)     7190 2023-09-05 17:20:37.000000 sky130-hdl21-5.0.0/sky130_hdl21/test_netlists.py
--rw-r--r--   0 dan        (501) staff       (20)    13614 2023-07-11 14:50:48.000000 sky130-hdl21-5.0.0/sky130_hdl21/test_pdk.py
--rw-r--r--   0 dan        (501) staff       (20)    21806 2023-07-11 14:50:48.000000 sky130-hdl21-5.0.0/sky130_hdl21/test_site_sims.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-11-14 18:40:38.479091 sky130-hdl21-5.0.0/sky130_hdl21.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)    20707 2023-11-14 18:40:38.000000 sky130-hdl21-5.0.0/sky130_hdl21.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      749 2023-11-14 18:40:38.000000 sky130-hdl21-5.0.0/sky130_hdl21.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-11-14 18:40:38.000000 sky130-hdl21-5.0.0/sky130_hdl21.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       58 2023-11-14 18:40:38.000000 sky130-hdl21-5.0.0/sky130_hdl21.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       13 2023-11-14 18:40:38.000000 sky130-hdl21-5.0.0/sky130_hdl21.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1524 2024-05-24 16:13:54.035862 sky130_hdl21-6.0.0rc0/LICENSE
+-rw-r--r--   0        0        0     1321 2024-05-24 16:20:26.505731 sky130_hdl21-6.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0    20435 2023-09-05 17:20:37.569826 sky130_hdl21-6.0.0rc0/readme.md
+-rw-r--r--   0        0        0      333 2023-07-11 14:50:48.432908 sky130_hdl21-6.0.0rc0/sky130_hdl21/__init__.py
+-rw-r--r--   0        0        0      153 2023-07-11 14:50:48.433006 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/__init__.py
+-rw-r--r--   0        0        0    61602 2023-08-25 22:51:16.179401 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/high_density.py
+-rw-r--r--   0        0        0    53672 2023-08-25 22:51:16.179861 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/high_speed.py
+-rw-r--r--   0        0        0    50419 2023-08-25 22:51:16.180189 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_leakage.py
+-rw-r--r--   0        0        0   101450 2023-08-25 22:51:16.180523 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_power.py
+-rw-r--r--   0        0        0    54196 2023-08-25 22:51:16.180834 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_speed.py
+-rw-r--r--   0        0        0    54623 2023-08-25 22:51:16.181132 sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/medium_speed.py
+-rw-r--r--   0        0        0    16083 2024-04-19 00:12:11.470278 sky130_hdl21-6.0.0rc0/sky130_hdl21/pdk_data.py
+-rw-r--r--   0        0        0    13536 2024-04-19 00:12:11.470616 sky130_hdl21-6.0.0rc0/sky130_hdl21/pdk_logic.py
+-rw-r--r--   0        0        0       26 2023-07-11 14:50:48.434932 sky130_hdl21-6.0.0rc0/sky130_hdl21/primitives/__init__.py
+-rw-r--r--   0        0        0    15069 2024-04-19 00:12:11.470940 sky130_hdl21-6.0.0rc0/sky130_hdl21/primitives/prim_dicts.py
+-rw-r--r--   0        0        0     7888 2024-04-19 00:12:11.471254 sky130_hdl21-6.0.0rc0/sky130_hdl21/primitives/primitives.py
+-rw-r--r--   0        0        0     7190 2023-09-05 17:20:37.570542 sky130_hdl21-6.0.0rc0/sky130_hdl21/test_netlists.py
+-rw-r--r--   0        0        0    13614 2023-07-11 14:50:48.443513 sky130_hdl21-6.0.0rc0/sky130_hdl21/test_pdk.py
+-rw-r--r--   0        0        0    21806 2023-07-11 14:50:48.443308 sky130_hdl21-6.0.0rc0/sky130_hdl21/test_site_sims.py
+-rw-r--r--   0        0        0    21574 1970-01-01 00:00:00.000000 sky130_hdl21-6.0.0rc0/PKG-INFO
```

### Comparing `sky130-hdl21-5.0.0/PKG-INFO` & `sky130_hdl21-6.0.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,31 @@
 Metadata-Version: 2.1
 Name: sky130-hdl21
-Version: 5.0.0
+Version: 6.0.0rc0
 Summary: SkyWater 130nm PDK Package for Hdl21
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
+Project-URL: Documentation, https://github.com/dan-fritchman/Hdl21/blob/main/pdks/Sky130/readme.md
+Project-URL: Homepage, https://github.com/dan-fritchman/Hdl21
+Project-URL: Repository, https://github.com/dan-fritchman/Hdl21
 Provides-Extra: dev
 
 
 # Sky130 Hdl21
 
 Hdl21 PDK package for the open-source SkyWater 130nm PDK.  
 https://pypi.org/project/sky130-hdl21/
@@ -318,7 +334,8 @@
 ```
 
 ## Development 
 
 ```
 pip install -e ".[dev]"
 ```
+
```

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/high_density.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/high_density.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/high_speed.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/high_speed.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/low_leakage.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_leakage.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/low_power.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_power.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/low_speed.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/low_speed.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/digital_cells/medium_speed.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/digital_cells/medium_speed.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/pdk_data.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/pdk_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 # Std-Lib Imports
 from copy import deepcopy
-from dataclasses import field
-from typing import Dict, Tuple, List
-from types import SimpleNamespace
-
-# PyPi Imports
-from pydantic.dataclasses import dataclass
+from typing import List
 
 # Hdl21 Imports
 import hdl21 as h
 from hdl21.prefix import (
     MILLI,
-    µ,
     MEGA,
     TERA,
 )
 from hdl21.primitives import (
     MosType,
     MosVth,
     MosFamily,
@@ -31,15 +25,14 @@
     DiodeParams,
     BipolarParams,
 )
 
 # Vlsirtool Types to ease downstream parsing
 from vlsirtools import SpiceType
 
-FIXME = None  # FIXME: Replace with real values!
 PDK_NAME = "sky130"
 
 """
 The following section contains all the necessary @paramclasses required to describe
 parameters of devices in the Sky130 Open PDK. It contains params:
 
 - MosParams (aka. Sky130MosParams) - standard MOS device parameters
@@ -129,31 +122,31 @@
         dtype=h.Scalar,
         desc="Source Resistive Value",
         default=h.Literal("0.29 / w"),
     )
     sa = h.Param(
         dtype=h.Scalar,
         desc="Spacing between Adjacent Gate to Drain",
-        default=h.Literal(0),
+        default=0,
     )
     sb = h.Param(
         dtype=h.Scalar,
         desc="Spacing between Adjacent Gate to Source",
-        default=h.Literal(0),
+        default=0,
     )
     sd = h.Param(
         dtype=h.Scalar,
         desc="Spacing between Adjacent Drain to Source",
-        default=h.Literal(0),
+        default=0,
     )
     mult = h.Param(dtype=h.Scalar, desc="Multiplier", default=1)
     m = h.Param(dtype=h.Scalar, desc="Multiplier", default=1)
 
 
-# FIXME: keep this alias as prior versions may have used it
+# NOTE: probably add a deprecation note for this alias; prior versions may have used it
 Sky130MosParams = MosParams
 
 
 @h.paramclass
 class Sky130Mos20VParams:
     """
     A parameter class representing the MOSFET parameters for the Sky130 technology with a 20V rating.
```

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/pdk_logic.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/pdk_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,21 +349,18 @@
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

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/primitives/prim_dicts.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/primitives/prim_dicts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,26 @@
-from ..pdk_data import *
-
-# Individuate component types
-MosKey = Tuple[str, MosType, MosVth, MosFamily]
-
 """
 These dictionaries are used to map all of the devices of the Sky130 technology
 to their corresponding caller functions above. Keys and names are used to 
 differentiate individual components and populate a namespace which can be used
 to find and determine the correct internal device to use.
 """
 
+# Std-Lib Imports
+from typing import Tuple, Dict
+from dataclasses import dataclass, field
+
+# Local Imports
+from hdl21.prefix import µ
+from ..pdk_data import *
+
+# Individuate component types
+MosKey = Tuple[str, MosType, MosVth, MosFamily]
+
+
 xtors: Dict[MosKey, h.ExternalModule] = {
     # Add all generic transistors
     ("NMOS_1p8V_STD", MosType.NMOS, MosVth.STD, MosFamily.CORE): xtor_module(
         "sky130_fd_pr__nfet_01v8"
     ),
     ("NMOS_1p8V_LOW", MosType.NMOS, MosVth.LOW, MosFamily.CORE): xtor_module(
         "sky130_fd_pr__nfet_01v8_lvt"
```

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/primitives/primitives.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/primitives/primitives.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from ..pdk_data import *
-
 """
 These dictionaries are used to map all of the devices of the Sky130 technology
 to their corresponding caller functions above. Keys and names are used to 
 differentiate individual components and populate a namespace which can be used
 to find and determine the correct internal device to use.
 """
 
+from ..pdk_data import *
+
 NMOS_1p8V_STD = xtor_module("sky130_fd_pr__nfet_01v8")
 NMOS_1p8V_LOW = xtor_module("sky130_fd_pr__nfet_01v8_lvt")
 PMOS_1p8V_STD = xtor_module("sky130_fd_pr__pfet_01v8")
 PMOS_1p8V_HIGH = xtor_module("sky130_fd_pr__pfet_01v8_hvt")
 PMOS_1p8V_LOW = xtor_module("sky130_fd_pr__pfet_01v8_lvt")
 PMOS_5p5V_D10_STD = xtor_module("sky130_fd_pr__pfet_g5v0d10v5")
 NMOS_5p5V_D10_STD = xtor_module("sky130_fd_pr__nfet_g5v0d10v5")
```

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/test_netlists.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/test_netlists.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/test_pdk.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/test_pdk.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21/test_site_sims.py` & `sky130_hdl21-6.0.0rc0/sky130_hdl21/test_site_sims.py`

 * *Files identical despite different names*

### Comparing `sky130-hdl21-5.0.0/sky130_hdl21.egg-info/PKG-INFO` & `sky130_hdl21-6.0.0rc0/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: sky130-hdl21
-Version: 5.0.0
-Summary: SkyWater 130nm PDK Package for Hdl21
-Home-page: https://github.com/dan-fritchman/Hdl21
-Author: Dan Fritchman, Thomas Pluck
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 
 # Sky130 Hdl21
 
 Hdl21 PDK package for the open-source SkyWater 130nm PDK.  
 https://pypi.org/project/sky130-hdl21/
```

