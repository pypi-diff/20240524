# Comparing `tmp/cadproxdk-1.0.tar.gz` & `tmp/cadproxdk-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadproxdk-1.0.tar", last modified: Fri May 24 06:47:38 2024, max compression
+gzip compressed data, was "cadproxdk-1.5.tar", last modified: Fri May 24 06:50:56 2024, max compression
```

## Comparing `cadproxdk-1.0.tar` & `cadproxdk-1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 06:47:38.504346 cadproxdk-1.0/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-1.0/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4487 2024-05-24 06:47:38.500346 cadproxdk-1.0/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-1.0/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 06:47:38.496345 cadproxdk-1.0/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-1.0/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-1.0/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-1.0/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 06:47:38.500346 cadproxdk-1.0/cadproxdk.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4487 2024-05-24 06:47:38.000000 cadproxdk-1.0/cadproxdk.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 06:47:38.000000 cadproxdk-1.0/cadproxdk.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 06:47:38.000000 cadproxdk-1.0/cadproxdk.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 06:47:38.000000 cadproxdk-1.0/cadproxdk.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 06:47:38.000000 cadproxdk-1.0/cadproxdk.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 06:47:38.000000 cadproxdk-1.0/cadproxdk.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 06:47:38.504346 cadproxdk-1.0/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2144 2024-05-24 06:44:43.000000 cadproxdk-1.0/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 06:50:56.830348 cadproxdk-1.5/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-1.5/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4487 2024-05-24 06:50:56.830348 cadproxdk-1.5/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-1.5/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 06:50:56.822348 cadproxdk-1.5/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-1.5/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-1.5/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-1.5/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 06:50:56.830348 cadproxdk-1.5/cadproxdk.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4487 2024-05-24 06:50:56.000000 cadproxdk-1.5/cadproxdk.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 06:50:56.000000 cadproxdk-1.5/cadproxdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 06:50:56.000000 cadproxdk-1.5/cadproxdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 06:50:56.000000 cadproxdk-1.5/cadproxdk.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 06:50:56.000000 cadproxdk-1.5/cadproxdk.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 06:50:56.000000 cadproxdk-1.5/cadproxdk.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 06:50:56.830348 cadproxdk-1.5/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2144 2024-05-24 06:50:50.000000 cadproxdk-1.5/setup.py
```

### Comparing `cadproxdk-1.0/PKG-INFO` & `cadproxdk-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 1.0
+Version: 1.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-1.0/README.md` & `cadproxdk-1.5/README.md`

 * *Files identical despite different names*

### Comparing `cadproxdk-1.0/app/main.py` & `cadproxdk-1.5/app/main.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-1.0/app/utils.py` & `cadproxdk-1.5/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-1.0/cadproxdk.egg-info/PKG-INFO` & `cadproxdk-1.5/cadproxdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 1.0
+Version: 1.5
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-1.0/setup.py` & `cadproxdk-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
         print_post_install_message()
 
 setup(
     name='cadproxdk',
-    version='1.0',  # Initial version
+    version='1.5',  # Initial version
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadproxdk',  # Update with your GitHub repository URL
     packages=find_packages(),
```

