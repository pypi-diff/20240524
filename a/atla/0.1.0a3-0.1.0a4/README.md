# Comparing `tmp/atla-0.1.0a3.tar.gz` & `tmp/atla-0.1.0a4.tar.gz`

## Comparing `atla-0.1.0a3.tar` & `atla-0.1.0a4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/__init__.py
--rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_base_client.py
--rw-r--r--   0        0        0    16177 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_resource.py
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_types.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_typing.py
--rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/lib/.keep
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/resources/__init__.py
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/resources/evaluate.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/types/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/types/evaluate_create_params.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 atla-0.1.0a3/src/atla/types/evaluate_create_response.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.0a3/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.0a3/LICENSE
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 atla-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0    14171 2020-02-02 00:00:00.000000 atla-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/__init__.py
+-rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_base_client.py
+-rw-r--r--   0        0        0    17390 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_types.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_utils/_typing.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/lib/.keep
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/resources/__init__.py
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/resources/evaluate.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/types/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/types/evaluate_create_params.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 atla-0.1.0a4/src/atla/types/evaluate_create_response.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.0a4/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.0a4/LICENSE
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 atla-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0    14381 2020-02-02 00:00:00.000000 atla-0.1.0a4/PKG-INFO
```

### Comparing `atla-0.1.0a3/src/atla/__init__.py` & `atla-0.1.0a4/src/atla/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_base_client.py` & `atla-0.1.0a4/src/atla/_base_client.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_client.py` & `atla-0.1.0a4/src/atla/_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 )
 from ._utils import (
     is_given,
     get_async_library,
 )
 from ._version import __version__
 from ._streaming import Stream as Stream, AsyncStream as AsyncStream
