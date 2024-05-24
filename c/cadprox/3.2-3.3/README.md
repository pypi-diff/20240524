# Comparing `tmp/cadprox-3.2.tar.gz` & `tmp/cadprox-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-3.2.tar", last modified: Fri May 24 11:22:03 2024, max compression
+gzip compressed data, was "cadprox-3.3.tar", last modified: Fri May 24 11:26:53 2024, max compression
```

## Comparing `cadprox-3.2.tar` & `cadprox-3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:22:03.980337 cadprox-3.2/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.2/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:22:03.980337 cadprox-3.2/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.2/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:22:03.972337 cadprox-3.2/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.2/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3847 2024-05-24 11:21:30.000000 cadprox-3.2/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    10478 2024-05-24 11:21:14.000000 cadprox-3.2/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:22:03.980337 cadprox-3.2/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:22:03.980337 cadprox-3.2/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:21:55.000000 cadprox-3.2/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:26:53.573100 cadprox-3.3/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.3/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:26:53.569100 cadprox-3.3/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.3/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:26:53.565100 cadprox-3.3/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.3/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3847 2024-05-24 11:26:27.000000 cadprox-3.3/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    10932 2024-05-24 11:25:59.000000 cadprox-3.3/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:26:53.569100 cadprox-3.3/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:26:53.573100 cadprox-3.3/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:26:44.000000 cadprox-3.3/setup.py
```

### Comparing `cadprox-3.2/PKG-INFO` & `cadprox-3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.2
+Version: 3.3
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.2/README.md` & `cadprox-3.3/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-3.2/app/main.py` & `cadprox-3.3/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-3.2/app/utils.py` & `cadprox-3.3/app/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,21 @@
 # Fetch and export environment variables
 S3_ACCESS_KEY = os.getenv('S3_ACCESS_KEY')
 S3_SECRET_KEY = os.getenv('S3_SECRET_KEY')
 S3_REGION = os.getenv('S3_REGION')
 S3_BUCKET = os.getenv('S3_BUCKET')
 S3_CADDY_FILENAME = os.getenv('S3_CADDY_FILENAME', 'Caddyfile')
 
+# Log the environment variables
+logger.info(f"S3_ACCESS_KEY: {S3_ACCESS_KEY}")
+logger.info(f"S3_SECRET_KEY: {S3_SECRET_KEY}")
+logger.info(f"S3_REGION: {S3_REGION}")
+logger.info(f"S3_BUCKET: {S3_BUCKET}")
+logger.info(f"S3_CADDY_FILENAME: {S3_CADDY_FILENAME}")
+
 # Validate environment variables
 if not all([S3_ACCESS_KEY, S3_SECRET_KEY, S3_REGION, S3_BUCKET, S3_CADDY_FILENAME]):
     logger.error("One or more required environment variables are missing or not loaded correctly.")
     sys.exit(1)
 
 os.environ['S3_ACCESS_KEY'] = S3_ACCESS_KEY
 os.environ['S3_SECRET_KEY'] = S3_SECRET_KEY
@@ -100,14 +107,15 @@
                         return False
             else:
                 return False
     return False
 
 def download_caddyfile_from_s3(s3_client, bucket_name, s3_caddy_filename, local_caddyfile_path):
     try:
+        logger.info(f"Downloading Caddyfile from bucket: {bucket_name}, key: {s3_caddy_filename}")
         s3_client.download_file(bucket_name, s3_caddy_filename, local_caddyfile_path)
         logger.info(f"Downloaded Caddyfile from S3 bucket {bucket_name}")
     except s3_client.exceptions.NoSuchKey:
         logger.info(f"Caddyfile {s3_caddy_filename} not found in S3 bucket {bucket_name}. Creating a new one.")
         with open(local_caddyfile_path, 'w') as f:
             f.write('')
     except NoCredentialsError:
@@ -119,14 +127,15 @@
     except Exception as e:
         logger.error(f"Error downloading Caddyfile from S3: {e}")
         logger.error(traceback.format_exc())
         sys.exit(1)
 
 def upload_caddyfile_to_s3(s3_client, bucket_name, s3_caddy_filename, local_caddyfile_path):
     try:
+        logger.info(f"Uploading Caddyfile to bucket: {bucket_name}, key: {s3_caddy_filename}")
         s3_client.upload_file(local_caddyfile_path, bucket_name, s3_caddy_filename)
         logger.info(f"Uploaded Caddyfile to S3 bucket {bucket_name}")
     except NoCredentialsError:
         logger.error("AWS credentials not available.")
         sys.exit(1)
     except PartialCredentialsError:
         logger.error("Incomplete AWS credentials provided.")
```

### Comparing `cadprox-3.2/cadprox.egg-info/PKG-INFO` & `cadprox-3.3/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.2
+Version: 3.3
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.2/setup.py` & `cadprox-3.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='3.2',
+    version='3.3',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

