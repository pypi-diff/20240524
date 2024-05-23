# Comparing `tmp/dtw_python-1.4.4.tar.gz` & `tmp/dtw_python-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtw_python-1.4.4.tar", last modified: Sat May 18 16:29:50 2024, max compression
+gzip compressed data, was "dtw_python-1.5.0.tar", last modified: Thu May 23 22:25:25 2024, max compression
```

## Comparing `dtw_python-1.4.4.tar` & `dtw_python-1.5.0.tar`

### file list

```diff
@@ -1,57 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.631978 dtw_python-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-18 16:29:40.000000 dtw_python-1.4.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26255 2024-05-18 16:29:40.000000 dtw_python-1.4.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-18 16:29:40.000000 dtw_python-1.4.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 16:29:40.000000 dtw_python-1.4.4/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-18 16:29:40.000000 dtw_python-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-18 16:29:50.631978 dtw_python-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-18 16:29:40.000000 dtw_python-1.4.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.623978 dtw_python-1.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-18 16:29:40.000000 dtw_python-1.4.4/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     7350 2024-05-18 16:29:40.000000 dtw_python-1.4.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-18 16:29:40.000000 dtw_python-1.4.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-18 16:29:40.000000 dtw_python-1.4.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.627977 dtw_python-1.4.4/dtw/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/_backtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)  1204329 2024-05-18 16:29:49.000000 dtw_python-1.4.4/dtw/_dtw_utils.c
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/_dtw_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/_globalCostMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/countPaths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.627977 dtw_python-1.4.4/dtw/data/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/data/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   250698 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/data/aami3a.csv
--rw-r--r--   0 runner    (1001) docker     (127)   252781 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/data/aami3b.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/dtw.py
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/dtwPlot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/dtw_core.c
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/dtw_core.h
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/dtw_test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/mvm.py
--rw-r--r--   0 runner    (1001) docker     (127)    26034 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/stepPattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/warp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/warpArea.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-18 16:29:40.000000 dtw_python-1.4.4/dtw/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.631978 dtw_python-1.4.4/dtw_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 16:29:50.000000 dtw_python-1.4.4/dtw_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-18 16:29:40.000000 dtw_python-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-18 16:29:50.631978 dtw_python-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-18 16:29:40.000000 dtw_python-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:29:50.631978 dtw_python-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/query.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/reference.csv
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_countPaths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_cran.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_doctests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_dtw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_dtw_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-18 16:29:40.000000 dtw_python-1.4.4/tests/test_issues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.694884 dtw_python-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 22:25:18.000000 dtw_python-1.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26255 2024-05-23 22:25:18.000000 dtw_python-1.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-23 22:25:18.000000 dtw_python-1.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 22:25:18.000000 dtw_python-1.5.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-23 22:25:18.000000 dtw_python-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    48135 2024-05-23 22:25:25.694884 dtw_python-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-23 22:25:18.000000 dtw_python-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.686884 dtw_python-1.5.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7350 2024-05-23 22:25:18.000000 dtw_python-1.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.690884 dtw_python-1.5.0/dtw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/_backtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1229066 2024-05-23 22:25:24.000000 dtw_python-1.5.0/dtw/_dtw_utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/_dtw_utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/_globalCostMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/countPaths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.690884 dtw_python-1.5.0/dtw/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   250698 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/data/aami3a.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   252781 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/data/aami3b.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15695 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/dtw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/dtwPlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/dtw_core.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/dtw_core.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/dtw_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/mvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26005 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/stepPattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/warp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/warpArea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-23 22:25:18.000000 dtw_python-1.5.0/dtw/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.694884 dtw_python-1.5.0/dtw_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    48135 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-23 22:25:25.000000 dtw_python-1.5.0/dtw_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.690884 dtw_python-1.5.0/maintainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-23 22:25:18.000000 dtw_python-1.5.0/maintainer/roxypick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-23 22:25:18.000000 dtw_python-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 22:25:25.694884 dtw_python-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-23 22:25:18.000000 dtw_python-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:25:25.694884 dtw_python-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/query.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/reference.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_countPaths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_cran.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_dtw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_dtw_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-23 22:25:18.000000 dtw_python-1.5.0/tests/test_issues.py
```

### Comparing `dtw_python-1.4.4/CHANGELOG.md` & `dtw_python-1.5.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/CONTRIBUTING.rst` & `dtw_python-1.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/COPYING` & `dtw_python-1.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/PKG-INFO` & `dtw_python-1.5.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: dtw-python
-Version: 1.4.4
-Summary: A comprehensive implementation of dynamic time warping (DTW) algorithms. DTW computes the optimal (least cumulative distance) alignment between points of two time series. Common DTW variants covered include local (slope) and global (window) constraints, subsequence matches, arbitrary distance definitions, normalizations, minimum variance matching, and so on. Provides cumulative distances, alignments, specialized plot styles, etc.
-Home-page: https://DynamicTimeWarping.github.io
-Author: Toni Giorgino
-Author-email: toni.giorgino@gmail.com
-License: GNU General Public License v3
-Keywords: dtw,timeseries
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-License-File: COPYING
-License-File: AUTHORS.rst
-Requires-Dist: numpy>=1.19
-Requires-Dist: scipy>=1.1
-
 Welcome to the dtw-python package
 =================================
 
 Comprehensive implementation of `Dynamic Time Warping algorithms
 <https://dynamictimewarping.github.io>`__.
 
 DTW is a family of algorithms which compute the local stretch or
