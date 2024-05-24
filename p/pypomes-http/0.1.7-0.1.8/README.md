# Comparing `tmp/pypomes_http-0.1.7.tar.gz` & `tmp/pypomes_http-0.1.8.tar.gz`

## Comparing `pypomes_http-0.1.7.tar` & `pypomes_http-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/src/pypomes_http/__init__.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/src/pypomes_http/http_async.py
--rw-r--r--   0        0        0    15862 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/src/pypomes_http/http_pomes.py
--rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/src/pypomes_http/http_statuses.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 pypomes_http-0.1.8/src/pypomes_http/__init__.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pypomes_http-0.1.8/src/pypomes_http/http_async.py
+-rw-r--r--   0        0        0    17497 2020-02-02 00:00:00.000000 pypomes_http-0.1.8/src/pypomes_http/http_pomes.py
+-rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 pypomes_http-0.1.8/src/pypomes_http/http_statuses.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.8/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.8/PKG-INFO
```

### Comparing `pypomes_http-0.1.7/src/pypomes_http/__init__.py` & `pypomes_http-0.1.8/src/pypomes_http/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from .http_async import (
     HttpAsync,
 )
 from .http_pomes import (
-    HTTP_DELETE_TIMEOUT, HTTP_GET_TIMEOUT, HTTP_PATCH_TIMEOUT, HTTP_POST_TIMEOUT, HTTP_PUT_TIMEOUT,
+    HTTP_DELETE_TIMEOUT, HTTP_GET_TIMEOUT, HTTP_HEAD_TIMEOUT,
+    HTTP_PATCH_TIMEOUT, HTTP_POST_TIMEOUT, HTTP_PUT_TIMEOUT,
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
     http_status_code, http_status_name, http_status_description,
     http_get_parameter, http_get_parameters,
-    http_delete, http_get, http_patch, http_post, http_put,
+    http_delete, http_get,  http_head, http_patch, http_post, http_put,
 )
 
 __all__ = [
     # http_async
     "HttpAsync",
     # http_pomes
-    "HTTP_DELETE_TIMEOUT", "HTTP_GET_TIMEOUT", "HTTP_PATCH_TIMEOUT", "HTTP_POST_TIMEOUT", "HTTP_PUT_TIMEOUT",
+    "HTTP_DELETE_TIMEOUT", "HTTP_GET_TIMEOUT", "HTTP_HEAD_TIMEOUT",
+    "HTTP_PATCH_TIMEOUT", "HTTP_POST_TIMEOUT", "HTTP_PUT_TIMEOUT",
     "MIMETYPE_BINARY", "MIMETYPE_CSS", "MIMETYPE_CSV", "MIMETYPE_HTML", "MIMETYPE_JAVASCRIPT",
     "MIMETYPE_JSON", "MIMETYPE_MULTIPART", "MIMETYPE_PDF", "MIMETYPE_PKCS7", "MIMETYPE_SOAP",
     "MIMETYPE_TEXT", "MIMETYPE_URLENCODED", "MIMETYPE_XML", "MIMETYPE_ZIP",
     "http_status_code", "http_status_name", "http_status_description",
     "http_get_parameter", "http_get_parameters",
-    "http_delete", "http_get", "http_patch", "http_post", "http_put",
+    "http_delete", "http_get", "http_head", "http_patch", "http_post", "http_put",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_http")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_http-0.1.7/src/pypomes_http/http_async.py` & `pypomes_http-0.1.8/src/pypomes_http/http_async.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.7/src/pypomes_http/http_pomes.py` & `pypomes_http-0.1.8/src/pypomes_http/http_pomes.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from requests import Response
 from typing import Any, Final
 
 from .http_statuses import _HTTP_STATUSES
 
 HTTP_DELETE_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_DELETE_TIMEOUT", 300)
 HTTP_GET_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_GET_TIMEOUT", 300)
+HTTP_HEAD_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_HEAD_TIMEOUT", 300)
 HTTP_PATCH_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_POST_TIMEOUT", 300)
 HTTP_POST_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_POST_TIMEOUT", 300)
 HTTP_PUT_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_PUT_TIMEOUT", 300)
 
 MIMETYPE_BINARY: Final[str] = "application/octet-stream"
 MIMETYPE_CSS: Final[str] = "text/css"
 MIMETYPE_CSV: Final[str] = "text/csv"
@@ -148,15 +149,15 @@
                 headers: dict = None,
                 params: dict = None,
                 data: dict = None,
                 json: dict = None, auth: str = None,
                 timeout: int | None = HTTP_DELETE_TIMEOUT,
                 logger: logging.Logger = None) -> Response:
     """
-    Issue a *DELETE* request to the given *url*, and return the retrieved response.
+    Issue a *DELETE* request to the given *url*, and return the response received.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
@@ -176,15 +177,15 @@
              headers: dict = None,
              params: dict = None,
              data: dict = None,
              json: dict = None, auth: str = None,
              timeout: int | None = HTTP_GET_TIMEOUT,
              logger: logging.Logger = None) -> Response:
     """
