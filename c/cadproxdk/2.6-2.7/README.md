# Comparing `tmp/cadproxdk-2.6.tar.gz` & `tmp/cadproxdk-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadproxdk-2.6.tar", last modified: Fri May 24 08:02:17 2024, max compression
+gzip compressed data, was "cadproxdk-2.7.tar", last modified: Fri May 24 08:05:22 2024, max compression
```

## Comparing `cadproxdk-2.6.tar` & `cadproxdk-2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:02:17.250110 cadproxdk-2.6/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-2.6/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 08:02:17.250110 cadproxdk-2.6/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-2.6/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:02:17.242110 cadproxdk-2.6/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-2.6/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-2.6/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-2.6/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:02:17.246110 cadproxdk-2.6/cadproxdk.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 08:02:17.000000 cadproxdk-2.6/cadproxdk.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 08:02:17.000000 cadproxdk-2.6/cadproxdk.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 08:02:17.000000 cadproxdk-2.6/cadproxdk.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 08:02:17.000000 cadproxdk-2.6/cadproxdk.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 08:02:17.000000 cadproxdk-2.6/cadproxdk.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 08:02:17.000000 cadproxdk-2.6/cadproxdk.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 08:02:17.250110 cadproxdk-2.6/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     3017 2024-05-24 08:02:06.000000 cadproxdk-2.6/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:05:22.651479 cadproxdk-2.7/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-2.7/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 08:05:22.647479 cadproxdk-2.7/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-2.7/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:05:22.643479 cadproxdk-2.7/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-2.7/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-2.7/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-2.7/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:05:22.647479 cadproxdk-2.7/cadproxdk.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 08:05:22.000000 cadproxdk-2.7/cadproxdk.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 08:05:22.000000 cadproxdk-2.7/cadproxdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 08:05:22.000000 cadproxdk-2.7/cadproxdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 08:05:22.000000 cadproxdk-2.7/cadproxdk.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 08:05:22.000000 cadproxdk-2.7/cadproxdk.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 08:05:22.000000 cadproxdk-2.7/cadproxdk.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 08:05:22.651479 cadproxdk-2.7/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2885 2024-05-24 08:05:09.000000 cadproxdk-2.7/setup.py
```

### Comparing `cadproxdk-2.6/PKG-INFO` & `cadproxdk-2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 2.6
+Version: 2.7
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-2.6/README.md` & `cadproxdk-2.7/README.md`

 * *Files identical despite different names*

### Comparing `cadproxdk-2.6/app/main.py` & `cadproxdk-2.7/app/main.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-2.6/app/utils.py` & `cadproxdk-2.7/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-2.6/cadproxdk.egg-info/PKG-INFO` & `cadproxdk-2.7/cadproxdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 2.6
+Version: 2.7
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-2.6/setup.py` & `cadproxdk-2.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,22 @@
         return False
 
 def create_caddy_config():
     current_dir = os.path.abspath(os.getcwd())
     caddy_config_path = os.path.join(current_dir, 'caddy_config')
     caddyfile_path = os.path.join(caddy_config_path, 'Caddyfile')
 
-    try:
-        if not os.path.exists(caddy_config_path):
-            os.makedirs(caddy_config_path)
-            print(f"Created directory: {caddy_config_path}")
-
-        if not os.path.exists(caddyfile_path):
-            with open(caddyfile_path, 'w') as f:
-                f.write('')  # Create an empty Caddyfile
-            print(f"Created file: {caddyfile_path}")
-    except Exception as e:
-        print(f"Error creating Caddyfile: {e}")
-        sys.exit(1)
+    if not os.path.exists(caddy_config_path):
+        os.makedirs(caddy_config_path)
+        print(f"Created directory: {caddy_config_path}")
+
+    if not os.path.exists(caddyfile_path):
+        with open(caddyfile_path, 'w') as f:
+            f.write('')  # Create an empty Caddyfile
+        print(f"Created file: {caddyfile_path}")
 
 def print_post_install_message():
     current_dir = os.path.abspath(os.getcwd())
     caddyfile_path = os.path.join(current_dir, 'caddy_config', 'Caddyfile')
     message = f"""
     CADProxy installation is complete!
     
@@ -55,15 +51,15 @@
     def run(self):
         install.run(self)
         create_caddy_config()
         print_post_install_message()
 
 setup(
     name='cadproxdk',
-    version='2.6',  # Incremented version
+    version='2.7',  # Incremented version
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadproxdk',  # Update with your GitHub repository URL
     packages=find_packages(),
```

