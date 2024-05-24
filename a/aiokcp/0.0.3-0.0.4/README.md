# Comparing `tmp/aiokcp-0.0.3.tar.gz` & `tmp/aiokcp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiokcp-0.0.3.tar", last modified: Tue May 21 02:19:40 2024, max compression
+gzip compressed data, was "aiokcp-0.0.4.tar", last modified: Fri May 24 06:48:29 2024, max compression
```

## Comparing `aiokcp-0.0.3.tar` & `aiokcp-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 02:19:40.516199 aiokcp-0.0.3/
--rw-rw-rw-   0        0        0     1088 2024-05-20 09:29:30.000000 aiokcp-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    12498 2024-05-21 02:19:40.510198 aiokcp-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    11758 2024-05-20 11:51:58.000000 aiokcp-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 02:19:40.449152 aiokcp-0.0.3/aiokcp/
--rw-rw-rw-   0        0        0      290 2024-05-13 01:37:48.000000 aiokcp-0.0.3/aiokcp/__init__.py
--rw-rw-rw-   0        0        0    15330 2024-05-21 02:17:57.000000 aiokcp-0.0.3/aiokcp/core.py
--rw-rw-rw-   0        0        0     1397 2024-05-21 02:18:10.000000 aiokcp-0.0.3/aiokcp/crypto.py
--rw-rw-rw-   0        0        0      308 2024-05-13 08:47:58.000000 aiokcp-0.0.3/aiokcp/exceptions.py
--rw-rw-rw-   0        0        0    33114 2024-05-13 08:39:55.000000 aiokcp-0.0.3/aiokcp/ikcp.c
--rw-rw-rw-   0        0        0    12436 2024-05-13 08:40:42.000000 aiokcp-0.0.3/aiokcp/ikcp.h
--rw-rw-rw-   0        0        0   744822 2024-05-20 15:40:22.000000 aiokcp-0.0.3/aiokcp/kcp.c
--rw-rw-rw-   0        0        0     1870 2024-05-20 07:35:38.000000 aiokcp-0.0.3/aiokcp/kcp.pyi
--rw-rw-rw-   0        0        0     1275 2024-05-14 03:27:01.000000 aiokcp-0.0.3/aiokcp/stream.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:19:40.497201 aiokcp-0.0.3/aiokcp/sync/
--rw-rw-rw-   0        0        0      286 2024-05-15 12:41:39.000000 aiokcp-0.0.3/aiokcp/sync/__init__.py
--rw-rw-rw-   0        0        0     3639 2024-05-20 07:36:56.000000 aiokcp-0.0.3/aiokcp/sync/server.py
--rw-rw-rw-   0        0        0    15660 2024-05-21 02:16:51.000000 aiokcp-0.0.3/aiokcp/sync/sock.py
--rw-rw-rw-   0        0        0      301 2024-05-21 02:18:28.000000 aiokcp-0.0.3/aiokcp/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-21 02:19:40.505200 aiokcp-0.0.3/aiokcp.egg-info/
--rw-rw-rw-   0        0        0    12498 2024-05-21 02:19:40.000000 aiokcp-0.0.3/aiokcp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      417 2024-05-21 02:19:40.000000 aiokcp-0.0.3/aiokcp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 02:19:40.000000 aiokcp-0.0.3/aiokcp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-21 02:19:40.000000 aiokcp-0.0.3/aiokcp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 02:19:40.000000 aiokcp-0.0.3/aiokcp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      816 2024-05-21 02:19:15.000000 aiokcp-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 02:19:40.516199 aiokcp-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      637 2024-05-21 02:09:25.000000 aiokcp-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:48:29.298126 aiokcp-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2024-05-20 09:29:30.000000 aiokcp-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    12933 2024-05-24 06:48:29.293125 aiokcp-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12193 2024-05-24 06:31:44.000000 aiokcp-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 06:48:29.235127 aiokcp-0.0.4/aiokcp/
+-rw-rw-rw-   0        0        0      290 2024-05-13 01:37:48.000000 aiokcp-0.0.4/aiokcp/__init__.py
+-rw-rw-rw-   0        0        0    15410 2024-05-21 03:35:08.000000 aiokcp-0.0.4/aiokcp/core.py
+-rw-rw-rw-   0        0        0     2975 2024-05-24 02:15:56.000000 aiokcp-0.0.4/aiokcp/crypto.py
+-rw-rw-rw-   0        0        0      308 2024-05-13 08:47:58.000000 aiokcp-0.0.4/aiokcp/exceptions.py
+-rw-rw-rw-   0        0        0    33114 2024-05-13 08:39:55.000000 aiokcp-0.0.4/aiokcp/ikcp.c
+-rw-rw-rw-   0        0        0    12436 2024-05-13 08:40:42.000000 aiokcp-0.0.4/aiokcp/ikcp.h
+-rw-rw-rw-   0        0        0   744822 2024-05-20 15:40:22.000000 aiokcp-0.0.4/aiokcp/kcp.c
+-rw-rw-rw-   0        0        0     1870 2024-05-20 07:35:38.000000 aiokcp-0.0.4/aiokcp/kcp.pyi
+-rw-rw-rw-   0        0        0     1275 2024-05-14 03:27:01.000000 aiokcp-0.0.4/aiokcp/stream.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:48:29.279127 aiokcp-0.0.4/aiokcp/sync/
+-rw-rw-rw-   0        0        0      286 2024-05-15 12:41:39.000000 aiokcp-0.0.4/aiokcp/sync/__init__.py
+-rw-rw-rw-   0        0        0     3639 2024-05-20 07:36:56.000000 aiokcp-0.0.4/aiokcp/sync/server.py
+-rw-rw-rw-   0        0        0    15660 2024-05-21 02:16:51.000000 aiokcp-0.0.4/aiokcp/sync/sock.py
+-rw-rw-rw-   0        0        0      301 2024-05-21 02:18:28.000000 aiokcp-0.0.4/aiokcp/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 06:48:29.288127 aiokcp-0.0.4/aiokcp.egg-info/
+-rw-rw-rw-   0        0        0    12933 2024-05-24 06:48:29.000000 aiokcp-0.0.4/aiokcp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2024-05-24 06:48:29.000000 aiokcp-0.0.4/aiokcp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 06:48:29.000000 aiokcp-0.0.4/aiokcp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-24 06:48:29.000000 aiokcp-0.0.4/aiokcp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-24 06:48:29.000000 aiokcp-0.0.4/aiokcp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      816 2024-05-24 06:32:04.000000 aiokcp-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 06:48:29.298126 aiokcp-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      637 2024-05-21 02:09:25.000000 aiokcp-0.0.4/setup.py
```

### Comparing `aiokcp-0.0.3/LICENSE` & `aiokcp-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.3/PKG-INFO` & `aiokcp-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokcp
-Version: 0.0.3
+Version: 0.0.4
 Summary: KCP for asyncio and socketserver, based on kcp
 Author: ryanrain2016
 Author-email: ryanrain2016 <holidaylover2010@gmail.com>
 Project-URL: Homepage, https://github.com/ryanrain2016/aiokcp
 Project-URL: Issues, https://github.com/ryanrain2016/aiokcp/issues
 Keywords: asyncio,kcp,socket,aio,aiokcp
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,24 @@
 
 # aiokcp
 [kcp](https://github.com/skywind3000/kcp)的python实践, 提供了类似python中TCP相关的标准库相同的编程接口(asyncio, socket, socketserver)，原tcp代码使用修改导入的方式可以轻松实现从tcp到kcp的平移替换。
 
 ## 什么是KCP？
 KCP是一个致力于低延时的基于UDP自动重传的可靠传输协议。本身不包含任何网络传输的功能，使用回调的方式处理udp数据包的传输。详情见[kcp](https://github.com/skywind3000/kcp)
 
+## 如何安装
+`aiokcp`是基于cython绑定调用的kcp库，打包可能需要安装平台的编译工具。windows系统需要安装`vsbuilder`，linux系统需要安装`gcc`。安装完成后，可以通过`pip`安装
+```bash
+pip install aiokcp
+```
+如果需要数据包加密，可以选择安装`cryptography`
+```bash
+pip install aiokcp[crypto]
+```
+
 ## 例子
 例子详见`aiokcp/examples`目录
 ### asyncio 低级接口
 这里实现了类似`loop.create_connection`和`loop.create_server`的功能
 ```py
 import asyncio
 import time
@@ -334,15 +344,15 @@
         port = randint(10000, 20000)
         server_thread(port)
         client_thread(port)
 
     thread_test()
 ```
 ### 可选的udp数据包加密
-内置的加密方法需要安装`cryptography`, 默认采用的aes+cbc模式加密。也可以自定义加密对象, 只需要实现`encrypt`和`decrypt`方法即可
+默认数据包不加密，但提供加密的方法和参数。内置的加密方法需要安装`cryptography`, 采用的aes+cbc模式加密+hmac校验。也可以自定义加密对象, 只需要实现`encrypt`和`decrypt`方法即可
 ```py
 from aiokcp import (create_connection, create_server, open_connection,
                     start_server)
 from aiokcp.crypto import get_crypto
 from aiokcp.sync import KCPSocket
 
 # need cryptography installed
```

### Comparing `aiokcp-0.0.3/README.md` & `aiokcp-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # aiokcp
 [kcp](https://github.com/skywind3000/kcp)的python实践, 提供了类似python中TCP相关的标准库相同的编程接口(asyncio, socket, socketserver)，原tcp代码使用修改导入的方式可以轻松实现从tcp到kcp的平移替换。
 
 ## 什么是KCP？
 KCP是一个致力于低延时的基于UDP自动重传的可靠传输协议。本身不包含任何网络传输的功能，使用回调的方式处理udp数据包的传输。详情见[kcp](https://github.com/skywind3000/kcp)
 
+## 如何安装
+`aiokcp`是基于cython绑定调用的kcp库，打包可能需要安装平台的编译工具。windows系统需要安装`vsbuilder`，linux系统需要安装`gcc`。安装完成后，可以通过`pip`安装
+```bash
+pip install aiokcp
+```
+如果需要数据包加密，可以选择安装`cryptography`
+```bash
+pip install aiokcp[crypto]
+```
+
 ## 例子
 例子详见`aiokcp/examples`目录
 ### asyncio 低级接口
 这里实现了类似`loop.create_connection`和`loop.create_server`的功能
 ```py
 import asyncio
 import time
@@ -314,15 +324,15 @@
         port = randint(10000, 20000)
         server_thread(port)
         client_thread(port)
 
     thread_test()
 ```
 ### 可选的udp数据包加密
-内置的加密方法需要安装`cryptography`, 默认采用的aes+cbc模式加密。也可以自定义加密对象, 只需要实现`encrypt`和`decrypt`方法即可
+默认数据包不加密，但提供加密的方法和参数。内置的加密方法需要安装`cryptography`, 采用的aes+cbc模式加密+hmac校验。也可以自定义加密对象, 只需要实现`encrypt`和`decrypt`方法即可
 ```py
 from aiokcp import (create_connection, create_server, open_connection,
                     start_server)
 from aiokcp.crypto import get_crypto
 from aiokcp.sync import KCPSocket
 
 # need cryptography installed
```

### Comparing `aiokcp-0.0.3/aiokcp/core.py` & `aiokcp-0.0.4/aiokcp/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,20 +265,22 @@
         self.crypto = crypto
 
     def connection_made(self, transport):
         self._transport = transport
 
     def datagram_received(self, data, addr):
         if len(data) < 24:
+            # invalid data, drop it
             return
         if self.crypto is not None:
             try:
                 data = self.crypto.decrypt(data)
             except:
-                pass
+                # invalid data, drop it
+                return
         if addr in self._transport_map:
             transport = self._transport_map[addr]
         else:
             conv_id = conv_bytes_to_id(data[:4])
             kcp = KCP(**self._kcp_kwargs, conv_id=conv_id)
             transport = KCPStreamTransport(kcp,
                                            addr,
```

### Comparing `aiokcp-0.0.3/aiokcp/ikcp.c` & `aiokcp-0.0.4/aiokcp/ikcp.c`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.3/aiokcp/ikcp.h` & `aiokcp-0.0.4/aiokcp/ikcp.h`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.3/aiokcp/kcp.c` & `aiokcp-0.0.4/aiokcp/kcp.c`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.3/aiokcp/kcp.pyi` & `aiokcp-0.0.4/aiokcp/kcp.pyi`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.3/aiokcp/stream.py` & `aiokcp-0.0.4/aiokcp/stream.py`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.3/aiokcp/sync/server.py` & `aiokcp-0.0.4/aiokcp/sync/server.py`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.3/aiokcp/sync/sock.py` & `aiokcp-0.0.4/aiokcp/sync/sock.py`

 * *Files identical despite different names*

### Comparing `aiokcp-0.0.3/aiokcp.egg-info/PKG-INFO` & `aiokcp-0.0.4/aiokcp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokcp
-Version: 0.0.3
+Version: 0.0.4
 Summary: KCP for asyncio and socketserver, based on kcp
 Author: ryanrain2016
 Author-email: ryanrain2016 <holidaylover2010@gmail.com>
 Project-URL: Homepage, https://github.com/ryanrain2016/aiokcp
 Project-URL: Issues, https://github.com/ryanrain2016/aiokcp/issues
 Keywords: asyncio,kcp,socket,aio,aiokcp
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,24 @@
 
 # aiokcp
 [kcp](https://github.com/skywind3000/kcp)的python实践, 提供了类似python中TCP相关的标准库相同的编程接口(asyncio, socket, socketserver)，原tcp代码使用修改导入的方式可以轻松实现从tcp到kcp的平移替换。
 
 ## 什么是KCP？
 KCP是一个致力于低延时的基于UDP自动重传的可靠传输协议。本身不包含任何网络传输的功能，使用回调的方式处理udp数据包的传输。详情见[kcp](https://github.com/skywind3000/kcp)
 
+## 如何安装
+`aiokcp`是基于cython绑定调用的kcp库，打包可能需要安装平台的编译工具。windows系统需要安装`vsbuilder`，linux系统需要安装`gcc`。安装完成后，可以通过`pip`安装
+```bash
+pip install aiokcp
+```
+如果需要数据包加密，可以选择安装`cryptography`
+```bash
+pip install aiokcp[crypto]
+```
+
 ## 例子
 例子详见`aiokcp/examples`目录
 ### asyncio 低级接口
 这里实现了类似`loop.create_connection`和`loop.create_server`的功能
 ```py
 import asyncio
 import time
@@ -334,15 +344,15 @@
         port = randint(10000, 20000)
         server_thread(port)
         client_thread(port)
 
     thread_test()
 ```
 ### 可选的udp数据包加密
-内置的加密方法需要安装`cryptography`, 默认采用的aes+cbc模式加密。也可以自定义加密对象, 只需要实现`encrypt`和`decrypt`方法即可
+默认数据包不加密，但提供加密的方法和参数。内置的加密方法需要安装`cryptography`, 采用的aes+cbc模式加密+hmac校验。也可以自定义加密对象, 只需要实现`encrypt`和`decrypt`方法即可
 ```py
 from aiokcp import (create_connection, create_server, open_connection,
                     start_server)
 from aiokcp.crypto import get_crypto
 from aiokcp.sync import KCPSocket
 
 # need cryptography installed
```

### Comparing `aiokcp-0.0.3/pyproject.toml` & `aiokcp-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiokcp"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="ryanrain2016", email="holidaylover2010@gmail.com" },
 ]
 description = "KCP for asyncio and socketserver, based on kcp"
 readme = "README.md"
 
 requires-python = ">=3.8"
```

### Comparing `aiokcp-0.0.3/setup.py` & `aiokcp-0.0.4/setup.py`

 * *Files identical despite different names*

