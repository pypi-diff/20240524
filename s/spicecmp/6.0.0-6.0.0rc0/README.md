# Comparing `tmp/spicecmp-6.0.0.tar.gz` & `tmp/spicecmp-6.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicecmp-6.0.0.tar", last modified: Fri May 24 17:16:08 2024, max compression
+gzip compressed data, was "spicecmp-6.0.0rc0.tar", last modified: Fri May 24 17:03:20 2024, max compression
```

## Comparing `spicecmp-6.0.0.tar` & `spicecmp-6.0.0rc0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:16:08.667409 spicecmp-6.0.0/
--rw-r--r--   0 dan        (501) staff       (20)     2842 2023-06-26 21:21:08.000000 spicecmp-6.0.0/.gitignore
--rw-r--r--   0 dan        (501) staff       (20)     5399 2024-05-24 17:16:08.667148 spicecmp-6.0.0/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     4962 2023-06-26 21:21:08.000000 spicecmp-6.0.0/readme.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-24 17:16:08.667460 spicecmp-6.0.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     1043 2024-05-24 17:12:12.000000 spicecmp-6.0.0/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:16:08.665117 spicecmp-6.0.0/spicecmp/
--rw-r--r--   0 dan        (501) staff       (20)      311 2024-05-24 17:12:12.000000 spicecmp-6.0.0/spicecmp/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    10416 2023-06-26 21:21:08.000000 spicecmp-6.0.0/spicecmp/benches.py
--rw-r--r--   0 dan        (501) staff       (20)     3773 2023-06-26 21:21:08.000000 spicecmp-6.0.0/spicecmp/compare_me.py
--rw-r--r--   0 dan        (501) staff       (20)     3334 2023-06-26 21:21:08.000000 spicecmp-6.0.0/spicecmp/compare_meas.py
--rw-r--r--   0 dan        (501) staff       (20)      170 2023-06-26 21:21:08.000000 spicecmp-6.0.0/spicecmp/corner.py
--rw-r--r--   0 dan        (501) staff       (20)      133 2023-06-26 21:21:08.000000 spicecmp-6.0.0/spicecmp/errormode.py
--rw-r--r--   0 dan        (501) staff       (20)      747 2023-06-26 21:21:08.000000 spicecmp-6.0.0/spicecmp/mos.py
--rw-r--r--   0 dan        (501) staff       (20)     2517 2023-06-26 21:21:08.000000 spicecmp-6.0.0/spicecmp/pdk.py
--rw-r--r--   0 dan        (501) staff       (20)      873 2023-06-26 21:21:08.000000 spicecmp-6.0.0/spicecmp/pdk_sim_combo.py
--rw-r--r--   0 dan        (501) staff       (20)      904 2023-06-26 21:21:08.000000 spicecmp-6.0.0/spicecmp/simulator.py
--rw-r--r--   0 dan        (501) staff       (20)     1856 2023-06-26 21:21:08.000000 spicecmp-6.0.0/spicecmp/testcase.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:16:08.666678 spicecmp-6.0.0/spicecmp.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     5399 2024-05-24 17:16:08.000000 spicecmp-6.0.0/spicecmp.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      460 2024-05-24 17:16:08.000000 spicecmp-6.0.0/spicecmp.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-24 17:16:08.000000 spicecmp-6.0.0/spicecmp.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       72 2024-05-24 17:16:08.000000 spicecmp-6.0.0/spicecmp.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       15 2024-05-24 17:16:08.000000 spicecmp-6.0.0/spicecmp.egg-info/top_level.txt
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:16:08.666309 spicecmp-6.0.0/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2023-06-26 21:21:08.000000 spicecmp-6.0.0/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)      106 2024-05-24 17:12:12.000000 spicecmp-6.0.0/tests/test_spicecmp.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:03:20.199398 spicecmp-6.0.0rc0/
+-rw-r--r--   0 dan        (501) staff       (20)     2842 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/.gitignore
+-rw-r--r--   0 dan        (501) staff       (20)     5411 2024-05-24 17:03:20.199126 spicecmp-6.0.0rc0/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     4962 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-24 17:03:20.199452 spicecmp-6.0.0rc0/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)     1046 2024-05-24 16:44:54.000000 spicecmp-6.0.0rc0/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:03:20.197139 spicecmp-6.0.0rc0/spicecmp/
+-rw-r--r--   0 dan        (501) staff       (20)      314 2024-05-24 16:26:39.000000 spicecmp-6.0.0rc0/spicecmp/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    10416 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/spicecmp/benches.py
+-rw-r--r--   0 dan        (501) staff       (20)     3773 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/spicecmp/compare_me.py
+-rw-r--r--   0 dan        (501) staff       (20)     3334 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/spicecmp/compare_meas.py
+-rw-r--r--   0 dan        (501) staff       (20)      170 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/spicecmp/corner.py
+-rw-r--r--   0 dan        (501) staff       (20)      133 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/spicecmp/errormode.py
+-rw-r--r--   0 dan        (501) staff       (20)      747 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/spicecmp/mos.py
+-rw-r--r--   0 dan        (501) staff       (20)     2517 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/spicecmp/pdk.py
+-rw-r--r--   0 dan        (501) staff       (20)      873 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/spicecmp/pdk_sim_combo.py
+-rw-r--r--   0 dan        (501) staff       (20)      904 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/spicecmp/simulator.py
+-rw-r--r--   0 dan        (501) staff       (20)     1856 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/spicecmp/testcase.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:03:20.198665 spicecmp-6.0.0rc0/spicecmp.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     5411 2024-05-24 17:03:20.000000 spicecmp-6.0.0rc0/spicecmp.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      460 2024-05-24 17:03:20.000000 spicecmp-6.0.0rc0/spicecmp.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-24 17:03:20.000000 spicecmp-6.0.0rc0/spicecmp.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       81 2024-05-24 17:03:20.000000 spicecmp-6.0.0rc0/spicecmp.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       15 2024-05-24 17:03:20.000000 spicecmp-6.0.0rc0/spicecmp.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-24 17:03:20.198147 spicecmp-6.0.0rc0/tests/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2023-06-26 21:21:08.000000 spicecmp-6.0.0rc0/tests/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)      109 2024-05-24 16:26:49.000000 spicecmp-6.0.0rc0/tests/test_spicecmp.py
```

### Comparing `spicecmp-6.0.0/.gitignore` & `spicecmp-6.0.0rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `spicecmp-6.0.0/PKG-INFO` & `spicecmp-6.0.0rc0/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: spicecmp
-Version: 6.0.0
-Summary: Spice Models and Results Comparisons
-Home-page: https://github.com/Vlsir/Vlsir
-Author: Dan Fritchman
-Author-email: dan@fritch.mn
-Requires-Python: >=3.7, <3.12
-Description-Content-Type: text/markdown
-Requires-Dist: pandas~=1.3
-Requires-Dist: hdl21==6.0.0
-Requires-Dist: vlsir==6.0.0
-Requires-Dist: vlsirtools==6.0.0
-Provides-Extra: dev
-Requires-Dist: vlsirdev; extra == "dev"
-
 
 # SpiceCmp 
 
 A Python library for making comparisons between Spice-class simulators.
 
 
 ## Running
```

