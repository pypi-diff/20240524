# Comparing `tmp/pelicanfs-0.0.3.tar.gz` & `tmp/pelicanfs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelicanfs-0.0.3.tar", last modified: Wed May  1 00:28:07 2024, max compression
+gzip compressed data, was "pelicanfs-1.0.0.tar", last modified: Fri May 24 03:01:28 2024, max compression
```

## Comparing `pelicanfs-0.0.3.tar` & `pelicanfs-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:28:07.496639 pelicanfs-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 00:28:03.000000 pelicanfs-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-01 00:28:07.496639 pelicanfs-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-01 00:28:03.000000 pelicanfs-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-01 00:28:03.000000 pelicanfs-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-01 00:28:07.496639 pelicanfs-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-01 00:28:03.000000 pelicanfs-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:28:07.492639 pelicanfs-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:28:07.496639 pelicanfs-0.0.3/src/pelicanfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:28:03.000000 pelicanfs-0.0.3/src/pelicanfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-05-01 00:28:03.000000 pelicanfs-0.0.3/src/pelicanfs/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-01 00:28:03.000000 pelicanfs-0.0.3/src/pelicanfs/dir_header_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:28:07.496639 pelicanfs-0.0.3/src/pelicanfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-01 00:28:07.000000 pelicanfs-0.0.3/src/pelicanfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-01 00:28:07.000000 pelicanfs-0.0.3/src/pelicanfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:28:07.000000 pelicanfs-0.0.3/src/pelicanfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 00:28:07.000000 pelicanfs-0.0.3/src/pelicanfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 00:28:07.000000 pelicanfs-0.0.3/src/pelicanfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:01:28.320799 pelicanfs-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 03:01:24.000000 pelicanfs-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-24 03:01:28.320799 pelicanfs-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-24 03:01:24.000000 pelicanfs-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-24 03:01:24.000000 pelicanfs-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-24 03:01:28.320799 pelicanfs-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-24 03:01:24.000000 pelicanfs-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:01:28.316799 pelicanfs-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:01:28.316799 pelicanfs-1.0.0/src/pelicanfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:01:24.000000 pelicanfs-1.0.0/src/pelicanfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25803 2024-05-24 03:01:24.000000 pelicanfs-1.0.0/src/pelicanfs/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-24 03:01:24.000000 pelicanfs-1.0.0/src/pelicanfs/dir_header_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:01:28.320799 pelicanfs-1.0.0/src/pelicanfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-24 03:01:28.000000 pelicanfs-1.0.0/src/pelicanfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-24 03:01:28.000000 pelicanfs-1.0.0/src/pelicanfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:01:28.000000 pelicanfs-1.0.0/src/pelicanfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-24 03:01:28.000000 pelicanfs-1.0.0/src/pelicanfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-24 03:01:28.000000 pelicanfs-1.0.0/src/pelicanfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 03:01:28.000000 pelicanfs-1.0.0/src/pelicanfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:01:28.320799 pelicanfs-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    21651 2024-05-24 03:01:24.000000 pelicanfs-1.0.0/test/test_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-24 03:01:24.000000 pelicanfs-1.0.0/test/test_osdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-24 03:01:24.000000 pelicanfs-1.0.0/test/test_utils.py
```

### Comparing `pelicanfs-0.0.3/LICENSE` & `pelicanfs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pelicanfs-0.0.3/PKG-INFO` & `pelicanfs-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-Metadata-Version: 2.1
-Name: pelicanfs
-Version: 0.0.3
-Summary: An FSSpec Implementation using the Pelican System
-Home-page: https://github.com/PelicanPlatform/pelicanfs
-Project-URL: Source, https://github.com/PelicanPlatform/pelicanfs
-Project-URL: Pelican Source, https://github.com/PelicanPlatform/pelican
-Project-URL: Bug Reports, https://github.com/PelicanPlatform/pelicanfs/issues
-Keywords: pelican,fsspec
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp==3.9.4
-Requires-Dist: aiosignal==1.3.1
-Requires-Dist: async-timeout==4.0.3
-Requires-Dist: attrs==23.2.0
-Requires-Dist: frozenlist==1.4.1
-Requires-Dist: fsspec==2024.3.1
-Requires-Dist: idna==3.7
-Requires-Dist: multidict==6.0.5
-Requires-Dist: yarl==1.9.4
-
 # PelicanFS
 
 ## Overview
 
 PelicanFS is a file system interface (fsspec) for the Pelican Platform.  For more information about pelican, see our [main website](https://pelicanplatform.org) or [Github page](https://github.com/PelicanPlatform/pelican). For more information about fsspec, visit the [filesystem-spec](https://filesystem-spec.readthedocs.io/en/latest/index.html) page.
 
 
@@ -55,34 +24,68 @@
 cd pelicanfs
 pip install -e .
 ```
 
 
 ### Using PelicanFS
 
-To use pelicanfs, first create a `PelicanFileSystem` and provide it with the url for the director of your data federation. As an example using the OSDF director
+To use pelicanfs, first create a `PelicanFileSystem` and provide it with the pelican federation url. As an example using the OSDF federation
 
 ```python
 from pelicanfs.core import PelicanFileSystem
 
-pelfs = PelicanFileSystem("https://osdf-director.osg-htc.org/")
+pelfs = PelicanFileSystem("pelican://osg-htc.org")
 ```
 
 Once `pelfs` is pointed at your federation's director, fsspec commands can be applied to Pelican namespaces. For example:
 
 ```python
 hello_world = pelfs.cat('/ospool/uc-shared/public/OSG-Staff/validation/test.txt')
 print(hello_world)
 ```
 
 ### Getting an FSMap
 
-Sometimes various systems that interact with an fsspec want a key-value mapper rather than a url. To do that, call the `PelicanMap` function with the namespace path and a `PelicanFileSystem` object rather than using the fsspec `get_mapper` call. For example
+Sometimes various systems that interact with an fsspec want a key-value mapper rather than a url. To do that, call the `PelicanMap` function with the namespace path and a `PelicanFileSystem` object rather than using the fsspec `get_mapper` call. For example:
 
 ```python
 from pelicanfs.core import PelicanFileSystem, PelicanMap
 
 pelfs = PelicanFileSystem(“some-director-url”)
 file1 = PelicanMap(“/namespace/file/1”, pelfs=pelfs)
 file2 = PelicanMap(“/namespace/file/2”, pelfs=pelfs)
 ds = xarray.open_mfdataset([file1,file2], engine='zarr')
 ```
+
+### Specifying Endpoints
+
+The following describes how to specify endpoints to get data from, rather than letting PelicanFS and the director determine the best cache. PelicanFS allows you to specify whether to read directly from the origin (bypassing data staging altogether) or to name a specific cache to stage data into. 
+
+**Note**
+> If both direct reads and a specific cache are set, PelicanFS will use the specified cache and ignore the direct reads setting.
+
+
+#### Enabling Direct Reads
+
+Sometimes you might wish to read data directly from an origin rather than via a cache. To enable this at PelicanFileSystem creation, just pass in `direct_reads=True` to the constructor.
+
+```python
+pelfs = PelicanFileSystem("pelican://osg-htc.org", direct_reads=True)
+```
+
+#### Specifying a Cache
+
+If you want to specify a specific cache to stage your data into (as opposed to the highest priority working cache), this can be done by passing in a cache URL during PelicanFileSystem construction via the `preferred_caches` variable:
+
+```python
+pelfs = PelicanFileSystem("pelican://osg-htc.org", preferred_caches=["https://cache.example.com"])
+```
+
+or
+
+```python
+pelfs = PelicanFileSystem("pelican://osg-htc.org", preferred_caches=["https://cache.example.com",
+    "https://cache2.example.com", "+"])
+```
+
+Note that the special cache value `"+"` indicates that the provided preferred caches should be prepended to the
+list of caches from the director.
```

### Comparing `pelicanfs-0.0.3/src/pelicanfs/dir_header_parser.py` & `pelicanfs-1.0.0/src/pelicanfs/dir_header_parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
-def parse_metalink(headers={}):
+def parse_metalink(headers: dict[str, str]) -> tuple[list[tuple[str, int]], str]:
     """
     Parse the metalink headers to get a list of caches to attempt to try in priority orider
     """
-    linkPrio = []
+    linkPrio: list[tuple[str, int]] = []
 
     if "Link" in headers:
         links = headers["Link"].split(",")
         for mlink in links:
             elmts = mlink.split(";")
             mdict = {}
             for elm in elmts[1:]:
@@ -17,27 +17,23 @@
             priority = len(headers)
             if mdict["pri"]:
                 priority = int(mdict["pri"])
             
             link = elmts[0].strip(" <>")
 
             linkPrio.append([link, priority])
-
     linkPrio.sort(key=lambda x: x[1])
-    return linkPrio
 
-def get_dirlist_loc(headers={}):
-    """
-    Parse the headers to get the dirlist location
+    # Pull out the namespace information; we'll use this to populate
+    # the namespace prefix cache later
+    namespace = ""
+    for info in headers.get("X-Pelican-Namespace", "").split(","):
+        info = info.strip()
+        pair = info.split("=", 1)
+        if len(pair) < 2:
+            continue
+        key, val = pair
+        if key == "namespace":
+            namespace = val
+            break
 
-    This will None if there is no dirlist location
-    """
-    if "X-Pelican-Namespace" in headers:
-        namespace = headers["X-Pelican-Namespace"]
-        elmts = namespace.split(", ")
-        for elm in elmts:
-            left, right = elm.split("=", 1)
-            if left == "collections-url":
-                return right
-        
-    
-    return None
+    return linkPrio, namespace
```

