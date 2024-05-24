# Comparing `tmp/cadprox-3.tar.gz` & `tmp/cadprox-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-3.tar", last modified: Fri May 24 11:11:25 2024, max compression
+gzip compressed data, was "cadprox-3.1.tar", last modified: Fri May 24 11:15:42 2024, max compression
```

## Comparing `cadprox-3.tar` & `cadprox-3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:11:25.605301 cadprox-3/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4487 2024-05-24 11:11:25.601301 cadprox-3/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:11:25.597301 cadprox-3/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3822 2024-05-24 11:11:00.000000 cadprox-3/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    10078 2024-05-24 11:08:21.000000 cadprox-3/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:11:25.601301 cadprox-3/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4487 2024-05-24 11:11:25.000000 cadprox-3/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:11:25.000000 cadprox-3/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:11:25.000000 cadprox-3/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:11:25.000000 cadprox-3/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:11:25.000000 cadprox-3/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:11:25.000000 cadprox-3/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:11:25.605301 cadprox-3/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1678 2024-05-24 11:11:21.000000 cadprox-3/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:15:42.523282 cadprox-3.1/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.1/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:15:42.523282 cadprox-3.1/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.1/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:15:42.515282 cadprox-3.1/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.1/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3847 2024-05-24 11:15:13.000000 cadprox-3.1/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    10097 2024-05-24 11:14:53.000000 cadprox-3.1/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:15:42.523282 cadprox-3.1/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:15:42.000000 cadprox-3.1/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:15:42.523282 cadprox-3.1/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:15:33.000000 cadprox-3.1/setup.py
```

### Comparing `cadprox-3/PKG-INFO` & `cadprox-3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3
+Version: 3.1
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3/README.md` & `cadprox-3.1/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-3/app/main.py` & `cadprox-3.1/app/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 
         external_ip = get_external_ip()
         if not external_ip:
             print("Failed to retrieve external IP address.")
             sys.exit(1)
 
         if check_port_in_use(backend_server_port):
-            print(f"Error: Port {backend_server_port} active.OK")
-            #sys.exit(1)
+            print(f"Warning: Port {backend_server_port} is already in use.")
+            # Continue without exiting
 
         if add_dns_record(subdomain, external_ip, api_token, zone_id):
             wait_until_resolvable(subdomain)
 
             local_caddyfile_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'Caddyfile')
 
             download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
```

### Comparing `cadprox-3/app/utils.py` & `cadprox-3.1/app/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 S3_ACCESS_KEY = os.getenv('S3_ACCESS_KEY')
 S3_SECRET_KEY = os.getenv('S3_SECRET_KEY')
 S3_REGION = os.getenv('S3_REGION')
 S3_BUCKET = os.getenv('S3_BUCKET')
 S3_CADDY_FILENAME = os.getenv('S3_CADDY_FILENAME', 'Caddyfile')
 
 # Validate environment variables
-if not all([S3_ACCESS_KEY, S3_SECRET_KEY, S3_REGION, S3_BUCKET]):
+if not all([S3_ACCESS_KEY, S3_SECRET_KEY, S3_REGION, S3_BUCKET, S3_CADDY_FILENAME]):
     logger.error("One or more required environment variables are missing or not loaded correctly.")
     sys.exit(1)
 
 os.environ['S3_ACCESS_KEY'] = S3_ACCESS_KEY
 os.environ['S3_SECRET_KEY'] = S3_SECRET_KEY
 os.environ['S3_REGION'] = S3_REGION
 os.environ['S3_BUCKET'] = S3_BUCKET
```

### Comparing `cadprox-3/cadprox.egg-info/PKG-INFO` & `cadprox-3.1/cadprox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3
+Version: 3.1
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3/setup.py` & `cadprox-3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='3',
+    version='3.1',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

