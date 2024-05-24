# Comparing `tmp/writer_sdk-0.1.0a2.tar.gz` & `tmp/writer_sdk-0.1.0a3.tar.gz`

## Comparing `writer_sdk-0.1.0a2.tar` & `writer_sdk-0.1.0a3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writer/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writer_ai/lib/.keep
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/__init__.py
--rw-r--r--   0        0        0    64416 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_base_client.py
--rw-r--r--   0        0        0    16163 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_constants.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_resource.py
--rw-r--r--   0        0        0    28383 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_response.py
--rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_streaming.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_types.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/__init__.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/lib/.keep
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/resources/__init__.py
--rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/resources/chat.py
--rw-r--r--   0        0        0    14107 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/resources/completions.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/resources/models.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/chat.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/chat_chat_params.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/chat_streaming_data.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/completion.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/completion_create_params.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/model_list_response.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/src/writerai/types/streaming_data.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writer/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writer_ai/lib/.keep
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/__init__.py
+-rw-r--r--   0        0        0    64416 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_base_client.py
+-rw-r--r--   0        0        0    16155 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_constants.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_resource.py
+-rw-r--r--   0        0        0    28383 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_response.py
+-rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_streaming.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_types.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_utils/__init__.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_utils/_typing.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/lib/.keep
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/resources/__init__.py
+-rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/resources/chat.py
+-rw-r--r--   0        0        0    14107 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/resources/completions.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/resources/models.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/types/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/types/chat.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/types/chat_chat_params.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/types/chat_streaming_data.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/types/completion.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/types/completion_create_params.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/types/model_list_response.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/src/writerai/types/streaming_data.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 writer_sdk-0.1.0a3/PKG-INFO
```

### Comparing `writer_sdk-0.1.0a2/src/writerai/__init__.py` & `writer_sdk-0.1.0a3/src/writerai/__init__.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_base_client.py` & `writer_sdk-0.1.0a3/src/writerai/_base_client.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_client.py` & `writer_sdk-0.1.0a3/src/writerai/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 "The api_key client option must be set either by passing api_key to the client or by setting the WRITER_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
             base_url = os.environ.get("WRITER_BASE_URL")
         if base_url is None:
-            base_url = f"https://api.qordobadev.com"
+            base_url = f"https://api.writer.com"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             http_client=http_client,
@@ -263,15 +263,15 @@
                 "The api_key client option must be set either by passing api_key to the client or by setting the WRITER_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
             base_url = os.environ.get("WRITER_BASE_URL")
         if base_url is None:
-            base_url = f"https://api.qordobadev.com"
+            base_url = f"https://api.writer.com"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             http_client=http_client,
```

### Comparing `writer_sdk-0.1.0a2/src/writerai/_compat.py` & `writer_sdk-0.1.0a3/src/writerai/_compat.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_exceptions.py` & `writer_sdk-0.1.0a3/src/writerai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_files.py` & `writer_sdk-0.1.0a3/src/writerai/_files.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_models.py` & `writer_sdk-0.1.0a3/src/writerai/_models.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_qs.py` & `writer_sdk-0.1.0a3/src/writerai/_qs.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_resource.py` & `writer_sdk-0.1.0a3/src/writerai/_resource.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_response.py` & `writer_sdk-0.1.0a3/src/writerai/_response.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_streaming.py` & `writer_sdk-0.1.0a3/src/writerai/_streaming.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_types.py` & `writer_sdk-0.1.0a3/src/writerai/_types.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_utils/__init__.py` & `writer_sdk-0.1.0a3/src/writerai/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_utils/_logs.py` & `writer_sdk-0.1.0a3/src/writerai/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_utils/_proxy.py` & `writer_sdk-0.1.0a3/src/writerai/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_utils/_sync.py` & `writer_sdk-0.1.0a3/src/writerai/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_utils/_transform.py` & `writer_sdk-0.1.0a3/src/writerai/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_utils/_typing.py` & `writer_sdk-0.1.0a3/src/writerai/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/_utils/_utils.py` & `writer_sdk-0.1.0a3/src/writerai/_utils/_utils.py`

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

### Comparing `writer_sdk-0.1.0a2/src/writerai/resources/__init__.py` & `writer_sdk-0.1.0a3/src/writerai/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/resources/chat.py` & `writer_sdk-0.1.0a3/src/writerai/resources/chat.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/resources/completions.py` & `writer_sdk-0.1.0a3/src/writerai/resources/completions.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/resources/models.py` & `writer_sdk-0.1.0a3/src/writerai/resources/models.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/types/__init__.py` & `writer_sdk-0.1.0a3/src/writerai/types/__init__.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/types/chat.py` & `writer_sdk-0.1.0a3/src/writerai/types/chat.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/types/chat_chat_params.py` & `writer_sdk-0.1.0a3/src/writerai/types/chat_chat_params.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/types/completion.py` & `writer_sdk-0.1.0a3/src/writerai/types/completion.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/src/writerai/types/completion_create_params.py` & `writer_sdk-0.1.0a3/src/writerai/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/LICENSE` & `writer_sdk-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `writer_sdk-0.1.0a2/pyproject.toml` & `writer_sdk-0.1.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "writer-sdk"
-version = "0.1.0-alpha.2"
+version = "0.1.0-alpha.3"
 description = "The official Python library for the writer API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Writer", email = "dev-feedback@writer.com" },
 ]
 dependencies = [
```

### Comparing `writer_sdk-0.1.0a2/PKG-INFO` & `writer_sdk-0.1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: writer-sdk
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: The official Python library for the writer API
 Project-URL: Homepage, https://github.com/WriterColab/sdk.python
 Project-URL: Repository, https://github.com/WriterColab/sdk.python
 Author-email: Writer <dev-feedback@writer.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

