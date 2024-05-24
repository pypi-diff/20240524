# Comparing `tmp/cloudoll-2.2.8.tar.gz` & `tmp/cloudoll-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudoll-2.2.8.tar", last modified: Wed Mar 20 15:55:56 2024, max compression
+gzip compressed data, was "cloudoll-2.2.9.tar", last modified: Tue Mar 26 11:52:24 2024, max compression
```

## Comparing `cloudoll-2.2.8.tar` & `cloudoll-2.2.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-20 15:55:56.050404 cloudoll-2.2.8/
--rw-r--r--   0 xiaobei    (501) staff       (20)     1063 2023-11-29 10:35:40.000000 cloudoll-2.2.8/LICENSE
--rw-r--r--   0 xiaobei    (501) staff       (20)     8084 2024-03-20 15:55:56.049990 cloudoll-2.2.8/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)     7450 2024-02-26 06:29:13.000000 cloudoll-2.2.8/README.md
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-20 15:55:56.035829 cloudoll-2.2.8/cloudoll/
--rw-r--r--   0 xiaobei    (501) staff       (20)       22 2024-03-20 15:54:15.000000 cloudoll-2.2.8/cloudoll/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)       59 2023-12-05 02:24:33.000000 cloudoll-2.2.8/cloudoll/__main__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     4491 2024-03-11 07:32:12.000000 cloudoll-2.2.8/cloudoll/cli.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-20 15:55:56.039272 cloudoll-2.2.8/cloudoll/error/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.2.8/cloudoll/error/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.2.8/cloudoll/error/errors.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-20 15:55:56.039598 cloudoll-2.2.8/cloudoll/logging/
--rw-r--r--   0 xiaobei    (501) staff       (20)     5072 2024-03-04 12:36:26.000000 cloudoll-2.2.8/cloudoll/logging/__init__.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-20 15:55:56.040202 cloudoll-2.2.8/cloudoll/mail/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.2.8/cloudoll/mail/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     5691 2023-07-19 08:33:26.000000 cloudoll-2.2.8/cloudoll/mail/smtp.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-20 15:55:56.043073 cloudoll-2.2.8/cloudoll/orm/
--rw-r--r--   0 xiaobei    (501) staff       (20)     7389 2024-03-14 05:21:27.000000 cloudoll-2.2.8/cloudoll/orm/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     1880 2024-03-01 10:33:11.000000 cloudoll-2.2.8/cloudoll/orm/base.py
--rw-r--r--   0 xiaobei    (501) staff       (20)       83 2024-03-12 07:17:27.000000 cloudoll-2.2.8/cloudoll/orm/err.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     9100 2024-03-18 08:44:39.000000 cloudoll-2.2.8/cloudoll/orm/field.py
--rw-r--r--   0 xiaobei    (501) staff       (20)    19552 2024-03-20 02:06:28.000000 cloudoll-2.2.8/cloudoll/orm/model.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     2177 2024-03-01 06:23:06.000000 cloudoll-2.2.8/cloudoll/orm/mysql.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     4152 2024-03-04 08:28:39.000000 cloudoll-2.2.8/cloudoll/orm/parse.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     1747 2024-03-01 03:13:48.000000 cloudoll-2.2.8/cloudoll/orm/postgres.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-20 15:55:56.044564 cloudoll-2.2.8/cloudoll/robot/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.2.8/cloudoll/robot/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-08-17 06:14:54.000000 cloudoll-2.2.8/cloudoll/robot/dingtalk.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.2.8/cloudoll/robot/feishu.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     2687 2023-08-27 10:17:58.000000 cloudoll-2.2.8/cloudoll/robot/slack.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-20 15:55:56.046240 cloudoll-2.2.8/cloudoll/utils/
--rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-11-20 03:38:20.000000 cloudoll-2.2.8/cloudoll/utils/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)      459 2023-11-29 10:35:40.000000 cloudoll-2.2.8/cloudoll/utils/common.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     9394 2024-03-04 08:45:31.000000 cloudoll-2.2.8/cloudoll/utils/m2d.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     7570 2024-03-08 09:13:33.000000 cloudoll-2.2.8/cloudoll/utils/patch_loop.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     5955 2024-03-20 14:45:38.000000 cloudoll-2.2.8/cloudoll/utils/watch.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-20 15:55:56.049430 cloudoll-2.2.8/cloudoll/web/
--rw-r--r--   0 xiaobei    (501) staff       (20)    17361 2024-03-20 06:42:28.000000 cloudoll-2.2.8/cloudoll/web/__init__.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     1584 2024-02-26 02:42:42.000000 cloudoll-2.2.8/cloudoll/web/exception.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.2.8/cloudoll/web/html.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     3555 2023-08-17 06:07:18.000000 cloudoll-2.2.8/cloudoll/web/http.py
--rw-r--r--   0 xiaobei    (501) staff       (20)     1121 2023-07-19 08:38:07.000000 cloudoll-2.2.8/cloudoll/web/jwt.py
--rw-r--r--   0 xiaobei    (501) staff       (20)      461 2024-03-08 07:14:46.000000 cloudoll-2.2.8/cloudoll/web/settings.py
-drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-20 15:55:56.038641 cloudoll-2.2.8/cloudoll.egg-info/
--rw-r--r--   0 xiaobei    (501) staff       (20)     8084 2024-03-20 15:55:55.000000 cloudoll-2.2.8/cloudoll.egg-info/PKG-INFO
--rw-r--r--   0 xiaobei    (501) staff       (20)      954 2024-03-20 15:55:55.000000 cloudoll-2.2.8/cloudoll.egg-info/SOURCES.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        1 2024-03-20 15:55:55.000000 cloudoll-2.2.8/cloudoll.egg-info/dependency_links.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)       46 2024-03-20 15:55:55.000000 cloudoll-2.2.8/cloudoll.egg-info/entry_points.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)      116 2024-03-20 15:55:55.000000 cloudoll-2.2.8/cloudoll.egg-info/requires.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)        9 2024-03-20 15:55:55.000000 cloudoll-2.2.8/cloudoll.egg-info/top_level.txt
--rw-r--r--   0 xiaobei    (501) staff       (20)       38 2024-03-20 15:55:56.050533 cloudoll-2.2.8/setup.cfg
--rw-r--r--   0 xiaobei    (501) staff       (20)     4441 2023-11-23 13:13:49.000000 cloudoll-2.2.8/setup.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-26 11:52:24.112594 cloudoll-2.2.9/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1063 2023-11-29 10:35:40.000000 cloudoll-2.2.9/LICENSE
+-rw-r--r--   0 xiaobei    (501) staff       (20)     8084 2024-03-26 11:52:24.112397 cloudoll-2.2.9/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7450 2024-02-26 06:29:13.000000 cloudoll-2.2.9/README.md
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-26 11:52:24.106518 cloudoll-2.2.9/cloudoll/
+-rw-r--r--   0 xiaobei    (501) staff       (20)       22 2024-03-26 11:51:29.000000 cloudoll-2.2.9/cloudoll/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)       59 2023-12-05 02:24:33.000000 cloudoll-2.2.9/cloudoll/__main__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     4491 2024-03-11 07:32:12.000000 cloudoll-2.2.9/cloudoll/cli.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-26 11:52:24.107683 cloudoll-2.2.9/cloudoll/error/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.2.9/cloudoll/error/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3501 2023-03-15 06:24:14.000000 cloudoll-2.2.9/cloudoll/error/errors.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-26 11:52:24.107835 cloudoll-2.2.9/cloudoll/logging/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     5564 2024-03-26 11:49:52.000000 cloudoll-2.2.9/cloudoll/logging/__init__.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-26 11:52:24.108167 cloudoll-2.2.9/cloudoll/mail/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.2.9/cloudoll/mail/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     5691 2023-07-19 08:33:26.000000 cloudoll-2.2.9/cloudoll/mail/smtp.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-26 11:52:24.109724 cloudoll-2.2.9/cloudoll/orm/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7487 2024-03-25 09:22:44.000000 cloudoll-2.2.9/cloudoll/orm/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1880 2024-03-01 10:33:11.000000 cloudoll-2.2.9/cloudoll/orm/base.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)       83 2024-03-12 07:17:27.000000 cloudoll-2.2.9/cloudoll/orm/err.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     9100 2024-03-18 08:44:39.000000 cloudoll-2.2.9/cloudoll/orm/field.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)    19319 2024-03-26 11:07:03.000000 cloudoll-2.2.9/cloudoll/orm/model.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     2177 2024-03-01 06:23:06.000000 cloudoll-2.2.9/cloudoll/orm/mysql.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     4152 2024-03-04 08:28:39.000000 cloudoll-2.2.9/cloudoll/orm/parse.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1747 2024-03-01 03:13:48.000000 cloudoll-2.2.9/cloudoll/orm/postgres.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-26 11:52:24.110378 cloudoll-2.2.9/cloudoll/robot/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-03-15 06:24:14.000000 cloudoll-2.2.9/cloudoll/robot/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     6380 2023-08-17 06:14:54.000000 cloudoll-2.2.9/cloudoll/robot/dingtalk.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3114 2023-03-22 06:01:06.000000 cloudoll-2.2.9/cloudoll/robot/feishu.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     2687 2023-08-27 10:17:58.000000 cloudoll-2.2.9/cloudoll/robot/slack.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-26 11:52:24.111159 cloudoll-2.2.9/cloudoll/utils/
+-rw-r--r--   0 xiaobei    (501) staff       (20)        0 2023-11-20 03:38:20.000000 cloudoll-2.2.9/cloudoll/utils/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)      459 2023-11-29 10:35:40.000000 cloudoll-2.2.9/cloudoll/utils/common.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     9394 2024-03-04 08:45:31.000000 cloudoll-2.2.9/cloudoll/utils/m2d.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     7570 2024-03-08 09:13:33.000000 cloudoll-2.2.9/cloudoll/utils/patch_loop.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     5955 2024-03-20 14:45:38.000000 cloudoll-2.2.9/cloudoll/utils/watch.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-26 11:52:24.112101 cloudoll-2.2.9/cloudoll/web/
+-rw-r--r--   0 xiaobei    (501) staff       (20)    17361 2024-03-20 06:42:28.000000 cloudoll-2.2.9/cloudoll/web/__init__.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1584 2024-02-26 02:42:42.000000 cloudoll-2.2.9/cloudoll/web/exception.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     2077 2023-03-15 06:24:14.000000 cloudoll-2.2.9/cloudoll/web/html.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     3555 2023-08-17 06:07:18.000000 cloudoll-2.2.9/cloudoll/web/http.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)     1121 2023-07-19 08:38:07.000000 cloudoll-2.2.9/cloudoll/web/jwt.py
+-rw-r--r--   0 xiaobei    (501) staff       (20)      461 2024-03-08 07:14:46.000000 cloudoll-2.2.9/cloudoll/web/settings.py
+drwxr-xr-x   0 xiaobei    (501) staff       (20)        0 2024-03-26 11:52:24.107445 cloudoll-2.2.9/cloudoll.egg-info/
+-rw-r--r--   0 xiaobei    (501) staff       (20)     8084 2024-03-26 11:52:24.000000 cloudoll-2.2.9/cloudoll.egg-info/PKG-INFO
+-rw-r--r--   0 xiaobei    (501) staff       (20)      954 2024-03-26 11:52:24.000000 cloudoll-2.2.9/cloudoll.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        1 2024-03-26 11:52:24.000000 cloudoll-2.2.9/cloudoll.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)       46 2024-03-26 11:52:24.000000 cloudoll-2.2.9/cloudoll.egg-info/entry_points.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)      116 2024-03-26 11:52:24.000000 cloudoll-2.2.9/cloudoll.egg-info/requires.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)        9 2024-03-26 11:52:24.000000 cloudoll-2.2.9/cloudoll.egg-info/top_level.txt
+-rw-r--r--   0 xiaobei    (501) staff       (20)       38 2024-03-26 11:52:24.112639 cloudoll-2.2.9/setup.cfg
+-rw-r--r--   0 xiaobei    (501) staff       (20)     4441 2023-11-23 13:13:49.000000 cloudoll-2.2.9/setup.py
```

### Comparing `cloudoll-2.2.8/LICENSE` & `cloudoll-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/PKG-INFO` & `cloudoll-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.2.8
+Version: 2.2.9
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `cloudoll-2.2.8/README.md` & `cloudoll-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/cli.py` & `cloudoll-2.2.9/cloudoll/cli.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/error/errors.py` & `cloudoll-2.2.9/cloudoll/error/errors.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/logging/__init__.py` & `cloudoll-2.2.9/cloudoll/logging/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "info",
     "warning",
     "error",
     "exception",
     "critical",
     "print_info",
     "print_error",
+    "print_warn",
 )
 _COLORS = {
     # 终端输出日志颜色配置
     "DEBUG": "white",
     "INFO": "green",
     "WARNING": "yellow",
     "ERROR": "red",
@@ -36,17 +37,19 @@
     YELLOW = "\033[93m"
     BLUE = "\033[94m"
     END = "\033[0m"
 
 
 _FORMATS = {
     # 终端输出格式
-    "console_format": "%(log_color)s[%(levelname)s]-%(asctime)s-%(pathname)s-%(module)s-%(funcName)s-[line:%(lineno)d]: %(message)s",
+    # "console_format": "%(log_color)s[%(levelname)s]-%(asctime)s-%(pathname)s-%(module)s-%(funcName)s-[line:%(lineno)d]: %(message)s",
+    "console_format": "%(log_color)s%(asctime)s %(levelname)s %(funcName)s %(message)s",
     # 日志输出格式
-    "log_format": "[%(levelname)s]-%(asctime)s-%(pathname)s-%(module)s-%(funcName)s-[line:%(lineno)d]: %(message)s",
+    # "log_format": "[%(levelname)s]-%(asctime)s-%(pathname)s-%(module)s-%(funcName)s-[line:%(lineno)d]: %(message)s",
+    "log_format": "%(asctime)s %(levelname)s %(funcName)s %(message)s",
 }
 
 _LOG_SIZE = 1024 * 1024 * 1  # 1MB 日志最大1MB
 _LOG_FILES_COUNT = 3  # 最多保留3个日志文件
 
 
 class HandleLog:
@@ -134,20 +137,31 @@
 
         return getattr(logger, method, None)
 
 
 _handler = None
 
 
-def print_info(*msg, **kw):
-    print(f"{ColorAnsi.GREEN}{msg}{kw}{ColorAnsi.END}")
+def print_format(color_ansi, type, *args):
+    ft = color_ansi + "{}" + ColorAnsi.END
+    timestamp = ft.format(datetime.now().strftime("%Y-%m-%d %H:%M:%S") + " " + type)
+    text = " ".join(ft.format(str(arg)) for arg in args)
+    print(timestamp, text)
 
 
-def print_error(*msg, **kw):
-    print(f"{ColorAnsi.RED}{msg}{kw}{ColorAnsi.END}")
+def print_info(*args):
+    print_format(ColorAnsi.GREEN, "INFO", *args)
+
+
+def print_error(*args):
+    print_format(ColorAnsi.RED, "ERROR", *args)
+
+
+def print_warn(*args):
+    print_format(ColorAnsi.YELLOW, "WARN", *args)
 
 
 def _get_handle():
     global _handler
     handler = _handler if _handler else HandleLog()
     _handler = handler
     return handler
```

