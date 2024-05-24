# Comparing `tmp/cadproxdk-1.7.tar.gz` & `tmp/cadproxdk-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadproxdk-1.7.tar", last modified: Fri May 24 06:56:35 2024, max compression
+gzip compressed data, was "cadproxdk-1.8.tar", last modified: Fri May 24 07:06:17 2024, max compression
```

## Comparing `cadproxdk-1.7.tar` & `cadproxdk-1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 06:56:35.730338 cadproxdk-1.7/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-1.7/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 06:56:35.730338 cadproxdk-1.7/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-1.7/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 06:56:35.722338 cadproxdk-1.7/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-1.7/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-1.7/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-1.7/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 06:56:35.726338 cadproxdk-1.7/cadproxdk.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 06:56:35.000000 cadproxdk-1.7/cadproxdk.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 06:56:35.000000 cadproxdk-1.7/cadproxdk.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 06:56:35.000000 cadproxdk-1.7/cadproxdk.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 06:56:35.000000 cadproxdk-1.7/cadproxdk.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 06:56:35.000000 cadproxdk-1.7/cadproxdk.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 06:56:35.000000 cadproxdk-1.7/cadproxdk.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 06:56:35.730338 cadproxdk-1.7/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2774 2024-05-24 06:55:46.000000 cadproxdk-1.7/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:06:17.230360 cadproxdk-1.8/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-1.8/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 07:06:17.226360 cadproxdk-1.8/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-1.8/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:06:17.222360 cadproxdk-1.8/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-1.8/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-1.8/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-1.8/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:06:17.226360 cadproxdk-1.8/cadproxdk.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 07:06:17.000000 cadproxdk-1.8/cadproxdk.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 07:06:17.000000 cadproxdk-1.8/cadproxdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 07:06:17.000000 cadproxdk-1.8/cadproxdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 07:06:17.000000 cadproxdk-1.8/cadproxdk.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 07:06:17.000000 cadproxdk-1.8/cadproxdk.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 07:06:17.000000 cadproxdk-1.8/cadproxdk.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 07:06:17.230360 cadproxdk-1.8/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2774 2024-05-24 07:06:03.000000 cadproxdk-1.8/setup.py
```

### Comparing `cadproxdk-1.7/PKG-INFO` & `cadproxdk-1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 1.7
+Version: 1.8
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-1.7/README.md` & `cadproxdk-1.8/README.md`

 * *Files identical despite different names*

### Comparing `cadproxdk-1.7/app/main.py` & `cadproxdk-1.8/app/main.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-1.7/app/utils.py` & `cadproxdk-1.8/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-1.7/cadproxdk.egg-info/PKG-INFO` & `cadproxdk-1.8/cadproxdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 1.7
+Version: 1.8
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-1.7/setup.py` & `cadproxdk-1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def run(self):
         install.run(self)
         create_caddy_config()
         print_post_install_message()
 
 setup(
     name='cadproxdk',
-    version='1.7',  # Initial version
+    version='1.8',  # Initial version
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadproxdk',  # Update with your GitHub repository URL
     packages=find_packages(),
```

