# Comparing `tmp/cadprox-2.8.tar.gz` & `tmp/cadprox-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-2.8.tar", last modified: Fri May 24 10:57:59 2024, max compression
+gzip compressed data, was "cadprox-2.9.tar", last modified: Fri May 24 11:09:07 2024, max compression
```

## Comparing `cadprox-2.8.tar` & `cadprox-2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:57:59.356233 cadprox-2.8/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.8/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:57:59.356233 cadprox-2.8/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.8/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:57:59.352233 cadprox-2.8/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.8/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2888 2024-05-24 10:57:21.000000 cadprox-2.8/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8992 2024-05-24 10:54:12.000000 cadprox-2.8/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:57:59.356233 cadprox-2.8/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:57:59.356233 cadprox-2.8/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 10:57:36.000000 cadprox-2.8/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:09:07.409007 cadprox-2.9/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.9/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:09:07.409007 cadprox-2.9/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.9/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:09:07.401007 cadprox-2.9/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.9/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3830 2024-05-24 11:08:34.000000 cadprox-2.9/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    10078 2024-05-24 11:08:21.000000 cadprox-2.9/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:09:07.405007 cadprox-2.9/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:09:07.000000 cadprox-2.9/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:09:07.000000 cadprox-2.9/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:09:07.000000 cadprox-2.9/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:09:07.000000 cadprox-2.9/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:09:07.000000 cadprox-2.9/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:09:07.000000 cadprox-2.9/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:09:07.409007 cadprox-2.9/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:08:51.000000 cadprox-2.9/setup.py
```

### Comparing `cadprox-2.8/PKG-INFO` & `cadprox-2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.8
+Version: 2.9
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.8/README.md` & `cadprox-2.9/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-2.8/app/main.py` & `cadprox-2.9/app/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 import boto3
 from .utils import (
     get_external_ip,
     add_dns_record,
     download_caddyfile_from_s3,
     upload_caddyfile_to_s3,
     update_caddyfile,
+    remove_caddyfile_entry,
     format_caddyfile,
     restart_caddy,
     check_port_in_use,
     check_domain_exists,
     wait_until_resolvable,
     load_profiles,
     create_profile
 )
 
 def main():
     parser = argparse.ArgumentParser(description='CADProxy Command Line Tool')
-    parser.add_argument('command', choices=['add', 'create'], help='Command to execute')
-    parser.add_argument('subdomain', help='Subdomain to add', nargs='?')
+    parser.add_argument('command', choices=['add', 'create', 'remove'], help='Command to execute')
+    parser.add_argument('subdomain', help='Subdomain to add or remove', nargs='?')
     parser.add_argument('-p', '--port', required=False, help='Backend server port')
 
     args = parser.parse_args()
 
     if args.command == 'create':
         profile_name = args.subdomain
         if profile_name:
@@ -63,28 +64,49 @@
 
         external_ip = get_external_ip()
         if not external_ip:
             print("Failed to retrieve external IP address.")
             sys.exit(1)
 
         if check_port_in_use(backend_server_port):
-            print(f"Error: Port {backend_server_port} is active. OK")
-            #sys.exit(1)
+            print(f"Error: Port {backend_server_port} is already in use.")
+            sys.exit(1)
 
-        add_dns_record(subdomain, external_ip, api_token, zone_id)
-        wait_until_resolvable(subdomain)
+        if add_dns_record(subdomain, external_ip, api_token, zone_id):
+            wait_until_resolvable(subdomain)
 
-        local_caddyfile_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'Caddyfile')
+            local_caddyfile_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'Caddyfile')
 
-        download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
+            download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
 
-        if check_domain_exists(subdomain):
-            print(f"Error: Domain {subdomain} already exists in the Caddy configuration.")
-            sys.exit(1)
+            if check_domain_exists(subdomain):
+                print(f"Error: Domain {subdomain} already exists in the Caddy configuration.")
+                sys.exit(1)
+
+            update_caddyfile(subdomain, backend_server_port)
+            format_caddyfile()
+            upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
+            restart_caddy()
+
+    if args.command == 'remove':
+        subdomain = args.subdomain
+        if not subdomain:
+            print("Error: Subdomain must be provided.")
+            return
+
+        s3_client = boto3.client(
+            's3',
+            aws_access_key_id=os.getenv('S3_ACCESS_KEY'),
+            aws_secret_access_key=os.getenv('S3_SECRET_KEY'),
+            region_name=os.getenv('S3_REGION')
+        )
+
+        local_caddyfile_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'Caddyfile')
 