### Comparing `cloudoll-2.2.8/cloudoll/mail/smtp.py` & `cloudoll-2.2.9/cloudoll/mail/smtp.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/orm/__init__.py` & `cloudoll-2.2.9/cloudoll/orm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from redis import asyncio as aioredis
 from .parse import parse_coon
 import aiopg, aiomysql
 from .base import MeteBase, QueryTypes
 from typing import Any
-from ..logging import error, print_info
+from ..logging import print_info, print_error
 import traceback
 
 
 async def create_engine(**kw):
     url = kw.get("url")
     driver = None
     configs = {}
@@ -31,15 +31,15 @@
         redis://[[username]:[password]]@localhost:6379/0
         rediss://[[username]:[password]]@localhost:6379/0
         """
         if url is None:
             url = f"{driver}://{configs['username']}:{configs['password']}@{configs['host']}:{configs['port']}/{configs['db']}"
         return await aioredis.from_url(url, **query)
     else:
-        error("Not suport this database type.")
+        print_error("Not suport this database type.")
 
 
 class Postgres(MeteBase):
     def __init__(self, pool=None):
         self.pool = pool
         self.driver = "postgres"
 
@@ -100,19 +100,21 @@
             self.pool = await aiopg.create_pool(
                 dsn=dsn,
                 timeout=kw.get("timeout"),
                 echo=kw.get("echo", False),
                 maxsize=kw.get("maxsize", 10),
                 minsize=kw.get("pool_size", 5),
             )
-            print(f"Database connection successfuly for postgres/{kw.get('db')}")
+            print_info(f"Database connection successfuly for postgres/{kw.get('db')}")
         except Exception as e:
-            error(e)
+            # error(e)
             # print(traceback.format_exc())
-            error(f"Database connection failed,the instance : postgres/{kw.get('db')}")
+            print_error(
+                f"Database connection failed,the instance : postgres/{kw.get('db')}"
+            )
 
         return self
 
 
 class AttrDict(dict):
     """Dict that can get attribute by dot, and doesn't raise KeyError"""
 
