# Comparing `tmp/domolibrary_execution-0.0.8.tar.gz` & `tmp/domolibrary_execution-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary_execution-0.0.8.tar", last modified: Thu May  9 19:49:19 2024, max compression
+gzip compressed data, was "domolibrary_execution-0.0.9.tar", last modified: Tue May 14 00:58:50 2024, max compression
```

## Comparing `domolibrary_execution-0.0.8.tar` & `domolibrary_execution-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-09 19:49:19.596207 domolibrary_execution-0.0.8/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.8/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.8/MANIFEST.in
--rw-r--r--   0 codespace  (1000) codespace  (1000)      810 2024-05-09 19:49:19.596207 domolibrary_execution-0.0.8/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-04-19 18:24:29.000000 domolibrary_execution-0.0.8/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-09 19:49:19.592207 domolibrary_execution-0.0.8/domolibrary_execution/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4304 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/FactoryAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5903 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/FactoryRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3582 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/FactoryUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.8/domolibrary_execution/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15277 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/_modidx.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2680 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.8/domolibrary_execution/process.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-09 19:49:19.592207 domolibrary_execution-0.0.8/domolibrary_execution/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2968 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/utils/domojupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7104 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/utils/factory.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-09 19:49:19.592207 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      810 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      700 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 18:25:06.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      923 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-09 19:49:19.596207 domolibrary_execution-0.0.8/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2596 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.8/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-14 00:58:50.241508 domolibrary_execution-0.0.9/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.9/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.9/MANIFEST.in
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      810 2024-05-14 00:58:50.241508 domolibrary_execution-0.0.9/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-04-19 18:24:29.000000 domolibrary_execution-0.0.9/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-14 00:58:50.229508 domolibrary_execution-0.0.9/domolibrary_execution/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4304 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.9/domolibrary_execution/FactoryAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5903 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.9/domolibrary_execution/FactoryRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3582 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.9/domolibrary_execution/FactoryUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.9/domolibrary_execution/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15277 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.9/domolibrary_execution/_modidx.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2680 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.9/domolibrary_execution/process.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-14 00:58:50.241508 domolibrary_execution-0.0.9/domolibrary_execution/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.9/domolibrary_execution/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2968 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.9/domolibrary_execution/utils/domojupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7104 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.9/domolibrary_execution/utils/factory.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-14 00:58:50.237508 domolibrary_execution-0.0.9/domolibrary_execution.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      810 2024-05-14 00:58:50.000000 domolibrary_execution-0.0.9/domolibrary_execution.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      700 2024-05-14 00:58:50.000000 domolibrary_execution-0.0.9/domolibrary_execution.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-14 00:58:50.000000 domolibrary_execution-0.0.9/domolibrary_execution.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2024-05-14 00:58:50.000000 domolibrary_execution-0.0.9/domolibrary_execution.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 18:25:06.000000 domolibrary_execution-0.0.9/domolibrary_execution.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2024-05-14 00:58:50.000000 domolibrary_execution-0.0.9/domolibrary_execution.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-05-14 00:58:50.000000 domolibrary_execution-0.0.9/domolibrary_execution.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      923 2024-05-14 00:55:45.000000 domolibrary_execution-0.0.9/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-14 00:58:50.241508 domolibrary_execution-0.0.9/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2596 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.9/setup.py
```

### Comparing `domolibrary_execution-0.0.8/LICENSE` & `domolibrary_execution-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.8/PKG-INFO` & `domolibrary_execution-0.0.9/domolibrary_execution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: domolibrary_execution
-Version: 0.0.8
+Name: domolibrary-execution
+Version: 0.0.9
 Home-page: https://github.com//domolibrary_execution
 Author: 
 Author-email: 
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary_execution-0.0.8/domolibrary_execution/FactoryAuth.py` & `domolibrary_execution-0.0.9/domolibrary_execution/FactoryAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.8/domolibrary_execution/FactoryRole.py` & `domolibrary_execution-0.0.9/domolibrary_execution/FactoryRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.8/domolibrary_execution/FactoryUser.py` & `domolibrary_execution-0.0.9/domolibrary_execution/FactoryUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.8/domolibrary_execution/_modidx.py` & `domolibrary_execution-0.0.9/domolibrary_execution/_modidx.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.8/domolibrary_execution/process.py` & `domolibrary_execution-0.0.9/domolibrary_execution/process.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.8/domolibrary_execution/utils/domojupyter.py` & `domolibrary_execution-0.0.9/domolibrary_execution/utils/domojupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.8/domolibrary_execution/utils/factory.py` & `domolibrary_execution-0.0.9/domolibrary_execution/utils/factory.py`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.8/domolibrary_execution.egg-info/PKG-INFO` & `domolibrary_execution-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: domolibrary-execution
-Version: 0.0.8
+Name: domolibrary_execution
+Version: 0.0.9
 Home-page: https://github.com//domolibrary_execution
 Author: 
 Author-email: 
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary_execution-0.0.8/domolibrary_execution.egg-info/SOURCES.txt` & `domolibrary_execution-0.0.9/domolibrary_execution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.8/settings.ini` & `domolibrary_execution-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domolibrary_execution
 lib_name = %(repo)s
-version = 0.0.8
+version = 0.0.9
 min_python = 3.8
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = %(repo)s
```

### Comparing `domolibrary_execution-0.0.8/setup.py` & `domolibrary_execution-0.0.9/setup.py`

 * *Files identical despite different names*

