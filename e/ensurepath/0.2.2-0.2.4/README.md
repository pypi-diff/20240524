# Comparing `tmp/ensurepath-0.2.2.tar.gz` & `tmp/ensurepath-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensurepath-0.2.2.tar", last modified: Fri May 24 18:21:26 2024, max compression
+gzip compressed data, was "ensurepath-0.2.4.tar", last modified: Fri May 24 19:08:31 2024, max compression
```

## Comparing `ensurepath-0.2.2.tar` & `ensurepath-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 18:21:26.467859 ensurepath-0.2.2/
--rw-r--r--   0 jp        (1000) wheel      (998)     1275 2024-05-24 15:00:16.000000 ensurepath-0.2.2/LICENSE.md
--rw-r--r--   0 jp        (1000) wheel      (998)     4013 2024-05-24 18:21:26.467859 ensurepath-0.2.2/PKG-INFO
--rw-r--r--   0 jp        (1000) wheel      (998)     1396 2024-05-24 18:20:06.000000 ensurepath-0.2.2/README.md
-drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 18:21:26.467859 ensurepath-0.2.2/ensurepath.egg-info/
--rw-r--r--   0 jp        (1000) wheel      (998)     4013 2024-05-24 18:21:26.000000 ensurepath-0.2.2/ensurepath.egg-info/PKG-INFO
--rw-r--r--   0 jp        (1000) wheel      (998)      218 2024-05-24 18:21:26.000000 ensurepath-0.2.2/ensurepath.egg-info/SOURCES.txt
--rw-r--r--   0 jp        (1000) wheel      (998)        1 2024-05-24 18:21:26.000000 ensurepath-0.2.2/ensurepath.egg-info/dependency_links.txt
--rw-r--r--   0 jp        (1000) wheel      (998)       20 2024-05-24 18:21:26.000000 ensurepath-0.2.2/ensurepath.egg-info/requires.txt
--rw-r--r--   0 jp        (1000) wheel      (998)       11 2024-05-24 18:21:26.000000 ensurepath-0.2.2/ensurepath.egg-info/top_level.txt
--rw-r--r--   0 jp        (1000) wheel      (998)     1318 2024-05-24 17:50:07.000000 ensurepath-0.2.2/ensurepath.py
--rw-r--r--   0 jp        (1000) wheel      (998)     1232 2024-05-24 18:20:17.000000 ensurepath-0.2.2/pyproject.toml
--rw-r--r--   0 jp        (1000) wheel      (998)       38 2024-05-24 18:21:26.467859 ensurepath-0.2.2/setup.cfg
+drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 19:08:31.203070 ensurepath-0.2.4/
+-rw-r--r--   0 jp        (1000) wheel      (998)     1275 2024-05-24 15:00:16.000000 ensurepath-0.2.4/LICENSE.md
+-rw-r--r--   0 jp        (1000) wheel      (998)     4013 2024-05-24 19:08:31.199737 ensurepath-0.2.4/PKG-INFO
+-rw-r--r--   0 jp        (1000) wheel      (998)     1396 2024-05-24 18:20:06.000000 ensurepath-0.2.4/README.md
+drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 19:08:31.199737 ensurepath-0.2.4/ensurepath.egg-info/
+-rw-r--r--   0 jp        (1000) wheel      (998)     4013 2024-05-24 19:08:31.000000 ensurepath-0.2.4/ensurepath.egg-info/PKG-INFO
+-rw-r--r--   0 jp        (1000) wheel      (998)      218 2024-05-24 19:08:31.000000 ensurepath-0.2.4/ensurepath.egg-info/SOURCES.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)        1 2024-05-24 19:08:31.000000 ensurepath-0.2.4/ensurepath.egg-info/dependency_links.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)       20 2024-05-24 19:08:31.000000 ensurepath-0.2.4/ensurepath.egg-info/requires.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)       11 2024-05-24 19:08:31.000000 ensurepath-0.2.4/ensurepath.egg-info/top_level.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)     1572 2024-05-24 18:55:06.000000 ensurepath-0.2.4/ensurepath.py
+-rw-r--r--   0 jp        (1000) wheel      (998)     1232 2024-05-24 19:07:18.000000 ensurepath-0.2.4/pyproject.toml
+-rw-r--r--   0 jp        (1000) wheel      (998)       38 2024-05-24 19:08:31.203070 ensurepath-0.2.4/setup.cfg
```

### Comparing `ensurepath-0.2.2/LICENSE.md` & `ensurepath-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ensurepath-0.2.2/PKG-INFO` & `ensurepath-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensurepath
-Version: 0.2.2
+Version: 0.2.4
 Summary: Ensure python, pip and with pip installed binarys (scripts for win) are in your PATH variable.
 Author: Konxell
 Maintainer: Konxell
 License: Unlicense (Public Domain)
         ============================
         
         This is free and unencumbered software released into the public domain.