```

### Comparing `dtw_python-1.4.4/docs/conf.py` & `dtw_python-1.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/__init__.py` & `dtw_python-1.5.0/dtw/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Please see the help for the dtw.dtw() function which is the package's
 main entry point.
 
 """
 
 __author__ = """Toni Giorgino"""
 __email__ = 'toni.giorgino@gmail.com'
-__version__ = '1.4.4'
+__version__ = '1.5.0'
 
 # There are no comments in this package because it mirrors closely the R sources.
 
 # List of things to export on "from dtw import *"
 from dtw.dtw import *
 from dtw.stepPattern import *
 from dtw.countPaths import *
```

### Comparing `dtw_python-1.4.4/dtw/__main__.py` & `dtw_python-1.5.0/dtw/__main__.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/_backtrack.py` & `dtw_python-1.5.0/dtw/_backtrack.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/_dtw_utils.c` & `dtw_python-1.5.0/dtw/_dtw_utils.c`

 * *Files 1% similar despite different names*

```diff
@@ -1697,200 +1697,164 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":770
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":735
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":742
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":747
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":756
- * # The int types are mapped a bit surprising --
- * # numpy.int corresponds to 'l' and numpy.long to 'q'
- * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
- * ctypedef npy_longlong   longlong_t
- */
-typedef npy_long __pyx_t_5numpy_int_t;
-
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
- * # numpy.int corresponds to 'l' and numpy.long to 'q'
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+ * ctypedef double complex complex128_t
  * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
+ * ctypedef npy_ulonglong  ulonglong_t
  * 
- * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
- * ctypedef npy_longlong   longlong_t
- * 
- * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
- * ctypedef npy_ulonglong  ulonglong_t
- */
-typedef npy_ulong __pyx_t_5numpy_uint_t;
-
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
- * 
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
  * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":762
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
+ * ctypedef npy_longlong   longlong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":795
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":798
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":799
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":800
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
- * ctypedef npy_cfloat      cfloat_t
+ * ctypedef float complex       cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
 /* #### Code section: complex_type_declarations ### */
 /* Declarations.proto */
 #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
@@ -1910,14 +1874,26 @@
     typedef double _Complex __pyx_t_double_complex;
   #endif
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
+/* Declarations.proto */
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+  #ifdef __cplusplus
+    typedef ::std::complex< long double > __pyx_t_long_double_complex;
+  #else
+    typedef long double _Complex __pyx_t_long_double_complex;
+  #endif
+#else
+    typedef struct { long double real, imag; } __pyx_t_long_double_complex;
+#endif
+static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double, long double);
+
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 #ifndef _ARRAYARRAY_H
 struct arrayobject;
 typedef struct arrayobject arrayobject;
 #endif
@@ -1948,49 +1924,31 @@
  *     or the provided default value if no such value was found.
  */
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
- * ctypedef npy_longdouble longdouble_t
- * 
- * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
- * ctypedef npy_cdouble     cdouble_t
- * ctypedef npy_clongdouble clongdouble_t
- */
-typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
-
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1096
  * 
- * ctypedef npy_cfloat      cfloat_t
- * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
- * ctypedef npy_clongdouble clongdouble_t
+ * # Iterator API added in v1.6
+ * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil             # <<<<<<<<<<<<<<
+ * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil
  * 
  */
-typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
+typedef int (*__pyx_t_5numpy_NpyIter_IterNextFunc)(NpyIter *);
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
- * ctypedef npy_cfloat      cfloat_t
- * ctypedef npy_cdouble     cdouble_t
- * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1097
+ * # Iterator API added in v1.6
+ * ctypedef int (*NpyIter_IterNextFunc)(NpyIter* it) noexcept nogil
+ * ctypedef void (*NpyIter_GetMultiIndexFunc)(NpyIter* it, npy_intp* outcoords) noexcept nogil             # <<<<<<<<<<<<<<
  * 
- * ctypedef npy_cdouble     complex_t
+ * cdef extern from "numpy/arrayobject.h":
  */
-typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
-
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":775
- * ctypedef npy_clongdouble clongdouble_t
- * 
- * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew1(a):
- */
-typedef npy_cdouble __pyx_t_5numpy_complex_t;
+typedef void (*__pyx_t_5numpy_NpyIter_GetMultiIndexFunc)(NpyIter *, npy_intp *);
 struct __pyx_defaults;
 typedef struct __pyx_defaults __pyx_defaults;
 struct __pyx_defaults {
   __Pyx_memviewslice __pyx_arg_sm;
 };
 
 /* "View.MemoryView":114
@@ -3243,14 +3201,52 @@
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_conj_double(__pyx_t_double_complex);
     #if 1
         static CYTHON_INLINE double __Pyx_c_abs_double(__pyx_t_double_complex);
         static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_pow_double(__pyx_t_double_complex, __pyx_t_double_complex);
     #endif
 #endif
 
+/* Arithmetic.proto */
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+    #define __Pyx_c_eq_long__double(a, b)   ((a)==(b))
+    #define __Pyx_c_sum_long__double(a, b)  ((a)+(b))
+    #define __Pyx_c_diff_long__double(a, b) ((a)-(b))
+    #define __Pyx_c_prod_long__double(a, b) ((a)*(b))
+    #define __Pyx_c_quot_long__double(a, b) ((a)/(b))
+    #define __Pyx_c_neg_long__double(a)     (-(a))
+  #ifdef __cplusplus
+    #define __Pyx_c_is_zero_long__double(z) ((z)==(long double)0)
+    #define __Pyx_c_conj_long__double(z)    (::std::conj(z))
+    #if 1
+        #define __Pyx_c_abs_long__double(z)     (::std::abs(z))
+        #define __Pyx_c_pow_long__double(a, b)  (::std::pow(a, b))
+    #endif
+  #else
+    #define __Pyx_c_is_zero_long__double(z) ((z)==0)
+    #define __Pyx_c_conj_long__double(z)    (conjl(z))
+    #if 1
+        #define __Pyx_c_abs_long__double(z)     (cabsl(z))
+        #define __Pyx_c_pow_long__double(a, b)  (cpowl(a, b))
+    #endif
+ #endif
+#else
+    static CYTHON_INLINE int __Pyx_c_eq_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_sum_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_diff_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_prod_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_neg_long__double(__pyx_t_long_double_complex);
+    static CYTHON_INLINE int __Pyx_c_is_zero_long__double(__pyx_t_long_double_complex);
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_conj_long__double(__pyx_t_long_double_complex);
+    #if 1
+        static CYTHON_INLINE long double __Pyx_c_abs_long__double(__pyx_t_long_double_complex);
+        static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_pow_long__double(__pyx_t_long_double_complex, __pyx_t_long_double_complex);
+    #endif
+#endif
+
 /* MemviewSliceCopyTemplate.proto */
 static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object);
 
@@ -3323,14 +3319,26 @@
 static PyObject *__pyx_memoryview_setitem_indexed(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryview_convert_item_to_object(struct __pyx_memoryview_obj *__pyx_v_self, char *__pyx_v_itemp); /* proto*/
 static PyObject *__pyx_memoryview_assign_item_from_object(struct __pyx_memoryview_obj *__pyx_v_self, char *__pyx_v_itemp, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryview__get_base(struct __pyx_memoryview_obj *__pyx_v_self); /* proto*/
 static PyObject *__pyx_memoryviewslice_convert_item_to_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp); /* proto*/
 static PyObject *__pyx_memoryviewslice_assign_item_from_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryviewslice__get_base(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_8itemsize_itemsize(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_9alignment_alignment(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_6fields_fields(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_5names_names(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyArray_ArrayDescr *__pyx_f_5numpy_5dtype_8subarray_subarray(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_uint64 __pyx_f_5numpy_5dtype_5flags_flags(PyArray_Descr *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_7numiter_numiter(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_4size_size(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_5index_index(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_2nd_nd(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_9broadcast_10dimensions_dimensions(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE void **__pyx_f_5numpy_9broadcast_5iters_iters(PyArrayMultiIterObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self); /* proto*/
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self); /* proto*/
@@ -3630,15 +3638,14 @@
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_Dimension_d_is_not_direct[] = "Dimension %d is not direct";
 static const char __pyx_k_Index_out_of_bounds_axis_d[] = "Index out of bounds (axis %d)";
 static const char __pyx_k_Step_may_not_be_zero_axis_d[] = "Step may not be zero (axis %d)";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
-static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_All_dimensions_preceding_dimensi[] = "All dimensions preceding dimension %d must be indexed and not sliced";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Cannot_transpose_memoryview_with[] = "Cannot transpose memoryview with indirect dimensions";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
@@ -3646,15 +3653,16 @@
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got ";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis ";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_Utility_functions_for_DTW_alignm[] = "Utility functions for DTW alignments.";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension ";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
-static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
+static const char __pyx_k_numpy__core_multiarray_failed_to[] = "numpy._core.multiarray failed to import";
+static const char __pyx_k_numpy__core_umath_failed_to_impo[] = "numpy._core.umath failed to import";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 /* #### Code section: decls ### */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
@@ -3955,16 +3963,16 @@
   PyObject *__pyx_n_s_nan;
   PyObject *__pyx_n_s_ndim;
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
   PyObject *__pyx_n_s_np;
   PyObject *__pyx_n_s_nstepsp;
   PyObject *__pyx_n_s_numpy;
-  PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
-  PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
+  PyObject *__pyx_kp_u_numpy__core_multiarray_failed_to;
+  PyObject *__pyx_kp_u_numpy__core_umath_failed_to_impo;
   PyObject *__pyx_n_s_obj;
   PyObject *__pyx_n_s_ones;
   PyObject *__pyx_n_s_out;
   PyObject *__pyx_n_s_pack;
   PyObject *__pyx_n_s_pickle;
   PyObject *__pyx_n_s_pyx_PickleError;
   PyObject *__pyx_n_s_pyx_checksum;
@@ -4215,16 +4223,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_nan);
   Py_CLEAR(clear_module_state->__pyx_n_s_ndim);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_CLEAR(clear_module_state->__pyx_n_s_np);
   Py_CLEAR(clear_module_state->__pyx_n_s_nstepsp);
   Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy__core_multiarray_failed_to);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy__core_umath_failed_to_impo);
   Py_CLEAR(clear_module_state->__pyx_n_s_obj);
   Py_CLEAR(clear_module_state->__pyx_n_s_ones);
   Py_CLEAR(clear_module_state->__pyx_n_s_out);
   Py_CLEAR(clear_module_state->__pyx_n_s_pack);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
@@ -4453,16 +4461,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_nan);
   Py_VISIT(traverse_module_state->__pyx_n_s_ndim);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_VISIT(traverse_module_state->__pyx_n_s_np);
   Py_VISIT(traverse_module_state->__pyx_n_s_nstepsp);
   Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy__core_multiarray_failed_to);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy__core_umath_failed_to_impo);
   Py_VISIT(traverse_module_state->__pyx_n_s_obj);
   Py_VISIT(traverse_module_state->__pyx_n_s_ones);
   Py_VISIT(traverse_module_state->__pyx_n_s_out);
   Py_VISIT(traverse_module_state->__pyx_n_s_pack);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
@@ -4795,16 +4803,16 @@
 #define __pyx_n_s_nan __pyx_mstate_global->__pyx_n_s_nan
 #define __pyx_n_s_ndim __pyx_mstate_global->__pyx_n_s_ndim
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
 #define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
 #define __pyx_n_s_nstepsp __pyx_mstate_global->__pyx_n_s_nstepsp
 #define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
-#define __pyx_kp_u_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy_core_multiarray_failed_to
-#define __pyx_kp_u_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_u_numpy_core_umath_failed_to_impor
+#define __pyx_kp_u_numpy__core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy__core_multiarray_failed_to
+#define __pyx_kp_u_numpy__core_umath_failed_to_impo __pyx_mstate_global->__pyx_kp_u_numpy__core_umath_failed_to_impo
 #define __pyx_n_s_obj __pyx_mstate_global->__pyx_n_s_obj
 #define __pyx_n_s_ones __pyx_mstate_global->__pyx_n_s_ones
 #define __pyx_n_s_out __pyx_mstate_global->__pyx_n_s_out
 #define __pyx_n_s_pack __pyx_mstate_global->__pyx_n_s_pack
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
@@ -18508,262 +18516,686 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":286
+ * 
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ELSIZE(self)
+ * 
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_8itemsize_itemsize(PyArray_Descr *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":287
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:
+ *             return PyDataType_ELSIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyDataType_ELSIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":286
+ * 
+ *         @property
+ *         cdef inline npy_intp itemsize(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ELSIZE(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+ * 
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ALIGNMENT(self)
+ * 
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_5dtype_9alignment_alignment(PyArray_Descr *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:
+ *             return PyDataType_ALIGNMENT(self)             # <<<<<<<<<<<<<<
+ * 
+ *         # Use fields/names with care as they may be NULL.  You must check
+ */
+  __pyx_r = PyDataType_ALIGNMENT(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+ * 
+ *         @property
+ *         cdef inline npy_intp alignment(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_ALIGNMENT(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":296
+ *         # for this using PyDataType_HASFIELDS.
+ *         @property
+ *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
+ *             return <object>PyDataType_FIELDS(self)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_6fields_fields(PyArray_Descr *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1;
+  __Pyx_RefNannySetupContext("fields", 1);
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":297
+ *         @property
+ *         cdef inline object fields(self):
+ *             return <object>PyDataType_FIELDS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyDataType_FIELDS(__pyx_v_self);
+  __Pyx_INCREF(((PyObject *)__pyx_t_1));
+  __pyx_r = ((PyObject *)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":296
+ *         # for this using PyDataType_HASFIELDS.
+ *         @property
+ *         cdef inline object fields(self):             # <<<<<<<<<<<<<<
+ *             return <object>PyDataType_FIELDS(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":300
+ * 
+ *         @property
+ *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
+ *             return <tuple>PyDataType_NAMES(self)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_5dtype_5names_names(PyArray_Descr *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1;
+  __Pyx_RefNannySetupContext("names", 1);
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":301
+ *         @property
+ *         cdef inline tuple names(self):
+ *             return <tuple>PyDataType_NAMES(self)             # <<<<<<<<<<<<<<
+ * 
+ *         # Use PyDataType_HASSUBARRAY to test whether this field is
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyDataType_NAMES(__pyx_v_self);
+  __Pyx_INCREF(((PyObject*)__pyx_t_1));
+  __pyx_r = ((PyObject*)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":300
+ * 
+ *         @property
+ *         cdef inline tuple names(self):             # <<<<<<<<<<<<<<
+ *             return <tuple>PyDataType_NAMES(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":307
+ *         # this field via the inline helper method PyDataType_SHAPE.
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_SUBARRAY(self)
+ * 
+ */
+
+static CYTHON_INLINE PyArray_ArrayDescr *__pyx_f_5numpy_5dtype_8subarray_subarray(PyArray_Descr *__pyx_v_self) {
+  PyArray_ArrayDescr *__pyx_r;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":308
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:
+ *             return PyDataType_SUBARRAY(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyDataType_SUBARRAY(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":307
+ *         # this field via the inline helper method PyDataType_SHAPE.
+ *         @property
+ *         cdef inline PyArray_ArrayDescr* subarray(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             return PyDataType_SUBARRAY(self)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":311
+ * 
+ *         @property
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)
+ */
+
+static CYTHON_INLINE npy_uint64 __pyx_f_5numpy_5dtype_5flags_flags(PyArray_Descr *__pyx_v_self) {
+  npy_uint64 __pyx_r;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":313
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyDataType_FLAGS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":311
+ * 
+ *         @property
+ *         cdef inline npy_uint64 flags(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The data types flags."""
+ *             return PyDataType_FLAGS(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":323
+ * 
+ *         @property
+ *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_7numiter_numiter(PyArrayMultiIterObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":325
+ *         cdef inline int numiter(self) noexcept nogil:
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_NUMITER(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":323
+ * 
+ *         @property
+ *         cdef inline int numiter(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of arrays that need to be broadcast to the same shape."""
+ *             return PyArray_MultiIter_NUMITER(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":328
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_4size_size(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":330
+ *         cdef inline npy_intp size(self) noexcept nogil:
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_SIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":328
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The total broadcasted size."""
+ *             return PyArray_MultiIter_SIZE(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":333
+ * 
+ *         @property
+ *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_9broadcast_5index_index(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":335
+ *         cdef inline npy_intp index(self) noexcept nogil:
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_INDEX(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":333
+ * 
+ *         @property
+ *         cdef inline npy_intp index(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The current (1-d) index into the broadcasted result."""
+ *             return PyArray_MultiIter_INDEX(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":338
+ * 
+ *         @property
+ *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_9broadcast_2nd_nd(PyArrayMultiIterObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":340
+ *         cdef inline int nd(self) noexcept nogil:
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_NDIM(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":338
+ * 
+ *         @property
+ *         cdef inline int nd(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The number of dimensions in the broadcasted result."""
+ *             return PyArray_MultiIter_NDIM(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":343
+ * 
+ *         @property
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_9broadcast_10dimensions_dimensions(PyArrayMultiIterObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":345
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_MultiIter_DIMS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":343
+ * 
+ *         @property
+ *         cdef inline npy_intp* dimensions(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """The shape of the broadcasted result."""
+ *             return PyArray_MultiIter_DIMS(self)
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":348
+ * 
+ *         @property
+ *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ */
+
+static CYTHON_INLINE void **__pyx_f_5numpy_9broadcast_5iters_iters(PyArrayMultiIterObject *__pyx_v_self) {
+  void **__pyx_r;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":351
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ *             return PyArray_MultiIter_ITERS(self)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyArray_MultiIter_ITERS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":348
+ * 
+ *         @property
+ *         cdef inline void** iters(self) noexcept nogil:             # <<<<<<<<<<<<<<
+ *             """An array of iterator objects that holds the iterators for the arrays to be broadcast together.
+ *             On return, the iterators are adjusted for broadcasting."""
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":366
  * 
  *         @property
- *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":249
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":369
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":246
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":366
  * 
  *         @property
- *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline PyObject* base(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":255
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":375
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":252
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":372
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
- *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":261
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":381
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":258
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":378
  * 
  *         @property
- *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline int ndim(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
- *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":269
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":389
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":264
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":384
  * 
  *         @property
- *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *shape(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
- *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":276
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":396
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":272
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":392
  * 
  *         @property
- *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp *strides(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
- *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":282
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":402
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":279
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":399
  * 
  *         @property
- *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline npy_intp size(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
- *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":291
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":411
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
- *     ctypedef unsigned char      npy_bool
+ * 
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":285
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":405
  * 
  *         @property
- *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *         cdef inline char* data(self) noexcept nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
- * ctypedef npy_cdouble     complex_t
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":807
+ * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
@@ -18771,30 +19203,30 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":778
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":808
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 778, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 808, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
- * ctypedef npy_cdouble     complex_t
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":807
+ * ctypedef long double complex clongdouble_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
   /* function exit code */
@@ -18804,15 +19236,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18821,29 +19253,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":781
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":811
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 811, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":810
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18854,15 +19286,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18871,29 +19303,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":784
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":814
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 784, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 814, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":813
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18904,15 +19336,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18921,29 +19353,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":787
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":817
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 787, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 817, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":816
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18954,15 +19386,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18971,29 +19403,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":820
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 790, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 820, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":819
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19004,209 +19436,219 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
+  PyObject *__pyx_t_2;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":794
+    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":824
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
-    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
+    __pyx_t_2 = __pyx_f_5numpy_5dtype_8subarray_subarray(__pyx_v_d)->shape;
+    __Pyx_INCREF(((PyObject*)__pyx_t_2));
+    __pyx_r = ((PyObject*)__pyx_t_2);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":823
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":796
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":826
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":822
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  * 
- * cdef inline void set_array_base(ndarray arr, object base):
+ * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
- * cdef inline void set_array_base(ndarray arr, object base):
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1012
+ * cdef inline void set_array_base(ndarray arr, object base) except *:
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 1012, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     int _import_umath() except -1
  * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ * cdef inline void set_array_base(ndarray arr, object base) except *:             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1015
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":978
+    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1016
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1018
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19222,15 +19664,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19238,68 +19680,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1024
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")
+ *         raise ImportError("numpy._core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 985, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1024, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.multiarray failed to import")
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 986, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1025, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 987, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1026, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 987, __pyx_L5_except_error)
+      __PYX_ERR(2, 1026, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1023
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19307,15 +19749,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1022
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19330,16 +19772,16 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
- *         raise ImportError("numpy.core.multiarray failed to import")
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
@@ -19354,15 +19796,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19370,68 +19812,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1030
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 991, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1030, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1031
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 992, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1031, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 993, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1032, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 993, __pyx_L5_except_error)
+      __PYX_ERR(2, 1032, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19439,16 +19881,16 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
- *         raise ImportError("numpy.core.multiarray failed to import")
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+ *         raise ImportError("numpy._core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
   /* function exit code */
@@ -19462,16 +19904,16 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
- *         raise ImportError("numpy.core.umath failed to import")
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1034
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
@@ -19486,15 +19928,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19502,68 +19944,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":997
+      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 997, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 1036, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1037
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 998, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 1037, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+      /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 999, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 1038, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 999, __pyx_L5_except_error)
+      __PYX_ERR(2, 1038, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+    /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19571,16 +20013,16 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
- *         raise ImportError("numpy.core.umath failed to import")
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1034
+ *         raise ImportError("numpy._core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
   /* function exit code */
@@ -19594,173 +20036,175 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1002
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
- * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_timedelta64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1068
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1017
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1056
  * 
  * 
- * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ * cdef inline bint is_datetime64_object(object obj) noexcept:             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1078
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1071
  * 
  * 
- * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_datetime get_datetime64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1085
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1081
  * 
  * 
- * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+/* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1053
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1092
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ * 
+ * 
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1088
  * 
  * 
- * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) noexcept nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -23027,16 +23471,16 @@
     {&__pyx_n_s_nan, __pyx_k_nan, sizeof(__pyx_k_nan), 0, 0, 1, 1},
     {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
     {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
     {&__pyx_n_s_nstepsp, __pyx_k_nstepsp, sizeof(__pyx_k_nstepsp), 0, 0, 1, 1},
     {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-    {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
-    {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy__core_multiarray_failed_to, __pyx_k_numpy__core_multiarray_failed_to, sizeof(__pyx_k_numpy__core_multiarray_failed_to), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy__core_umath_failed_to_impo, __pyx_k_numpy__core_umath_failed_to_impo, sizeof(__pyx_k_numpy__core_umath_failed_to_impo), 0, 1, 0, 0},
     {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
     {&__pyx_n_s_ones, __pyx_k_ones, sizeof(__pyx_k_ones), 0, 0, 1, 1},
     {&__pyx_n_s_out, __pyx_k_out, sizeof(__pyx_k_out), 0, 0, 1, 1},
     {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
@@ -23094,15 +23538,15 @@
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 156, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 159, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(1, 373, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 618, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 914, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 987, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 1026, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -23141,33 +23585,33 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *         __pyx_import_array()
  *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 987, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy__core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 1026, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-qv7imtqn/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-1e9jof8w/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1032
  *         _import_umath()
  *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy._core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 993, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy__core_umath_failed_to_impo); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 1032, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
   /* "dtw/_dtw_utils.pyx":102
  *     tnstepsp = np.array([6], dtype=DTYPE)
  * 
  *     tdir = np.array( (1, 1, 2, 2, 3, 3, 0, 0, 1, 0, 1, 0, 1, 0, 1, 0, 0, 0,-1, 1,-1, 1,-1, 1),             # <<<<<<<<<<<<<<
@@ -23594,31 +24038,31 @@
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 203, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 203, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 230, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 239, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 829, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 831, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 869, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 271, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 316, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 320, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 359, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 848, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 850, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 852, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 854, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 856, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 858, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 860, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 862, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 864, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 930, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_3_0_10(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(arrayobject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(4, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
@@ -30620,14 +31064,168 @@
             z.real = z_r * cos(z_theta);
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
+/* Declarations */
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+  #ifdef __cplusplus
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      return ::std::complex< long double >(x, y);
+    }
+  #else
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      return x + y*(__pyx_t_long_double_complex)_Complex_I;
+    }
+  #endif
+#else
+    static CYTHON_INLINE __pyx_t_long_double_complex __pyx_t_long_double_complex_from_parts(long double x, long double y) {
+      __pyx_t_long_double_complex z;
+      z.real = x;
+      z.imag = y;
+      return z;
+    }
+#endif
+
+/* Arithmetic */
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
+#else
+    static CYTHON_INLINE int __Pyx_c_eq_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+       return (a.real == b.real) && (a.imag == b.imag);
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_sum_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real + b.real;
+        z.imag = a.imag + b.imag;
+        return z;
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_diff_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real - b.real;
+        z.imag = a.imag - b.imag;
+        return z;
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_prod_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        __pyx_t_long_double_complex z;
+        z.real = a.real * b.real - a.imag * b.imag;
+        z.imag = a.real * b.imag + a.imag * b.real;
+        return z;
+    }
+    #if 1
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        if (b.imag == 0) {
+            return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.real);
+        } else if (fabsl(b.real) >= fabsl(b.imag)) {
+            if (b.real == 0 && b.imag == 0) {
+                return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.imag);
+            } else {
+                long double r = b.imag / b.real;
+                long double s = (long double)(1.0) / (b.real + b.imag * r);
+                return __pyx_t_long_double_complex_from_parts(
+                    (a.real + a.imag * r) * s, (a.imag - a.real * r) * s);
+            }
+        } else {
+            long double r = b.real / b.imag;
+            long double s = (long double)(1.0) / (b.imag + b.real * r);
+            return __pyx_t_long_double_complex_from_parts(
+                (a.real * r + a.imag) * s, (a.imag * r - a.real) * s);
+        }
+    }
+    #else
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_quot_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+        if (b.imag == 0) {
+            return __pyx_t_long_double_complex_from_parts(a.real / b.real, a.imag / b.real);
+        } else {
+            long double denom = b.real * b.real + b.imag * b.imag;
+            return __pyx_t_long_double_complex_from_parts(
+                (a.real * b.real + a.imag * b.imag) / denom,
+                (a.imag * b.real - a.real * b.imag) / denom);
+        }
+    }
+    #endif
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_neg_long__double(__pyx_t_long_double_complex a) {
+        __pyx_t_long_double_complex z;
+        z.real = -a.real;
+        z.imag = -a.imag;
+        return z;
+    }
+    static CYTHON_INLINE int __Pyx_c_is_zero_long__double(__pyx_t_long_double_complex a) {
+       return (a.real == 0) && (a.imag == 0);
+    }
+    static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_conj_long__double(__pyx_t_long_double_complex a) {
+        __pyx_t_long_double_complex z;
+        z.real =  a.real;
+        z.imag = -a.imag;
+        return z;
+    }
+    #if 1
+        static CYTHON_INLINE long double __Pyx_c_abs_long__double(__pyx_t_long_double_complex z) {
+          #if !defined(HAVE_HYPOT) || defined(_MSC_VER)
+            return sqrtl(z.real*z.real + z.imag*z.imag);
+          #else
+            return hypotl(z.real, z.imag);
+          #endif
+        }
+        static CYTHON_INLINE __pyx_t_long_double_complex __Pyx_c_pow_long__double(__pyx_t_long_double_complex a, __pyx_t_long_double_complex b) {
+            __pyx_t_long_double_complex z;
+            long double r, lnr, theta, z_r, z_theta;
+            if (b.imag == 0 && b.real == (int)b.real) {
+                if (b.real < 0) {
+                    long double denom = a.real * a.real + a.imag * a.imag;
+                    a.real = a.real / denom;
+                    a.imag = -a.imag / denom;
+                    b.real = -b.real;
+                }
+                switch ((int)b.real) {
+                    case 0:
+                        z.real = 1;
+                        z.imag = 0;
+                        return z;
+                    case 1:
+                        return a;
+                    case 2:
+                        return __Pyx_c_prod_long__double(a, a);
+                    case 3:
+                        z = __Pyx_c_prod_long__double(a, a);
+                        return __Pyx_c_prod_long__double(z, a);
+                    case 4:
+                        z = __Pyx_c_prod_long__double(a, a);
+                        return __Pyx_c_prod_long__double(z, z);
+                }
+            }
+            if (a.imag == 0) {
+                if (a.real == 0) {
+                    return a;
+                } else if ((b.imag == 0) && (a.real >= 0)) {
+                    z.real = powl(a.real, b.real);
+                    z.imag = 0;
+                    return z;
+                } else if (a.real > 0) {
+                    r = a.real;
+                    theta = 0;
+                } else {
+                    r = -a.real;
+                    theta = atan2l(0.0, -1.0);
+                }
+            } else {
+                r = __Pyx_c_abs_long__double(a);
+                theta = atan2l(a.imag, a.real);
+            }
+            lnr = logl(r);
+            z_r = expl(lnr * b.real - theta * b.imag);
+            z_theta = theta * b.real + lnr * b.imag;
+            z.real = z_r * cosl(z_theta);
+            z.imag = z_r * sinl(z_theta);
+            return z;
+        }
+    #endif
+#endif
+
 /* MemviewSliceCopyTemplate */
   static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object)
 {
```

### Comparing `dtw_python-1.4.4/dtw/_dtw_utils.pyx` & `dtw_python-1.5.0/dtw/_dtw_utils.pyx`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/_globalCostMatrix.py` & `dtw_python-1.5.0/dtw/_globalCostMatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     # All input arguments
     out = _computeCM_wrapper(wm,
                              lm,
                              nsteps,
                              dir,
                              cm)
 
-    out['stepPattern'] = step_pattern;
+    out['stepPattern'] = step_pattern
     return out
 
 
 def _test_computeCM2(TS=5):
     import numpy as np
     ITYPE = np.int32
```

### Comparing `dtw_python-1.4.4/dtw/countPaths.py` & `dtw_python-1.5.0/dtw/countPaths.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/data/aami3a.csv` & `dtw_python-1.5.0/dtw/data/aami3a.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/data/aami3b.csv` & `dtw_python-1.5.0/dtw/data/aami3b.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/dtw.py` & `dtw_python-1.5.0/dtw/dtw.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/dtwPlot.py` & `dtw_python-1.5.0/dtw/dtwPlot.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/dtw_core.c` & `dtw_python-1.5.0/dtw/dtw_core.c`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/dtw_core.h` & `dtw_python-1.5.0/dtw/dtw_core.h`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/dtw_test_data.py` & `dtw_python-1.5.0/dtw/dtw_test_data.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/mvm.py` & `dtw_python-1.5.0/dtw/mvm.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/stepPattern.py` & `dtw_python-1.5.0/dtw/stepPattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -562,50 +562,50 @@
 symmetric1 = StepPattern(_c(
     1, 1, 1, -1,
     1, 0, 0, 1,
     2, 0, 1, -1,
     2, 0, 0, 1,
     3, 1, 0, -1,
     3, 0, 0, 1
-));
+))
 
 ## Normal symmetric
 ## normalization: N+M
 symmetric2 = StepPattern(_c(
     1, 1, 1, -1,
     1, 0, 0, 2,
     2, 0, 1, -1,
     2, 0, 0, 1,
     3, 1, 0, -1,
     3, 0, 0, 1
-), "N+M");
+), "N+M")
 
 ## classic asymmetric pattern: max slope 2, min slope 0
 ## normalization: N
 asymmetric = StepPattern(_c(
     1, 1, 0, -1,
     1, 0, 0, 1,
     2, 1, 1, -1,
     2, 0, 0, 1,
     3, 1, 2, -1,
     3, 0, 0, 1
-), "N");
+), "N")
 
 # % \item{\code{symmetricVelichkoZagoruyko}}{symmetric, reproduced from %
 # [Sakoe1978]. Use distance matrix \code{1-d}}
 # 
 
 ## normalization: max[N,M]
 ## note: local distance matrix is 1-d
 ## \cite{Velichko}
 _symmetricVelichkoZagoruyko = StepPattern(_c(
     1, 0, 1, -1,
     2, 1, 1, -1,
     2, 0, 0, -1.001,
-    3, 1, 0, -1));
+    3, 1, 0, -1))
 
 # % \item{\code{asymmetricItakura}}{asymmetric, slope contrained 0.5 -- 2
 # from reference [Itakura1975]. This is the recursive definition % that
 # generates the Itakura parallelogram; }
 # 
 
 ## Itakura slope-limited asymmetric \cite{Itakura1975}
@@ -618,48 +618,48 @@
     2, 0, 0, 1,
     3, 2, 1, -1,
     3, 1, 0, 1,
     3, 0, 0, 1,
     4, 2, 2, -1,
     4, 1, 0, 1,
     4, 0, 0, 1
-));
+))
 
 #############################
 ## Slope-limited versions
 ##
 ## Taken from Table I, page 47 of "Dynamic programming algorithm
 ## optimization for spoken word recognition," Acoustics, Speech, and
 ## Signal Processing, vol.26, no.1, pp. 43-49, Feb 1978 URL:
 ## http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=1163055
 ##
 ## Mostly unchecked
 
 
 ## Row P=0
