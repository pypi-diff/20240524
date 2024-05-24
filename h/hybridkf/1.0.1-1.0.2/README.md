# Comparing `tmp/hybridkf-1.0.1.tar.gz` & `tmp/hybridkf-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hybridkf-1.0.1.tar", last modified: Fri May 24 18:22:48 2024, max compression
+gzip compressed data, was "hybridkf-1.0.2.tar", last modified: Fri May 24 21:08:38 2024, max compression
```

## Comparing `hybridkf-1.0.1.tar` & `hybridkf-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 18:22:48.475611 hybridkf-1.0.1/
--rw-r--r--   0 aleckain   (501) staff       (20)     5707 2024-05-24 18:22:48.475326 hybridkf-1.0.1/PKG-INFO
--rw-r--r--   0 aleckain   (501) staff       (20)     5192 2024-05-24 17:56:29.000000 hybridkf-1.0.1/README.md
-drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 18:22:48.475116 hybridkf-1.0.1/hybridkf.egg-info/
--rw-r--r--   0 aleckain   (501) staff       (20)     5707 2024-05-24 18:22:48.000000 hybridkf-1.0.1/hybridkf.egg-info/PKG-INFO
--rw-r--r--   0 aleckain   (501) staff       (20)      177 2024-05-24 18:22:48.000000 hybridkf-1.0.1/hybridkf.egg-info/SOURCES.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 18:22:48.000000 hybridkf-1.0.1/hybridkf.egg-info/dependency_links.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       23 2024-05-24 18:22:48.000000 hybridkf-1.0.1/hybridkf.egg-info/requires.txt
--rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 18:22:48.000000 hybridkf-1.0.1/hybridkf.egg-info/top_level.txt
--rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-24 18:22:48.475673 hybridkf-1.0.1/setup.cfg
--rw-r--r--   0 aleckain   (501) staff       (20)      783 2024-05-24 18:22:31.000000 hybridkf-1.0.1/setup.py
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:08:38.690578 hybridkf-1.0.2/
+-rw-r--r--   0 aleckain   (501) staff       (20)     5775 2024-05-24 21:08:38.690317 hybridkf-1.0.2/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)     5192 2024-05-24 17:56:29.000000 hybridkf-1.0.2/README.md
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:08:38.688786 hybridkf-1.0.2/hybridkf/
+-rw-r--r--   0 aleckain   (501) staff       (20)       36 2024-05-24 21:05:14.000000 hybridkf-1.0.2/hybridkf/__init__.py
+-rw-r--r--   0 aleckain   (501) staff       (20)     9514 2024-05-24 20:57:59.000000 hybridkf-1.0.2/hybridkf/main.py
+drwxr-xr-x   0 aleckain   (501) staff       (20)        0 2024-05-24 21:08:38.690054 hybridkf-1.0.2/hybridkf.egg-info/
+-rw-r--r--   0 aleckain   (501) staff       (20)     5775 2024-05-24 21:08:38.000000 hybridkf-1.0.2/hybridkf.egg-info/PKG-INFO
+-rw-r--r--   0 aleckain   (501) staff       (20)      215 2024-05-24 21:08:38.000000 hybridkf-1.0.2/hybridkf.egg-info/SOURCES.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        1 2024-05-24 21:08:38.000000 hybridkf-1.0.2/hybridkf.egg-info/dependency_links.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       23 2024-05-24 21:08:38.000000 hybridkf-1.0.2/hybridkf.egg-info/requires.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)        9 2024-05-24 21:08:38.000000 hybridkf-1.0.2/hybridkf.egg-info/top_level.txt
+-rw-r--r--   0 aleckain   (501) staff       (20)       38 2024-05-24 21:08:38.690626 hybridkf-1.0.2/setup.cfg
+-rw-r--r--   0 aleckain   (501) staff       (20)      783 2024-05-24 21:06:46.000000 hybridkf-1.0.2/setup.py
```

### Comparing `hybridkf-1.0.1/PKG-INFO` & `hybridkf-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: hybridkf
-Version: 1.0.1
+Version: 1.0.2
 Summary: An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.
 Home-page: https://github.com/akain0/hybridkf
 Author: akain0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
 
 # Hybrid Kalman Filter (hybridkf)
 
 [![PyPI version](https://badge.fury.io/py/hybridkf.svg)](https://badge.fury.io/py/hybridkf)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 The Hybrid Kalman Filter (HKF) is an extension of the traditional Kalman filter that combines elements of both linear and nonlinear models to provide accurate state estimation in dynamic systems. It is particularly useful in scenarios where the underlying system dynamics exhibit both linear and nonlinear behavior with regards to physical systems that exhibit a continuous-time model and discrete-time measurements are recorded for state estimation.
```

### Comparing `hybridkf-1.0.1/README.md` & `hybridkf-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hybridkf-1.0.1/hybridkf.egg-info/PKG-INFO` & `hybridkf-1.0.2/hybridkf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: hybridkf
-Version: 1.0.1
+Version: 1.0.2
 Summary: An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.
 Home-page: https://github.com/akain0/hybridkf
 Author: akain0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
 
 # Hybrid Kalman Filter (hybridkf)
 
 [![PyPI version](https://badge.fury.io/py/hybridkf.svg)](https://badge.fury.io/py/hybridkf)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 The Hybrid Kalman Filter (HKF) is an extension of the traditional Kalman filter that combines elements of both linear and nonlinear models to provide accurate state estimation in dynamic systems. It is particularly useful in scenarios where the underlying system dynamics exhibit both linear and nonlinear behavior with regards to physical systems that exhibit a continuous-time model and discrete-time measurements are recorded for state estimation.
```

### Comparing `hybridkf-1.0.1/setup.py` & `hybridkf-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hybridkf',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     description='''An advanced implementation of the Kalman filter that handles and processes (pragmatic) continuous time-model state observations with discrete time-measurements for state estimation.'''
     ,
     author='akain0',
     install_requires=[
         'numpy',
         'scipy',
```

