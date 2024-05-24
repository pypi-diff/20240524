# Comparing `tmp/python_project_manager-2.0.0.tar.gz` & `tmp/python_project_manager-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_project_manager-2.0.0.tar", last modified: Tue May 21 22:03:01 2024, max compression
+gzip compressed data, was "python_project_manager-2.1.0.tar", last modified: Fri May 24 15:31:07 2024, max compression
```

## Comparing `python_project_manager-2.0.0.tar` & `python_project_manager-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 22:03:01.210039 python_project_manager-2.0.0/
--rw-rw-rw-   0        0        0    35821 2024-05-21 12:45:57.000000 python_project_manager-2.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      226 2024-05-21 22:03:01.196452 python_project_manager-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-21 12:45:57.000000 python_project_manager-2.0.0/README.md
--rw-rw-rw-   0        0        0     1061 2024-05-21 22:02:44.000000 python_project_manager-2.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-21 22:03:01.035507 python_project_manager-2.0.0/python_project_manager/
--rw-rw-rw-   0        0        0       97 2024-05-21 12:45:57.000000 python_project_manager-2.0.0/python_project_manager/__init__.py
--rw-rw-rw-   0        0        0    12576 2024-05-21 21:50:27.000000 python_project_manager-2.0.0/python_project_manager/app.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:03:01.115952 python_project_manager-2.0.0/python_project_manager/builtin_engines/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:45:57.000000 python_project_manager-2.0.0/python_project_manager/builtin_engines/__init__.py
--rw-rw-rw-   0        0        0     1829 2024-05-21 21:52:42.000000 python_project_manager-2.0.0/python_project_manager/builtin_engines/builtin_pyinstaller.py
--rw-rw-rw-   0        0        0     5196 2024-05-21 21:55:05.000000 python_project_manager-2.0.0/python_project_manager/builtin_engines/builtin_setuptools.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:03:01.176272 python_project_manager-2.0.0/python_project_manager/builtin_engines/toml/
--rw-rw-rw-   0        0        0      985 2024-05-21 12:45:57.000000 python_project_manager-2.0.0/python_project_manager/builtin_engines/toml/__init__.py
--rw-rw-rw-   0        0        0    39995 2024-05-21 12:45:57.000000 python_project_manager-2.0.0/python_project_manager/builtin_engines/toml/decoder.py
--rw-rw-rw-   0        0        0    10240 2024-05-21 12:45:57.000000 python_project_manager-2.0.0/python_project_manager/builtin_engines/toml/encoder.py
--rw-rw-rw-   0        0        0      377 2024-05-21 12:45:57.000000 python_project_manager-2.0.0/python_project_manager/builtin_engines/toml/ordered.py
--rw-rw-rw-   0        0        0      725 2024-05-21 12:45:57.000000 python_project_manager-2.0.0/python_project_manager/builtin_engines/toml/tz.py
--rw-rw-rw-   0        0        0     3278 2024-05-21 14:08:59.000000 python_project_manager-2.0.0/python_project_manager/config.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:03:01.190325 python_project_manager-2.0.0/python_project_manager.egg-info/
--rw-rw-rw-   0        0        0      226 2024-05-21 22:03:00.000000 python_project_manager-2.0.0/python_project_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      874 2024-05-21 22:03:00.000000 python_project_manager-2.0.0/python_project_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 22:03:00.000000 python_project_manager-2.0.0/python_project_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      691 2024-05-21 22:03:00.000000 python_project_manager-2.0.0/python_project_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-05-21 22:03:00.000000 python_project_manager-2.0.0/python_project_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-21 22:03:00.000000 python_project_manager-2.0.0/python_project_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       29 2024-05-21 12:45:57.000000 python_project_manager-2.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 22:03:01.211029 python_project_manager-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 15:31:07.658243 python_project_manager-2.1.0/
+-rw-rw-rw-   0        0        0    35821 2024-05-21 12:45:57.000000 python_project_manager-2.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      263 2024-05-24 15:31:07.655396 python_project_manager-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:45:57.000000 python_project_manager-2.1.0/README.md
+-rw-rw-rw-   0        0        0     1061 2024-05-24 15:31:01.000000 python_project_manager-2.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-24 15:31:07.595883 python_project_manager-2.1.0/python_project_manager/
+-rw-rw-rw-   0        0        0       97 2024-05-21 12:45:57.000000 python_project_manager-2.1.0/python_project_manager/__init__.py
+-rw-rw-rw-   0        0        0    12665 2024-05-24 13:51:44.000000 python_project_manager-2.1.0/python_project_manager/app.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:31:07.632203 python_project_manager-2.1.0/python_project_manager/builtin_engines/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:45:57.000000 python_project_manager-2.1.0/python_project_manager/builtin_engines/__init__.py
+-rw-rw-rw-   0        0        0     1829 2024-05-21 21:52:42.000000 python_project_manager-2.1.0/python_project_manager/builtin_engines/builtin_pyinstaller.py
+-rw-rw-rw-   0        0        0     5196 2024-05-21 21:55:05.000000 python_project_manager-2.1.0/python_project_manager/builtin_engines/builtin_setuptools.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:31:07.649117 python_project_manager-2.1.0/python_project_manager/builtin_engines/toml/
+-rw-rw-rw-   0        0        0      985 2024-05-21 12:45:57.000000 python_project_manager-2.1.0/python_project_manager/builtin_engines/toml/__init__.py
+-rw-rw-rw-   0        0        0    39995 2024-05-21 12:45:57.000000 python_project_manager-2.1.0/python_project_manager/builtin_engines/toml/decoder.py
+-rw-rw-rw-   0        0        0    10240 2024-05-21 12:45:57.000000 python_project_manager-2.1.0/python_project_manager/builtin_engines/toml/encoder.py
+-rw-rw-rw-   0        0        0      377 2024-05-21 12:45:57.000000 python_project_manager-2.1.0/python_project_manager/builtin_engines/toml/ordered.py
+-rw-rw-rw-   0        0        0      725 2024-05-21 12:45:57.000000 python_project_manager-2.1.0/python_project_manager/builtin_engines/toml/tz.py
+-rw-rw-rw-   0        0        0     3652 2024-05-24 15:17:11.000000 python_project_manager-2.1.0/python_project_manager/config.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:31:07.652390 python_project_manager-2.1.0/python_project_manager.egg-info/
+-rw-rw-rw-   0        0        0      263 2024-05-24 15:31:07.000000 python_project_manager-2.1.0/python_project_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      874 2024-05-24 15:31:07.000000 python_project_manager-2.1.0/python_project_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 15:31:07.000000 python_project_manager-2.1.0/python_project_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      691 2024-05-24 15:31:07.000000 python_project_manager-2.1.0/python_project_manager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-05-24 15:31:07.000000 python_project_manager-2.1.0/python_project_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-24 15:31:07.000000 python_project_manager-2.1.0/python_project_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       51 2024-05-23 15:54:45.000000 python_project_manager-2.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 15:31:07.659355 python_project_manager-2.1.0/setup.cfg
```

### Comparing `python_project_manager-2.0.0/LICENSE.txt` & `python_project_manager-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.0.0/pyproject.toml` & `python_project_manager-2.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "python-project-manager"
 description = "A Python package."
 authors = []
 readme = "README.md"
 keywords = []
