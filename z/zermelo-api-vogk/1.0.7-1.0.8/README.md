# Comparing `tmp/zermelo_api_vogk-1.0.7.tar.gz` & `tmp/zermelo_api_vogk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zermelo_api_vogk-1.0.7.tar", last modified: Thu May 23 08:11:32 2024, max compression
+gzip compressed data, was "zermelo_api_vogk-1.0.8.tar", last modified: Thu May 23 22:15:36 2024, max compression
```

## Comparing `zermelo_api_vogk-1.0.7.tar` & `zermelo_api_vogk-1.0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 08:11:32.485494 zermelo_api_vogk-1.0.7/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.7/LICENSE
--rw-r--r--   0 klaas     (1000) klaas     (1000)     4057 2024-05-23 08:11:32.485494 zermelo_api_vogk-1.0.7/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3485 2024-05-23 08:08:40.000000 zermelo_api_vogk-1.0.7/README.md
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 08:11:32.465493 zermelo_api_vogk-1.0.7/app/
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 08:11:32.469493 zermelo_api_vogk-1.0.7/app/zermelo_api/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      567 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/__init__.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 08:11:32.477493 zermelo_api_vogk-1.0.7/app/zermelo_api/src/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/__init__.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3144 2024-05-23 08:08:40.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/appointments.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     4100 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/branches.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/config.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      618 2024-05-17 10:07:35.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/credentials.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1556 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/groepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      674 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/io_json.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1136 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/leerjaren.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     6089 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/lesgroepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      812 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/lokalen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/time_utils.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3786 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/users.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1806 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/vakdoclok.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     2291 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/vakken.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     5831 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/vaklessen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3612 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/zermelo_api.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1523 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.7/app/zermelo_api/src/zermelo_collection.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 08:11:32.481493 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/
--rw-r--r--   0 klaas     (1000) klaas     (1000)     4057 2024-05-23 08:11:32.000000 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      834 2024-05-23 08:11:32.000000 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/SOURCES.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-05-23 08:11:32.000000 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/dependency_links.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       15 2024-05-23 08:11:32.000000 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/requires.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-05-23 08:11:32.000000 zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/top_level.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-05-23 08:11:32.485494 zermelo_api_vogk-1.0.7/setup.cfg
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      874 2024-05-23 08:10:36.000000 zermelo_api_vogk-1.0.7/setup.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 22:15:36.905723 zermelo_api_vogk-1.0.8/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.8/LICENSE
+-rw-r--r--   0 klaas     (1000) klaas     (1000)     4065 2024-05-23 22:15:36.905723 zermelo_api_vogk-1.0.8/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3493 2024-05-23 22:15:35.000000 zermelo_api_vogk-1.0.8/README.md
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 22:15:36.889723 zermelo_api_vogk-1.0.8/app/
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 22:15:36.889723 zermelo_api_vogk-1.0.8/app/zermelo_api/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      567 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/__init__.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 22:15:36.901723 zermelo_api_vogk-1.0.8/app/zermelo_api/src/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/__init__.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3144 2024-05-23 08:08:40.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/appointments.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     4100 2024-05-23 07:09:10.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/branches.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/config.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      618 2024-05-17 10:07:35.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/credentials.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1556 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/groepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      674 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/io_json.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1136 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/leerjaren.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     6132 2024-05-23 22:15:35.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/lesgroepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      812 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/lokalen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/time_utils.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3786 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/users.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1806 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/vakdoclok.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     2291 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/vakken.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     5831 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/vaklessen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3657 2024-05-23 22:15:35.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/zermelo_api.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1523 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.8/app/zermelo_api/src/zermelo_collection.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-23 22:15:36.905723 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/
+-rw-r--r--   0 klaas     (1000) klaas     (1000)     4065 2024-05-23 22:15:36.000000 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      834 2024-05-23 22:15:36.000000 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/SOURCES.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-05-23 22:15:36.000000 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/dependency_links.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       15 2024-05-23 22:15:36.000000 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/requires.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-05-23 22:15:36.000000 zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/top_level.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-05-23 22:15:36.905723 zermelo_api_vogk-1.0.8/setup.cfg
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      874 2024-05-23 22:15:35.000000 zermelo_api_vogk-1.0.8/setup.py
```

### Comparing `zermelo_api_vogk-1.0.7/LICENSE` & `zermelo_api_vogk-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/PKG-INFO` & `zermelo_api_vogk-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zermelo_api_vogk
-Version: 1.0.7
+Version: 1.0.8
 Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
 Author: Klaas Vogel
 Author-email: zermelo_api@klaasvogel.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
