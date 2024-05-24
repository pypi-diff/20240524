# Comparing `tmp/pycrunch-0.5.7.tar.gz` & `tmp/pycrunch-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycrunch-0.5.7.tar", last modified: Mon Feb 27 14:28:34 2023, max compression
+gzip compressed data, was "dist/pycrunch-0.5.8.tar", last modified: Fri May 24 15:45:04 2024, max compression
```

## Comparing `pycrunch-0.5.7.tar` & `pycrunch-0.5.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 jj        (1000) nordvpn    (997)        0 2023-02-27 14:28:34.000000 pycrunch-0.5.7/
--rw-r--r--   0 jj        (1000) nordvpn    (997)      621 2023-02-08 19:10:46.000000 pycrunch-0.5.7/LICENSE
--rw-r--r--   0 jj        (1000) nordvpn    (997)     1717 2023-02-08 19:10:46.000000 pycrunch-0.5.7/setup.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)      353 2023-02-08 19:10:46.000000 pycrunch-0.5.7/Makefile
--rw-r--r--   0 jj        (1000) nordvpn    (997)     5560 2023-02-08 19:10:46.000000 pycrunch-0.5.7/README.md
-drwxr-xr-x   0 jj        (1000) nordvpn    (997)        0 2023-02-27 14:28:34.000000 pycrunch-0.5.7/src/
-drwxr-xr-x   0 jj        (1000) nordvpn    (997)        0 2023-02-27 14:28:34.000000 pycrunch-0.5.7/src/pycrunch/
--rw-r--r--   0 jj        (1000) nordvpn    (997)     2582 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/csvlib.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)      751 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/ipython_ext.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)     1919 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/progress.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)     2951 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/pandaslib.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)     5123 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/cubes.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)     1161 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/exporting.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)    11262 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/__init__.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)    13140 2023-02-27 14:25:46.000000 pycrunch-0.5.7/src/pycrunch/elements.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)     5946 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/importing.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)     6130 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/lemonpy.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)      589 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/variables.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)     2323 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/users.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)    15107 2023-02-08 19:10:46.000000 pycrunch-0.5.7/src/pycrunch/shoji.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)       22 2023-02-27 14:26:45.000000 pycrunch-0.5.7/src/pycrunch/version.py
-drwxr-xr-x   0 jj        (1000) nordvpn    (997)        0 2023-02-27 14:28:34.000000 pycrunch-0.5.7/src/pycrunch.egg-info/
--rwxr-xr-x   0 jj        (1000) nordvpn    (997)      837 2023-02-27 14:28:34.000000 pycrunch-0.5.7/src/pycrunch.egg-info/SOURCES.txt
--rwxr-xr-x   0 jj        (1000) nordvpn    (997)      279 2023-02-27 14:28:34.000000 pycrunch-0.5.7/src/pycrunch.egg-info/requires.txt
--rwxr-xr-x   0 jj        (1000) nordvpn    (997)        1 2023-02-27 14:28:34.000000 pycrunch-0.5.7/src/pycrunch.egg-info/dependency_links.txt
--rwxr-xr-x   0 jj        (1000) nordvpn    (997)     7301 2023-02-27 14:28:34.000000 pycrunch-0.5.7/src/pycrunch.egg-info/PKG-INFO
--rwxr-xr-x   0 jj        (1000) nordvpn    (997)        9 2023-02-27 14:28:34.000000 pycrunch-0.5.7/src/pycrunch.egg-info/top_level.txt
--rwxr-xr-x   0 jj        (1000) nordvpn    (997)        1 2018-03-06 20:31:34.000000 pycrunch-0.5.7/src/pycrunch.egg-info/zip-safe
--rw-r--r--   0 jj        (1000) nordvpn    (997)     7652 2023-02-08 19:10:46.000000 pycrunch-0.5.7/COPYING.LESSER
--rw-r--r--   0 jj        (1000) nordvpn    (997)    35148 2023-02-08 19:10:46.000000 pycrunch-0.5.7/COPYING
-drwxr-xr-x   0 jj        (1000) nordvpn    (997)        0 2023-02-27 14:28:34.000000 pycrunch-0.5.7/.github/
-drwxr-xr-x   0 jj        (1000) nordvpn    (997)        0 2023-02-27 14:28:34.000000 pycrunch-0.5.7/.github/workflows/
--rw-r--r--   0 jj        (1000) nordvpn    (997)     1355 2023-02-08 19:10:46.000000 pycrunch-0.5.7/.github/workflows/build-and-test.yaml
--rw-r--r--   0 jj        (1000) nordvpn    (997)      159 2023-02-08 19:10:46.000000 pycrunch-0.5.7/.coveragerc
--rw-r--r--   0 jj        (1000) nordvpn    (997)     7301 2023-02-27 14:28:34.000000 pycrunch-0.5.7/PKG-INFO
-drwxr-xr-x   0 jj        (1000) nordvpn    (997)        0 2023-02-27 14:28:34.000000 pycrunch-0.5.7/tests/
--rw-r--r--   0 jj        (1000) nordvpn    (997)     1006 2023-02-08 19:10:46.000000 pycrunch-0.5.7/tests/test_csvlib.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)     6014 2023-02-08 19:10:46.000000 pycrunch-0.5.7/tests/test_http.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)    10540 2023-02-08 19:10:46.000000 pycrunch-0.5.7/tests/test_elements.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)        0 2023-02-08 19:10:46.000000 pycrunch-0.5.7/tests/__init__.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)    14589 2023-02-08 19:10:46.000000 pycrunch-0.5.7/tests/test_shoji.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)     2278 2023-02-08 19:10:46.000000 pycrunch-0.5.7/tests/test_cube.py
--rw-r--r--   0 jj        (1000) nordvpn    (997)      121 2023-02-08 19:10:46.000000 pycrunch-0.5.7/RELEASING.txt
--rw-r--r--   0 jj        (1000) nordvpn    (997)      168 2023-02-08 19:10:46.000000 pycrunch-0.5.7/MANIFEST.in
--rw-r--r--   0 jj        (1000) nordvpn    (997)      474 2023-02-27 14:28:34.000000 pycrunch-0.5.7/setup.cfg
--rw-r--r--   0 jj        (1000) nordvpn    (997)      422 2023-02-08 19:10:46.000000 pycrunch-0.5.7/.gitignore
--rw-r--r--   0 jj        (1000) nordvpn    (997)      955 2023-02-08 19:10:46.000000 pycrunch-0.5.7/tox.ini
+drwxr-xr-x   0 jj        (1000) jj        (1000)        0 2024-05-24 15:45:04.000000 pycrunch-0.5.8/
+-rw-r--r--   0 jj        (1000) jj        (1000)      621 2023-02-08 19:10:46.000000 pycrunch-0.5.8/LICENSE
+-rw-r--r--   0 jj        (1000) jj        (1000)     1717 2023-02-08 19:10:46.000000 pycrunch-0.5.8/setup.py
+-rw-r--r--   0 jj        (1000) jj        (1000)      353 2023-02-08 19:10:46.000000 pycrunch-0.5.8/Makefile
+-rw-r--r--   0 jj        (1000) jj        (1000)     5560 2023-02-08 19:10:46.000000 pycrunch-0.5.8/README.md
+drwxr-xr-x   0 jj        (1000) jj        (1000)        0 2024-05-24 15:45:04.000000 pycrunch-0.5.8/src/
+drwxr-xr-x   0 jj        (1000) jj        (1000)        0 2024-05-24 15:45:04.000000 pycrunch-0.5.8/src/pycrunch/
+-rw-r--r--   0 jj        (1000) jj        (1000)     2582 2023-02-08 19:10:46.000000 pycrunch-0.5.8/src/pycrunch/csvlib.py
+-rw-r--r--   0 jj        (1000) jj        (1000)      751 2023-02-08 19:10:46.000000 pycrunch-0.5.8/src/pycrunch/ipython_ext.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     1919 2023-02-08 19:10:46.000000 pycrunch-0.5.8/src/pycrunch/progress.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     2951 2023-02-08 19:10:46.000000 pycrunch-0.5.8/src/pycrunch/pandaslib.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     5123 2023-02-08 19:10:46.000000 pycrunch-0.5.8/src/pycrunch/cubes.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     1161 2023-02-08 19:10:46.000000 pycrunch-0.5.8/src/pycrunch/exporting.py
+-rw-r--r--   0 jj        (1000) jj        (1000)    11309 2024-05-24 15:25:26.000000 pycrunch-0.5.8/src/pycrunch/__init__.py
+-rw-r--r--   0 jj        (1000) jj        (1000)    13885 2024-05-24 15:25:26.000000 pycrunch-0.5.8/src/pycrunch/elements.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     5968 2024-05-24 15:25:26.000000 pycrunch-0.5.8/src/pycrunch/importing.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     6130 2023-02-08 19:10:46.000000 pycrunch-0.5.8/src/pycrunch/lemonpy.py
+-rw-r--r--   0 jj        (1000) jj        (1000)      589 2023-02-08 19:10:46.000000 pycrunch-0.5.8/src/pycrunch/variables.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     2323 2023-02-08 19:10:46.000000 pycrunch-0.5.8/src/pycrunch/users.py
+-rw-r--r--   0 jj        (1000) jj        (1000)    15107 2024-05-06 21:28:44.000000 pycrunch-0.5.8/src/pycrunch/shoji.py
+-rw-r--r--   0 jj        (1000) jj        (1000)       22 2024-05-24 15:25:26.000000 pycrunch-0.5.8/src/pycrunch/version.py
+drwxr-xr-x   0 jj        (1000) jj        (1000)        0 2024-05-24 15:45:04.000000 pycrunch-0.5.8/src/pycrunch.egg-info/
+-rwxr-xr-x   0 jj        (1000) jj        (1000)      837 2024-05-24 15:45:04.000000 pycrunch-0.5.8/src/pycrunch.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jj        (1000) jj        (1000)      279 2024-05-24 15:45:04.000000 pycrunch-0.5.8/src/pycrunch.egg-info/requires.txt
+-rwxr-xr-x   0 jj        (1000) jj        (1000)        1 2024-05-24 15:45:04.000000 pycrunch-0.5.8/src/pycrunch.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jj        (1000) jj        (1000)     7301 2024-05-24 15:45:04.000000 pycrunch-0.5.8/src/pycrunch.egg-info/PKG-INFO
+-rwxr-xr-x   0 jj        (1000) jj        (1000)        9 2024-05-24 15:45:04.000000 pycrunch-0.5.8/src/pycrunch.egg-info/top_level.txt
+-rwxr-xr-x   0 jj        (1000) jj        (1000)        1 2018-03-06 20:31:34.000000 pycrunch-0.5.8/src/pycrunch.egg-info/zip-safe
+-rw-r--r--   0 jj        (1000) jj        (1000)     7652 2023-02-08 19:10:46.000000 pycrunch-0.5.8/COPYING.LESSER
+-rw-r--r--   0 jj        (1000) jj        (1000)    35148 2023-02-08 19:10:46.000000 pycrunch-0.5.8/COPYING
+drwxr-xr-x   0 jj        (1000) jj        (1000)        0 2024-05-24 15:45:04.000000 pycrunch-0.5.8/.github/
+drwxr-xr-x   0 jj        (1000) jj        (1000)        0 2024-05-24 15:45:04.000000 pycrunch-0.5.8/.github/workflows/
+-rw-r--r--   0 jj        (1000) jj        (1000)     1380 2024-05-24 15:25:26.000000 pycrunch-0.5.8/.github/workflows/build-and-test.yaml
+-rw-r--r--   0 jj        (1000) jj        (1000)      159 2023-02-08 19:10:46.000000 pycrunch-0.5.8/.coveragerc
+-rw-r--r--   0 jj        (1000) jj        (1000)     7301 2024-05-24 15:45:04.000000 pycrunch-0.5.8/PKG-INFO
+drwxr-xr-x   0 jj        (1000) jj        (1000)        0 2024-05-24 15:45:04.000000 pycrunch-0.5.8/tests/
+-rw-r--r--   0 jj        (1000) jj        (1000)     1006 2023-02-08 19:10:46.000000 pycrunch-0.5.8/tests/test_csvlib.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     6014 2023-02-08 19:10:46.000000 pycrunch-0.5.8/tests/test_http.py
+-rw-r--r--   0 jj        (1000) jj        (1000)    10540 2023-02-08 19:10:46.000000 pycrunch-0.5.8/tests/test_elements.py
+-rw-r--r--   0 jj        (1000) jj        (1000)        0 2023-02-08 19:10:46.000000 pycrunch-0.5.8/tests/__init__.py
+-rw-r--r--   0 jj        (1000) jj        (1000)    14589 2023-02-08 19:10:46.000000 pycrunch-0.5.8/tests/test_shoji.py
+-rw-r--r--   0 jj        (1000) jj        (1000)     2278 2023-02-08 19:10:46.000000 pycrunch-0.5.8/tests/test_cube.py
+-rw-r--r--   0 jj        (1000) jj        (1000)      121 2023-02-08 19:10:46.000000 pycrunch-0.5.8/RELEASING.txt
+-rw-r--r--   0 jj        (1000) jj        (1000)      168 2023-02-08 19:10:46.000000 pycrunch-0.5.8/MANIFEST.in
+-rw-r--r--   0 jj        (1000) jj        (1000)      474 2024-05-24 15:45:04.000000 pycrunch-0.5.8/setup.cfg
+-rw-r--r--   0 jj        (1000) jj        (1000)      427 2024-05-24 15:25:26.000000 pycrunch-0.5.8/.gitignore
+-rw-r--r--   0 jj        (1000) jj        (1000)      955 2023-02-08 19:10:46.000000 pycrunch-0.5.8/tox.ini
```

### Comparing `pycrunch-0.5.7/LICENSE` & `pycrunch-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/setup.py` & `pycrunch-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/README.md` & `pycrunch-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch/csvlib.py` & `pycrunch-0.5.8/src/pycrunch/csvlib.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch/ipython_ext.py` & `pycrunch-0.5.8/src/pycrunch/ipython_ext.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch/progress.py` & `pycrunch-0.5.8/src/pycrunch/progress.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch/pandaslib.py` & `pycrunch-0.5.8/src/pycrunch/pandaslib.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch/cubes.py` & `pycrunch-0.5.8/src/pycrunch/cubes.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch/exporting.py` & `pycrunch-0.5.8/src/pycrunch/exporting.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch/__init__.py` & `pycrunch-0.5.8/src/pycrunch/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -191,14 +191,16 @@
 from pycrunch.shoji import TaskError, TaskProgressTimeoutError
 from pycrunch import importing
 from pycrunch.lemonpy import ClientError, ServerError, urljoin
 from pycrunch.version import __version__
 
 Session = elements.ElementSession
 
