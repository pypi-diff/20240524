# Comparing `tmp/ph_utils-0.0.8.tar.gz` & `tmp/ph_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ph_utils-0.0.8.tar", last modified: Fri May 17 09:35:39 2024, max compression
+gzip compressed data, was "ph_utils-0.0.9.tar", last modified: Thu May 23 09:47:46 2024, max compression
```

## Comparing `ph_utils-0.0.8.tar` & `ph_utils-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     9592 2024-05-17 08:54:46.495620 ph_utils-0.0.8/LICENSE
--rw-r--r--   0        0        0     4764 2024-05-17 08:54:46.495620 ph_utils-0.0.8/README.md
--rw-r--r--   0        0        0      804 2024-05-17 09:35:39.755991 ph_utils-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      505 2024-05-17 08:54:46.496617 ph_utils-0.0.8/src/ph_utils/__init__.py
--rw-r--r--   0        0        0     5351 2024-05-17 08:59:28.753822 ph_utils-0.0.8/src/ph_utils/common.py
--rw-r--r--   0        0        0     3403 2024-05-17 08:54:46.496617 ph_utils-0.0.8/src/ph_utils/config.py
--rw-r--r--   0        0        0     2348 2024-05-17 08:54:46.496617 ph_utils-0.0.8/src/ph_utils/crypto.py
--rw-r--r--   0        0        0     8067 2024-05-17 08:54:46.497614 ph_utils-0.0.8/src/ph_utils/date.py
--rw-r--r--   0        0        0     8851 2024-05-17 08:54:46.497614 ph_utils-0.0.8/src/ph_utils/logger.py
--rw-r--r--   0        0        0      293 2024-05-17 08:54:46.498612 ph_utils-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      713 2024-05-17 08:54:46.498612 ph_utils-0.0.8/tests/common_utils.py
--rw-r--r--   0        0        0      193 2024-05-17 08:54:46.498612 ph_utils-0.0.8/tests/config_utils.py
--rw-r--r--   0        0        0      201 2024-05-17 08:54:46.498612 ph_utils-0.0.8/tests/crypto_utils.py
--rw-r--r--   0        0        0      501 2024-05-17 08:54:46.498612 ph_utils-0.0.8/tests/date_utils.py
--rw-r--r--   0        0        0      280 2024-05-17 08:54:46.499609 ph_utils-0.0.8/tests/logger_utils.py
--rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 ph_utils-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     9592 2024-05-17 08:54:46.495620 ph_utils-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4764 2024-05-17 08:54:46.495620 ph_utils-0.0.9/README.md
+-rw-r--r--   0        0        0      804 2024-05-23 09:47:46.181799 ph_utils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      505 2024-05-17 08:54:46.496617 ph_utils-0.0.9/src/ph_utils/__init__.py
+-rw-r--r--   0        0        0     5351 2024-05-17 08:59:28.753822 ph_utils-0.0.9/src/ph_utils/common.py
+-rw-r--r--   0        0        0     3403 2024-05-17 08:54:46.496617 ph_utils-0.0.9/src/ph_utils/config.py
+-rw-r--r--   0        0        0     2348 2024-05-17 08:54:46.496617 ph_utils-0.0.9/src/ph_utils/crypto.py
+-rw-r--r--   0        0        0     8067 2024-05-17 08:54:46.497614 ph_utils-0.0.9/src/ph_utils/date.py
+-rw-r--r--   0        0        0    11561 2024-05-23 09:46:02.121309 ph_utils-0.0.9/src/ph_utils/logger.py
+-rw-r--r--   0        0        0      293 2024-05-17 08:54:46.498612 ph_utils-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      713 2024-05-17 08:54:46.498612 ph_utils-0.0.9/tests/common_utils.py
+-rw-r--r--   0        0        0      193 2024-05-17 08:54:46.498612 ph_utils-0.0.9/tests/config_utils.py
+-rw-r--r--   0        0        0      201 2024-05-17 08:54:46.498612 ph_utils-0.0.9/tests/crypto_utils.py
+-rw-r--r--   0        0        0      501 2024-05-17 08:54:46.498612 ph_utils-0.0.9/tests/date_utils.py
+-rw-r--r--   0        0        0      280 2024-05-17 08:54:46.499609 ph_utils-0.0.9/tests/logger_utils.py
+-rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 ph_utils-0.0.9/PKG-INFO
```

### Comparing `ph_utils-0.0.8/LICENSE` & `ph_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ph_utils-0.0.8/README.md` & `ph_utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ph_utils-0.0.8/pyproject.toml` & `ph_utils-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ph-utils"
-version = "0.0.8"
+version = "0.0.9"
 description = "The python3 tool classes"
 authors = [
     { name = "Tenny", email = "tenny.shu@foxmail.com" },
 ]
 dependencies = []
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `ph_utils-0.0.8/src/ph_utils/common.py` & `ph_utils-0.0.9/src/ph_utils/common.py`

 * *Files identical despite different names*

