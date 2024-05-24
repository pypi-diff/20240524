# Comparing `tmp/volue-insight-timeseries-1.1.0.tar.gz` & `tmp/volue-insight-timeseries-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volue-insight-timeseries-1.1.0.tar", last modified: Wed May 15 09:02:32 2024, max compression
+gzip compressed data, was "volue-insight-timeseries-1.2.0.tar", last modified: Fri May 24 12:41:51 2024, max compression
```

## Comparing `volue-insight-timeseries-1.1.0.tar` & `volue-insight-timeseries-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:02:32.889647 volue-insight-timeseries-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 09:02:26.000000 volue-insight-timeseries-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 09:02:26.000000 volue-insight-timeseries-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-15 09:02:32.889647 volue-insight-timeseries-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-15 09:02:26.000000 volue-insight-timeseries-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-15 09:02:32.893647 volue-insight-timeseries-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-15 09:02:26.000000 volue-insight-timeseries-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:02:32.889647 volue-insight-timeseries-1.1.0/volue_insight_timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 09:02:26.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-15 09:02:26.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-15 09:02:26.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    65949 2024-05-15 09:02:26.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries/curves.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-15 09:02:26.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    20124 2024-05-15 09:02:26.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-15 09:02:26.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 09:02:32.889647 volue-insight-timeseries-1.1.0/volue_insight_timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-15 09:02:32.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-15 09:02:32.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 09:02:32.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 09:02:32.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 09:02:32.000000 volue-insight-timeseries-1.1.0/volue_insight_timeseries.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:41:51.979786 volue-insight-timeseries-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-24 12:41:45.000000 volue-insight-timeseries-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 12:41:45.000000 volue-insight-timeseries-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-24 12:41:51.979786 volue-insight-timeseries-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-24 12:41:45.000000 volue-insight-timeseries-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-24 12:41:51.979786 volue-insight-timeseries-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-24 12:41:45.000000 volue-insight-timeseries-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:41:51.975786 volue-insight-timeseries-1.2.0/volue_insight_timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 12:41:45.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-24 12:41:45.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-24 12:41:45.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65949 2024-05-24 12:41:45.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries/curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-24 12:41:45.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20124 2024-05-24 12:41:45.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-24 12:41:45.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:41:51.979786 volue-insight-timeseries-1.2.0/volue_insight_timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-24 12:41:51.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-24 12:41:51.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:41:51.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 12:41:51.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 12:41:51.000000 volue-insight-timeseries-1.2.0/volue_insight_timeseries.egg-info/top_level.txt
```

### Comparing `volue-insight-timeseries-1.1.0/LICENSE` & `volue-insight-timeseries-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.1.0/PKG-INFO` & `volue-insight-timeseries-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: volue-insight-timeseries
-Version: 1.1.0
+Version: 1.2.0
 Summary: Volue Insight API python library
 Home-page: https://www.volueinsight.com
 Author: Volue Insight
 Author-email: support.insight@volue.com
-Requires-Python: >=3.9, <3.12a0
+Requires-Python: >=3.9, <3.13a0
 License-File: LICENSE
 
 This library is meant as a simple toolkit for working with data from https://api.volueinsight.com/ (or equivalent services).  Note that access is based on some sort of login credentials, this library is not all that useful unless you have a valid Volue Insight account.
```

### Comparing `volue-insight-timeseries-1.1.0/README.md` & `volue-insight-timeseries-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Volue Insight API python library for working with timeseries.
 
 This library is meant as a simple toolkit for working with data from
 https://api.volueinsight.com/ (or equivalent services). Note that access
 is based on having a valid Volue Insight account. Please contact
 sales.insight@volue.com in order to get a trial account.
 
-The library is tested against Python 3.9, 3.10 and 3.11 - we recommend using 
+The library is tested against Python 3.9, 3.10, 3.11 and 3.12 - we recommend using 
 the latest Python version.
 
 
 ## Documentation
 
 The 
 [documentation](https://wattsight-volue-insight-timeseries.readthedocs-hosted.com/en/master/) 
@@ -50,15 +50,15 @@
 If you previously have used wapi-python, you should switch to use this package
 going forward. We will not add any new features to wapi-python, it is only in 
 the event of a severe bug that we will do any changes to it.
 
 These are the steps you will have to do in order to successfully
 make the switch. 
 
-* Use Python 3.9, 3.10 or 3.11
+* Use Python 3.9, 3.10, 3.11 or 3.12
 * Use Pandas 1.5.0 or newer
 * Use [zoneinfo](https://docs.python.org/3/library/zoneinfo.html), not pytz for handling time zone information
 
 
 ## Copyright (MIT License)
 
 Copyright (c) 2018-2022 Volue Insight AS
```

### Comparing `volue-insight-timeseries-1.1.0/setup.py` & `volue-insight-timeseries-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 # Get current version from the VERSION file
 with open(os.path.join(here, 'volue_insight_timeseries/VERSION')) as fv:
     version = fv.read().strip()
 
 setup(
     name='volue-insight-timeseries',
-    python_requires='>=3.9, <3.12a0',
+    python_requires='>=3.9, <3.13a0',
     packages=find_packages(),
     install_requires=extract_requirements('requirements.txt'),
     tests_require=[
         'pytest',
         'pytest-cov >= 2.5',
         'requests-mock >= 1.3',
     ],
```

### Comparing `volue-insight-timeseries-1.1.0/volue_insight_timeseries/auth.py` & `volue-insight-timeseries-1.2.0/volue_insight_timeseries/auth.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.1.0/volue_insight_timeseries/curves.py` & `volue-insight-timeseries-1.2.0/volue_insight_timeseries/curves.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.1.0/volue_insight_timeseries/events.py` & `volue-insight-timeseries-1.2.0/volue_insight_timeseries/events.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.1.0/volue_insight_timeseries/session.py` & `volue-insight-timeseries-1.2.0/volue_insight_timeseries/session.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.1.0/volue_insight_timeseries/util.py` & `volue-insight-timeseries-1.2.0/volue_insight_timeseries/util.py`

 * *Files identical despite different names*

### Comparing `volue-insight-timeseries-1.1.0/volue_insight_timeseries.egg-info/PKG-INFO` & `volue-insight-timeseries-1.2.0/volue_insight_timeseries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: volue-insight-timeseries
-Version: 1.1.0
+Version: 1.2.0
 Summary: Volue Insight API python library
 Home-page: https://www.volueinsight.com
 Author: Volue Insight
 Author-email: support.insight@volue.com
-Requires-Python: >=3.9, <3.12a0
+Requires-Python: >=3.9, <3.13a0
 License-File: LICENSE
 
 This library is meant as a simple toolkit for working with data from https://api.volueinsight.com/ (or equivalent services).  Note that access is based on some sort of login credentials, this library is not all that useful unless you have a valid Volue Insight account.
```

### Comparing `volue-insight-timeseries-1.1.0/volue_insight_timeseries.egg-info/SOURCES.txt` & `volue-insight-timeseries-1.2.0/volue_insight_timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

