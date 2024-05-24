# Comparing `tmp/aiorobonect-1.0.2.tar.gz` & `tmp/aiorobonect-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-1.0.2.tar", last modified: Mon May  6 11:02:45 2024, max compression
+gzip compressed data, was "aiorobonect-1.0.3.tar", last modified: Thu May 23 15:16:20 2024, max compression
```

## Comparing `aiorobonect-1.0.2.tar` & `aiorobonect-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:45.426974 aiorobonect-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-06 11:02:45.430974 aiorobonect-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:45.426974 aiorobonect-1.0.2/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/aiorobonect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/aiorobonect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-06 11:02:15.000000 aiorobonect-1.0.2/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:02:45.426974 aiorobonect-1.0.2/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-06 11:02:45.000000 aiorobonect-1.0.2/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-06 11:02:45.000000 aiorobonect-1.0.2/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:02:45.000000 aiorobonect-1.0.2/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-06 11:02:45.000000 aiorobonect-1.0.2/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 11:02:45.000000 aiorobonect-1.0.2/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-06 11:02:45.430974 aiorobonect-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-06 11:02:21.000000 aiorobonect-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:16:20.728973 aiorobonect-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-23 15:15:55.000000 aiorobonect-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-23 15:16:20.728973 aiorobonect-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-23 15:15:55.000000 aiorobonect-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:16:20.724973 aiorobonect-1.0.3/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-23 15:15:55.000000 aiorobonect-1.0.3/aiorobonect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-23 15:15:55.000000 aiorobonect-1.0.3/aiorobonect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 15:15:55.000000 aiorobonect-1.0.3/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-23 15:15:55.000000 aiorobonect-1.0.3/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:16:20.728973 aiorobonect-1.0.3/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-23 15:16:20.000000 aiorobonect-1.0.3/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-23 15:16:20.000000 aiorobonect-1.0.3/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:16:20.000000 aiorobonect-1.0.3/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 15:16:20.000000 aiorobonect-1.0.3/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 15:16:20.000000 aiorobonect-1.0.3/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-23 15:16:20.728973 aiorobonect-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-23 15:15:58.000000 aiorobonect-1.0.3/setup.py
```

### Comparing `aiorobonect-1.0.2/LICENSE` & `aiorobonect-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-1.0.2/PKG-INFO` & `aiorobonect-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 1.0.2
+Version: 1.0.3
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-1.0.2/README.md` & `aiorobonect-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-1.0.2/aiorobonect/client.py` & `aiorobonect-1.0.3/aiorobonect/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 class RobonectClient:
     """Class to communicate with the Robonect API."""
 
     def __init__(self, host, username, password, transform_json=False) -> None:
         """Initialize the Communication API to get data."""
         self.auth = None
         self.host = host
+        self.scheme = None
         self.username = username
         self.password = password
         self.client = None
         self.sleeping = None
         self.transform_json = transform_json
         if username is not None and password is not None:
             self.auth = (username, password)
@@ -84,23 +85,42 @@
 
         if command == "job":
             _LOGGER.debug(f"Job params: {params}")
             return
 
         result_json = None
         await self.client_start()
-        url = f"http://{self.host}/json?cmd={command}&{params}"
-        _LOGGER.debug(f"Calling {url}")
-        response = await self.client.get(url)
-        if response.status_code == 200:
+
+        def create_url(scheme):
+            return f"{scheme}://{self.host}/json?cmd={command}&{params}"
+
+        if self.scheme is None:
+            self.scheme = ["http", "https"]
+
+        response = None
+
+        for scheme in self.scheme:
+            url = create_url(scheme)
+            _LOGGER.debug(f"Calling {url}")
+            try:
+                response = await self.client.get(url)
+                if response.status_code == 200:
+                    self.scheme = [scheme]
+                    break  # Exit the loop on successful response
+            except httpx.RequestError as e:
+                _LOGGER.error(
+                    f"Failed to connect using {scheme.upper()}://{self.host}: {e}"
+                )
+
+        if response and response.status_code == 200:
             result_text = response.text
             _LOGGER.debug(f"Rest API call result for {command}: {result_text}")
             result_json = json.loads(result_text)
             result_json["sync_time"] = datetime.now()
-        elif response.status_code >= 400:
+        elif response and response.status_code >= 400:
             response.raise_for_status()
         await self.client_close()
 
         if self.transform_json:
             return transform_json_to_single_depth(result_json)
 
         return result_json
```

### Comparing `aiorobonect-1.0.2/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-1.0.3/aiorobonect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 1.0.2
+Version: 1.0.3
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-1.0.2/setup.cfg` & `aiorobonect-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiorobonect-1.0.2/setup.py` & `aiorobonect-1.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v1.0.2",
+    version="v1.0.3",
 )
```

