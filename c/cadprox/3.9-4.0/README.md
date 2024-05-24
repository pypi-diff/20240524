# Comparing `tmp/cadprox-3.9.tar.gz` & `tmp/cadprox-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-3.9.tar", last modified: Fri May 24 12:47:51 2024, max compression
+gzip compressed data, was "cadprox-4.0.tar", last modified: Fri May 24 13:00:39 2024, max compression
```

## Comparing `cadprox-3.9.tar` & `cadprox-4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:47:51.063850 cadprox-3.9/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.9/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:47:51.059849 cadprox-3.9/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.9/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:47:51.051849 cadprox-3.9/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.9/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     4420 2024-05-24 12:31:50.000000 cadprox-3.9/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    12900 2024-05-24 12:47:26.000000 cadprox-3.9/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:47:51.059849 cadprox-3.9/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 12:47:50.000000 cadprox-3.9/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 12:47:51.063850 cadprox-3.9/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1952 2024-05-24 12:47:44.000000 cadprox-3.9/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 13:00:39.287293 cadprox-4.0/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.0/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 13:00:39.287293 cadprox-4.0/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-4.0/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 13:00:39.279292 cadprox-4.0/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.0/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4436 2024-05-24 13:00:07.000000 cadprox-4.0/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    12983 2024-05-24 12:59:13.000000 cadprox-4.0/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 13:00:39.283292 cadprox-4.0/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 13:00:39.287293 cadprox-4.0/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1952 2024-05-24 13:00:32.000000 cadprox-4.0/setup.py
```

### Comparing `cadprox-3.9/PKG-INFO` & `cadprox-4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.9
+Version: 4.0
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.9/README.md` & `cadprox-4.0/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-3.9/app/main.py` & `cadprox-4.0/app/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             if check_domain_exists(subdomain, local_caddyfile_path):
                 print(f"Error: Domain {subdomain} already exists in the Caddy configuration.")
                 sys.exit(1)
 
             update_caddyfile(subdomain, backend_server_port, local_caddyfile_path)
             format_caddyfile(local_caddyfile_path)
             upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
-            restart_caddy(local_caddyfile_path)
+            restart_caddy(local_caddyfile_path, docker)
 
     if args.command in ['remove', 'docker_remove']:
         subdomain = args.subdomain
         docker = args.command == 'docker_remove'
         if not subdomain:
             print("Error: Subdomain must be provided.")
             return
@@ -108,11 +108,11 @@
         s3_caddy_filename = 'Caddyfile_docker' if docker else 'Caddyfile'
         local_caddyfile_path = os.path.join(os.getcwd(), s3_caddy_filename)
 
         download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
         remove_caddyfile_entry(subdomain, local_caddyfile_path)
         format_caddyfile(local_caddyfile_path)
         upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
-        restart_caddy(local_caddyfile_path)
+        restart_caddy(local_caddyfile_path, docker)
 
 if __name__ == "__main__":
     main()
```

### Comparing `cadprox-3.9/app/utils.py` & `cadprox-4.0/app/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,22 +177,22 @@
         logger.error(traceback.format_exc())
     except FileNotFoundError:
         logger.error(f"Caddyfile {caddyfile_path} not found.")
     except Exception as e:
         logger.error(f"Error removing Caddyfile entry: {e}")
         logger.error(traceback.format_exc())
 
-def format_caddyfile(caddyfile_path=None):
-    if is_caddy_running_in_docker():
+def format_caddyfile(caddyfile_path=None, docker=False):
+    if docker:
         format_caddyfile_docker(caddyfile_path)
     else:
         format_caddyfile_system(caddyfile_path)
 
-def restart_caddy(caddyfile_path=None):
-    if is_caddy_running_in_docker():
+def restart_caddy(caddyfile_path=None, docker=False):
+    if docker:
         restart_caddy_docker(caddyfile_path)
     else:
         restart_caddy_system()
 
 def is_caddy_running_in_docker():
     try:
         result = subprocess.run(['docker', 'ps', '--filter', 'name=caddy', '--format', '{{.Names}}'], capture_output=True, text=True)
@@ -221,16 +221,17 @@
     caddyfile_path = caddyfile_path or get_caddyfile_path()
     result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'reload', '--config', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddy server reloaded successfully within Docker")
     else:
         logger.error(f"Failed to reload Caddy server in Docker: {result.stderr}")
 
-def restart_caddy_system():
-    result = subprocess.run(['sudo', 'caddy', 'reload'], capture_output=True, text=True)
+def restart_caddy_system(caddyfile_path=None):
+    caddyfile_path = caddyfile_path or get_caddyfile_path()
+    result = subprocess.run(['caddy', 'reload', '--config', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddy server reloaded successfully")
     else:
         logger.error(f"Failed to reload Caddy server: {result.stderr}")
 
 def check_port_in_use(port):
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
```

### Comparing `cadprox-3.9/cadprox.egg-info/PKG-INFO` & `cadprox-4.0/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.9
+Version: 4.0
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.9/setup.py` & `cadprox-4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         print("Please ensure Docker is installed and the Caddy container is running if you intend to use Docker-based Caddy.")
         # Do not exit since system Caddy may still be used
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='3.9',
+    version='4.0',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

