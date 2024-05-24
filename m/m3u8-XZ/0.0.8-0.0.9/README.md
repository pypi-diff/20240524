# Comparing `tmp/m3u8_XZ-0.0.8.tar.gz` & `tmp/m3u8_XZ-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "H:\PythonProject\XZlib\packaging_m3u8\dist\.tmp-aadr1bee\m3u8_XZ-0.0.8.tar", last modified: Fri Aug 11 06:45:59 2023, max compression
+gzip compressed data, was "H:\PythonProject\XZlib\packaging_m3u8\dist\.tmp-au21pcte\m3u8_XZ-0.0.9.tar", last modified: Mon Aug 14 04:58:58 2023, max compression
```

## Comparing `m3u8_XZ-0.0.8.tar` & `m3u8_XZ-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-11 06:45:59.183117 m3u8_XZ-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-03-23 03:00:43.000000 m3u8_XZ-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      835 2023-08-11 06:45:59.183117 m3u8_XZ-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-06-06 11:17:28.000000 m3u8_XZ-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-11 06:45:59.171150 m3u8_XZ-0.0.8/m3u8_XZ/
--rw-rw-rw-   0        0        0      170 2023-06-23 07:09:11.000000 m3u8_XZ-0.0.8/m3u8_XZ/__init__.py
--rw-rw-rw-   0        0        0      678 2023-05-05 05:15:21.000000 m3u8_XZ-0.0.8/m3u8_XZ/cryptoModel.py
--rw-rw-rw-   0        0        0     7904 2023-08-11 06:44:31.000000 m3u8_XZ-0.0.8/m3u8_XZ/xz.py
-drwxrwxrwx   0        0        0        0 2023-08-11 06:45:59.181122 m3u8_XZ-0.0.8/m3u8_XZ.egg-info/
--rw-rw-rw-   0        0        0      835 2023-08-11 06:45:59.000000 m3u8_XZ-0.0.8/m3u8_XZ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-08-11 06:45:59.000000 m3u8_XZ-0.0.8/m3u8_XZ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-11 06:45:59.000000 m3u8_XZ-0.0.8/m3u8_XZ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-08-11 06:45:59.000000 m3u8_XZ-0.0.8/m3u8_XZ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-11 06:45:59.000000 m3u8_XZ-0.0.8/m3u8_XZ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      522 2023-03-23 11:30:25.000000 m3u8_XZ-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-11 06:45:59.183117 m3u8_XZ-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      768 2023-08-11 06:45:43.000000 m3u8_XZ-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-14 04:58:58.770181 m3u8_XZ-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-03-23 03:00:43.000000 m3u8_XZ-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1210 2023-08-14 04:58:58.769179 m3u8_XZ-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      833 2023-08-12 06:59:38.000000 m3u8_XZ-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-14 04:58:58.756218 m3u8_XZ-0.0.9/m3u8_XZ/
+-rw-rw-rw-   0        0        0      170 2023-06-23 07:09:11.000000 m3u8_XZ-0.0.9/m3u8_XZ/__init__.py
+-rw-rw-rw-   0        0        0      678 2023-05-05 05:15:21.000000 m3u8_XZ-0.0.9/m3u8_XZ/cryptoModel.py
+-rw-rw-rw-   0        0        0     8301 2023-08-12 06:56:15.000000 m3u8_XZ-0.0.9/m3u8_XZ/xz.py
+drwxrwxrwx   0        0        0        0 2023-08-14 04:58:58.767188 m3u8_XZ-0.0.9/m3u8_XZ.egg-info/
+-rw-rw-rw-   0        0        0     1210 2023-08-14 04:58:58.000000 m3u8_XZ-0.0.9/m3u8_XZ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-08-14 04:58:58.000000 m3u8_XZ-0.0.9/m3u8_XZ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-14 04:58:58.000000 m3u8_XZ-0.0.9/m3u8_XZ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-08-14 04:58:58.000000 m3u8_XZ-0.0.9/m3u8_XZ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-14 04:58:58.000000 m3u8_XZ-0.0.9/m3u8_XZ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      522 2023-03-23 11:30:25.000000 m3u8_XZ-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-14 04:58:58.770181 m3u8_XZ-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      768 2023-08-14 04:58:37.000000 m3u8_XZ-0.0.9/setup.py
```

### Comparing `m3u8_XZ-0.0.8/LICENSE` & `m3u8_XZ-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `m3u8_XZ-0.0.8/m3u8_XZ/cryptoModel.py` & `m3u8_XZ-0.0.9/m3u8_XZ/cryptoModel.py`

 * *Files identical despite different names*

