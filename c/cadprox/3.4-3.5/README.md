# Comparing `tmp/cadprox-3.4.tar.gz` & `tmp/cadprox-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-3.4.tar", last modified: Fri May 24 11:35:31 2024, max compression
+gzip compressed data, was "cadprox-3.5.tar", last modified: Fri May 24 11:40:57 2024, max compression
```

## Comparing `cadprox-3.4.tar` & `cadprox-3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:35:31.802557 cadprox-3.4/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.4/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:35:31.802557 cadprox-3.4/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.4/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:35:31.794557 cadprox-3.4/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.4/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3847 2024-05-24 11:34:32.000000 cadprox-3.4/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    11188 2024-05-24 11:34:06.000000 cadprox-3.4/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:35:31.798557 cadprox-3.4/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:35:31.000000 cadprox-3.4/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:35:31.802557 cadprox-3.4/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:35:15.000000 cadprox-3.4/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:40:57.129932 cadprox-3.5/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.5/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:40:57.129932 cadprox-3.5/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.5/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:40:57.125933 cadprox-3.5/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.5/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3925 2024-05-24 11:40:33.000000 cadprox-3.5/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    11188 2024-05-24 11:34:06.000000 cadprox-3.5/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:40:57.129932 cadprox-3.5/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:40:57.000000 cadprox-3.5/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:40:57.129932 cadprox-3.5/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:40:48.000000 cadprox-3.5/setup.py
```

### Comparing `cadprox-3.4/PKG-INFO` & `cadprox-3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.4
+Version: 3.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.4/README.md` & `cadprox-3.5/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-3.4/app/main.py` & `cadprox-3.5/app/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,16 @@
         if not profile:
             print(f"Error: No profile found for main domain '{main_domain}'.")
             return
 
         api_token = profile['CLOUDFLARE_API_TOKEN']
         zone_id = profile['CLOUDFLARE_ZONE_ID']
         s3_caddy_filename = profile['S3_CADDY_FILENAME']
+        if not s3_caddy_filename:
+            s3_caddy_filename = 'Caddyfile'
 
         external_ip = get_external_ip()
         if not external_ip:
             print("Failed to retrieve external IP address.")
             sys.exit(1)
 
         if check_port_in_use(backend_server_port):
```

### Comparing `cadprox-3.4/app/utils.py` & `cadprox-3.5/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadprox-3.4/cadprox.egg-info/PKG-INFO` & `cadprox-3.5/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.4
+Version: 3.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.4/setup.py` & `cadprox-3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='3.4',
+    version='3.5',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

