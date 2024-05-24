# Comparing `tmp/shopify_custom_api-0.0.5.tar.gz` & `tmp/shopify_custom_api-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shopify_custom_api-0.0.5.tar", last modified: Tue May 21 10:38:45 2024, max compression
+gzip compressed data, was "shopify_custom_api-0.1.0.tar", last modified: Fri May 24 03:27:29 2024, max compression
```

## Comparing `shopify_custom_api-0.0.5.tar` & `shopify_custom_api-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:45.016169 shopify_custom_api-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-21 10:38:37.000000 shopify_custom_api-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-21 10:38:45.016169 shopify_custom_api-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-21 10:38:37.000000 shopify_custom_api-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:45.016169 shopify_custom_api-0.0.5/cshopify/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 10:38:37.000000 shopify_custom_api-0.0.5/cshopify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-21 10:38:37.000000 shopify_custom_api-0.0.5/cshopify/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:38:45.016169 shopify_custom_api-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-21 10:38:37.000000 shopify_custom_api-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:45.016169 shopify_custom_api-0.0.5/shopify_custom_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-21 10:38:44.000000 shopify_custom_api-0.0.5/shopify_custom_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-21 10:38:44.000000 shopify_custom_api-0.0.5/shopify_custom_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:38:44.000000 shopify_custom_api-0.0.5/shopify_custom_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 10:38:44.000000 shopify_custom_api-0.0.5/shopify_custom_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 10:38:44.000000 shopify_custom_api-0.0.5/shopify_custom_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:27:29.163810 shopify_custom_api-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-24 03:27:20.000000 shopify_custom_api-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-24 03:27:29.163810 shopify_custom_api-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-24 03:27:20.000000 shopify_custom_api-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:27:29.159809 shopify_custom_api-0.1.0/cshopify/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-24 03:27:20.000000 shopify_custom_api-0.1.0/cshopify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-24 03:27:20.000000 shopify_custom_api-0.1.0/cshopify/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 03:27:29.163810 shopify_custom_api-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-24 03:27:20.000000 shopify_custom_api-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:27:29.163810 shopify_custom_api-0.1.0/shopify_custom_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-24 03:27:29.000000 shopify_custom_api-0.1.0/shopify_custom_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-24 03:27:29.000000 shopify_custom_api-0.1.0/shopify_custom_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:27:29.000000 shopify_custom_api-0.1.0/shopify_custom_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 03:27:29.000000 shopify_custom_api-0.1.0/shopify_custom_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 03:27:29.000000 shopify_custom_api-0.1.0/shopify_custom_api.egg-info/top_level.txt
```

### Comparing `shopify_custom_api-0.0.5/LICENSE.txt` & `shopify_custom_api-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shopify_custom_api-0.0.5/cshopify/api.py` & `shopify_custom_api-0.1.0/cshopify/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,30 +15,29 @@
         url = f"https://{self.store_name}.myshopify.com/admin/api/{self.version}/{endpoint}.json"
 
         headers = {"X-Shopify-Access-Token": self.access_token}
 
         if data is not None:
             headers["Content-Type"] = "application/json"
 
-        print(headers)
 
         return request(
             method=method, url=url, params=params, json=data, headers=headers, **kwargs
         )
 
     def get(self, endpoint, params=None):
         # Get request
         return self.__request("GET", endpoint, params=params)
 
     def post(self, endpoint, data, params=None):
         # Post request
         assert self.validateJSON(data), "input data type must be JSON"
-        return self.__request("POST", endpoint, data, params=params)
+        return self.__request("POST", endpoint, data)
 
     def put(self, endpoint, data, params=None):
         # Put request
         assert self.validateJSON(data), "input data type must be JSON"
-        return self.__request("PUT", endpoint, data, params=params)
+        return self.__request("PUT", endpoint, data)
 
     def delete(self, endpoint, params=None):
         # Delete request
-        return self.__request("DELETE", endpoint, params=params)
+        return self.__request("DELETE", endpoint)
```

### Comparing `shopify_custom_api-0.0.5/setup.py` & `shopify_custom_api-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Verify packages found
 packages = find_packages()
 print("Packages found:", packages)
 
 setup(
     name="shopify_custom_api",
-    version="0.0.5",
+    version="0.1.0",
     description="A simple library that helps call Shopify's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bachnguyen2001/shopify_custom_api.git",
     author="Nguyen Ngoc Bach",
     author_email="bachnguyenfptu@gmail.com",
     license="MIT",
```

