# Comparing `tmp/cadprox-2.7.tar.gz` & `tmp/cadprox-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-2.7.tar", last modified: Fri May 24 10:54:54 2024, max compression
+gzip compressed data, was "cadprox-2.8.tar", last modified: Fri May 24 10:57:59 2024, max compression
```

## Comparing `cadprox-2.7.tar` & `cadprox-2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:54:54.575514 cadprox-2.7/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.7/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:54:54.575514 cadprox-2.7/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.7/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:54:54.567514 cadprox-2.7/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.7/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2892 2024-05-24 10:54:26.000000 cadprox-2.7/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8992 2024-05-24 10:54:12.000000 cadprox-2.7/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:54:54.575514 cadprox-2.7/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:54:54.000000 cadprox-2.7/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:54:54.575514 cadprox-2.7/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 10:54:42.000000 cadprox-2.7/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:57:59.356233 cadprox-2.8/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.8/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:57:59.356233 cadprox-2.8/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-2.8/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:57:59.352233 cadprox-2.8/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.8/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2888 2024-05-24 10:57:21.000000 cadprox-2.8/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8992 2024-05-24 10:54:12.000000 cadprox-2.8/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 10:57:59.356233 cadprox-2.8/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 10:57:59.000000 cadprox-2.8/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 10:57:59.356233 cadprox-2.8/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 10:57:36.000000 cadprox-2.8/setup.py
```

### Comparing `cadprox-2.7/PKG-INFO` & `cadprox-2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.7
+Version: 2.8
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.7/README.md` & `cadprox-2.8/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-2.7/app/main.py` & `cadprox-2.8/app/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 
         external_ip = get_external_ip()
         if not external_ip:
             print("Failed to retrieve external IP address.")
             sys.exit(1)
 
         if check_port_in_use(backend_server_port):
-            print(f"Error: Port {backend_server_port} is already in use.")
-            sys.exit(1)
+            print(f"Error: Port {backend_server_port} is active. OK")
+            #sys.exit(1)
 
         add_dns_record(subdomain, external_ip, api_token, zone_id)
         wait_until_resolvable(subdomain)
 
         local_caddyfile_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', 'Caddyfile')
 
         download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
```

### Comparing `cadprox-2.7/app/utils.py` & `cadprox-2.8/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadprox-2.7/cadprox.egg-info/PKG-INFO` & `cadprox-2.8/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 2.7
+Version: 2.8
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-2.7/setup.py` & `cadprox-2.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='2.7',
+    version='2.8',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

