# Comparing `tmp/cadprox-1.8.tar.gz` & `tmp/cadprox-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadprox-1.8.tar", last modified: Fri May 24 04:45:38 2024, max compression
+gzip compressed data, was "cadprox-1.9.tar", last modified: Fri May 24 04:53:46 2024, max compression
```

## Comparing `cadprox-1.8.tar` & `cadprox-1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:45:38.963753 cadprox-1.8/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-1.8/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)     4679 2024-05-24 04:45:38.963753 cadprox-1.8/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)     4095 2024-05-24 04:38:51.000000 cadprox-1.8/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:45:38.955753 cadprox-1.8/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-1.8/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-1.8/app/config.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3094 2024-05-24 04:27:05.000000 cadprox-1.8/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     8164 2024-05-24 04:27:16.000000 cadprox-1.8/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:45:38.963753 cadprox-1.8/cadprox.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)     4679 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      269 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 04:45:38.000000 cadprox-1.8/cadprox.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 04:45:38.963753 cadprox-1.8/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)     1756 2024-05-24 04:45:18.000000 cadprox-1.8/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:53:46.008244 cadprox-1.9/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-24 03:13:50.000000 cadprox-1.9/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)     4435 2024-05-24 04:53:46.008244 cadprox-1.9/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3853 2024-05-24 04:49:17.000000 cadprox-1.9/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:53:46.004244 cadprox-1.9/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-24 03:13:48.000000 cadprox-1.9/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-24 03:13:48.000000 cadprox-1.9/app/config.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2956 2024-05-24 04:49:42.000000 cadprox-1.9/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     8164 2024-05-24 04:27:16.000000 cadprox-1.9/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-24 04:53:46.008244 cadprox-1.9/cadprox.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)     4435 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      269 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       42 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       39 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-24 04:53:45.000000 cadprox-1.9/cadprox.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-24 04:53:46.008244 cadprox-1.9/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1755 2024-05-24 04:53:39.000000 cadprox-1.9/setup.py
```

### Comparing `cadprox-1.8/PKG-INFO` & `cadprox-1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 1.8
+Version: 1.9
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
-Home-page: https://github.com/yourusername/cadprox
-Author: Piotr Tamu (Thriveroute)
-Author-email: your.email@example.com
+Home-page: https://github.com/reegen66/cadprox
+Author: Piotr Tamu (Thriveroute.com)
+Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -124,17 +124,14 @@
 ## Logging and Error Handling
 
 CADProxy uses Python's `logging` module for logging information, errors, and debugging messages. Logs are displayed in the console for easy tracking of actions and errors.
 
 ### Example Output
 
 ```bash
-Python executable: /usr/bin/python3
-Python path: ['/usr/bin', '/usr/lib/python38.zip', '/usr/lib/python3.8', '/usr/lib/python3.8/lib-dynload', '/usr/local/lib/python3.8/dist-packages', '/usr/lib/python3/dist-packages']
-Boto3 version: 1.17.49
 CLOUDFLARE_API_TOKEN: <hidden>
 CLOUDFLARE_ZONE_ID: <hidden>
 S3_CADDY_FILENAME: Caddyfile
 MAIN_DOMAIN: aiagency.dev
 INFO: Downloaded Caddyfile from S3 bucket caddy-configs
 INFO: Successfully added DNS record: subdomain.aiagency.dev -> 192.0.2.1
 INFO: subdomain.aiagency.dev is now resolvable
```

