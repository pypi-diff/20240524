# Comparing `tmp/metasdk-1.7.8.tar.gz` & `tmp/metasdk-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasdk-1.7.8.tar", last modified: Wed Apr  3 11:34:54 2024, max compression
+gzip compressed data, was "metasdk-1.7.9.tar", last modified: Fri Apr 12 07:54:38 2024, max compression
```

## Comparing `metasdk-1.7.8.tar` & `metasdk-1.7.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.063845 metasdk-1.7.8/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1074 2022-08-11 12:23:20.000000 metasdk-1.7.8/LICENSE
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.8/MANIFEST.in
--rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-03 11:34:54.063845 metasdk-1.7.8/PKG-INFO
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2236 2024-02-12 19:35:51.000000 metasdk-1.7.8/README.md
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.055845 metasdk-1.7.8/metasdk/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)    16426 2024-02-12 19:35:51.000000 metasdk-1.7.8/metasdk/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      190 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/__state.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3803 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/apiclient.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     6152 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/event_bus.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3523 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/exceptions.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      102 2024-04-03 11:33:07.000000 metasdk-1.7.8/metasdk/info.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1815 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/internal.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.059845 metasdk-1.7.8/metasdk/logger/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     6374 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/logger/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1862 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/logger/bulk_logger.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     3478 2024-01-25 19:39:16.000000 metasdk-1.7.8/metasdk/logger/logger.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.063845 metasdk-1.7.8/metasdk/services/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     8667 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/ApiProxyService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5098 2024-04-01 14:33:24.000000 metasdk-1.7.8/metasdk/services/AuthService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      634 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/CacheService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5086 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/DbQueryService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2924 2024-01-25 19:39:16.000000 metasdk-1.7.8/metasdk/services/DbService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1355 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/DevService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1066 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/ExportService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2563 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/ExternalSystemService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)    21782 2024-04-03 11:33:07.000000 metasdk-1.7.8/metasdk/services/FeedService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1939 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/IssueService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     5823 2024-01-25 19:39:16.000000 metasdk-1.7.8/metasdk/services/LockService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1394 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/MailService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1936 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/MediaService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1362 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/MetaqlService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      968 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/ObjectLogService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2554 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/SettingsService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     8731 2023-12-07 09:05:36.000000 metasdk-1.7.8/metasdk/services/StarterService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      691 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/UserManagementService.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1157 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/services/__init__.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.063845 metasdk-1.7.8/metasdk/tools/
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/tools/__init__.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1079 2024-01-25 19:39:16.000000 metasdk-1.7.8/metasdk/tools/extract_event_handlers.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2252 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/utils.py
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     2051 2022-08-11 12:23:20.000000 metasdk-1.7.8/metasdk/worker.py
-drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-03 11:34:54.059845 metasdk-1.7.8/metasdk.egg-info/
--rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-03 11:34:54.000000 metasdk-1.7.8/metasdk.egg-info/PKG-INFO
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1172 2024-04-03 11:34:54.000000 metasdk-1.7.8/metasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        1 2024-04-03 11:34:54.000000 metasdk-1.7.8/metasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      172 2024-04-03 11:34:54.000000 metasdk-1.7.8/metasdk.egg-info/requires.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)        8 2024-04-03 11:34:54.000000 metasdk-1.7.8/metasdk.egg-info/top_level.txt
--rw-rw-r--   0 zhas      (1000) zhas      (1000)      205 2024-04-03 11:34:54.063845 metasdk-1.7.8/setup.cfg
--rw-rw-r--   0 zhas      (1000) zhas      (1000)     1193 2022-08-11 12:23:20.000000 metasdk-1.7.8/setup.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.211857 metasdk-1.7.9/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1074 2022-08-11 12:23:20.000000 metasdk-1.7.9/LICENSE
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.9/MANIFEST.in
+-rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-12 07:54:38.211857 metasdk-1.7.9/PKG-INFO
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2236 2024-02-12 19:35:51.000000 metasdk-1.7.9/README.md
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.203857 metasdk-1.7.9/metasdk/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)    16426 2024-04-11 12:36:26.000000 metasdk-1.7.9/metasdk/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      190 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/__state.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3803 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/apiclient.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     6152 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/event_bus.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3523 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/exceptions.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      102 2024-04-12 07:54:23.000000 metasdk-1.7.9/metasdk/info.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1815 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/internal.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.203857 metasdk-1.7.9/metasdk/logger/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     6374 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/logger/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1862 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/logger/bulk_logger.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     3478 2024-01-25 19:39:16.000000 metasdk-1.7.9/metasdk/logger/logger.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.207857 metasdk-1.7.9/metasdk/services/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     8667 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/ApiProxyService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5097 2024-04-12 07:54:23.000000 metasdk-1.7.9/metasdk/services/AuthService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      634 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/CacheService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5086 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/DbQueryService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2924 2024-01-25 19:39:16.000000 metasdk-1.7.9/metasdk/services/DbService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1355 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/DevService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1066 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/ExportService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2563 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/ExternalSystemService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)    21782 2024-04-03 11:33:07.000000 metasdk-1.7.9/metasdk/services/FeedService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1939 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/IssueService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     5823 2024-01-25 19:39:16.000000 metasdk-1.7.9/metasdk/services/LockService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1394 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/MailService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1936 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/MediaService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1362 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/MetaqlService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      968 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/ObjectLogService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2554 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/SettingsService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     9916 2024-04-12 07:54:23.000000 metasdk-1.7.9/metasdk/services/StarterService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      691 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/UserManagementService.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1157 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/services/__init__.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.207857 metasdk-1.7.9/metasdk/tools/
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        0 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/tools/__init__.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1079 2024-01-25 19:39:16.000000 metasdk-1.7.9/metasdk/tools/extract_event_handlers.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2252 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/utils.py
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     2051 2022-08-11 12:23:20.000000 metasdk-1.7.9/metasdk/worker.py
+drwxrwxr-x   0 zhas      (1000) zhas      (1000)        0 2024-04-12 07:54:38.203857 metasdk-1.7.9/metasdk.egg-info/
+-rw-r--r--   0 zhas      (1000) zhas      (1000)     2830 2024-04-12 07:54:38.000000 metasdk-1.7.9/metasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1172 2024-04-12 07:54:38.000000 metasdk-1.7.9/metasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        1 2024-04-12 07:54:38.000000 metasdk-1.7.9/metasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      172 2024-04-12 07:54:38.000000 metasdk-1.7.9/metasdk.egg-info/requires.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)        8 2024-04-12 07:54:38.000000 metasdk-1.7.9/metasdk.egg-info/top_level.txt
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)      205 2024-04-12 07:54:38.211857 metasdk-1.7.9/setup.cfg
+-rw-rw-r--   0 zhas      (1000) zhas      (1000)     1193 2022-08-11 12:23:20.000000 metasdk-1.7.9/setup.py
```

### Comparing `metasdk-1.7.8/LICENSE` & `metasdk-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/PKG-INFO` & `metasdk-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasdk
-Version: 1.7.8
+Version: 1.7.9
 Summary: Devision Meta SDK
 Home-page: https://github.com/devision-io/metasdk
 Author: Artur Geraschenko
 Author-email: arturgspb@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `metasdk-1.7.8/README.md` & `metasdk-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/__init__.py` & `metasdk-1.7.9/metasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/apiclient.py` & `metasdk-1.7.9/metasdk/apiclient.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/event_bus.py` & `metasdk-1.7.9/metasdk/event_bus.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/exceptions.py` & `metasdk-1.7.9/metasdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/internal.py` & `metasdk-1.7.9/metasdk/internal.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/logger/__init__.py` & `metasdk-1.7.9/metasdk/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/logger/bulk_logger.py` & `metasdk-1.7.9/metasdk/logger/bulk_logger.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/logger/logger.py` & `metasdk-1.7.9/metasdk/logger/logger.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/ApiProxyService.py` & `metasdk-1.7.9/metasdk/services/ApiProxyService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/AuthService.py` & `metasdk-1.7.9/metasdk/services/AuthService.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def _authenticate_user(self, token: str) -> Dict:
         """
         Совершает запрос к серверу верификации на проверку Access токена.
 
         :param token: Access Token
         :return: ответ от сервера верификации
         """
-        verify_url = "oauth2/verifyJWTServiceToken"
+        verify_url = "oauth2/verifyJWTAccessToken"
         url = urllib.parse.urljoin(self.__app.auth_service_host, verify_url)
         response = requests.get(url, params={"assertion": token})
         if response.status_code == 200:
             return response.json()
         elif response.status_code == 403:
             raise ForbiddenError("Invalid authorization token")
         else:
```

