# Comparing `tmp/python_inoreader-0.7.0.tar.gz` & `tmp/python_inoreader-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_inoreader-0.7.0.tar", last modified: Fri May  3 11:17:38 2024, max compression
+gzip compressed data, was "python_inoreader-0.7.1.tar", last modified: Fri May 24 09:21:43 2024, max compression
```

## Comparing `python_inoreader-0.7.0.tar` & `python_inoreader-0.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:17:38.012538 python_inoreader-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-03 11:17:38.012538 python_inoreader-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:17:38.012538 python_inoreader-0.7.0/inoreader/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/article.py
--rw-r--r--   0 runner    (1001) docker     (127)    10436 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22407 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/sim.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/inoreader/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-03 11:17:29.000000 python_inoreader-0.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:17:38.012538 python_inoreader-0.7.0/python_inoreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 11:17:38.000000 python_inoreader-0.7.0/python_inoreader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:17:38.012538 python_inoreader-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:21:43.836351 python_inoreader-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-24 09:21:43.836351 python_inoreader-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:21:43.836351 python_inoreader-0.7.1/inoreader/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/inoreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/inoreader/article.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/inoreader/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/inoreader/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/inoreader/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/inoreader/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/inoreader/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22407 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/inoreader/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/inoreader/sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/inoreader/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/inoreader/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-24 09:21:39.000000 python_inoreader-0.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:21:43.836351 python_inoreader-0.7.1/python_inoreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-24 09:21:43.000000 python_inoreader-0.7.1/python_inoreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-24 09:21:43.000000 python_inoreader-0.7.1/python_inoreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:21:43.000000 python_inoreader-0.7.1/python_inoreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 09:21:43.000000 python_inoreader-0.7.1/python_inoreader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 09:21:43.000000 python_inoreader-0.7.1/python_inoreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 09:21:43.000000 python_inoreader-0.7.1/python_inoreader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 09:21:43.840351 python_inoreader-0.7.1/setup.cfg
```

### Comparing `python_inoreader-0.7.0/PKG-INFO` & `python_inoreader-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-inoreader
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python wrapper of Inoreader API
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Linusp/python-inoreader
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python_inoreader-0.7.0/README.md` & `python_inoreader-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `python_inoreader-0.7.0/inoreader/article.py` & `python_inoreader-0.7.1/inoreader/article.py`

 * *Files identical despite different names*

### Comparing `python_inoreader-0.7.0/inoreader/client.py` & `python_inoreader-0.7.1/inoreader/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,19 @@
             return response["items"], None
 
     def fetch_articles(
         self, stream_id=None, folder=None, tags=None, unread=True, starred=False, limit=None, n=50
     ):
         self.check_token()
 
-        if not stream_id and folder:
-            stream_id = self.GENERAL_TAG_TEMPLATE.format(folder)
+        if not stream_id:
+            if folder:
+                stream_id = self.GENERAL_TAG_TEMPLATE.format(folder)
+            elif tags:
+                stream_id = self.GENERAL_TAG_TEMPLATE.format(tags[0])
 
         params = {"stream_id": stream_id, "n": n, "c": str(uuid4())}
         if unread:
             params["xt"] = self.READ_TAG
 
         if starred:
             params["it"] = self.STARRED_TAG
```

### Comparing `python_inoreader-0.7.0/inoreader/config.py` & `python_inoreader-0.7.1/inoreader/config.py`

 * *Files identical despite different names*

### Comparing `python_inoreader-0.7.0/inoreader/filter.py` & `python_inoreader-0.7.1/inoreader/filter.py`

 * *Files identical despite different names*

### Comparing `python_inoreader-0.7.0/inoreader/main.py` & `python_inoreader-0.7.1/inoreader/main.py`

 * *Files identical despite different names*

### Comparing `python_inoreader-0.7.0/inoreader/sim.py` & `python_inoreader-0.7.1/inoreader/sim.py`

 * *Files identical despite different names*

### Comparing `python_inoreader-0.7.0/inoreader/subscription.py` & `python_inoreader-0.7.1/inoreader/subscription.py`

 * *Files identical despite different names*

### Comparing `python_inoreader-0.7.0/inoreader/utils.py` & `python_inoreader-0.7.1/inoreader/utils.py`

 * *Files identical despite different names*

### Comparing `python_inoreader-0.7.0/pyproject.toml` & `python_inoreader-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-inoreader"
-version = "0.7.0"
+version = "0.7.1"
 description = "Python wrapper of Inoreader API"
 authors = [
     {name = "Linusp", email = "linusp1024@gmail.com"},
 ]
 dependencies = [
     "lxml",
     "requests",
```

### Comparing `python_inoreader-0.7.0/python_inoreader.egg-info/PKG-INFO` & `python_inoreader-0.7.1/python_inoreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-inoreader
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python wrapper of Inoreader API
 Author-email: Linusp <linusp1024@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Linusp/python-inoreader
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