### Comparing `m3u8_XZ-0.0.8/m3u8_XZ/xz.py` & `m3u8_XZ-0.0.9/m3u8_XZ/xz.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -- coding:utf-8 --
 # Time:2023-03-23 10:48
 # Author:XZ
 # File:xz.py
 # IED:PyCharm
 import time
+from threading import Thread
+
 import aiohttp
 import asyncio
 import requests as req
 import re
 import os
 from .cryptoModel import DecodeByte
 
@@ -21,19 +23,19 @@
     print_callback = None
     logger = None
 
     def __init__(self, url=None, folder='m3u8_XZ_test', path='./down_load/', m3u8_file=None, logger=True, headers=None, print_callback=None):
         # 下载文件名
         self.file_name = folder + '.mp4'
         # 下载存储文件夹
-        self.path = path + folder + '/'
+        self.path = os.path.join(path, folder)
         if not os.path.exists(self.path):
             os.makedirs(self.path)
         # 缓存文件夹
-        self.temp_path = self.path + 'temp/'
+        self.temp_path = os.path.join(self.path, 'temp')
         if not os.path.exists(self.temp_path):
             os.makedirs(self.temp_path)
         # m3u8
         self.url = url
         if headers:
             self.headers = headers
         else:
@@ -153,15 +155,15 @@
             if self.cry['key']:
                 # 如果源文件有iv就读取，如果没有就用文件名
                 iv = self.cry["iv"] if self.cry["iv"] else ts_name.split('.')[0].zfill(16)
                 data = DecodeByte.do_decode(self.cry["key"], iv, data, self.cry["method"])
                 if not data:
                     raise Exception('解密失败')
             # 保存
-            with open(self.temp_path + ts_name, 'wb') as f:
+            with open(os.path.join(self.temp_path, ts_name), 'wb') as f:
                 f.write(data)
                 # 打印进度
                 self.num += 1
                 M3U8.log('\r下载中:{:3.0f}%| {}/{}'.format(self.num / self.list_length * 100, self.num, self.list_length),
                           end='', flush=True)
                 #
                 if M3U8.print_callback:
@@ -179,20 +181,20 @@
         # 文件总数
         length = len(file_list)
         # 开始合并文件
         with open(dest_file, 'ab') as f:
             # 循环文件列表
             for i, file in enumerate(file_list):
                 # 读取每个文件
-                with open(source_path + file, 'rb') as rf:
+                with open(os.path.join(source_path, file), 'rb') as rf:
                     # 把每个文件的内容 追加到同一个文件
                     data = rf.read()
                     f.write(data)
                 # 清除缓存文件
-                os.remove(source_path + file)
+                os.remove(os.path.join(source_path, file))
                 # 打印进度
                 M3U8.log('\r合并中:{:3.0f}%'.format(i / length * 100), end='', flush=True)
                 #
                 if M3U8.print_callback:
                     M3U8.print_callback(combined_num=i, combine_count=length)
         # 移除缓存文件夹
         os.rmdir(source_path)
@@ -212,7 +214,15 @@
                 M3U8.print_callback(over_time=over_time)
 
     @staticmethod
     def log(*args, **kwargs):
         if M3U8.logger:
             print(*args, **kwargs)
 
+    def run_thread(self):
+        if self.url or self.m3u8_file:
+            # 创建事件循环对象
+            loop = asyncio.new_event_loop()
+            # 创建子线程并启动异步任务
+            thread = Thread(target=self.run, args=(loop,), daemon=True)
+            thread.start()
+
```

### Comparing `m3u8_XZ-0.0.8/pyproject.toml` & `m3u8_XZ-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `m3u8_XZ-0.0.8/setup.py` & `m3u8_XZ-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="m3u8_XZ",
-    version="0.0.8",
+    version="0.0.9",
     author="XZ",
     author_email="345841407@qq.com",
     description="download m3u8 video by m3u8 url or by local m3u8 file",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

