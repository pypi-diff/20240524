# Comparing `tmp/aiocmcapi-0.7.1.tar.gz` & `tmp/aiocmcapi-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocmcapi-0.7.1.tar", last modified: Wed May 22 09:51:22 2024, max compression
+gzip compressed data, was "aiocmcapi-0.7.2.tar", last modified: Thu May 23 18:52:08 2024, max compression
```

## Comparing `aiocmcapi-0.7.1.tar` & `aiocmcapi-0.7.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:51:22.347402 aiocmcapi-0.7.1/
--rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     3407 2024-05-22 09:51:22.346405 aiocmcapi-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     3137 2024-05-22 09:50:20.000000 aiocmcapi-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 09:51:22.339418 aiocmcapi-0.7.1/aiocmcapi/
--rw-rw-rw-   0        0        0       58 2024-05-21 07:51:43.000000 aiocmcapi-0.7.1/aiocmcapi/__init__.py
--rw-rw-rw-   0        0        0     1077 2024-05-22 08:57:17.000000 aiocmcapi-0.7.1/aiocmcapi/client.py
--rw-rw-rw-   0        0        0     1361 2024-05-22 08:57:27.000000 aiocmcapi-0.7.1/aiocmcapi/currency.py
--rw-rw-rw-   0        0        0      357 2024-05-22 09:02:53.000000 aiocmcapi-0.7.1/aiocmcapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:51:22.346405 aiocmcapi-0.7.1/aiocmcapi.egg-info/
--rw-rw-rw-   0        0        0     3407 2024-05-22 09:51:22.000000 aiocmcapi-0.7.1/aiocmcapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-05-22 09:51:22.000000 aiocmcapi-0.7.1/aiocmcapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:51:22.000000 aiocmcapi-0.7.1/aiocmcapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-22 09:51:22.000000 aiocmcapi-0.7.1/aiocmcapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-22 09:51:22.000000 aiocmcapi-0.7.1/aiocmcapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      354 2024-05-22 09:49:21.000000 aiocmcapi-0.7.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 09:51:22.347402 aiocmcapi-0.7.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 18:52:08.201615 aiocmcapi-0.7.2/
+-rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     3407 2024-05-23 18:52:08.200617 aiocmcapi-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3137 2024-05-22 09:50:20.000000 aiocmcapi-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 18:52:08.195613 aiocmcapi-0.7.2/aiocmcapi/
+-rw-rw-rw-   0        0        0       74 2024-05-23 06:15:57.000000 aiocmcapi-0.7.2/aiocmcapi/__init__.py
+-rw-rw-rw-   0        0        0     1071 2024-05-23 18:39:26.000000 aiocmcapi-0.7.2/aiocmcapi/client.py
+-rw-rw-rw-   0        0        0     1782 2024-05-23 08:12:53.000000 aiocmcapi-0.7.2/aiocmcapi/currency.py
+-rw-rw-rw-   0        0        0      291 2024-05-23 06:15:57.000000 aiocmcapi-0.7.2/aiocmcapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:52:08.199613 aiocmcapi-0.7.2/aiocmcapi.egg-info/
+-rw-rw-rw-   0        0        0     3407 2024-05-23 18:52:08.000000 aiocmcapi-0.7.2/aiocmcapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-23 18:52:08.000000 aiocmcapi-0.7.2/aiocmcapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 18:52:08.000000 aiocmcapi-0.7.2/aiocmcapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-23 18:52:08.000000 aiocmcapi-0.7.2/aiocmcapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 18:52:08.000000 aiocmcapi-0.7.2/aiocmcapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      348 2024-05-23 18:52:00.000000 aiocmcapi-0.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 18:52:08.201615 aiocmcapi-0.7.2/setup.cfg
```

### Comparing `aiocmcapi-0.7.1/LICENSE` & `aiocmcapi-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.7.1/PKG-INFO` & `aiocmcapi-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.7.1
+Version: 0.7.2
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.9.5
```

### Comparing `aiocmcapi-0.7.1/README.md` & `aiocmcapi-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.7.1/aiocmcapi/client.py` & `aiocmcapi-0.7.2/aiocmcapi/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from aiohttp import ClientSession
 
-from .exceptions import EndpointNotFoundError
+from .exceptions import EndpointNotFound
 
 class BaseClient:
     def __init__(self, api_key: str):
         self._session = ClientSession(
             base_url="http://pro-api.coinmarketcap.com",
             headers={
                 "X-CMC_PRO_API_KEY": api_key
@@ -27,14 +27,12 @@
             params=params
         ) as r:
             json = await r.json()
             if close:
                 await self.close_session()
             
             try:
-                if json['status']:
-                    pass
-            except:
-                await self.close_session()
-                raise EndpointNotFoundError(endpoint)
-
-            return json
+                if json['statusCode'] == 404:
+                    await self.close_session()
+                    raise EndpointNotFound(endpoint)
+            except KeyError:
+                return json
```

### Comparing `aiocmcapi-0.7.1/aiocmcapi/currency.py` & `aiocmcapi-0.7.2/aiocmcapi/currency.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,60 @@
 from typing import Any
 
-from .exceptions import ResponseDataError
+from .exceptions import NoDataResponse
 from .client import Client
 
-class Meta:
+class CurrencyMeta:
     def __init__(self, cmc_id: int):
         self.cmc_id = cmc_id
 
     async def update(self, client: Client):
         # 'async with' raises AttributeError: __aenter__
         r = await client.get(
             endpoint="/v2/cryptocurrency/info",
             params={'id': self.cmc_id},
             close=True
         )
 
         try:
-            self.meta.update(client)
             self.data = r['data'][str(self.cmc_id)]
         except KeyError:
-            raise ResponseDataError(status=r['status'])
+            raise NoDataResponse(status=r['status'])
         
     def __getattr__(self, __name: str) -> Any:
         return self.data[__name]
 
 class Currency:
     def __init__(self, cmc_id: int):
-        self.meta = Meta(cmc_id)
+        self.meta = CurrencyMeta(cmc_id)
         self.cmc_id = cmc_id
 
     async def update(self, client: Client):
         # 'async with' raises AttributeError: __aenter__
         r = await client.get(
             endpoint="/v2/cryptocurrency/quotes/latest",
             params={'id': self.cmc_id}
         )
+        await self.meta.update(client)
 
         try:
-            self.meta.update(client)
             self.data = r['data'][str(self.cmc_id)]
         except KeyError:
-            raise ResponseDataError(status=r['status'])
+            raise NoDataResponse(status=r['status'])
 
     def __getattr__(self, __name: str) -> Any:
-        return self.data[__name]
+        return self.data[__name]
+
+class CurrenciesList:
+    def __init__(self, cmc_ids: list):
+        self.currencies: list = []
+
+        for cmc_id in cmc_ids:
+            self.currencies.append(Currency(cmc_id))
+
+    async def update(self, api_key: str):
+        for currency in self.currencies:
+            client = Client(api_key)
+            await currency.update(client)
+    
+    def __getitem__(self, c_list_id: int):
+        return self.currencies[c_list_id]
```

### Comparing `aiocmcapi-0.7.1/aiocmcapi.egg-info/PKG-INFO` & `aiocmcapi-0.7.2/aiocmcapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.7.1
+Version: 0.7.2
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.9.5
```

