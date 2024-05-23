# Comparing `tmp/zermelo_api_vogk-1.0.6.tar.gz` & `tmp/zermelo_api_vogk-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zermelo_api_vogk-1.0.6.tar", last modified: Thu May 23 07:09:15 2024, max compression
+gzip compressed data, was "zermelo_api_vogk-1.0.7.tar", last modified: Thu May 23 08:11:32 2024, max compression
```

## Comparing `zermelo_api_vogk-1.0.6.tar` & `zermelo_api_vogk-1.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 07:09:15.505049 zermelo_api_vogk-1.0.6/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.6/LICENSE
--rw-r--r--   0 klaas     (1000) klaas     (1000)     4032 2024-05-23 07:09:15.505049 zermelo_api_vogk-1.0.6/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3460 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.6/README.md
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 07:09:15.485048 zermelo_api_vogk-1.0.6/app/
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 07:09:15.485048 zermelo_api_vogk-1.0.6/app/zermelo_api/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      567 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/__init__.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 07:09:15.497049 zermelo_api_vogk-1.0.6/app/zermelo_api/src/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/__init__.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3138 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/appointments.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     4100 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/branches.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/config.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      618 2024-05-17 10:07:35.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/credentials.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1556 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/groepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      674 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/io_json.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1136 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/leerjaren.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     6089 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/lesgroepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      812 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/lokalen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/time_utils.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3786 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/users.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1806 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/vakdoclok.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     2291 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/vakken.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     5831 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/vaklessen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3612 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/zermelo_api.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1523 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.6/app/zermelo_api/src/zermelo_collection.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 07:09:15.501049 zermelo_api_vogk-1.0.6/app/zermelo_api_vogk.egg-info/
--rw-r--r--   0 klaas     (1000) klaas     (1000)     4032 2024-05-23 07:09:15.000000 zermelo_api_vogk-1.0.6/app/zermelo_api_vogk.egg-info/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      834 2024-05-23 07:09:15.000000 zermelo_api_vogk-1.0.6/app/zermelo_api_vogk.egg-info/SOURCES.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-05-23 07:09:15.000000 zermelo_api_vogk-1.0.6/app/zermelo_api_vogk.egg-info/dependency_links.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       15 2024-05-23 07:09:15.000000 zermelo_api_vogk-1.0.6/app/zermelo_api_vogk.egg-info/requires.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-05-23 07:09:15.000000 zermelo_api_vogk-1.0.6/app/zermelo_api_vogk.egg-info/top_level.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-05-23 07:09:15.505049 zermelo_api_vogk-1.0.6/setup.cfg
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      874 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.6/setup.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 08:11:32.485494 zermelo_api_vogk-1.0.7/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.7/LICENSE
+-rw-r--r--   0 klaas     (1000) klaas     (1000)     4057 2024-05-23 08:11:32.485494 zermelo_api_vogk-1.0.7/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3485 2024-05-23 08:08:40.000000 zermelo_api_vogk-1.0.7/README.md
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 08:11:32.465493 zermelo_api_vogk-1.0.7/app/
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 08:11:32.469493 zermelo_api_vogk-1.0.7/app/zermelo_api/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      567 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/__init__.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 08:11:32.477493 zermelo_api_vogk-1.0.7/app/zermelo_api/src/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/__init__.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3144 2024-05-23 08:08:40.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/appointments.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     4100 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/branches.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/config.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      618 2024-05-17 10:07:35.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/credentials.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1556 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/groepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      674 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/io_json.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1136 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/leerjaren.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     6089 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/lesgroepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      812 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/lokalen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/time_utils.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3786 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/users.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1806 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/vakdoclok.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     2291 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/vakken.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     5831 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/vaklessen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3612 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/zermelo_api.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1523 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/zermelo_collection.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 08:11:32.481493 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/
+-rw-r--r--   0 klaas     (1000) klaas     (1000)     4057 2024-05-23 08:11:32.000000 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      834 2024-05-23 08:11:32.000000 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/SOURCES.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-05-23 08:11:32.000000 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/dependency_links.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       15 2024-05-23 08:11:32.000000 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/requires.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-05-23 08:11:32.000000 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/top_level.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-05-23 08:11:32.485494 zermelo_api_vogk-1.0.7/setup.cfg
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      874 2024-05-23 08:10:36.000000 zermelo_api_vogk-1.0.7/setup.py
```

### Comparing `zermelo_api_vogk-1.0.6/LICENSE` & `zermelo_api_vogk-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/PKG-INFO` & `zermelo_api_vogk-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zermelo_api_vogk
-Version: 1.0.6
+Version: 1.0.7
 Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
 Author: Klaas Vogel
 Author-email: zermelo_api@klaasvogel.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
@@ -14,19 +14,20 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Provides-Extra: dev
 
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.6
+# V1.0.6.1
  - async loading lesgroepen done
  - async loading appointments done
  - enabled packages in __init__
  - made generator for branches
+ - bugfix appointments
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.6/README.md` & `zermelo_api_vogk-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.6
+# V1.0.6.1
  - async loading lesgroepen done
  - async loading appointments done
  - enabled packages in __init__
  - made generator for branches
+ - bugfix appointments
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/__init__.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/__init__.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/appointments.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/appointments.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     #     status, data = zermelo.getData(query, from_id=True)
     #     if status != 200:
     #         raise Exception(data)
     #     return from_zermelo_dict(cls, data[0])
 
 
 async def get_appointments(zermelo: ZermeloAPI, query: str) -> list[Appointment]:
-    status, data = zermelo.getData(query)
+    status, data = await zermelo.getData(query)
     if status != 200:
         raise Exception(data)
     return [from_zermelo_dict(Appointment, row) for row in data]
 
 
 async def get_user_appointments(
     zermelo: ZermeloAPI, user: int | str, **kwargs
```

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/branches.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/branches.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/config.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/config.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/credentials.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/credentials.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/groepen.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/groepen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/io_json.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/io_json.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/leerjaren.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/leerjaren.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/lesgroepen.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/lesgroepen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/lokalen.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/lokalen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/users.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/users.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/vakdoclok.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/vakdoclok.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/vakken.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/vakken.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/vaklessen.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/vaklessen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/zermelo_api.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/zermelo_api.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api/src/zermelo_collection.py` & `zermelo_api_vogk-1.0.7/app/zermelo_api/src/zermelo_collection.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api_vogk.egg-info/PKG-INFO` & `zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zermelo_api_vogk
-Version: 1.0.6
+Version: 1.0.7
 Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
 Author: Klaas Vogel
 Author-email: zermelo_api@klaasvogel.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
@@ -14,19 +14,20 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Provides-Extra: dev
 
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.6
+# V1.0.6.1
  - async loading lesgroepen done
  - async loading appointments done
  - enabled packages in __init__
  - made generator for branches
+ - bugfix appointments
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.6/app/zermelo_api_vogk.egg-info/SOURCES.txt` & `zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.6/setup.py` & `zermelo_api_vogk-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="zermelo_api_vogk",
-    version="1.0.6",
+    version="1.0.7",
     description="A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KlaasVogel/zermelo_api_vogk",
     author="Klaas Vogel",
```

