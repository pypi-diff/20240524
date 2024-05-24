# Comparing `tmp/aiohttp_oauth2_client-0.1.0.tar.gz` & `tmp/aiohttp_oauth2_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_oauth2_client-0.1.0.tar", last modified: Thu May 23 11:10:48 2024, max compression
+gzip compressed data, was "aiohttp_oauth2_client-1.0.0.tar", last modified: Fri May 24 13:54:19 2024, max compression
```

## Comparing `aiohttp_oauth2_client-0.1.0.tar` & `aiohttp_oauth2_client-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jenkins  (631603198) vito     (631600010)        0 2024-05-23 11:10:48.488353 aiohttp_oauth2_client-0.1.0/
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)    11357 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/LICENSE
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)      707 2024-05-23 11:10:48.488353 aiohttp_oauth2_client-0.1.0/PKG-INFO
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)     2281 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/README.md
-drwxr-xr-x   0 jenkins  (631603198) vito     (631600010)        0 2024-05-23 11:10:48.481353 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)        0 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/__init__.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)      933 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/client.py
-drwxr-xr-x   0 jenkins  (631603198) vito     (631600010)        0 2024-05-23 11:10:48.483353 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)        0 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/__init__.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)     4441 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/authorization_code.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)     2088 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/client_credentials.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)     3918 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/common.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)     3750 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/device_code.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)     1302 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/resource_owner_password_credentials.py
-drwxr-xr-x   0 jenkins  (631603198) vito     (631600010)        0 2024-05-23 11:10:48.485353 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)        0 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/__init__.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)      612 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/errors.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)      388 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/grant.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)     1217 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/pkce.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)     3858 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/request.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)     1886 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/response.py
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)     1737 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/token.py
-drwxr-xr-x   0 jenkins  (631603198) vito     (631600010)        0 2024-05-23 11:10:48.486353 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client.egg-info/
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)      707 2024-05-23 11:10:48.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client.egg-info/PKG-INFO
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)      884 2024-05-23 11:10:48.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)        1 2024-05-23 11:10:48.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)      163 2024-05-23 11:10:48.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client.egg-info/requires.txt
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)       22 2024-05-23 11:10:48.000000 aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client.egg-info/top_level.txt
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)      639 2024-05-23 11:09:04.000000 aiohttp_oauth2_client-0.1.0/pyproject.toml
--rw-r--r--   0 jenkins  (631603198) vito     (631600010)       38 2024-05-23 11:10:48.488353 aiohttp_oauth2_client-0.1.0/setup.cfg
+drwxr-xr-x   0 jenkins  (631603198) vito     (631600010)        0 2024-05-24 13:54:19.624893 aiohttp_oauth2_client-1.0.0/
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)    11357 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/LICENSE
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     8252 2024-05-24 13:54:19.623893 aiohttp_oauth2_client-1.0.0/PKG-INFO
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     7150 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/README.md
+drwxr-xr-x   0 jenkins  (631603198) vito     (631600010)        0 2024-05-24 13:54:19.619892 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)        0 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/__init__.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)      933 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/client.py
+drwxr-xr-x   0 jenkins  (631603198) vito     (631600010)        0 2024-05-24 13:54:19.621893 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)        0 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/__init__.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     4441 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/authorization_code.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     2088 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/client_credentials.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     3918 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/common.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     3750 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/device_code.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     1302 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/resource_owner_password_credentials.py
+drwxr-xr-x   0 jenkins  (631603198) vito     (631600010)        0 2024-05-24 13:54:19.622892 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)        0 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/__init__.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)      612 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/errors.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)      388 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/grant.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     1217 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/pkce.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     3858 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/request.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     1886 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/response.py
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     1737 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/token.py
+drwxr-xr-x   0 jenkins  (631603198) vito     (631600010)        0 2024-05-24 13:54:19.622892 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client.egg-info/
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)     8252 2024-05-24 13:54:19.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)      884 2024-05-24 13:54:19.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)        1 2024-05-24 13:54:19.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)      181 2024-05-24 13:54:19.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client.egg-info/requires.txt
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)       22 2024-05-24 13:54:19.000000 aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client.egg-info/top_level.txt
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)      978 2024-05-24 13:51:12.000000 aiohttp_oauth2_client-1.0.0/pyproject.toml
+-rw-r--r--   0 jenkins  (631603198) vito     (631600010)       38 2024-05-24 13:54:19.624893 aiohttp_oauth2_client-1.0.0/setup.cfg
```

### Comparing `aiohttp_oauth2_client-0.1.0/LICENSE` & `aiohttp_oauth2_client-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/client.py` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/client.py`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/authorization_code.py` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/authorization_code.py`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/client_credentials.py` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/client_credentials.py`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/common.py` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/common.py`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/device_code.py` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/device_code.py`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/grant/resource_owner_password_credentials.py` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/grant/resource_owner_password_credentials.py`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/errors.py` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/errors.py`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/pkce.py` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/pkce.py`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/request.py` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/request.py`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/response.py` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/response.py`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client/models/token.py` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client/models/token.py`

 * *Files identical despite different names*

### Comparing `aiohttp_oauth2_client-0.1.0/aiohttp_oauth2_client.egg-info/SOURCES.txt` & `aiohttp_oauth2_client-1.0.0/aiohttp_oauth2_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