-    Issue a *GET* request to the given *url*, and return the retrieved response.
+    Issue a *GET* request to the given *url*, and return the response received.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
@@ -196,24 +197,53 @@
     :param logger: optional logger
     :return: the response to the GET operation
     """
     return _http_rest(errors, "GET", url, headers,
                       params, data, json, auth, timeout, logger)
 
 
+def http_head(errors: list[str] | None,
+              url: str,
+              headers: dict = None,
+              params: dict = None,
+              data: dict = None,
+              json: dict = None, auth: str = None,
+              timeout: int | None = HTTP_HEAD_TIMEOUT,
+              logger: logging.Logger = None) -> Response:
+    """
+    Issue a *HEAD* request to the given *url*, and return the response received.
+
+    The returned response might be *None*.
+    The request might contain *headers* and *parameters*.
+
+    :param errors: incidental error messages
+    :param url: the destination URL
+    :param headers: optional headers
+    :param params: optional parameters
+    :param data: optionaL data to send in the body of the request
+    :param json: optional JSON to send in the body of the request
+    :param auth: optional authentication scheme to use
+    :param timeout: timeout, in seconds (defaults to HTTP_GET_TIMEOUT - use None to omit)
+    :param logger: optional logger
+    :return: the response to the GET operation
+    """
+    return _http_rest(errors, "HEAD", url, headers,
+                      params, data, json, auth, timeout, logger)
+
+
 def http_patch(errors: list[str] | None,
                url: str,
                headers: dict = None,
                params: dict = None,
                data: dict = None,
                json: dict = None, auth: str = None,
                timeout: int | None = HTTP_PATCH_TIMEOUT,
                logger: logging.Logger = None) -> Response:
     """
-    Issue a *PATCH* request to the given *url*, and return the retrieved response.
+    Issue a *PATCH* request to the given *url*, and return the response received.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
@@ -235,15 +265,15 @@
               params: dict = None,
               data: dict = None,
               json: dict = None,
               auth: str = None,
               timeout: int | None = HTTP_POST_TIMEOUT,
               logger: logging.Logger = None) -> Response:
     """
-    Issue a *POST* request to the given *url*, and return the retrieved response.
+    Issue a *POST* request to the given *url*, and return the response received.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
@@ -262,18 +292,18 @@
 def http_put(errors: list[str] | None,
              url: str,
              headers: dict = None,
              params: dict = None,
              data: dict = None,
              json: dict = None,
              auth: str = None,
-             timeout: int | None = HTTP_POST_TIMEOUT,
+             timeout: int | None = HTTP_PUT_TIMEOUT,
              logger: logging.Logger = None) -> Response:
     """
-    Issue a *PUT* request to the given *url*, and return the retrieved response.
+    Issue a *PUT* request to the given *url*, and return the response received.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
@@ -296,21 +326,21 @@
                params: dict,
                data: dict | None,
                json: dict | None,
                auth: str | None,
                timeout: int,
                logger: logging.Logger) -> Response:
     """
-    Issue a *REST* request to the given *url*, and return the retrieved response.
+    Issue a *REST* request to the given *url*, and return the response received.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
-    :param method: the REST method to use (GET, POST or PUT)
+    :param method: the REST method to use (DELETE, GET, HEAD, PATCH, POST or PUT)
     :param url: the destination URL
     :param headers: optional headers
     :param params: optional parameters
     :param data: optionaL data to send in the body of the request
     :param json: optional JSON to send in the body of the request
     :param auth: optional authentication scheme to use
     :param timeout: timeout, in seconds (defaults to HTTP_POST_TIMEOUT - use None to omit)
@@ -364,14 +394,21 @@
                 case "GET":
                     result = requests.get(url=url,
                                           headers=op_headers,
                                           params=params,
                                           data=data,
                                           json=json,
                                           timeout=timeout)
+                case "HEAD":
+                    result = requests.head(url=url,
+                                           headers=op_headers,
+                                           params=params,
+                                           data=data,
+                                           json=json,
+                                           timeout=timeout)
                 case "PATCH":
                     result = requests.patch(url=url,
                                             headers=op_headers,
                                             params=params,
                                             data=data,
                                             json=json,
                                             timeout=timeout)
```

### Comparing `pypomes_http-0.1.7/src/pypomes_http/http_statuses.py` & `pypomes_http-0.1.8/src/pypomes_http/http_statuses.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.7/LICENSE` & `pypomes_http-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.7/pyproject.toml` & `pypomes_http-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_http"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (HTTP modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=3.0.2",
     "pip>=24.0",
-    "pypomes_core>=1.0.5",
-    "pypomes_security>=0.1.3",
+    "pypomes_core>=1.0.6",
+    "pypomes_security>=0.1.4",
     "requests>=2.31.0",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-HTTP"
```

### Comparing `pypomes_http-0.1.7/PKG-INFO` & `pypomes_http-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pypomes_http
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of Python pomes, pennyeach (HTTP modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-HTTP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-HTTP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=3.0.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=1.0.5
-Requires-Dist: pypomes-security>=0.1.3
+Requires-Dist: pypomes-core>=1.0.6
+Requires-Dist: pypomes-security>=0.1.4
 Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