### Comparing `metasdk-1.7.8/metasdk/services/CacheService.py` & `metasdk-1.7.9/metasdk/services/CacheService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/DbQueryService.py` & `metasdk-1.7.9/metasdk/services/DbQueryService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/DbService.py` & `metasdk-1.7.9/metasdk/services/DbService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/DevService.py` & `metasdk-1.7.9/metasdk/services/DevService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/ExportService.py` & `metasdk-1.7.9/metasdk/services/ExportService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/ExternalSystemService.py` & `metasdk-1.7.9/metasdk/services/ExternalSystemService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/FeedService.py` & `metasdk-1.7.9/metasdk/services/FeedService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/IssueService.py` & `metasdk-1.7.9/metasdk/services/IssueService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/LockService.py` & `metasdk-1.7.9/metasdk/services/LockService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/MailService.py` & `metasdk-1.7.9/metasdk/services/MailService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/MediaService.py` & `metasdk-1.7.9/metasdk/services/MediaService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/MetaqlService.py` & `metasdk-1.7.9/metasdk/services/MetaqlService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/ObjectLogService.py` & `metasdk-1.7.9/metasdk/services/ObjectLogService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/SettingsService.py` & `metasdk-1.7.9/metasdk/services/SettingsService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/StarterService.py` & `metasdk-1.7.9/metasdk/services/StarterService.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 from time import sleep
 
 import requests
 import time
 
