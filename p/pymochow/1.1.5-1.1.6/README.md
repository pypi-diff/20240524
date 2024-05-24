# Comparing `tmp/pymochow-1.1.5.tar.gz` & `tmp/pymochow-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymochow-1.1.5.tar", last modified: Wed May  8 08:16:28 2024, max compression
+gzip compressed data, was "pymochow-1.1.6.tar", last modified: Fri May 24 01:49:09 2024, max compression
```

## Comparing `pymochow-1.1.5.tar` & `pymochow-1.1.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:16:28.451719 pymochow-1.1.5/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-08 07:53:52.000000 pymochow-1.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      310 2024-05-08 08:16:28.451719 pymochow-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1433 2024-05-08 07:53:52.000000 pymochow-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:16:28.449719 pymochow-1.1.5/pymochow/
--rwxr-xr-x   0 root         (0) root         (0)      854 2024-05-08 08:13:45.000000 pymochow-1.1.5/pymochow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:16:28.449719 pymochow-1.1.5/pymochow/auth/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2074 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/auth/bce_credentials.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/auth/bce_v1_signer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:16:28.450719 pymochow-1.1.5/pymochow/client/
--rw-r--r--   0 root         (0) root         (0)       93 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3323 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/client/mochow_client.py
--rw-r--r--   0 root         (0) root         (0)     3472 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/compat.py
--rw-r--r--   0 root         (0) root         (0)     3946 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/configuration.py
--rw-r--r--   0 root         (0) root         (0)     2533 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:16:28.450719 pymochow-1.1.5/pymochow/http/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3143 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/http/handler.py
--rw-r--r--   0 root         (0) root         (0)    10887 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/http/http_client.py
--rw-r--r--   0 root         (0) root         (0)      723 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/http/http_content_types.py
--rw-r--r--   0 root         (0) root         (0)     2686 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/http/http_headers.py
--rw-r--r--   0 root         (0) root         (0)      783 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/http/http_methods.py
--rw-r--r--   0 root         (0) root         (0)     2496 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:16:28.450719 pymochow-1.1.5/pymochow/model/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11796 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/model/database.py
--rw-r--r--   0 root         (0) root         (0)     3327 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/model/enum.py
--rw-r--r--   0 root         (0) root         (0)     5998 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/model/schema.py
--rw-r--r--   0 root         (0) root         (0)    17402 2024-05-08 08:12:07.000000 pymochow-1.1.5/pymochow/model/table.py
--rw-r--r--   0 root         (0) root         (0)     1152 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:16:28.451719 pymochow-1.1.5/pymochow/retry/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/retry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4917 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/retry/retry_policy.py
--rw-r--r--   0 root         (0) root         (0)    22235 2024-05-08 07:53:52.000000 pymochow-1.1.5/pymochow/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 08:16:28.451719 pymochow-1.1.5/pymochow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      310 2024-05-08 08:16:28.000000 pymochow-1.1.5/pymochow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      854 2024-05-08 08:16:28.000000 pymochow-1.1.5/pymochow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 08:16:28.000000 pymochow-1.1.5/pymochow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-08 08:16:28.000000 pymochow-1.1.5/pymochow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-08 08:16:28.000000 pymochow-1.1.5/pymochow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 08:16:28.451719 pymochow-1.1.5/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1083 2024-05-08 07:53:52.000000 pymochow-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 01:49:09.991982 pymochow-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-02-20 08:09:26.000000 pymochow-1.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      310 2024-05-24 01:49:09.990982 pymochow-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1433 2024-02-20 08:09:26.000000 pymochow-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 01:49:09.988982 pymochow-1.1.6/pymochow/
+-rwxr-xr-x   0 root         (0) root         (0)      854 2024-05-24 01:48:37.000000 pymochow-1.1.6/pymochow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 01:49:09.989982 pymochow-1.1.6/pymochow/auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2024-03-26 02:23:15.000000 pymochow-1.1.6/pymochow/auth/bce_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-03-26 02:23:15.000000 pymochow-1.1.6/pymochow/auth/bce_v1_signer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 01:49:09.989982 pymochow-1.1.6/pymochow/client/
+-rw-r--r--   0 root         (0) root         (0)       93 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/client/mochow_client.py
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/compat.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2024-03-26 02:23:15.000000 pymochow-1.1.6/pymochow/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 01:49:09.990982 pymochow-1.1.6/pymochow/http/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3143 2024-02-22 10:33:25.000000 pymochow-1.1.6/pymochow/http/handler.py
+-rw-r--r--   0 root         (0) root         (0)    10887 2024-03-26 02:23:15.000000 pymochow-1.1.6/pymochow/http/http_client.py
+-rw-r--r--   0 root         (0) root         (0)      723 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/http/http_content_types.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2024-03-26 02:23:15.000000 pymochow-1.1.6/pymochow/http/http_headers.py
+-rw-r--r--   0 root         (0) root         (0)      783 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/http/http_methods.py
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 01:49:09.990982 pymochow-1.1.6/pymochow/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11796 2024-05-24 01:45:17.000000 pymochow-1.1.6/pymochow/model/database.py
+-rw-r--r--   0 root         (0) root         (0)     3327 2024-05-24 01:45:17.000000 pymochow-1.1.6/pymochow/model/enum.py
+-rw-r--r--   0 root         (0) root         (0)     5999 2024-05-24 01:46:35.000000 pymochow-1.1.6/pymochow/model/schema.py
+-rw-r--r--   0 root         (0) root         (0)    17402 2024-05-24 01:45:17.000000 pymochow-1.1.6/pymochow/model/table.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 01:49:09.990982 pymochow-1.1.6/pymochow/retry/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/retry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/retry/retry_policy.py
+-rw-r--r--   0 root         (0) root         (0)    22235 2024-02-20 08:09:26.000000 pymochow-1.1.6/pymochow/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 01:49:09.990982 pymochow-1.1.6/pymochow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      310 2024-05-24 01:49:09.000000 pymochow-1.1.6/pymochow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      854 2024-05-24 01:49:09.000000 pymochow-1.1.6/pymochow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 01:49:09.000000 pymochow-1.1.6/pymochow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-24 01:49:09.000000 pymochow-1.1.6/pymochow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-24 01:49:09.000000 pymochow-1.1.6/pymochow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 01:49:09.991982 pymochow-1.1.6/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1083 2024-02-20 08:09:26.000000 pymochow-1.1.6/setup.py
```

### Comparing `pymochow-1.1.5/LICENSE` & `pymochow-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/README.md` & `pymochow-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/__init__.py` & `pymochow-1.1.6/pymochow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 This module defines some common string constants.
 """
 from builtins import str
 from builtins import bytes
 from . import protocol
 from .client.mochow_client import MochowClient
 
-SDK_VERSION = b'1.1.5'
+SDK_VERSION = b'1.1.6'
 URL_PREFIX = b'/v1'
 DEFAULT_ENCODING = 'UTF-8'
 
 __all__ = [
     "MochowClient",
 ]
```

### Comparing `pymochow-1.1.5/pymochow/auth/bce_credentials.py` & `pymochow-1.1.6/pymochow/auth/bce_credentials.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/auth/bce_v1_signer.py` & `pymochow-1.1.6/pymochow/auth/bce_v1_signer.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/client/mochow_client.py` & `pymochow-1.1.6/pymochow/client/mochow_client.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/compat.py` & `pymochow-1.1.6/pymochow/compat.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/configuration.py` & `pymochow-1.1.6/pymochow/configuration.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/exception.py` & `pymochow-1.1.6/pymochow/exception.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/http/handler.py` & `pymochow-1.1.6/pymochow/http/handler.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/http/http_client.py` & `pymochow-1.1.6/pymochow/http/http_client.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/http/http_content_types.py` & `pymochow-1.1.6/pymochow/http/http_content_types.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/http/http_headers.py` & `pymochow-1.1.6/pymochow/http/http_headers.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/http/http_methods.py` & `pymochow-1.1.6/pymochow/http/http_methods.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/http/http_response.py` & `pymochow-1.1.6/pymochow/http/http_response.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/model/database.py` & `pymochow-1.1.6/pymochow/model/database.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/model/enum.py` & `pymochow-1.1.6/pymochow/model/enum.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/model/schema.py` & `pymochow-1.1.6/pymochow/model/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     def __init__(
             self,
             index_name,
             index_type,
             field,
             metric_type,
             params=None,
-            auto_build=True,
+            auto_build=False,
             **kwargs):
         super().__init__(index_name=index_name, index_type=index_type, field=field)
         self._metric_type = metric_type
         self._params = params
         self._auto_build = auto_build
         self._state = kwargs.get('state', None)
```

### Comparing `pymochow-1.1.5/pymochow/model/table.py` & `pymochow-1.1.6/pymochow/model/table.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/protocol.py` & `pymochow-1.1.6/pymochow/protocol.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/retry/retry_policy.py` & `pymochow-1.1.6/pymochow/retry/retry_policy.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow/utils.py` & `pymochow-1.1.6/pymochow/utils.py`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/pymochow.egg-info/SOURCES.txt` & `pymochow-1.1.6/pymochow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymochow-1.1.5/setup.py` & `pymochow-1.1.6/setup.py`

 * *Files identical despite different names*

