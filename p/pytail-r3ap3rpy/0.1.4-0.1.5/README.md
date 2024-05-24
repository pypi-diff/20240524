# Comparing `tmp/pytail-r3ap3rpy-0.1.4.tar.gz` & `tmp/pytail_r3ap3rpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytail-r3ap3rpy-0.1.4.tar", last modified: Thu Feb 15 13:34:25 2024, max compression
+gzip compressed data, was "pytail_r3ap3rpy-0.1.5.tar", last modified: Fri May 24 17:01:26 2024, max compression
```

## Comparing `pytail-r3ap3rpy-0.1.4.tar` & `pytail_r3ap3rpy-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:34:25.821018 pytail-r3ap3rpy-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-15 13:34:25.821018 pytail-r3ap3rpy-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-02-15 13:34:19.000000 pytail-r3ap3rpy-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:34:25.821018 pytail-r3ap3rpy-0.1.4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1118 2024-02-15 13:34:19.000000 pytail-r3ap3rpy-0.1.4/bin/pytail
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:34:25.821018 pytail-r3ap3rpy-0.1.4/pytail/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-15 13:34:19.000000 pytail-r3ap3rpy-0.1.4/pytail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-02-15 13:34:19.000000 pytail-r3ap3rpy-0.1.4/pytail/pytail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 13:34:25.821018 pytail-r3ap3rpy-0.1.4/pytail_r3ap3rpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-15 13:34:25.000000 pytail-r3ap3rpy-0.1.4/pytail_r3ap3rpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-15 13:34:25.000000 pytail-r3ap3rpy-0.1.4/pytail_r3ap3rpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 13:34:25.000000 pytail-r3ap3rpy-0.1.4/pytail_r3ap3rpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-15 13:34:25.000000 pytail-r3ap3rpy-0.1.4/pytail_r3ap3rpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 13:34:25.821018 pytail-r3ap3rpy-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-15 13:34:19.000000 pytail-r3ap3rpy-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:01:26.761991 pytail_r3ap3rpy-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-24 17:01:26.761991 pytail_r3ap3rpy-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-24 17:01:21.000000 pytail_r3ap3rpy-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:01:26.757991 pytail_r3ap3rpy-0.1.5/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1118 2024-05-24 17:01:21.000000 pytail_r3ap3rpy-0.1.5/bin/pytail
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:01:26.757991 pytail_r3ap3rpy-0.1.5/pytail/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 17:01:21.000000 pytail_r3ap3rpy-0.1.5/pytail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-24 17:01:21.000000 pytail_r3ap3rpy-0.1.5/pytail/pytail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:01:26.761991 pytail_r3ap3rpy-0.1.5/pytail_r3ap3rpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-24 17:01:26.000000 pytail_r3ap3rpy-0.1.5/pytail_r3ap3rpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-24 17:01:26.000000 pytail_r3ap3rpy-0.1.5/pytail_r3ap3rpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:01:26.000000 pytail_r3ap3rpy-0.1.5/pytail_r3ap3rpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 17:01:26.000000 pytail_r3ap3rpy-0.1.5/pytail_r3ap3rpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 17:01:26.761991 pytail_r3ap3rpy-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-24 17:01:21.000000 pytail_r3ap3rpy-0.1.5/setup.py
```

### Comparing `pytail-r3ap3rpy-0.1.4/PKG-INFO` & `pytail_r3ap3rpy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytail-r3ap3rpy
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://pypi.org/project/pytail-r3ap3rpy/
 Author: Szabó Dániel Ernő
 Author-email: r3ap3rpy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytail-r3ap3rpy-0.1.4/README.md` & `pytail_r3ap3rpy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pytail-r3ap3rpy-0.1.4/bin/pytail` & `pytail_r3ap3rpy-0.1.5/bin/pytail`

 * *Files identical despite different names*

### Comparing `pytail-r3ap3rpy-0.1.4/pytail_r3ap3rpy.egg-info/PKG-INFO` & `pytail_r3ap3rpy-0.1.5/pytail_r3ap3rpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytail-r3ap3rpy
-Version: 0.1.4
+Version: 0.1.5
 Home-page: https://pypi.org/project/pytail-r3ap3rpy/
 Author: Szabó Dániel Ernő
 Author-email: r3ap3rpy@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pytail-r3ap3rpy-0.1.4/setup.py` & `pytail_r3ap3rpy-0.1.5/setup.py`

 * *Files identical despite different names*

