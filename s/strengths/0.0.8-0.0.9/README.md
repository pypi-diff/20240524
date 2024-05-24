# Comparing `tmp/strengths-0.0.8.tar.gz` & `tmp/strengths-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strengths-0.0.8.tar", last modified: Tue Dec 12 05:16:22 2023, max compression
+gzip compressed data, was "strengths-0.0.9.tar", last modified: Thu Dec 21 12:19:18 2023, max compression
```

## Comparing `strengths-0.0.8.tar` & `strengths-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-12-12 05:16:22.750637 strengths-0.0.8/
--rw-rw-rw-   0        0        0     1115 2023-12-06 10:15:51.000000 strengths-0.0.8/LICENCE
--rw-rw-rw-   0        0        0      404 2023-12-06 10:15:51.000000 strengths-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      247 2023-12-12 05:16:22.749637 strengths-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-12-06 10:15:51.000000 strengths-0.0.8/README.rst
--rw-rw-rw-   0        0        0      237 2023-12-06 10:15:51.000000 strengths-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-12-12 05:16:22.750637 strengths-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-12-12 05:16:22.696637 strengths-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-12-12 05:16:22.725637 strengths-0.0.8/src/strengths/
--rw-rw-rw-   0        0        0      487 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/__init__.py
--rw-rw-rw-   0        0        0    10346 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/coarsegrain.py
--rw-rw-rw-   0        0        0      788 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/constants.py
--rw-rw-rw-   0        0        0     3636 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/engine_collection.py
-drwxrwxrwx   0        0        0        0 2023-12-12 05:16:22.697637 strengths-0.0.8/src/strengths/engines/
-drwxrwxrwx   0        0        0        0 2023-12-12 05:16:22.737637 strengths-0.0.8/src/strengths/engines/strengths_engine/
--rw-rw-rw-   0        0        0  2856162 2023-12-12 05:13:28.000000 strengths-0.0.8/src/strengths/engines/strengths_engine/engine_w.dll
-drwxrwxrwx   0        0        0        0 2023-12-12 05:16:22.746637 strengths-0.0.8/src/strengths/engines/strengths_engine/src/
--rw-rw-rw-   0        0        0     1877 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/engines/strengths_engine/src/Euler3D.hpp
--rw-rw-rw-   0        0        0     4808 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/engines/strengths_engine/src/Gillespie3D.hpp
--rw-rw-rw-   0        0        0    17000 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/engines/strengths_engine/src/SimulationAlgorithm3DBase.hpp
--rw-rw-rw-   0        0        0     3070 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/engines/strengths_engine/src/TauLeap3D.hpp
--rw-rw-rw-   0        0        0    19532 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/engines/strengths_engine/src/engine.cpp
--rw-rw-rw-   0        0        0     1449 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/filepath.py
--rw-rw-rw-   0        0        0     8893 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/kinetics.py
--rw-rw-rw-   0        0        0     5265 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/kineticsrdengine.py
--rw-rw-rw-   0        0        0    16815 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/librdengine.py
--rw-rw-rw-   0        0        0    13219 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/plot.py
--rw-rw-rw-   0        0        0     3800 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/rdengine.py
--rw-rw-rw-   0        0        0    13078 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/rdgraphspace.py
--rw-rw-rw-   0        0        0    14369 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/rdgridspace.py
--rw-rw-rw-   0        0        0    37662 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/rdnetwork.py
--rw-rw-rw-   0        0        0    13323 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/rdoutput.py
--rw-rw-rw-   0        0        0     9059 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/rdscript.py
--rw-rw-rw-   0        0        0     2084 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/rdspace.py
--rw-rw-rw-   0        0        0        0 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/rdspacebase.py
--rw-rw-rw-   0        0        0    23346 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/rdsystem.py
--rw-rw-rw-   0        0        0     3942 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/simulate.py
--rw-rw-rw-   0        0        0      381 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/text_array_rw.py
--rw-rw-rw-   0        0        0     1086 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/typechecking.py
--rw-rw-rw-   0        0        0    61277 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/units.py
--rw-rw-rw-   0        0        0     7510 2023-12-06 10:15:51.000000 strengths-0.0.8/src/strengths/value_processing.py
-drwxrwxrwx   0        0        0        0 2023-12-12 05:16:22.748637 strengths-0.0.8/src/strengths.egg-info/
--rw-rw-rw-   0        0        0      247 2023-12-12 05:16:22.000000 strengths-0.0.8/src/strengths.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1185 2023-12-12 05:16:22.000000 strengths-0.0.8/src/strengths.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-12 05:16:22.000000 strengths-0.0.8/src/strengths.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-12-12 05:16:22.000000 strengths-0.0.8/src/strengths.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-12-21 12:19:18.430703 strengths-0.0.9/
+-rw-rw-rw-   0        0        0     1115 2023-12-21 11:52:06.000000 strengths-0.0.9/LICENCE
+-rw-rw-rw-   0        0        0      635 2023-12-21 11:52:06.000000 strengths-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      247 2023-12-21 12:19:18.430703 strengths-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-12-21 11:52:06.000000 strengths-0.0.9/README.rst
+-rw-rw-rw-   0        0        0      237 2023-12-21 11:52:06.000000 strengths-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-12-21 12:19:18.430703 strengths-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-12-21 11:52:06.000000 strengths-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-21 12:19:18.377319 strengths-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-12-21 12:19:18.408561 strengths-0.0.9/src/strengths/
+-rw-rw-rw-   0        0        0      487 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/__init__.py
+-rw-rw-rw-   0        0        0    10346 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/coarsegrain.py
+-rw-rw-rw-   0        0        0      788 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/constants.py
+-rw-rw-rw-   0        0        0     3315 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/engine_collection.py
+drwxrwxrwx   0        0        0        0 2023-12-21 12:19:18.377319 strengths-0.0.9/src/strengths/engines/
+drwxrwxrwx   0        0        0        0 2023-12-21 12:19:18.377319 strengths-0.0.9/src/strengths/engines/strengths_engine/
+drwxrwxrwx   0        0        0        0 2023-12-21 12:19:18.415070 strengths-0.0.9/src/strengths/engines/strengths_engine/src/
+-rw-rw-rw-   0        0        0     1877 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/engines/strengths_engine/src/Euler3D.hpp
+-rw-rw-rw-   0        0        0     1875 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/engines/strengths_engine/src/EulerGraph.hpp
+-rw-rw-rw-   0        0        0     4808 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/engines/strengths_engine/src/Gillespie3D.hpp
+-rw-rw-rw-   0        0        0     6621 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/engines/strengths_engine/src/GillespieGraph.hpp
+-rw-rw-rw-   0        0        0    17006 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/engines/strengths_engine/src/SimulationAlgorithm3DBase.hpp
+-rw-rw-rw-   0        0        0    16727 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/engines/strengths_engine/src/SimulationAlgorithmGraphBase.hpp
+-rw-rw-rw-   0        0        0     3070 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/engines/strengths_engine/src/TauLeap3D.hpp
+-rw-rw-rw-   0        0        0     3172 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/engines/strengths_engine/src/TauLeapGraph.hpp
+-rw-rw-rw-   0        0        0    19438 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/engines/strengths_engine/src/engine.cpp
+-rw-rw-rw-   0        0        0     1449 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/filepath.py
+-rw-rw-rw-   0        0        0     8893 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/kinetics.py
+-rw-rw-rw-   0        0        0     5265 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/kineticsrdengine.py
+-rw-rw-rw-   0        0        0    16815 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/librdengine.py
+-rw-rw-rw-   0        0        0    13219 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/plot.py
+-rw-rw-rw-   0        0        0     3800 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/rdengine.py
+-rw-rw-rw-   0        0        0    13078 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/rdgraphspace.py
+-rw-rw-rw-   0        0        0    14369 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/rdgridspace.py
+-rw-rw-rw-   0        0        0    37662 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/rdnetwork.py
+-rw-rw-rw-   0        0        0    13323 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/rdoutput.py
+-rw-rw-rw-   0        0        0     9059 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/rdscript.py
+-rw-rw-rw-   0        0        0     2084 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/rdspace.py
+-rw-rw-rw-   0        0        0        0 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/rdspacebase.py
+-rw-rw-rw-   0        0        0    23346 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/rdsystem.py
+-rw-rw-rw-   0        0        0     3942 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/simulate.py
+-rw-rw-rw-   0        0        0      381 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/text_array_rw.py
+-rw-rw-rw-   0        0        0     1086 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/typechecking.py
+-rw-rw-rw-   0        0        0    61277 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/units.py
+-rw-rw-rw-   0        0        0     7510 2023-12-21 11:52:06.000000 strengths-0.0.9/src/strengths/value_processing.py
+drwxrwxrwx   0        0        0        0 2023-12-21 12:19:18.430703 strengths-0.0.9/src/strengths.egg-info/
+-rw-rw-rw-   0        0        0      247 2023-12-21 12:19:18.000000 strengths-0.0.9/src/strengths.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1706 2023-12-21 12:19:18.000000 strengths-0.0.9/src/strengths.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-21 12:19:18.000000 strengths-0.0.9/src/strengths.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-12-21 12:19:18.000000 strengths-0.0.9/src/strengths.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-12-21 12:19:18.430703 strengths-0.0.9/tests/
+-rw-rw-rw-   0        0        0     8415 2023-12-21 11:52:06.000000 strengths-0.0.9/tests/test_coarsegrain.py
+-rw-rw-rw-   0        0        0     1872 2023-12-21 11:52:06.000000 strengths-0.0.9/tests/test_graph.py
+-rw-rw-rw-   0        0        0     9274 2023-12-21 11:52:06.000000 strengths-0.0.9/tests/test_librdengine.py
+-rw-rw-rw-   0        0        0     3601 2023-12-21 11:52:06.000000 strengths-0.0.9/tests/test_loadrds.py
+-rw-rw-rw-   0        0        0     3834 2023-12-21 11:52:06.000000 strengths-0.0.9/tests/test_meshgrid.py
+-rw-rw-rw-   0        0        0     8117 2023-12-21 11:52:06.000000 strengths-0.0.9/tests/test_rdnetwork.py
+-rw-rw-rw-   0        0        0     8555 2023-12-21 11:52:06.000000 strengths-0.0.9/tests/test_rdoutput.py
+-rw-rw-rw-   0        0        0    11027 2023-12-21 11:52:06.000000 strengths-0.0.9/tests/test_rdsystem.py
+-rw-rw-rw-   0        0        0     2927 2023-12-21 11:52:06.000000 strengths-0.0.9/tests/test_simulate.py
+-rw-rw-rw-   0        0        0      529 2023-12-21 11:52:06.000000 strengths-0.0.9/tests/test_unitarray.py
+-rw-rw-rw-   0        0        0    11303 2023-12-21 11:52:06.000000 strengths-0.0.9/tests/test_units.py
```

### Comparing `strengths-0.0.8/LICENCE` & `strengths-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/README.rst` & `strengths-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/coarsegrain.py` & `strengths-0.0.9/src/strengths/coarsegrain.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/constants.py` & `strengths-0.0.9/src/strengths/constants.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/engine_collection.py` & `strengths-0.0.9/src/strengths/engine_collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import platform
 import strengths
 import ctypes
