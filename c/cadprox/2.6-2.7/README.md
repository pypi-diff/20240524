# Comparing `tmp/cadprox-2.6.tar.gz` & `tmp/cadprox-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-2.6.tar", last modified: Fri May 24 10:50:27 2024, max compression
+gzip compressed data, was "cadprox-2.7.tar", last modified: Fri May 24 10:54:54 2024, max compression
```

## Comparing `cadprox-2.6.tar` & `cadprox-2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:50:27.968797 cadprox-2.6/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.6/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:50:27.964797 cadprox-2.6/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.6/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:50:27.960797 cadprox-2.6/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.6/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2892 2024-05-24 10:50:15.000000 cadprox-2.6/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     9387 2024-05-24 10:45:00.000000 cadprox-2.6/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:50:27.964797 cadprox-2.6/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:50:27.000000 cadprox-2.6/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:50:27.968797 cadprox-2.6/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 10:49:50.000000 cadprox-2.6/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:54:54.575514 cadprox-2.7/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.7/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:54:54.575514 cadprox-2.7/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.7/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:54:54.567514 cadprox-2.7/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.7/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2892 2024-05-24 10:54:26.000000 cadprox-2.7/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8992 2024-05-24 10:54:12.000000 cadprox-2.7/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:54:54.575514 cadprox-2.7/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:54:54.575514 cadprox-2.7/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 10:54:42.000000 cadprox-2.7/setup.py
```

### Comparing `cadprox-2.6/PKG-INFO` & `cadprox-2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.6
+Version: 2.7
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.6/README.md` & `cadprox-2.7/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-2.6/app/main.py` & `cadprox-2.7/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-2.6/app/utils.py` & `cadprox-2.7/app/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,58 @@
+import requests
+import subprocess
+import socket
 import os
-from dotenv import load_dotenv
-import logging
-import sys
+import re
+import time
 import boto3
+from botocore.exceptions import NoCredentialsError, PartialCredentialsError
+import json
+import sys
+import logging
+import traceback
+from dotenv import load_dotenv
+
+# Load environment variables from user's current directory
 def load_user_env():
-    # Get the current working directory
     current_working_directory = os.getcwd()
-
-    # Construct the path to the .env file in the current working directory
     dotenv_path = os.path.join(current_working_directory, '.env')
-
-    # Load the .env file
     load_dotenv(dotenv_path)
 
-    # Log the environment variables to ensure they are loaded
-    logger.info(f"S3_ACCESS_KEY: {os.getenv('S3_ACCESS_KEY')}")
-    logger.info(f"S3_SECRET_KEY: {os.getenv('S3_SECRET_KEY')}")
-    logger.info(f"S3_REGION: {os.getenv('S3_REGION')}")
-    logger.info(f"S3_BUCKET: {os.getenv('S3_BUCKET')}")
-    logger.info(f"S3_CADDY_FILENAME: {os.getenv('S3_CADDY_FILENAME')}")
-
-    # Ensure these environment variables are set correctly
-    S3_ACCESS_KEY = os.getenv('S3_ACCESS_KEY')
-    S3_SECRET_KEY = os.getenv('S3_SECRET_KEY')
-    S3_REGION = os.getenv('S3_REGION')
-    S3_BUCKET = os.getenv('S3_BUCKET')
-    S3_CADDY_FILENAME = os.getenv('S3_CADDY_FILENAME', 'Caddyfile')
-
-    # Validate that none of the required environment variables are None
-    if not all([S3_ACCESS_KEY, S3_SECRET_KEY, S3_REGION, S3_BUCKET]):
-        logger.error("One or more required environment variables are missing or not loaded correctly.")
-        sys.exit(1)
-
-    # Export the variables as environment variables
-    os.environ['S3_ACCESS_KEY'] = S3_ACCESS_KEY
-    os.environ['S3_SECRET_KEY'] = S3_SECRET_KEY
-    os.environ['S3_REGION'] = S3_REGION
-    os.environ['S3_BUCKET'] = S3_BUCKET
-    os.environ['S3_CADDY_FILENAME'] = S3_CADDY_FILENAME
+load_user_env()
 
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 
-# Load user environment variables and export them
-load_user_env()
+# Fetch and export environment variables
+S3_ACCESS_KEY = os.getenv('S3_ACCESS_KEY')
+S3_SECRET_KEY = os.getenv('S3_SECRET_KEY')
+S3_REGION = os.getenv('S3_REGION')
+S3_BUCKET = os.getenv('S3_BUCKET')
+S3_CADDY_FILENAME = os.getenv('S3_CADDY_FILENAME', 'Caddyfile')
+
+# Validate environment variables
+if not all([S3_ACCESS_KEY, S3_SECRET_KEY, S3_REGION, S3_BUCKET]):
+    logger.error("One or more required environment variables are missing or not loaded correctly.")
+    sys.exit(1)
+
+os.environ['S3_ACCESS_KEY'] = S3_ACCESS_KEY
+os.environ['S3_SECRET_KEY'] = S3_SECRET_KEY
+os.environ['S3_REGION'] = S3_REGION
+os.environ['S3_BUCKET'] = S3_BUCKET
+os.environ['S3_CADDY_FILENAME'] = S3_CADDY_FILENAME
 
 def load_s3_client():
     return boto3.client(
         's3',
         aws_access_key_id=os.getenv('S3_ACCESS_KEY'),
         aws_secret_access_key=os.getenv('S3_SECRET_KEY'),
         region_name=os.getenv('S3_REGION')
     )
+
 def get_external_ip():
     try:
         response = requests.get('https://api.ipify.org?format=json')
         response.raise_for_status()
         return response.json()['ip']
     except requests.RequestException as e:
         logger.error(f"Error retrieving external IP address: {e}")
