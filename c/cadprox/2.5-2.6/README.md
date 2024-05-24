# Comparing `tmp/cadprox-2.5.tar.gz` & `tmp/cadprox-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-2.5.tar", last modified: Fri May 24 10:45:28 2024, max compression
+gzip compressed data, was "cadprox-2.6.tar", last modified: Fri May 24 10:50:27 2024, max compression
```

## Comparing `cadprox-2.5.tar` & `cadprox-2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:45:28.389458 cadprox-2.5/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.5/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:45:28.389458 cadprox-2.5/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.5/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:45:28.385458 cadprox-2.5/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.5/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2977 2024-05-24 10:26:04.000000 cadprox-2.5/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     9387 2024-05-24 10:45:00.000000 cadprox-2.5/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:45:28.389458 cadprox-2.5/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:45:28.000000 cadprox-2.5/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:45:28.389458 cadprox-2.5/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1773 2024-05-24 10:45:16.000000 cadprox-2.5/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:50:27.968797 cadprox-2.6/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.6/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:50:27.964797 cadprox-2.6/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.6/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:50:27.960797 cadprox-2.6/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.6/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2892 2024-05-24 10:50:15.000000 cadprox-2.6/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     9387 2024-05-24 10:45:00.000000 cadprox-2.6/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:50:27.964797 cadprox-2.6/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:50:27.968797 cadprox-2.6/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 10:49:50.000000 cadprox-2.6/setup.py
```

### Comparing `cadprox-2.5/PKG-INFO` & `cadprox-2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.5
+Version: 2.6
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.5/README.md` & `cadprox-2.6/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-2.5/app/main.py` & `cadprox-2.6/app/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#cadprox/app/main.py
 import argparse
 import os
 import sys
 import boto3
 from .utils import (
     get_external_ip,
     add_dns_record,
@@ -74,18 +73,18 @@
         add_dns_record(subdomain, external_ip, api_token, zone_id)
         wait_until_resolvable(subdomain)
 
         local_caddyfile_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'Caddyfile')
 
         download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
 
-        if check_domain_exists(subdomain, local_caddyfile_path):
+        if check_domain_exists(subdomain):
             print(f"Error: Domain {subdomain} already exists in the Caddy configuration.")
             sys.exit(1)
 
-        update_caddyfile(subdomain, backend_server_port, local_caddyfile_path)
-        format_caddyfile(local_caddyfile_path)
+        update_caddyfile(subdomain, backend_server_port)
+        format_caddyfile()
         upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
         restart_caddy()
 
 if __name__ == "__main__":
     main()
```

### Comparing `cadprox-2.5/app/utils.py` & `cadprox-2.6/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadprox-2.5/cadprox.egg-info/PKG-INFO` & `cadprox-2.6/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.5
+Version: 2.6
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.5/setup.py` & `cadprox-2.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#cadprox/setup.py
 from setuptools import setup, find_packages
 import subprocess
 import sys
 
 def check_caddy_installed():
     try:
         result = subprocess.run(['caddy', 'version'], capture_output=True, text=True, check=True)
@@ -18,28 +17,27 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='2.5',  # Increment the version number
+    version='2.6',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/reegen66/cadprox',  # Update with your GitHub repository URL
+    url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-
     python_requires='>=3.11',
     install_requires=[
         'requests',
         'dnspython',
         'boto3',
         'python-dotenv'
     ],
```

