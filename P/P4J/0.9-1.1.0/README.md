# Comparing `tmp/P4J-0.9.tar.gz` & `tmp/p4j-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/P4J-0.9.tar", last modified: Mon Jul 25 19:22:04 2016, max compression
+gzip compressed data, was "p4j-1.1.0.tar", last modified: Fri May 24 20:23:48 2024, max compression
```

## Comparing `P4J-0.9.tar` & `p4j-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxr-xr-x   0 phuijse   (1000) users      (100)        0 2016-07-25 19:22:04.000000 P4J-0.9/
--rw-r--r--   0 phuijse   (1000) users      (100)     2110 2016-07-23 02:10:51.000000 P4J-0.9/README.md
--rw-r--r--   0 phuijse   (1000) users      (100)     3383 2016-07-25 19:22:04.000000 P4J-0.9/PKG-INFO
-drwxr-xr-x   0 phuijse   (1000) users      (100)        0 2016-07-25 19:22:04.000000 P4J-0.9/P4J.egg-info/
--rw-r--r--   0 phuijse   (1000) root         (0)        4 2016-07-25 19:22:04.000000 P4J-0.9/P4J.egg-info/top_level.txt
--rw-r--r--   0 phuijse   (1000) root         (0)     3383 2016-07-25 19:22:04.000000 P4J-0.9/P4J.egg-info/PKG-INFO
--rw-r--r--   0 phuijse   (1000) root         (0)        1 2016-07-25 19:22:04.000000 P4J-0.9/P4J.egg-info/dependency_links.txt
--rw-r--r--   0 phuijse   (1000) root         (0)      467 2016-07-25 19:22:04.000000 P4J-0.9/P4J.egg-info/SOURCES.txt
--rw-r--r--   0 phuijse   (1000) root         (0)       12 2016-07-25 19:22:04.000000 P4J-0.9/P4J.egg-info/requires.txt
--rw-r--r--   0 phuijse   (1000) users      (100)       78 2016-07-12 22:08:36.000000 P4J-0.9/MANIFEST.in
-drwxr-xr-x   0 phuijse   (1000) users      (100)        0 2016-07-25 19:22:04.000000 P4J-0.9/examples/
-drwxr-xr-x   0 phuijse   (1000) users      (100)        0 2016-07-25 19:22:04.000000 P4J-0.9/examples/.ipynb_checkpoints/
--rw-r--r--   0 phuijse   (1000) users      (100)   136779 2016-07-23 02:19:28.000000 P4J-0.9/examples/.ipynb_checkpoints/periodogram_demo-checkpoint.ipynb
--rw-r--r--   0 phuijse   (1000) users      (100)   138284 2016-07-23 02:20:19.000000 P4J-0.9/examples/.ipynb_checkpoints/regression_demo-checkpoint.ipynb
--rw-r--r--   0 phuijse   (1000) users      (100)   136779 2016-07-23 02:19:28.000000 P4J-0.9/examples/periodogram_demo.ipynb
--rw-r--r--   0 phuijse   (1000) users      (100)   138284 2016-07-23 02:20:19.000000 P4J-0.9/examples/regression_demo.ipynb
--rw-r--r--   0 phuijse   (1000) users      (100)      101 2016-07-25 19:22:04.000000 P4J-0.9/setup.cfg
--rw-r--r--   0 phuijse   (1000) users      (100)     1691 2016-07-15 00:32:59.000000 P4J-0.9/setup.py
--rw-r--r--   0 phuijse   (1000) users      (100)     1085 2016-07-10 21:38:51.000000 P4J-0.9/LICENSE
-drwxr-xr-x   0 phuijse   (1000) users      (100)        0 2016-07-25 19:22:04.000000 P4J-0.9/P4J/
--rw-r--r--   0 phuijse   (1000) users      (100)     9973 2016-07-25 19:20:19.000000 P4J-0.9/P4J/periodogram.py
--rw-r--r--   0 phuijse   (1000) users      (100)    11976 2016-07-23 19:34:34.000000 P4J-0.9/P4J/generator.py
--rw-r--r--   0 phuijse   (1000) users      (100)      226 2016-07-25 19:20:51.000000 P4J-0.9/P4J/__init__.py
--rw-r--r--   0 phuijse   (1000) users      (100)      414 2016-07-14 22:54:02.000000 P4J-0.9/P4J/dictionary.py
--rw-r--r--   0 phuijse   (1000) users      (100)     4861 2016-07-22 22:23:55.000000 P4J-0.9/P4J/regression.py
--rw-r--r--   0 phuijse   (1000) users      (100)     2076 2016-07-15 00:28:08.000000 P4J-0.9/README.rst
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.745179 p4j-1.1.0/
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1085 2022-09-06 19:58:41.000000 p4j-1.1.0/LICENSE
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     5261 2024-05-24 20:23:48.745179 p4j-1.1.0/PKG-INFO
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     4500 2024-05-24 19:56:42.000000 p4j-1.1.0/README.md
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1037 2024-05-24 20:07:16.000000 p4j-1.1.0/pyproject.toml
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)       38 2024-05-24 20:23:48.745179 p4j-1.1.0/setup.cfg
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)      910 2024-05-18 10:47:26.000000 p4j-1.1.0/setup.py
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.738512 p4j-1.1.0/src/
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.741846 p4j-1.1.0/src/P4J/
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1136 2024-05-24 19:47:32.000000 p4j-1.1.0/src/P4J/__init__.py
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.745179 p4j-1.1.0/src/P4J/algorithms/
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)        0 2022-09-06 19:58:41.000000 p4j-1.1.0/src/P4J/algorithms/__init__.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1084450 2024-05-24 20:23:46.000000 p4j-1.1.0/src/P4J/algorithms/analysis_of_variance.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1087413 2024-05-24 20:23:46.000000 p4j-1.1.0/src/P4J/algorithms/multiharmonic_aov.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1109454 2024-05-24 20:23:47.000000 p4j-1.1.0/src/P4J/algorithms/mutual_information.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1063964 2024-05-24 20:23:47.000000 p4j-1.1.0/src/P4J/algorithms/phase_dispersion_minimization.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)  1050607 2024-05-24 20:23:47.000000 p4j-1.1.0/src/P4J/algorithms/string_length.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)   178817 2024-05-24 20:23:47.000000 p4j-1.1.0/src/P4J/algorithms/utilities.c
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     3429 2024-05-23 16:03:37.000000 p4j-1.1.0/src/P4J/base_periodogram.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)    11977 2024-05-23 18:10:57.000000 p4j-1.1.0/src/P4J/generator.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1883 2022-09-06 19:58:41.000000 p4j-1.1.0/src/P4J/math.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     9791 2022-09-06 19:58:41.000000 p4j-1.1.0/src/P4J/periodograms.py
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.745179 p4j-1.1.0/src/P4J.egg-info/
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     5261 2024-05-24 20:23:48.000000 p4j-1.1.0/src/P4J.egg-info/PKG-INFO
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)      659 2024-05-24 20:23:48.000000 p4j-1.1.0/src/P4J.egg-info/SOURCES.txt
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)        1 2024-05-24 20:23:48.000000 p4j-1.1.0/src/P4J.egg-info/dependency_links.txt
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)       18 2024-05-24 20:23:48.000000 p4j-1.1.0/src/P4J.egg-info/requires.txt
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)        4 2024-05-24 20:23:48.000000 p4j-1.1.0/src/P4J.egg-info/top_level.txt
+drwxr-xr-x   0 phuijse   (1000) phuijse   (1000)        0 2024-05-24 20:23:48.745179 p4j-1.1.0/tests/
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)      463 2022-09-06 19:58:41.000000 p4j-1.1.0/tests/test_generator.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     1268 2022-09-06 19:58:41.000000 p4j-1.1.0/tests/test_multiband_periodogram.py
+-rw-r--r--   0 phuijse   (1000) phuijse   (1000)     3083 2022-09-06 19:58:41.000000 p4j-1.1.0/tests/test_periodogram.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `P4J-0.9/LICENSE` & `p4j-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `P4J-0.9/P4J/generator.py` & `p4j-1.1.0/src/P4J/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
     s: ndarray
         Vector containing the uncertainties
     expected_s_2: float
         Expectation of the square of s computed analytically
         
     """
     np.random.seed(rseed)  
-    print(dist)
+    #print(dist)
     if dist == 'EMG':  # Exponential modified Gaussian
         # the mean of a EMG rv is mu + 1/(K*sigma)
         # the variance of a EMG rv is sigma**2 + 1/(K*sigma)**2
         K = 1.824328605481941
         sigma = 0.05*0.068768312946785953
         mu = 0.05*0.87452567616276777
         # IMPORTANT NOTE
```

