# Comparing `tmp/payrex_python-0.1.0.tar.gz` & `tmp/payrex_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payrex_python-0.1.0.tar", last modified: Thu May 16 03:03:48 2024, max compression
+gzip compressed data, was "payrex_python-0.1.1.tar", last modified: Fri May 24 05:32:10 2024, max compression
```

## Comparing `payrex_python-0.1.0.tar` & `payrex_python-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 josephisleta   (502) staff       (20)        0 2024-05-16 03:03:48.284814 payrex_python-0.1.0/
--rw-r--r--   0 josephisleta   (502) staff       (20)     1099 2024-05-14 03:07:47.000000 payrex_python-0.1.0/LICENSE
--rw-r--r--   0 josephisleta   (502) staff       (20)     2487 2024-05-16 03:03:48.283836 payrex_python-0.1.0/PKG-INFO
--rw-r--r--   0 josephisleta   (502) staff       (20)     1903 2024-05-16 01:15:47.000000 payrex_python-0.1.0/README.md
-drwxr-xr-x   0 josephisleta   (502) staff       (20)        0 2024-05-16 03:03:48.279754 payrex_python-0.1.0/payrex/
--rw-r--r--   0 josephisleta   (502) staff       (20)     1676 2024-05-16 01:15:31.000000 payrex_python-0.1.0/payrex/__init__.py
--rw-r--r--   0 josephisleta   (502) staff       (20)       82 2024-05-14 03:07:47.000000 payrex_python-0.1.0/payrex/api_resource.py
--rw-r--r--   0 josephisleta   (502) staff       (20)      363 2024-05-15 10:12:03.000000 payrex_python-0.1.0/payrex/client.py
--rw-r--r--   0 josephisleta   (502) staff       (20)      171 2024-05-16 00:59:24.000000 payrex_python-0.1.0/payrex/config.py
--rw-r--r--   0 josephisleta   (502) staff       (20)      172 2024-05-15 10:12:03.000000 payrex_python-0.1.0/payrex/error.py
--rw-r--r--   0 josephisleta   (502) staff       (20)     2191 2024-05-16 01:15:31.000000 payrex_python-0.1.0/payrex/http_client.py
-drwxr-xr-x   0 josephisleta   (502) staff       (20)        0 2024-05-16 03:03:48.280263 payrex_python-0.1.0/payrex/services/
--rw-r--r--   0 josephisleta   (502) staff       (20)      802 2024-05-15 10:12:03.000000 payrex_python-0.1.0/payrex/services/service_factory.py
-drwxr-xr-x   0 josephisleta   (502) staff       (20)        0 2024-05-16 03:03:48.283355 payrex_python-0.1.0/payrex_python.egg-info/
--rw-r--r--   0 josephisleta   (502) staff       (20)     2487 2024-05-16 03:03:48.000000 payrex_python-0.1.0/payrex_python.egg-info/PKG-INFO
--rw-r--r--   0 josephisleta   (502) staff       (20)      359 2024-05-16 03:03:48.000000 payrex_python-0.1.0/payrex_python.egg-info/SOURCES.txt
--rw-r--r--   0 josephisleta   (502) staff       (20)        1 2024-05-16 03:03:48.000000 payrex_python-0.1.0/payrex_python.egg-info/dependency_links.txt
--rw-r--r--   0 josephisleta   (502) staff       (20)        9 2024-05-16 03:03:48.000000 payrex_python-0.1.0/payrex_python.egg-info/requires.txt
--rw-r--r--   0 josephisleta   (502) staff       (20)        7 2024-05-16 03:03:48.000000 payrex_python-0.1.0/payrex_python.egg-info/top_level.txt
--rw-r--r--   0 josephisleta   (502) staff       (20)       38 2024-05-16 03:03:48.284856 payrex_python-0.1.0/setup.cfg
--rw-r--r--   0 josephisleta   (502) staff       (20)      819 2024-05-16 01:22:24.000000 payrex_python-0.1.0/setup.py
+drwxr-xr-x   0 josephisleta   (502) staff       (20)        0 2024-05-24 05:32:10.312492 payrex_python-0.1.1/
+-rw-r--r--   0 josephisleta   (502) staff       (20)     1099 2024-05-16 03:45:33.000000 payrex_python-0.1.1/LICENSE
+-rw-r--r--   0 josephisleta   (502) staff       (20)     2487 2024-05-24 05:32:10.311860 payrex_python-0.1.1/PKG-INFO
+-rw-r--r--   0 josephisleta   (502) staff       (20)     1903 2024-05-16 03:45:33.000000 payrex_python-0.1.1/README.md
+drwxr-xr-x   0 josephisleta   (502) staff       (20)        0 2024-05-24 05:32:10.305772 payrex_python-0.1.1/payrex/
+-rw-r--r--   0 josephisleta   (502) staff       (20)     1676 2024-05-16 03:45:33.000000 payrex_python-0.1.1/payrex/__init__.py
+-rw-r--r--   0 josephisleta   (502) staff       (20)       82 2024-05-16 03:45:33.000000 payrex_python-0.1.1/payrex/api_resource.py
+-rw-r--r--   0 josephisleta   (502) staff       (20)      363 2024-05-16 03:45:33.000000 payrex_python-0.1.1/payrex/client.py
+-rw-r--r--   0 josephisleta   (502) staff       (20)      171 2024-05-24 02:25:41.000000 payrex_python-0.1.1/payrex/config.py
+-rw-r--r--   0 josephisleta   (502) staff       (20)      172 2024-05-16 03:45:33.000000 payrex_python-0.1.1/payrex/error.py
+-rw-r--r--   0 josephisleta   (502) staff       (20)     2393 2024-05-24 05:26:29.000000 payrex_python-0.1.1/payrex/http_client.py
+drwxr-xr-x   0 josephisleta   (502) staff       (20)        0 2024-05-24 05:32:10.310939 payrex_python-0.1.1/payrex_python.egg-info/
+-rw-r--r--   0 josephisleta   (502) staff       (20)     2487 2024-05-24 05:32:10.000000 payrex_python-0.1.1/payrex_python.egg-info/PKG-INFO
+-rw-r--r--   0 josephisleta   (502) staff       (20)      324 2024-05-24 05:32:10.000000 payrex_python-0.1.1/payrex_python.egg-info/SOURCES.txt
+-rw-r--r--   0 josephisleta   (502) staff       (20)        1 2024-05-24 05:32:10.000000 payrex_python-0.1.1/payrex_python.egg-info/dependency_links.txt
+-rw-r--r--   0 josephisleta   (502) staff       (20)        9 2024-05-24 05:32:10.000000 payrex_python-0.1.1/payrex_python.egg-info/requires.txt
+-rw-r--r--   0 josephisleta   (502) staff       (20)        7 2024-05-24 05:32:10.000000 payrex_python-0.1.1/payrex_python.egg-info/top_level.txt
+-rw-r--r--   0 josephisleta   (502) staff       (20)       38 2024-05-24 05:32:10.312534 payrex_python-0.1.1/setup.cfg
+-rw-r--r--   0 josephisleta   (502) staff       (20)      819 2024-05-24 05:26:29.000000 payrex_python-0.1.1/setup.py
```

### Comparing `payrex_python-0.1.0/LICENSE` & `payrex_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `payrex_python-0.1.0/PKG-INFO` & `payrex_python-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payrex-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: PayRex Python Library
 Home-page: https://github.com/payrexhq/payrex-python
 Author: PayRex
 Author-email: support@payrexhq.com
 License: MIT
 Keywords: payrex
 Classifier: Development Status :: 4 - Beta
```