-version = "2.0.0"
+version = "2.1.0"
 dynamic = [ "dependencies",]
 
 [project.scripts]
 ppm = "python_project_manager.app:cli"
 ppm-builtin-setuptools-build = "python_project_manager.builtin_engines.builtin_setuptools:_build"
 ppm-builtin-setuptools-install = "python_project_manager.builtin_engines.builtin_setuptools:_install"
 ppm-builtin-setuptools-uninstall = "python_project_manager.builtin_engines.builtin_setuptools:_uninstall"
```

### Comparing `python_project_manager-2.0.0/python_project_manager/app.py` & `python_project_manager-2.1.0/python_project_manager/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,17 +172,18 @@
     if not cli_command:
         print(f"Script '{script_name}' not found")
         return
 
     ## Smart change directory
     cwd = os.getcwd() # Get the current working directory
 
-    # Check if the command has a change directory command
-    has_change_directory_command = re.search(r'(^|\s)cd\s\w*', cli_command)
-    if not has_change_directory_command:
+    # Checks if 'cwd' is in the 'src' directory
+    skip_chdir = re.search(r'(^|\s)cd\s\w*', cli_command) # Check for 'cd' command
+    skip_chdir = skip_chdir and re.search(r'(^|\s)unittest\s\w', cli_command) # Check for 'unittest' command
+    if not skip_chdir:
         # Searches for the 'python' command along with the script path
         python_command = re.search(r'python.*\.py', cli_command)
         if python_command:
             # Get the python path
             python_path = re.search(r'\S*\.py', python_command[0])
             if python_path:
                 # Get the first dir in python path