@@ -14,20 +14,20 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Provides-Extra: dev
 
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.6.1
+# V1.0.8
  - async loading lesgroepen done
  - async loading appointments done
  - enabled packages in __init__
  - made generator for branches
- - bugfix appointments
+ - bugfix: appointments, rooster
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.7/README.md` & `zermelo_api_vogk-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.6.1
+# V1.0.8
  - async loading lesgroepen done
  - async loading appointments done
  - enabled packages in __init__
  - made generator for branches
- - bugfix appointments
+ - bugfix: appointments, rooster
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/__init__.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/__init__.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/appointments.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/appointments.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/branches.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/branches.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/config.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/config.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/credentials.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/credentials.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/groepen.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/groepen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/io_json.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/io_json.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/leerjaren.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/leerjaren.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/lesgroepen.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/lesgroepen.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                     )
                 )
             results: list[tuple[Vak, list[Lesgroep]]] = await asyncio.gather(*tasks1)
             tasks2 = []
             for vak, lesgroepen in results:
                 self.extend(lesgroepen)
                 if not len(lesgroepen):
-                    logger.warning(vak)
+                    logger.debug(f"no regular groups found for {vak.subjectName}")
                     maingroepen = groepen.get_department_groups(leerjaar.id, True)
                     tasks2.append(
                         asyncio.create_task(
                             find_lesgroepen(
                                 leerjaar, vak, maingroepen, leerlingen, personeel
                             )
                         )
```

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/lokalen.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/lokalen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/users.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/users.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/vakdoclok.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/vakdoclok.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/vakken.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/vakken.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/vaklessen.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/vaklessen.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/zermelo_api.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/zermelo_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,17 @@
         logger.debug(f"get name: {data[0]}")
         row = data[0]
         if not row["prefix"]:
             return " ".join([row["firstName"], row["lastName"]])
         else:
             return " ".join([row["firstName"], row["prefix"], row["lastName"]])
 
-    async def getData(self, task, from_id=False) -> tuple[int, list[dict] | str]:
+    async def getData(
+        self, task, from_id=False
+    ) -> tuple[int, list[dict] | str | Exception]:
         result = (500, "unknown error")
         request = (
             self.zerurl + task + f"?access_token={self.credentials.token}"
             if from_id
             else self.zerurl + task + f"&access_token={self.credentials.token}"
         )
         logger.debug(request)
@@ -82,19 +84,20 @@
             if json_response:
                 json_status = json_response["response"]["status"]
                 if json_status == 200:
                     result = (200, json_response["response"]["data"])
                     logger.debug("    **** JSON OK ****")
                 else:
                     logger.debug(f"oeps, geen juiste response: {task}")
-                    result = (json_status, json_response["response"]["message"])
+                    result = (json_status, json_response["response"])
             else:
                 logger.error("JSON - response is leeg")
         except Exception as e:
             logger.error(e)
+            result = (500, e)
         finally:
             return result
 
     async def load_query(self, query: str) -> list[dict]:
         try:
             status, data = await self.getData(query)
             if status != 200:
```

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api/src/zermelo_collection.py` & `zermelo_api_vogk-1.0.8/app/zermelo_api/src/zermelo_collection.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/PKG-INFO` & `zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zermelo_api_vogk
-Version: 1.0.7
+Version: 1.0.8
 Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
 Author: Klaas Vogel
 Author-email: zermelo_api@klaasvogel.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
@@ -14,20 +14,20 @@
 License-File: LICENSE
 Requires-Dist: aiohttp
 Provides-Extra: dev
 
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
-# V1.0.6.1
+# V1.0.8
  - async loading lesgroepen done
  - async loading appointments done
  - enabled packages in __init__
  - made generator for branches
- - bugfix appointments
+ - bugfix: appointments, rooster
 
 # V1.0.2
  - replacement of request for working with asyncio
  - first rough test if asyncio is working
  - TODO: refactor leerlingen (sort should be done later)
  - loading branches seems done.
  - Next check Lesgroepen en vakdocloks
```

### Comparing `zermelo_api_vogk-1.0.7/app/zermelo_api_vogk.egg-info/SOURCES.txt` & `zermelo_api_vogk-1.0.8/app/zermelo_api_vogk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-1.0.7/setup.py` & `zermelo_api_vogk-1.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="zermelo_api_vogk",
-    version="1.0.7",
+    version="1.0.8",
     description="A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KlaasVogel/zermelo_api_vogk",
     author="Klaas Vogel",
```