@@ -187,13 +189,15 @@
                 charset=kw.get("charset", "utf8"),
                 autocommit=False,  # kw.get("autocommit", False),
                 maxsize=kw.get("maxsize", 10),
                 minsize=kw.get("pool_size", 5),
                 cursorclass=AttrDictCursor,
                 loop=loop,
             )
-            print(f"Database connection successfuly for mysql/{kw.get('db')}.")
+            print_info(f"Database connection successfuly for mysql/{kw.get('db')}.")
         except Exception as e:
-            print(e)
+            # print(e)
             # print(traceback.format_exc())
-            error(f"Database connection failed,the instance : mysql/{kw.get('db')}")
+            print_error(
+                f"Database connection failed,the instance : mysql/{kw.get('db')}"
+            )
         return self
```

### Comparing `cloudoll-2.2.8/cloudoll/orm/base.py` & `cloudoll-2.2.9/cloudoll/orm/base.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/orm/field.py` & `cloudoll-2.2.9/cloudoll/orm/field.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/orm/model.py` & `cloudoll-2.2.9/cloudoll/orm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,22 +68,15 @@
 
 class Model(metaclass=ModelMetaclass):
     def __init__(self, **kw):
         for k in self.__fields__:
             f = getattr(self, k, None)
             f.value = None
         for k, v in kw.items():
