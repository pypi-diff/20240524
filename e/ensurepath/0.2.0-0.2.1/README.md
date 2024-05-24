# Comparing `tmp/ensurepath-0.2.0.tar.gz` & `tmp/ensurepath-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensurepath-0.2.0.tar", last modified: Fri May 24 17:51:20 2024, max compression
+gzip compressed data, was "ensurepath-0.2.1.tar", last modified: Fri May 24 18:18:13 2024, max compression
```

## Comparing `ensurepath-0.2.0.tar` & `ensurepath-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 17:51:20.010267 ensurepath-0.2.0/
--rw-r--r--   0 jp        (1000) wheel      (998)     1275 2024-05-24 15:00:16.000000 ensurepath-0.2.0/LICENSE.md
--rw-r--r--   0 jp        (1000) wheel      (998)     3590 2024-05-24 17:51:20.010267 ensurepath-0.2.0/PKG-INFO
--rw-r--r--   0 jp        (1000) wheel      (998)      973 2024-05-24 15:48:48.000000 ensurepath-0.2.0/README.md
-drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 17:51:20.010267 ensurepath-0.2.0/ensurepath.egg-info/
--rw-r--r--   0 jp        (1000) wheel      (998)     3590 2024-05-24 17:51:20.000000 ensurepath-0.2.0/ensurepath.egg-info/PKG-INFO
--rw-r--r--   0 jp        (1000) wheel      (998)      218 2024-05-24 17:51:20.000000 ensurepath-0.2.0/ensurepath.egg-info/SOURCES.txt
--rw-r--r--   0 jp        (1000) wheel      (998)        1 2024-05-24 17:51:20.000000 ensurepath-0.2.0/ensurepath.egg-info/dependency_links.txt
--rw-r--r--   0 jp        (1000) wheel      (998)       20 2024-05-24 17:51:20.000000 ensurepath-0.2.0/ensurepath.egg-info/requires.txt
--rw-r--r--   0 jp        (1000) wheel      (998)       11 2024-05-24 17:51:20.000000 ensurepath-0.2.0/ensurepath.egg-info/top_level.txt
--rw-r--r--   0 jp        (1000) wheel      (998)     1318 2024-05-24 17:50:07.000000 ensurepath-0.2.0/ensurepath.py
--rw-r--r--   0 jp        (1000) wheel      (998)     1232 2024-05-24 17:50:18.000000 ensurepath-0.2.0/pyproject.toml
--rw-r--r--   0 jp        (1000) wheel      (998)       38 2024-05-24 17:51:20.010267 ensurepath-0.2.0/setup.cfg
+drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 18:18:13.030996 ensurepath-0.2.1/
+-rw-r--r--   0 jp        (1000) wheel      (998)     1275 2024-05-24 15:00:16.000000 ensurepath-0.2.1/LICENSE.md
+-rw-r--r--   0 jp        (1000) wheel      (998)     4013 2024-05-24 18:18:13.027663 ensurepath-0.2.1/PKG-INFO
+-rw-r--r--   0 jp        (1000) wheel      (998)     1396 2024-05-24 18:17:10.000000 ensurepath-0.2.1/README.md
+drwxr-xr-x   0 jp        (1000) wheel      (998)        0 2024-05-24 18:18:13.027663 ensurepath-0.2.1/ensurepath.egg-info/
+-rw-r--r--   0 jp        (1000) wheel      (998)     4013 2024-05-24 18:18:13.000000 ensurepath-0.2.1/ensurepath.egg-info/PKG-INFO
+-rw-r--r--   0 jp        (1000) wheel      (998)      218 2024-05-24 18:18:13.000000 ensurepath-0.2.1/ensurepath.egg-info/SOURCES.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)        1 2024-05-24 18:18:13.000000 ensurepath-0.2.1/ensurepath.egg-info/dependency_links.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)       20 2024-05-24 18:18:13.000000 ensurepath-0.2.1/ensurepath.egg-info/requires.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)       11 2024-05-24 18:18:13.000000 ensurepath-0.2.1/ensurepath.egg-info/top_level.txt
+-rw-r--r--   0 jp        (1000) wheel      (998)     1318 2024-05-24 17:50:07.000000 ensurepath-0.2.1/ensurepath.py
+-rw-r--r--   0 jp        (1000) wheel      (998)     1232 2024-05-24 18:10:01.000000 ensurepath-0.2.1/pyproject.toml
+-rw-r--r--   0 jp        (1000) wheel      (998)       38 2024-05-24 18:18:13.030996 ensurepath-0.2.1/setup.cfg
```

### Comparing `ensurepath-0.2.0/LICENSE.md` & `ensurepath-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ensurepath-0.2.0/PKG-INFO` & `ensurepath-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensurepath
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ensure python, pip and with pip installed binarys (scripts for win) are in your PATH variable.
 Author: Konxell
 Maintainer: Konxell
 License: Unlicense (Public Domain)
         ============================
         
         This is free and unencumbered software released into the public domain.
@@ -54,30 +54,44 @@
 
 # ensurepath
 
 Does exactly one thing:
 
 - ensure that python, pip and with pip installed binarys are in your path.
 
-## use
 
+
+## USAGE
+
+If `python` command is available:
 ```bash
-$ pip install ensurepath
+$ python -m pip install ensurepath
 ...
 $ python -m ensurepath
 ...
 ```
