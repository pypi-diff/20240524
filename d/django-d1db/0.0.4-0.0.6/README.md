# Comparing `tmp/django_d1db-0.0.4.tar.gz` & `tmp/django_d1db-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_d1db-0.0.4.tar", last modified: Mon May 20 21:47:04 2024, max compression
+gzip compressed data, was "django_d1db-0.0.6.tar", last modified: Fri May 24 21:45:46 2024, max compression
```

## Comparing `django_d1db-0.0.4.tar` & `django_d1db-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-20 21:47:04.723789 django_d1db-0.0.4/
--rw-r--r--   0 gmassadas   (502) staff       (20)     1073 2024-05-20 16:10:54.000000 django_d1db-0.0.4/LICENSE
--rw-r--r--   0 gmassadas   (502) staff       (20)     1563 2024-05-20 21:47:04.723010 django_d1db-0.0.4/PKG-INFO
--rw-r--r--   0 gmassadas   (502) staff       (20)      771 2024-05-20 17:09:44.000000 django_d1db-0.0.4/README.md
-drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-20 21:47:04.719098 django_d1db-0.0.4/django_d1/
--rw-r--r--   0 gmassadas   (502) staff       (20)        0 2024-05-19 10:45:59.000000 django_d1db-0.0.4/django_d1/__init__.py
--rw-r--r--   0 gmassadas   (502) staff       (20)     2674 2024-05-20 20:58:52.000000 django_d1db-0.0.4/django_d1/base.py
--rw-r--r--   0 gmassadas   (502) staff       (20)      140 2024-05-20 17:29:56.000000 django_d1db-0.0.4/django_d1/client.py
--rw-r--r--   0 gmassadas   (502) staff       (20)      150 2024-05-20 17:29:56.000000 django_d1db-0.0.4/django_d1/creation.py
--rw-r--r--   0 gmassadas   (502) staff       (20)     5219 2024-05-20 20:46:35.000000 django_d1db-0.0.4/django_d1/database.py
--rw-r--r--   0 gmassadas   (502) staff       (20)     1277 2024-05-20 21:46:50.000000 django_d1db-0.0.4/django_d1/features.py
--rw-r--r--   0 gmassadas   (502) staff       (20)      175 2024-05-20 17:29:56.000000 django_d1db-0.0.4/django_d1/introspection.py
--rw-r--r--   0 gmassadas   (502) staff       (20)     2719 2024-05-20 21:42:30.000000 django_d1db-0.0.4/django_d1/operations.py
--rw-r--r--   0 gmassadas   (502) staff       (20)      415 2024-05-20 17:29:56.000000 django_d1db-0.0.4/django_d1/schema.py
-drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-20 21:47:04.722125 django_d1db-0.0.4/django_d1db.egg-info/
--rw-r--r--   0 gmassadas   (502) staff       (20)     1563 2024-05-20 21:47:04.000000 django_d1db-0.0.4/django_d1db.egg-info/PKG-INFO
--rw-r--r--   0 gmassadas   (502) staff       (20)      369 2024-05-20 21:47:04.000000 django_d1db-0.0.4/django_d1db.egg-info/SOURCES.txt
--rw-r--r--   0 gmassadas   (502) staff       (20)        1 2024-05-20 21:47:04.000000 django_d1db-0.0.4/django_d1db.egg-info/dependency_links.txt
--rw-r--r--   0 gmassadas   (502) staff       (20)       10 2024-05-20 21:47:04.000000 django_d1db-0.0.4/django_d1db.egg-info/top_level.txt
--rw-r--r--   0 gmassadas   (502) staff       (20)      785 2024-05-20 21:46:50.000000 django_d1db-0.0.4/pyproject.toml
--rw-r--r--   0 gmassadas   (502) staff       (20)       38 2024-05-20 21:47:04.723960 django_d1db-0.0.4/setup.cfg
+drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-24 21:45:46.601437 django_d1db-0.0.6/
+-rw-r--r--   0 gmassadas   (502) staff       (20)     1073 2024-05-20 16:10:54.000000 django_d1db-0.0.6/LICENSE
+-rw-r--r--   0 gmassadas   (502) staff       (20)     1563 2024-05-24 21:45:46.600762 django_d1db-0.0.6/PKG-INFO
+-rw-r--r--   0 gmassadas   (502) staff       (20)      771 2024-05-20 17:09:44.000000 django_d1db-0.0.6/README.md
+drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-24 21:45:46.596050 django_d1db-0.0.6/django_d1/
+-rw-r--r--   0 gmassadas   (502) staff       (20)        0 2024-05-19 10:45:59.000000 django_d1db-0.0.6/django_d1/__init__.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)     2674 2024-05-20 20:58:52.000000 django_d1db-0.0.6/django_d1/base.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)      140 2024-05-20 17:29:56.000000 django_d1db-0.0.6/django_d1/client.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)      150 2024-05-20 17:29:56.000000 django_d1db-0.0.6/django_d1/creation.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)     5610 2024-05-24 21:44:42.000000 django_d1db-0.0.6/django_d1/database.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)     1277 2024-05-20 21:46:50.000000 django_d1db-0.0.6/django_d1/features.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)      175 2024-05-20 17:29:56.000000 django_d1db-0.0.6/django_d1/introspection.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)     2719 2024-05-20 21:42:30.000000 django_d1db-0.0.6/django_d1/operations.py
+-rw-r--r--   0 gmassadas   (502) staff       (20)      415 2024-05-20 17:29:56.000000 django_d1db-0.0.6/django_d1/schema.py
+drwxr-xr-x   0 gmassadas   (502) staff       (20)        0 2024-05-24 21:45:46.599666 django_d1db-0.0.6/django_d1db.egg-info/
+-rw-r--r--   0 gmassadas   (502) staff       (20)     1563 2024-05-24 21:45:46.000000 django_d1db-0.0.6/django_d1db.egg-info/PKG-INFO
+-rw-r--r--   0 gmassadas   (502) staff       (20)      369 2024-05-24 21:45:46.000000 django_d1db-0.0.6/django_d1db.egg-info/SOURCES.txt
+-rw-r--r--   0 gmassadas   (502) staff       (20)        1 2024-05-24 21:45:46.000000 django_d1db-0.0.6/django_d1db.egg-info/dependency_links.txt
+-rw-r--r--   0 gmassadas   (502) staff       (20)       10 2024-05-24 21:45:46.000000 django_d1db-0.0.6/django_d1db.egg-info/top_level.txt
+-rw-r--r--   0 gmassadas   (502) staff       (20)      785 2024-05-24 21:45:34.000000 django_d1db-0.0.6/pyproject.toml
+-rw-r--r--   0 gmassadas   (502) staff       (20)       38 2024-05-24 21:45:46.601619 django_d1db-0.0.6/setup.cfg
```

### Comparing `django_d1db-0.0.4/LICENSE` & `django_d1db-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_d1db-0.0.4/PKG-INFO` & `django_d1db-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-d1db
-Version: 0.0.4
+Version: 0.0.6
 Summary: Django backend for Cloudflare D1
 Author: Gabriel Massadas
 Project-URL: Bug Reports, https://github.com/G4brym/django-d1/issues
 Project-URL: Source, https://github.com/G4brym/django-d1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