+import pathlib
 
 from strengths.librdengine import LibRDEngine
 
 def _get_strengths_path():
         path = ""
         for i in strengths.__path__ :
             path += i
         return path
 
-def _get_os_specific_engine_lib_name() :
-    os = platform.system()
-    if   os == "Windows" :
-        return "engine_w.dll"
-    elif os == "Linux" :
-        return "engine_l.so"
-    elif os == "Darwin" :
-        return "engine_m.so"
-    else :
-        raise OSError("It seems that we havent planed any precompiled engine " +
-                      "libaray for your operating system. You can try to " +
-                      "build the engine dynamic library from sources, and then " +
-                      "use it through a LibRDEngineRefrence object.")
+def _get_engine_path() :
+    # Assumes the engine library binary file is the 
+    # only non directory item in the strengths_engine 
+    # directory.
+
+    strnpath = _get_strengths_path()
+    sedirpath = strnpath + "/engines/strengths_engine"
+    path = pathlib.Path(sedirpath)
+    content = path.iterdir()
+    files = []
+    for i in content :
+        if not i.is_dir() : 
+            files.append(i)
+    return str(files[0])
 
 def gillespie_engine():
     """
     Engine using the original Gillespie algorithm (Gillespie, 1977) [#Gillespie1977]_.
     Diffusion is treated as a first order reaction according to Bernstein's method (Bernstein, 2005) [#Bernstein2005]_.
     """
     # references :
     # .. [#Bernstein2005] Bernstein, D. (2005). Simulating mesoscopic reaction-diffusion systems using the Gillespie algorithm. Physical Review E, 71(4), Article 041103. https://doi.org/10.1103/PhysRevE.71.041103
     # .. [#Gillespie1977] Gillespie, D. T. (1977). Exact stochastic simulation of coupled chemical reactions. The Journal of Physical Chemistry, 81(25), 2340-2361. https://doi.org/10.1021/j100540a008
     
