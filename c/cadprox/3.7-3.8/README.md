# Comparing `tmp/cadprox-3.7.tar.gz` & `tmp/cadprox-3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-3.7.tar", last modified: Fri May 24 12:02:35 2024, max compression
+gzip compressed data, was "cadprox-3.8.tar", last modified: Fri May 24 12:34:45 2024, max compression
```

## Comparing `cadprox-3.7.tar` & `cadprox-3.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:02:35.679213 cadprox-3.7/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.7/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:02:35.679213 cadprox-3.7/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.7/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:02:35.675213 cadprox-3.7/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.7/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3868 2024-05-24 11:45:26.000000 cadprox-3.7/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    12294 2024-05-24 12:02:17.000000 cadprox-3.7/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:02:35.679213 cadprox-3.7/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 12:02:35.679213 cadprox-3.7/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 12:02:29.000000 cadprox-3.7/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:34:45.959349 cadprox-3.8/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.8/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:34:45.959349 cadprox-3.8/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.8/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:34:45.951348 cadprox-3.8/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.8/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4420 2024-05-24 12:31:50.000000 cadprox-3.8/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    12683 2024-05-24 12:31:03.000000 cadprox-3.8/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:34:45.955349 cadprox-3.8/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 12:34:45.000000 cadprox-3.8/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 12:34:45.959349 cadprox-3.8/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1952 2024-05-24 12:34:22.000000 cadprox-3.8/setup.py
```

### Comparing `cadprox-3.7/PKG-INFO` & `cadprox-3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.7
+Version: 3.8
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.7/README.md` & `cadprox-3.8/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-3.7/app/main.py` & `cadprox-3.8/app/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,99 +16,103 @@
     wait_until_resolvable,
     load_profiles,
     create_profile
 )
 
 def main():
     parser = argparse.ArgumentParser(description='CADProxy Command Line Tool')
-    parser.add_argument('command', choices=['add', 'create', 'remove'], help='Command to execute')
+    parser.add_argument('command', choices=['add', 'create', 'remove', 'docker_add', 'docker_create', 'docker_remove'], help='Command to execute')
     parser.add_argument('subdomain', help='Subdomain to add or remove', nargs='?')
     parser.add_argument('-p', '--port', required=False, help='Backend server port')
 
     args = parser.parse_args()
 
-    if args.command == 'create':
+    if args.command == 'create' or args.command == 'docker_create':
         profile_name = args.subdomain
+        docker = args.command == 'docker_create'
         if profile_name:
-            create_profile(profile_name)
+            create_profile(profile_name, docker)
         else:
             print("Error: Profile name must be provided.")
         return
 
-    if args.command == 'add':
+    if args.command in ['add', 'docker_add']:
         if not args.subdomain or not args.port:
             print("Error: Subdomain and port must be provided.")
             return
 
         subdomain = args.subdomain
         backend_server_port = args.port
+        docker = args.command == 'docker_add'
 
         s3_client = boto3.client(
             's3',
             aws_access_key_id=os.getenv('S3_ACCESS_KEY'),
             aws_secret_access_key=os.getenv('S3_SECRET_KEY'),
             region_name=os.getenv('S3_REGION')
         )
 
-        profiles = load_profiles(s3_client)
+        profiles = load_profiles(s3_client, docker)
         main_domain = ".".join(subdomain.split(".")[-2:])
 
         profile = profiles.get(main_domain)
 
         if not profile:
             print(f"Error: No profile found for main domain '{main_domain}'.")
             return
 
         api_token = profile['CLOUDFLARE_API_TOKEN']
         zone_id = profile['CLOUDFLARE_ZONE_ID']
-        s3_caddy_filename = profile.get('S3_CADDY_FILENAME', 'Caddyfile')
+        s3_caddy_filename = profile.get('S3_CADDY_FILENAME', 'Caddyfile_docker' if docker else 'Caddyfile')
         if not s3_caddy_filename:
-            s3_caddy_filename = 'Caddyfile'
+            s3_caddy_filename = 'Caddyfile_docker' if docker else 'Caddyfile'
 
         external_ip = get_external_ip()
         if not external_ip:
             print("Failed to retrieve external IP address.")
             sys.exit(1)
 
         if check_port_in_use(backend_server_port):
             print(f"Warning: Port {backend_server_port} is already in use.")
             # Continue without exiting
 
         if add_dns_record(subdomain, external_ip, api_token, zone_id):
             wait_until_resolvable(subdomain)
 