+Otherwise:
+```bash
+$ [path to python] -m pip install ensurepath
+...
+$ [path to python] -m ensurepath
+...
+```
 
-## why
+## Why
 
 The need occured for me when we started using pipx in a python class just to use `pipx ensurepath`.
 That is because the micrsoft store (msstore) install of python does add `python` and `pip` to the path, but not the `scripts` folder where with pip installed shell commands are located.
 I tried to also make this script add pip and python to the path if they are not in yet, but have not tested this further.
 
-# issues
+## msstroe
+
+If you're installing python from the msstore and also want that the commands that are installed with the installed packages to just work on the comandline, you're exactly right here!
+
+# Issues
 
 If you encouter any error feel free to create an issue and I will try to help, when I have the time. But this is not a python install support service ;-)
 
 This how not been tested thoroughly use at your own risk!
 
-# thanks
-This script only uses the [`userpath`](https://pypi.org/project/userpath/) module from [ofek](https://github.com/ofek), thank you!
+# Thanks
+This script only uses the [`userpath`](https://pypi.org/project/userpath/) module from [ofek](https://github.com/ofek), without you this wouldn't be possible! Thanks for your great work on `userpath`!
```

### Comparing `ensurepath-0.2.0/README.md` & `ensurepath-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 # ensurepath
 
 Does exactly one thing:
 
 - ensure that python, pip and with pip installed binarys are in your path.
 
-## use
 
+
+## USAGE
+
+If `python` command is available:
 ```bash
-$ pip install ensurepath
+$ python -m pip install ensurepath
 ...
 $ python -m ensurepath
 ...
 ```
+Otherwise:
+```bash
+$ [path to python] -m pip install ensurepath
+...
+$ [path to python] -m ensurepath
+...
+```
 
-## why
+## Why
 
 The need occured for me when we started using pipx in a python class just to use `pipx ensurepath`.
 That is because the micrsoft store (msstore) install of python does add `python` and `pip` to the path, but not the `scripts` folder where with pip installed shell commands are located.
 I tried to also make this script add pip and python to the path if they are not in yet, but have not tested this further.
 
-# issues
+## msstroe
+
+If you're installing python from the msstore and also want that the commands that are installed with the installed packages to just work on the comandline, you're exactly right here!
+
+# Issues
 
 If you encouter any error feel free to create an issue and I will try to help, when I have the time. But this is not a python install support service ;-)
 
 This how not been tested thoroughly use at your own risk!
 
-# thanks
-This script only uses the [`userpath`](https://pypi.org/project/userpath/) module from [ofek](https://github.com/ofek), thank you!
+# Thanks
+This script only uses the [`userpath`](https://pypi.org/project/userpath/) module from [ofek](https://github.com/ofek), without you this wouldn't be possible! Thanks for your great work on `userpath`!
```

### Comparing `ensurepath-0.2.0/ensurepath.egg-info/PKG-INFO` & `ensurepath-0.2.1/ensurepath.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensurepath
-Version: 0.2.0
+Version: 0.2.1
 Summary: Ensure python, pip and with pip installed binarys (scripts for win) are in your PATH variable.
 Author: Konxell
 Maintainer: Konxell
 License: Unlicense (Public Domain)
         ============================
         
         This is free and unencumbered software released into the public domain.
@@ -54,30 +54,44 @@
 
 # ensurepath
 
 Does exactly one thing:
 
 - ensure that python, pip and with pip installed binarys are in your path.
 
-## use
 
+
+## USAGE
+
+If `python` command is available:
 ```bash
-$ pip install ensurepath
+$ python -m pip install ensurepath
 ...
 $ python -m ensurepath
 ...
 ```
+Otherwise:
+```bash
+$ [path to python] -m pip install ensurepath
+...
+$ [path to python] -m ensurepath
+...
+```
 
-## why
+## Why
 
 The need occured for me when we started using pipx in a python class just to use `pipx ensurepath`.
 That is because the micrsoft store (msstore) install of python does add `python` and `pip` to the path, but not the `scripts` folder where with pip installed shell commands are located.
 I tried to also make this script add pip and python to the path if they are not in yet, but have not tested this further.
 
-# issues
+## msstroe
+
+If you're installing python from the msstore and also want that the commands that are installed with the installed packages to just work on the comandline, you're exactly right here!
+
+# Issues
 
 If you encouter any error feel free to create an issue and I will try to help, when I have the time. But this is not a python install support service ;-)
 
 This how not been tested thoroughly use at your own risk!
 
-# thanks
-This script only uses the [`userpath`](https://pypi.org/project/userpath/) module from [ofek](https://github.com/ofek), thank you!
+# Thanks
+This script only uses the [`userpath`](https://pypi.org/project/userpath/) module from [ofek](https://github.com/ofek), without you this wouldn't be possible! Thanks for your great work on `userpath`!
```

### Comparing `ensurepath-0.2.0/ensurepath.py` & `ensurepath-0.2.1/ensurepath.py`

 * *Files identical despite different names*

### Comparing `ensurepath-0.2.0/pyproject.toml` & `ensurepath-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ensurepath"
 description = "Ensure python, pip and with pip installed binarys (scripts for win) are in your PATH variable."
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 requires-python = ">=3.7"
 keywords = [
   "path",
   "user path",
   "windows",
   "linux",
   "msstore",
```

