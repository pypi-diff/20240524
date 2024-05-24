# Comparing `tmp/cadprox-3.1.tar.gz` & `tmp/cadprox-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-3.1.tar", last modified: Fri May 24 11:15:42 2024, max compression
+gzip compressed data, was "cadprox-3.2.tar", last modified: Fri May 24 11:22:03 2024, max compression
```

## Comparing `cadprox-3.1.tar` & `cadprox-3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:15:42.523282 cadprox-3.1/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.1/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:15:42.523282 cadprox-3.1/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.1/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:15:42.515282 cadprox-3.1/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.1/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3847 2024-05-24 11:15:13.000000 cadprox-3.1/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    10097 2024-05-24 11:14:53.000000 cadprox-3.1/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:15:42.523282 cadprox-3.1/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:15:42.523282 cadprox-3.1/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:15:33.000000 cadprox-3.1/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:22:03.980337 cadprox-3.2/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.2/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:22:03.980337 cadprox-3.2/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.2/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:22:03.972337 cadprox-3.2/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.2/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3847 2024-05-24 11:21:30.000000 cadprox-3.2/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    10478 2024-05-24 11:21:14.000000 cadprox-3.2/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:22:03.980337 cadprox-3.2/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:22:03.000000 cadprox-3.2/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:22:03.980337 cadprox-3.2/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:21:55.000000 cadprox-3.2/setup.py
```

### Comparing `cadprox-3.1/PKG-INFO` & `cadprox-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.1
+Version: 3.2
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.1/README.md` & `cadprox-3.2/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-3.1/app/main.py` & `cadprox-3.2/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-3.1/app/utils.py` & `cadprox-3.2/app/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,49 +54,56 @@
         response = requests.get('https://api.ipify.org?format=json')
         response.raise_for_status()
         return response.json()['ip']
     except requests.RequestException as e:
         logger.error(f"Error retrieving external IP address: {e}")
         return None
 
-def add_dns_record(subdomain, ip_address, api_token, zone_id, max_retries=5, initial_wait_time=5):
+def add_dns_record(subdomain, ip_address, api_token, zone_id, max_retries=1, initial_wait_time=5):
     url = f"https://api.cloudflare.com/client/v4/zones/{zone_id}/dns_records"
     headers = {
         'Authorization': f"Bearer {api_token}",
         'Content-Type': 'application/json'
     }
     data = {
         'type': 'A',
         'name': subdomain,
         'content': ip_address,
         'ttl': 120,
         'proxied': True
     }
 
     wait_time = initial_wait_time
-    for attempt in range(max_retries):
+    for attempt in range(max_retries + 1):
         response = requests.post(url, headers=headers, data=json.dumps(data))
         if response.status_code == 200:
             success_info = response.json()
             logger.info(f"Successfully added DNS record: {json.dumps(success_info, indent=2)}")
             return True
         else:
             error_info = response.json()
             if any(e['code'] == 81057 for e in error_info.get('errors', [])):
                 # If the record already exists, proceed without error
                 logger.info(f"DNS record for {subdomain} already exists. Continuing...")
                 return True
             logger.error(f"Failed to add DNS record: {json.dumps(error_info, indent=2)}")
             if response.status_code == 429 or any(e['code'] == 971 for e in error_info.get('errors', [])):
-                logger.info(f"Retrying in {wait_time} seconds...")
-                time.sleep(wait_time)
-                wait_time *= 2
+                if attempt < max_retries:
+                    logger.info(f"Retrying in {wait_time} seconds...")
+                    time.sleep(wait_time)
+                    wait_time *= 2
+                else:
+                    logger.warning("Max retries exceeded or throttling issue. Please consider throttling your request speed.")
+                    user_input = input("Add host to Caddyfile anyway? (yes/no): ").strip().lower()
+                    if user_input == 'yes':
+                        return True
+                    else:
+                        return False
             else:
                 return False
-    logger.error("Max retries exceeded. Could not add DNS record.")
     return False
 
 def download_caddyfile_from_s3(s3_client, bucket_name, s3_caddy_filename, local_caddyfile_path):
     try:
         s3_client.download_file(bucket_name, s3_caddy_filename, local_caddyfile_path)
         logger.info(f"Downloaded Caddyfile from S3 bucket {bucket_name}")
     except s3_client.exceptions.NoSuchKey:
```

### Comparing `cadprox-3.1/cadprox.egg-info/PKG-INFO` & `cadprox-3.2/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.1
+Version: 3.2
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.1/setup.py` & `cadprox-3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='3.1',
+    version='3.2',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

