# Comparing `tmp/aiocmcapi-0.7.2.tar.gz` & `tmp/aiocmcapi-0.7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocmcapi-0.7.2.tar", last modified: Thu May 23 18:52:08 2024, max compression
+gzip compressed data, was "aiocmcapi-0.7.2.1.tar", last modified: Fri May 24 06:46:51 2024, max compression
```

## Comparing `aiocmcapi-0.7.2.tar` & `aiocmcapi-0.7.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 18:52:08.201615 aiocmcapi-0.7.2/
--rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.7.2/LICENSE
--rw-rw-rw-   0        0        0     3407 2024-05-23 18:52:08.200617 aiocmcapi-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     3137 2024-05-22 09:50:20.000000 aiocmcapi-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 18:52:08.195613 aiocmcapi-0.7.2/aiocmcapi/
--rw-rw-rw-   0        0        0       74 2024-05-23 06:15:57.000000 aiocmcapi-0.7.2/aiocmcapi/__init__.py
--rw-rw-rw-   0        0        0     1071 2024-05-23 18:39:26.000000 aiocmcapi-0.7.2/aiocmcapi/client.py
--rw-rw-rw-   0        0        0     1782 2024-05-23 08:12:53.000000 aiocmcapi-0.7.2/aiocmcapi/currency.py
--rw-rw-rw-   0        0        0      291 2024-05-23 06:15:57.000000 aiocmcapi-0.7.2/aiocmcapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:52:08.199613 aiocmcapi-0.7.2/aiocmcapi.egg-info/
--rw-rw-rw-   0        0        0     3407 2024-05-23 18:52:08.000000 aiocmcapi-0.7.2/aiocmcapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-05-23 18:52:08.000000 aiocmcapi-0.7.2/aiocmcapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 18:52:08.000000 aiocmcapi-0.7.2/aiocmcapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-23 18:52:08.000000 aiocmcapi-0.7.2/aiocmcapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 18:52:08.000000 aiocmcapi-0.7.2/aiocmcapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      348 2024-05-23 18:52:00.000000 aiocmcapi-0.7.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 18:52:08.201615 aiocmcapi-0.7.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 06:46:51.919822 aiocmcapi-0.7.2.1/
+-rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.7.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4129 2024-05-24 06:46:51.918820 aiocmcapi-0.7.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3857 2024-05-24 06:32:06.000000 aiocmcapi-0.7.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 06:46:51.913821 aiocmcapi-0.7.2.1/aiocmcapi/
+-rw-rw-rw-   0        0        0       58 2024-05-24 06:23:16.000000 aiocmcapi-0.7.2.1/aiocmcapi/__init__.py
+-rw-rw-rw-   0        0        0     1071 2024-05-23 18:39:26.000000 aiocmcapi-0.7.2.1/aiocmcapi/client.py
+-rw-rw-rw-   0        0        0     1989 2024-05-24 06:26:28.000000 aiocmcapi-0.7.2.1/aiocmcapi/currency.py
+-rw-rw-rw-   0        0        0      291 2024-05-23 06:15:57.000000 aiocmcapi-0.7.2.1/aiocmcapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:46:51.917819 aiocmcapi-0.7.2.1/aiocmcapi.egg-info/
+-rw-rw-rw-   0        0        0     4129 2024-05-24 06:46:51.000000 aiocmcapi-0.7.2.1/aiocmcapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-24 06:46:51.000000 aiocmcapi-0.7.2.1/aiocmcapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 06:46:51.000000 aiocmcapi-0.7.2.1/aiocmcapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-24 06:46:51.000000 aiocmcapi-0.7.2.1/aiocmcapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-24 06:46:51.000000 aiocmcapi-0.7.2.1/aiocmcapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      350 2024-05-24 06:45:51.000000 aiocmcapi-0.7.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 06:46:51.919822 aiocmcapi-0.7.2.1/setup.cfg
```

### Comparing `aiocmcapi-0.7.2/LICENSE` & `aiocmcapi-0.7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.7.2/PKG-INFO` & `aiocmcapi-0.7.2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.7.2
+Version: 0.7.2.1
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.9.5
 
@@ -112,14 +112,48 @@
 
 ```
 Bitcoin | BTC
 Description: Bitcoin (BTC) is a cryptocurrency launched in 2010. Users are able to generate BTC through the process of mining. Bitcoin has a current supply of 19,700,812. The last known price of Bitcoin is 66,941.7329356 USD and is down -0.14 over the last 24 hours. It is currently trading on 11048 active market(s) with $23,083,624,310.30 traded over the last 24 hours. More information can be found at https://bitcoin.org/.
 Website: https://bitcoin.org/
 ```
 
