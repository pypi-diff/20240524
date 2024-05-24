# Comparing `tmp/mongomock_persistence-0.0.2.tar.gz` & `tmp/mongomock_persistence-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongomock_persistence-0.0.2.tar", last modified: Thu May 23 14:26:54 2024, max compression
+gzip compressed data, was "mongomock_persistence-0.0.3.tar", last modified: Fri May 24 13:56:06 2024, max compression
```

## Comparing `mongomock_persistence-0.0.2.tar` & `mongomock_persistence-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 14:26:54.376789 mongomock_persistence-0.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2024-05-23 07:12:01.000000 mongomock_persistence-0.0.2/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3682 2024-05-23 14:26:54.376789 mongomock_persistence-0.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2024-05-23 14:18:45.000000 mongomock_persistence-0.0.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 14:26:54.372789 mongomock_persistence-0.0.2/mongomock_persistence/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       65 2024-05-23 10:09:48.000000 mongomock_persistence-0.0.2/mongomock_persistence/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2529 2024-05-23 11:42:54.000000 mongomock_persistence-0.0.2/mongomock_persistence/store.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 14:26:54.376789 mongomock_persistence-0.0.2/mongomock_persistence.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3682 2024-05-23 14:26:54.000000 mongomock_persistence-0.0.2/mongomock_persistence.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      411 2024-05-23 14:26:54.000000 mongomock_persistence-0.0.2/mongomock_persistence.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 14:26:54.000000 mongomock_persistence-0.0.2/mongomock_persistence.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 14:25:07.000000 mongomock_persistence-0.0.2/mongomock_persistence.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2024-05-23 14:26:54.000000 mongomock_persistence-0.0.2/mongomock_persistence.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-05-23 14:26:54.000000 mongomock_persistence-0.0.2/mongomock_persistence.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       81 2024-05-23 12:29:37.000000 mongomock_persistence-0.0.2/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1048 2024-05-23 14:26:54.376789 mongomock_persistence-0.0.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       69 2024-05-23 12:12:28.000000 mongomock_persistence-0.0.2/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 14:26:54.372789 mongomock_persistence-0.0.2/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1836 2024-05-23 11:36:49.000000 mongomock_persistence-0.0.2/tests/test__persistence.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 13:56:06.846942 mongomock_persistence-0.0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2024-05-23 07:12:01.000000 mongomock_persistence-0.0.3/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3682 2024-05-24 13:56:06.846942 mongomock_persistence-0.0.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2683 2024-05-24 13:30:01.000000 mongomock_persistence-0.0.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 13:56:06.846942 mongomock_persistence-0.0.3/mongomock_persistence/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2024-05-24 13:54:40.000000 mongomock_persistence-0.0.3/mongomock_persistence/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1030 2024-05-24 13:54:40.000000 mongomock_persistence-0.0.3/mongomock_persistence/database.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2529 2024-05-24 13:30:01.000000 mongomock_persistence-0.0.3/mongomock_persistence/store.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 13:56:06.846942 mongomock_persistence-0.0.3/mongomock_persistence.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3682 2024-05-24 13:56:06.000000 mongomock_persistence-0.0.3/mongomock_persistence.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2024-05-24 13:56:06.000000 mongomock_persistence-0.0.3/mongomock_persistence.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-24 13:56:06.000000 mongomock_persistence-0.0.3/mongomock_persistence.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-24 13:56:06.000000 mongomock_persistence-0.0.3/mongomock_persistence.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2024-05-24 13:56:06.000000 mongomock_persistence-0.0.3/mongomock_persistence.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-05-24 13:56:06.000000 mongomock_persistence-0.0.3/mongomock_persistence.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       81 2024-05-24 13:30:01.000000 mongomock_persistence-0.0.3/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1048 2024-05-24 13:56:06.846942 mongomock_persistence-0.0.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       69 2024-05-24 13:30:01.000000 mongomock_persistence-0.0.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-24 13:56:06.846942 mongomock_persistence-0.0.3/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1836 2024-05-24 13:30:01.000000 mongomock_persistence-0.0.3/tests/test__persistence.py
```

### Comparing `mongomock_persistence-0.0.2/LICENSE` & `mongomock_persistence-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mongomock_persistence-0.0.2/PKG-INFO` & `mongomock_persistence-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomock-persistence
-Version: 0.0.2
+Version: 0.0.3
 Summary: Mongomock with persistence
 Author: Ivan Kondov
 Author-email: ivan.kondov@kit.edu
 License: BSD-3-Clause
 Keywords: database testing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mongomock_persistence-0.0.2/README.md` & `mongomock_persistence-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mongomock_persistence-0.0.2/mongomock_persistence/store.py` & `mongomock_persistence-0.0.3/mongomock_persistence/store.py`

 * *Files identical despite different names*

### Comparing `mongomock_persistence-0.0.2/mongomock_persistence.egg-info/PKG-INFO` & `mongomock_persistence-0.0.3/mongomock_persistence.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongomock-persistence
-Version: 0.0.2
+Version: 0.0.3
 Summary: Mongomock with persistence
 Author: Ivan Kondov
 Author-email: ivan.kondov@kit.edu
 License: BSD-3-Clause
 Keywords: database testing
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mongomock_persistence-0.0.2/setup.cfg` & `mongomock_persistence-0.0.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mongomock-persistence
-version = 0.0.2
+version = 0.0.3
 author = Ivan Kondov
 author_email = ivan.kondov@kit.edu
 description = Mongomock with persistence
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = database testing
 license = BSD-3-Clause
```

### Comparing `mongomock_persistence-0.0.2/tests/test__persistence.py` & `mongomock_persistence-0.0.3/tests/test__persistence.py`

 * *Files identical despite different names*

