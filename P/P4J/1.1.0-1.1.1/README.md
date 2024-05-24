# Comparing `tmp/p4j-1.1.0.tar.gz` & `tmp/p4j-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p4j-1.1.0.tar", last modified: Fri May 24 20:23:48 2024, max compression
+gzip compressed data, was "p4j-1.1.1.tar", last modified: Fri May 24 20:47:53 2024, max compression
```

## Comparing `p4j-1.1.0.tar` & `p4j-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.745179 p4j-1.1.0/
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1085 2022-09-06 19:58:41.000000 p4j-1.1.0/LICENSE
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)     5261 2024-05-24 20:23:48.745179 p4j-1.1.0/PKG-INFO
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)     4500 2024-05-24 19:56:42.000000 p4j-1.1.0/README.md
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1037 2024-05-24 20:07:16.000000 p4j-1.1.0/pyproject.toml
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)       38 2024-05-24 20:23:48.745179 p4j-1.1.0/setup.cfg
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)      910 2024-05-18 10:47:26.000000 p4j-1.1.0/setup.py
-drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.738512 p4j-1.1.0/src/
-drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.741846 p4j-1.1.0/src/P4J/
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1136 2024-05-24 19:47:32.000000 p4j-1.1.0/src/P4J/__init__.py
-drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.745179 p4j-1.1.0/src/P4J/algorithms/
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)        0 2022-09-06 19:58:41.000000 p4j-1.1.0/src/P4J/algorithms/__init__.py
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1084450 2024-05-24 20:23:46.000000 p4j-1.1.0/src/P4J/algorithms/analysis_of_variance.c
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1087413 2024-05-24 20:23:46.000000 p4j-1.1.0/src/P4J/algorithms/multiharmonic_aov.c
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1109454 2024-05-24 20:23:47.000000 p4j-1.1.0/src/P4J/algorithms/mutual_information.c
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1063964 2024-05-24 20:23:47.000000 p4j-1.1.0/src/P4J/algorithms/phase_dispersion_minimization.c
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1050607 2024-05-24 20:23:47.000000 p4j-1.1.0/src/P4J/algorithms/string_length.c
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)   178817 2024-05-24 20:23:47.000000 p4j-1.1.0/src/P4J/algorithms/utilities.c
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)     3429 2024-05-23 16:03:37.000000 p4j-1.1.0/src/P4J/base_periodogram.py
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)    11977 2024-05-23 18:10:57.000000 p4j-1.1.0/src/P4J/generator.py
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1883 2022-09-06 19:58:41.000000 p4j-1.1.0/src/P4J/math.py
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)     9791 2022-09-06 19:58:41.000000 p4j-1.1.0/src/P4J/periodograms.py
-drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.745179 p4j-1.1.0/src/P4J.egg-info/
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)     5261 2024-05-24 20:23:48.000000 p4j-1.1.0/src/P4J.egg-info/PKG-INFO
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)      659 2024-05-24 20:23:48.000000 p4j-1.1.0/src/P4J.egg-info/SOURCES.txt
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)        1 2024-05-24 20:23:48.000000 p4j-1.1.0/src/P4J.egg-info/dependency_links.txt
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)       18 2024-05-24 20:23:48.000000 p4j-1.1.0/src/P4J.egg-info/requires.txt
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)        4 2024-05-24 20:23:48.000000 p4j-1.1.0/src/P4J.egg-info/top_level.txt
-drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.745179 p4j-1.1.0/tests/
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)      463 2022-09-06 19:58:41.000000 p4j-1.1.0/tests/test_generator.py
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1268 2022-09-06 19:58:41.000000 p4j-1.1.0/tests/test_multiband_periodogram.py
--rw-r--r--   0 phuijse   (1000) phuijse   (1000)     3083 2022-09-06 19:58:41.000000 p4j-1.1.0/tests/test_periodogram.py
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:47:53.313759 p4j-1.1.1/
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1085 2022-09-06 19:58:41.000000 p4j-1.1.1/LICENSE
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     5262 2024-05-24 20:47:53.313759 p4j-1.1.1/PKG-INFO
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     4500 2024-05-24 19:56:42.000000 p4j-1.1.1/README.md
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1038 2024-05-24 20:35:23.000000 p4j-1.1.1/pyproject.toml
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)       38 2024-05-24 20:47:53.313759 p4j-1.1.1/setup.cfg
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)      910 2024-05-18 10:47:26.000000 p4j-1.1.1/setup.py
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:47:53.307092 p4j-1.1.1/src/
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:47:53.307092 p4j-1.1.1/src/P4J/
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1136 2024-05-24 20:46:30.000000 p4j-1.1.1/src/P4J/__init__.py
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:47:53.313759 p4j-1.1.1/src/P4J/algorithms/
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)        0 2022-09-06 19:58:41.000000 p4j-1.1.1/src/P4J/algorithms/__init__.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1084450 2024-05-24 20:36:35.000000 p4j-1.1.1/src/P4J/algorithms/analysis_of_variance.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1087413 2024-05-24 20:36:35.000000 p4j-1.1.1/src/P4J/algorithms/multiharmonic_aov.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1109454 2024-05-24 20:36:36.000000 p4j-1.1.1/src/P4J/algorithms/mutual_information.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1063964 2024-05-24 20:36:36.000000 p4j-1.1.1/src/P4J/algorithms/phase_dispersion_minimization.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1050607 2024-05-24 20:36:37.000000 p4j-1.1.1/src/P4J/algorithms/string_length.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)   178817 2024-05-24 20:36:37.000000 p4j-1.1.1/src/P4J/algorithms/utilities.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     3429 2024-05-23 16:03:37.000000 p4j-1.1.1/src/P4J/base_periodogram.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)    11977 2024-05-23 18:10:57.000000 p4j-1.1.1/src/P4J/generator.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1883 2022-09-06 19:58:41.000000 p4j-1.1.1/src/P4J/math.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     9791 2022-09-06 19:58:41.000000 p4j-1.1.1/src/P4J/periodograms.py
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:47:53.313759 p4j-1.1.1/src/P4J.egg-info/
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     5262 2024-05-24 20:47:53.000000 p4j-1.1.1/src/P4J.egg-info/PKG-INFO
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)      659 2024-05-24 20:47:53.000000 p4j-1.1.1/src/P4J.egg-info/SOURCES.txt
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)        1 2024-05-24 20:47:53.000000 p4j-1.1.1/src/P4J.egg-info/dependency_links.txt
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)       19 2024-05-24 20:47:53.000000 p4j-1.1.1/src/P4J.egg-info/requires.txt
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)        4 2024-05-24 20:47:53.000000 p4j-1.1.1/src/P4J.egg-info/top_level.txt
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:47:53.313759 p4j-1.1.1/tests/
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)      463 2022-09-06 19:58:41.000000 p4j-1.1.1/tests/test_generator.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1268 2022-09-06 19:58:41.000000 p4j-1.1.1/tests/test_multiband_periodogram.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     3083 2022-09-06 19:58:41.000000 p4j-1.1.1/tests/test_periodogram.py
```

### Comparing `p4j-1.1.0/LICENSE` & `p4j-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `p4j-1.1.0/PKG-INFO` & `p4j-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: P4J
-Version: 1.1.0
+Version: 1.1.1
 Summary: Periodic light curve analysis tools based on Information Theory
 Author-email: Pablo Huijse <pablo.huijse@gmail.com>
 Project-URL: Homepage, https://github.com/phuijse/P4J
 Project-URL: Repository, https://github.com/phuijse/P4J
 Keywords: astronomy,time series,period estimation,information theory
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>1.9.0
+Requires-Dist: numpy>1.19.0
 Requires-Dist: scipy
 
 # P4J
 
 ## Description
 
 P4J is a python package for period detection on irregularly sampled and heteroscedastic time series based on *Information Theoretic* objective functions. P4J was developed for astronomical light curves, irregularly sampled time series of stellar magnitude or flux. The core of this package is a class called periodogram that sweeps an array of periods/frequencies looking for the one that maximizes a given criterion. The main contribution of this work is a criterion for period detection based on the maximization of Cauchy-Schwarz Quadratic Mutual Information (Huijse et al., 2017). Information theoretic criteria incorporate information on the whole probability density function of the process and are more robust than classical second-order statistics based criteria (Principe, 2010). For comparison P4J also incorporates other period detection methods used in astronomy such as the Phase Dispersion Minimization periodogram (Stellingwerf, 1973), Lafler-Kinman's string length (Clarke, 2002) and the Orthogonal multiharmonic AoV periodogram (Schwarzenberg-Czerny, 1996).
```