-            local_caddyfile_path = os.path.join(os.getcwd(), 'Caddyfile')
+            local_caddyfile_path = os.path.join(os.getcwd(), s3_caddy_filename)
 
             download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
 
-            if check_domain_exists(subdomain):
+            if check_domain_exists(subdomain, local_caddyfile_path):
                 print(f"Error: Domain {subdomain} already exists in the Caddy configuration.")
                 sys.exit(1)
 
-            update_caddyfile(subdomain, backend_server_port)
-            format_caddyfile()
+            update_caddyfile(subdomain, backend_server_port, local_caddyfile_path)
+            format_caddyfile(local_caddyfile_path)
             upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
-            restart_caddy()
+            restart_caddy(local_caddyfile_path)
 
-    if args.command == 'remove':
+    if args.command in ['remove', 'docker_remove']:
         subdomain = args.subdomain
+        docker = args.command == 'docker_remove'
         if not subdomain:
             print("Error: Subdomain must be provided.")
             return
 
         s3_client = boto3.client(
             's3',
             aws_access_key_id=os.getenv('S3_ACCESS_KEY'),
             aws_secret_access_key=os.getenv('S3_SECRET_KEY'),
             region_name=os.getenv('S3_REGION')
         )
 
-        local_caddyfile_path = os.path.join(os.getcwd(), 'Caddyfile')
+        s3_caddy_filename = 'Caddyfile_docker' if docker else 'Caddyfile'
+        local_caddyfile_path = os.path.join(os.getcwd(), s3_caddy_filename)
 
-        download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), os.getenv('S3_CADDY_FILENAME'), local_caddyfile_path)
-        remove_caddyfile_entry(subdomain)
-        format_caddyfile()
-        upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), os.getenv('S3_CADDY_FILENAME'), local_caddyfile_path)
-        restart_caddy()
+        download_caddyfile_from_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
+        remove_caddyfile_entry(subdomain, local_caddyfile_path)
+        format_caddyfile(local_caddyfile_path)
+        upload_caddyfile_to_s3(s3_client, os.getenv('S3_BUCKET'), s3_caddy_filename, local_caddyfile_path)
+        restart_caddy(local_caddyfile_path)
 
 if __name__ == "__main__":
     main()
```

### Comparing `cadprox-3.7/app/utils.py` & `cadprox-3.8/app/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,23 +34,22 @@
 logger.info(f"S3_ACCESS_KEY: {S3_ACCESS_KEY}")
 logger.info(f"S3_SECRET_KEY: {S3_SECRET_KEY}")
 logger.info(f"S3_REGION: {S3_REGION}")
 logger.info(f"S3_BUCKET: {S3_BUCKET}")
 logger.info(f"S3_CADDY_FILENAME: {S3_CADDY_FILENAME}")
 
 # Validate environment variables
-if not all([S3_ACCESS_KEY, S3_SECRET_KEY, S3_REGION, S3_BUCKET, S3_CADDY_FILENAME]):
+if not all([S3_ACCESS_KEY, S3_SECRET_KEY, S3_REGION, S3_BUCKET]):
     logger.error("One or more required environment variables are missing or not loaded correctly.")
     sys.exit(1)
 
 os.environ['S3_ACCESS_KEY'] = S3_ACCESS_KEY
 os.environ['S3_SECRET_KEY'] = S3_SECRET_KEY
 os.environ['S3_REGION'] = S3_REGION
 os.environ['S3_BUCKET'] = S3_BUCKET
