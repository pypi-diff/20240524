# Comparing `tmp/life360-7.0.0b6.tar.gz` & `tmp/life360-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "life360-7.0.0b6.tar", last modified: Mon Apr 29 20:11:52 2024, max compression
+gzip compressed data, was "life360-7.0.1.tar", last modified: Fri May 24 13:58:54 2024, max compression
```

## Comparing `life360-7.0.0b6.tar` & `life360-7.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:11:52.252387 life360-7.0.0b6/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 20:11:49.000000 life360-7.0.0b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 20:11:52.252387 life360-7.0.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-29 20:11:49.000000 life360-7.0.0b6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:11:52.252387 life360-7.0.0b6/life360/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-29 20:11:49.000000 life360-7.0.0b6/life360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-29 20:11:49.000000 life360-7.0.0b6/life360/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-29 20:11:49.000000 life360-7.0.0b6/life360/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-29 20:11:49.000000 life360-7.0.0b6/life360/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 20:11:49.000000 life360-7.0.0b6/life360/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:11:52.252387 life360-7.0.0b6/life360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 20:11:52.000000 life360-7.0.0b6/life360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-29 20:11:52.000000 life360-7.0.0b6/life360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:11:52.000000 life360-7.0.0b6/life360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 20:11:52.000000 life360-7.0.0b6/life360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 20:11:52.000000 life360-7.0.0b6/life360.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:11:52.252387 life360-7.0.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-29 20:11:49.000000 life360-7.0.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:54.451793 life360-7.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-24 13:58:48.000000 life360-7.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-24 13:58:54.451793 life360-7.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-24 13:58:48.000000 life360-7.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:54.451793 life360-7.0.1/life360/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-24 13:58:48.000000 life360-7.0.1/life360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13361 2024-05-24 13:58:48.000000 life360-7.0.1/life360/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-24 13:58:48.000000 life360-7.0.1/life360/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-24 13:58:48.000000 life360-7.0.1/life360/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 13:58:48.000000 life360-7.0.1/life360/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:58:54.451793 life360-7.0.1/life360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-24 13:58:54.000000 life360-7.0.1/life360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-24 13:58:54.000000 life360-7.0.1/life360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:58:54.000000 life360-7.0.1/life360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 13:58:54.000000 life360-7.0.1/life360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 13:58:54.000000 life360-7.0.1/life360.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:58:54.451793 life360-7.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-24 13:58:48.000000 life360-7.0.1/setup.py
```

### Comparing `life360-7.0.0b6/LICENSE` & `life360-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b6/PKG-INFO` & `life360-7.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 7.0.0b6
+Version: 7.0.1
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `life360-7.0.0b6/README.md` & `life360-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b6/life360/__init__.py` & `life360-7.0.1/life360/__init__.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b6/life360/api.py` & `life360-7.0.1/life360/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 
 _HEADERS = {
     "accept": "application/json",
     "cache-control": "no-cache",
     "user-agent": USER_AGENT,
 }
 
-_RETRY_EXCEPTIONS = (ClientConnectionError, asyncio.TimeoutError)
+_TIMEOUT_EXCEPTIONS = (asyncio.TimeoutError, TimeoutError)
+_RETRY_EXCEPTIONS = (ClientConnectionError, *_TIMEOUT_EXCEPTIONS)
 _RETRY_CLIENT_RESPONSE_ERRORS = (
     HTTP_Error.BAD_GATEWAY,
     HTTP_Error.SERVICE_UNAVAILABLE,
     HTTP_Error.GATEWAY_TIME_OUT,
     HTTP_Error.SERVER_UNKNOWN_ERROR,
 )
 
@@ -278,15 +279,15 @@
             try:
                 resp = cast(
                     ClientResponse,
                     await getattr(self._session, method)(url, **kwargs),
                 )
                 status = resp.status
                 resp.raise_for_status()
-            except ClientError as exc:
+            except (ClientError, *_TIMEOUT_EXCEPTIONS) as exc:
                 self._logger.debug(
                     "Request error: %s(%s), attempt %i: %s",
                     method.upper(),
                     self._redact(url, _URL_REDACTIONS),
                     attempt,
                     self._redact(repr(exc), _EXC_REPR_REDACTIONS),
                 )
```

### Comparing `life360-7.0.0b6/life360/const.py` & `life360-7.0.1/life360/const.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b6/life360/exceptions.py` & `life360-7.0.1/life360/exceptions.py`

 * *Files identical despite different names*

### Comparing `life360-7.0.0b6/life360.egg-info/PKG-INFO` & `life360-7.0.1/life360.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: life360
-Version: 7.0.0b6
+Version: 7.0.1
 Summary: Life360 Communications Module
 Home-page: https://github.com/pnbruckner/life360
 Author: Phil Bruckner
 Author-email: pnbruckner@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `life360-7.0.0b6/setup.py` & `life360-7.0.1/setup.py`

 * *Files identical despite different names*