-        update_caddyfile(subdomain, backend_server_port)
+        download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), os.getenv('S3_CADDY_FILENAME'), local_caddyfile_path)
+        remove_caddyfile_entry(subdomain)
         format_caddyfile()
-        upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
+        upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), os.getenv('S3_CADDY_FILENAME'), local_caddyfile_path)
         restart_caddy()
 
 if __name__ == "__main__":
     main()
```

### Comparing `cadprox-2.8/app/utils.py` & `cadprox-2.9/app/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,26 +74,30 @@
 
     wait_time = initial_wait_time
     for attempt in range(max_retries):
         response = requests.post(url, headers=headers, data=json.dumps(data))
         if response.status_code == 200:
             success_info = response.json()
             logger.info(f"Successfully added DNS record: {json.dumps(success_info, indent=2)}")
-            return
+            return True
         else:
             error_info = response.json()
+            if any(e['code'] == 81057 for e in error_info.get('errors', [])):
+                # If the record already exists, proceed without error
+                logger.info(f"DNS record for {subdomain} already exists. Continuing...")
+                return True
             logger.error(f"Failed to add DNS record: {json.dumps(error_info, indent=2)}")
             if response.status_code == 429 or any(e['code'] == 971 for e in error_info.get('errors', [])):
                 logger.info(f"Retrying in {wait_time} seconds...")
                 time.sleep(wait_time)
                 wait_time *= 2
             else:
-                sys.exit(1)
+                return False
     logger.error("Max retries exceeded. Could not add DNS record.")
-    sys.exit(1)
+    return False
 
 def download_caddyfile_from_s3(s3_client, bucket_name, s3_caddy_filename, local_caddyfile_path):
     try:
         s3_client.download_file(bucket_name, s3_caddy_filename, local_caddyfile_path)
         logger.info(f"Downloaded Caddyfile from S3 bucket {bucket_name}")
     except s3_client.exceptions.NoSuchKey:
         logger.info(f"Caddyfile {s3_caddy_filename} not found in S3 bucket {bucket_name}. Creating a new one.")
@@ -135,14 +139,32 @@
         with open(caddyfile_path, 'a') as caddy_file:
             caddy_file.write(new_entry)
         logger.info(f"Updated Caddyfile with new entry for {subdomain}")
     except PermissionError:
         logger.error(f"Permission denied when trying to write to {caddyfile_path}")
         logger.error(traceback.format_exc())
 
+def remove_caddyfile_entry(subdomain):
+    caddyfile_path = get_caddyfile_path()
+    try:
+        with open(caddyfile_path, 'r') as caddy_file:
+            content = caddy_file.read()
+        new_content = re.sub(rf"{subdomain} \{{.*?\}}\n", '', content, flags=re.DOTALL)
+        with open(caddyfile_path, 'w') as caddy_file:
+            caddy_file.write(new_content)
+        logger.info(f"Removed Caddyfile entry for {subdomain}")
+    except PermissionError:
+        logger.error(f"Permission denied when trying to modify {caddyfile_path}")
+        logger.error(traceback.format_exc())
+    except FileNotFoundError:
+        logger.error(f"Caddyfile {caddyfile_path} not found.")
+    except Exception as e:
+        logger.error(f"Error removing Caddyfile entry: {e}")
+        logger.error(traceback.format_exc())
+
 def format_caddyfile():
     caddyfile_path = get_caddyfile_path()
     result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddyfile formatted successfully")
     else:
         logger.error(f"Failed to format Caddyfile: {result.stderr}")
```

### Comparing `cadprox-2.8/cadprox.egg-info/PKG-INFO` & `cadprox-2.9/cadprox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.8
+Version: 2.9
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.8/setup.py` & `cadprox-2.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='2.8',
+    version='2.9',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

