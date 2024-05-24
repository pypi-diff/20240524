# Comparing `tmp/cadproxdk-3.8.tar.gz` & `tmp/cadproxdk-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadproxdk-3.8.tar", last modified: Fri May 24 09:24:47 2024, max compression
+gzip compressed data, was "cadproxdk-3.9.tar", last modified: Fri May 24 09:35:50 2024, max compression
```

## Comparing `cadproxdk-3.8.tar` & `cadproxdk-3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:24:47.180271 cadproxdk-3.8/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-3.8/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 09:24:47.180271 cadproxdk-3.8/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-3.8/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:24:47.172271 cadproxdk-3.8/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-3.8/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-3.8/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-3.8/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:24:47.176271 cadproxdk-3.8/cadproxdk.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 09:24:47.000000 cadproxdk-3.8/cadproxdk.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 09:24:47.000000 cadproxdk-3.8/cadproxdk.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 09:24:47.000000 cadproxdk-3.8/cadproxdk.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 09:24:47.000000 cadproxdk-3.8/cadproxdk.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 09:24:47.000000 cadproxdk-3.8/cadproxdk.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 09:24:47.000000 cadproxdk-3.8/cadproxdk.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 09:24:47.180271 cadproxdk-3.8/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1840 2024-05-24 09:24:34.000000 cadproxdk-3.8/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:35:50.579362 cadproxdk-3.9/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-3.9/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 09:35:50.579362 cadproxdk-3.9/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-3.9/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:35:50.571362 cadproxdk-3.9/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-3.9/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-3.9/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-3.9/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:35:50.575362 cadproxdk-3.9/cadproxdk.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 09:35:50.000000 cadproxdk-3.9/cadproxdk.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 09:35:50.000000 cadproxdk-3.9/cadproxdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 09:35:50.000000 cadproxdk-3.9/cadproxdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 09:35:50.000000 cadproxdk-3.9/cadproxdk.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 09:35:50.000000 cadproxdk-3.9/cadproxdk.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 09:35:50.000000 cadproxdk-3.9/cadproxdk.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 09:35:50.579362 cadproxdk-3.9/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1997 2024-05-24 09:35:44.000000 cadproxdk-3.9/setup.py
```

### Comparing `cadproxdk-3.8/PKG-INFO` & `cadproxdk-3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 3.8
+Version: 3.9
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-3.8/README.md` & `cadproxdk-3.9/README.md`

 * *Files identical despite different names*

### Comparing `cadproxdk-3.8/app/main.py` & `cadproxdk-3.9/app/main.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-3.8/app/utils.py` & `cadproxdk-3.9/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-3.8/cadproxdk.egg-info/PKG-INFO` & `cadproxdk-3.9/cadproxdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 3.8
+Version: 3.9
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-3.8/setup.py` & `cadproxdk-3.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 from setuptools import setup, find_packages
 from pathlib import Path
 import os
 
 # Function to create the directory and file
 def create_caddy_config():
     current_dir = Path().absolute()
@@ -9,29 +10,33 @@
     caddyfile_path = caddy_config_path / 'Caddyfile'
 
     try:
         # Create directory if it doesn't exist
         if not caddy_config_path.exists():
             caddy_config_path.mkdir(parents=True, exist_ok=True)
             print(f"Created directory: {caddy_config_path}")
+        else:
+            print(f"Directory already exists: {caddy_config_path}")
 
         # Create file if it doesn't exist
         if not caddyfile_path.exists():
             caddyfile_path.touch()
             print(f"Created file: {caddyfile_path}")
+        else:
+            print(f"File already exists: {caddyfile_path}")
 
     except Exception as e:
         print(f"Error creating caddy config: {e}")
 
 # Call the function to create the directory and file
 create_caddy_config()
 
 setup(
     name='cadproxdk',
-    version='3.8',  # Incremented version
+    version='3.9',  # Incremented version
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadproxdk',  # Update with your GitHub repository URL
     packages=find_packages(),
```

