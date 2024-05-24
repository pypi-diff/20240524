# Comparing `tmp/unique_sdk-0.8.2.tar.gz` & `tmp/unique_sdk-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unique_sdk-0.8.2.tar", max compression
+gzip compressed data, was "unique_sdk-0.8.3.tar", max compression
```

## Comparing `unique_sdk-0.8.2.tar` & `unique_sdk-0.8.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1065 2024-05-22 19:47:22.860739 unique_sdk-0.8.2/LICENSE
--rw-r--r--   0        0        0    22975 2024-05-22 19:47:22.860739 unique_sdk-0.8.2/README.md
--rw-r--r--   0        0        0     1400 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2768 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/__init__.py
--rw-r--r--   0        0        0    11523 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_api_requestor.py
--rw-r--r--   0        0        0     3603 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_api_resource.py
--rw-r--r--   0        0        0       46 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_api_version.py
--rw-r--r--   0        0        0     2912 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_error.py
--rw-r--r--   0        0        0     2513 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_http_client.py
--rw-r--r--   0        0        0     3949 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_list_object.py
--rw-r--r--   0        0        0      270 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_object_classes.py
--rw-r--r--   0        0        0      255 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_request_options.py
--rw-r--r--   0        0        0    10525 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_unique_object.py
--rw-r--r--   0        0        0     1707 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_unique_ql.py
--rw-r--r--   0        0        0      576 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_unique_response.py
--rw-r--r--   0        0        0     5902 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_util.py
--rw-r--r--   0        0        0       18 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_version.py
--rw-r--r--   0        0        0     2855 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/_webhook.py
--rw-r--r--   0        0        0        0 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/api_resources/__init__.py
--rw-r--r--   0        0        0     1738 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/api_resources/_chat_completion.py
--rw-r--r--   0        0        0     3823 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/api_resources/_content.py
--rw-r--r--   0        0        0      374 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/api_resources/_event.py
--rw-r--r--   0        0        0     2310 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/api_resources/_integrated.py
--rw-r--r--   0        0        0     5025 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/api_resources/_message.py
--rw-r--r--   0        0        0     1235 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/api_resources/_search.py
--rw-r--r--   0        0        0     1366 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/api_resources/_search_string.py
--rw-r--r--   0        0        0     2532 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/api_resources/_short_term_memory.py
--rw-r--r--   0        0        0     3037 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/utils/chat_history.py
--rw-r--r--   0        0        0     2059 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/utils/file_io.py
--rw-r--r--   0        0        0     4948 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/utils/sources.py
--rw-r--r--   0        0        0     1740 2024-05-22 19:47:22.864739 unique_sdk-0.8.2/unique_sdk/utils/token.py
--rw-r--r--   0        0        0    23435 1970-01-01 00:00:00.000000 unique_sdk-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-24 14:00:10.514789 unique_sdk-0.8.3/LICENSE
+-rw-r--r--   0        0        0    23945 2024-05-24 14:00:10.514789 unique_sdk-0.8.3/README.md
+-rw-r--r--   0        0        0     1400 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2768 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/__init__.py
+-rw-r--r--   0        0        0    11523 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_api_requestor.py
+-rw-r--r--   0        0        0     3603 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_api_resource.py
+-rw-r--r--   0        0        0       46 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_api_version.py
+-rw-r--r--   0        0        0     2912 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_error.py
+-rw-r--r--   0        0        0     2513 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_http_client.py
+-rw-r--r--   0        0        0     3949 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_list_object.py
+-rw-r--r--   0        0        0      270 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_object_classes.py
+-rw-r--r--   0        0        0      255 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_request_options.py
+-rw-r--r--   0        0        0    10525 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_unique_object.py
+-rw-r--r--   0        0        0     1707 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_unique_ql.py
+-rw-r--r--   0        0        0      576 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_unique_response.py
+-rw-r--r--   0        0        0     5902 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_util.py
+-rw-r--r--   0        0        0       18 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_version.py
+-rw-r--r--   0        0        0     2855 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/_webhook.py
+-rw-r--r--   0        0        0        0 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/api_resources/__init__.py
+-rw-r--r--   0        0        0     1738 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/api_resources/_chat_completion.py
+-rw-r--r--   0        0        0     3823 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/api_resources/_content.py
+-rw-r--r--   0        0        0      374 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/api_resources/_event.py
+-rw-r--r--   0        0        0     2310 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/api_resources/_integrated.py
+-rw-r--r--   0        0        0     5025 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/api_resources/_message.py
+-rw-r--r--   0        0        0     1235 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/api_resources/_search.py
+-rw-r--r--   0        0        0     1366 2024-05-24 14:00:10.518789 unique_sdk-0.8.3/unique_sdk/api_resources/_search_string.py
+-rw-r--r--   0        0        0     1744 2024-05-24 14:00:10.522789 unique_sdk-0.8.3/unique_sdk/api_resources/_short_term_memory.py
+-rw-r--r--   0        0        0     3037 2024-05-24 14:00:10.522789 unique_sdk-0.8.3/unique_sdk/utils/chat_history.py
+-rw-r--r--   0        0        0     2059 2024-05-24 14:00:10.522789 unique_sdk-0.8.3/unique_sdk/utils/file_io.py
+-rw-r--r--   0        0        0     4948 2024-05-24 14:00:10.522789 unique_sdk-0.8.3/unique_sdk/utils/sources.py
+-rw-r--r--   0        0        0     1740 2024-05-24 14:00:10.522789 unique_sdk-0.8.3/unique_sdk/utils/token.py
+-rw-r--r--   0        0        0    24405 1970-01-01 00:00:00.000000 unique_sdk-0.8.3/PKG-INFO
```

### Comparing `unique_sdk-0.8.2/LICENSE` & `unique_sdk-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/README.md` & `unique_sdk-0.8.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 4. [Webhook Triggers](#webhook-triggers)
 5. [Available API Resources](#available-api-resources)
    - [Content](#content)
    - [Message](#message)
    - [Chat Completion](#chat-completion)
    - [Search](#search)
    - [Search String](#search-string)
+   - [Short Term Memory](#short-term-memory)
 6. [UniqueQL](#uniqueql)
    - [Query Structure](#uniqueql-query-structure)
    - [Metadata Filtering](#metadata-filtering)
 7. [Util functions](#utils)
    - [Chat History](#chat-history)
    - [File Io](#file-io)
    - [Sources](#sources)
@@ -503,19 +504,55 @@
     user_id,
     company_id,
     prompt="Was ist der Sinn des Lebens, des Universums und des ganzen Rests?",
     chat_id=chat_id
 )
 ```
 
+### Short Term Memory
+
+For saving data in between chats there is the Short Term Memory functionality to save small data in between rounds of chat e.g. language, search results and so on.
+For this 10k chars can be used. You can save a short term memory for a chat `chatId` or for a message `messageId`.
+you need to provide an `memoryName` as an identifier.
+
+you can then save it and retreive it live defined below.
+
+#### `unique_sdk.ShortTermMemory.create`
+
+```python
+c = unique_sdk.ShortTermMemory.create(
+    user_id,
+    company_id,
+    data="hello",
+    chatId="chat_x0xxtj89f7drjp4vmued3q",
+    # messageId = "msg_id",
+    memoryName="your memory name",
+)
+print(c)
+```
+
+#### `unique_sdk.ShortTermMemory.find-latest`
+
+```python
+m = unique_sdk.ShortTermMemory.find_latest(
+    user_id,
+    company_id,
+    chatId="chat_x0xxtj89f7drjp4vmued3q",
+     # messageId = "msg_id",
+    memoryName="your memory name",
+)
+print(m)
+```
+
 ## UniqueQL
 
 [UniqueQL](https://unique-ch.atlassian.net/wiki/x/coAXHQ) is an advanced query language designed to enhance search capabilities within various search modes such as Vector, Full-Text Search (FTS), and Combined. This query language enables users to perform detailed searches by filtering through metadata attributes like filenames, URLs, dates, and more. UniqueQL is versatile and can be translated into different query formats for various database systems, including PostgreSQL and Qdrant.
 
 ### UniqueQL Query Structure
+
 A UniqueQL query is composed of a path, an operator, and a value. The path specifies the metadata attribute to be filtered, the operator defines the type of comparison, and the value provides the criteria for the filter.
 
 A metadata filter can be designed with UniqueQL's `UQLOperator` and `UQLCombinator` as follows:
 
 ```python
 metadata_filter = {
         "path": ['diet', '*'],
@@ -542,15 +579,14 @@
                     "value": true,
                 },
             ],
         },
     }
 ```
 
-
 ### Metadata Filtering
 
 A metadata filter such as the one designed above can be used in a `Search.create` call by passing it the `metaDataFilter` parameter.
 
 ```python
     search_results = unique_sdk.Search.create(
         user_id=user_id,
@@ -559,15 +595,14 @@
         searchString=search_string,
         searchType="COMBINED",
         # limit=2,
         metaDataFilter=metadata_filter,
     )
 ```
 
-
 ## Utils
 
 ### Chat History
 
 #### `unique_sdk.util.chat_history.load_history`
 
 A helper function that makes sure the chat history is fully loaded and cut to the size of the token window that it fits into the next round of chat interactions.
```

### Comparing `unique_sdk-0.8.2/pyproject.toml` & `unique_sdk-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unique-sdk"
-version = "0.8.2"
+version = "0.8.3"
 description = ""
 authors = [
     "Konstantin Krauss <konstantin@unique.ch>",
     "Andreas Hauri <andreas@unique.ch>",
 ]
 readme = "README.md"
 license = "MIT"
```

### Comparing `unique_sdk-0.8.2/unique_sdk/__init__.py` & `unique_sdk-0.8.3/unique_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/_api_requestor.py` & `unique_sdk-0.8.3/unique_sdk/_api_requestor.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/_api_resource.py` & `unique_sdk-0.8.3/unique_sdk/_api_resource.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/_error.py` & `unique_sdk-0.8.3/unique_sdk/_error.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/_http_client.py` & `unique_sdk-0.8.3/unique_sdk/_http_client.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/_list_object.py` & `unique_sdk-0.8.3/unique_sdk/_list_object.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/_unique_object.py` & `unique_sdk-0.8.3/unique_sdk/_unique_object.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/_unique_ql.py` & `unique_sdk-0.8.3/unique_sdk/_unique_ql.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/_unique_response.py` & `unique_sdk-0.8.3/unique_sdk/_unique_response.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/_util.py` & `unique_sdk-0.8.3/unique_sdk/_util.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/_webhook.py` & `unique_sdk-0.8.3/unique_sdk/_webhook.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/api_resources/_chat_completion.py` & `unique_sdk-0.8.3/unique_sdk/api_resources/_chat_completion.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/api_resources/_content.py` & `unique_sdk-0.8.3/unique_sdk/api_resources/_content.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/api_resources/_integrated.py` & `unique_sdk-0.8.3/unique_sdk/api_resources/_integrated.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/api_resources/_message.py` & `unique_sdk-0.8.3/unique_sdk/api_resources/_message.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/api_resources/_search.py` & `unique_sdk-0.8.3/unique_sdk/api_resources/_search.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/api_resources/_search_string.py` & `unique_sdk-0.8.3/unique_sdk/api_resources/_search_string.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/utils/chat_history.py` & `unique_sdk-0.8.3/unique_sdk/utils/chat_history.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/utils/file_io.py` & `unique_sdk-0.8.3/unique_sdk/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/utils/sources.py` & `unique_sdk-0.8.3/unique_sdk/utils/sources.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/unique_sdk/utils/token.py` & `unique_sdk-0.8.3/unique_sdk/utils/token.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.2/PKG-INFO` & `unique_sdk-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unique-sdk
-Version: 0.8.2
+Version: 0.8.3
 Summary: 
 License: MIT
 Author: Konstantin Krauss
 Author-email: konstantin@unique.ch
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,14 +27,15 @@
 4. [Webhook Triggers](#webhook-triggers)
 5. [Available API Resources](#available-api-resources)
    - [Content](#content)
    - [Message](#message)
    - [Chat Completion](#chat-completion)
    - [Search](#search)
    - [Search String](#search-string)
+   - [Short Term Memory](#short-term-memory)
 6. [UniqueQL](#uniqueql)
    - [Query Structure](#uniqueql-query-structure)
    - [Metadata Filtering](#metadata-filtering)
 7. [Util functions](#utils)
    - [Chat History](#chat-history)
    - [File Io](#file-io)
    - [Sources](#sources)
@@ -518,19 +519,55 @@
     user_id,
     company_id,
     prompt="Was ist der Sinn des Lebens, des Universums und des ganzen Rests?",
     chat_id=chat_id
 )
 ```
 
+### Short Term Memory
+
+For saving data in between chats there is the Short Term Memory functionality to save small data in between rounds of chat e.g. language, search results and so on.
+For this 10k chars can be used. You can save a short term memory for a chat `chatId` or for a message `messageId`.
+you need to provide an `memoryName` as an identifier.
+
+you can then save it and retreive it live defined below.
+
+#### `unique_sdk.ShortTermMemory.create`
+
+```python
+c = unique_sdk.ShortTermMemory.create(
+    user_id,
+    company_id,
+    data="hello",
+    chatId="chat_x0xxtj89f7drjp4vmued3q",
+    # messageId = "msg_id",
+    memoryName="your memory name",
+)
+print(c)
+```
+
+#### `unique_sdk.ShortTermMemory.find-latest`
+
+```python
+m = unique_sdk.ShortTermMemory.find_latest(
+    user_id,
+    company_id,
+    chatId="chat_x0xxtj89f7drjp4vmued3q",
+     # messageId = "msg_id",
+    memoryName="your memory name",
+)
+print(m)
+```
+
 ## UniqueQL
 
 [UniqueQL](https://unique-ch.atlassian.net/wiki/x/coAXHQ) is an advanced query language designed to enhance search capabilities within various search modes such as Vector, Full-Text Search (FTS), and Combined. This query language enables users to perform detailed searches by filtering through metadata attributes like filenames, URLs, dates, and more. UniqueQL is versatile and can be translated into different query formats for various database systems, including PostgreSQL and Qdrant.
 
 ### UniqueQL Query Structure
+
 A UniqueQL query is composed of a path, an operator, and a value. The path specifies the metadata attribute to be filtered, the operator defines the type of comparison, and the value provides the criteria for the filter.
 
 A metadata filter can be designed with UniqueQL's `UQLOperator` and `UQLCombinator` as follows:
 
 ```python
 metadata_filter = {
         "path": ['diet', '*'],
@@ -557,15 +594,14 @@
                     "value": true,
                 },
             ],
         },
     }
 ```
 
-
 ### Metadata Filtering
 
 A metadata filter such as the one designed above can be used in a `Search.create` call by passing it the `metaDataFilter` parameter.
 
 ```python
     search_results = unique_sdk.Search.create(
         user_id=user_id,
@@ -574,15 +610,14 @@
         searchString=search_string,
         searchType="COMBINED",
         # limit=2,
         metaDataFilter=metadata_filter,
     )
 ```
 
-
 ## Utils
 
 ### Chat History
 
 #### `unique_sdk.util.chat_history.load_history`
 
 A helper function that makes sure the chat history is fully loaded and cut to the size of the token window that it fits into the next round of chat interactions.
```

