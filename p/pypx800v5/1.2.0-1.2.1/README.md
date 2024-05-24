# Comparing `tmp/pypx800v5-1.2.0.tar.gz` & `tmp/pypx800v5-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypx800v5-1.2.0.tar", last modified: Tue Mar 19 17:00:58 2024, max compression
+gzip compressed data, was "pypx800v5-1.2.1.tar", last modified: Fri May 24 12:31:26 2024, max compression
```

## Comparing `pypx800v5-1.2.0.tar` & `pypx800v5-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 matthieu  (1000) matthieu  (1000)        0 2024-03-19 17:00:58.895622 pypx800v5-1.2.0/
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1065 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/LICENSE
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     3093 2024-03-19 17:00:58.895622 pypx800v5-1.2.0/PKG-INFO
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     2665 2023-09-30 18:40:31.000000 pypx800v5-1.2.0/README.md
-drwxr-xr-x   0 matthieu  (1000) matthieu  (1000)        0 2024-03-19 17:00:58.895622 pypx800v5-1.2.0/pypx800v5/
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1971 2023-09-29 20:15:49.000000 pypx800v5-1.2.0/pypx800v5/__init__.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)      794 2023-09-28 20:33:02.000000 pypx800v5-1.2.0/pypx800v5/const.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1101 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/counter.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)      334 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/exceptions.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)      715 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/extension.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)    12648 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/ipx800.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     3595 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/ipx800_io.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)      618 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/object.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1461 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/tempo.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     4263 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/thermostat.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1648 2023-11-06 11:14:44.000000 pypx800v5-1.2.0/pypx800v5/x010v.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)      585 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/x24d.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1703 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/x4fp.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     2291 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/x4vr.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)      582 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/x8d.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1127 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/x8r.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1842 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/xdimmer.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     4213 2024-03-19 17:00:36.000000 pypx800v5-1.2.0/pypx800v5/xdisplay.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1834 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/xpwm.py
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1276 2023-09-28 20:12:28.000000 pypx800v5-1.2.0/pypx800v5/xthl.py
-drwxr-xr-x   0 matthieu  (1000) matthieu  (1000)        0 2024-03-19 17:00:58.895622 pypx800v5-1.2.0/pypx800v5.egg-info/
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)     3093 2024-03-19 17:00:58.000000 pypx800v5-1.2.0/pypx800v5.egg-info/PKG-INFO
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)      559 2024-03-19 17:00:58.000000 pypx800v5-1.2.0/pypx800v5.egg-info/SOURCES.txt
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)        1 2024-03-19 17:00:58.000000 pypx800v5-1.2.0/pypx800v5.egg-info/dependency_links.txt
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)       10 2024-03-19 17:00:58.000000 pypx800v5-1.2.0/pypx800v5.egg-info/top_level.txt
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)       38 2024-03-19 17:00:58.895622 pypx800v5-1.2.0/setup.cfg
--rw-r--r--   0 matthieu  (1000) matthieu  (1000)      644 2024-03-19 16:55:21.000000 pypx800v5-1.2.0/setup.py
+drwxr-xr-x   0 matthieu  (1000) matthieu  (1000)        0 2024-05-24 12:31:26.549474 pypx800v5-1.2.1/
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1065 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/LICENSE
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     3093 2024-05-24 12:31:26.549474 pypx800v5-1.2.1/PKG-INFO
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     2665 2023-09-30 18:40:31.000000 pypx800v5-1.2.1/README.md
+drwxr-xr-x   0 matthieu  (1000) matthieu  (1000)        0 2024-05-24 12:31:26.546141 pypx800v5-1.2.1/pypx800v5/
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1971 2023-09-29 20:15:49.000000 pypx800v5-1.2.1/pypx800v5/__init__.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)      794 2023-09-28 20:33:02.000000 pypx800v5-1.2.1/pypx800v5/const.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1101 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/counter.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)      334 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/exceptions.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)      715 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/extension.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)    12648 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/ipx800.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     3595 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/ipx800_io.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)      618 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/object.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1461 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/tempo.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     4263 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/thermostat.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1648 2023-11-06 11:14:44.000000 pypx800v5-1.2.1/pypx800v5/x010v.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)      585 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/x24d.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1703 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/x4fp.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     2291 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/x4vr.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)      582 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/x8d.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1127 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/x8r.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1842 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/xdimmer.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     4213 2024-03-19 17:00:36.000000 pypx800v5-1.2.1/pypx800v5/xdisplay.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1834 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/xpwm.py
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     1276 2023-09-28 20:12:28.000000 pypx800v5-1.2.1/pypx800v5/xthl.py
+drwxr-xr-x   0 matthieu  (1000) matthieu  (1000)        0 2024-05-24 12:31:26.546141 pypx800v5-1.2.1/pypx800v5.egg-info/
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)     3093 2024-05-24 12:31:26.000000 pypx800v5-1.2.1/pypx800v5.egg-info/PKG-INFO
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)      559 2024-05-24 12:31:26.000000 pypx800v5-1.2.1/pypx800v5.egg-info/SOURCES.txt
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)        1 2024-05-24 12:31:26.000000 pypx800v5-1.2.1/pypx800v5.egg-info/dependency_links.txt
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)       10 2024-05-24 12:31:26.000000 pypx800v5-1.2.1/pypx800v5.egg-info/top_level.txt
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)       38 2024-05-24 12:31:26.549474 pypx800v5-1.2.1/setup.cfg
+-rw-r--r--   0 matthieu  (1000) matthieu  (1000)      644 2024-05-24 12:29:02.000000 pypx800v5-1.2.1/setup.py
```

### Comparing `pypx800v5-1.2.0/LICENSE` & `pypx800v5-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/PKG-INFO` & `pypx800v5-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypx800v5
-Version: 1.2.0
+Version: 1.2.1
 Summary: Control the IPX800V5 and its extensions.
 Home-page: https://github.com/aohzan/pypx800v5
 Author: Aohzan
 Author-email: aohzan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypx800v5-1.2.0/README.md` & `pypx800v5-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/__init__.py` & `pypx800v5-1.2.1/pypx800v5/__init__.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/const.py` & `pypx800v5-1.2.1/pypx800v5/const.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/counter.py` & `pypx800v5-1.2.1/pypx800v5/counter.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/extension.py` & `pypx800v5-1.2.1/pypx800v5/extension.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/ipx800.py` & `pypx800v5-1.2.1/pypx800v5/ipx800.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/ipx800_io.py` & `pypx800v5-1.2.1/pypx800v5/ipx800_io.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/object.py` & `pypx800v5-1.2.1/pypx800v5/object.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/tempo.py` & `pypx800v5-1.2.1/pypx800v5/tempo.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/thermostat.py` & `pypx800v5-1.2.1/pypx800v5/thermostat.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/x010v.py` & `pypx800v5-1.2.1/pypx800v5/x010v.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/x24d.py` & `pypx800v5-1.2.1/pypx800v5/x24d.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/x4fp.py` & `pypx800v5-1.2.1/pypx800v5/x4fp.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/x4vr.py` & `pypx800v5-1.2.1/pypx800v5/x4vr.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/x8d.py` & `pypx800v5-1.2.1/pypx800v5/x8d.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/x8r.py` & `pypx800v5-1.2.1/pypx800v5/x8r.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/xdimmer.py` & `pypx800v5-1.2.1/pypx800v5/xdimmer.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/xdisplay.py` & `pypx800v5-1.2.1/pypx800v5/xdisplay.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/xpwm.py` & `pypx800v5-1.2.1/pypx800v5/xpwm.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5/xthl.py` & `pypx800v5-1.2.1/pypx800v5/xthl.py`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/pypx800v5.egg-info/PKG-INFO` & `pypx800v5-1.2.1/pypx800v5.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypx800v5
-Version: 1.2.0
+Version: 1.2.1
 Summary: Control the IPX800V5 and its extensions.
 Home-page: https://github.com/aohzan/pypx800v5
 Author: Aohzan
 Author-email: aohzan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pypx800v5-1.2.0/pypx800v5.egg-info/SOURCES.txt` & `pypx800v5-1.2.1/pypx800v5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypx800v5-1.2.0/setup.py` & `pypx800v5-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pypx800v5",
-    version="1.2.0",
+    version="1.2.1",
     author="Aohzan",
     author_email="aohzan@gmail.com",
     description="Control the IPX800V5 and its extensions.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aohzan/pypx800v5",
     packages=setuptools.find_packages(),
```

