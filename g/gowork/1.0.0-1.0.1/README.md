# Comparing `tmp/gowork-1.0.0.tar.gz` & `tmp/gowork-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gowork-1.0.0.tar", last modified: Tue Apr 16 20:15:06 2024, max compression
+gzip compressed data, was "gowork-1.0.1.tar", last modified: Fri May 24 12:37:42 2024, max compression
```

## Comparing `gowork-1.0.0.tar` & `gowork-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:15:05.996420 gowork-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-16 20:15:05.996420 gowork-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-16 20:14:54.000000 gowork-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:15:05.996420 gowork-1.0.0/gowork/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:15:05.996420 gowork-1.0.0/gowork/safe/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/safe/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:15:05.996420 gowork-1.0.0/gowork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-16 20:15:05.000000 gowork-1.0.0/gowork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-16 20:15:05.000000 gowork-1.0.0/gowork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:15:05.000000 gowork-1.0.0/gowork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 20:15:05.000000 gowork-1.0.0/gowork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 20:15:05.000000 gowork-1.0.0/gowork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:15:05.996420 gowork-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 20:14:54.000000 gowork-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:37:42.699927 gowork-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-24 12:37:42.695927 gowork-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-24 12:37:35.000000 gowork-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:37:42.695927 gowork-1.0.1/gowork/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-24 12:37:35.000000 gowork-1.0.1/gowork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-24 12:37:35.000000 gowork-1.0.1/gowork/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-24 12:37:35.000000 gowork-1.0.1/gowork/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-24 12:37:35.000000 gowork-1.0.1/gowork/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:37:42.695927 gowork-1.0.1/gowork/safe/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-24 12:37:35.000000 gowork-1.0.1/gowork/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-24 12:37:35.000000 gowork-1.0.1/gowork/safe/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:37:42.695927 gowork-1.0.1/gowork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-24 12:37:42.000000 gowork-1.0.1/gowork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-24 12:37:42.000000 gowork-1.0.1/gowork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:37:42.000000 gowork-1.0.1/gowork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-24 12:37:42.000000 gowork-1.0.1/gowork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 12:37:42.000000 gowork-1.0.1/gowork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:37:42.699927 gowork-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-24 12:37:35.000000 gowork-1.0.1/setup.py
```

### Comparing `gowork-1.0.0/PKG-INFO` & `gowork-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gowork
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to help track your credentials and database engines
 Home-page: https://github.com/Phomint/GoWork
 Author: Patrick Amaral
 Author-email: patrick.dev.atom@gmail.com
 License: GPLv3
 Keywords: databases,athena,mysql,mongodb
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gowork-1.0.0/README.rst` & `gowork-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `gowork-1.0.0/gowork/databases.py` & `gowork-1.0.1/gowork/databases.py`

 * *Files identical despite different names*

### Comparing `gowork-1.0.0/gowork/monitor.py` & `gowork-1.0.1/gowork/monitor.py`

 * *Files identical despite different names*

### Comparing `gowork-1.0.0/gowork/safe/configs.py` & `gowork-1.0.1/gowork/safe/configs.py`

 * *Files identical despite different names*

### Comparing `gowork-1.0.0/gowork.egg-info/PKG-INFO` & `gowork-1.0.1/gowork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gowork
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to help track your credentials and database engines
 Home-page: https://github.com/Phomint/GoWork
 Author: Patrick Amaral
 Author-email: patrick.dev.atom@gmail.com
 License: GPLv3
 Keywords: databases,athena,mysql,mongodb
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gowork-1.0.0/setup.py` & `gowork-1.0.1/setup.py`

 * *Files identical despite different names*