```

### Comparing `python_project_manager-2.0.0/python_project_manager/builtin_engines/builtin_pyinstaller.py` & `python_project_manager-2.1.0/python_project_manager/builtin_engines/builtin_pyinstaller.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.0.0/python_project_manager/builtin_engines/builtin_setuptools.py` & `python_project_manager-2.1.0/python_project_manager/builtin_engines/builtin_setuptools.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.0.0/python_project_manager/builtin_engines/toml/__init__.py` & `python_project_manager-2.1.0/python_project_manager/builtin_engines/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.0.0/python_project_manager/builtin_engines/toml/decoder.py` & `python_project_manager-2.1.0/python_project_manager/builtin_engines/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.0.0/python_project_manager/builtin_engines/toml/encoder.py` & `python_project_manager-2.1.0/python_project_manager/builtin_engines/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.0.0/python_project_manager/builtin_engines/toml/tz.py` & `python_project_manager-2.1.0/python_project_manager/builtin_engines/toml/tz.py`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.0.0/python_project_manager/config.py` & `python_project_manager-2.1.0/python_project_manager/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import re
 from typing import Tuple
+from dotenv import dotenv_values
 
 class Config:
 
-    _raw_config: dict = {}# Raw config data
-    _value_config: dict = {}# Config data with dynamic values parsed
+    _raw_config: dict = {} # Raw config data
+    _value_config: dict = {} # Config data with dynamic values parsed
 
     @staticmethod
     def get(key: str, default=None):
         keys = key.split('.')
         value = Config._value_config
         for key in keys:
             if key not in value:
@@ -59,14 +60,19 @@
     def parse(string: str, dict_obj: dict) -> str:
         # Parse dynamic values
         def parse_match(match: re.Match[str]) -> str:
             return parse_dynamic_value(match.group(0), dict_obj)
         
         # Parse dynamic values recursively
         def parse_dynamic_value(dynamic_value, dict, recursive_check: list = None) -> str:
+            if isinstance(dynamic_value, str) and dynamic_value.startswith('%env:') and dynamic_value.endswith('%'):
+                dynamic_value = dynamic_value[1:-1] # Remove the %'s
+                env_key = dynamic_value.split(':')[1] # Get the env key
+                return dotenv_values('.env')[env_key] # Get the env value
+
             if recursive_check is None: # Initialize the recursive check list
                 recursive_check = []
 
             # Check for circular references
             if dynamic_value in recursive_check:
                 raise Exception(
                     f'Circular reference detected: {' => '.join(recursive_check)} => {dynamic_value}')
```

### Comparing `python_project_manager-2.0.0/python_project_manager.egg-info/SOURCES.txt` & `python_project_manager-2.1.0/python_project_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_project_manager-2.0.0/python_project_manager.egg-info/entry_points.txt` & `python_project_manager-2.1.0/python_project_manager.egg-info/entry_points.txt`

 * *Files identical despite different names*

