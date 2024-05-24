# Comparing `tmp/cadprox-1.5.tar.gz` & `tmp/cadprox-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-1.5.tar", last modified: Fri May 24 04:08:07 2024, max compression
+gzip compressed data, was "cadprox-1.6.tar", last modified: Fri May 24 04:22:44 2024, max compression
```

## Comparing `cadprox-1.5.tar` & `cadprox-1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:08:06.996594 cadprox-1.5/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-1.5/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:08:06.996594 cadprox-1.5/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      287 2024-05-24 03:13:51.000000 cadprox-1.5/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:08:06.992594 cadprox-1.5/cadprox/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-1.5/cadprox/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-1.5/cadprox/config.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     7922 2024-05-24 03:57:25.000000 cadprox-1.5/cadprox/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     7922 2024-05-24 04:01:13.000000 cadprox-1.5/cadprox/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:08:06.996594 cadprox-1.5/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:08:06.000000 cadprox-1.5/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      285 2024-05-24 04:08:06.000000 cadprox-1.5/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 04:08:06.000000 cadprox-1.5/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       46 2024-05-24 04:08:06.000000 cadprox-1.5/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 04:08:06.000000 cadprox-1.5/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        8 2024-05-24 04:08:06.000000 cadprox-1.5/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 04:08:06.996594 cadprox-1.5/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)      905 2024-05-24 04:07:22.000000 cadprox-1.5/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:22:44.800379 cadprox-1.6/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-1.6/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:22:44.796379 cadprox-1.6/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      287 2024-05-24 03:13:51.000000 cadprox-1.6/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:22:44.792379 cadprox-1.6/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-1.6/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-1.6/app/config.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3094 2024-05-24 04:21:50.000000 cadprox-1.6/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     7922 2024-05-24 04:21:59.000000 cadprox-1.6/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:22:44.796379 cadprox-1.6/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)      871 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      269 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 04:22:44.000000 cadprox-1.6/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 04:22:44.800379 cadprox-1.6/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)      901 2024-05-24 04:22:36.000000 cadprox-1.6/setup.py
```

### Comparing `cadprox-1.5/PKG-INFO` & `cadprox-1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 1.5
+Version: 1.6
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadprox
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-1.5/cadprox/main.py` & `cadprox-1.6/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadprox-1.5/cadprox.egg-info/PKG-INFO` & `cadprox-1.6/cadprox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 1.5
+Version: 1.6
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cadprox
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cadprox-1.5/setup.py` & `cadprox-1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cadprox',
-    version='1.5',
+    version='1.6',
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadprox',  # Update with your GitHub repository URL
     packages=find_packages(),
@@ -20,11 +20,11 @@
         'requests',
         'dnspython',
         'boto3',
         'python-dotenv'
     ],
     entry_points={
         'console_scripts': [
-            'cadprox=cadprox.main:main',
+            'cadprox=app.main:main',
         ],
     },
 )
```

