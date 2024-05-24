# Comparing `tmp/conf_master-1.0.1.tar.gz` & `tmp/conf_master-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_master-1.0.1.tar", max compression
+gzip compressed data, was "conf_master-1.0.2.tar", max compression
```

## Comparing `conf_master-1.0.1.tar` & `conf_master-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1107 2024-05-24 17:39:25.661378 conf_master-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1358 2024-05-24 18:47:26.433966 conf_master-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      519 2024-05-24 18:12:30.119187 conf_master-1.0.1/README.md
--rw-r--r--   0        0        0      109 2024-05-24 17:39:25.660379 conf_master-1.0.1/src/conf_master/__init__.py
--rw-r--r--   0        0        0     2072 2024-05-24 18:46:11.919554 conf_master-1.0.1/src/conf_master/conf_master.py
--rw-r--r--   0        0        0      332 2024-05-24 18:37:34.117998 conf_master-1.0.1/src/conf_master/exceptions.py
--rw-r--r--   0        0        0      531 2024-05-24 18:46:56.010723 conf_master-1.0.1/src/conf_master/loaders.py
--rw-r--r--   0        0        0      345 2024-05-24 18:25:51.397917 conf_master-1.0.1/src/conf_master/validators.py
--rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 conf_master-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1107 2024-05-24 17:39:25.661378 conf_master-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1358 2024-05-24 18:53:57.322786 conf_master-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      519 2024-05-24 18:12:30.119187 conf_master-1.0.2/README.md
+-rw-r--r--   0        0        0      109 2024-05-24 17:39:25.660379 conf_master-1.0.2/src/conf_master/__init__.py
+-rw-r--r--   0        0        0     2072 2024-05-24 18:46:11.919554 conf_master-1.0.2/src/conf_master/conf_master.py
+-rw-r--r--   0        0        0      332 2024-05-24 18:37:34.117998 conf_master-1.0.2/src/conf_master/exceptions.py
+-rw-r--r--   0        0        0      531 2024-05-24 18:46:56.010723 conf_master-1.0.2/src/conf_master/loaders.py
+-rw-r--r--   0        0        0      481 2024-05-24 18:53:46.070893 conf_master-1.0.2/src/conf_master/validators.py
+-rw-r--r--   0        0        0     1484 1970-01-01 00:00:00.000000 conf_master-1.0.2/PKG-INFO
```

### Comparing `conf_master-1.0.1/LICENSE.txt` & `conf_master-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conf_master-1.0.1/pyproject.toml` & `conf_master-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "conf-master"
-version = "1.0.1"
+version = "1.0.2"
 description = ""
 readme = "README.md"
 authors = ["alvaroroco <alvaroroco@gmail.com>"]
 license = "MIT"
 keywords = []
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `conf_master-1.0.1/README.md` & `conf_master-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `conf_master-1.0.1/src/conf_master/conf_master.py` & `conf_master-1.0.2/src/conf_master/conf_master.py`

 * *Files identical despite different names*

### Comparing `conf_master-1.0.1/src/conf_master/loaders.py` & `conf_master-1.0.2/src/conf_master/loaders.py`

 * *Files identical despite different names*

### Comparing `conf_master-1.0.1/PKG-INFO` & `conf_master-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf-master
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 License: MIT
 Author: alvaroroco
 Author-email: alvaroroco@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

