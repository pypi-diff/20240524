# Comparing `tmp/ensurepath-0.1.0.tar.gz` & `tmp/ensurepath-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensurepath-0.1.0.tar", last modified: Fri May 24 15:58:07 2024, max compression
+gzip compressed data, was "ensurepath-0.2.0.tar", last modified: Fri May 24 17:51:20 2024, max compression
```

## Comparing `ensurepath-0.1.0.tar` & `ensurepath-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 15:58:07.081877 ensurepath-0.1.0/
--rw-r--r--   0 jp        (1000) wheel      (998)     1275 2024-05-24 15:00:16.000000 ensurepath-0.1.0/LICENSE.md
--rw-r--r--   0 jp        (1000) wheel      (998)     3590 2024-05-24 15:58:07.081877 ensurepath-0.1.0/PKG-INFO
--rw-r--r--   0 jp        (1000) wheel      (998)      973 2024-05-24 15:48:48.000000 ensurepath-0.1.0/README.md
-drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 15:58:07.081877 ensurepath-0.1.0/ensurepath.egg-info/
--rw-r--r--   0 jp        (1000) wheel      (998)     3590 2024-05-24 15:58:07.000000 ensurepath-0.1.0/ensurepath.egg-info/PKG-INFO
--rw-r--r--   0 jp        (1000) wheel      (998)      218 2024-05-24 15:58:07.000000 ensurepath-0.1.0/ensurepath.egg-info/SOURCES.txt
--rw-r--r--   0 jp        (1000) wheel      (998)        1 2024-05-24 15:58:07.000000 ensurepath-0.1.0/ensurepath.egg-info/dependency_links.txt
--rw-r--r--   0 jp        (1000) wheel      (998)       20 2024-05-24 15:58:07.000000 ensurepath-0.1.0/ensurepath.egg-info/requires.txt
--rw-r--r--   0 jp        (1000) wheel      (998)       11 2024-05-24 15:58:07.000000 ensurepath-0.1.0/ensurepath.egg-info/top_level.txt
--rw-------   0 jp        (1000) wheel      (998)     1314 2024-05-24 15:50:57.000000 ensurepath-0.1.0/ensurepath.py
--rw-r--r--   0 jp        (1000) wheel      (998)     1232 2024-05-24 15:56:39.000000 ensurepath-0.1.0/pyproject.toml
--rw-r--r--   0 jp        (1000) wheel      (998)       38 2024-05-24 15:58:07.081877 ensurepath-0.1.0/setup.cfg
+drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 17:51:20.010267 ensurepath-0.2.0/
+-rw-r--r--   0 jp        (1000) wheel      (998)     1275 2024-05-24 15:00:16.000000 ensurepath-0.2.0/LICENSE.md
+-rw-r--r--   0 jp        (1000) wheel      (998)     3590 2024-05-24 17:51:20.010267 ensurepath-0.2.0/PKG-INFO
+-rw-r--r--   0 jp        (1000) wheel      (998)      973 2024-05-24 15:48:48.000000 ensurepath-0.2.0/README.md
+drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 17:51:20.010267 ensurepath-0.2.0/ensurepath.egg-info/
+-rw-r--r--   0 jp        (1000) wheel      (998)     3590 2024-05-24 17:51:20.000000 ensurepath-0.2.0/ensurepath.egg-info/PKG-INFO
+-rw-r--r--   0 jp        (1000) wheel      (998)      218 2024-05-24 17:51:20.000000 ensurepath-0.2.0/ensurepath.egg-info/SOURCES.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)        1 2024-05-24 17:51:20.000000 ensurepath-0.2.0/ensurepath.egg-info/dependency_links.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)       20 2024-05-24 17:51:20.000000 ensurepath-0.2.0/ensurepath.egg-info/requires.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)       11 2024-05-24 17:51:20.000000 ensurepath-0.2.0/ensurepath.egg-info/top_level.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)     1318 2024-05-24 17:50:07.000000 ensurepath-0.2.0/ensurepath.py
+-rw-r--r--   0 jp        (1000) wheel      (998)     1232 2024-05-24 17:50:18.000000 ensurepath-0.2.0/pyproject.toml
+-rw-r--r--   0 jp        (1000) wheel      (998)       38 2024-05-24 17:51:20.010267 ensurepath-0.2.0/setup.cfg
```

### Comparing `ensurepath-0.1.0/LICENSE.md` & `ensurepath-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ensurepath-0.1.0/PKG-INFO` & `ensurepath-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensurepath
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ensure python, pip and with pip installed binarys (scripts for win) are in your PATH variable.
 Author: Konxell
 Maintainer: Konxell
 License: Unlicense (Public Domain)
         ============================
         
         This is free and unencumbered software released into the public domain.
```

### Comparing `ensurepath-0.1.0/README.md` & `ensurepath-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ensurepath-0.1.0/ensurepath.egg-info/PKG-INFO` & `ensurepath-0.2.0/ensurepath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensurepath
-Version: 0.1.0
+Version: 0.2.0
 Summary: Ensure python, pip and with pip installed binarys (scripts for win) are in your PATH variable.
 Author: Konxell
 Maintainer: Konxell
 License: Unlicense (Public Domain)
         ============================
         
         This is free and unencumbered software released into the public domain.
```

### Comparing `ensurepath-0.1.0/ensurepath.py` & `ensurepath-0.2.0/ensurepath.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     packages = json.loads(pip_json.stdout)
     locations = set([pkg['location'] for pkg in packages] + [python_path] )
 
     path_added = False
     need_shell_restart = False
 
     for location in locations:
-        for subdir in ['bin', 'Scripts']:
+        for subdir in ['bin', 'Scripts', '']:
             path = os.path.join(os.path.dirname(location), subdir)
             if os.path.isdir(path):
                 if not userpath.in_current_path(path):
                     userpath.append(path)
                     if not path_added:
                         path_added = True
                     print(f"added the following path to your environment variables: {path}")
```

### Comparing `ensurepath-0.1.0/pyproject.toml` & `ensurepath-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ensurepath"
 description = "Ensure python, pip and with pip installed binarys (scripts for win) are in your PATH variable."
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 requires-python = ">=3.7"
 keywords = [
   "path",
   "user path",
   "windows",
   "linux",
   "msstore",
```