### Comparing `spicecmp-6.0.0/readme.md` & `spicecmp-6.0.0rc0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: spicecmp
+Version: 6.0.0rc0
+Summary: Spice Models and Results Comparisons
+Home-page: https://github.com/Vlsir/Vlsir
+Author: Dan Fritchman
+Author-email: dan@fritch.mn
+Requires-Python: >=3.7, <3.12
+Description-Content-Type: text/markdown
+Requires-Dist: pandas~=1.3
+Requires-Dist: hdl21==6.0.0rc0
+Requires-Dist: vlsir==6.0.0rc0
+Requires-Dist: vlsirtools==6.0.0rc0
+Provides-Extra: dev
+Requires-Dist: vlsirdev; extra == "dev"
+
 
 # SpiceCmp 
 
 A Python library for making comparisons between Spice-class simulators.
 
 
 ## Running
```

### Comparing `spicecmp-6.0.0/setup.py` & `spicecmp-6.0.0rc0/setup.py`

 * *Files 11% similar despite different names*

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
     name="spicecmp",
     version=VLSIR_VERSION,
     description="Spice Models and Results Comparisons",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `spicecmp-6.0.0/spicecmp/benches.py` & `spicecmp-6.0.0rc0/spicecmp/benches.py`

 * *Files identical despite different names*

### Comparing `spicecmp-6.0.0/spicecmp/compare_me.py` & `spicecmp-6.0.0rc0/spicecmp/compare_me.py`

 * *Files identical despite different names*

### Comparing `spicecmp-6.0.0/spicecmp/compare_meas.py` & `spicecmp-6.0.0rc0/spicecmp/compare_meas.py`

 * *Files identical despite different names*

### Comparing `spicecmp-6.0.0/spicecmp/mos.py` & `spicecmp-6.0.0rc0/spicecmp/mos.py`

 * *Files identical despite different names*

### Comparing `spicecmp-6.0.0/spicecmp/pdk.py` & `spicecmp-6.0.0rc0/spicecmp/pdk.py`

 * *Files identical despite different names*

### Comparing `spicecmp-6.0.0/spicecmp/pdk_sim_combo.py` & `spicecmp-6.0.0rc0/spicecmp/pdk_sim_combo.py`

 * *Files identical despite different names*

### Comparing `spicecmp-6.0.0/spicecmp/simulator.py` & `spicecmp-6.0.0rc0/spicecmp/simulator.py`

 * *Files identical despite different names*

### Comparing `spicecmp-6.0.0/spicecmp/testcase.py` & `spicecmp-6.0.0rc0/spicecmp/testcase.py`

 * *Files identical despite different names*

### Comparing `spicecmp-6.0.0/spicecmp.egg-info/PKG-INFO` & `spicecmp-6.0.0rc0/spicecmp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spicecmp
-Version: 6.0.0
+Version: 6.0.0rc0
 Summary: Spice Models and Results Comparisons
 Home-page: https://github.com/Vlsir/Vlsir
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pandas~=1.3
-Requires-Dist: hdl21==6.0.0
-Requires-Dist: vlsir==6.0.0
-Requires-Dist: vlsirtools==6.0.0
+Requires-Dist: hdl21==6.0.0rc0
+Requires-Dist: vlsir==6.0.0rc0
+Requires-Dist: vlsirtools==6.0.0rc0
 Provides-Extra: dev
 Requires-Dist: vlsirdev; extra == "dev"
 
 
 # SpiceCmp 
 
 A Python library for making comparisons between Spice-class simulators.
```