+UnsafeSession = elements.UnsafeElementSession
+
 __all__ = [
     'cubes',
     'elements',
     'shoji',
     'TaskError', 'TaskProgressTimeoutError',
     'importing',
     'ClientError', 'ServerError', 'CrunchError',
```

### Comparing `pycrunch-0.5.7/src/pycrunch/elements.py` & `pycrunch-0.5.8/src/pycrunch/elements.py`

 * *Files 3% similar despite different names*

```diff
@@ -356,7 +356,37 @@
 
     @property
     def password(self):
         warnings.warn(
             "`session.password` is being deprecated.", PendingDeprecationWarning
         )
         return self.__password
+
+
+class UnsafeElementSession(ElementSession):
+    """
+    A subclass of ElementSession that disables SSL/TLS verification.
+    This is mean to be used for development purposes only.
+    """
+
+    def __init__(
+        self,
+        email=None,
+        password=None,
+        token=None,
+        site_url=None,
+        progress_tracking=None,
+    ):
+        super(UnsafeElementSession, self).__init__(
+            email,
+            password,
+            token,
+            site_url,
+            progress_tracking,
+        )
+
+        # Skip SSL/TLS verification
+        self.verify = False
+
+        if self.token:
+            # Use Bearer token for authentication
+            self.headers.update({"Authorization": "Bearer {}".format(self.token)})
```

### Comparing `pycrunch-0.5.7/src/pycrunch/importing.py` & `pycrunch-0.5.8/src/pycrunch/importing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import mimetypes
 import os
 import time
 
 import six
 
-from pycrunch import shoji, csvlib
+from pycrunch import csvlib, shoji
 
 
 class Importer(object):
     """A class for collecting the various ways to import data into Crunch.
 
     If the 'strict' argument is omitted or None, then any given CSV file
     is expected to conform to any previous metadata provided; that is,
@@ -49,21 +49,21 @@
                     self.frequency *= self.backoff_rate
                     if self.frequency > self.backoff_max:
                         self.frequency = self.backoff_max
         else:
             raise ValueError("The batch did not reach the '%s' state in the "
                              "given time. Please check again later." % status)
 
-    def add_source(self, ds, filename, fp, mimetype):
+    def add_source(self, ds, filename, fp, mimetype, data=None):
         """Create a new Source on the given dataset and return its URL."""
         sources_url = ds.user_url.catalogs['sources']
         # Don't call Catalog.post here (which would force application/json);
         # we want requests.Session to set multipart/form-data with a boundary.
         new_source_url = ds.session.post(
-            sources_url, files={"uploaded_file": (filename, fp, mimetype)}
+            sources_url, files={"uploaded_file": (filename, fp, mimetype)}, data=data
         ).headers["Location"]
 
         if self.strict is not None:
             r = ds.session.get(new_source_url)
             if r.payload is None:
                 raise TypeError("Response could not be parsed.", r)
             source = r.payload
```

### Comparing `pycrunch-0.5.7/src/pycrunch/lemonpy.py` & `pycrunch-0.5.8/src/pycrunch/lemonpy.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch/variables.py` & `pycrunch-0.5.8/src/pycrunch/variables.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch/users.py` & `pycrunch-0.5.8/src/pycrunch/users.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch/shoji.py` & `pycrunch-0.5.8/src/pycrunch/shoji.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch.egg-info/SOURCES.txt` & `pycrunch-0.5.8/src/pycrunch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/src/pycrunch.egg-info/PKG-INFO` & `pycrunch-0.5.8/src/pycrunch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrunch
-Version: 0.5.7
+Version: 0.5.8
 Summary: Crunch.io Client Library
 Home-page: https://github.com/Crunch-io/pycrunch
 Author: Crunch.io
 Author-email: dev@crunch.io
 License: LGPL
 Description: pycrunch
         ========
```

### Comparing `pycrunch-0.5.7/COPYING.LESSER` & `pycrunch-0.5.8/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/COPYING` & `pycrunch-0.5.8/COPYING`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/.github/workflows/build-and-test.yaml` & `pycrunch-0.5.8/.github/workflows/build-and-test.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -8,31 +8,32 @@
   pull_request:
     branches:
       - main
       - master
 
 jobs:
   test:
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-20.04
     strategy:
       max-parallel: 4
       matrix:
         python-version:
           - 2.7
-          - 3.5
           - 3.6
           - 3.7
           - 3.8
           - 3.9
     steps:
     - uses: actions/checkout@v1
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      if: matrix.python-version != '2.7'
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
+
     - name: Install dependencies
       run: |
         pip install --upgrade pip
         pip install tox tox-gh-actions
 
     - name: Test with tox ${{env.TOXENV}}
       if: matrix.python-version == '3.6'
```

### Comparing `pycrunch-0.5.7/PKG-INFO` & `pycrunch-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrunch
-Version: 0.5.7
+Version: 0.5.8
 Summary: Crunch.io Client Library
 Home-page: https://github.com/Crunch-io/pycrunch
 Author: Crunch.io
 Author-email: dev@crunch.io
 License: LGPL
 Description: pycrunch
         ========
```

### Comparing `pycrunch-0.5.7/tests/test_csvlib.py` & `pycrunch-0.5.8/tests/test_csvlib.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/tests/test_http.py` & `pycrunch-0.5.8/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/tests/test_elements.py` & `pycrunch-0.5.8/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/tests/test_shoji.py` & `pycrunch-0.5.8/tests/test_shoji.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/tests/test_cube.py` & `pycrunch-0.5.8/tests/test_cube.py`

 * *Files identical despite different names*

### Comparing `pycrunch-0.5.7/tox.ini` & `pycrunch-0.5.8/tox.ini`

 * *Files identical despite different names*