### Comparing `payrex_python-0.1.0/README.md` & `payrex_python-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `payrex_python-0.1.0/payrex/__init__.py` & `payrex_python-0.1.1/payrex/__init__.py`

 * *Files identical despite different names*

### Comparing `payrex_python-0.1.0/payrex/http_client.py` & `payrex_python-0.1.1/payrex/http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,21 +24,27 @@
         if method.lower() in ['post', 'put']:
             data = self._encode_params(params)
         else:
             data = None
 
         response = requests.request(method, url, auth=auth, headers=headers, data=data)
 
-        if response.status_code != 200:
+        if not response.content:
+            raise Exception(response)
+
+        if response.status_code < 200 or response.status_code >= 400:
             self._handle_error(response)
 
         return ApiResource(response.json())
 
     def _handle_error(self, response):
-        json_response_body = response.json()
+        try:
+            json_response_body = response.json()
+        except json.JSONDecodeError:
+            raise Exception(response.content)
 
         if response.status_code == 400:
             raise RequestInvalidException(json_response_body)
         elif response.status_code == 401:
             raise AuthenticationInvalidException(json_response_body)
         elif response.status_code == 404:
             raise ResourceNotFoundException(json_response_body)
```

### Comparing `payrex_python-0.1.0/payrex_python.egg-info/PKG-INFO` & `payrex_python-0.1.1/payrex_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payrex-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: PayRex Python Library
 Home-page: https://github.com/payrexhq/payrex-python
 Author: PayRex
 Author-email: support@payrexhq.com
 License: MIT
 Keywords: payrex
 Classifier: Development Status :: 4 - Beta
```

### Comparing `payrex_python-0.1.0/setup.py` & `payrex_python-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='payrex-python',
-    version='0.1.0',
+    version='0.1.1',
     author='PayRex',
     author_email='support@payrexhq.com',
     description='PayRex Python Library',
     long_description=(Path(__file__).parent / 'README.md').read_text(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

