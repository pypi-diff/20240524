# Comparing `tmp/zamino_fix-1.1.7.tar.gz` & `tmp/zamino_fix-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zamino_fix-1.1.7.tar", last modified: Sun May 19 21:39:34 2024, max compression
+gzip compressed data, was "zamino_fix-1.1.8.tar", last modified: Thu May 23 22:49:05 2024, max compression
```

## Comparing `zamino_fix-1.1.7.tar` & `zamino_fix-1.1.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:39:34.408360 zamino_fix-1.1.7/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1083 2024-03-18 23:50:51.000000 zamino_fix-1.1.7/LICENSE
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-19 21:39:34.408360 zamino_fix-1.1.7/PKG-INFO
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      199 2024-03-18 23:53:23.000000 zamino_fix-1.1.7/README.md
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:39:34.408360 zamino_fix-1.1.7/ZAmino.fix.egg-info/
--rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      596 2024-05-19 21:39:34.000000 zamino_fix-1.1.7/ZAmino.fix.egg-info/PKG-INFO
--rw-------   0 u0_a303  (10303) u0_a303  (10303)      626 2024-05-19 21:39:34.000000 zamino_fix-1.1.7/ZAmino.fix.egg-info/SOURCES.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-05-19 21:39:34.000000 zamino_fix-1.1.7/ZAmino.fix.egg-info/dependency_links.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       76 2024-05-19 21:39:34.000000 zamino_fix-1.1.7/ZAmino.fix.egg-info/requires.txt
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       10 2024-05-19 21:39:34.000000 zamino_fix-1.1.7/ZAmino.fix.egg-info/top_level.txt
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:39:34.398359 zamino_fix-1.1.7/ZAminofix/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      423 2024-05-19 21:38:56.000000 zamino_fix-1.1.7/ZAminofix/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    12887 2023-01-20 09:14:27.000000 zamino_fix-1.1.7/ZAminofix/acm.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:39:34.408360 zamino_fix-1.1.7/ZAminofix/asyncfix/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      256 2023-01-20 07:25:50.000000 zamino_fix-1.1.7/ZAminofix/asyncfix/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13760 2023-01-20 07:25:50.000000 zamino_fix-1.1.7/ZAminofix/asyncfix/acm.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    98035 2023-05-21 20:55:10.000000 zamino_fix-1.1.7/ZAminofix/asyncfix/client.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13195 2023-05-21 21:07:37.000000 zamino_fix-1.1.7/ZAminofix/asyncfix/socket.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   110680 2023-04-06 18:02:18.000000 zamino_fix-1.1.7/ZAminofix/asyncfix/sub_client.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    94465 2024-05-12 08:17:35.000000 zamino_fix-1.1.7/ZAminofix/client.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:39:34.408360 zamino_fix-1.1.7/ZAminofix/lib/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)        0 2023-01-20 07:25:50.000000 zamino_fix-1.1.7/ZAminofix/lib/__init__.py
-drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-19 21:39:34.408360 zamino_fix-1.1.7/ZAminofix/lib/util/
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)       99 2023-01-20 09:15:29.000000 zamino_fix-1.1.7/ZAminofix/lib/util/__init__.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    31646 2023-01-20 07:25:50.000000 zamino_fix-1.1.7/ZAminofix/lib/util/exceptions.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     4088 2024-04-10 15:12:03.000000 zamino_fix-1.1.7/ZAminofix/lib/util/headers.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)     1215 2023-01-20 09:10:25.000000 zamino_fix-1.1.7/ZAminofix/lib/util/helpers.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   198201 2024-04-29 01:02:27.000000 zamino_fix-1.1.7/ZAminofix/lib/util/objects.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)    13852 2024-05-19 21:36:10.000000 zamino_fix-1.1.7/ZAminofix/socket.py
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)   107423 2024-05-13 10:55:56.000000 zamino_fix-1.1.7/ZAminofix/sub_client.py
--rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-05-19 21:39:34.408360 zamino_fix-1.1.7/setup.cfg
--rw-rw----   0 u0_a303  (10303) u0_a303  (10303)      698 2024-05-19 21:39:20.000000 zamino_fix-1.1.7/setup.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-23 22:49:05.624381 zamino_fix-1.1.8/
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)     1088 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/LICENSE
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      621 2024-05-23 22:49:05.624381 zamino_fix-1.1.8/PKG-INFO
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)      199 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/README.md
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-23 22:49:05.624381 zamino_fix-1.1.8/ZAmino.fix.egg-info/
+-rw-r--r--   0 u0_a303  (10303) u0_a303  (10303)      621 2024-05-23 22:49:05.000000 zamino_fix-1.1.8/ZAmino.fix.egg-info/PKG-INFO
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)      626 2024-05-23 22:49:05.000000 zamino_fix-1.1.8/ZAmino.fix.egg-info/SOURCES.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-05-23 22:49:05.000000 zamino_fix-1.1.8/ZAmino.fix.egg-info/dependency_links.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       85 2024-05-23 22:49:05.000000 zamino_fix-1.1.8/ZAmino.fix.egg-info/requires.txt
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       10 2024-05-23 22:49:05.000000 zamino_fix-1.1.8/ZAmino.fix.egg-info/top_level.txt
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-23 22:49:05.614381 zamino_fix-1.1.8/ZAminofix/
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)     1328 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/__init__.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)    12887 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/acm.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-23 22:49:05.614381 zamino_fix-1.1.8/ZAminofix/asyncfix/
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)      262 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/asyncfix/__init__.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)    13760 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/asyncfix/acm.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)    98035 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/asyncfix/client.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)    13638 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/asyncfix/socket.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)   110832 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/asyncfix/sub_client.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)    94465 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/client.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-23 22:49:05.614381 zamino_fix-1.1.8/ZAminofix/lib/
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)        1 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/lib/__init__.py
+drwx------   0 u0_a303  (10303) u0_a303  (10303)        0 2024-05-23 22:49:05.624381 zamino_fix-1.1.8/ZAminofix/lib/util/
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       99 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/lib/util/__init__.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)    31646 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/lib/util/exceptions.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)     4088 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/lib/util/headers.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)     1215 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/lib/util/helpers.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)   198201 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/lib/util/objects.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)    14219 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/socket.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)   107685 2024-05-23 22:47:42.000000 zamino_fix-1.1.8/ZAminofix/sub_client.py
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)       38 2024-05-23 22:49:05.624381 zamino_fix-1.1.8/setup.cfg
+-rw-------   0 u0_a303  (10303) u0_a303  (10303)      716 2024-05-23 22:48:07.000000 zamino_fix-1.1.8/setup.py
```

### Comparing `zamino_fix-1.1.7/LICENSE` & `zamino_fix-1.1.8/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 ZOOM37Z
+Copyright (c) 2024 zoom-Adham
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `zamino_fix-1.1.7/PKG-INFO` & `zamino_fix-1.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ZAmino.fix
-Version: 1.1.7
+Version: 1.1.8
 Summary: Aminofix update. https://t.me/ZAminoZ
 Author: ZOOM
-Keywords: ZAminoZAmino.fixaminoapps,ZAminofix,amino,amino-bot
+Keywords: ZAmino,ZAmino.fixaminoapps,ZAminofix,amino,amino-bot
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: websocket-client==1.3.1
 Requires-Dist: setuptools
 Requires-Dist: json_minify
 Requires-Dist: six
 Requires-Dist: aiohttp
 Requires-Dist: websockets
+Requires-Dist: colorama
 
 ### Telegram
 `https://t.me/ZAminoZ`
 ### About lib
 `Fix amino.fix`
 ### How to install?
 `pip install ZAmino.fix`
