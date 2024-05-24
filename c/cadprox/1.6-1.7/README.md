# Comparing `tmp/cadprox-1.6.tar.gz` & `tmp/cadprox-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-1.6.tar", last modified: Fri May 24 04:22:44 2024, max compression
+gzip compressed data, was "cadprox-1.7.tar", last modified: Fri May 24 04:28:00 2024, max compression
```

## Comparing `cadprox-1.6.tar` & `cadprox-1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:22:44.800379 cadprox-1.6/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-1.6/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:22:44.796379 cadprox-1.6/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      287 2024-05-24 03:13:51.000000 cadprox-1.6/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:22:44.792379 cadprox-1.6/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-1.6/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-1.6/app/config.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3094 2024-05-24 04:21:50.000000 cadprox-1.6/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     7922 2024-05-24 04:21:59.000000 cadprox-1.6/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:22:44.796379 cadprox-1.6/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      269 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 04:22:44.800379 cadprox-1.6/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)      901 2024-05-24 04:22:36.000000 cadprox-1.6/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:28:00.977989 cadprox-1.7/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-1.7/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:28:00.977989 cadprox-1.7/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      287 2024-05-24 03:13:51.000000 cadprox-1.7/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:28:00.969988 cadprox-1.7/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-1.7/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-1.7/app/config.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3094 2024-05-24 04:27:05.000000 cadprox-1.7/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8164 2024-05-24 04:27:16.000000 cadprox-1.7/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:28:00.977989 cadprox-1.7/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      269 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 04:28:00.000000 cadprox-1.7/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 04:28:00.977989 cadprox-1.7/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)      933 2024-05-24 04:27:55.000000 cadprox-1.7/setup.py
```

### Comparing `cadprox-1.6/PKG-INFO` & `cadprox-1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 1.6
+Version: 1.7
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadprox
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-1.6/app/main.py` & `cadprox-1.7/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-1.6/app/utils.py` & `cadprox-1.7/app/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 import time
 import boto3
 from botocore.exceptions import NoCredentialsError, PartialCredentialsError
 import json
 import sys
 import logging
+import traceback
 from dotenv import load_dotenv
 
 load_dotenv()
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 
@@ -85,38 +86,41 @@
         logger.error("AWS credentials not available.")
         sys.exit(1)
     except PartialCredentialsError:
         logger.error("Incomplete AWS credentials provided.")
         sys.exit(1)
     except Exception as e:
         logger.error(f"Error downloading Caddyfile from S3: {e}")
+        logger.error(traceback.format_exc())
         sys.exit(1)
 
 def upload_caddyfile_to_s3(s3_client, bucket_name, s3_caddy_filename, local_caddyfile_path):
     try:
         s3_client.upload_file(local_caddyfile_path, bucket_name, s3_caddy_filename)
         logger.info(f"Uploaded Caddyfile to S3 bucket {bucket_name}")
     except NoCredentialsError:
         logger.error("AWS credentials not available.")
         sys.exit(1)
     except PartialCredentialsError:
         logger.error("Incomplete AWS credentials provided.")
         sys.exit(1)
     except Exception as e:
         logger.error(f"Error uploading Caddyfile to S3: {e}")
+        logger.error(traceback.format_exc())
         sys.exit(1)
 
 def update_caddyfile(subdomain, port, caddyfile_path):
     new_entry = f"{subdomain} {{\n    reverse_proxy localhost:{port}\n}}\n"
     try:
         with open(caddyfile_path, 'a') as caddy_file:
             caddy_file.write(new_entry)
         logger.info(f"Updated Caddyfile with new entry for {subdomain}")
     except PermissionError:
         logger.error(f"Permission denied when trying to write to {caddyfile_path}")
+        logger.error(traceback.format_exc())
 
 def format_caddyfile(caddyfile_path):
     result = subprocess.run(['caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddyfile formatted successfully")
     else:
         logger.error(f"Failed to format Caddyfile: {result.stderr}")
@@ -174,14 +178,15 @@
         logger.error("AWS credentials not available.")
         return {}
     except PartialCredentialsError:
         logger.error("Incomplete AWS credentials provided.")
         return {}
     except Exception as e:
         logger.error(f"Error loading profiles: {e}")
+        logger.error(traceback.format_exc())
         return {}
 
 def prompt_for_profile():
     profile = {
         "CLOUDFLARE_API_TOKEN": input("CLOUDFLARE_API_TOKEN: "),
         "CLOUDFLARE_ZONE_ID": input("CLOUDFLARE_ZONE_ID: "),
         "S3_CADDY_FILENAME": input("S3_CADDY_FILENAME: "),
@@ -206,7 +211,8 @@
             Bucket=S3_BUCKET,
             Key='caddy_profiles.json',
             Body=json.dumps(caddy_profiles)
         )
         logger.info(f"Profile '{profile_name}' created successfully.")
     except Exception as e:
         logger.error(f"Error creating profile: {e}")
+        logger.error(traceback.format_exc())
```

### Comparing `cadprox-1.6/cadprox.egg-info/PKG-INFO` & `cadprox-1.7/cadprox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 1.6
+Version: 1.7
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadprox
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-1.6/setup.py` & `cadprox-1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cadprox',
-    version='1.6',
+    version='1.7',  # Increment the version number
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadprox',  # Update with your GitHub repository URL
     packages=find_packages(),
```

