# Comparing `tmp/cadprox-2.1.tar.gz` & `tmp/cadprox-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-2.1.tar", last modified: Fri May 24 05:54:05 2024, max compression
+gzip compressed data, was "cadprox-2.2.tar", last modified: Fri May 24 10:32:13 2024, max compression
```

## Comparing `cadprox-2.1.tar` & `cadprox-2.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 05:54:05.386840 cadprox-2.1/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.1/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 05:54:05.386840 cadprox-2.1/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.1/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 05:54:05.378840 cadprox-2.1/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.1/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-2.1/app/config.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2956 2024-05-24 04:49:42.000000 cadprox-2.1/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8164 2024-05-24 04:27:16.000000 cadprox-2.1/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 05:54:05.386840 cadprox-2.1/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 05:54:05.000000 cadprox-2.1/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      269 2024-05-24 05:54:05.000000 cadprox-2.1/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 05:54:05.000000 cadprox-2.1/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 05:54:05.000000 cadprox-2.1/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 05:54:05.000000 cadprox-2.1/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 05:54:05.000000 cadprox-2.1/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 05:54:05.386840 cadprox-2.1/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1755 2024-05-24 05:53:53.000000 cadprox-2.1/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:32:13.096797 cadprox-2.2/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.2/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:32:13.096797 cadprox-2.2/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.2/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:32:13.092797 cadprox-2.2/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.2/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2977 2024-05-24 10:26:04.000000 cadprox-2.2/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8538 2024-05-24 10:30:44.000000 cadprox-2.2/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:32:13.096797 cadprox-2.2/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:32:13.096797 cadprox-2.2/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1773 2024-05-24 10:31:48.000000 cadprox-2.2/setup.py
```

### Comparing `cadprox-2.1/PKG-INFO` & `cadprox-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.1
+Version: 2.2
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.1/README.md` & `cadprox-2.2/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-2.1/app/main.py` & `cadprox-2.2/app/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#cadprox/app/main.py
 import argparse
 import os
 import sys
 import boto3
 from .utils import (
     get_external_ip,
     add_dns_record,
```

### Comparing `cadprox-2.1/app/utils.py` & `cadprox-2.2/app/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#cadprox/app/utils.py
 import requests
 import subprocess
 import socket
 import os
 import re
 import time
 import boto3
@@ -13,14 +14,22 @@
 from dotenv import load_dotenv
 
 load_dotenv()
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 
+# Log the environment variables to ensure they are loaded
+logger.info(f"S3_ACCESS_KEY: {os.getenv('S3_ACCESS_KEY')}")
+logger.info(f"S3_SECRET_KEY: {os.getenv('S3_SECRET_KEY')}")
+logger.info(f"S3_REGION: {os.getenv('S3_REGION')}")
+logger.info(f"S3_BUCKET: {os.getenv('S3_BUCKET')}")
+logger.info(f"S3_CADDY_FILENAME: {os.getenv('S3_CADDY_FILENAME')}")
+
+
 S3_ACCESS_KEY = os.getenv('S3_ACCESS_KEY')
 S3_SECRET_KEY = os.getenv('S3_SECRET_KEY')
 S3_REGION = os.getenv('S3_REGION')
 S3_BUCKET = os.getenv('S3_BUCKET')
 S3_CADDY_FILENAME = os.getenv('S3_CADDY_FILENAME', 'Caddyfile')
 
 def load_s3_client():
```

### Comparing `cadprox-2.1/cadprox.egg-info/PKG-INFO` & `cadprox-2.2/cadprox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.1
+Version: 2.2
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.1/setup.py` & `cadprox-2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#cadprox/setup.py
 from setuptools import setup, find_packages
 import subprocess
 import sys
 
 def check_caddy_installed():
     try:
         result = subprocess.run(['caddy', 'version'], capture_output=True, text=True, check=True)
@@ -17,15 +18,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='2.1',  # Increment the version number
+    version='2.2',  # Increment the version number
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',  # Update with your GitHub repository URL
     packages=find_packages(),
```