-symmetricP0 = symmetric2;
+symmetricP0 = symmetric2
 
 ## normalization: N ?
 asymmetricP0 = StepPattern(_c(
     1, 0, 1, -1,
     1, 0, 0, 0,
     2, 1, 1, -1,
     2, 0, 0, 1,
     3, 1, 0, -1,
     3, 0, 0, 1
-), "N");
+), "N")
 
 ## alternative implementation
 _asymmetricP0b = StepPattern(_c(
     1, 0, 1, -1,
     2, 1, 1, -1,
     2, 0, 0, 1,
     3, 1, 0, -1,
     3, 0, 0, 1
-), "N");
+), "N")
 
 ## Row P=1/2
 symmetricP05 = StepPattern(_c(
     1, 1, 3, -1,
     1, 0, 2, 2,
     1, 0, 1, 1,
     1, 0, 0, 1,
@@ -671,15 +671,15 @@
     4, 2, 1, -1,
     4, 1, 0, 2,
     4, 0, 0, 1,
     5, 3, 1, -1,
     5, 2, 0, 2,
     5, 1, 0, 1,
     5, 0, 0, 1
-), "N+M");
+), "N+M")
 
 asymmetricP05 = StepPattern(_c(
     1, 1, 3, -1,
     1, 0, 2, 1 / 3,
     1, 0, 1, 1 / 3,
     1, 0, 0, 1 / 3,
     2, 1, 2, -1,
@@ -690,67 +690,67 @@
     4, 2, 1, -1,
     4, 1, 0, 1,
     4, 0, 0, 1,
     5, 3, 1, -1,
     5, 2, 0, 1,
     5, 1, 0, 1,
     5, 0, 0, 1
-), "N");
+), "N")
 
 ## Row P=1
 ## Implementation of Sakoe's P=1, Symmetric algorithm
 
 symmetricP1 = StepPattern(_c(
     1, 1, 2, -1,  # First branch: g(i-1,j-2)+
     1, 0, 1, 2,  # + 2d(i  ,j-1)
     1, 0, 0, 1,  # +  d(i  ,j)
     2, 1, 1, -1,  # Second branch: g(i-1,j-1)+
     2, 0, 0, 2,  # +2d(i,  j)
     3, 2, 1, -1,  # Third branch: g(i-2,j-1)+
     3, 1, 0, 2,  # + 2d(i-1,j)
     3, 0, 0, 1  # +  d(  i,j)
-), "N+M");
+), "N+M")
 
 asymmetricP1 = StepPattern(_c(
     1, 1, 2, -1,
     1, 0, 1, .5,
     1, 0, 0, .5,
     2, 1, 1, -1,
     2, 0, 0, 1,
     3, 2, 1, -1,
     3, 1, 0, 1,
     3, 0, 0, 1
-), "N");
+), "N")
 
 ## Row P=2
 symmetricP2 = StepPattern(_c(
     1, 2, 3, -1,
     1, 1, 2, 2,
     1, 0, 1, 2,
     1, 0, 0, 1,
     2, 1, 1, -1,
     2, 0, 0, 2,
     3, 3, 2, -1,
     3, 2, 1, 2,
     3, 1, 0, 2,
     3, 0, 0, 1
-), "N+M");
+), "N+M")
 
 asymmetricP2 = StepPattern(_c(
     1, 2, 3, -1,
     1, 1, 2, 2 / 3,
     1, 0, 1, 2 / 3,
     1, 0, 0, 2 / 3,
     2, 1, 1, -1,
     2, 0, 0, 1,
     3, 3, 2, -1,
     3, 2, 1, 1,
     3, 1, 0, 1,
     3, 0, 0, 1
-), "N");
+), "N")
 
 ################################
 ## Taken from Table III, page 49.
 ## Four varieties of DP-algorithm compared
 
 ## 1st row:  asymmetric
 