```

### Comparing `zamino_fix-1.1.7/ZAmino.fix.egg-info/PKG-INFO` & `zamino_fix-1.1.8/ZAmino.fix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ZAmino.fix
-Version: 1.1.7
+Version: 1.1.8
 Summary: Aminofix update. https://t.me/ZAminoZ
 Author: ZOOM
-Keywords: ZAminoZAmino.fixaminoapps,ZAminofix,amino,amino-bot
+Keywords: ZAmino,ZAmino.fixaminoapps,ZAminofix,amino,amino-bot
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: websocket-client==1.3.1
 Requires-Dist: setuptools
 Requires-Dist: json_minify
 Requires-Dist: six
 Requires-Dist: aiohttp
 Requires-Dist: websockets
+Requires-Dist: colorama
 
 ### Telegram
 `https://t.me/ZAminoZ`
 ### About lib
 `Fix amino.fix`
 ### How to install?
 `pip install ZAmino.fix`
```

### Comparing `zamino_fix-1.1.7/ZAmino.fix.egg-info/SOURCES.txt` & `zamino_fix-1.1.8/ZAmino.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.7/ZAminofix/acm.py` & `zamino_fix-1.1.8/ZAminofix/acm.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.7/ZAminofix/asyncfix/acm.py` & `zamino_fix-1.1.8/ZAminofix/asyncfix/acm.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.7/ZAminofix/asyncfix/client.py` & `zamino_fix-1.1.8/ZAminofix/asyncfix/client.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.7/ZAminofix/asyncfix/socket.py` & `zamino_fix-1.1.8/ZAminofix/asyncfix/socket.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,29 +24,38 @@
         if self.socket_enabled:
             self.reconnect_thread = Thread(target=self.reconnect_handler)
             self.reconnect_thread.start()
 
         websocket.enableTrace(socket_trace)
 
     def reconnect_handler(self):