```

### Comparing `django_d1db-0.0.4/README.md` & `django_d1db-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `django_d1db-0.0.4/django_d1/base.py` & `django_d1db-0.0.6/django_d1/base.py`

 * *Files identical despite different names*

### Comparing `django_d1db-0.0.4/django_d1/database.py` & `django_d1db-0.0.6/django_d1/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from urllib import request
 import json
 import http.client
 
 from django.db import DatabaseError, Error, DataError, OperationalError, \
 IntegrityError, InternalError, ProgrammingError, NotSupportedError, InterfaceError
 
 def retry(times, exceptions):
@@ -29,24 +28,28 @@
                     attempt += 1
             return func(*args, **kwargs)
         return newfn
     return decorator
 
 class D1Result:
     lastrowid = None
+    rowcount = -1
 
     def __init__(self, data):
         self.data = data
 
     def __iter__(self):
         return iter(self.data)
 
     def set_lastrowid(self, value):
         self.lastrowid = value
 
+    def set_rowcount(self, value):
+        self.rowcount = value
+
     @staticmethod
     def from_dict(data):
         result = []
 
         for row in data:
             row_items = ()
             for k, v in row.items():
@@ -75,18 +78,25 @@
 
     NotSupportedError = NotSupportedError
     DatabaseError = DatabaseError
     InterfaceError = InterfaceError
     Error = Error
 
     lastrowid = None
+
     def set_lastrowid(self, value):
         self.lastrowid = value
 
+    rowcount = None
+
+    def set_rowcount(self, value):
+        self.rowcount = value
+
     _defer_foreign_keys = False
+
     def defer_foreign_keys(self, state):
         _defer_foreign_keys = state
 
     @staticmethod
     def connect(database_id, account_id, token):
         return D1Database(database_id, account_id, token)
 
@@ -150,17 +160,23 @@
 
         query_result = response["result"][0]
         if query_result["success"] == False:
             raise DatabaseError(query_result)
 
         result = D1Result.from_dict(query_result["results"])
 
-        if query_result["meta"] and query_result["meta"]["last_row_id"]:
-            result.set_lastrowid = query_result["meta"]["last_row_id"]
-            self.set_lastrowid = query_result["meta"]["last_row_id"]
+        meta = query_result.get("meta")
+        if query_result["meta"]:
+            if meta["last_row_id"]:
+                result.set_lastrowid(meta["last_row_id"])
+                self.set_lastrowid(meta["last_row_id"])
+
+            if meta["rows_read"] or meta["rows_written"]:
+                result.set_rowcount(meta.get("rows_read", 0) + meta.get("rows_read", 0))
+                self.set_rowcount(meta.get("rows_read", 0) + meta.get("rows_read", 0))
 
         return result
 
     query = None
     params = None
 
     def execute(self, query, params=None):
```

### Comparing `django_d1db-0.0.4/django_d1/features.py` & `django_d1db-0.0.6/django_d1/features.py`

 * *Files identical despite different names*

### Comparing `django_d1db-0.0.4/django_d1/operations.py` & `django_d1db-0.0.6/django_d1/operations.py`

 * *Files identical despite different names*

### Comparing `django_d1db-0.0.4/django_d1db.egg-info/PKG-INFO` & `django_d1db-0.0.6/django_d1db.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-d1db
-Version: 0.0.4
+Version: 0.0.6
 Summary: Django backend for Cloudflare D1
 Author: Gabriel Massadas
 Project-URL: Bug Reports, https://github.com/G4brym/django-d1/issues
 Project-URL: Source, https://github.com/G4brym/django-d1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
```

### Comparing `django_d1db-0.0.4/pyproject.toml` & `django_d1db-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-d1db"
-version = "0.0.4"
+version = "0.0.6"
 authors = [
   { name="Gabriel Massadas" },
 ]
 description = "Django backend for Cloudflare D1"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

