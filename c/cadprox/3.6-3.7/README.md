# Comparing `tmp/cadprox-3.6.tar.gz` & `tmp/cadprox-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-3.6.tar", last modified: Fri May 24 11:45:43 2024, max compression
+gzip compressed data, was "cadprox-3.7.tar", last modified: Fri May 24 12:02:35 2024, max compression
```

## Comparing `cadprox-3.6.tar` & `cadprox-3.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:45:43.138736 cadprox-3.6/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.6/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:45:43.134736 cadprox-3.6/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.6/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:45:43.126736 cadprox-3.6/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.6/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3868 2024-05-24 11:45:26.000000 cadprox-3.6/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)    10994 2024-05-24 11:45:02.000000 cadprox-3.6/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 11:45:43.134736 cadprox-3.6/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 11:45:43.000000 cadprox-3.6/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 11:45:43.138736 cadprox-3.6/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 11:45:33.000000 cadprox-3.6/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:02:35.679213 cadprox-3.7/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-3.7/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:02:35.679213 cadprox-3.7/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3907 2024-05-24 05:53:44.000000 cadprox-3.7/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:02:35.675213 cadprox-3.7/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-3.7/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3868 2024-05-24 11:45:26.000000 cadprox-3.7/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)    12294 2024-05-24 12:02:17.000000 cadprox-3.7/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 12:02:35.679213 cadprox-3.7/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4489 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      255 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 12:02:35.000000 cadprox-3.7/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 12:02:35.679213 cadprox-3.7/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1680 2024-05-24 12:02:29.000000 cadprox-3.7/setup.py
```

### Comparing `cadprox-3.6/PKG-INFO` & `cadprox-3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.6
+Version: 3.7
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.6/README.md` & `cadprox-3.7/README.md`

 * *Files identical despite different names*

### Comparing `cadprox-3.6/app/main.py` & `cadprox-3.7/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-3.6/app/utils.py` & `cadprox-3.7/app/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,29 +174,64 @@
     except FileNotFoundError:
         logger.error(f"Caddyfile {caddyfile_path} not found.")
     except Exception as e:
         logger.error(f"Error removing Caddyfile entry: {e}")
         logger.error(traceback.format_exc())
 
 def format_caddyfile():
+    if is_caddy_running_in_docker():
+        format_caddyfile_docker()
+    else:
+        format_caddyfile_system()
+
+def restart_caddy():
+    if is_caddy_running_in_docker():
+        restart_caddy_docker()
+    else:
+        restart_caddy_system()
+
+def is_caddy_running_in_docker():
+    try:
+        result = subprocess.run(['docker', 'ps', '--filter', 'name=caddy', '--format', '{{.Names}}'], capture_output=True, text=True)
+        return 'caddy' in result.stdout.strip().split('\n')
+    except Exception as e:
+        logger.error(f"Error checking Docker containers: {e}")
+        return False
+
+def format_caddyfile_docker():
     caddyfile_path = get_caddyfile_path()
     result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
+        logger.info("Caddyfile formatted successfully within Docker")
+    else:
+        logger.error(f"Failed to format Caddyfile within Docker: {result.stderr}")
+
+def format_caddyfile_system():
+    caddyfile_path = get_caddyfile_path()
+    result = subprocess.run(['caddy', 'fmt', '--overwrite', caddyfile_path], capture_output=True, text=True)
+    if result.returncode == 0:
         logger.info("Caddyfile formatted successfully")
     else:
         logger.error(f"Failed to format Caddyfile: {result.stderr}")
 
-def restart_caddy():
+def restart_caddy_docker():
     caddyfile_path = get_caddyfile_path()
     result = subprocess.run(['docker', 'exec', 'caddy', 'caddy', 'reload', '--config', caddyfile_path], capture_output=True, text=True)
     if result.returncode == 0:
         logger.info("Caddy server reloaded successfully within Docker")
     else:
         logger.error(f"Failed to reload Caddy server in Docker: {result.stderr}")
 
+def restart_caddy_system():
+    result = subprocess.run(['sudo', 'caddy', 'reload'], capture_output=True, text=True)
+    if result.returncode == 0:
+        logger.info("Caddy server reloaded successfully")
+    else:
+        logger.error(f"Failed to reload Caddy server: {result.stderr}")
+
 def check_port_in_use(port):
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
         return sock.connect_ex(('localhost', int(port))) == 0
 
 def check_domain_exists(subdomain):
     caddyfile_path = get_caddyfile_path()
     try:
```

### Comparing `cadprox-3.6/cadprox.egg-info/PKG-INFO` & `cadprox-3.7/cadprox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 3.6
+Version: 3.7
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-3.6/setup.py` & `cadprox-3.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='3.6',
+    version='3.7',
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',
     packages=find_packages(),
```

