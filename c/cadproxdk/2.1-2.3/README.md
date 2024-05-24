# Comparing `tmp/cadproxdk-2.1.tar.gz` & `tmp/cadproxdk-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadproxdk-2.1.tar", last modified: Fri May 24 07:44:55 2024, max compression
+gzip compressed data, was "cadproxdk-2.3.tar", last modified: Fri May 24 07:47:26 2024, max compression
```

## Comparing `cadproxdk-2.1.tar` & `cadproxdk-2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:44:55.642281 cadproxdk-2.1/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-2.1/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 07:44:55.642281 cadproxdk-2.1/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-2.1/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:44:55.634281 cadproxdk-2.1/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-2.1/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-2.1/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-2.1/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:44:55.642281 cadproxdk-2.1/cadproxdk.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 07:44:55.000000 cadproxdk-2.1/cadproxdk.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 07:44:55.000000 cadproxdk-2.1/cadproxdk.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 07:44:55.000000 cadproxdk-2.1/cadproxdk.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 07:44:55.000000 cadproxdk-2.1/cadproxdk.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 07:44:55.000000 cadproxdk-2.1/cadproxdk.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 07:44:55.000000 cadproxdk-2.1/cadproxdk.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 07:44:55.642281 cadproxdk-2.1/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2778 2024-05-24 07:44:05.000000 cadproxdk-2.1/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:47:26.097967 cadproxdk-2.3/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-2.3/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 07:47:26.097967 cadproxdk-2.3/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-2.3/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:47:26.089966 cadproxdk-2.3/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-2.3/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-2.3/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-2.3/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:47:26.093966 cadproxdk-2.3/cadproxdk.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 07:47:26.097967 cadproxdk-2.3/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2885 2024-05-24 07:47:09.000000 cadproxdk-2.3/setup.py
```

### Comparing `cadproxdk-2.1/PKG-INFO` & `cadproxdk-2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 2.1
+Version: 2.3
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-2.1/README.md` & `cadproxdk-2.3/README.md`

 * *Files identical despite different names*

### Comparing `cadproxdk-2.1/app/main.py` & `cadproxdk-2.3/app/main.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-2.1/app/utils.py` & `cadproxdk-2.3/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-2.1/cadproxdk.egg-info/PKG-INFO` & `cadproxdk-2.3/cadproxdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 2.1
+Version: 2.3
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-2.1/setup.py` & `cadproxdk-2.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,28 +11,30 @@
             return True
         else:
             return False
     except FileNotFoundError:
         return False
 
 def create_caddy_config():
-    caddy_config_path = os.path.expanduser('~/caddy_config')
+    current_dir = os.path.abspath(os.getcwd())
+    caddy_config_path = os.path.join(current_dir, 'caddy_config')
     caddyfile_path = os.path.join(caddy_config_path, 'Caddyfile')
 
     if not os.path.exists(caddy_config_path):
         os.makedirs(caddy_config_path)
         print(f"Created directory: {caddy_config_path}")
 
     if not os.path.exists(caddyfile_path):
         with open(caddyfile_path, 'w') as f:
             f.write('')  # Create an empty Caddyfile
         print(f"Created file: {caddyfile_path}")
 
 def print_post_install_message():
-    caddyfile_path = os.path.expanduser('~/caddy_config/Caddyfile')
+    current_dir = os.path.abspath(os.getcwd())
+    caddyfile_path = os.path.join(current_dir, 'caddy_config', 'Caddyfile')
     message = f"""
     CADProxy installation is complete!
     
     Please run the following Docker command to start Caddy with the appropriate configuration:
 
     sudo docker run -d --name caddy -p 8088:80 -p 8543:443 -v {caddyfile_path}:/etc/caddy/Caddyfile caddy
 
@@ -49,15 +51,15 @@
     def run(self):
         install.run(self)
         create_caddy_config()
         print_post_install_message()
 
 setup(
     name='cadproxdk',
-    version='2.1',  # Incremented version
+    version='2.3',  # Incremented version
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadproxdk',  # Update with your GitHub repository URL
     packages=find_packages(),
```

