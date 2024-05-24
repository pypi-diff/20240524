# Comparing `tmp/cadprox-3.8.tar.gz` & `tmp/cadprox-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-3.8.tar", last modified: Fri May 24 12:34:45 2024, max compression
+gzip compressed data, was "cadprox-3.9.tar", last modified: Fri May 24 12:47:51 2024, max compression
```

## Comparing `cadprox-3.8.tar` & `cadprox-3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:34:45.959349 cadprox-3.8/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.8/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:34:45.959349 cadprox-3.8/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.8/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:34:45.951348 cadprox-3.8/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.8/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     4420 2024-05-24 12:31:50.000000 cadprox-3.8/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    12683 2024-05-24 12:31:03.000000 cadprox-3.8/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:34:45.955349 cadprox-3.8/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 12:34:45.959349 cadprox-3.8/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1952 2024-05-24 12:34:22.000000 cadprox-3.8/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:47:51.063850 cadprox-3.9/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.9/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:47:51.059849 cadprox-3.9/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.9/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:47:51.051849 cadprox-3.9/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.9/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4420 2024-05-24 12:31:50.000000 cadprox-3.9/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    12900 2024-05-24 12:47:26.000000 cadprox-3.9/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:47:51.059849 cadprox-3.9/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 12:47:51.063850 cadprox-3.9/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1952 2024-05-24 12:47:44.000000 cadprox-3.9/setup.py
```

### Comparing `cadprox-3.8/PKG-INFO` & `cadprox-3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.8
+Version: 3.9
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.8/README.md` & `cadprox-3.9/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-3.8/app/main.py` & `cadprox-3.9/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-3.8/app/utils.py` & `cadprox-3.9/app/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 import subprocess
 import socket
 import os
 import re
 import time
 import boto3
-from botocore.exceptions import NoCredentialsError, PartialCredentialsError
+from botocore.exceptions import NoCredentialsError, PartialCredentialsError, ClientError
 import json
 import sys
 import logging
 import traceback
 from dotenv import load_dotenv
 
 # Load environment variables from user's current directory
@@ -109,18 +109,23 @@
     return False
 
 def download_caddyfile_from_s3(s3_client, bucket_name, s3_caddy_filename, local_caddyfile_path):
     try:
         logger.info(f"Downloading Caddyfile from bucket: {bucket_name}, key: {s3_caddy_filename}")
         s3_client.download_file(bucket_name, s3_caddy_filename, local_caddyfile_path)
         logger.info(f"Downloaded Caddyfile from S3 bucket {bucket_name}")
-    except s3_client.exceptions.NoSuchKey:
-        logger.info(f"Caddyfile {s3_caddy_filename} not found in S3 bucket {bucket_name}. Creating a new one.")
-        with open(local_caddyfile_path, 'w') as f:
-            f.write('')
+    except ClientError as e:
+        if e.response['Error']['Code'] == '404':
+            logger.info(f"Caddyfile {s3_caddy_filename} not found in S3 bucket {bucket_name}. Creating a new one.")
+            with open(local_caddyfile_path, 'w') as f:
+                f.write('')
+        else:
+            logger.error(f"Error downloading Caddyfile from S3: {e}")
+            logger.error(traceback.format_exc())
+            sys.exit(1)
     except NoCredentialsError:
         logger.error("AWS credentials not available.")
         sys.exit(1)
     except PartialCredentialsError:
         logger.error("Incomplete AWS credentials provided.")
         sys.exit(1)
     except Exception as e:
```

### Comparing `cadprox-3.8/cadprox.egg-info/PKG-INFO` & `cadprox-3.9/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.8
+Version: 3.9
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.8/setup.py` & `cadprox-3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         print("Please ensure Docker is installed and the Caddy container is running if you intend to use Docker-based Caddy.")
         # Do not exit since system Caddy may still be used
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='3.8',
+    version='3.9',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