-            # print(f"{k}----{v}")
-            f = getattr(self, k, None)
-            if isinstance(f, Field):
-                if v is None:
-                    v = f.default
-                f.value = v
-            else:
-                setattr(self, k, v)
+            self[k] = v
 
         # super().__init__(self, **kw)
 
     def __str__(self):
         return "<Model: %s>" % self.__class__.__name__
 
     def __repr__(self):
```

### Comparing `cloudoll-2.2.8/cloudoll/orm/mysql.py` & `cloudoll-2.2.9/cloudoll/orm/mysql.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/orm/parse.py` & `cloudoll-2.2.9/cloudoll/orm/parse.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/orm/postgres.py` & `cloudoll-2.2.9/cloudoll/orm/postgres.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/robot/dingtalk.py` & `cloudoll-2.2.9/cloudoll/robot/dingtalk.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/robot/feishu.py` & `cloudoll-2.2.9/cloudoll/robot/feishu.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/robot/slack.py` & `cloudoll-2.2.9/cloudoll/robot/slack.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/utils/m2d.py` & `cloudoll-2.2.9/cloudoll/utils/m2d.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/utils/patch_loop.py` & `cloudoll-2.2.9/cloudoll/utils/patch_loop.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/utils/watch.py` & `cloudoll-2.2.9/cloudoll/utils/watch.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/web/__init__.py` & `cloudoll-2.2.9/cloudoll/web/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/web/exception.py` & `cloudoll-2.2.9/cloudoll/web/exception.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/web/html.py` & `cloudoll-2.2.9/cloudoll/web/html.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/web/http.py` & `cloudoll-2.2.9/cloudoll/web/http.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll/web/jwt.py` & `cloudoll-2.2.9/cloudoll/web/jwt.py`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/cloudoll.egg-info/PKG-INFO` & `cloudoll-2.2.9/cloudoll.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudoll
-Version: 2.2.8
+Version: 2.2.9
 Summary: 辅助快速创建可分布的微服务。
 Home-page: https://gitee.com/chuchur/cloudoll-py
 Author: chuchur
 Author-email: chuchur@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `cloudoll-2.2.8/cloudoll.egg-info/SOURCES.txt` & `cloudoll-2.2.9/cloudoll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudoll-2.2.8/setup.py` & `cloudoll-2.2.9/setup.py`

 * *Files identical despite different names*

