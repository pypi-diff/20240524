# Comparing `tmp/cadprox-2.4.tar.gz` & `tmp/cadprox-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-2.4.tar", last modified: Fri May 24 10:43:18 2024, max compression
+gzip compressed data, was "cadprox-2.5.tar", last modified: Fri May 24 10:45:28 2024, max compression
```

## Comparing `cadprox-2.4.tar` & `cadprox-2.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:43:18.890392 cadprox-2.4/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.4/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:43:18.890392 cadprox-2.4/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.4/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:43:18.882391 cadprox-2.4/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.4/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2977 2024-05-24 10:26:04.000000 cadprox-2.4/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     9375 2024-05-24 10:42:48.000000 cadprox-2.4/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:43:18.890392 cadprox-2.4/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:43:18.890392 cadprox-2.4/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1773 2024-05-24 10:43:11.000000 cadprox-2.4/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:45:28.389458 cadprox-2.5/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.5/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:45:28.389458 cadprox-2.5/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.5/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:45:28.385458 cadprox-2.5/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.5/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2977 2024-05-24 10:26:04.000000 cadprox-2.5/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     9387 2024-05-24 10:45:00.000000 cadprox-2.5/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:45:28.389458 cadprox-2.5/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:45:28.389458 cadprox-2.5/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1773 2024-05-24 10:45:16.000000 cadprox-2.5/setup.py
```

### Comparing `cadprox-2.4/PKG-INFO` & `cadprox-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.4
+Version: 2.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.4/README.md` & `cadprox-2.5/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-2.4/app/main.py` & `cadprox-2.5/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-2.4/app/utils.py` & `cadprox-2.5/app/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from dotenv import load_dotenv
 import logging
 import sys
-
+import boto3
 def load_user_env():
     # Get the current working directory
     current_working_directory = os.getcwd()
 
     # Construct the path to the .env file in the current working directory
     dotenv_path = os.path.join(current_working_directory, '.env')
```

### Comparing `cadprox-2.4/cadprox.egg-info/PKG-INFO` & `cadprox-2.5/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.4
+Version: 2.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.4/setup.py` & `cadprox-2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='2.4',  # Increment the version number
+    version='2.5',  # Increment the version number
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',  # Update with your GitHub repository URL
     packages=find_packages(),
```