-        # Made by enchart#3410 thx
-        # Fixed by The_Phoenix#3967
         while True:
             time.sleep(self.reconnectTime)
 
             if self.active:
                 if self.debug is True:
                     print(f"[socket][reconnect_handler] Reconnecting Socket")
 
                 self.close()
                 self.run_amino_socket()
 
     def handle_message(self, ws, data):
         self.client.handle_socket_message(data)
         return
+    def handle_close(self, ws, close_status_code, close_msg):
+        if self.debug:
+            print(f"[socket][close] Socket closed: {close_status_code} - {close_msg}")
+        self.active = False
+        self.run_amino_socket()
+
+    def handle_error(self, ws, error):
+        if self.debug:
+            print(f"[socket][error] Socket error: {error}")
+        self.active = False
+        self.run_amino_socket()
 
     def send(self, data):
         if self.debug is True:
             print(f"[socket][send] Sending Data : {data}")
         
         if not self.socket_thread:
             self.run_amino_socket()
@@ -69,15 +78,17 @@
                 "NDCAUTH": f"sid={self.client.sid}",
                 "NDC-MSG-SIG": helpers.signature(final)
             }
 
             self.socket = websocket.WebSocketApp(
                 f"{self.socket_url}/?signbody={final.replace('|', '%7C')}",
                 on_message = self.handle_message,
-                header = self.headers
+                on_close=self.handle_close,
+                on_error=self.handle_error,
+                header=self.headers
             )
 
             self.active = True
             self.socket_thread = Thread(target=self.socket.run_forever)
             self.socket_thread.start()
 
             if self.reconnect_thread is None:
@@ -251,8 +262,8 @@
     def on_timestamp_message(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]).Event)
     def on_welcome_message(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]).Event)
     def on_invite_message(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]).Event)
 
     def on_user_typing_start(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]).Event)
     def on_user_typing_end(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]).Event)
 
