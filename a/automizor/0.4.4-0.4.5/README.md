# Comparing `tmp/automizor-0.4.4.tar.gz` & `tmp/automizor-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automizor-0.4.4.tar", last modified: Thu May  2 17:24:17 2024, max compression
+gzip compressed data, was "automizor-0.4.5.tar", last modified: Fri May 24 14:00:28 2024, max compression
```

## Comparing `automizor-0.4.4.tar` & `automizor-0.4.5.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:24:17.373111 automizor-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-02 17:24:08.000000 automizor-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 17:24:08.000000 automizor-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 17:24:17.373111 automizor-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 17:24:08.000000 automizor-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:24:17.369111 automizor-0.4.4/automizor/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:24:17.369111 automizor-0.4.4/automizor/job/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/job/_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:24:17.369111 automizor-0.4.4/automizor/log/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/log/_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:24:17.369111 automizor-0.4.4/automizor/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/storage/_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:24:17.373111 automizor-0.4.4/automizor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:24:17.373111 automizor-0.4.4/automizor/vault/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/vault/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-02 17:24:08.000000 automizor-0.4.4/automizor/vault/_vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:24:17.373111 automizor-0.4.4/automizor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 17:24:17.000000 automizor-0.4.4/automizor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 17:24:17.000000 automizor-0.4.4/automizor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:24:17.000000 automizor-0.4.4/automizor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 17:24:17.000000 automizor-0.4.4/automizor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 17:24:17.000000 automizor-0.4.4/automizor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 17:24:17.373111 automizor-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 17:24:08.000000 automizor-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:00:28.840700 automizor-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-24 14:00:20.000000 automizor-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-24 14:00:20.000000 automizor-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-24 14:00:28.840700 automizor-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 14:00:20.000000 automizor-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:00:28.840700 automizor-0.4.5/automizor/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:00:28.840700 automizor-0.4.5/automizor/datastore/
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/datastore/_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:00:28.840700 automizor-0.4.5/automizor/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/job/_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:00:28.840700 automizor-0.4.5/automizor/log/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/log/_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:00:28.840700 automizor-0.4.5/automizor/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/storage/_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:00:28.840700 automizor-0.4.5/automizor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:00:28.840700 automizor-0.4.5/automizor/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/vault/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4688 2024-05-24 14:00:20.000000 automizor-0.4.5/automizor/vault/_vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:00:28.840700 automizor-0.4.5/automizor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-24 14:00:28.000000 automizor-0.4.5/automizor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-24 14:00:28.000000 automizor-0.4.5/automizor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:00:28.000000 automizor-0.4.5/automizor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 14:00:28.000000 automizor-0.4.5/automizor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 14:00:28.000000 automizor-0.4.5/automizor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 14:00:28.844700 automizor-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-24 14:00:20.000000 automizor-0.4.5/setup.py
```

### Comparing `automizor-0.4.4/LICENSE` & `automizor-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/PKG-INFO` & `automizor-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automizor
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python Automizor framework
 Home-page: https://github.com/automizor/automizor-python
 Author: Christian Fischer
 Author-email: christian@automizor.io
 License: Apache License
 Keywords: automizor framework
 Classifier: Intended Audience :: Developers
```

### Comparing `automizor-0.4.4/automizor/exceptions.py` & `automizor-0.4.5/automizor/exceptions.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/automizor/job/__init__.py` & `automizor-0.4.5/automizor/job/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/automizor/job/_job.py` & `automizor-0.4.5/automizor/job/_job.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/automizor/log/__init__.py` & `automizor-0.4.5/automizor/log/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/automizor/log/_log.py` & `automizor-0.4.5/automizor/log/_log.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/automizor/storage/__init__.py` & `automizor-0.4.5/automizor/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/automizor/storage/_storage.py` & `automizor-0.4.5/automizor/storage/_storage.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/automizor/utils/__init__.py` & `automizor-0.4.5/automizor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/automizor/vault/__init__.py` & `automizor-0.4.5/automizor/vault/__init__.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/automizor/vault/_container.py` & `automizor-0.4.5/automizor/vault/_container.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/automizor/vault/_vault.py` & `automizor-0.4.5/automizor/vault/_vault.py`

 * *Files identical despite different names*

### Comparing `automizor-0.4.4/automizor.egg-info/PKG-INFO` & `automizor-0.4.5/automizor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automizor
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python Automizor framework
 Home-page: https://github.com/automizor/automizor-python
 Author: Christian Fischer
 Author-email: christian@automizor.io
 License: Apache License
 Keywords: automizor framework
 Classifier: Intended Audience :: Developers
```

### Comparing `automizor-0.4.4/automizor.egg-info/SOURCES.txt` & `automizor-0.4.5/automizor.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 automizor/__init__.py
 automizor/exceptions.py
 automizor.egg-info/PKG-INFO
 automizor.egg-info/SOURCES.txt
 automizor.egg-info/dependency_links.txt
 automizor.egg-info/requires.txt
 automizor.egg-info/top_level.txt
+automizor/datastore/__init__.py
+automizor/datastore/_datastore.py
 automizor/job/__init__.py
 automizor/job/_job.py
 automizor/log/__init__.py
 automizor/log/_log.py
 automizor/storage/__init__.py
 automizor/storage/_storage.py
 automizor/utils/__init__.py
```

### Comparing `automizor-0.4.4/setup.py` & `automizor-0.4.5/setup.py`

 * *Files identical despite different names*