```

### Comparing `ensurepath-0.2.2/README.md` & `ensurepath-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ensurepath-0.2.2/ensurepath.egg-info/PKG-INFO` & `ensurepath-0.2.4/ensurepath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensurepath
-Version: 0.2.2
+Version: 0.2.4
 Summary: Ensure python, pip and with pip installed binarys (scripts for win) are in your PATH variable.
 Author: Konxell
 Maintainer: Konxell
 License: Unlicense (Public Domain)
         ============================
         
         This is free and unencumbered software released into the public domain.
```

### Comparing `ensurepath-0.2.2/ensurepath.py` & `ensurepath-0.2.4/ensurepath.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,37 +2,43 @@
 import sys
 import subprocess
 import sys
 import json
 import userpath
 
 def ensurepath():
+    # get all installed packages as json and parse them
     pip_json = subprocess.run([sys.executable, "-m", "pip", "list", '-v', '--format', 'json'], stdout=subprocess.PIPE)
+    packages = json.loads(pip_json.stdout)
 
+    # get python binary directory path
     python_path = os.path.dirname(os.path.realpath(sys.executable))
 
-    packages = json.loads(pip_json.stdout)
-    locations = set([pkg['location'] for pkg in packages] + [python_path] )
+    locations = set()
+    locations.add(python_path)
+    for pkg in packages:
+        for subdir in ['bin','Scripts']:
+            # add possible binary containing folders to locations
+            locations.add(os.path.join(os.path.dirname(pkg['location']), subdir))
 
     path_added = False
     need_shell_restart = False
 
     for location in locations:
-        for subdir in ['bin', 'Scripts', '']:
-            path = os.path.join(os.path.dirname(location), subdir)
-            if os.path.isdir(path):
-                if not userpath.in_current_path(path):
-                    userpath.append(path)
-                    if not path_added:
-                        path_added = True
-                    print(f"added the following path to your environment variables: {path}")
-                    need_shell_restart = need_shell_restart or userpath.need_shell_restart(path)
+        # if location is directory and not in PATH add it to the PATH
+        if os.path.isdir(location):
+            if not userpath.in_current_path(location):
+                userpath.append(location)
+                if not path_added:
+                    path_added = True
+                print(f"Succes! Added the following path to your PATH environment variables:\n {path}")
+                need_shell_restart = need_shell_restart or userpath.need_shell_restart(location)
 
     if need_shell_restart:
-        print("Please now restart your shell or terminal")
+        print("\nPlease now restart your shell or terminal")
 
     if not path_added:
         print("It seems like there was nothing todo, here (that is probably a good thing)!")
     return path_added
 
 if __name__ == "__main__":
     ensurepath()
```

### Comparing `ensurepath-0.2.2/pyproject.toml` & `ensurepath-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ensurepath"
 description = "Ensure python, pip and with pip installed binarys (scripts for win) are in your PATH variable."
 readme = "README.md"
-version = "0.2.2"
+version = "0.2.4"
 requires-python = ">=3.7"
 keywords = [
   "path",
   "user path",
   "windows",
   "linux",
   "msstore",
```

