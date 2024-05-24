# Comparing `tmp/cadprox-3.3.tar.gz` & `tmp/cadprox-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-3.3.tar", last modified: Fri May 24 11:26:53 2024, max compression
+gzip compressed data, was "cadprox-3.4.tar", last modified: Fri May 24 11:35:31 2024, max compression
```

## Comparing `cadprox-3.3.tar` & `cadprox-3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:26:53.573100 cadprox-3.3/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.3/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:26:53.569100 cadprox-3.3/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.3/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:26:53.565100 cadprox-3.3/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.3/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3847 2024-05-24 11:26:27.000000 cadprox-3.3/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    10932 2024-05-24 11:25:59.000000 cadprox-3.3/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:26:53.569100 cadprox-3.3/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:26:53.000000 cadprox-3.3/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:26:53.573100 cadprox-3.3/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:26:44.000000 cadprox-3.3/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:35:31.802557 cadprox-3.4/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.4/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:35:31.802557 cadprox-3.4/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.4/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:35:31.794557 cadprox-3.4/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.4/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3847 2024-05-24 11:34:32.000000 cadprox-3.4/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    11188 2024-05-24 11:34:06.000000 cadprox-3.4/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:35:31.798557 cadprox-3.4/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:35:31.802557 cadprox-3.4/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:35:15.000000 cadprox-3.4/setup.py
```

### Comparing `cadprox-3.3/PKG-INFO` & `cadprox-3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.3
+Version: 3.4
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.3/README.md` & `cadprox-3.4/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-3.3/app/main.py` & `cadprox-3.4/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-3.3/app/utils.py` & `cadprox-3.4/app/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,17 @@
                     else:
                         return False
             else:
                 return False
     return False
 
 def download_caddyfile_from_s3(s3_client, bucket_name, s3_caddy_filename, local_caddyfile_path):
+    if not s3_caddy_filename:
+        logger.error("S3_CADDY_FILENAME is empty. Cannot download Caddyfile.")
+        sys.exit(1)
     try:
         logger.info(f"Downloading Caddyfile from bucket: {bucket_name}, key: {s3_caddy_filename}")
         s3_client.download_file(bucket_name, s3_caddy_filename, local_caddyfile_path)
         logger.info(f"Downloaded Caddyfile from S3 bucket {bucket_name}")
     except s3_client.exceptions.NoSuchKey:
         logger.info(f"Caddyfile {s3_caddy_filename} not found in S3 bucket {bucket_name}. Creating a new one.")
         with open(local_caddyfile_path, 'w') as f:
@@ -126,14 +129,17 @@
         sys.exit(1)
     except Exception as e:
         logger.error(f"Error downloading Caddyfile from S3: {e}")
         logger.error(traceback.format_exc())
         sys.exit(1)
 
 def upload_caddyfile_to_s3(s3_client, bucket_name, s3_caddy_filename, local_caddyfile_path):
+    if not s3_caddy_filename:
+        logger.error("S3_CADDY_FILENAME is empty. Cannot upload Caddyfile.")
+        sys.exit(1)
     try:
         logger.info(f"Uploading Caddyfile to bucket: {bucket_name}, key: {s3_caddy_filename}")
         s3_client.upload_file(local_caddyfile_path, bucket_name, s3_caddy_filename)
         logger.info(f"Uploaded Caddyfile to S3 bucket {bucket_name}")
     except NoCredentialsError:
         logger.error("AWS credentials not available.")
         sys.exit(1)
```

### Comparing `cadprox-3.3/cadprox.egg-info/PKG-INFO` & `cadprox-3.4/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.3
+Version: 3.4
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.3/setup.py` & `cadprox-3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='3.3',
+    version='3.4',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