+### For multiple currencies
+
+```py
+import asyncio
+
+from aiocmcapi.currency import CurrenciesList
+
+async def main():
+    currencies = CurrenciesList(
+        cmc_ids=[1, 1027],
+        update_api_key="YOUR_API_KEY_HERE"
+    )
+    await currencies.update_all()
+    # to update one currency -> await currencies.update(c_list_id: int)
+    # example: await currencies.update(0) -> Currency(cmc_id=1).update(self.api_key)
+    
+    # currencies[0] -> Currency(cmc_id=1)
+    # currencies[1] -> Currency(cmc_id=1027)
+    btc = currencies[0]
+    eth = currencies[1]
+
+    print(f"{btc.name}\n{eth.name}")
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+Output:
+
+```
+Bitcoin
+Ethereum
+```
+
 ## Example for other API endpoints
 
 [CoinMarketCap API endpoint overview](https://coinmarketcap.com/api/documentation/v1/#section/Endpoint-Overview)
 
 ```py
 import asyncio
```

### Comparing `aiocmcapi-0.7.2/README.md` & `aiocmcapi-0.7.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -102,14 +102,48 @@
 
 ```
 Bitcoin | BTC
 Description: Bitcoin (BTC) is a cryptocurrency launched in 2010. Users are able to generate BTC through the process of mining. Bitcoin has a current supply of 19,700,812. The last known price of Bitcoin is 66,941.7329356 USD and is down -0.14 over the last 24 hours. It is currently trading on 11048 active market(s) with $23,083,624,310.30 traded over the last 24 hours. More information can be found at https://bitcoin.org/.
 Website: https://bitcoin.org/
 ```
 
+### For multiple currencies
+
+```py
+import asyncio
+
+from aiocmcapi.currency import CurrenciesList
+
+async def main():
+    currencies = CurrenciesList(
+        cmc_ids=[1, 1027],
+        update_api_key="YOUR_API_KEY_HERE"
+    )
+    await currencies.update_all()
+    # to update one currency -> await currencies.update(c_list_id: int)
+    # example: await currencies.update(0) -> Currency(cmc_id=1).update(self.api_key)
+    
+    # currencies[0] -> Currency(cmc_id=1)
+    # currencies[1] -> Currency(cmc_id=1027)
+    btc = currencies[0]
+    eth = currencies[1]
+
+    print(f"{btc.name}\n{eth.name}")
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+Output:
+
+```
+Bitcoin
+Ethereum
+```
+
 ## Example for other API endpoints
 
 [CoinMarketCap API endpoint overview](https://coinmarketcap.com/api/documentation/v1/#section/Endpoint-Overview)
 
 ```py
 import asyncio
```

### Comparing `aiocmcapi-0.7.2/aiocmcapi/client.py` & `aiocmcapi-0.7.2.1/aiocmcapi/client.py`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.7.2/aiocmcapi/currency.py` & `aiocmcapi-0.7.2.1/aiocmcapi/currency.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,20 +41,25 @@
         except KeyError:
             raise NoDataResponse(status=r['status'])
 
     def __getattr__(self, __name: str) -> Any:
         return self.data[__name]
 
 class CurrenciesList:
-    def __init__(self, cmc_ids: list):
+    def __init__(self, update_api_key: str, cmc_ids: list):
         self.currencies: list = []
+        self.api_key: str = update_api_key
 
         for cmc_id in cmc_ids:
             self.currencies.append(Currency(cmc_id))
 
-    async def update(self, api_key: str):
+    async def update_all(self):
         for currency in self.currencies:
-            client = Client(api_key)
+            client = Client(self.api_key)
             await currency.update(client)
     
+    async def update(self, c_list_id: int):
+        client = Client(self.api_key)
+        await self.currencies[c_list_id].update(client)
+    
     def __getitem__(self, c_list_id: int):
         return self.currencies[c_list_id]
```

### Comparing `aiocmcapi-0.7.2/aiocmcapi.egg-info/PKG-INFO` & `aiocmcapi-0.7.2.1/aiocmcapi.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.7.2
+Version: 0.7.2.1
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.9.5
 
@@ -112,14 +112,48 @@
 
 ```
 Bitcoin | BTC
 Description: Bitcoin (BTC) is a cryptocurrency launched in 2010. Users are able to generate BTC through the process of mining. Bitcoin has a current supply of 19,700,812. The last known price of Bitcoin is 66,941.7329356 USD and is down -0.14 over the last 24 hours. It is currently trading on 11048 active market(s) with $23,083,624,310.30 traded over the last 24 hours. More information can be found at https://bitcoin.org/.
 Website: https://bitcoin.org/
 ```
 
+### For multiple currencies
+
+```py
+import asyncio
+
+from aiocmcapi.currency import CurrenciesList
+
+async def main():
+    currencies = CurrenciesList(
+        cmc_ids=[1, 1027],
+        update_api_key="YOUR_API_KEY_HERE"
+    )
+    await currencies.update_all()
+    # to update one currency -> await currencies.update(c_list_id: int)
+    # example: await currencies.update(0) -> Currency(cmc_id=1).update(self.api_key)
+    
+    # currencies[0] -> Currency(cmc_id=1)
+    # currencies[1] -> Currency(cmc_id=1027)
+    btc = currencies[0]
+    eth = currencies[1]
+
+    print(f"{btc.name}\n{eth.name}")
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+Output:
+
+```
+Bitcoin
+Ethereum
+```
+
 ## Example for other API endpoints
 
 [CoinMarketCap API endpoint overview](https://coinmarketcap.com/api/documentation/v1/#section/Endpoint-Overview)
 
 ```py
 import asyncio
```