+from metasdk.exceptions import BadRequestError, UnexpectedError
+
 
 class StarterService:
     headers = {'Accept': 'application/json', 'Content-Type': 'application/json'}
 
     def __init__(self, app, db, starter_api_url):
         """
         Прямые запросы к БД скорее всего уйдут в апи запускатора, так как скорее всего пбудет много БД для тасков запускатора, так как
@@ -162,7 +164,32 @@
                 except Exception:
                     raise IOError("Starter response read error: " + resp.text)
             except (requests.exceptions.ConnectionError, requests.exceptions.Timeout) as e:
                 # При ошибках подключения пытаемся еще раз
                 last_e = e
                 sleep(3)
         raise last_e
+
+    def stop_task(self, task_id: str, service_id: str) -> str:
+        """
+        Остановить задачу запускатора.
+
+        :param task_id: ID задачи
+        :param service_id: ID службы. Например "meta.datasource_share"
+        :return: None
+        """
+        last_e = None
+        url = f"{self.__starter_api_url}/services/{service_id}/tasks/{task_id}"
+        for _ in range(self.max_retries):
+            try:
+                resp = requests.delete(url=url, headers=self.headers, timeout=15)
+                if resp.status_code == 200:
+                    return task_id
+                elif resp.status_code == 400:
+                    error = resp.json()
+                    raise BadRequestError("Bad Request", {"error": error})
+                else:
+                    raise UnexpectedError("Непредвиденная ошибка при остановке задачи", {"error": resp.text})
+            except (requests.exceptions.ConnectionError, requests.exceptions.Timeout) as e:
+                last_e = e
+                sleep(3)
+        raise last_e
```

### Comparing `metasdk-1.7.8/metasdk/services/UserManagementService.py` & `metasdk-1.7.9/metasdk/services/UserManagementService.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/services/__init__.py` & `metasdk-1.7.9/metasdk/services/__init__.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/tools/extract_event_handlers.py` & `metasdk-1.7.9/metasdk/tools/extract_event_handlers.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/utils.py` & `metasdk-1.7.9/metasdk/utils.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk/worker.py` & `metasdk-1.7.9/metasdk/worker.py`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/metasdk.egg-info/PKG-INFO` & `metasdk-1.7.9/metasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasdk
-Version: 1.7.8
+Version: 1.7.9
 Summary: Devision Meta SDK
 Home-page: https://github.com/devision-io/metasdk
 Author: Artur Geraschenko
 Author-email: arturgspb@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
```

### Comparing `metasdk-1.7.8/metasdk.egg-info/SOURCES.txt` & `metasdk-1.7.9/metasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metasdk-1.7.8/setup.py` & `metasdk-1.7.9/setup.py`

 * *Files identical despite different names*