@@ -787,133 +787,133 @@
     1, 1, 0, 1,
     1, 0, 0, 0,
     2, 1, 1, -1,
     2, 0, 0, 1,
     3, 1, 2, -1,
     3, 0, 1, 1,
     3, 0, 0, 0
-));
+))
 
 typeIb = StepPattern(_c(
     1, 2, 1, -1,
     1, 1, 0, 1,
     1, 0, 0, 1,
     2, 1, 1, -1,
     2, 0, 0, 1,
     3, 1, 2, -1,
     3, 0, 1, 1,
     3, 0, 0, 1
-));
+))
 
 typeIc = StepPattern(_c(
     1, 2, 1, -1,
     1, 1, 0, 1,
     1, 0, 0, 1,
     2, 1, 1, -1,
     2, 0, 0, 1,
     3, 1, 2, -1,
     3, 0, 1, 1,
     3, 0, 0, 0
-), "N");
+), "N")
 
 typeId = StepPattern(_c(
     1, 2, 1, -1,
     1, 1, 0, 2,
     1, 0, 0, 1,
     2, 1, 1, -1,
     2, 0, 0, 2,
     3, 1, 2, -1,
     3, 0, 1, 2,
     3, 0, 0, 1
-), "N+M");
+), "N+M")
 
 ## ----------
 ## smoothed variants of above
 
 typeIas = StepPattern(_c(
     1, 2, 1, -1,
     1, 1, 0, .5,
     1, 0, 0, .5,
     2, 1, 1, -1,
     2, 0, 0, 1,
     3, 1, 2, -1,
     3, 0, 1, .5,
     3, 0, 0, .5
-));
+))
 
 typeIbs = StepPattern(_c(
     1, 2, 1, -1,
     1, 1, 0, 1,
     1, 0, 0, 1,
     2, 1, 1, -1,
     2, 0, 0, 1,
     3, 1, 2, -1,
     3, 0, 1, 1,
     3, 0, 0, 1
-));
+))
 
 typeIcs = StepPattern(_c(
     1, 2, 1, -1,
     1, 1, 0, 1,
     1, 0, 0, 1,
     2, 1, 1, -1,
     2, 0, 0, 1,
     3, 1, 2, -1,
     3, 0, 1, .5,
     3, 0, 0, .5
-), "N");
+), "N")
 
 typeIds = StepPattern(_c(
     1, 2, 1, -1,
     1, 1, 0, 1.5,
     1, 0, 0, 1.5,
     2, 1, 1, -1,
     2, 0, 0, 2,
     3, 1, 2, -1,
     3, 0, 1, 1.5,
     3, 0, 0, 1.5
-), "N+M");
+), "N+M")
 
 ## ----------
 
 typeIIa = StepPattern(_c(
     1, 1, 1, -1,
     1, 0, 0, 1,
     2, 1, 2, -1,
     2, 0, 0, 1,
     3, 2, 1, -1,
     3, 0, 0, 1
-));
+))
 
 typeIIb = StepPattern(_c(
     1, 1, 1, -1,
     1, 0, 0, 1,
     2, 1, 2, -1,
     2, 0, 0, 2,
     3, 2, 1, -1,
     3, 0, 0, 2
-));
+))
 
 typeIIc = StepPattern(_c(
     1, 1, 1, -1,
     1, 0, 0, 1,
     2, 1, 2, -1,
     2, 0, 0, 1,
     3, 2, 1, -1,
     3, 0, 0, 2
-), "N");
+), "N")
 
 typeIId = StepPattern(_c(
     1, 1, 1, -1,
     1, 0, 0, 2,
     2, 1, 2, -1,
     2, 0, 0, 3,
     3, 2, 1, -1,
     3, 0, 0, 3
-), "N+M");
+), "N+M")
 
 ## ----------
 
 ## Rabiner [3] discusses why this is not equivalent to Itakura's
 
 typeIIIc = StepPattern(_c(
     1, 1, 2, -1,
@@ -922,15 +922,15 @@
     2, 0, 0, 1,
     3, 2, 1, -1,
     3, 1, 0, 1,
     3, 0, 0, 1,
     4, 2, 2, -1,
     4, 1, 0, 1,
     4, 0, 0, 1
-), "N");
+), "N")
 
 ## ----------
 
 ## numbers follow as production rules in fig 2.16
 
 typeIVc = StepPattern(_c(
     1, 1, 1, -1,
@@ -956,15 +956,15 @@
     8, 2, 0, 1,
     8, 1, 0, 1,
     8, 0, 0, 1,
     9, 3, 3, -1,
     9, 2, 0, 1,
     9, 1, 0, 1,
     9, 0, 0, 1
-), "N");
+), "N")
 
 #############################
 ## 
 ## Mori's asymmetric step-constrained pattern. Normalized in the
 ## reference length.
 ##
 ## Mori, A.; Uchida, S.; Kurazume, R.; Taniguchi, R.; Hasegawa, T. &