-os.environ['S3_CADDY_FILENAME'] = S3_CADDY_FILENAME
 
 def load_s3_client():
     return boto3.client(
         's3',
         aws_access_key_id=os.getenv('S3_ACCESS_KEY'),
         aws_secret_access_key=os.getenv('S3_SECRET_KEY'),
         region_name=os.getenv('S3_REGION')
@@ -144,27 +143,27 @@
         logger.error(f"Error uploading Caddyfile to S3: {e}")
         logger.error(traceback.format_exc())
         sys.exit(1)
 
 def get_caddyfile_path():
     return os.path.join(os.getcwd(), 'Caddyfile')
 
-def update_caddyfile(subdomain, port):
-    caddyfile_path = get_caddyfile_path()
+def update_caddyfile(subdomain, port, caddyfile_path=None):
+    caddyfile_path = caddyfile_path or get_caddyfile_path()
     new_entry = f"{subdomain} {{\n    reverse_proxy localhost:{port}\n}}\n"
     try:
         with open(caddyfile_path, 'a') as caddy_file:
             caddy_file.write(new_entry)
         logger.info(f"Updated Caddyfile with new entry for {subdomain}")
     except PermissionError:
         logger.error(f"Permission denied when trying to write to {caddyfile_path}")
         logger.error(traceback.format_exc())
 
-def remove_caddyfile_entry(subdomain):
-    caddyfile_path = get_caddyfile_path()
+def remove_caddyfile_entry(subdomain, caddyfile_path=None):
+    caddyfile_path = caddyfile_path or get_caddyfile_path()
     try:
         with open(caddyfile_path, 'r') as caddy_file:
             content = caddy_file.read()
         new_content = re.sub(rf"{subdomain} \{{.*?\}}\n", '', content, flags=re.DOTALL)
         with open(caddyfile_path, 'w') as caddy_file:
             caddy_file.write(new_content)
         logger.info(f"Removed Caddyfile entry for {subdomain}")
@@ -173,52 +172,52 @@
         logger.error(traceback.format_exc())
     except FileNotFoundError:
         logger.error(f"Caddyfile {caddyfile_path} not found.")
     except Exception as e:
         logger.error(f"Error removing Caddyfile entry: {e}")
         logger.error(traceback.format_exc())
 
-def format_caddyfile():
+def format_caddyfile(caddyfile_path=None):
     if is_caddy_running_in_docker():
-        format_caddyfile_docker()
+        format_caddyfile_docker(caddyfile_path)
     else:
-        format_caddyfile_system()
+        format_caddyfile_system(caddyfile_path)
 
-def restart_caddy():
+def restart_caddy(caddyfile_path=None):
     if is_caddy_running_in_docker():
-        restart_caddy_docker()
+        restart_caddy_docker(caddyfile_path)
     else:
         restart_caddy_system()
 
 def is_caddy_running_in_docker():
     try:
         result = subprocess.run(['docker', 'ps', '--filter', 'name=caddy', '--format', '{{.Names}}'], capture_output=True, text=True)
         return 'caddy' in result.stdout.strip().split('\n')
     except Exception as e:
         logger.error(f"Error checking Docker containers: {e}")
         return False
 
-def format_caddyfile_docker():
-    caddyfile_path = get_caddyfile_path()
+def format_caddyfile_docker(caddyfile_path=None):
+    caddyfile_path = caddyfile_path or get_caddyfile_path()
     result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddyfile formatted successfully within Docker")
     else:
         logger.error(f"Failed to format Caddyfile within Docker: {result.stderr}")
 
-def format_caddyfile_system():
-    caddyfile_path = get_caddyfile_path()
+def format_caddyfile_system(caddyfile_path=None):
+    caddyfile_path = caddyfile_path or get_caddyfile_path()
     result = subprocess.run(['caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddyfile formatted successfully")
     else:
         logger.error(f"Failed to format Caddyfile: {result.stderr}")
 
-def restart_caddy_docker():
-    caddyfile_path = get_caddyfile_path()
+def restart_caddy_docker(caddyfile_path=None):
+    caddyfile_path = caddyfile_path or get_caddyfile_path()
     result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'reload', '--config', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddy server reloaded successfully within Docker")
     else:
         logger.error(f"Failed to reload Caddy server in Docker: {result.stderr}")
 
 def restart_caddy_system():
@@ -228,16 +227,16 @@
     else:
         logger.error(f"Failed to reload Caddy server: {result.stderr}")
 
 def check_port_in_use(port):
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
         return sock.connect_ex(('localhost', int(port))) == 0
 
-def check_domain_exists(subdomain):
-    caddyfile_path = get_caddyfile_path()
+def check_domain_exists(subdomain, caddyfile_path=None):
+    caddyfile_path = caddyfile_path or get_caddyfile_path()
     try:
         with open(caddyfile_path, 'r') as caddy_file:
             content = caddy_file.read()
             return re.search(rf"{subdomain} \{{.*?\}}", content, flags=re.DOTALL) is not None
     except FileNotFoundError:
         logger.error(f"Caddyfile {caddyfile_path} not found.")
         return False
@@ -260,17 +259,18 @@
             return True
         logger.info(f"Waiting for {subdomain} to become resolvable... ({attempts + 1}/{max_attempts})")
         time.sleep(wait_time)
         attempts += 1
     logger.warning(f"{subdomain} is not resolvable after {max_attempts} attempts, continuing anyway")
     return False
 
-def load_profiles(s3_client):
+def load_profiles(s3_client, docker=False):
+    key = 'caddy_profiles_docker.json' if docker else 'caddy_profiles.json'
     try:
-        response = s3_client.get_object(Bucket=os.getenv('S3_BUCKET'), Key='caddy_profiles.json')
+        response = s3_client.get_object(Bucket=os.getenv('S3_BUCKET'), Key=key)
         profiles = json.loads(response['Body'].read().decode('utf-8'))
         return profiles
     except s3_client.exceptions.NoSuchKey:
         return {}
     except NoCredentialsError:
         logger.error("AWS credentials not available.")
         return {}
@@ -287,29 +287,30 @@
         "CLOUDFLARE_API_TOKEN": input("CLOUDFLARE_API_TOKEN: "),
         "CLOUDFLARE_ZONE_ID": input("CLOUDFLARE_ZONE_ID: "),
         "S3_CADDY_FILENAME": input("S3_CADDY_FILENAME: "),
         "MAIN_DOMAIN": input("MAIN_DOMAIN: ")
     }
     return profile
 
-def create_profile(profile_name):
+def create_profile(profile_name, docker=False):
     profile = prompt_for_profile()
     profile_key = profile["MAIN_DOMAIN"]
     s3_client = load_s3_client()
 
     try:
-        caddy_profiles = load_profiles(s3_client)
+        caddy_profiles = load_profiles(s3_client, docker)
     except Exception as e:
         caddy_profiles = {}
 
     caddy_profiles[profile_key] = profile
 
+    key = 'caddy_profiles_docker.json' if docker else 'caddy_profiles.json'
     try:
         s3_client.put_object(
             Bucket=os.getenv('S3_BUCKET'),
-            Key='caddy_profiles.json',
+            Key=key,
             Body=json.dumps(caddy_profiles)
         )
         logger.info(f"Profile '{profile_name}' created successfully.")
     except Exception as e:
         logger.error(f"Error creating profile: {e}")
         logger.error(traceback.format_exc())
```

### Comparing `cadprox-3.7/cadprox.egg-info/PKG-INFO` & `cadprox-3.8/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.7
+Version: 3.8
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.7/setup.py` & `cadprox-3.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from setuptools import setup, find_packages
 import subprocess
 import sys
 
 def check_caddy_installed():
     try:
         result = subprocess.run(['caddy', 'version'], capture_output=True, text=True, check=True)
-        print(f"Caddy version: {result.stdout.strip()}")
-    except subprocess.CalledProcessError as e:
-        print("Caddy is not installed or not found in PATH.")
-        print("Please install Caddy before proceeding.")
-        print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
-        sys.exit(1)
-    except FileNotFoundError:
-        print("Caddy is not installed or not found in PATH.")
+        print(f"Caddy (system) version: {result.stdout.strip()}")
+    except (subprocess.CalledProcessError, FileNotFoundError):
+        print("Caddy (system) is not installed or not found in PATH.")
         print("Please install Caddy before proceeding.")
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
+    
+    try:
+        result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'version'], capture_output=True, text=True, check=True)
+        print(f"Caddy (Docker) version: {result.stdout.strip()}")
+    except (subprocess.CalledProcessError, FileNotFoundError):
+        print("Caddy (Docker) is not installed or not found.")
+        print("Please ensure Docker is installed and the Caddy container is running if you intend to use Docker-based Caddy.")
+        # Do not exit since system Caddy may still be used
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='3.7',
+    version='3.8',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

