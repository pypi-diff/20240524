# Comparing `tmp/cadprox-3.5.tar.gz` & `tmp/cadprox-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-3.5.tar", last modified: Fri May 24 11:40:57 2024, max compression
+gzip compressed data, was "cadprox-3.6.tar", last modified: Fri May 24 11:45:43 2024, max compression
```

## Comparing `cadprox-3.5.tar` & `cadprox-3.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:40:57.129932 cadprox-3.5/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.5/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:40:57.129932 cadprox-3.5/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.5/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:40:57.125933 cadprox-3.5/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.5/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3925 2024-05-24 11:40:33.000000 cadprox-3.5/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    11188 2024-05-24 11:34:06.000000 cadprox-3.5/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:40:57.129932 cadprox-3.5/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:40:57.129932 cadprox-3.5/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:40:48.000000 cadprox-3.5/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:45:43.138736 cadprox-3.6/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.6/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:45:43.134736 cadprox-3.6/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.6/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:45:43.126736 cadprox-3.6/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.6/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3868 2024-05-24 11:45:26.000000 cadprox-3.6/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    10994 2024-05-24 11:45:02.000000 cadprox-3.6/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:45:43.134736 cadprox-3.6/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:45:43.138736 cadprox-3.6/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:45:33.000000 cadprox-3.6/setup.py
```

### Comparing `cadprox-3.5/PKG-INFO` & `cadprox-3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.5
+Version: 3.6
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.5/README.md` & `cadprox-3.6/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-3.5/app/main.py` & `cadprox-3.6/app/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
         if not profile:
             print(f"Error: No profile found for main domain '{main_domain}'.")
             return
 
         api_token = profile['CLOUDFLARE_API_TOKEN']
         zone_id = profile['CLOUDFLARE_ZONE_ID']
-        s3_caddy_filename = profile['S3_CADDY_FILENAME']
+        s3_caddy_filename = profile.get('S3_CADDY_FILENAME', 'Caddyfile')
         if not s3_caddy_filename:
             s3_caddy_filename = 'Caddyfile'
 
         external_ip = get_external_ip()
         if not external_ip:
             print("Failed to retrieve external IP address.")
             sys.exit(1)
@@ -72,15 +72,15 @@
         if check_port_in_use(backend_server_port):
             print(f"Warning: Port {backend_server_port} is already in use.")
             # Continue without exiting
 
         if add_dns_record(subdomain, external_ip, api_token, zone_id):
             wait_until_resolvable(subdomain)
 
-            local_caddyfile_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'Caddyfile')
+            local_caddyfile_path = os.path.join(os.getcwd(), 'Caddyfile')
 
             download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
 
             if check_domain_exists(subdomain):
                 print(f"Error: Domain {subdomain} already exists in the Caddy configuration.")
                 sys.exit(1)
 
@@ -98,15 +98,15 @@
         s3_client = boto3.client(
             's3',
             aws_access_key_id=os.getenv('S3_ACCESS_KEY'),
             aws_secret_access_key=os.getenv('S3_SECRET_KEY'),
             region_name=os.getenv('S3_REGION')
         )
 
-        local_caddyfile_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'Caddyfile')
+        local_caddyfile_path = os.path.join(os.getcwd(), 'Caddyfile')
 
         download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), os.getenv('S3_CADDY_FILENAME'), local_caddyfile_path)
         remove_caddyfile_entry(subdomain)
         format_caddyfile()
         upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), os.getenv('S3_CADDY_FILENAME'), local_caddyfile_path)
         restart_caddy()
```

### Comparing `cadprox-3.5/app/utils.py` & `cadprox-3.6/app/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,14 @@
                     else:
                         return False
             else:
                 return False
     return False
 
 def download_caddyfile_from_s3(s3_client, bucket_name, s3_caddy_filename, local_caddyfile_path):
-    if not s3_caddy_filename:
-        logger.error("S3_CADDY_FILENAME is empty. Cannot download Caddyfile.")
-        sys.exit(1)
     try:
         logger.info(f"Downloading Caddyfile from bucket: {bucket_name}, key: {s3_caddy_filename}")
         s3_client.download_file(bucket_name, s3_caddy_filename, local_caddyfile_path)
         logger.info(f"Downloaded Caddyfile from S3 bucket {bucket_name}")
     except s3_client.exceptions.NoSuchKey:
         logger.info(f"Caddyfile {s3_caddy_filename} not found in S3 bucket {bucket_name}. Creating a new one.")
         with open(local_caddyfile_path, 'w') as f:
@@ -129,17 +126,14 @@
         sys.exit(1)
     except Exception as e:
         logger.error(f"Error downloading Caddyfile from S3: {e}")
         logger.error(traceback.format_exc())
         sys.exit(1)
 
 def upload_caddyfile_to_s3(s3_client, bucket_name, s3_caddy_filename, local_caddyfile_path):
-    if not s3_caddy_filename:
-        logger.error("S3_CADDY_FILENAME is empty. Cannot upload Caddyfile.")
-        sys.exit(1)
     try:
         logger.info(f"Uploading Caddyfile to bucket: {bucket_name}, key: {s3_caddy_filename}")
         s3_client.upload_file(local_caddyfile_path, bucket_name, s3_caddy_filename)
         logger.info(f"Uploaded Caddyfile to S3 bucket {bucket_name}")
     except NoCredentialsError:
         logger.error("AWS credentials not available.")
         sys.exit(1)
@@ -148,15 +142,15 @@
         sys.exit(1)
     except Exception as e:
         logger.error(f"Error uploading Caddyfile to S3: {e}")
         logger.error(traceback.format_exc())
         sys.exit(1)
 
 def get_caddyfile_path():
-    return os.path.expanduser('~/caddy_config/Caddyfile')
+    return os.path.join(os.getcwd(), 'Caddyfile')
 
 def update_caddyfile(subdomain, port):
     caddyfile_path = get_caddyfile_path()
     new_entry = f"{subdomain} {{\n    reverse_proxy localhost:{port}\n}}\n"
     try:
         with open(caddyfile_path, 'a') as caddy_file:
             caddy_file.write(new_entry)
@@ -188,15 +182,16 @@
     result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddyfile formatted successfully")
     else:
         logger.error(f"Failed to format Caddyfile: {result.stderr}")
 
 def restart_caddy():
-    result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'reload'], capture_output=True, text=True)
+    caddyfile_path = get_caddyfile_path()
+    result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'reload', '--config', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddy server reloaded successfully within Docker")
     else:
         logger.error(f"Failed to reload Caddy server in Docker: {result.stderr}")
 
 def check_port_in_use(port):
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
```

### Comparing `cadprox-3.5/cadprox.egg-info/PKG-INFO` & `cadprox-3.6/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.5
+Version: 3.6
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.5/setup.py` & `cadprox-3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='3.5',
+    version='3.6',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

