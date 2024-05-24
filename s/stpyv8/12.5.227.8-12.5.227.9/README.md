# Comparing `tmp/stpyv8-12.5.227.8.tar.gz` & `tmp/stpyv8-12.5.227.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stpyv8-12.5.227.8.tar", last modified: Thu May 16 09:39:40 2024, max compression
+gzip compressed data, was "stpyv8-12.5.227.9.tar", last modified: Fri May 24 11:47:52 2024, max compression
```

## Comparing `stpyv8-12.5.227.8.tar` & `stpyv8-12.5.227.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:40.058517 stpyv8-12.5.227.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-05-16 09:39:40.058517 stpyv8-12.5.227.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10787 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/STPyV8.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:39:40.058517 stpyv8-12.5.227.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:40.054517 stpyv8-12.5.227.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/src/Context.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/src/Engine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    16149 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/src/Exception.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/src/Isolate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/src/Locker.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/src/Platform.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/src/STPyV8.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/src/Utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    60620 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/src/Wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:40.054517 stpyv8-12.5.227.8/stpyv8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-05-16 09:39:40.000000 stpyv8-12.5.227.8/stpyv8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-16 09:39:40.000000 stpyv8-12.5.227.8/stpyv8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:39:40.000000 stpyv8-12.5.227.8/stpyv8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 09:39:40.000000 stpyv8-12.5.227.8/stpyv8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 09:39:40.000000 stpyv8-12.5.227.8/stpyv8.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:39:40.054517 stpyv8-12.5.227.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/tests/test_Context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/tests/test_Engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/tests/test_ICU.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/tests/test_Isolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/tests/test_Locker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/tests/test_Thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    36586 2024-05-16 09:39:36.000000 stpyv8-12.5.227.8/tests/test_Wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:52.165703 stpyv8-12.5.227.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-05-24 11:47:52.165703 stpyv8-12.5.227.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10787 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/STPyV8.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 11:47:52.165703 stpyv8-12.5.227.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:52.161703 stpyv8-12.5.227.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/src/Context.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/src/Engine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16149 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/src/Exception.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/src/Isolate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/src/Locker.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/src/Platform.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/src/STPyV8.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/src/Utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    60620 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/src/Wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:52.165703 stpyv8-12.5.227.9/stpyv8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-05-24 11:47:52.000000 stpyv8-12.5.227.9/stpyv8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-24 11:47:52.000000 stpyv8-12.5.227.9/stpyv8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:47:52.000000 stpyv8-12.5.227.9/stpyv8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 11:47:52.000000 stpyv8-12.5.227.9/stpyv8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-24 11:47:52.000000 stpyv8-12.5.227.9/stpyv8.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:47:52.165703 stpyv8-12.5.227.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/tests/test_Context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/tests/test_Engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/tests/test_ICU.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/tests/test_Isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/tests/test_Locker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/tests/test_Thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36586 2024-05-24 11:47:48.000000 stpyv8-12.5.227.9/tests/test_Wrapper.py
```

### Comparing `stpyv8-12.5.227.8/LICENSE.txt` & `stpyv8-12.5.227.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/PKG-INFO` & `stpyv8-12.5.227.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stpyv8
-Version: 12.5.227.8
+Version: 12.5.227.9
 Summary: Python Wrapper for Google V8 Engine
 Home-page: https://github.com/cloudflare/stpyv8
 Author: Philip Syme, Angelo Dell'Aera
 License: Apache License 2.0
 Platform: x86
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `stpyv8-12.5.227.8/README.md` & `stpyv8-12.5.227.9/README.md`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/STPyV8.py` & `stpyv8-12.5.227.9/STPyV8.py`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/setup.py` & `stpyv8-12.5.227.9/setup.py`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/src/Context.cpp` & `stpyv8-12.5.227.9/src/Context.cpp`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/src/Engine.cpp` & `stpyv8-12.5.227.9/src/Engine.cpp`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/src/Exception.cpp` & `stpyv8-12.5.227.9/src/Exception.cpp`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/src/Isolate.cpp` & `stpyv8-12.5.227.9/src/Isolate.cpp`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/src/Locker.cpp` & `stpyv8-12.5.227.9/src/Locker.cpp`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/src/Platform.cpp` & `stpyv8-12.5.227.9/src/Platform.cpp`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/src/Utils.cpp` & `stpyv8-12.5.227.9/src/Utils.cpp`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/src/Wrapper.cpp` & `stpyv8-12.5.227.9/src/Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/stpyv8.egg-info/PKG-INFO` & `stpyv8-12.5.227.9/stpyv8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stpyv8
-Version: 12.5.227.8
+Version: 12.5.227.9
 Summary: Python Wrapper for Google V8 Engine
 Home-page: https://github.com/cloudflare/stpyv8
 Author: Philip Syme, Angelo Dell'Aera
 License: Apache License 2.0
 Platform: x86
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
```

### Comparing `stpyv8-12.5.227.8/tests/test_Context.py` & `stpyv8-12.5.227.9/tests/test_Context.py`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/tests/test_Engine.py` & `stpyv8-12.5.227.9/tests/test_Engine.py`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/tests/test_ICU.py` & `stpyv8-12.5.227.9/tests/test_ICU.py`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/tests/test_Locker.py` & `stpyv8-12.5.227.9/tests/test_Locker.py`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/tests/test_Thread.py` & `stpyv8-12.5.227.9/tests/test_Thread.py`

 * *Files identical despite different names*

### Comparing `stpyv8-12.5.227.8/tests/test_Wrapper.py` & `stpyv8-12.5.227.9/tests/test_Wrapper.py`

 * *Files identical despite different names*

