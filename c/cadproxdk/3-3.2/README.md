# Comparing `tmp/cadproxdk-3.tar.gz` & `tmp/cadproxdk-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadproxdk-3.tar", last modified: Fri May 24 08:43:23 2024, max compression
+gzip compressed data, was "cadproxdk-3.2.tar", last modified: Fri May 24 08:47:27 2024, max compression
```

## Comparing `cadproxdk-3.tar` & `cadproxdk-3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:43:23.875681 cadproxdk-3/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-3/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4545 2024-05-24 08:43:23.875681 cadproxdk-3/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-3/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:43:23.871681 cadproxdk-3/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-3/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-3/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-3/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:43:23.875681 cadproxdk-3/cadproxdk.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4545 2024-05-24 08:43:23.000000 cadproxdk-3/cadproxdk.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 08:43:23.000000 cadproxdk-3/cadproxdk.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 08:43:23.000000 cadproxdk-3/cadproxdk.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 08:43:23.000000 cadproxdk-3/cadproxdk.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 08:43:23.000000 cadproxdk-3/cadproxdk.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 08:43:23.000000 cadproxdk-3/cadproxdk.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 08:43:23.875681 cadproxdk-3/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2240 2024-05-24 08:43:12.000000 cadproxdk-3/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:47:27.981382 cadproxdk-3.2/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-3.2/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 08:47:27.981382 cadproxdk-3.2/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-3.2/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:47:27.973382 cadproxdk-3.2/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-3.2/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-3.2/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-3.2/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 08:47:27.981382 cadproxdk-3.2/cadproxdk.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 08:47:27.000000 cadproxdk-3.2/cadproxdk.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 08:47:27.000000 cadproxdk-3.2/cadproxdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 08:47:27.000000 cadproxdk-3.2/cadproxdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 08:47:27.000000 cadproxdk-3.2/cadproxdk.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 08:47:27.000000 cadproxdk-3.2/cadproxdk.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 08:47:27.000000 cadproxdk-3.2/cadproxdk.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 08:47:27.981382 cadproxdk-3.2/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2340 2024-05-24 08:47:06.000000 cadproxdk-3.2/setup.py
```

### Comparing `cadproxdk-3/PKG-INFO` & `cadproxdk-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 3
+Version: 3.2
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-3/README.md` & `cadproxdk-3.2/README.md`

 * *Files identical despite different names*

### Comparing `cadproxdk-3/app/main.py` & `cadproxdk-3.2/app/main.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-3/app/utils.py` & `cadproxdk-3.2/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-3/cadproxdk.egg-info/PKG-INFO` & `cadproxdk-3.2/cadproxdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 3
+Version: 3.2
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-3/setup.py` & `cadproxdk-3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from setuptools import setup, find_packages
 import os
 from setuptools.command.install import install
 from pathlib import Path
 
-def create_caddy_config():
-    current_dir = Path().absolute()
-    caddy_config_path = current_dir / 'caddy_config'
-    caddyfile_path = caddy_config_path / 'Caddyfile'
-
-    if not caddy_config_path.exists():
-        caddy_config_path.mkdir(parents=True)
-        print(f"Created directory: {caddy_config_path}")
-
-    if not caddyfile_path.exists():
-        caddyfile_path.touch()
-        print(f"Created file: {caddyfile_path}")
-
-def print_post_install_message():
-    current_dir = Path().absolute()
-    caddyfile_path = current_dir / 'caddy_config' / 'Caddyfile'
-    message = f"""
-    CADProxy installation is complete!
-    
-    Please run the following Docker command to start Caddy with the appropriate configuration:
-
-    docker run -d --name caddy -p 8088:80 -p 8543:443 -v {caddyfile_path}:/etc/caddy/Caddyfile caddy
-
-    Make sure the Caddyfile is located at {caddyfile_path}
-    """
-    print(message)
-
-class PostInstallCommand(install):
+class CustomInstallCommand(install):
     def run(self):
         install.run(self)
-        create_caddy_config()
-        print_post_install_message()
+        self.create_caddy_config()
+        self.print_post_install_message()
+
+    def create_caddy_config(self):
+        current_dir = Path().absolute()
+        caddy_config_path = current_dir / 'caddy_config'
+        caddyfile_path = caddy_config_path / 'Caddyfile'
+
+        if not caddy_config_path.exists():
+            caddy_config_path.mkdir(parents=True)
+            print(f"Created directory: {caddy_config_path}")
+
+        if not caddyfile_path.exists():
+            caddyfile_path.touch()
+            print(f"Created file: {caddyfile_path}")
+
+    def print_post_install_message(self):
+        current_dir = Path().absolute()
+        caddyfile_path = current_dir / 'caddy_config' / 'Caddyfile'
+        message = f"""
+        CADProxy installation is complete!
+
+        Please run the following Docker command to start Caddy with the appropriate configuration:
+
+        docker run -d --name caddy -p 8088:80 -p 8543:443 -v {caddyfile_path}:/etc/caddy/Caddyfile caddy
+
+        Make sure the Caddyfile is located at {caddyfile_path}
+        """
+        print(message)
 
 setup(
     name='cadproxdk',
-    version='3',  # Incremented version
+    version='3.2',  # Incremented version
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadproxdk',  # Update with your GitHub repository URL
     packages=find_packages(),
@@ -61,10 +61,10 @@
     ],
     entry_points={
         'console_scripts': [
             'cadprox=app.main:main',
         ],
     },
     cmdclass={
-        'install': PostInstallCommand,
+        'install': CustomInstallCommand,
     }
 )
```

