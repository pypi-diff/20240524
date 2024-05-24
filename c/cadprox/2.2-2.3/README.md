# Comparing `tmp/cadprox-2.2.tar.gz` & `tmp/cadprox-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-2.2.tar", last modified: Fri May 24 10:32:13 2024, max compression
+gzip compressed data, was "cadprox-2.3.tar", last modified: Fri May 24 10:37:29 2024, max compression
```

## Comparing `cadprox-2.2.tar` & `cadprox-2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:32:13.096797 cadprox-2.2/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.2/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:32:13.096797 cadprox-2.2/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.2/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:32:13.092797 cadprox-2.2/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.2/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2977 2024-05-24 10:26:04.000000 cadprox-2.2/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8538 2024-05-24 10:30:44.000000 cadprox-2.2/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:32:13.096797 cadprox-2.2/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:32:13.000000 cadprox-2.2/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:32:13.096797 cadprox-2.2/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1773 2024-05-24 10:31:48.000000 cadprox-2.2/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:37:29.934663 cadprox-2.3/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.3/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:37:29.934663 cadprox-2.3/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.3/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:37:29.926663 cadprox-2.3/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.3/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2977 2024-05-24 10:26:04.000000 cadprox-2.3/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8789 2024-05-24 10:35:46.000000 cadprox-2.3/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:37:29.930663 cadprox-2.3/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:37:29.000000 cadprox-2.3/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:37:29.934663 cadprox-2.3/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1773 2024-05-24 10:37:22.000000 cadprox-2.3/setup.py
```

### Comparing `cadprox-2.2/PKG-INFO` & `cadprox-2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.2
+Version: 2.3
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.2/README.md` & `cadprox-2.3/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-2.2/app/main.py` & `cadprox-2.3/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-2.2/app/utils.py` & `cadprox-2.3/app/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 
 S3_ACCESS_KEY = os.getenv('S3_ACCESS_KEY')
 S3_SECRET_KEY = os.getenv('S3_SECRET_KEY')
 S3_REGION = os.getenv('S3_REGION')
 S3_BUCKET = os.getenv('S3_BUCKET')
 S3_CADDY_FILENAME = os.getenv('S3_CADDY_FILENAME', 'Caddyfile')
 
+# Validate that none of the required environment variables are None
+if not all([S3_ACCESS_KEY, S3_SECRET_KEY, S3_REGION, S3_BUCKET]):
+    logger.error("One or more required environment variables are missing or not loaded correctly.")
+    sys.exit(1)
+
 def load_s3_client():
     return boto3.client(
         's3',
         aws_access_key_id=S3_ACCESS_KEY,
         aws_secret_access_key=S3_SECRET_KEY,
         region_name=S3_REGION
     )
```

### Comparing `cadprox-2.2/cadprox.egg-info/PKG-INFO` & `cadprox-2.3/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.2
+Version: 2.3
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.2/setup.py` & `cadprox-2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='2.2',  # Increment the version number
+    version='2.3',  # Increment the version number
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',  # Update with your GitHub repository URL
     packages=find_packages(),
```

