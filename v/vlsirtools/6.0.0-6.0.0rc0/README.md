# Comparing `tmp/vlsirtools-6.0.0.tar.gz` & `tmp/vlsirtools-6.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlsirtools-6.0.0.tar", last modified: Fri May 24 17:15:37 2024, max compression
+gzip compressed data, was "vlsirtools-6.0.0rc0.tar", last modified: Fri May 24 16:31:51 2024, max compression
```

## Comparing `vlsirtools-6.0.0.tar` & `vlsirtools-6.0.0rc0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:15:37.819541 vlsirtools-6.0.0/
--rw-r--r--   0 dan        (501) staff       (20)     2772 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/.gitignore
--rw-r--r--   0 dan        (501) staff       (20)     1521 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)     2795 2024-05-24 17:15:37.819272 vlsirtools-6.0.0/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2368 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-24 17:15:37.819592 vlsirtools-6.0.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     1079 2024-05-24 17:12:12.000000 vlsirtools-6.0.0/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:15:37.810450 vlsirtools-6.0.0/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-06-13 20:36:42.000000 vlsirtools-6.0.0/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)      807 2024-05-24 16:07:55.000000 vlsirtools-6.0.0/tests/test_netlist.py
--rw-r--r--   0 dan        (501) staff       (20)     3790 2023-06-28 18:09:23.000000 vlsirtools-6.0.0/tests/test_primitives.py
--rw-r--r--   0 dan        (501) staff       (20)    21820 2024-05-24 17:12:12.000000 vlsirtools-6.0.0/tests/test_vlsirtools.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:15:37.812346 vlsirtools-6.0.0/vlsirtools/
--rw-r--r--   0 dan        (501) staff       (20)      610 2024-05-24 17:12:12.000000 vlsirtools-6.0.0/vlsirtools/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:15:37.815745 vlsirtools-6.0.0/vlsirtools/netlist/
--rw-r--r--   0 dan        (501) staff       (20)      428 2024-05-24 16:07:55.000000 vlsirtools-6.0.0/vlsirtools/netlist/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    31961 2023-08-30 20:52:59.000000 vlsirtools-6.0.0/vlsirtools/netlist/base.py
--rw-r--r--   0 dan        (501) staff       (20)     3283 2024-05-24 16:07:55.000000 vlsirtools-6.0.0/vlsirtools/netlist/fmt.py
--rw-r--r--   0 dan        (501) staff       (20)     2460 2024-05-24 16:07:55.000000 vlsirtools-6.0.0/vlsirtools/netlist/main.py
--rw-r--r--   0 dan        (501) staff       (20)    14534 2023-06-28 18:09:27.000000 vlsirtools-6.0.0/vlsirtools/netlist/spectre.py
--rw-r--r--   0 dan        (501) staff       (20)     2112 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/vlsirtools/netlist/spectre_spice_shared.py
--rw-r--r--   0 dan        (501) staff       (20)    26453 2023-08-30 20:52:59.000000 vlsirtools-6.0.0/vlsirtools/netlist/spice.py
--rw-r--r--   0 dan        (501) staff       (20)    10660 2023-06-28 18:09:27.000000 vlsirtools-6.0.0/vlsirtools/netlist/verilog.py
--rw-r--r--   0 dan        (501) staff       (20)    16643 2023-08-30 20:52:59.000000 vlsirtools-6.0.0/vlsirtools/primitives.py
--rw-r--r--   0 dan        (501) staff       (20)     6456 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/vlsirtools/pytest.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:15:37.816165 vlsirtools-6.0.0/vlsirtools/spectre/
--rw-r--r--   0 dan        (501) staff       (20)      122 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/vlsirtools/spectre/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:15:37.818173 vlsirtools-6.0.0/vlsirtools/spice/
--rw-r--r--   0 dan        (501) staff       (20)       84 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/vlsirtools/spice/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     5453 2023-11-14 18:31:14.000000 vlsirtools-6.0.0/vlsirtools/spice/base.py
--rw-r--r--   0 dan        (501) staff       (20)    12654 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/vlsirtools/spice/ngspice.py
--rw-r--r--   0 dan        (501) staff       (20)     7030 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/vlsirtools/spice/sim_data.py
--rw-r--r--   0 dan        (501) staff       (20)    11233 2023-11-14 18:31:14.000000 vlsirtools-6.0.0/vlsirtools/spice/spectre.py
--rw-r--r--   0 dan        (501) staff       (20)     5711 2023-11-14 18:31:14.000000 vlsirtools-6.0.0/vlsirtools/spice/spice.py
--rw-r--r--   0 dan        (501) staff       (20)    14053 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/vlsirtools/spice/xyce.py
--rw-r--r--   0 dan        (501) staff       (20)     3459 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/vlsirtools/spicetype.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:15:37.818472 vlsirtools-6.0.0/vlsirtools/xyce/
--rw-r--r--   0 dan        (501) staff       (20)      113 2023-06-26 21:21:08.000000 vlsirtools-6.0.0/vlsirtools/xyce/__init__.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:15:37.818805 vlsirtools-6.0.0/vlsirtools.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     2795 2024-05-24 17:15:37.000000 vlsirtools-6.0.0/vlsirtools.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      880 2024-05-24 17:15:37.000000 vlsirtools-6.0.0/vlsirtools.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-24 17:15:37.000000 vlsirtools-6.0.0/vlsirtools.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       53 2024-05-24 17:15:37.000000 vlsirtools-6.0.0/vlsirtools.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       17 2024-05-24 17:15:37.000000 vlsirtools-6.0.0/vlsirtools.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.354662 vlsirtools-6.0.0rc0/
+-rw-r--r--   0 dan        (501) staff       (20)     2772 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/.gitignore
+-rw-r--r--   0 dan        (501) staff       (20)     1521 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/LICENSE
+-rw-r--r--   0 dan        (501) staff       (20)     2676 2024-05-24 16:31:51.354413 vlsirtools-6.0.0rc0/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2368 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-24 16:31:51.354719 vlsirtools-6.0.0rc0/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)     1149 2024-05-24 16:25:05.000000 vlsirtools-6.0.0rc0/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.345793 vlsirtools-6.0.0rc0/tests/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2022-06-13 20:36:42.000000 vlsirtools-6.0.0rc0/tests/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)      807 2024-05-24 16:07:55.000000 vlsirtools-6.0.0rc0/tests/test_netlist.py
+-rw-r--r--   0 dan        (501) staff       (20)     3790 2023-06-28 18:09:23.000000 vlsirtools-6.0.0rc0/tests/test_primitives.py
+-rw-r--r--   0 dan        (501) staff       (20)    21823 2024-05-24 16:27:03.000000 vlsirtools-6.0.0rc0/tests/test_vlsirtools.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.347183 vlsirtools-6.0.0rc0/vlsirtools/
+-rw-r--r--   0 dan        (501) staff       (20)      613 2024-05-24 16:27:15.000000 vlsirtools-6.0.0rc0/vlsirtools/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.350625 vlsirtools-6.0.0rc0/vlsirtools/netlist/
+-rw-r--r--   0 dan        (501) staff       (20)      428 2024-05-24 16:07:55.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    31961 2023-08-30 20:52:59.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/base.py
+-rw-r--r--   0 dan        (501) staff       (20)     3283 2024-05-24 16:07:55.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/fmt.py
+-rw-r--r--   0 dan        (501) staff       (20)     2460 2024-05-24 16:07:55.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/main.py
+-rw-r--r--   0 dan        (501) staff       (20)    14534 2023-06-28 18:09:27.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/spectre.py
+-rw-r--r--   0 dan        (501) staff       (20)     2112 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/spectre_spice_shared.py
+-rw-r--r--   0 dan        (501) staff       (20)    26453 2023-08-30 20:52:59.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/spice.py
+-rw-r--r--   0 dan        (501) staff       (20)    10660 2023-06-28 18:09:27.000000 vlsirtools-6.0.0rc0/vlsirtools/netlist/verilog.py
+-rw-r--r--   0 dan        (501) staff       (20)    16643 2023-08-30 20:52:59.000000 vlsirtools-6.0.0rc0/vlsirtools/primitives.py
+-rw-r--r--   0 dan        (501) staff       (20)     6456 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/pytest.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.351187 vlsirtools-6.0.0rc0/vlsirtools/spectre/
+-rw-r--r--   0 dan        (501) staff       (20)      122 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spectre/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.353351 vlsirtools-6.0.0rc0/vlsirtools/spice/
+-rw-r--r--   0 dan        (501) staff       (20)       84 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     5453 2023-11-14 18:31:14.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/base.py
+-rw-r--r--   0 dan        (501) staff       (20)    12654 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/ngspice.py
+-rw-r--r--   0 dan        (501) staff       (20)     7030 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/sim_data.py
+-rw-r--r--   0 dan        (501) staff       (20)    11233 2023-11-14 18:31:14.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/spectre.py
+-rw-r--r--   0 dan        (501) staff       (20)     5711 2023-11-14 18:31:14.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/spice.py
+-rw-r--r--   0 dan        (501) staff       (20)    14053 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spice/xyce.py
+-rw-r--r--   0 dan        (501) staff       (20)     3459 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/spicetype.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.353909 vlsirtools-6.0.0rc0/vlsirtools/xyce/
+-rw-r--r--   0 dan        (501) staff       (20)      113 2023-06-26 21:21:08.000000 vlsirtools-6.0.0rc0/vlsirtools/xyce/__init__.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 16:31:51.348291 vlsirtools-6.0.0rc0/vlsirtools.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     2676 2024-05-24 16:31:51.000000 vlsirtools-6.0.0rc0/vlsirtools.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      880 2024-05-24 16:31:51.000000 vlsirtools-6.0.0rc0/vlsirtools.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-24 16:31:51.000000 vlsirtools-6.0.0rc0/vlsirtools.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       97 2024-05-24 16:31:51.000000 vlsirtools-6.0.0rc0/vlsirtools.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       17 2024-05-24 16:31:51.000000 vlsirtools-6.0.0rc0/vlsirtools.egg-info/top_level.txt
```

### Comparing `vlsirtools-6.0.0/.gitignore` & `vlsirtools-6.0.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/LICENSE` & `vlsirtools-6.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/PKG-INFO` & `vlsirtools-6.0.0rc0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: vlsirtools
-Version: 6.0.0
+Version: 6.0.0rc0
 Summary: Tools for the Vlsir IC Design Schema
 Home-page: https://github.com/Vlsir/Vlsir
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: vlsir==6.0.0
-Requires-Dist: numpy~=1.21
-Requires-Dist: pandas~=1.3
 Provides-Extra: dev
