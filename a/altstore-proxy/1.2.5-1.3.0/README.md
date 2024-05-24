# Comparing `tmp/altstore_proxy-1.2.5.tar.gz` & `tmp/altstore_proxy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altstore_proxy-1.2.5.tar", last modified: Mon May 20 10:17:36 2024, max compression
+gzip compressed data, was "altstore_proxy-1.3.0.tar", last modified: Fri May 24 19:34:24 2024, max compression
```

## Comparing `altstore_proxy-1.2.5.tar` & `altstore_proxy-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:17:36.892157 altstore_proxy-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 10:17:25.000000 altstore_proxy-1.2.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-20 10:17:36.892157 altstore_proxy-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-20 10:17:25.000000 altstore_proxy-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:17:36.892157 altstore_proxy-1.2.5/altstore_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:17:25.000000 altstore_proxy-1.2.5/altstore_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:17:36.892157 altstore_proxy-1.2.5/altstore_proxy/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:17:25.000000 altstore_proxy-1.2.5/altstore_proxy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-20 10:17:25.000000 altstore_proxy-1.2.5/altstore_proxy/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-20 10:17:25.000000 altstore_proxy-1.2.5/altstore_proxy/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-20 10:17:25.000000 altstore_proxy-1.2.5/altstore_proxy/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:17:36.892157 altstore_proxy-1.2.5/altstore_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-20 10:17:36.000000 altstore_proxy-1.2.5/altstore_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-20 10:17:36.000000 altstore_proxy-1.2.5/altstore_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:17:36.000000 altstore_proxy-1.2.5/altstore_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 10:17:36.000000 altstore_proxy-1.2.5/altstore_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:17:36.000000 altstore_proxy-1.2.5/altstore_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 10:17:36.000000 altstore_proxy-1.2.5/altstore_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 10:17:36.000000 altstore_proxy-1.2.5/altstore_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:17:36.892157 altstore_proxy-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-20 10:17:25.000000 altstore_proxy-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:24.636584 altstore_proxy-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-24 19:34:20.000000 altstore_proxy-1.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 19:34:24.636584 altstore_proxy-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-24 19:34:20.000000 altstore_proxy-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:24.632584 altstore_proxy-1.3.0/altstore_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:20.000000 altstore_proxy-1.3.0/altstore_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:24.636584 altstore_proxy-1.3.0/altstore_proxy/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:20.000000 altstore_proxy-1.3.0/altstore_proxy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-24 19:34:20.000000 altstore_proxy-1.3.0/altstore_proxy/providers/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-24 19:34:20.000000 altstore_proxy-1.3.0/altstore_proxy/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-24 19:34:20.000000 altstore_proxy-1.3.0/altstore_proxy/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-05-24 19:34:20.000000 altstore_proxy-1.3.0/altstore_proxy/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:24.636584 altstore_proxy-1.3.0/altstore_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 19:34:24.000000 altstore_proxy-1.3.0/altstore_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-24 19:34:24.000000 altstore_proxy-1.3.0/altstore_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:34:24.000000 altstore_proxy-1.3.0/altstore_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-24 19:34:24.000000 altstore_proxy-1.3.0/altstore_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:34:24.000000 altstore_proxy-1.3.0/altstore_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-24 19:34:24.000000 altstore_proxy-1.3.0/altstore_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-24 19:34:24.000000 altstore_proxy-1.3.0/altstore_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:34:24.636584 altstore_proxy-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 19:34:20.000000 altstore_proxy-1.3.0/setup.py
```

### Comparing `altstore_proxy-1.2.5/LICENSE.md` & `altstore_proxy-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.2.5/PKG-INFO` & `altstore_proxy-1.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,39 @@
-Metadata-Version: 2.1
-Name: altstore_proxy
-Version: 1.2.5
-Summary: A simple proxy for slow AltStore servers
-Home-page: https://github.com/rix1337/AltStore-Proxy
-Author: rix1337
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-#  AltStore-Proxy
+# AltStore-Proxy
 
 [![PyPI version](https://badge.fury.io/py/altstore-proxy.svg)](https://badge.fury.io/py/altstore-proxy)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
 A simple proxy for slow AltStore servers
 
+# Features
+
+- Meant for use as custom Repo with AltStore Beta
+- Useful for manual sideloading / automatic update notifications with AltStore
+
 # Setup
 
 `pip install altstore_proxy`
 
 # Run
 
 ```
 altstore_proxy
   --port=8080
   --baseurl=https://example.com
   --cache=/tmp/altstore_cache
   --repos=https://fake.tld/apps.json,https://foo.bar/altstore.json
+  --discord_webhook=https://discord.com/api/webhooks/foo/bar
 ```
 
 # Docker
+
 ```
 docker run -d \
   --name="AltStore-Proxy" \
   -p port:8080 \
   -v /path/to/cache/:/cache:rw \
   -e 'BASEURL'='https://example.com'
   -e 'REPOS'='https://fake.tld/apps.json,https://foo.bar/altstore.json'
+  -e 'DISCORD_WEBHOOK'='https://discord.com/api/webhooks/foo/bar'
   rix1337/docker-altstore-proxy:latest
   ```
-
-
```

### Comparing `altstore_proxy-1.2.5/altstore_proxy/providers/version.py` & `altstore_proxy-1.3.0/altstore_proxy/providers/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # AltStore-Proxy
 # Project by https://github.com/rix1337
 
 import re
 
 
 def get_version():
-    return "1.2.5"
+    return "1.3.0"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub(r'[^\d.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `altstore_proxy-1.2.5/altstore_proxy/run.py` & `altstore_proxy-1.3.0/altstore_proxy/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from socketserver import ThreadingMixIn
 from wsgiref.simple_server import make_server, WSGIServer, WSGIRequestHandler
 
 import requests
 from bottle import Bottle, abort, static_file
 from tqdm import tqdm
 
-from altstore_proxy.providers import shared_state, version
+from altstore_proxy.providers import shared_state, version, notifications
 
 
 class ThreadingWSGIServer(ThreadingMixIn, WSGIServer):
     daemon_threads = True
 
 
 class NoLoggingWSGIRequestHandler(WSGIRequestHandler):
@@ -43,34 +43,38 @@
     total_size_in_bytes = int(response.headers.get('content-length', 0))
 
     # Resolve the actual URL if the provided URL is a shortened URL
     if "tinyurl.com" in url:
         url = response.url
 
     filename = os.path.join(shared_state.values["cache"], os.path.basename(url))
+
+    if filename.startswith("/"):
+        filename = filename[1:]
+
     os.makedirs(os.path.dirname(filename), exist_ok=True)
 
     # Check if file already exists and compare sizes
     if os.path.exists(filename):
         existing_file_size = os.path.getsize(filename)
         if existing_file_size == total_size_in_bytes:
             print(f"File {filename} already exists with the same size. Skipping download.")
-            return filename
+            return filename, True
 
     print(f"Downloading {url} to {filename}")
     progress_bar = tqdm(total=total_size_in_bytes, unit='iB', unit_scale=True)
     with open(filename, 'wb') as f:
         for data in response.iter_content(chunk_size=1024):
             progress_bar.update(len(data))
             f.write(data)
     progress_bar.close()
     if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
         print("ERROR, something went wrong")
 
-    return filename
+    return filename, False
 
 
 def update_json_proxy(shared_state_dict, shared_state_lock):
     shared_state.set_state(shared_state_dict, shared_state_lock)
 
     try:
         while True:
@@ -86,24 +90,26 @@
             }
 
             for repo in shared_state.values["repos_to_cache"]:
                 response = requests.get(repo)
                 data = response.json()
                 for app in data['apps']:
                     print("Found " + app['name'] + ", v." + app['version'])
-                    download_url = app['downloadURL']
-                    filename = download_and_cache_ipa(download_url)
-                    if filename.startswith("/"):
-                        filename = filename[1:]
-                    app['downloadURL'] = shared_state.values["baseurl"] + '/' + filename
+                    app['filename'], skipped = download_and_cache_ipa(app['downloadURL'])
+                    app['downloadURL'] = shared_state.values["baseurl"] + '/' + app['filename']
+
+                    if not skipped:
+                        if shared_state.values['discord_webhook']:
+                            notifications.discord_webhook(shared_state, app)
+
                 merged_json['apps'].extend(data['apps'])
 
-            shared_state.update("ready", True)
             shared_state.update("merged_json", merged_json)
 
+            print("[AltStore-Proxy] Cache updated. Next update in 1 hour.")
             time.sleep(3600)
     except KeyboardInterrupt:
         sys.exit(0)
 
 
 def main():
     with multiprocessing.Manager() as manager:
@@ -115,14 +121,15 @@
         shared_state.update("ready", False)
 
         parser = argparse.ArgumentParser()
         parser.add_argument("--port", help="Desired Port, defaults to 8080")
         parser.add_argument("--baseurl", help="Base URL for the AltStore-Proxy (for reverse proxy usage)")
         parser.add_argument("--cache", help="Desired Cache Directory, defaults to ./cache")
         parser.add_argument("--repos", help="Desired apps.json Repositories to Cache - comma separated")
+        parser.add_argument("--discord_webhook", help="Discord Webhook URL for notifications")
         arguments = parser.parse_args()
 
         if arguments.port:
             try:
                 shared_state.update("port", int(arguments.port))
             except ValueError:
                 print("[AltStore-Proxy] Port must be an integer")
@@ -164,81 +171,95 @@
             shared_state.update("repos_to_cache", [
                 "https://raw.githubusercontent.com/arichornlover/arichornlover.github.io/main/apps.json",
                 "https://raw.githubusercontent.com/lo-cafe/winston-altstore/main/apps.json"
             ])
             print("[AltStore-Proxy] No repositories provided, using default repositories: " + str(
                 shared_state.values["repos_to_cache"]))
 
+        if arguments.discord_webhook:
+            shared_state.update("discord_webhook", arguments.discord_webhook)
+            print("[AltStore-Proxy] Using Discord Webhook for update notifications")
+        else:
+            shared_state.update("discord_webhook", "")
+            print("[AltStore-Proxy] No update notifications set up.")
+
         app = Bottle()
 
         @app.get("/")
         def status():
-            repos_html = ''.join(
-                f'<li><a href="{repo}">{repo}</a></li>' for repo in shared_state.values["repos_to_cache"])
-            return f'''
-            <html>
-            <head>
-                <title>AltStore-Proxy</title>
-                <style>
-                    body {{
-                        background: linear-gradient(to right, #f9f9f9, #e0e0e0);
-                        font-family: Arial, sans-serif;
-                        padding: 20px;
-                        text-align: center;
-                    }}
-                    button {{
-                        font-size: 20px;
-                        padding: 10px 20px;
-                        margin-top: 20px;
-                        background-color: #4CAF50; /* Green */
-                        border: none;
-                        color: white;
-                        text-align: center;
-                        text-decoration: none;
-                        display: inline-block;
-                        font-size: 16px;
-                        transition-duration: 0.4s;
-                        cursor: pointer;
-                    }}
-                    button:hover {{
-                        background-color: #45a049;
-                    }}
-                </style>
-            </head>
-            <body>
-                <h1>AltStore-Proxy</h1>
-                <a href="/apps.json">Source for use in AltStore</a><br>
-                <a href="altstore://source?url={shared_state.values["baseurl"]}/apps.json">
-                    <button>Add this source to AltStore to receive app updates</button>
-                </a>
-                <h2>Source Repositories</h2>
-                <ul>
-                    {repos_html}
-                </ul>
-            </body>
-            </html>'''
+            try:
+                app_links = ""
+                for app in shared_state.values["merged_json"]['apps']:
+                    app_links += f'<a href="{app["downloadURL"]}" class="button grey">{app["name"]}</a><br>'
+
+                return f'''
+                <html>
+                <head>
+                    <title>AltStore-Proxy</title>
+                    <style>
+                        body {{
+                            background: linear-gradient(to right, #f9f9f9, #e0e0e0);
+                            font-family: Arial, sans-serif;
+                            padding: 20px;
+                            text-align: center;
+                        }}
+                        .button {{
+                            display: inline-block;
+                            font-size: 16px;
+                            margin: 10px;
+                            padding: 10px 20px;
+                            color: white;
+                            text-decoration: none;
+                            transition-duration: 0.4s;
+                            cursor: pointer;
+                            border-radius: 5px;
+                        }}
+                        .button.grey {{
+                            background-color: #808080; /* Grey */
+                        }}
+                        .button.grey:hover {{
+                            background-color: #696969; /* Darker Grey */
+                        }}
+                        .button.green {{
+                            background-color: #4CAF50; /* Green */
+                        }}
+                        .button.green:hover {{
+                            background-color: #45a049;
+                        }}
+                    </style>
+                </head>
+                <body>
+                    <h1>AltStore-Proxy</h1>
+                    {app_links}
+                    <a href="altstore://source?url={shared_state.values["baseurl"]}/apps.json">
+                        <button class="button green">Add this source to AltStore to receive app updates</button>
+                    </a><br><br>
+                    <a href="/apps.json">Source for use in AltStore</a>
+                </body>
+                </html>'''
+            except Exception as e:
+                print("[AntiGateHandler] status - Error: " + str(e))
+            return abort(503, "Cache not initialized. Please try again later.")
 
         @app.get('/cache/<filename:path>')
         def serve_file(filename):
-            return static_file(filename, root=shared_state.values["cache"], download=filename)
+            return static_file(filename, root=shared_state.values["cache"], download=filename,
+                               mimetype='application/octet-stream')
 
         @app.get("/apps.json")
         def status():
             try:
                 return shared_state.values["merged_json"]
             except Exception as e:
                 print("[AntiGateHandler] status - Error: " + str(e))
             return abort(503, "Cache not initialized. Please try again later.")
 
         hourly_update = multiprocessing.Process(target=update_json_proxy, args=(shared_state_dict, shared_state_lock,))
         hourly_update.start()
 
-        while not shared_state.values["ready"]:
-            time.sleep(1)
-
         print(
             "[AltStore-Proxy] Add this source to AltStore by opening " + shared_state.values[
                 "baseurl"] + " on your mobile device.")
         try:
             Server(app, listen='0.0.0.0', port=shared_state.values["port"]).serve_forever()
         except KeyboardInterrupt:
             hourly_update.terminate()
```

### Comparing `altstore_proxy-1.2.5/altstore_proxy.egg-info/PKG-INFO` & `altstore_proxy-1.3.0/altstore_proxy.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 Metadata-Version: 2.1
 Name: altstore-proxy
-Version: 1.2.5
+Version: 1.3.0
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-#  AltStore-Proxy
+# AltStore-Proxy
 
 [![PyPI version](https://badge.fury.io/py/altstore-proxy.svg)](https://badge.fury.io/py/altstore-proxy)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
 A simple proxy for slow AltStore servers
 
+# Features
+
+- Meant for use as custom Repo with AltStore Beta
+- Useful for manual sideloading / automatic update notifications with AltStore
+
 # Setup
 
 `pip install altstore_proxy`
 
 # Run
 
 ```
 altstore_proxy
   --port=8080
   --baseurl=https://example.com
   --cache=/tmp/altstore_cache
   --repos=https://fake.tld/apps.json,https://foo.bar/altstore.json
+  --discord_webhook=https://discord.com/api/webhooks/foo/bar
 ```
 
 # Docker
+
 ```
 docker run -d \
   --name="AltStore-Proxy" \
   -p port:8080 \
   -v /path/to/cache/:/cache:rw \
   -e 'BASEURL'='https://example.com'
   -e 'REPOS'='https://fake.tld/apps.json,https://foo.bar/altstore.json'
+  -e 'DISCORD_WEBHOOK'='https://discord.com/api/webhooks/foo/bar'
   rix1337/docker-altstore-proxy:latest
   ```
```

### Comparing `altstore_proxy-1.2.5/setup.py` & `altstore_proxy-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # AltStore-Proxy
-# Project by https://github.com/rix1337
+# Projekt by https://github.com/rix1337
 
 import setuptools
 
 from altstore_proxy.providers.version import get_version
 
 try:
     with open('README.md', encoding='utf-8') as f:
```

