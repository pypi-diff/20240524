# Comparing `tmp/cadproxdk-2.3.tar.gz` & `tmp/cadproxdk-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadproxdk-2.3.tar", last modified: Fri May 24 07:47:26 2024, max compression
+gzip compressed data, was "cadproxdk-2.4.tar", last modified: Fri May 24 07:51:40 2024, max compression
```

## Comparing `cadproxdk-2.3.tar` & `cadproxdk-2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:47:26.097967 cadproxdk-2.3/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-2.3/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 07:47:26.097967 cadproxdk-2.3/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-2.3/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:47:26.089966 cadproxdk-2.3/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-2.3/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-2.3/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-2.3/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:47:26.093966 cadproxdk-2.3/cadproxdk.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 07:47:26.000000 cadproxdk-2.3/cadproxdk.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 07:47:26.097967 cadproxdk-2.3/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     2885 2024-05-24 07:47:09.000000 cadproxdk-2.3/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:51:40.336879 cadproxdk-2.4/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 05:12:06.000000 cadproxdk-2.4/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 07:51:40.336879 cadproxdk-2.4/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:12:06.000000 cadproxdk-2.4/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:51:40.328878 cadproxdk-2.4/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 05:12:03.000000 cadproxdk-2.4/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2676 2024-05-24 06:27:14.000000 cadproxdk-2.4/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8235 2024-05-24 06:28:50.000000 cadproxdk-2.4/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 07:51:40.332878 cadproxdk-2.4/cadproxdk.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4547 2024-05-24 07:51:40.000000 cadproxdk-2.4/cadproxdk.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      267 2024-05-24 07:51:40.000000 cadproxdk-2.4/cadproxdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 07:51:40.000000 cadproxdk-2.4/cadproxdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 07:51:40.000000 cadproxdk-2.4/cadproxdk.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       84 2024-05-24 07:51:40.000000 cadproxdk-2.4/cadproxdk.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 07:51:40.000000 cadproxdk-2.4/cadproxdk.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 07:51:40.336879 cadproxdk-2.4/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2881 2024-05-24 07:51:32.000000 cadproxdk-2.4/setup.py
```

### Comparing `cadproxdk-2.3/PKG-INFO` & `cadproxdk-2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 2.3
+Version: 2.4
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-2.3/README.md` & `cadproxdk-2.4/README.md`

 * *Files identical despite different names*

### Comparing `cadproxdk-2.3/app/main.py` & `cadproxdk-2.4/app/main.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-2.3/app/utils.py` & `cadproxdk-2.4/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadproxdk-2.3/cadproxdk.egg-info/PKG-INFO` & `cadproxdk-2.4/cadproxdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadproxdk
-Version: 2.3
+Version: 2.4
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadproxdk
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadproxdk-2.3/setup.py` & `cadproxdk-2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def run(self):
         install.run(self)
         create_caddy_config()
         print_post_install_message()
 
 setup(
     name='cadproxdk',
-    version='2.3',  # Incremented version
+    version='2.4',  # Updated version
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadproxdk',  # Update with your GitHub repository URL
     packages=find_packages(),
```