-from ._exceptions import APIStatusError
+from ._exceptions import AtlaError, APIStatusError
 from ._base_client import (
     DEFAULT_MAX_RETRIES,
     SyncAPIClient,
     AsyncAPIClient,
 )
 
 __all__ = [
@@ -53,20 +53,22 @@
 
 class Atla(SyncAPIClient):
     evaluate: resources.EvaluateResource
     with_raw_response: AtlaWithRawResponse
     with_streaming_response: AtlaWithStreamedResponse
 
     # client options
+    api_key: str
 
     _environment: Literal["production", "development"] | NotGiven
 
     def __init__(
         self,
         *,
+        api_key: str | None = None,
         environment: Literal["production", "development"] | NotGiven = NOT_GIVEN,
         base_url: str | httpx.URL | None | NotGiven = NOT_GIVEN,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         # Configure a custom httpx client.
@@ -79,15 +81,26 @@
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
-        """Construct a new synchronous atla client instance."""
+        """Construct a new synchronous atla client instance.
+
+        This automatically infers the `api_key` argument from the `ATLA_API_KEY` environment variable if it is not provided.
+        """
+        if api_key is None:
+            api_key = os.environ.get("ATLA_API_KEY")
+        if api_key is None:
+            raise AtlaError(
+                "The api_key client option must be set either by passing api_key to the client or by setting the ATLA_API_KEY environment variable"
+            )
+        self.api_key = api_key
+
         self._environment = environment
 
         base_url_env = os.environ.get("ATLA_BASE_URL")
         if is_given(base_url) and base_url is not None:
             # cast required because mypy doesn't understand the type narrowing
             base_url = cast("str | httpx.URL", base_url)  # pyright: ignore[reportUnnecessaryCast]
         elif is_given(environment):
@@ -138,14 +151,15 @@
             "X-Stainless-Async": "false",
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
+        api_key: str | None = None,
         environment: Literal["production", "development"] | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.Client | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
@@ -172,14 +186,15 @@
         if default_query is not None:
             params = {**params, **default_query}
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
+            api_key=api_key or self.api_key,
             base_url=base_url or self.base_url,
             environment=environment or self._environment,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
@@ -226,20 +241,22 @@
 
 class AsyncAtla(AsyncAPIClient):
     evaluate: resources.AsyncEvaluateResource
     with_raw_response: AsyncAtlaWithRawResponse
     with_streaming_response: AsyncAtlaWithStreamedResponse
 
     # client options
+    api_key: str
 
     _environment: Literal["production", "development"] | NotGiven
 
     def __init__(
         self,
         *,
+        api_key: str | None = None,
         environment: Literal["production", "development"] | NotGiven = NOT_GIVEN,
         base_url: str | httpx.URL | None | NotGiven = NOT_GIVEN,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         # Configure a custom httpx client.
@@ -252,15 +269,26 @@
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
-        """Construct a new async atla client instance."""
+        """Construct a new async atla client instance.
+
+        This automatically infers the `api_key` argument from the `ATLA_API_KEY` environment variable if it is not provided.
+        """
+        if api_key is None:
+            api_key = os.environ.get("ATLA_API_KEY")
+        if api_key is None:
+            raise AtlaError(
+                "The api_key client option must be set either by passing api_key to the client or by setting the ATLA_API_KEY environment variable"
+            )
+        self.api_key = api_key
+
         self._environment = environment
 
         base_url_env = os.environ.get("ATLA_BASE_URL")
         if is_given(base_url) and base_url is not None:
             # cast required because mypy doesn't understand the type narrowing
             base_url = cast("str | httpx.URL", base_url)  # pyright: ignore[reportUnnecessaryCast]
         elif is_given(environment):
@@ -311,14 +339,15 @@
             "X-Stainless-Async": f"async:{get_async_library()}",
             **self._custom_headers,
         }
 
     def copy(
         self,
         *,
+        api_key: str | None = None,
         environment: Literal["production", "development"] | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | Timeout | None | NotGiven = NOT_GIVEN,
         http_client: httpx.AsyncClient | None = None,
         max_retries: int | NotGiven = NOT_GIVEN,
         default_headers: Mapping[str, str] | None = None,
         set_default_headers: Mapping[str, str] | None = None,
@@ -345,14 +374,15 @@
         if default_query is not None:
             params = {**params, **default_query}
         elif set_default_query is not None:
             params = set_default_query
 
         http_client = http_client or self._client
         return self.__class__(
+            api_key=api_key or self.api_key,
             base_url=base_url or self.base_url,
             environment=environment or self._environment,
             timeout=self.timeout if isinstance(timeout, NotGiven) else timeout,
             http_client=http_client,
             max_retries=max_retries if is_given(max_retries) else self.max_retries,
             default_headers=headers,
             default_query=params,
```

### Comparing `atla-0.1.0a3/src/atla/_compat.py` & `atla-0.1.0a4/src/atla/_compat.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_exceptions.py` & `atla-0.1.0a4/src/atla/_exceptions.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_files.py` & `atla-0.1.0a4/src/atla/_files.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_models.py` & `atla-0.1.0a4/src/atla/_models.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_qs.py` & `atla-0.1.0a4/src/atla/_qs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_resource.py` & `atla-0.1.0a4/src/atla/_resource.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_response.py` & `atla-0.1.0a4/src/atla/_response.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_streaming.py` & `atla-0.1.0a4/src/atla/_streaming.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_types.py` & `atla-0.1.0a4/src/atla/_types.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_utils/__init__.py` & `atla-0.1.0a4/src/atla/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_utils/_logs.py` & `atla-0.1.0a4/src/atla/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_utils/_proxy.py` & `atla-0.1.0a4/src/atla/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_utils/_sync.py` & `atla-0.1.0a4/src/atla/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_utils/_transform.py` & `atla-0.1.0a4/src/atla/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_utils/_typing.py` & `atla-0.1.0a4/src/atla/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/_utils/_utils.py` & `atla-0.1.0a4/src/atla/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/resources/__init__.py` & `atla-0.1.0a4/src/atla/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/resources/evaluate.py` & `atla-0.1.0a4/src/atla/resources/evaluate.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/types/evaluate_create_params.py` & `atla-0.1.0a4/src/atla/types/evaluate_create_params.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/src/atla/types/evaluate_create_response.py` & `atla-0.1.0a4/src/atla/types/evaluate_create_response.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/LICENSE` & `atla-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a3/pyproject.toml` & `atla-0.1.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atla"
-version = "0.1.0-alpha.3"
+version = "0.1.0-alpha.4"
 description = "The official Python library for the atla API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Atla", email = "support@atla.com" },
 ]
 dependencies = [
```

### Comparing `atla-0.1.0a3/PKG-INFO` & `atla-0.1.0a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: atla
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: The official Python library for the atla API
 Project-URL: Homepage, https://github.com/atla-ai/atla-sdk-python
 Project-URL: Repository, https://github.com/atla-ai/atla-sdk-python
 Author-email: Atla <support@atla.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -60,14 +60,15 @@
 
 ```python
 from atla import Atla
 
 client = Atla(
     # defaults to "production".
     environment="development",
+    api_key="My API Key",
 )
 
 evaluate_create_response = client.evaluate.create(
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
     metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
 )
@@ -81,14 +82,15 @@
 ```python
 import asyncio
 from atla import AsyncAtla
 
 client = AsyncAtla(
     # defaults to "production".
     environment="development",
+    api_key="My API Key",
 )
 
 
 async def main() -> None:
     evaluate_create_response = await client.evaluate.create(
         input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
         metrics=["precision", "recall"],
@@ -120,15 +122,17 @@
 
 All errors inherit from `atla.APIError`.
 
 ```python
 import atla
 from atla import Atla
 
-client = Atla()
+client = Atla(
+    api_key="My API Key",
+)
 
 try:
     client.evaluate.create(
         input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
         metrics=["precision", "recall"],
         response="If you have any questions about my rate, please let me know.",
     )
@@ -167,14 +171,15 @@
 ```python
 from atla import Atla
 
 # Configure the default for all requests:
 client = Atla(
     # default is 2
     max_retries=0,
+    api_key="My API Key",
 )
 
 # Or, configure per-request:
 client.with_options(max_retries=5).evaluate.create(
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
     metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
@@ -189,19 +194,21 @@
 ```python
 from atla import Atla
 
 # Configure the default for all requests:
 client = Atla(
     # 20 seconds (default is 1 minute)
     timeout=20.0,
+    api_key="My API Key",
 )
 
 # More granular control:
 client = Atla(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
+    api_key="My API Key",
 )
 
 # Override per-request:
 client.with_options(timeout=5.0).evaluate.create(
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
     metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
@@ -239,15 +246,17 @@
 ### Accessing raw response data (e.g. headers)
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
 from atla import Atla
 
-client = Atla()
+client = Atla(
+    api_key="My API Key",
+)
 response = client.evaluate.with_raw_response.create(
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
     metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
 )
 print(response.headers.get('X-My-Header'))
 
@@ -328,14 +337,15 @@
 client = Atla(
     # Or use the `ATLA_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
     http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
     ),
+    api_key="My API Key",
 )
 ```
 
 ### Managing HTTP resources
 
 By default the library closes underlying HTTP connections whenever the client is [garbage collected](https://docs.python.org/3/reference/datamodel.html#object.__del__). You can manually close the client using the `.close()` method if desired, or with a context manager that closes when exiting.
```