### Comparing `p4j-1.1.0/README.md` & `p4j-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `p4j-1.1.0/pyproject.toml` & `p4j-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "P4J"
 dynamic = ["version"]
 dependencies = [
-  "numpy>1.9.0",
+  "numpy>1.19.0",
   "scipy"
 ]
 requires-python = ">=3.8"
 authors = [{name = "Pablo Huijse", email = "pablo.huijse@gmail.com"}]
 description = "Periodic light curve analysis tools based on Information Theory"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
```

### Comparing `p4j-1.1.0/setup.py` & `p4j-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `p4j-1.1.0/src/P4J/__init__.py` & `p4j-1.1.1/src/P4J/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 more robust than classical second-order statistics based criteria [2, 3, 4].
 For comparison P4J also incorporates classical methods for period detection
 used in astronomy such as Phase Dispersion Minimization [5], Lafler-Kinman's
 string length [6], and the orthogonal multiharmonic AoV periodogram [7].
 
 """
 
-__version__ = '1.1.0'
+__version__ = '1.1.1'
 
 from .generator import synthetic_light_curve_generator
 from .periodograms import periodogram, MultiBandPeriodogram
```

### Comparing `p4j-1.1.0/src/P4J/algorithms/analysis_of_variance.c` & `p4j-1.1.1/src/P4J/algorithms/analysis_of_variance.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         "depends": [],
         "extra_compile_args": [
             "-O3",
             "-ffast-math"
         ],
         "include_dirs": [
             ".",
-            "/tmp/build-env-3iyu44p0/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-71zr5fnz/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "P4J.algorithms.analysis_of_variance",
         "sources": [
             "src/P4J/algorithms/analysis_of_variance.pyx"
```

### Comparing `p4j-1.1.0/src/P4J/algorithms/multiharmonic_aov.c` & `p4j-1.1.1/src/P4J/algorithms/multiharmonic_aov.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         "depends": [],
         "extra_compile_args": [
             "-O3",
             "-ffast-math"
         ],
         "include_dirs": [
             ".",
-            "/tmp/build-env-3iyu44p0/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-71zr5fnz/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "P4J.algorithms.multiharmonic_aov",
         "sources": [
             "src/P4J/algorithms/multiharmonic_aov.pyx"
```

### Comparing `p4j-1.1.0/src/P4J/algorithms/mutual_information.c` & `p4j-1.1.1/src/P4J/algorithms/mutual_information.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         "depends": [],
         "extra_compile_args": [
             "-O3",
             "-ffast-math"
         ],
         "include_dirs": [
             ".",
-            "/tmp/build-env-3iyu44p0/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-71zr5fnz/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "P4J.algorithms.mutual_information",
         "sources": [
             "src/P4J/algorithms/mutual_information.pyx"
```

### Comparing `p4j-1.1.0/src/P4J/algorithms/phase_dispersion_minimization.c` & `p4j-1.1.1/src/P4J/algorithms/phase_dispersion_minimization.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         "depends": [],
         "extra_compile_args": [
             "-O3",
             "-ffast-math"
         ],
         "include_dirs": [
             ".",
-            "/tmp/build-env-3iyu44p0/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-71zr5fnz/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "P4J.algorithms.phase_dispersion_minimization",
         "sources": [
             "src/P4J/algorithms/phase_dispersion_minimization.pyx"
```

### Comparing `p4j-1.1.0/src/P4J/algorithms/string_length.c` & `p4j-1.1.1/src/P4J/algorithms/string_length.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         "depends": [],
         "extra_compile_args": [
             "-O3",
             "-ffast-math"
         ],
         "include_dirs": [
             ".",
-            "/tmp/build-env-3iyu44p0/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-71zr5fnz/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "P4J.algorithms.string_length",
         "sources": [
             "src/P4J/algorithms/string_length.pyx"
```

### Comparing `p4j-1.1.0/src/P4J/algorithms/utilities.c` & `p4j-1.1.1/src/P4J/algorithms/utilities.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         "depends": [],
         "extra_compile_args": [
             "-O3",
             "-ffast-math"
         ],
         "include_dirs": [
             ".",
-            "/tmp/build-env-3iyu44p0/lib/python3.8/site-packages/numpy/core/include"
+            "/tmp/build-env-71zr5fnz/lib/python3.8/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "P4J.algorithms.utilities",
         "sources": [
             "src/P4J/algorithms/utilities.pyx"
```

### Comparing `p4j-1.1.0/src/P4J/base_periodogram.py` & `p4j-1.1.1/src/P4J/base_periodogram.py`

 * *Files identical despite different names*

### Comparing `p4j-1.1.0/src/P4J/generator.py` & `p4j-1.1.1/src/P4J/generator.py`

 * *Files identical despite different names*

### Comparing `p4j-1.1.0/src/P4J/math.py` & `p4j-1.1.1/src/P4J/math.py`

 * *Files identical despite different names*

### Comparing `p4j-1.1.0/src/P4J/periodograms.py` & `p4j-1.1.1/src/P4J/periodograms.py`

 * *Files identical despite different names*

### Comparing `p4j-1.1.0/src/P4J.egg-info/PKG-INFO` & `p4j-1.1.1/src/P4J.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: P4J
-Version: 1.1.0
+Version: 1.1.1
 Summary: Periodic light curve analysis tools based on Information Theory
 Author-email: Pablo Huijse <pablo.huijse@gmail.com>
 Project-URL: Homepage, https://github.com/phuijse/P4J
 Project-URL: Repository, https://github.com/phuijse/P4J
 Keywords: astronomy,time series,period estimation,information theory
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>1.9.0
+Requires-Dist: numpy>1.19.0
 Requires-Dist: scipy
 
 # P4J
 
 ## Description
 
 P4J is a python package for period detection on irregularly sampled and heteroscedastic time series based on *Information Theoretic* objective functions. P4J was developed for astronomical light curves, irregularly sampled time series of stellar magnitude or flux. The core of this package is a class called periodogram that sweeps an array of periods/frequencies looking for the one that maximizes a given criterion. The main contribution of this work is a criterion for period detection based on the maximization of Cauchy-Schwarz Quadratic Mutual Information (Huijse et al., 2017). Information theoretic criteria incorporate information on the whole probability density function of the process and are more robust than classical second-order statistics based criteria (Principe, 2010). For comparison P4J also incorporates other period detection methods used in astronomy such as the Phase Dispersion Minimization periodogram (Stellingwerf, 1973), Lafler-Kinman's string length (Clarke, 2002) and the Orthogonal multiharmonic AoV periodogram (Schwarzenberg-Czerny, 1996).
```

### Comparing `p4j-1.1.0/src/P4J.egg-info/SOURCES.txt` & `p4j-1.1.1/src/P4J.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p4j-1.1.0/tests/test_multiband_periodogram.py` & `p4j-1.1.1/tests/test_multiband_periodogram.py`

 * *Files identical despite different names*

### Comparing `p4j-1.1.0/tests/test_periodogram.py` & `p4j-1.1.1/tests/test_periodogram.py`

 * *Files identical despite different names*

