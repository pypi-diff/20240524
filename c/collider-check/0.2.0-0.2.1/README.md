# Comparing `tmp/collider_check-0.2.0.tar.gz` & `tmp/collider_check-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collider_check-0.2.0.tar", last modified: Tue Apr 23 15:41:39 2024, max compression
+gzip compressed data, was "collider_check-0.2.1.tar", last modified: Fri May 24 07:46:56 2024, max compression
```

## Comparing `collider_check-0.2.0.tar` & `collider_check-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-04-23 15:41:39.693974 collider_check-0.2.0/
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1072 2024-04-23 15:24:05.000000 collider_check-0.2.0/LICENSE
--rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-04-23 15:41:39.693974 collider_check-0.2.0/PKG-INFO
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      798 2024-04-23 15:24:05.000000 collider_check-0.2.0/README.md
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      913 2024-04-23 15:37:53.000000 collider_check-0.2.0/pyproject.toml
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       38 2024-04-23 15:41:39.693974 collider_check-0.2.0/setup.cfg
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-04-23 15:41:39.693974 collider_check-0.2.0/src/
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-04-23 15:41:39.693974 collider_check-0.2.0/src/collider_check/
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1027 2024-04-23 15:24:05.000000 collider_check-0.2.0/src/collider_check/__init__.py
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)    27100 2024-04-23 15:36:13.000000 collider_check-0.2.0/src/collider_check/collider_check.py
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-04-23 15:41:39.693974 collider_check-0.2.0/src/collider_check.egg-info/
--rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-04-23 15:41:39.000000 collider_check-0.2.0/src/collider_check.egg-info/PKG-INFO
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      329 2024-04-23 15:41:39.000000 collider_check-0.2.0/src/collider_check.egg-info/SOURCES.txt
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)        1 2024-04-23 15:41:39.000000 collider_check-0.2.0/src/collider_check.egg-info/dependency_links.txt
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       64 2024-04-23 15:41:39.000000 collider_check-0.2.0/src/collider_check.egg-info/requires.txt
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       15 2024-04-23 15:41:39.000000 collider_check-0.2.0/src/collider_check.egg-info/top_level.txt
-drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-04-23 15:41:39.693974 collider_check-0.2.0/tests/
--rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     6763 2024-04-23 15:24:05.000000 collider_check-0.2.0/tests/test_check.py
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 07:46:56.247410 collider_check-0.2.1/
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1072 2024-04-23 15:24:05.000000 collider_check-0.2.1/LICENSE
+-rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-05-24 07:46:56.247410 collider_check-0.2.1/PKG-INFO
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      798 2024-04-23 15:24:05.000000 collider_check-0.2.1/README.md
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      913 2024-05-24 07:43:45.000000 collider_check-0.2.1/pyproject.toml
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       38 2024-05-24 07:46:56.247410 collider_check-0.2.1/setup.cfg
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 07:46:56.247410 collider_check-0.2.1/src/
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 07:46:56.247410 collider_check-0.2.1/src/collider_check/
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     1027 2024-05-24 07:44:25.000000 collider_check-0.2.1/src/collider_check/__init__.py
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)    27427 2024-05-24 07:43:16.000000 collider_check-0.2.1/src/collider_check/collider_check.py
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 07:46:56.247410 collider_check-0.2.1/src/collider_check.egg-info/
+-rw-r--r--   0 cdroin    (1018) cdroin    (1018)     2863 2024-05-24 07:46:56.000000 collider_check-0.2.1/src/collider_check.egg-info/PKG-INFO
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)      329 2024-05-24 07:46:56.000000 collider_check-0.2.1/src/collider_check.egg-info/SOURCES.txt
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)        1 2024-05-24 07:46:56.000000 collider_check-0.2.1/src/collider_check.egg-info/dependency_links.txt
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       64 2024-05-24 07:46:56.000000 collider_check-0.2.1/src/collider_check.egg-info/requires.txt
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)       15 2024-05-24 07:46:56.000000 collider_check-0.2.1/src/collider_check.egg-info/top_level.txt
+drwxrwxr-x   0 cdroin    (1018) cdroin    (1018)        0 2024-05-24 07:46:56.247410 collider_check-0.2.1/tests/
+-rw-rw-r--   0 cdroin    (1018) cdroin    (1018)     6763 2024-04-23 15:24:05.000000 collider_check-0.2.1/tests/test_check.py
```

### Comparing `collider_check-0.2.0/LICENSE` & `collider_check-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `collider_check-0.2.0/PKG-INFO` & `collider_check-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collider-check
-Version: 0.2.0
+Version: 0.2.1
 Summary: A small package that provides functions to check the observables in a collider, using a collider built with Xsuite.
 Author-email: Colas Droin <colas.noe.droin@cern.ch>
 License: MIT License
         
         Copyright (c) [2023] [Colas Droin]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `collider_check-0.2.0/README.md` & `collider_check-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `collider_check-0.2.0/pyproject.toml` & `collider_check-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = false
 
 [project]
 name = "collider-check"
-version = "0.2.0"
+version = "0.2.1"
 description = "A small package that provides functions to check the observables in a collider, using a collider built with Xsuite."
 readme = "README.md"
 authors = [{ name = "Colas Droin", email = "colas.noe.droin@cern.ch" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `collider_check-0.2.0/src/collider_check/__init__.py` & `collider_check-0.2.1/src/collider_check/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Package version
-__version__ = "0.1.7"
+__version__ = "0.2.1"
 
 import xtrack as xt
 
 # Import ColliderCheck class in the namespace
 from .collider_check import ColliderCheck
```

### Comparing `collider_check-0.2.0/src/collider_check/collider_check.py` & `collider_check-0.2.1/src/collider_check/collider_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,21 @@
 
     @property
     def nemitt_y(self):
         if self.configuration is not None:
             return self.configuration["config_collider"]["config_beambeam"]["nemitt_y"]
         print("Warning: no configuration provided. Using default value of 2.2e-6 for nemitt_y.")
         return 2.2e-6
+    
+    @property
+    def n_lr_per_side(self):
+        if self.configuration is not None:
+            return self.configuration["config_collider"]["config_beambeam"]["num_long_range_encounters_per_side"]['ip1']
+        print("Warning: no configuration provided. Using default value of 1 for n_lr_per_side.")
+        return 16
 
     def _check_configuration(self):
         if self.configuration is None:
             raise ValueError(
                 "No configuration has been provided when instantiating the ColliderCheck object."
             )
```

### Comparing `collider_check-0.2.0/src/collider_check.egg-info/PKG-INFO` & `collider_check-0.2.1/src/collider_check.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collider-check
-Version: 0.2.0
+Version: 0.2.1
 Summary: A small package that provides functions to check the observables in a collider, using a collider built with Xsuite.
 Author-email: Colas Droin <colas.noe.droin@cern.ch>
 License: MIT License
         
         Copyright (c) [2023] [Colas Droin]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `collider_check-0.2.0/tests/test_check.py` & `collider_check-0.2.1/tests/test_check.py`

 * *Files identical despite different names*