@@ -82,31 +79,30 @@
             success_info = response.json()
             logger.info(f"Successfully added DNS record: {json.dumps(success_info, indent=2)}")
             return
         else:
             error_info = response.json()
             logger.error(f"Failed to add DNS record: {json.dumps(error_info, indent=2)}")
             if response.status_code == 429 or any(e['code'] == 971 for e in error_info.get('errors', [])):
-                # If rate limited, wait and retry
                 logger.info(f"Retrying in {wait_time} seconds...")
                 time.sleep(wait_time)
-                wait_time *= 2  # Exponential backoff
+                wait_time *= 2
             else:
-                sys.exit(1)  # Exit if the DNS record addition fails due to other reasons
+                sys.exit(1)
     logger.error("Max retries exceeded. Could not add DNS record.")
     sys.exit(1)
 
 def download_caddyfile_from_s3(s3_client, bucket_name, s3_caddy_filename, local_caddyfile_path):
     try:
         s3_client.download_file(bucket_name, s3_caddy_filename, local_caddyfile_path)
         logger.info(f"Downloaded Caddyfile from S3 bucket {bucket_name}")
     except s3_client.exceptions.NoSuchKey:
         logger.info(f"Caddyfile {s3_caddy_filename} not found in S3 bucket {bucket_name}. Creating a new one.")
         with open(local_caddyfile_path, 'w') as f:
-            f.write('')  # Create an empty Caddyfile
+            f.write('')
     except NoCredentialsError:
         logger.error("AWS credentials not available.")
         sys.exit(1)
     except PartialCredentialsError:
         logger.error("Incomplete AWS credentials provided.")
         sys.exit(1)
     except Exception as e:
@@ -125,43 +121,49 @@
         logger.error("Incomplete AWS credentials provided.")
         sys.exit(1)
     except Exception as e:
         logger.error(f"Error uploading Caddyfile to S3: {e}")
         logger.error(traceback.format_exc())
         sys.exit(1)
 
-def update_caddyfile(subdomain, port, caddyfile_path):
+def get_caddyfile_path():
+    return os.path.expanduser('~/caddy_config/Caddyfile')
+
+def update_caddyfile(subdomain, port):
+    caddyfile_path = get_caddyfile_path()
     new_entry = f"{subdomain} {{\n    reverse_proxy localhost:{port}\n}}\n"
     try:
         with open(caddyfile_path, 'a') as caddy_file:
             caddy_file.write(new_entry)
         logger.info(f"Updated Caddyfile with new entry for {subdomain}")
     except PermissionError:
         logger.error(f"Permission denied when trying to write to {caddyfile_path}")
         logger.error(traceback.format_exc())
 
-def format_caddyfile(caddyfile_path):
-    result = subprocess.run(['caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
+def format_caddyfile():
+    caddyfile_path = get_caddyfile_path()
+    result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddyfile formatted successfully")
     else:
         logger.error(f"Failed to format Caddyfile: {result.stderr}")
 
 def restart_caddy():
-    result = subprocess.run(['sudo', 'caddy', 'reload'], capture_output=True, text=True)
+    result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'reload'], capture_output=True, text=True)
     if result.returncode == 0:
-        logger.info("Caddy server reloaded successfully")
+        logger.info("Caddy server reloaded successfully within Docker")
     else:
-        logger.error(f"Failed to reload Caddy server: {result.stderr}")
+        logger.error(f"Failed to reload Caddy server in Docker: {result.stderr}")
 
 def check_port_in_use(port):
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
         return sock.connect_ex(('localhost', int(port))) == 0
 
-def check_domain_exists(subdomain, caddyfile_path):
+def check_domain_exists(subdomain):
+    caddyfile_path = get_caddyfile_path()
     try:
         with open(caddyfile_path, 'r') as caddy_file:
             content = caddy_file.read()
             return re.search(rf"{subdomain} \{{.*?\}}", content, flags=re.DOTALL) is not None
     except FileNotFoundError:
         logger.error(f"Caddyfile {caddyfile_path} not found.")
         return False
@@ -186,15 +188,15 @@
         time.sleep(wait_time)
         attempts += 1
     logger.warning(f"{subdomain} is not resolvable after {max_attempts} attempts, continuing anyway")
     return False
 
 def load_profiles(s3_client):
     try:
-        response = s3_client.get_object(Bucket=S3_BUCKET, Key='caddy_profiles.json')
+        response = s3_client.get_object(Bucket=os.getenv('S3_BUCKET'), Key='caddy_profiles.json')
         profiles = json.loads(response['Body'].read().decode('utf-8'))
         return profiles
     except s3_client.exceptions.NoSuchKey:
         return {}
     except NoCredentialsError:
         logger.error("AWS credentials not available.")
         return {}
@@ -225,15 +227,15 @@
     except Exception as e:
         caddy_profiles = {}
 
     caddy_profiles[profile_key] = profile
 
     try:
         s3_client.put_object(
-            Bucket=S3_BUCKET,
+            Bucket=os.getenv('S3_BUCKET'),
             Key='caddy_profiles.json',
             Body=json.dumps(caddy_profiles)
         )
         logger.info(f"Profile '{profile_name}' created successfully.")
     except Exception as e:
         logger.error(f"Error creating profile: {e}")
         logger.error(traceback.format_exc())
```

### Comparing `cadprox-2.6/cadprox.egg-info/PKG-INFO` & `cadprox-2.7/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.6
+Version: 2.7
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.6/setup.py` & `cadprox-2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='2.6',
+    version='2.7',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