@@ -978,13 +978,13 @@
     1, 1, 0, 2,
     1, 0, 0, 1,
     2, 1, 1, -1,
     2, 0, 0, 3,
     3, 1, 2, -1,
     3, 0, 1, 3,
     3, 0, 0, 3
-), "M");
+), "M")
 
 ## Completely unflexible: fixed slope 1. Only makes sense with
 ## open.begin and open.end
 rigid = StepPattern(_c(1, 1, 1, -1,
                        1, 0, 0, 1), "N")
```

### Comparing `dtw_python-1.4.4/dtw/warp.py` & `dtw_python-1.5.0/dtw/warp.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/warpArea.py` & `dtw_python-1.5.0/dtw/warpArea.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/dtw/window.py` & `dtw_python-1.5.0/dtw/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,8 +157,8 @@
          (iw >= n - 1 - 2 * (m - jw)) & \
          (jw > m - 1 - 2 * (n - iw))
     return ok
 
 
 def slantedBandWindow(iw, jw, query_size, reference_size, window_size):
     diagj = (iw * reference_size / query_size)
-    return abs(jw - diagj) <= window_size;
+    return abs(jw - diagj) <= window_size
```

### Comparing `dtw_python-1.4.4/dtw_python.egg-info/SOURCES.txt` & `dtw_python-1.5.0/dtw_python.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 CONTRIBUTING.rst
 COPYING
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
-docs/Makefile
 docs/conf.py