-    path = _get_strengths_path()+"/engines/strengths_engine/"+_get_os_specific_engine_lib_name()
-    
+    path = _get_engine_path()
     return LibRDEngine(
         ctypes.CDLL(path),
         option="gillespie",
         description="description",
         requires_molecules=True
         )
 
@@ -47,16 +48,15 @@
     Engine using the Gillespie tau leap method (Gillespie, 2001) [#Gillespie2001]_ with a static time step.
     Diffusion is treated as a first order reaction according to Bernstein's method (Bernstein, 2005) [#Bernstein2005]_.
     """
     # references :
     # .. [#Bernstein2005] Bernstein, D. (2005). Simulating mesoscopic reaction-diffusion systems using the Gillespie algorithm. Physical Review E, 71(4), Article 041103. https://doi.org/10.1103/PhysRevE.71.041103
     # .. [#Gillespie2001] Gillespie, D. T. (2001). Approximate accelerated stochastic simulation of chemically reacting systems. The Journal of Chemical Physics, 115(4), 1716-1733. https://doi.org/10.1063/1.1378322
     
-    path = _get_strengths_path()+"/engines/strengths_engine/"+_get_os_specific_engine_lib_name()
-
+    path = _get_engine_path()
     return LibRDEngine(
         ctypes.CDLL(path),
         option = "tauleap",
         description="description",
         requires_molecules=True
         )
 
@@ -64,15 +64,15 @@
     """
     Engine using a simple Euler method with a static time step.
     Diffusion is treated as a first order reaction according to Bernstein's method (Bernstein, 2005) [#Bernstein2005]_.
     """
     # references :
     # .. [#Bernstein2005] Bernstein, D. (2005). Simulating mesoscopic reaction-diffusion systems using the Gillespie algorithm. Physical Review E, 71(4), Article 041103. https://doi.org/10.1103/PhysRevE.71.041103
 
-    path = _get_strengths_path()+"/engines/strengths_engine/"+_get_os_specific_engine_lib_name()
+    path = _get_engine_path()
     return LibRDEngine(
         ctypes.CDLL(path),
         option = "euler",
         description = "description",
         requires_molecules=False
         )
```

### Comparing `strengths-0.0.8/src/strengths/engines/strengths_engine/src/Euler3D.hpp` & `strengths-0.0.9/src/strengths/engines/strengths_engine/src/Euler3D.hpp`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/engines/strengths_engine/src/Gillespie3D.hpp` & `strengths-0.0.9/src/strengths/engines/strengths_engine/src/Gillespie3D.hpp`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/engines/strengths_engine/src/SimulationAlgorithm3DBase.hpp` & `strengths-0.0.9/src/strengths/engines/strengths_engine/src/SimulationAlgorithm3DBase.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -96,24 +96,24 @@
             for(int n=0; n<6; n++)
                 {
                 this->mesh_neighbors[i*6+n] = GetNeighborIndex(xcoord, ycoord, zcoord, n);
                 }
             }
         }
 
-    void Build_mesh_kr(const std::vector<double> & k, const std::vector<int> & r_env)
+    void Build_mesh_kr(const std::vector<double> & k, const std::vector<double> & r_env)
     // builds mesh_kr
         {
         mesh_kr.clear();
         mesh_kr.resize(n_meshes*n_reactions, 0);
         for(int i=0;i<n_meshes;i++)
           {
           for(int r=0; r<n_reactions; r++)
             {
-            int q = 0;
+            double q = 0;
             for(int s=0; s<n_species; s++)
                 q+=sub[s*n_reactions+r];
             mesh_kr[i*n_reactions+r] = k[r]*pow(mesh_vol,1-q)*r_env[r*n_env+mesh_env[i]];
             }
           }
         }
 
@@ -313,15 +313,15 @@
         std::vector<double> mesh_x0,    //initial state //mesh first array : [mesh [species]]
         std::vector<int>    mesh_chstt, //species chemostats //mesh first array : [mesh [species]]
         std::vector<int>    mesh_env,   //meshes environment indices
         double mesh_vol,                //volume of a mesh
         std::vector<double> k,          //reaction rates
         std::vector<double> sub,        //N*M substrate matrix
         std::vector<double> sto,        //N*M stoechiometry matrix
-        std::vector<int>    r_env,      //reactions environments
+        std::vector<double> r_env,      //reactions environments
         std::vector<double> D,          //reactions diffusion coefficients
         std::vector<int> boundary_conditions,
         int sample_n,                   //number of sample timepoints
         std::vector<double> t_samples,  //sample timepoints
         int sampling_policy_code,       //tells when the system state should be sampled
         double sampling_interval,       //interval at which the system state should be sampled (if sampling_policy_code=2)
         double t_max,                   //time past which the simulation should be flagged as complete (if negative, there is no t_max).
```

### Comparing `strengths-0.0.8/src/strengths/engines/strengths_engine/src/TauLeap3D.hpp` & `strengths-0.0.9/src/strengths/engines/strengths_engine/src/TauLeap3D.hpp`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/engines/strengths_engine/src/engine.cpp` & `strengths-0.0.9/src/strengths/engines/strengths_engine/src/engine.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 #include "SimulationAlgorithmGraphBase.hpp"
 #include "EulerGraph.hpp"
 #include "TauLeapGraph.hpp"
 #include "GillespieGraph.hpp"
 
 #include <chrono>
 
+#ifdef CPYEMVER
+  #include <Python.h>
+
+  extern "C" PyObject * PyInit_engine()
+    {
+    return NULL;
+    }
+#endif
+
 std::vector<double> GenerateStochasticDistribution (std::vector<double> mesh_x, int n_meshes, int n_species, int seed)
   {
   /// generate a poisson distributed stochastic state that respects the floored total quantities of the input floating point state.
 
   std::mt19937 rng(seed);
   std::uniform_real_distribution<double> uiud(0, 1);
 
@@ -114,33 +123,20 @@
       if(delta_count == delta) break;
       }
     }
 
   return mesh_x_sto;
   }
 
-template <typename T_in, typename T_out>
-std::vector<T_out> ConvertVector(std::vector<T_in> & v_in)
-    {
-    std::vector<T_out> v_out(v_in.size());
-    for(size_t i=0; i<v_in.size(); i++)
-        {
-        v_out[i] = static_cast<T_out>(v_in[i]);
-        }
-    return v_out;
-    }
-
-template<typename T_out, typename T_in> std::vector<T_out> MkVec(T_in * a, int len, bool floor_values = false)
+template<typename T_out, typename T_in> std::vector<T_out> MkVec(T_in * a, int len)
     {
     std::vector<T_out> v(len);
     for(int i=0;i<len;i++)
         {
         v[i] = static_cast<T_out>(a[i]);
-        if(floor_values)
-            v[i] = floor(v[i]);
         }
     return v;
     }
 
 SimulationAlgorithm3DBase * global_grid_algo;
 SimulationAlgorithmGraphBase * global_graph_algo;
 int global_space_type; //0 : grid, 1 : graph
@@ -235,22 +231,22 @@
 
     std::vector<double> mesh_x;
     bool is_stochastic = (CompareStr(option, "tauleap") || CompareStr(option, "gillespie"));
 
     if(is_stochastic)
       {
       mesh_x = GenerateStochasticDistribution (
-        SpeciesFirstToMeshFirstArray(MkVec<double, double>(mesh_state, n_meshes*n_species, false), n_species, n_meshes),
+        SpeciesFirstToMeshFirstArray(MkVec<double, double>(mesh_state, n_meshes*n_species), n_species, n_meshes),
         n_meshes,
         n_species,
         seed);
       }
     else
       {
-      mesh_x = SpeciesFirstToMeshFirstArray(MkVec<double, double>(mesh_state, n_meshes*n_species, false), n_species, n_meshes);
+      mesh_x = SpeciesFirstToMeshFirstArray(MkVec<double, double>(mesh_state, n_meshes*n_species), n_species, n_meshes);
       }
 
     global_grid_algo->Init(
           w,
           h,
           d,
           n_species,
@@ -261,15 +257,15 @@
                                        n_species,
                                        n_meshes), //species first to mesh first
           MkVec<int,    int   >(mesh_env, n_meshes),
           mesh_vol,
           MkVec<double, double>(k, n_reactions),
           MkVec<double, int   >(sub, n_species*n_reactions),
           MkVec<double, int   >(sto, n_species*n_reactions),
-          MkVec<int,    int   >(r_env, n_reactions*n_env),
+          MkVec<double, int   >(r_env, n_reactions*n_env),
           MkVec<double, double>(D, n_species*n_env),
           boundary_conditions,
           sample_n,
           MkVec<double, double>(sample_t, sample_n),
 
           sampling_policy_code,
           sampling_interval,
@@ -345,22 +341,22 @@
 
     std::vector<double> mesh_x;
     bool is_stochastic = (CompareStr(option, "tauleap") || CompareStr(option, "gillespie"));
 
     if(is_stochastic)
       {
       mesh_x = GenerateStochasticDistribution (
-        SpeciesFirstToMeshFirstArray(MkVec<double, double>(mesh_state, n_meshes*n_species, false), n_species, n_meshes),
+        SpeciesFirstToMeshFirstArray(MkVec<double, double>(mesh_state, n_meshes*n_species), n_species, n_meshes),
         n_meshes,
         n_species,
         seed);
       }
     else
       {
-      mesh_x = SpeciesFirstToMeshFirstArray(MkVec<double, double>(mesh_state, n_meshes*n_species, false), n_species, n_meshes);
+      mesh_x = SpeciesFirstToMeshFirstArray(MkVec<double, double>(mesh_state, n_meshes*n_species), n_species, n_meshes);
       }
 
     global_graph_algo->Init(
           n_meshes,
           n_species,
           n_reactions,
           n_env,
@@ -379,15 +375,15 @@
           MkVec<int,    int   >(mesh_env, n_meshes),
           MkVec<double,    double>(mesh_vol, n_meshes),
 
 
           MkVec<double, double>(k, n_reactions),
           MkVec<double, int   >(sub, n_species*n_reactions),
           MkVec<double, int   >(sto, n_species*n_reactions),
-          MkVec<int,    int   >(r_env, n_reactions*n_env),
+          MkVec<double, int   >(r_env, n_reactions*n_env),
           MkVec<double, double>(D, n_species*n_env),
 
           sample_n,
           MkVec<double, double>(sample_t, sample_n),
 
           sampling_policy_code,
           sampling_interval,
@@ -404,15 +400,15 @@
     {
     bool unfinished = true;
     auto t0 = std::chrono::system_clock::now();
     for(;;)
         {
         if      (global_space_type == 0) unfinished = global_grid_algo->Iterate();
         else if (global_space_type == 1) unfinished = global_graph_algo->Iterate();
-        int dt = std::chrono::duration_cast<std::chrono::milliseconds>(std::chrono::system_clock::now() - t0).count();
+        int dt = static_cast<int>(std::chrono::duration_cast<std::chrono::milliseconds>(std::chrono::system_clock::now() - t0).count());
         if(!unfinished || dt>=breathe_dt)
             break;
         }
     return unfinished;
     }
 
 extern "C" int IterateN(int n_iterations)
@@ -574,14 +570,23 @@
     {
     if (global_space_type == 0)
       return global_grid_algo->NSamples();
     else
       return global_graph_algo->NSamples();
     }
 
+extern "C" int Sample()
+    {
+    if (global_space_type == 0)
+      global_grid_algo->Sample();
+    else
+      global_graph_algo->Sample();
+    return 0;
+    }
+
 extern "C" int Finalize ()
     {
     if(global_algo_freed)
       return 0;
 
     if (global_space_type == 0)
       delete global_grid_algo;
```

### Comparing `strengths-0.0.8/src/strengths/filepath.py` & `strengths-0.0.9/src/strengths/filepath.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/kinetics.py` & `strengths-0.0.9/src/strengths/kinetics.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/kineticsrdengine.py` & `strengths-0.0.9/src/strengths/kineticsrdengine.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/librdengine.py` & `strengths-0.0.9/src/strengths/librdengine.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/plot.py` & `strengths-0.0.9/src/strengths/plot.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/rdengine.py` & `strengths-0.0.9/src/strengths/rdengine.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/rdgraphspace.py` & `strengths-0.0.9/src/strengths/rdgraphspace.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/rdgridspace.py` & `strengths-0.0.9/src/strengths/rdgridspace.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/rdnetwork.py` & `strengths-0.0.9/src/strengths/rdnetwork.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/rdoutput.py` & `strengths-0.0.9/src/strengths/rdoutput.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/rdscript.py` & `strengths-0.0.9/src/strengths/rdscript.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/rdspace.py` & `strengths-0.0.9/src/strengths/rdspace.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/rdsystem.py` & `strengths-0.0.9/src/strengths/rdsystem.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/simulate.py` & `strengths-0.0.9/src/strengths/simulate.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/typechecking.py` & `strengths-0.0.9/src/strengths/typechecking.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/units.py` & `strengths-0.0.9/src/strengths/units.py`

 * *Files identical despite different names*

### Comparing `strengths-0.0.8/src/strengths/value_processing.py` & `strengths-0.0.9/src/strengths/value_processing.py`

 * *Files identical despite different names*

