# Comparing `tmp/trame-tauri-0.5.0.tar.gz` & `tmp/trame-tauri-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-tauri-0.5.0.tar", last modified: Tue May 21 21:59:23 2024, max compression
+gzip compressed data, was "trame-tauri-0.5.1.tar", last modified: Fri May 24 21:01:36 2024, max compression
```

## Comparing `trame-tauri-0.5.0.tar` & `trame-tauri-0.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/
--rw-r--r--   0 root         (0) root         (0)      583 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2518 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1736 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      925 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame/modules/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame/widgets/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame_tauri/
--rw-r--r--   0 root         (0) root         (0)       93 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame_tauri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame_tauri/module/
--rw-r--r--   0 root         (0) root         (0)      199 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame_tauri/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame_tauri/module/serve/
--rw-r--r--   0 root         (0) root         (0)    36142 2024-05-21 21:59:20.000000 trame-tauri-0.5.0/trame_tauri/module/serve/trame-tauri.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame_tauri/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame_tauri/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7776 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame_tauri/widgets/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame_tauri.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2518 2024-05-21 21:59:23.000000 trame-tauri-0.5.0/trame_tauri.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-21 21:59:23.000000 trame-tauri-0.5.0/trame_tauri.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 21:59:23.000000 trame-tauri-0.5.0/trame_tauri.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-21 21:59:23.000000 trame-tauri-0.5.0/trame_tauri.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-21 21:59:23.000000 trame-tauri-0.5.0/trame_tauri.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      925 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.110781 trame-tauri-0.5.1/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.110781 trame-tauri-0.5.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame/modules/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame/widgets/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame_tauri/
+-rw-r--r--   0 root         (0) root         (0)       93 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame_tauri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame_tauri/module/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame_tauri/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame_tauri/module/serve/
+-rw-r--r--   0 root         (0) root         (0)    36186 2024-05-24 21:01:32.000000 trame-tauri-0.5.1/trame_tauri/module/serve/trame-tauri.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame_tauri/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame_tauri/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7776 2024-05-24 21:01:12.000000 trame-tauri-0.5.1/trame_tauri/widgets/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 21:01:36.114781 trame-tauri-0.5.1/trame_tauri.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-05-24 21:01:36.000000 trame-tauri-0.5.1/trame_tauri.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-24 21:01:36.000000 trame-tauri-0.5.1/trame_tauri.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 21:01:36.000000 trame-tauri-0.5.1/trame_tauri.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-24 21:01:36.000000 trame-tauri-0.5.1/trame_tauri.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-24 21:01:36.000000 trame-tauri-0.5.1/trame_tauri.egg-info/top_level.txt
```

### Comparing `trame-tauri-0.5.0/LICENSE` & `trame-tauri-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-tauri-0.5.0/PKG-INFO` & `trame-tauri-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-tauri
-Version: 0.5.0
+Version: 0.5.1
 Summary: Helper widget to provide simpler integration with Tauri
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-tauri-0.5.0/README.rst` & `trame-tauri-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-tauri-0.5.0/setup.cfg` & `trame-tauri-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-tauri
-version = 0.5.0
+version = 0.5.1
 description = Helper widget to provide simpler integration with Tauri
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `trame-tauri-0.5.0/trame_tauri/module/serve/trame-tauri.umd.js` & `trame-tauri-0.5.1/trame_tauri/module/serve/trame-tauri.umd.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1334,16 +1334,17 @@
                     };
                 for (let o = 0; o < te.length; o++) {
                     const c = te[o];
                     t[c] > 0 && (ce[c] = Number(t[c]))
                 }
                 const m = t.main ? O : new f(u, ce),
                     _ = [];
-                y.onBeforeUnmount(() => {
-                    for (; _.length;) _.pop()();
+                y.onBeforeUnmount(async () => {
+                    const o = await Promise.all(_);
+                    for (_.length = 0; o.length;) o.pop()();
                     R(), de()
                 }), t.main ? m.scaleFactor().then(o => {
                     s.value = o, m.outerPosition().then(c => {
                         const p = c.toLogical(o);
                         i.value = [p.x, p.y]
                     }), m.outerSize().then(c => {
                         const p = c.toLogical(o);
```

### Comparing `trame-tauri-0.5.0/trame_tauri/widgets/tauri.py` & `trame-tauri-0.5.1/trame_tauri/widgets/tauri.py`

 * *Files identical despite different names*

### Comparing `trame-tauri-0.5.0/trame_tauri.egg-info/PKG-INFO` & `trame-tauri-0.5.1/trame_tauri.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-tauri
-Version: 0.5.0
+Version: 0.5.1
 Summary: Helper widget to provide simpler integration with Tauri
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