### Comparing `ph_utils-0.0.8/src/ph_utils/config.py` & `ph_utils-0.0.9/src/ph_utils/config.py`

 * *Files identical despite different names*

### Comparing `ph_utils-0.0.8/src/ph_utils/crypto.py` & `ph_utils-0.0.9/src/ph_utils/crypto.py`

 * *Files identical despite different names*

### Comparing `ph_utils-0.0.8/src/ph_utils/date.py` & `ph_utils-0.0.9/src/ph_utils/date.py`

 * *Files identical despite different names*

### Comparing `ph_utils-0.0.8/src/ph_utils/logger.py` & `ph_utils-0.0.9/src/ph_utils/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Copyright (c) [2023] [Tenny]
 # [ph-utils] is licensed under Mulan PSL v2.
 # You can use this software according to the terms and conditions of the Mulan PSL v2.
 # You may obtain a copy of Mulan PSL v2 at:
 #         http://license.coscl.org.cn/MulanPSL2
 # THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
 # See the Mulan PSL v2 for more details.
-from logging import config, Formatter, LogRecord
-import logging
 import json
+import logging
 import os
-from pathlib import Path
 import sys
+from logging import Formatter, LogRecord, config
+from pathlib import Path
+
+from ph_utils.common import is_blank
 
 
 class JsonFormatter(Formatter):
     """将日志记录为 json 格式
 
     Args:
         Formatter (logging.Formatter): 日志格式化
@@ -31,69 +33,113 @@
             }
         )
 
     def formatMessage(self, record: LogRecord) -> str:
         return record.getMessage()
 
 
+class NameFilter(logging.Filter):
+    """日志过滤器
+
+    Args:
+        Filter (logging.Filter): 日志过滤器
+    """
+
+    def __init__(self, name=""):
+        self.ignore_null = False
+        self.ignore_names = []
+        if is_blank(name) is False:
+            if name.startswith("required:"):
+                self.ignore_null = True
+                name = name.replace("required:", "")
+        if is_blank(name) is False:
+            self.ignore_names = name.split(",")
+
+    def filter(self, record: LogRecord) -> bool:
+        name = record.name
+        if self.ignore_null and is_blank(name):
+            return False
+        return name not in self.ignore_names
+
+
 def logger_config(
-    filename=None, dir_path=None, level="DEBUG", formatter="basic", loggers=None
+    filename=None,
+    dir_path=None,
+    level="DEBUG",
+    formatter="basic",
+    handlers=None,
+    loggers=None,
+    name_filter="",
+    custom_filters=None,
 ):
     """日志配置
 
     Args:
         filename (str): 日志文件名称, 如果为 None 则不记录日志到文件, 该名称不能带上后缀名
         dir (str): 日志文件记录路径, 默认为: cwd() + 'logs'
         level (str): 日志记录的等级, 默认为: DEBUG, DEBUG、INFO
         formatter (str): 日志格式化形式, basic、json
+        handlers (dict): handlers
         loggers (dict): 日志记录器, 原生的 loggers
