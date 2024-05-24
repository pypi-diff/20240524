# Comparing `tmp/cdproxy-1.1.tar.gz` & `tmp/cdproxy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdproxy-1.1.tar", last modified: Thu May 23 08:11:51 2024, max compression
+gzip compressed data, was "cdproxy-1.2.tar", last modified: Fri May 24 01:20:46 2024, max compression
```

## Comparing `cdproxy-1.1.tar` & `cdproxy-1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-23 08:11:51.385342 cdproxy-1.1/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-23 07:51:54.000000 cdproxy-1.1/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)      821 2024-05-23 08:11:51.385342 cdproxy-1.1/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      287 2024-05-23 07:45:42.000000 cdproxy-1.1/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-23 08:11:51.377341 cdproxy-1.1/cdprox/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-22 17:27:00.000000 cdproxy-1.1/cdprox/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-22 17:33:54.000000 cdproxy-1.1/cdprox/config.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     1932 2024-05-23 08:11:00.000000 cdproxy-1.1/cdprox/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3434 2024-05-23 07:48:35.000000 cdproxy-1.1/cdprox/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-23 08:11:51.385342 cdproxy-1.1/cdproxy.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)      821 2024-05-23 08:11:51.000000 cdproxy-1.1/cdproxy.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      281 2024-05-23 08:11:51.000000 cdproxy-1.1/cdproxy.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-23 08:11:51.000000 cdproxy-1.1/cdproxy.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       44 2024-05-23 08:11:51.000000 cdproxy-1.1/cdproxy.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       19 2024-05-23 08:11:51.000000 cdproxy-1.1/cdproxy.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        7 2024-05-23 08:11:51.000000 cdproxy-1.1/cdproxy.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-23 08:11:51.385342 cdproxy-1.1/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)      862 2024-05-23 08:11:35.000000 cdproxy-1.1/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 01:20:46.131678 cdproxy-1.2/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-23 07:51:54.000000 cdproxy-1.2/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)      842 2024-05-24 01:20:46.127678 cdproxy-1.2/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      287 2024-05-23 07:45:42.000000 cdproxy-1.2/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 01:20:46.123678 cdproxy-1.2/cdprox/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-22 17:27:00.000000 cdproxy-1.2/cdprox/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-22 17:33:54.000000 cdproxy-1.2/cdprox/config.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2806 2024-05-24 01:17:48.000000 cdproxy-1.2/cdprox/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     4496 2024-05-24 01:17:40.000000 cdproxy-1.2/cdprox/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 01:20:46.127678 cdproxy-1.2/cdproxy.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)      842 2024-05-24 01:20:46.000000 cdproxy-1.2/cdproxy.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      281 2024-05-24 01:20:46.000000 cdproxy-1.2/cdproxy.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 01:20:46.000000 cdproxy-1.2/cdproxy.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       44 2024-05-24 01:20:46.000000 cdproxy-1.2/cdproxy.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       25 2024-05-24 01:20:46.000000 cdproxy-1.2/cdproxy.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        7 2024-05-24 01:20:46.000000 cdproxy-1.2/cdproxy.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 01:20:46.131678 cdproxy-1.2/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)      909 2024-05-24 01:18:42.000000 cdproxy-1.2/setup.py
```

### Comparing `cdproxy-1.1/PKG-INFO` & `cdproxy-1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cdproxy
-Version: 1.1
+Version: 1.2
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cdproxy
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: dnspython
+Requires-Dist: boto3
 
 # cdprox
 
 cdprox is a Python package for adding DNS records to Cloudflare and configuring Caddy reverse proxies.
 
 Install caddy server (no docker)
```

### Comparing `cdproxy-1.1/cdproxy.egg-info/PKG-INFO` & `cdproxy-1.2/cdproxy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cdproxy
-Version: 1.1
+Version: 1.2
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cdproxy
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: dnspython
+Requires-Dist: boto3
 
 # cdprox
 
 cdprox is a Python package for adding DNS records to Cloudflare and configuring Caddy reverse proxies.
 
 Install caddy server (no docker)
```

### Comparing `cdproxy-1.1/setup.py` & `cdproxy-1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdproxy',
-    version='1.1',
+    version='1.2',  # Incremented version number
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cdproxy',  # Update with your GitHub repository URL
     packages=find_packages(),
@@ -15,14 +15,15 @@
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.11',
     install_requires=[
         'requests',
         'dnspython',
+        'boto3',
     ],
     entry_points={
         'console_scripts': [
             'cdprox=cdprox.main:main',
         ],
     },
 )
```

