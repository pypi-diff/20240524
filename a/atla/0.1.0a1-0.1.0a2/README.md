# Comparing `tmp/atla-0.1.0a1.tar.gz` & `tmp/atla-0.1.0a2.tar.gz`

## Comparing `atla-0.1.0a1.tar` & `atla-0.1.0a2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/__init__.py
--rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_base_client.py
--rw-r--r--   0        0        0    13419 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_constants.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_qs.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_resource.py
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_response.py
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_types.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/lib/.keep
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/resources/__init__.py
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/resources/evaluate.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/types/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/types/evaluate_create_params.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 atla-0.1.0a1/src/atla/types/evaluate_create_response.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.0a1/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.0a1/LICENSE
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 atla-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0    14001 2020-02-02 00:00:00.000000 atla-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/__init__.py
+-rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_base_client.py
+-rw-r--r--   0        0        0    13419 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_response.py
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_types.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/lib/.keep
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/resources/__init__.py
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/resources/evaluate.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/types/__init__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/types/evaluate_create_params.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 atla-0.1.0a2/src/atla/types/evaluate_create_response.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 atla-0.1.0a2/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 atla-0.1.0a2/LICENSE
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 atla-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0    14043 2020-02-02 00:00:00.000000 atla-0.1.0a2/PKG-INFO
```

### Comparing `atla-0.1.0a1/src/atla/__init__.py` & `atla-0.1.0a2/src/atla/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_base_client.py` & `atla-0.1.0a2/src/atla/_base_client.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_client.py` & `atla-0.1.0a2/src/atla/_client.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_compat.py` & `atla-0.1.0a2/src/atla/_compat.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_exceptions.py` & `atla-0.1.0a2/src/atla/_exceptions.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_files.py` & `atla-0.1.0a2/src/atla/_files.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_models.py` & `atla-0.1.0a2/src/atla/_models.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_qs.py` & `atla-0.1.0a2/src/atla/_qs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_resource.py` & `atla-0.1.0a2/src/atla/_resource.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_response.py` & `atla-0.1.0a2/src/atla/_response.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_streaming.py` & `atla-0.1.0a2/src/atla/_streaming.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_types.py` & `atla-0.1.0a2/src/atla/_types.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_utils/__init__.py` & `atla-0.1.0a2/src/atla/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_utils/_logs.py` & `atla-0.1.0a2/src/atla/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_utils/_proxy.py` & `atla-0.1.0a2/src/atla/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_utils/_sync.py` & `atla-0.1.0a2/src/atla/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_utils/_transform.py` & `atla-0.1.0a2/src/atla/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_utils/_typing.py` & `atla-0.1.0a2/src/atla/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/_utils/_utils.py` & `atla-0.1.0a2/src/atla/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/resources/__init__.py` & `atla-0.1.0a2/src/atla/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/resources/evaluate.py` & `atla-0.1.0a2/src/atla/resources/evaluate.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/types/evaluate_create_params.py` & `atla-0.1.0a2/src/atla/types/evaluate_create_params.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/src/atla/types/evaluate_create_response.py` & `atla-0.1.0a2/src/atla/types/evaluate_create_response.py`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/LICENSE` & `atla-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `atla-0.1.0a1/pyproject.toml` & `atla-0.1.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atla"
-version = "0.1.0-alpha.1"
+version = "0.1.0-alpha.2"
 description = "The official Python library for the atla API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Atla", email = "support@atla.com" },
 ]
 dependencies = [
```

### Comparing `atla-0.1.0a1/PKG-INFO` & `atla-0.1.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: atla
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: The official Python library for the atla API
 Project-URL: Homepage, https://github.com/atla-ai/atla-sdk-python
 Project-URL: Repository, https://github.com/atla-ai/atla-sdk-python
 Author-email: Atla <support@atla.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -61,15 +61,15 @@
 ```python
 from atla import Atla
 
 client = Atla()
 
 evaluate_create_response = client.evaluate.create(
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
-    metrics=["contradiction"],
+    metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
 )
 print(evaluate_create_response.evaluations)
 ```
 
 ## Async usage
 
@@ -81,15 +81,15 @@
 
 client = AsyncAtla()
 
 
 async def main() -> None:
     evaluate_create_response = await client.evaluate.create(
         input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
-        metrics=["contradiction"],
+        metrics=["precision", "recall"],
         response="If you have any questions about my rate, please let me know.",
     )
     print(evaluate_create_response.evaluations)
 
 
 asyncio.run(main())
 ```
@@ -119,15 +119,15 @@
 from atla import Atla
 
 client = Atla()
 
 try:
     client.evaluate.create(
         input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
-        metrics=["contradiction"],
+        metrics=["precision", "recall"],
         response="If you have any questions about my rate, please let me know.",
     )
 except atla.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except atla.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
@@ -166,15 +166,15 @@
     # default is 2
     max_retries=0,
 )
 
 # Or, configure per-request:
 client.with_options(max_retries=5).evaluate.create(
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
-    metrics=["contradiction"],
+    metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
 )
 ```
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
@@ -193,15 +193,15 @@
 client = Atla(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
 client.with_options(timeout=5.0).evaluate.create(
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
-    metrics=["contradiction"],
+    metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests that time out are [retried twice by default](https://github.com/atla-ai/atla-sdk-python/tree/main/#retries).
@@ -236,15 +236,15 @@
 
 ```py
 from atla import Atla
 
 client = Atla()
 response = client.evaluate.with_raw_response.create(
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
-    metrics=["contradiction"],
+    metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
 )
 print(response.headers.get('X-My-Header'))
 
 evaluate = response.parse()  # get the object that `evaluate.create()` would have returned
 print(evaluate.evaluations)
 ```
@@ -258,15 +258,15 @@
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
 ```python
 with client.evaluate.with_streaming_response.create(
     input="The sentence you are given might be too wordy, complicated, or unclear. Rewrite the sentence and make your writing clearer by keeping it concise. Whenever possible, break complex sentences into multiple sentences and eliminate unnecessary words.",
-    metrics=["contradiction"],
+    metrics=["precision", "recall"],
     response="If you have any questions about my rate, please let me know.",
 ) as response:
     print(response.headers.get("X-My-Header"))
 
     for line in response.iter_lines():
         print(line)
 ```
```