+        name_filter (str, optional): 根据 [name] 过滤日志, required: - 过滤 [name] 为空的日志 egg: 'required:a,b'、'a,b'
+        custom_filters (str, list): 自定义过滤器
     """
-    lsformatter = "logging.Formatter"
-    if formatter == "json":
-        lsformatter = "libs.logging.JsonFormatter"
+    config_filters = {}
+    use_filters = set()
+    if is_blank(name_filter) is False:
+        config_filters["name_filter"] = {"()": NameFilter, "name": name_filter}
+        use_filters.add("name_filter")
+    if custom_filters:
+        for item in custom_filters:
+            filter_name = item
+            if isinstance(filter_name, dict):
+                filter_name = list(item.keys())[0]
+                filter_value = item[filter_name]
+                if isinstance(filter_value, dict):
+                    config_filters[filter_name] = filter_value
+                else:
+                    config_filters[filter_name] = {"()": filter_value}
+                use_filters.add(filter_name)
+            else:
+                filter_name = filter_name.__name__
+                config_filters[filter_name] = {"()": item}
+                use_filters.add(filter_name)
     log_config = {
         "version": 1,
         "disable_existing_loggers": False,
-        "loggers": {
-            "app.error": {
-                "level": "ERROR",
-                "handlers": ["error_console"],
-                "propagate": False,
-                "qualname": "app.error",
-            },
-        },
+        "loggers": {},
+        "filters": config_filters,
         "handlers": {
             "console": {
                 "class": "logging.StreamHandler",
                 "formatter": "generic",
                 "stream": sys.stdout,
+                "filters": use_filters,
             },
             "error_console": {
                 "class": "logging.StreamHandler",
                 "formatter": "generic",
                 "stream": sys.stderr,
-            },
-            "access_console": {
-                "class": "logging.StreamHandler",
-                "formatter": "access",
-                "stream": sys.stdout,
+                "filters": use_filters,
             },
         },
         "formatters": {
             "generic": {
                 "format": "[%(asctime)s] (%(name)s) [%(levelname)s] [%(lineno)d]: %(message)s",
-                "class": lsformatter,
+                "class": JsonFormatter if formatter == "json" else logging.Formatter,
             },
             "access": {
                 "format": "[%(asctime)s] (%(name)s) [%(levelname)s] [%(host)s]: %(request)s %(message)s %(status)s %(byte)s",
                 "class": "logging.Formatter",
             },
         },
         "root": {"handlers": ["console"], "level": level},
     }
+    if handlers:
+        log_config["handlers"].update(handlers)
     if loggers:
         log_config["loggers"].update(loggers)
     if filename is not None:  # 记录日志到文件
         # 解析目录
         if not dir_path:
             dir_path = Path(os.getcwd(), "logs")
         else:
@@ -109,14 +155,15 @@
         file_handler = {
             "class": "logging.handlers.RotatingFileHandler",
             "formatter": "generic",
             "filename": f"{dir_path}.log",
             "backupCount": 2,
             "maxBytes": 10485760,  # 10M
             "encoding": "utf-8",
+            "filters": use_filters,
         }
         err_file_handler = {}
         err_file_handler.update(file_handler)
         err_file_handler["filename"] = f"{dir_path}_error.log"
         err_file_handler["level"] = "ERROR"
         err_file_handler["backupCount"] = 7
         # 配置记录到文件
@@ -128,26 +175,59 @@
         log_config["loggers"]["app.error"]["handlers"].append("file_err_handler")
         log_config["root"]["handlers"].append("file_handler")
         log_config["root"]["handlers"].append("file_err_handler")
     return log_config
 
 
 def init_logger(
-    filename=None, dir_path=None, level="DEBUG", formatter="basic", loggers=None
+    filename=None,
+    dir_path=None,
+    level="DEBUG",
+    formatter="basic",
+    handlers=None,
+    loggers=None,
+    name_filter="",
+    custom_filters=None,
 ):
     """初始化日志记录
 
     Args:
         filename (str, optional): 日志文件名称. Defaults to None.
         dir_path (str, optional): 日志记录文件夹. Defaults to cwd() + logs.
         level (str, optional): 记录的日志等级. Defaults to "DEBUG".
         formatter (str, optional): 日志格式, basic、json; json - JSON格式的日志. Defaults to "basic".
         loggers (dict, optional): 日志记录器. Defaults to None.
+        name_filter (str, optional): 根据 [name] 过滤日志, required: - 过滤 [name] 为空的日志 egg: 'required:a,b'、'a,b'
+        custom_filters (str, list): 自定义过滤器
+
+    egg:
+    1. 过滤日志名称为空，或者日志名称等于 root或SQL 的日志
+
+        init_logger(name_filter="required:root,SQL"
+
+    2. 使用自定义过滤器
+        class NameFilter(logging.Filter):
+            ...
+
+        init_logger(custom_filters=[NameFilter])
+        init_logger(custom_filters=[{ 'name_filter1': NameFilter }])
+        init_logger(custom_filters=[{ 'name_filter1': { '()': NameFilter } }])
     """
-    config.dictConfig(logger_config(filename, dir_path, level, formatter, loggers))
+    config.dictConfig(
+        logger_config(
+            filename,
+            dir_path,
+            level,
+            formatter,
+            handlers,
+            loggers,
+            name_filter,
+            custom_filters,
+        )
+    )
 
 
 def sanic_logger_config(filename=None, dir_path=None, level="DEBUG", formatter="basic"):
     """Sanic框架的日志配置
 
     Args:
         filename (str, optional): 日志文件名称. Defaults to None.
@@ -160,14 +240,21 @@
     """
     return logger_config(
         filename,
         dir_path,
         level,
         formatter,
         {
+            "access_console": {
+                "class": "logging.StreamHandler",
+                "formatter": "access",
+                "stream": sys.stdout,
+            },
+        },
+        {
             "sanic.access": {
                 "level": "INFO",
                 "handlers": ["access_console"],
                 "propagate": False,
                 "qualname": "sanic.access",
             },
             "sanic.error": {
```

### Comparing `ph_utils-0.0.8/tests/common_utils.py` & `ph_utils-0.0.9/tests/common_utils.py`

 * *Files identical despite different names*

### Comparing `ph_utils-0.0.8/PKG-INFO` & `ph_utils-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ph-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: The python3 tool classes
 Author-Email: Tenny <tenny.shu@foxmail.com>
 License: MulanPSL-2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://gitee.com/towardly/ph-utils_py
```

