# Comparing `tmp/viur_toolkit-0.1.0.dev8.tar.gz` & `tmp/viur_toolkit-0.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur_toolkit-0.1.0.dev8.tar", last modified: Tue May  7 19:40:53 2024, max compression
+gzip compressed data, was "viur_toolkit-0.1.0.dev9.tar", last modified: Wed May  8 19:47:57 2024, max compression
```

## Comparing `viur_toolkit-0.1.0.dev8.tar` & `viur_toolkit-0.1.0.dev9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:40:53.811251 viur_toolkit-0.1.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 19:40:53.811251 viur_toolkit-0.1.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-07 19:40:53.811251 viur_toolkit-0.1.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:40:53.807252 viur_toolkit-0.1.0.dev8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:40:53.807252 viur_toolkit-0.1.0.dev8/src/viur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:40:53.811251 viur_toolkit-0.1.0.dev8/src/viur/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/memcache.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-07 19:40:49.000000 viur_toolkit-0.1.0.dev8/src/viur/toolkit/viur.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:40:53.811251 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-07 19:40:53.000000 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-07 19:40:53.000000 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:40:53.000000 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 19:40:53.000000 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 19:40:53.000000 viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:47:57.207566 viur_toolkit-0.1.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-08 19:47:57.207566 viur_toolkit-0.1.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-08 19:47:57.207566 viur_toolkit-0.1.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:47:57.203566 viur_toolkit-0.1.0.dev9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:47:57.203566 viur_toolkit-0.1.0.dev9/src/viur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:47:57.207566 viur_toolkit-0.1.0.dev9/src/viur/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/src/viur/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/src/viur/toolkit/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/src/viur/toolkit/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/src/viur/toolkit/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/src/viur/toolkit/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/src/viur/toolkit/memcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/src/viur/toolkit/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/src/viur/toolkit/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/src/viur/toolkit/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/src/viur/toolkit/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-08 19:47:53.000000 viur_toolkit-0.1.0.dev9/src/viur/toolkit/viur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:47:57.207566 viur_toolkit-0.1.0.dev9/src/viur_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-08 19:47:57.000000 viur_toolkit-0.1.0.dev9/src/viur_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-08 19:47:57.000000 viur_toolkit-0.1.0.dev9/src/viur_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:47:57.000000 viur_toolkit-0.1.0.dev9/src/viur_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 19:47:57.000000 viur_toolkit-0.1.0.dev9/src/viur_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 19:47:57.000000 viur_toolkit-0.1.0.dev9/src/viur_toolkit.egg-info/top_level.txt
```

### Comparing `viur_toolkit-0.1.0.dev8/LICENSE` & `viur_toolkit-0.1.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev8/PKG-INFO` & `viur_toolkit-0.1.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-toolkit
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: A kit of helpers and tools to simplify more intensive use of ViUR
 Home-page: https://github.com/viur-framework/viur-toolkit
 Author: Sven Eberth
 Author-email: se@mausbrand.de
 Maintainer: Sven Eberth
 Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev8 Summary: A kit of
+Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev9 Summary: A kit of
 helpers and tools to simplify more intensive use of ViUR Home-page: https://
 github.com/viur-framework/viur-toolkit Author: Sven Eberth Author-email:
 se@mausbrand.de Maintainer: Sven Eberth Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
```

### Comparing `viur_toolkit-0.1.0.dev8/setup.cfg` & `viur_toolkit-0.1.0.dev9/setup.cfg`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev8/src/viur/toolkit/checks.py` & `viur_toolkit-0.1.0.dev9/src/viur/toolkit/checks.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev8/src/viur/toolkit/context.py` & `viur_toolkit-0.1.0.dev9/src/viur/toolkit/context.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev8/src/viur/toolkit/db.py` & `viur_toolkit-0.1.0.dev9/src/viur/toolkit/db.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev8/src/viur/toolkit/decorators.py` & `viur_toolkit-0.1.0.dev9/src/viur/toolkit/decorators.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev8/src/viur/toolkit/memcache.py` & `viur_toolkit-0.1.0.dev9/src/viur/toolkit/memcache.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev8/src/viur/toolkit/property.py` & `viur_toolkit-0.1.0.dev9/src/viur/toolkit/property.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev8/src/viur/toolkit/report.py` & `viur_toolkit-0.1.0.dev9/src/viur/toolkit/report.py`

 * *Files identical despite different names*

### Comparing `viur_toolkit-0.1.0.dev8/src/viur/toolkit/viur.py` & `viur_toolkit-0.1.0.dev9/src/viur/toolkit/viur.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,40 +6,50 @@
 import typing as t
 
 from viur.core import current, db
 from viur.core.skeleton import SkeletonInstance, skeletonByKind
 
 __all__ = [
     "change_language",
+    "get_task_retry_count",
     "without_render_preparation",
     "get_full_skel_from_ref_skel",
     "iter_skel",
 ]
 
 logger = logging.getLogger(__name__)
 
 
 def change_language(lang: str) -> None:
     """Change the current language"""
     current.session.get()["lang"] = lang
     current.language.set(lang)
 
 
+def get_task_retry_count() -> int:
+    """Return the number of times the current task is retried as int"""
+    try:
+        return int(current.request.get().request.headers.get("X-Appengine-Taskretrycount", -1))
+    except AttributeError:
+        # During warmup current.request is None (at least on local devserver)
+        return -1
+
+
 def without_render_preparation(skel: SkeletonInstance) -> SkeletonInstance:
     """Remove clones skel without render preparation if was set else the skel as is"""
     if skel.renderPreparation is not None:
         # TODO: ViUR, I DONT WANT TO HAVE RENDERPREPARATION ON MODULE LAYER!!!
         skel = skel.clone()
         skel.renderPreparation = None
     return skel
 
 
 def get_full_skel_from_ref_skel(ref_skel: SkeletonInstance) -> SkeletonInstance:
     kind_name = ref_skel.skeletonCls.__name__.removeprefix("RefSkelFor")
-    skel: SkeletonInstance = skeletonByKind(kind_name)() # noqa
+    skel: SkeletonInstance = skeletonByKind(kind_name)()  # noqa
     skel.fromDB(ref_skel["key"])
     return skel
 
 
 def iter_skel(query: db.Query) -> t.Iterator[SkeletonInstance]:
     """Fetch all entries for this query and yield the skel
```

### Comparing `viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/PKG-INFO` & `viur_toolkit-0.1.0.dev9/src/viur_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-toolkit
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: A kit of helpers and tools to simplify more intensive use of ViUR
 Home-page: https://github.com/viur-framework/viur-toolkit
 Author: Sven Eberth
 Author-email: se@mausbrand.de
 Maintainer: Sven Eberth
 Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev8 Summary: A kit of
+Metadata-Version: 2.1 Name: viur-toolkit Version: 0.1.0.dev9 Summary: A kit of
 helpers and tools to simplify more intensive use of ViUR Home-page: https://
 github.com/viur-framework/viur-toolkit Author: Sven Eberth Author-email:
 se@mausbrand.de Maintainer: Sven Eberth Maintainer-email: se@mausbrand.de
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
```

### Comparing `viur_toolkit-0.1.0.dev8/src/viur_toolkit.egg-info/SOURCES.txt` & `viur_toolkit-0.1.0.dev9/src/viur_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

