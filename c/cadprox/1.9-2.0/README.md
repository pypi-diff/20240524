# Comparing `tmp/cadprox-1.9.tar.gz` & `tmp/cadprox-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-1.9.tar", last modified: Fri May 24 04:53:46 2024, max compression
+gzip compressed data, was "cadprox-2.0.tar", last modified: Fri May 24 05:02:57 2024, max compression
```

## Comparing `cadprox-1.9.tar` & `cadprox-2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:53:46.008244 cadprox-1.9/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-1.9/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4435 2024-05-24 04:53:46.008244 cadprox-1.9/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     3853 2024-05-24 04:49:17.000000 cadprox-1.9/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:53:46.004244 cadprox-1.9/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-1.9/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-1.9/app/config.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2956 2024-05-24 04:49:42.000000 cadprox-1.9/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8164 2024-05-24 04:27:16.000000 cadprox-1.9/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:53:46.008244 cadprox-1.9/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4435 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      269 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 04:53:46.008244 cadprox-1.9/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1755 2024-05-24 04:53:39.000000 cadprox-1.9/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 05:02:57.590152 cadprox-2.0/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-2.0/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4481 2024-05-24 05:02:57.590152 cadprox-2.0/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3899 2024-05-24 05:02:27.000000 cadprox-2.0/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 05:02:57.586152 cadprox-2.0/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-2.0/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-2.0/app/config.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2956 2024-05-24 04:49:42.000000 cadprox-2.0/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8164 2024-05-24 04:27:16.000000 cadprox-2.0/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 05:02:57.590152 cadprox-2.0/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4481 2024-05-24 05:02:57.000000 cadprox-2.0/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      269 2024-05-24 05:02:57.000000 cadprox-2.0/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 05:02:57.000000 cadprox-2.0/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 05:02:57.000000 cadprox-2.0/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 05:02:57.000000 cadprox-2.0/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 05:02:57.000000 cadprox-2.0/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 05:02:57.590152 cadprox-2.0/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1755 2024-05-24 05:02:51.000000 cadprox-2.0/setup.py
```

### Comparing `cadprox-1.9/PKG-INFO` & `cadprox-2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 1.9
+Version: 2.0
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -147,7 +147,8 @@
 ## Contributing
 
 Contributions are welcome! Please open an issue or submit a pull request on GitHub.
 
 ## Contact
 
 For any issues, questions, or suggestions, please open an issue on the [GitHub repository](https://github.com/yourusername/cadprox).
+More info [Thriveroute.com](Thriveroute.com).
```

### Comparing `cadprox-1.9/README.md` & `cadprox-2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -129,7 +129,8 @@
 ## Contributing
 
 Contributions are welcome! Please open an issue or submit a pull request on GitHub.
 
 ## Contact
 
 For any issues, questions, or suggestions, please open an issue on the [GitHub repository](https://github.com/yourusername/cadprox).
+More info [Thriveroute.com](Thriveroute.com).
```

### Comparing `cadprox-1.9/app/main.py` & `cadprox-2.0/app/main.py`

 * *Files identical despite different names*

### Comparing `cadprox-1.9/app/utils.py` & `cadprox-2.0/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadprox-1.9/cadprox.egg-info/PKG-INFO` & `cadprox-2.0/cadprox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 1.9
+Version: 2.0
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/reegen66/cadprox
 Author: Piotr Tamu (Thriveroute.com)
 Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -147,7 +147,8 @@
 ## Contributing
 
 Contributions are welcome! Please open an issue or submit a pull request on GitHub.
 
 ## Contact
 
 For any issues, questions, or suggestions, please open an issue on the [GitHub repository](https://github.com/yourusername/cadprox).
+More info [Thriveroute.com](Thriveroute.com).
```

### Comparing `cadprox-1.9/setup.py` & `cadprox-2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='1.9',  # Increment the version number
+    version='2.0',  # Increment the version number
     author='Piotr Tamu (Thriveroute.com)',
     author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/reegen66/cadprox',  # Update with your GitHub repository URL
     packages=find_packages(),
```