### Comparing `cadprox-1.8/README.md` & `cadprox-1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -106,17 +106,14 @@
 ## Logging and Error Handling
 
 CADProxy uses Python's `logging` module for logging information, errors, and debugging messages. Logs are displayed in the console for easy tracking of actions and errors.
 
 ### Example Output
 
 ```bash
-Python executable: /usr/bin/python3
-Python path: ['/usr/bin', '/usr/lib/python38.zip', '/usr/lib/python3.8', '/usr/lib/python3.8/lib-dynload', '/usr/local/lib/python3.8/dist-packages', '/usr/lib/python3/dist-packages']
-Boto3 version: 1.17.49
 CLOUDFLARE_API_TOKEN: <hidden>
 CLOUDFLARE_ZONE_ID: <hidden>
 S3_CADDY_FILENAME: Caddyfile
 MAIN_DOMAIN: aiagency.dev
 INFO: Downloaded Caddyfile from S3 bucket caddy-configs
 INFO: Successfully added DNS record: subdomain.aiagency.dev -> 192.0.2.1
 INFO: subdomain.aiagency.dev is now resolvable
```

### Comparing `cadprox-1.8/app/main.py` & `cadprox-1.9/app/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,14 @@
     check_domain_exists,
     wait_until_resolvable,
     load_profiles,
     create_profile
 )
 
 def main():
-    print(f"Python executable: {sys.executable}")
-    print(f"Python path: {sys.path}")
-    print(f"Boto3 version: {boto3.__version__}")
-
     parser = argparse.ArgumentParser(description='CADProxy Command Line Tool')
     parser.add_argument('command', choices=['add', 'create'], help='Command to execute')
     parser.add_argument('subdomain', help='Subdomain to add', nargs='?')
     parser.add_argument('-p', '--port', required=False, help='Backend server port')
 
     args = parser.parse_args()
```

### Comparing `cadprox-1.8/app/utils.py` & `cadprox-1.9/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadprox-1.8/cadprox.egg-info/PKG-INFO` & `cadprox-1.9/cadprox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: cadprox
-Version: 1.8
+Version: 1.9
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
-Home-page: https://github.com/yourusername/cadprox
-Author: Piotr Tamu (Thriveroute)
-Author-email: your.email@example.com
+Home-page: https://github.com/reegen66/cadprox
+Author: Piotr Tamu (Thriveroute.com)
+Author-email: nonyour@ssenisub.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -124,17 +124,14 @@
 ## Logging and Error Handling
 
 CADProxy uses Python's `logging` module for logging information, errors, and debugging messages. Logs are displayed in the console for easy tracking of actions and errors.
 
 ### Example Output
 
 ```bash
-Python executable: /usr/bin/python3
-Python path: ['/usr/bin', '/usr/lib/python38.zip', '/usr/lib/python3.8', '/usr/lib/python3.8/lib-dynload', '/usr/local/lib/python3.8/dist-packages', '/usr/lib/python3/dist-packages']
-Boto3 version: 1.17.49
 CLOUDFLARE_API_TOKEN: <hidden>
 CLOUDFLARE_ZONE_ID: <hidden>
 S3_CADDY_FILENAME: Caddyfile
 MAIN_DOMAIN: aiagency.dev
 INFO: Downloaded Caddyfile from S3 bucket caddy-configs
 INFO: Successfully added DNS record: subdomain.aiagency.dev -> 192.0.2.1
 INFO: subdomain.aiagency.dev is now resolvable
```

### Comparing `cadprox-1.8/setup.py` & `cadprox-1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,27 +17,28 @@
         print("Refer to the installation guide: https://caddyserver.com/docs/install#debian-ubuntu-raspbian")
         sys.exit(1)
 
 check_caddy_installed()
 
 setup(
     name='cadprox',
-    version='1.8',  # Increment the version number
-    author='Piotr Tamu (Thriveroute)',
-    author_email='your.email@example.com',
+    version='1.9',  # Increment the version number
+    author='Piotr Tamu (Thriveroute.com)',
+    author_email='nonyour@ssenisub.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/yourusername/cadprox',  # Update with your GitHub repository URL
+    url='https://github.com/reegen66/cadprox',  # Update with your GitHub repository URL
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
+
     python_requires='>=3.11',
     install_requires=[
         'requests',
         'dnspython',
         'boto3',
         'python-dotenv'
     ],
```