-Requires-Dist: vlsirdev; extra == "dev"
+License-File: LICENSE
 
 
 # Vlsir Tools 
 
 Python-based tools and utilites for working with the Vlsir IC design schema. 
 
 ## Netlisting
```

### Comparing `vlsirtools-6.0.0/readme.md` & `vlsirtools-6.0.0rc0/readme.md`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/setup.py` & `vlsirtools-6.0.0rc0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pathlib
 
 # Get the long description from the README file
 here = pathlib.Path(__file__).parent.resolve()
 readme = here / "readme.md"
 long_description = "" if not readme.exists() else readme.read_text(encoding="utf-8")
 
-VLSIR_VERSION = "6.0.0"
+VLSIR_VERSION = "6.0.0rc0"
 
 setup(
     name="vlsirtools",
     version=VLSIR_VERSION,
     description="Tools for the Vlsir IC Design Schema",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -29,9 +29,11 @@
     packages=find_packages(),
     python_requires=">=3.7, <3.12",
     install_requires=[
         f"vlsir=={VLSIR_VERSION}",  # VLSIR Core Python Bindings
         "numpy~=1.21",  # For `sim_data` simulation results
         "pandas~=1.3",  # For CSV reading
     ],
-    extras_require={"dev": ["vlsirdev"]},
+    extras_require={
+        "dev": ["pytest==7.1", "coverage", "pytest-cov", "black==22.6", "twine"]
+    },
 )
```