-    def default(self, data): self.call(getframe(0).f_code.co_name, data)
+    def default(self, data): self.call(getframe(0).f_code.co_name, data)
```

### Comparing `zamino_fix-1.1.7/ZAminofix/asyncfix/sub_client.py` & `zamino_fix-1.1.8/ZAminofix/asyncfix/sub_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,36 +27,43 @@
         }
 
         if data: vc_headers["Content-Length"] = str(len(data))
         self.vc_headers = vc_headers
 
 
 class SubClient(client.Client):
-    def __init__(self, comId: str = None, aminoId: str = None, *, profile: objects.UserProfile, deviceId: str = None, proxies: dict = None, certificatePath: str = None):
+    def __init__(self,community_link: str = None ,comId: str = None, aminoId: str = None, *, profile: objects.UserProfile, deviceId: str = None, proxies: dict = None, certificatePath: str = None):
         client.Client.__init__(self, deviceId=deviceId, sub=True, proxies=proxies, certificatePath=certificatePath)
         self.vc_connect = False
         self.comId = comId
         self.aminoId = aminoId
         self.profile: objects.UserProfile = profile
         self.community: objects.Community
 
     def __await__(self):
         return self._init().__await__()
 
     async def _init(self):
-        if self.comId is not None:
-            self.community: objects.Community = await self.get_community_info(self.comId)
-        if self.aminoId is not None:
-            self.comId = (await client.Client().search_community(self.aminoId)).comId[0]
-            self.community: objects.Community = await client.Client().get_community_info(self.comId)
-        if self.comId is None and self.aminoId is None: raise exceptions.NoCommunity()
-        try: self.profile: objects.UserProfile = await self.get_user_info(userId=self.profile.userId)
-        except AttributeError: raise exceptions.FailedLogin()
-        except exceptions.UserUnavailable(): pass
-        return self
+        if comId is not None:
+            self.comId = comId
+            self.community: objects.Community = await self.get_community_info_async(comId)
+
+        if aminoId is not None:
+            link = "http://aminoapps.com/c/"
+            self.comId = (await self.get_from_code_async(link + aminoId)).comId
+            self.community: objects.Community = await self.get_community_info_async(self.comId)
+    
+        if comId is None and community_link is not None:
+            self.comId = (await self.get_from_code_async(community_link)).comId
+            self.community: objects.Community = await self.get_community_info_async(self.comId)
+    
+        if comId is None and aminoId is None and community_link is None: 
+            raise exceptions.NoCommunity()
+
+            return self
 
     def __del__(self):
         try:
             loop = asyncio.get_event_loop()
             loop.create_task(self._close_session())
         except RuntimeError:
             loop = asyncio.new_event_loop()
```

### Comparing `zamino_fix-1.1.7/ZAminofix/client.py` & `zamino_fix-1.1.8/ZAminofix/client.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.7/ZAminofix/lib/util/exceptions.py` & `zamino_fix-1.1.8/ZAminofix/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.7/ZAminofix/lib/util/headers.py` & `zamino_fix-1.1.8/ZAminofix/lib/util/headers.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.7/ZAminofix/lib/util/helpers.py` & `zamino_fix-1.1.8/ZAminofix/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.7/ZAminofix/lib/util/objects.py` & `zamino_fix-1.1.8/ZAminofix/lib/util/objects.py`

 * *Files identical despite different names*

### Comparing `zamino_fix-1.1.7/ZAminofix/socket.py` & `zamino_fix-1.1.8/ZAminofix/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import time
 import json
 import websocket
 import contextlib
 
-from threading import Thread
+from threading import Thread, Lock
 from sys import _getframe as getframe
 
 from .lib.util.helpers import gen_deviceId
 from .lib.util import objects, helpers
 
 class SocketHandler:
     SOCKET_URL = "wss://ws1.aminoapps.com"
     RECONNECT_TIME = 180
 
-    def __init__(self, client, socket_trace=False, debug=False):
+    def __init__(self, client, socket_trace=False, debug=True):
         self.socket_url = self.SOCKET_URL
         self.client = client
         self.debug = debug
         self.active = False
         self.headers = None
         self.socket = None
         self.socket_thread = None
         self.reconnect_thread = None