-docs/index.rst
-docs/make.bat
 dtw/__init__.py
 dtw/__main__.py
 dtw/_backtrack.py
 dtw/_dtw_utils.c
 dtw/_dtw_utils.pyx
 dtw/_globalCostMatrix.py
 dtw/countPaths.py
@@ -24,25 +21,24 @@
 dtw/dtw_core.h
 dtw/dtw_test_data.py
 dtw/mvm.py
 dtw/stepPattern.py
 dtw/warp.py
 dtw/warpArea.py
 dtw/window.py
-dtw/data/README.txt
 dtw/data/aami3a.csv
 dtw/data/aami3b.csv
 dtw_python.egg-info/PKG-INFO
 dtw_python.egg-info/SOURCES.txt
 dtw_python.egg-info/dependency_links.txt
 dtw_python.egg-info/entry_points.txt
 dtw_python.egg-info/not-zip-safe
 dtw_python.egg-info/requires.txt
 dtw_python.egg-info/top_level.txt
-tests/__init__.py
+maintainer/roxypick.py
 tests/query.csv
 tests/reference.csv
 tests/test_cli.py
 tests/test_countPaths.py
 tests/test_cran.py
 tests/test_doctests.py
 tests/test_dtw.py
```

### Comparing `dtw_python-1.4.4/tests/query.csv` & `dtw_python-1.5.0/tests/query.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/tests/reference.csv` & `dtw_python-1.5.0/tests/reference.csv`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/tests/test_cli.py` & `dtw_python-1.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/tests/test_countPaths.py` & `dtw_python-1.5.0/tests/test_countPaths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 import unittest
 
 import numpy as np
-from numpy import nan
 from numpy.testing import *
 
 from dtw import *
 from dtw.countPaths import *
 
 
 class Test_countPaths(unittest.TestCase):
```