### Comparing `vlsirtools-6.0.0/tests/test_netlist.py` & `vlsirtools-6.0.0rc0/tests/test_netlist.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/tests/test_primitives.py` & `vlsirtools-6.0.0rc0/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/tests/test_vlsirtools.py` & `vlsirtools-6.0.0rc0/tests/test_vlsirtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 def _prim(name: str) -> Reference:
     """Create a `Reference` to primitive `name`"""
     return Reference(external=QualifiedName(domain="vlsir.primitives", name=name))
 
 
 def test_version():
-    assert vlsirtools.__version__ == "6.0.0"  # VLSIR_VERSION
+    assert vlsirtools.__version__ == "6.0.0rc0"  # VLSIR_VERSION
 
 
 def test_verilog_netlist1():
     """Test netlisting to a handful of formats, including Verilog-compatible contents."""
 
     # "Verilog Compatibility" requires:
     # * All ports must be directed. No "NONE" directions.
```

### Comparing `vlsirtools-6.0.0/vlsirtools/__init__.py` & `vlsirtools-6.0.0rc0/vlsirtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 # Vlsir Tools
 """
 
-__version__ = "6.0.0"  # VLSIR_VERSION
+__version__ = "6.0.0rc0"  # VLSIR_VERSION
 
 # Python module namespaces
 from . import spice
 from . import spicetype
 from .spicetype import SpiceType
 
 # Primitive Definitions
```

### Comparing `vlsirtools-6.0.0/vlsirtools/netlist/base.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/base.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/netlist/fmt.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/fmt.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/netlist/main.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/main.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/netlist/spectre.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/spectre.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/netlist/spectre_spice_shared.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/spectre_spice_shared.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/netlist/spice.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/spice.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/netlist/verilog.py` & `vlsirtools-6.0.0rc0/vlsirtools/netlist/verilog.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/primitives.py` & `vlsirtools-6.0.0rc0/vlsirtools/primitives.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/pytest.py` & `vlsirtools-6.0.0rc0/vlsirtools/pytest.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/spice/base.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/base.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/spice/ngspice.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/ngspice.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/spice/sim_data.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/sim_data.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/spice/spectre.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/spectre.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/spice/spice.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/spice.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/spice/xyce.py` & `vlsirtools-6.0.0rc0/vlsirtools/spice/xyce.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools/spicetype.py` & `vlsirtools-6.0.0rc0/vlsirtools/spicetype.py`

 * *Files identical despite different names*

### Comparing `vlsirtools-6.0.0/vlsirtools.egg-info/PKG-INFO` & `vlsirtools-6.0.0rc0/vlsirtools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: vlsirtools
-Version: 6.0.0
+Version: 6.0.0rc0
 Summary: Tools for the Vlsir IC Design Schema
 Home-page: https://github.com/Vlsir/Vlsir
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: vlsir==6.0.0
-Requires-Dist: numpy~=1.21
-Requires-Dist: pandas~=1.3
 Provides-Extra: dev
-Requires-Dist: vlsirdev; extra == "dev"
+License-File: LICENSE
 
 
 # Vlsir Tools 
 
 Python-based tools and utilites for working with the Vlsir IC design schema. 
 
 ## Netlisting
```

### Comparing `vlsirtools-6.0.0/vlsirtools.egg-info/SOURCES.txt` & `vlsirtools-6.0.0rc0/vlsirtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