-        self.previous_socket = None  # Added to keep track of the previous socket
+        self.lock = Lock()
+        self.previous_socket = None
 
         websocket.enableTrace(socket_trace)
         self.run_amino_socket()
 
     def reconnect_handler(self):
         while True:
             time.sleep(self.RECONNECT_TIME)
@@ -39,19 +40,22 @@
     def handle_message(self, ws, data):
         self.client.handle_socket_message(data)
 
     def handle_close(self, ws, close_status_code, close_msg):
         if self.debug:
             print(f"[socket][close] Socket closed: {close_status_code} - {close_msg}")
         self.active = False
+        self.run_amino_socket()
+        
 
     def handle_error(self, ws, error):
         if self.debug:
             print(f"[socket][error] Socket error: {error}")
         self.active = False
+        self.run_amino_socket()
 
     def send(self, data):
         if self.debug:
             print(f"[socket][send] Sending Data: {data}")
         
         if not self.socket_thread or not self.socket_thread.is_alive():
             self.run_amino_socket()
@@ -60,61 +64,65 @@
             self.socket.send(data)
         except Exception as e:
             if self.debug:
                 print(f"[socket][send] Error sending data: {e}")
             self.run_amino_socket()
 
     def run_amino_socket(self):
-        try:
-            if self.debug:
-                print(f"[socket][start] Starting Socket")
+        with self.lock:
+            try:
+                if self.debug:
+                    print(f"[socket][start] Starting Socket")
 
-            if not self.client.sid:
-                return
+                if not self.client.sid:
+                    return
 
-            final = f"{self.client.device_id}|{int(time.time() * 1000)}"
-            self.headers = {
-                "NDCDEVICEID": gen_deviceId() if self.client.autoDevice else self.client.device_id,
-                "NDCAUTH": f"sid={self.client.sid}",
-                "NDC-MSG-SIG": helpers.signature(final)
-            }
-
-            self.socket = websocket.WebSocketApp(
-                f"{self.socket_url}/?signbody={final.replace('|', '%7C')}",
-                on_message=self.handle_message,
-                on_close=self.handle_close,
-                on_error=self.handle_error,
-                header=self.headers
-            )
-
-            self.active = True
-            self.previous_socket = self.socket
-            self.socket_thread = Thread(target=self.socket.run_forever)
-            self.socket_thread.start()
-
-            if not self.reconnect_thread:
-                self.reconnect_thread = Thread(target=self.reconnect_handler)
-                self.reconnect_thread.start()
-            
-            if self.debug:
-                print(f"[socket][start] Socket Started")
-        except Exception as e:
-            if self.debug:
-                print(f"[socket][start] Error starting socket: {e}")
+                final = f"{self.client.device_id}|{int(time.time() * 1000)}"
+                self.headers = {
+                    "NDCDEVICEID": gen_deviceId() if self.client.autoDevice else self.client.device_id,
+                    "NDCAUTH": f"sid={self.client.sid}",
+                    "NDC-MSG-SIG": helpers.signature(final)
+                }
+                if self.previous_socket:
+                    self.previous_socket.close()
+
+                self.socket = websocket.WebSocketApp(
+                    f"{self.socket_url}/?signbody={final.replace('|', '%7C')}",
+                    on_message=self.handle_message,
+                    on_close=self.handle_close,
+                    on_error=self.handle_error,
+                    header=self.headers
+                )
+
+                self.active = True
+                self.previous_socket = self.socket
+                self.socket_thread = Thread(target=self.socket.run_forever)
+                self.socket_thread.start()
+
+                if not self.reconnect_thread:
+                    self.reconnect_thread = Thread(target=self.reconnect_handler)
+                    self.reconnect_thread.start()
+                
+                if self.debug:
+                    print(f"[socket][start] Socket Started")
+            except Exception as e:
+                if self.debug:
+                    print(f"[socket][start] Error starting socket: {e}")
 
     def close(self):
