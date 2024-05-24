# Comparing `tmp/beambusters-1.3.2.tar.gz` & `tmp/beambusters-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beambusters-1.3.2.tar", max compression
+gzip compressed data, was "beambusters-1.3.3.tar", max compression
```

## Comparing `beambusters-1.3.2.tar` & `beambusters-1.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-05-24 12:54:44.154505 beambusters-1.3.2/LICENSE
--rw-r--r--   0        0        0      630 2024-05-24 12:54:44.154505 beambusters-1.3.2/README.md
--rwxr-xr-x   0        0        0        0 2024-05-24 12:54:44.154505 beambusters-1.3.2/beambusters/__init__.py
--rw-r--r--   0        0        0    12068 2024-05-24 12:54:44.154505 beambusters-1.3.2/beambusters/main.py
--rwxr-xr-x   0        0        0     3562 2024-05-24 12:54:44.154505 beambusters-1.3.2/beambusters/settings.py
--rwxr-xr-x   0        0        0     1394 2024-05-24 12:54:44.154505 beambusters-1.3.2/beambusters/utils.py
--rw-r--r--   0        0        0     2027 2024-05-24 12:54:56.002505 beambusters-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     3969 1970-01-01 00:00:00.000000 beambusters-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-24 13:01:40.140686 beambusters-1.3.3/LICENSE
+-rw-r--r--   0        0        0      630 2024-05-24 13:01:40.140686 beambusters-1.3.3/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-24 13:01:40.140686 beambusters-1.3.3/beambusters/__init__.py
+-rw-r--r--   0        0        0    12068 2024-05-24 13:01:40.140686 beambusters-1.3.3/beambusters/main.py
+-rwxr-xr-x   0        0        0     3562 2024-05-24 13:01:40.140686 beambusters-1.3.3/beambusters/settings.py
+-rwxr-xr-x   0        0        0     1394 2024-05-24 13:01:40.140686 beambusters-1.3.3/beambusters/utils.py
+-rw-r--r--   0        0        0     2027 2024-05-24 13:01:51.064720 beambusters-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3969 1970-01-01 00:00:00.000000 beambusters-1.3.3/PKG-INFO
```

### Comparing `beambusters-1.3.2/LICENSE` & `beambusters-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.2/README.md` & `beambusters-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.2/beambusters/main.py` & `beambusters-1.3.3/beambusters/main.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.2/beambusters/settings.py` & `beambusters-1.3.3/beambusters/settings.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.2/beambusters/utils.py` & `beambusters-1.3.3/beambusters/utils.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.2/pyproject.toml` & `beambusters-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beambusters"
-version = "1.3.2"
+version = "1.3.3"
 description = ""
 authors = ["Ana Rodrigues <anananacr@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 beambusters = "beambusters.main:app"
```

### Comparing `beambusters-1.3.2/PKG-INFO` & `beambusters-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beambusters
-Version: 1.3.2
+Version: 1.3.3
 Summary: 
 Author: Ana Rodrigues
 Author-email: anananacr@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