### Comparing `dtw_python-1.4.4/tests/test_cran.py` & `dtw_python-1.5.0/tests/test_cran.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import unittest
 
 import numpy as np
-from numpy import nan
 from numpy.testing import (assert_approx_equal, assert_equal,
-                           assert_array_equal, assert_raises)
+                           assert_array_equal)
 from dtw import *
 
 
 def i(l):
     return np.array([int(x) for x in l.split()], dtype=int)-1
```

### Comparing `dtw_python-1.4.4/tests/test_dtw.py` & `dtw_python-1.5.0/tests/test_dtw.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 
 import unittest
 
 import numpy as np
-from numpy import nan
-from numpy.testing import (assert_approx_equal,
-                           assert_array_equal, assert_raises)
 
 from dtw import *
 
 
 """
 # As in the JSS paper
```

### Comparing `dtw_python-1.4.4/tests/test_dtw_s.py` & `dtw_python-1.5.0/tests/test_dtw_s.py`

 * *Files identical despite different names*

### Comparing `dtw_python-1.4.4/tests/test_issues.py` & `dtw_python-1.5.0/tests/test_issues.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import unittest
 
 import numpy as np
-from numpy import nan
 from numpy.testing import (assert_approx_equal, assert_equal,
-                           assert_array_equal, assert_raises)
+                           assert_array_equal)
 from dtw import *
 
 
 def i(l):
     return np.array([int(x) for x in l.split()], dtype=int)-1
```