-        if self.debug:
-            print(f"[socket][close] Closing Socket")
-        self.active = False
-        try:
-            if self.previous_socket:
-                self.previous_socket.close()
-        except Exception as closeError:
+        with self.lock:
             if self.debug:
-                print(f"[socket][close] Error while closing Socket: {closeError}")
+                print(f"[socket][close] Closing Socket")
+            self.active = False
+            try:
+                if self.previous_socket:
+                    self.previous_socket.close()
+            except Exception as closeError:
+                if self.debug:
+                    print(f"[socket][close] Error while closing Socket: {closeError}")
 
 
 class Callbacks:
     def __init__(self, client):
         self.client = client
         self.handlers = {}
 
@@ -262,8 +270,8 @@
     def on_timestamp_message(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]).Event)
     def on_welcome_message(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]).Event)
     def on_invite_message(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]).Event)
 
     def on_user_typing_start(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]).Event)
     def on_user_typing_end(self, data): self.call(getframe(0).f_code.co_name, objects.Event(data["o"]).Event)
 
-    def default(self, data): self.call(getframe(0).f_code.co_name, data)
+    def default(self, data): self.call(getframe(0).f_code.co_name, data)
```

### Comparing `zamino_fix-1.1.7/ZAminofix/sub_client.py` & `zamino_fix-1.1.8/ZAminofix/sub_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,28 +29,30 @@
         }
 
         if data: vc_headers["Content-Length"] = str(len(data))
         self.vc_headers = vc_headers
 
 
 class SubClient(client.Client):
-    def __init__(self, comId: str = None, aminoId: str = None, deviceId: str = None, autoDevice: bool = False, proxies: dict = None, certificatePath: str = None):
+    def __init__(self,community_link: str = None, comId: str = None, aminoId: str = None, deviceId: str = None, autoDevice: bool = False, proxies: dict = None, certificatePath: str = None):
         client.Client.__init__(self, deviceId=deviceId, sub=True, proxies=proxies, certificatePath=certificatePath)
         self.vc_connect = False
 
         if comId is not None:
             self.comId = comId
             self.community: objects.Community = self.get_community_info(comId)
 
         if aminoId is not None:
             link = "http://aminoapps.com/c/"
             self.comId = self.get_from_code(link + aminoId).comId
             self.community: objects.Community = self.get_community_info(self.comId)
-
-        if comId is None and aminoId is None: raise exceptions.NoCommunity()
+        if comId is None and community_link is not None:
+            self.comId = self.get_from_code(community_link).comId
+            self.community: objects.Community = self.get_community_info(self.comId)
+        if comId is None and aminoId is None and community_link is None: raise exceptions.NoCommunity()
 
 
 
     def parse_headers(self, data: str = None, type: str = None) -> dict:
         return headers.ApisHeaders(deviceId=gen_deviceId() if self.autoDevice else self.device_id, data=data, type=type).headers
 
     def get_invite_codes(self, status: str = "normal", start: int = 0, size: int = 25) -> objects.InviteCodeList:
```

### Comparing `zamino_fix-1.1.7/setup.py` & `zamino_fix-1.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 requirements = [
     "httpx",
     "websocket-client==1.3.1", 
     "setuptools", 
     "json_minify", 
     "six",
     "aiohttp",
-    "websockets"
+    "websockets",
+    "colorama"
 ]
 
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 setup(
     name="ZAmino.fix",
     author="ZOOM",
-    version="1.1.7",
+    version="1.1.8",
     description="Aminofix update. https://t.me/ZAminoZ",
     packages=find_packages(),
     long_description=long_description,
     install_requires=requirements,
     keywords=[
-    	'ZAmino'
+    	'ZAmino',
     	'ZAmino.fix'
         'aminoapps',
         'ZAminofix',
         'amino',
         'amino-bot',
     ],
     python_requires='>=3.6',
```

