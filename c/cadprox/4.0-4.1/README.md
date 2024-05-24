# Comparing `tmp/cadprox-4.0.tar.gz` & `tmp/cadprox-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-4.0.tar", last modified: Fri May 24 13:00:39 2024, max compression
+gzip compressed data, was "cadprox-4.1.tar", last modified: Fri May 24 13:15:51 2024, max compression
```

## Comparing `cadprox-4.0.tar` & `cadprox-4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 13:00:39.287293 cadprox-4.0/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.0/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 13:00:39.287293 cadprox-4.0/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-4.0/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 13:00:39.279292 cadprox-4.0/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.0/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     4436 2024-05-24 13:00:07.000000 cadprox-4.0/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    12983 2024-05-24 12:59:13.000000 cadprox-4.0/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 13:00:39.283292 cadprox-4.0/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 13:00:39.000000 cadprox-4.0/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 13:00:39.287293 cadprox-4.0/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1952 2024-05-24 13:00:32.000000 cadprox-4.0/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 13:15:51.201595 cadprox-4.1/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-4.1/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 13:15:51.201595 cadprox-4.1/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-4.1/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 13:15:51.193595 cadprox-4.1/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-4.1/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4416 2024-05-24 13:15:31.000000 cadprox-4.1/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    12927 2024-05-24 13:15:17.000000 cadprox-4.1/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 13:15:51.197595 cadprox-4.1/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 13:15:51.000000 cadprox-4.1/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 13:15:51.000000 cadprox-4.1/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 13:15:51.000000 cadprox-4.1/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 13:15:51.000000 cadprox-4.1/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 13:15:51.000000 cadprox-4.1/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 13:15:51.000000 cadprox-4.1/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 13:15:51.201595 cadprox-4.1/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1952 2024-05-24 13:15:46.000000 cadprox-4.1/setup.py
```

### Comparing `cadprox-4.0/PKG-INFO` & `cadprox-4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.0
+Version: 4.1
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.0/README.md` & `cadprox-4.1/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-4.0/app/main.py` & `cadprox-4.1/app/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,24 +74,24 @@
         if check_port_in_use(backend_server_port):
             print(f"Warning: Port {backend_server_port} is already in use.")
             # Continue without exiting
 
         if add_dns_record(subdomain, external_ip, api_token, zone_id):
             wait_until_resolvable(subdomain)
 
-            local_caddyfile_path = os.path.join(os.getcwd(), s3_caddy_filename)
+            local_caddyfile_path = get_caddyfile_path(docker)
 
             download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
 
             if check_domain_exists(subdomain, local_caddyfile_path):
                 print(f"Error: Domain {subdomain} already exists in the Caddy configuration.")
                 sys.exit(1)
 
             update_caddyfile(subdomain, backend_server_port, local_caddyfile_path)
-            format_caddyfile(local_caddyfile_path)
+            format_caddyfile(local_caddyfile_path, docker)
             upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
             restart_caddy(local_caddyfile_path, docker)
 
     if args.command in ['remove', 'docker_remove']:
         subdomain = args.subdomain
         docker = args.command == 'docker_remove'
         if not subdomain:
@@ -102,17 +102,17 @@
             's3',
             aws_access_key_id=os.getenv('S3_ACCESS_KEY'),
             aws_secret_access_key=os.getenv('S3_SECRET_KEY'),
             region_name=os.getenv('S3_REGION')
         )
 
         s3_caddy_filename = 'Caddyfile_docker' if docker else 'Caddyfile'
-        local_caddyfile_path = os.path.join(os.getcwd(), s3_caddy_filename)
+        local_caddyfile_path = get_caddyfile_path(docker)
 
         download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
         remove_caddyfile_entry(subdomain, local_caddyfile_path)
-        format_caddyfile(local_caddyfile_path)
+        format_caddyfile(local_caddyfile_path, docker)
         upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
         restart_caddy(local_caddyfile_path, docker)
 
 if __name__ == "__main__":
     main()
```

### Comparing `cadprox-4.0/app/utils.py` & `cadprox-4.1/app/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,30 +145,30 @@
         logger.error("Incomplete AWS credentials provided.")
         sys.exit(1)
     except Exception as e:
         logger.error(f"Error uploading Caddyfile to S3: {e}")
         logger.error(traceback.format_exc())
         sys.exit(1)
 
