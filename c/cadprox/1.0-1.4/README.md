# Comparing `tmp/cadprox-1.0.tar.gz` & `tmp/cadprox-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-1.0.tar", last modified: Fri May 24 03:41:41 2024, max compression
+gzip compressed data, was "cadprox-1.4.tar", last modified: Fri May 24 04:01:29 2024, max compression
```

## Comparing `cadprox-1.0.tar` & `cadprox-1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 03:41:41.481979 cadprox-1.0/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-1.0/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 03:41:41.481979 cadprox-1.0/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      287 2024-05-24 03:13:51.000000 cadprox-1.0/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 03:41:41.477978 cadprox-1.0/cadprox/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-1.0/cadprox/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-1.0/cadprox/config.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3248 2024-05-24 03:28:42.000000 cadprox-1.0/cadprox/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     7926 2024-05-24 03:28:53.000000 cadprox-1.0/cadprox/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 03:41:41.481979 cadprox-1.0/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 03:41:41.000000 cadprox-1.0/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      285 2024-05-24 03:41:41.000000 cadprox-1.0/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 03:41:41.000000 cadprox-1.0/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       46 2024-05-24 03:41:41.000000 cadprox-1.0/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 03:41:41.000000 cadprox-1.0/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        8 2024-05-24 03:41:41.000000 cadprox-1.0/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 03:41:41.481979 cadprox-1.0/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)      946 2024-05-24 03:28:30.000000 cadprox-1.0/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:01:29.448024 cadprox-1.4/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-1.4/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:01:29.448024 cadprox-1.4/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      287 2024-05-24 03:13:51.000000 cadprox-1.4/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:01:29.444024 cadprox-1.4/cadprox/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-1.4/cadprox/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-1.4/cadprox/config.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     7922 2024-05-24 03:57:25.000000 cadprox-1.4/cadprox/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     7922 2024-05-24 04:01:13.000000 cadprox-1.4/cadprox/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:01:29.448024 cadprox-1.4/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:01:29.000000 cadprox-1.4/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      285 2024-05-24 04:01:29.000000 cadprox-1.4/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 04:01:29.000000 cadprox-1.4/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       46 2024-05-24 04:01:29.000000 cadprox-1.4/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 04:01:29.000000 cadprox-1.4/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        8 2024-05-24 04:01:29.000000 cadprox-1.4/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 04:01:29.452024 cadprox-1.4/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)      905 2024-05-24 03:59:36.000000 cadprox-1.4/setup.py
```

### Comparing `cadprox-1.0/PKG-INFO` & `cadprox-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 1.0
+Version: 1.4
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadprox
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-1.0/cadprox/utils.py` & `cadprox-1.4/cadprox/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 
 S3_ACCESS_KEY = os.getenv('S3_ACCESS_KEY')
 S3_SECRET_KEY = os.getenv('S3_SECRET_KEY')
 S3_REGION = os.getenv('S3_REGION')
 S3_BUCKET = os.getenv('S3_BUCKET')
 S3_CADDY_FILENAME = os.getenv('S3_CADDY_FILENAME', 'Caddyfile')
 
+def load_s3_client():
+    return boto3.client(
+        's3',
+        aws_access_key_id=S3_ACCESS_KEY,
+        aws_secret_access_key=S3_SECRET_KEY,
+        region_name=S3_REGION
+    )
+
 def get_external_ip():
     try:
         response = requests.get('https://api.ipify.org?format=json')
         response.raise_for_status()
         return response.json()['ip']
     except requests.RequestException as e:
         logger.error(f"Error retrieving external IP address: {e}")
@@ -172,18 +180,14 @@
         logger.error(f"Error loading profiles: {e}")
         return {}
 
 def prompt_for_profile():
     profile = {
         "CLOUDFLARE_API_TOKEN": input("CLOUDFLARE_API_TOKEN: "),
         "CLOUDFLARE_ZONE_ID": input("CLOUDFLARE_ZONE_ID: "),
-        "S3_ACCESS_KEY": input("S3_ACCESS_KEY: "),
-        "S3_SECRET_KEY": input("S3_SECRET_KEY: "),
-        "S3_REGION": input("S3_REGION: "),
-        "S3_BUCKET": input("S3_BUCKET: "),
         "S3_CADDY_FILENAME": input("S3_CADDY_FILENAME: "),
         "MAIN_DOMAIN": input("MAIN_DOMAIN: ")
     }
     return profile
 
 def create_profile(profile_name):
     profile = prompt_for_profile()
```

### Comparing `cadprox-1.0/cadprox.egg-info/PKG-INFO` & `cadprox-1.4/cadprox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 1.0
+Version: 1.4
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadprox
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-1.0/setup.py` & `cadprox-1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cadprox',
-    version='1.0',  # Starting new version for this project
+    version='1.4',
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadprox',  # Update with your GitHub repository URL
     packages=find_packages(),
```

