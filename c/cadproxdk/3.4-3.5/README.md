# Comparing `tmp/cadproxdk-3.4.tar.gz` & `tmp/cadproxdk-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadproxdk-3.4.tar", last modified: Fri May 24 08:58:56 2024, max compression
+gzip compressed data, was "cadproxdk-3.5.tar", last modified: Fri May 24 09:02:42 2024, max compression
```

## Comparing `cadproxdk-3.4.tar` & `cadproxdk-3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:58:56.737088 cadproxdk-3.4/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-3.4/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 08:58:56.737088 cadproxdk-3.4/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-3.4/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:58:56.733088 cadproxdk-3.4/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-3.4/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-3.4/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-3.4/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:58:56.737088 cadproxdk-3.4/cadproxdk.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 08:58:56.000000 cadproxdk-3.4/cadproxdk.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 08:58:56.000000 cadproxdk-3.4/cadproxdk.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 08:58:56.000000 cadproxdk-3.4/cadproxdk.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 08:58:56.000000 cadproxdk-3.4/cadproxdk.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 08:58:56.000000 cadproxdk-3.4/cadproxdk.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 08:58:56.000000 cadproxdk-3.4/cadproxdk.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 08:58:56.741088 cadproxdk-3.4/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2355 2024-05-24 08:58:50.000000 cadproxdk-3.4/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:02:42.005694 cadproxdk-3.5/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-3.5/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 09:02:42.005694 cadproxdk-3.5/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-3.5/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:02:42.001695 cadproxdk-3.5/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-3.5/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-3.5/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-3.5/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 09:02:42.005694 cadproxdk-3.5/cadproxdk.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 09:02:41.000000 cadproxdk-3.5/cadproxdk.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 09:02:42.005694 cadproxdk-3.5/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2645 2024-05-24 09:02:34.000000 cadproxdk-3.5/setup.py
```

### Comparing `cadproxdk-3.4/PKG-INFO` & `cadproxdk-3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 3.4
+Version: 3.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-3.4/README.md` & `cadproxdk-3.5/README.md`

 * *Files identical despite different names*

### Comparing `cadproxdk-3.4/app/main.py` & `cadproxdk-3.5/app/main.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-3.4/app/utils.py` & `cadproxdk-3.5/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-3.4/cadproxdk.egg-info/PKG-INFO` & `cadproxdk-3.5/cadproxdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 3.4
+Version: 3.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-3.4/setup.py` & `cadproxdk-3.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,30 @@
         self.print_post_install_message()
 
     def create_caddy_config(self):
         current_dir = Path().absolute()
         caddy_config_path = current_dir / 'caddy_config'
         caddyfile_path = caddy_config_path / 'Caddyfile'
 
-        if not caddy_config_path.exists():
+        try:
+            # Create directory if it doesn't exist
             caddy_config_path.mkdir(parents=True, exist_ok=True)
             print(f"Created directory: {caddy_config_path}")
 
-        if not caddyfile_path.exists():
+            # Create file if it doesn't exist
             caddyfile_path.touch()
             print(f"Created file: {caddyfile_path}")
 
+            # Set permissions to current user
+            os.chown(caddy_config_path, os.getuid(), os.getgid())
+            os.chown(caddyfile_path, os.getuid(), os.getgid())
+
+        except Exception as e:
+            print(f"Error creating caddy config: {e}")
+
     def print_post_install_message(self):
         current_dir = Path().absolute()
         caddyfile_path = current_dir / 'caddy_config' / 'Caddyfile'
         message = f"""
         CADProxy installation is complete!
 
         Please run the following Docker command to start Caddy with the appropriate configuration:
@@ -34,15 +42,15 @@
 
         Make sure the Caddyfile is located at {caddyfile_path}
         """
         print(message)
 
 setup(
     name='cadproxdk',
-    version='3.4',  # Incremented version
+    version='3.5',  # Incremented version
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadproxdk',  # Update with your GitHub repository URL
     packages=find_packages(),
```

