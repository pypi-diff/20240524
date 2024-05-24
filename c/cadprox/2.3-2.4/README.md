# Comparing `tmp/cadprox-2.3.tar.gz` & `tmp/cadprox-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-2.3.tar", last modified: Fri May 24 10:37:29 2024, max compression
+gzip compressed data, was "cadprox-2.4.tar", last modified: Fri May 24 10:43:18 2024, max compression
```

## Comparing `cadprox-2.3.tar` & `cadprox-2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:37:29.934663 cadprox-2.3/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.3/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:37:29.934663 cadprox-2.3/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.3/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:37:29.926663 cadprox-2.3/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.3/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2977 2024-05-24 10:26:04.000000 cadprox-2.3/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8789 2024-05-24 10:35:46.000000 cadprox-2.3/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:37:29.930663 cadprox-2.3/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:37:29.934663 cadprox-2.3/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1773 2024-05-24 10:37:22.000000 cadprox-2.3/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:43:18.890392 cadprox-2.4/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.4/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:43:18.890392 cadprox-2.4/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.4/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:43:18.882391 cadprox-2.4/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.4/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2977 2024-05-24 10:26:04.000000 cadprox-2.4/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     9375 2024-05-24 10:42:48.000000 cadprox-2.4/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:43:18.890392 cadprox-2.4/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:43:18.000000 cadprox-2.4/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:43:18.890392 cadprox-2.4/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1773 2024-05-24 10:43:11.000000 cadprox-2.4/setup.py
```

### Comparing `cadprox-2.3/PKG-INFO` & `cadprox-2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.3
+Version: 2.4
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.3/README.md` & `cadprox-2.4/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-2.3/app/main.py` & `cadprox-2.4/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-2.3/app/utils.py` & `cadprox-2.4/app/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,61 @@
-#cadprox/app/utils.py
-import requests
-import subprocess
-import socket
 import os
-import re
-import time
-import boto3
-from botocore.exceptions import NoCredentialsError, PartialCredentialsError
-import json
-import sys
-import logging
-import traceback
 from dotenv import load_dotenv
+import logging
+import sys
 
-load_dotenv()
+def load_user_env():
+    # Get the current working directory
+    current_working_directory = os.getcwd()
+
+    # Construct the path to the .env file in the current working directory
+    dotenv_path = os.path.join(current_working_directory, '.env')
+
+    # Load the .env file
+    load_dotenv(dotenv_path)
+
+    # Log the environment variables to ensure they are loaded
+    logger.info(f"S3_ACCESS_KEY: {os.getenv('S3_ACCESS_KEY')}")
+    logger.info(f"S3_SECRET_KEY: {os.getenv('S3_SECRET_KEY')}")
+    logger.info(f"S3_REGION: {os.getenv('S3_REGION')}")
+    logger.info(f"S3_BUCKET: {os.getenv('S3_BUCKET')}")
+    logger.info(f"S3_CADDY_FILENAME: {os.getenv('S3_CADDY_FILENAME')}")
+
+    # Ensure these environment variables are set correctly
+    S3_ACCESS_KEY = os.getenv('S3_ACCESS_KEY')
+    S3_SECRET_KEY = os.getenv('S3_SECRET_KEY')
+    S3_REGION = os.getenv('S3_REGION')
+    S3_BUCKET = os.getenv('S3_BUCKET')
+    S3_CADDY_FILENAME = os.getenv('S3_CADDY_FILENAME', 'Caddyfile')
+
+    # Validate that none of the required environment variables are None
+    if not all([S3_ACCESS_KEY, S3_SECRET_KEY, S3_REGION, S3_BUCKET]):
+        logger.error("One or more required environment variables are missing or not loaded correctly.")
+        sys.exit(1)
+
+    # Export the variables as environment variables
+    os.environ['S3_ACCESS_KEY'] = S3_ACCESS_KEY
+    os.environ['S3_SECRET_KEY'] = S3_SECRET_KEY
+    os.environ['S3_REGION'] = S3_REGION
+    os.environ['S3_BUCKET'] = S3_BUCKET
+    os.environ['S3_CADDY_FILENAME'] = S3_CADDY_FILENAME
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 
-# Log the environment variables to ensure they are loaded
-logger.info(f"S3_ACCESS_KEY: {os.getenv('S3_ACCESS_KEY')}")
-logger.info(f"S3_SECRET_KEY: {os.getenv('S3_SECRET_KEY')}")
-logger.info(f"S3_REGION: {os.getenv('S3_REGION')}")
-logger.info(f"S3_BUCKET: {os.getenv('S3_BUCKET')}")
-logger.info(f"S3_CADDY_FILENAME: {os.getenv('S3_CADDY_FILENAME')}")
-
-
-S3_ACCESS_KEY = os.getenv('S3_ACCESS_KEY')
-S3_SECRET_KEY = os.getenv('S3_SECRET_KEY')
-S3_REGION = os.getenv('S3_REGION')
-S3_BUCKET = os.getenv('S3_BUCKET')
-S3_CADDY_FILENAME = os.getenv('S3_CADDY_FILENAME', 'Caddyfile')
-
-# Validate that none of the required environment variables are None
-if not all([S3_ACCESS_KEY, S3_SECRET_KEY, S3_REGION, S3_BUCKET]):
-    logger.error("One or more required environment variables are missing or not loaded correctly.")
-    sys.exit(1)
+# Load user environment variables and export them
+load_user_env()
 
 def load_s3_client():
     return boto3.client(
         's3',
-        aws_access_key_id=S3_ACCESS_KEY,
-        aws_secret_access_key=S3_SECRET_KEY,
-        region_name=S3_REGION
+        aws_access_key_id=os.getenv('S3_ACCESS_KEY'),
+        aws_secret_access_key=os.getenv('S3_SECRET_KEY'),
+        region_name=os.getenv('S3_REGION')
     )
-
 def get_external_ip():
     try:
         response = requests.get('https://api.ipify.org?format=json')
         response.raise_for_status()
         return response.json()['ip']
     except requests.RequestException as e:
         logger.error(f"Error retrieving external IP address: {e}")
```

### Comparing `cadprox-2.3/cadprox.egg-info/PKG-INFO` & `cadprox-2.4/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.3
+Version: 2.4
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.3/setup.py` & `cadprox-2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='2.3',  # Increment the version number
+    version='2.4',  # Increment the version number
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',  # Update with your GitHub repository URL
     packages=find_packages(),
```

