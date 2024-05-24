# Comparing `tmp/atla-0.1.0a2.tar.gz` & `tmp/atla-0.1.0a3.tar.gz`

## Comparing `atla-0.1.0a2.tar` & `atla-0.1.0a3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/__init__.py
--rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_base_client.py
--rw-r--r--   0        0        0    13419 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_resource.py
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_types.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/lib/.keep
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/resources/__init__.py
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/resources/evaluate.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/types/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/types/evaluate_create_params.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/types/evaluate_create_response.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.0a2/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 atla-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0    14043 2020-02-02 00:00:00.000000 atla-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/__init__.py
+-rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_base_client.py
+-rw-r--r--   0        0        0    16177 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_types.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_typing.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/lib/.keep
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/resources/__init__.py
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/resources/evaluate.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/types/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/types/evaluate_create_params.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/types/evaluate_create_response.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.0a3/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 atla-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0    14171 2020-02-02 00:00:00.000000 atla-0.1.0a3/PKG-INFO
```

### Comparing `atla-0.1.0a2/src/atla/__init__.py` & `atla-0.1.0a3/src/atla/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from . import types
 from ._types import NOT_GIVEN, NoneType, NotGiven, Transport, ProxiesTypes
 from ._utils import file_from_path
-from ._client import Atla, Client, Stream, Timeout, AsyncAtla, Transport, AsyncClient, AsyncStream, RequestOptions
+from ._client import (
+    ENVIRONMENTS,
+    Atla,
+    Client,
+    Stream,
+    Timeout,
+    AsyncAtla,
+    Transport,
+    AsyncClient,
+    AsyncStream,
+    RequestOptions,
+)
 from ._models import BaseModel
 from ._version import __title__, __version__
 from ._response import APIResponse as APIResponse, AsyncAPIResponse as AsyncAPIResponse
 from ._constants import DEFAULT_TIMEOUT, DEFAULT_MAX_RETRIES, DEFAULT_CONNECTION_LIMITS
 from ._exceptions import (
     APIError,
     AtlaError,
@@ -54,14 +65,15 @@
     "RequestOptions",
     "Client",
     "AsyncClient",
     "Stream",
     "AsyncStream",
     "Atla",
     "AsyncAtla",
+    "ENVIRONMENTS",
     "file_from_path",
     "BaseModel",
     "DEFAULT_TIMEOUT",
     "DEFAULT_MAX_RETRIES",
     "DEFAULT_CONNECTION_LIMITS",
     "DefaultHttpxClient",
     "DefaultAsyncHttpxClient",
```

### Comparing `atla-0.1.0a2/src/atla/_base_client.py` & `atla-0.1.0a3/src/atla/_base_client.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_client.py` & `atla-0.1.0a3/src/atla/_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 import os
-from typing import Any, Union, Mapping
-from typing_extensions import Self, override
+from typing import Any, Dict, Union, Mapping, cast
+from typing_extensions import Self, Literal, override
 
 import httpx
 
 from . import resources, _exceptions
 from ._qs import Querystring
 from ._types import (
     NOT_GIVEN,
@@ -29,37 +29,46 @@
 from ._base_client import (
     DEFAULT_MAX_RETRIES,
     SyncAPIClient,
     AsyncAPIClient,
 )
 
 __all__ = [
+    "ENVIRONMENTS",
     "Timeout",
     "Transport",
     "ProxiesTypes",
     "RequestOptions",
     "resources",
     "Atla",
     "AsyncAtla",
     "Client",
     "AsyncClient",
 ]
 
+ENVIRONMENTS: Dict[str, str] = {
+    "production": "https://api.atla-ai.com",
+    "development": "https://api-dev.atla-ai.com",
+}
+
 
 class Atla(SyncAPIClient):
     evaluate: resources.EvaluateResource
     with_raw_response: AtlaWithRawResponse
     with_streaming_response: AtlaWithStreamedResponse
 
     # client options
 
+    _environment: Literal["production", "development"] | NotGiven
+
     def __init__(
         self,
         *,
-        base_url: str | httpx.URL | None = None,
+        environment: Literal["production", "development"] | NotGiven = NOT_GIVEN,
+        base_url: str | httpx.URL | None | NotGiven = NOT_GIVEN,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         # Configure a custom httpx client.
         # We provide a `DefaultHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
         # See the [httpx documentation](https://www.python-httpx.org/api/#client) for more details.
@@ -71,18 +80,39 @@
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new synchronous atla client instance."""
-        if base_url is None:
-            base_url = os.environ.get("ATLA_BASE_URL")
-        if base_url is None:
-            base_url = f"https://localhost:8080/test-api"
+        self._environment = environment
+
+        base_url_env = os.environ.get("ATLA_BASE_URL")
+        if is_given(base_url) and base_url is not None:
+            # cast required because mypy doesn't understand the type narrowing
+            base_url = cast("str | httpx.URL", base_url)  # pyright: ignore[reportUnnecessaryCast]
+        elif is_given(environment):
+            if base_url_env and base_url is not None:
+                raise ValueError(
+                    "Ambiguous URL; The `ATLA_BASE_URL` env var and the `environment` argument are given. If you want to use the environment, you must pass base_url=None",
+                )
+
+            try:
+                base_url = ENVIRONMENTS[environment]
+            except KeyError as exc:
+                raise ValueError(f"Unknown environment: {environment}") from exc
+        elif base_url_env is not None:
+            base_url = base_url_env
+        else:
+            self._environment = environment = "production"
+
+            try:
+                base_url = ENVIRONMENTS[environment]
+            except KeyError as exc:
+                raise ValueError(f"Unknown environment: {environment}") from exc
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             http_client=http_client,
@@ -108,14 +138,15 @@
             "X-Stainless-Async": "false",
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
+        environment: Literal["production", "development"] | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.Client | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
@@ -142,14 +173,15 @@
             params = {**params, **default_query}
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
             base_url=base_url or self.base_url,
+            environment=environment or self._environment,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
             **_extra_kwargs,
         )
@@ -195,18 +227,21 @@
 class AsyncAtla(AsyncAPIClient):
     evaluate: resources.AsyncEvaluateResource
     with_raw_response: AsyncAtlaWithRawResponse
     with_streaming_response: AsyncAtlaWithStreamedResponse
 
     # client options
 
+    _environment: Literal["production", "development"] | NotGiven
+
     def __init__(
         self,
         *,
-        base_url: str | httpx.URL | None = None,
+        environment: Literal["production", "development"] | NotGiven = NOT_GIVEN,
+        base_url: str | httpx.URL | None | NotGiven = NOT_GIVEN,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         # Configure a custom httpx client.
         # We provide a `DefaultAsyncHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
         # See the [httpx documentation](https://www.python-httpx.org/api/#asyncclient) for more details.
@@ -218,18 +253,39 @@
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new async atla client instance."""
-        if base_url is None:
-            base_url = os.environ.get("ATLA_BASE_URL")
-        if base_url is None:
-            base_url = f"https://localhost:8080/test-api"
+        self._environment = environment
+
+        base_url_env = os.environ.get("ATLA_BASE_URL")
+        if is_given(base_url) and base_url is not None:
+            # cast required because mypy doesn't understand the type narrowing
+            base_url = cast("str | httpx.URL", base_url)  # pyright: ignore[reportUnnecessaryCast]
+        elif is_given(environment):
+            if base_url_env and base_url is not None:
+                raise ValueError(
+                    "Ambiguous URL; The `ATLA_BASE_URL` env var and the `environment` argument are given. If you want to use the environment, you must pass base_url=None",
+                )
+
+            try:
+                base_url = ENVIRONMENTS[environment]
+            except KeyError as exc:
+                raise ValueError(f"Unknown environment: {environment}") from exc
+        elif base_url_env is not None:
+            base_url = base_url_env
+        else:
+            self._environment = environment = "production"
+
+            try:
+                base_url = ENVIRONMENTS[environment]
+            except KeyError as exc:
+                raise ValueError(f"Unknown environment: {environment}") from exc
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             http_client=http_client,
@@ -255,14 +311,15 @@
             "X-Stainless-Async": f"async:{get_async_library()}",
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
+        environment: Literal["production", "development"] | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.AsyncClient | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
@@ -289,14 +346,15 @@
             params = {**params, **default_query}
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
             base_url=base_url or self.base_url,
+            environment=environment or self._environment,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
             **_extra_kwargs,
         )
```

### Comparing `atla-0.1.0a2/src/atla/_compat.py` & `atla-0.1.0a3/src/atla/_compat.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_exceptions.py` & `atla-0.1.0a3/src/atla/_exceptions.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_files.py` & `atla-0.1.0a3/src/atla/_files.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_models.py` & `atla-0.1.0a3/src/atla/_models.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_qs.py` & `atla-0.1.0a3/src/atla/_qs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_resource.py` & `atla-0.1.0a3/src/atla/_resource.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_response.py` & `atla-0.1.0a3/src/atla/_response.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_streaming.py` & `atla-0.1.0a3/src/atla/_streaming.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_types.py` & `atla-0.1.0a3/src/atla/_types.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_utils/__init__.py` & `atla-0.1.0a3/src/atla/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_utils/_logs.py` & `atla-0.1.0a3/src/atla/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_utils/_proxy.py` & `atla-0.1.0a3/src/atla/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_utils/_sync.py` & `atla-0.1.0a3/src/atla/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_utils/_transform.py` & `atla-0.1.0a3/src/atla/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_utils/_typing.py` & `atla-0.1.0a3/src/atla/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/_utils/_utils.py` & `atla-0.1.0a3/src/atla/_utils/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     overload,
 )
 from pathlib import Path
 from typing_extensions import TypeGuard
 
 import sniffio
 
-from .._types import Headers, NotGiven, FileTypes, NotGivenOr, HeadersLike
+from .._types import NotGiven, FileTypes, NotGivenOr, HeadersLike
 from .._compat import parse_date as parse_date, parse_datetime as parse_datetime
 
 _T = TypeVar("_T")
 _TupleT = TypeVar("_TupleT", bound=Tuple[object, ...])
 _MappingT = TypeVar("_MappingT", bound=Mapping[str, object])
 _SequenceT = TypeVar("_SequenceT", bound=Sequence[object])
 CallableT = TypeVar("CallableT", bound=Callable[..., Any])
@@ -366,15 +366,14 @@
     file_name = os.path.basename(path)
     return (file_name, contents)
 
 
 def get_required_header(headers: HeadersLike, header: str) -> str:
     lower_header = header.lower()
     if isinstance(headers, Mapping):
-        headers = cast(Headers, headers)
         for k, v in headers.items():
             if k.lower() == lower_header and isinstance(v, str):
                 return v
 
     """ to deal with the case where the header looks like Stainless-Event-Id """
     intercaps_header = re.sub(r"([^\w])(\w)", lambda pat: pat.group(1) + pat.group(2).upper(), header.capitalize())
```

### Comparing `atla-0.1.0a2/src/atla/resources/__init__.py` & `atla-0.1.0a3/src/atla/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/resources/evaluate.py` & `atla-0.1.0a3/src/atla/resources/evaluate.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/types/evaluate_create_params.py` & `atla-0.1.0a3/src/atla/types/evaluate_create_params.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/src/atla/types/evaluate_create_response.py` & `atla-0.1.0a3/src/atla/types/evaluate_create_response.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/LICENSE` & `atla-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a2/pyproject.toml` & `atla-0.1.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atla"
-version = "0.1.0-alpha.2"
+version = "0.1.0-alpha.3"
 description = "The official Python library for the atla API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Atla", email = "support@atla.com" },
 ]
 dependencies = [
```

### Comparing `atla-0.1.0a2/PKG-INFO` & `atla-0.1.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: atla
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: The official Python library for the atla API
 Project-URL: Homepage, https://github.com/atla-ai/atla-sdk-python
 Project-URL: Repository, https://github.com/atla-ai/atla-sdk-python
 Author-email: Atla <support@atla.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -57,15 +57,18 @@
 ## Usage
 
 The full API of this library can be found in [api.md](https://github.com/atla-ai/atla-sdk-python/tree/main/api.md).
 
 ```python
 from atla import Atla
 
-client = Atla()
+client = Atla(
+    # defaults to "production".
+    environment="development",
+)
 
 evaluate_create_response = client.evaluate.create(
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
     metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
 )
 print(evaluate_create_response.evaluations)
@@ -75,15 +78,18 @@
 
 Simply import `AsyncAtla` instead of `Atla` and use `await` with each API call:
 
 ```python
 import asyncio
 from atla import AsyncAtla
 
-client = AsyncAtla()
+client = AsyncAtla(
+    # defaults to "production".
+    environment="development",
+)
 
 
 async def main() -> None:
     evaluate_create_response = await client.evaluate.create(
         input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
         metrics=["precision", "recall"],
         response="If you have any questions about my rate, please let me know.",
```