-def get_caddyfile_path():
+def get_caddyfile_path(docker=False):
+    if docker:
+        return os.path.join(os.getcwd(), 'Caddyfile_docker')
     return os.path.join(os.getcwd(), 'Caddyfile')
 
 def update_caddyfile(subdomain, port, caddyfile_path=None):
-    caddyfile_path = caddyfile_path or get_caddyfile_path()
     new_entry = f"{subdomain} {{\n    reverse_proxy localhost:{port}\n}}\n"
     try:
         with open(caddyfile_path, 'a') as caddy_file:
             caddy_file.write(new_entry)
         logger.info(f"Updated Caddyfile with new entry for {subdomain}")
     except PermissionError:
         logger.error(f"Permission denied when trying to write to {caddyfile_path}")
         logger.error(traceback.format_exc())
 
 def remove_caddyfile_entry(subdomain, caddyfile_path=None):
-    caddyfile_path = caddyfile_path or get_caddyfile_path()
     try:
         with open(caddyfile_path, 'r') as caddy_file:
             content = caddy_file.read()
         new_content = re.sub(rf"{subdomain} \{{.*?\}}\n", '', content, flags=re.DOTALL)
         with open(caddyfile_path, 'w') as caddy_file:
             caddy_file.write(new_content)
         logger.info(f"Removed Caddyfile entry for {subdomain}")
@@ -187,26 +187,26 @@
     else:
         format_caddyfile_system(caddyfile_path)
 
 def restart_caddy(caddyfile_path=None, docker=False):
     if docker:
         restart_caddy_docker(caddyfile_path)
     else:
-        restart_caddy_system()
+        restart_caddy_system(caddyfile_path)
 
 def is_caddy_running_in_docker():
     try:
         result = subprocess.run(['docker', 'ps', '--filter', 'name=caddy', '--format', '{{.Names}}'], capture_output=True, text=True)
         return 'caddy' in result.stdout.strip().split('\n')
     except Exception as e:
         logger.error(f"Error checking Docker containers: {e}")
         return False
 
 def format_caddyfile_docker(caddyfile_path=None):
-    caddyfile_path = caddyfile_path or get_caddyfile_path()
+    caddyfile_path = caddyfile_path or get_caddyfile_path(docker=True)
     result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddyfile formatted successfully within Docker")
     else:
         logger.error(f"Failed to format Caddyfile within Docker: {result.stderr}")
 
 def format_caddyfile_system(caddyfile_path=None):
@@ -214,15 +214,15 @@
     result = subprocess.run(['caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddyfile formatted successfully")
     else:
         logger.error(f"Failed to format Caddyfile: {result.stderr}")
 
 def restart_caddy_docker(caddyfile_path=None):
-    caddyfile_path = caddyfile_path or get_caddyfile_path()
+    caddyfile_path = caddyfile_path or get_caddyfile_path(docker=True)
     result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'reload', '--config', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddy server reloaded successfully within Docker")
     else:
         logger.error(f"Failed to reload Caddy server in Docker: {result.stderr}")
 
 def restart_caddy_system(caddyfile_path=None):
@@ -234,15 +234,14 @@
         logger.error(f"Failed to reload Caddy server: {result.stderr}")
 
 def check_port_in_use(port):
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
         return sock.connect_ex(('localhost', int(port))) == 0
 
 def check_domain_exists(subdomain, caddyfile_path=None):
-    caddyfile_path = caddyfile_path or get_caddyfile_path()
     try:
         with open(caddyfile_path, 'r') as caddy_file:
             content = caddy_file.read()
             return re.search(rf"{subdomain} \{{.*?\}}", content, flags=re.DOTALL) is not None
     except FileNotFoundError:
         logger.error(f"Caddyfile {caddyfile_path} not found.")
         return False
```

### Comparing `cadprox-4.0/cadprox.egg-info/PKG-INFO` & `cadprox-4.1/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 4.0
+Version: 4.1
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-4.0/setup.py` & `cadprox-4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         print("Please ensure Docker is installed and the Caddy container is running if you intend to use Docker-based Caddy.")
         # Do not exit since system Caddy may still be used
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='4.0',
+    version='4.1',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

