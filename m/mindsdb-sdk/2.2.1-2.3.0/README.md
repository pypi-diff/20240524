# Comparing `tmp/mindsdb_sdk-2.2.1.tar.gz` & `tmp/mindsdb_sdk-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mindsdb_sdk-2.2.1.tar", last modified: Tue Apr 23 18:25:28 2024, max compression
+gzip compressed data, was "dist/mindsdb_sdk-2.3.0.tar", last modified: Fri May 24 18:06:25 2024, max compression
```

## Comparing `mindsdb_sdk-2.2.1.tar` & `mindsdb_sdk-2.3.0.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/
--rwxr-xr-x   0 runner    (1001) docker     (127)      407 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/connect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/connectors/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/knowledge_bases.py
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/ml_engines.py
--rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/skills.py
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/utils/objects_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/utils/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/mindsdb_sdk/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:25:28.000000 mindsdb_sdk-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-23 18:25:15.000000 mindsdb_sdk-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      407 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/connectors/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10086 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/knowledge_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/ml_engines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20288 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/skills.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/utils/objects_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/utils/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/utils/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/utils/table_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/mindsdb_sdk/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/mindsdb_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/mindsdb_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/mindsdb_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/mindsdb_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/mindsdb_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/mindsdb_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:06:25.000000 mindsdb_sdk-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-24 18:06:15.000000 mindsdb_sdk-2.3.0/setup.py
```

### Comparing `mindsdb_sdk-2.2.1/PKG-INFO` & `mindsdb_sdk-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindsdb_sdk
-Version: 2.2.1
+Version: 2.3.0
 Summary: MindsDB Python SDK, provides an SDK to use a remote mindsdb instance
 Home-page: https://github.com/mindsdb/mindsdb_python_sdk
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb-sdk/
 Description: # Python MindsDB SDK
```

### Comparing `mindsdb_sdk-2.2.1/README.md` & `mindsdb_sdk-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/connect.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/connect.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 
 from mindsdb_sdk.connectors.rest_api import RestAPI
 
 DEFAULT_LOCAL_API_URL = 'http://127.0.0.1:47334'
 DEFAULT_CLOUD_API_URL = 'https://cloud.mindsdb.com'
 
 
-def connect(url: str = None, login: str = None, password: str = None, is_managed: bool = False, headers=None) -> Server:
+def connect(
+        url: str = None,
+        login: str = None,
+        password: str = None,
+        api_key: str = None,
+        is_managed: bool = False,
+        headers=None) -> Server:
     """
     Create connection to mindsdb server
 
     :param url: url to mindsdb server
     :param login: user login, for cloud version it contents email
     :param password: user password to login (for cloud version)
+    :param api_key: API key to authenticate (for cloud version)
     :param is_managed: whether or not the URL points to a managed instance
     :param headers: addtional headers to send with the connection, optional
     :return: Server object
 
     Examples
     --------
 
@@ -25,26 +32,25 @@
     Connect to local server
 
     >>> con = mindsdb_sdk.connect()
     >>> con = mindsdb_sdk.connect('http://127.0.0.1:47334')
 
     Connect to cloud server
 
-    >>> con = mindsdb_sdk.connect(login='a@b.com', password='-')
-    >>> con = mindsdb_sdk.connect('https://cloud.mindsdb.com', login='a@b.com', password='-')
+    >>> con = mindsdb_sdk.connect('https://cloud.mindsdb.com', api_key='-')
 
     Connect to MindsDB pro
 
     >>> con = mindsdb_sdk.connect('http://<YOUR_INSTANCE_IP>', login='a@b.com', password='-', is_managed=True)
 
     """
     if url is None:
         if login is not None:
             # default is cloud
             url = DEFAULT_CLOUD_API_URL
         else:
             # is local
             url = DEFAULT_LOCAL_API_URL
 
-    api = RestAPI(url, login, password, is_managed, headers=headers)
+    api = RestAPI(url, login, password, api_key, is_managed, headers=headers)
 
     return Server(api)
```

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/connectors/rest_api.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/connectors/rest_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import wraps
-from typing import List
+from typing import List, Union
 import io
 
 import requests
 import pandas as pd
 
-from .. import __about__
+from mindsdb_sdk import __about__
 
 
 def _try_relogin(fnc):
     @wraps(fnc)
     def wrapper(self, *args, **kwargs):
         try:
             return fnc(self, *args, **kwargs)
@@ -30,27 +30,30 @@
 def _raise_for_status(response):
     # show response text in error
     if 400 <= response.status_code < 600:
         raise requests.HTTPError(f'{response.reason}: {response.text}', response=response)
 
 
 class RestAPI:
-    def __init__(self, url=None, login=None, password=None, is_managed=False, headers=None):
+    def __init__(self, url=None, login=None, password=None, api_key=None, is_managed=False, headers=None):
 
         self.url = url
         self.username = login
         self.password = password
+        self.api_key = api_key
         self.is_managed = is_managed
         self.session = requests.Session()
 
         self.session.headers['User-Agent'] = f'python-sdk/{__about__.__version__}'
-
         if headers is not None:
             self.session.headers.update(headers)
-
+        if self.api_key is not None:
+            # Authenticate with API key instead of logging in, if present.
+            self.session.headers['X-Api-Key'] = self.api_key
+            return
         if login is not None:
             self.login()
 
     def login(self):
         managed_endpoint = '/api/login'
         cloud_endpoint = '/cloud/login'
 
@@ -69,15 +72,19 @@
             json = {'password': self.password, 'username': self.username}
             url = self.url + managed_endpoint
             r = self.session.post(url, json=json)
 
         _raise_for_status(r)
 
     @_try_relogin
-    def sql_query(self, sql, database='mindsdb', lowercase_columns=False):
+    def sql_query(self, sql, database=None, lowercase_columns=False):
+
+        if database is None:
+            # it means the database is included in query
+            database = 'mindsdb'
         url = self.url + '/api/sql/query'
         r = self.session.post(url, json={
             'query': sql,
             'context': {'db': database}
         })
         _raise_for_status(r)
 
@@ -120,37 +127,81 @@
     @_try_relogin
     def objects_tree(self, item=''):
         r = self.session.get(self.url + f'/api/tree/{item}')
         _raise_for_status(r)
 
         return pd.DataFrame(r.json())
 
-    @_try_relogin
-    def upload_file(self, name: str, df: pd.DataFrame):
-
-        # convert to file
+    @staticmethod
+    def read_file_as_bytes(file_path: str):
+        """
+        Read and return content of a file in bytes, given its path.
+        :param file_path: Path of the file to read.
+        :return: File content in bytes.
+        """
+        try:
+            with open(file_path, 'rb+') as file:
+                return file.read()
+        except FileNotFoundError:
+            raise Exception(f'File {file_path} does not exist.')
+        except PermissionError:
+            raise Exception(f'Permission denied when reading file {file_path}.')
+        except Exception as e:
+            raise Exception(f'Unknown error occurred when reading file {file_path} - {str(e)}')
+    @staticmethod
+    def read_dataframe_as_csv(data: pd.DataFrame):
+        """
+        Read and return content of a DataFrame as CSV in bytes.
+        :param data: DataFrame to read.
+        :return: DataFrame content as CSV in bytes.
+        """
         fd = io.BytesIO()
-        df.to_csv(fd, index=False)
+        data.to_csv(fd, index=False)
         fd.seek(0)
+        return fd.read()
+
+    def upload_data(self, file_name: str, data: bytes):
+        """
+        Upload binary data to MindsDB.
+        :param file_name: Name of the file.
+        :param data: Binary data to upload.
+        """
+        # remove suffix from file if present
+        name = file_name.split('.')[0]
 
         url = self.url + f'/api/files/{name}'
         r = self.session.put(
             url,
             data={
-                'source': name,
-                'name': name,
-                'source_type': 'file',
+                'original_file_name':file_name,
+                'name':name,
+                'source_type':'file',
             },
             files={
-                'file': fd,
+                'file': (file_name, data)
+
             }
         )
         _raise_for_status(r)
 
     @_try_relogin
+    def upload_file(self, name: str, data: Union[pd.DataFrame, str]):
+        """
+        Upload a file or a DataFrame to MindsDB.
+        :param name: Name of the file or DataFrame.
+        :param data: DataFrame data or file path.
+        """
+        if isinstance(data, pd.DataFrame):
+            data_in_bytes = self.read_dataframe_as_csv(data)
+        else:
+            data_in_bytes = self.read_file_as_bytes(data)
+
+        self.upload_data(name, data_in_bytes)
+
+    @_try_relogin
     def get_file_metadata(self, name: str) -> dict:
         # No endpoint currently to get single file.
         url = self.url + f'/api/files/'
         r = self.session.get(url)
         _raise_for_status(r)
         all_file_metadata = r.json()
         for metadata in all_file_metadata:
@@ -315,7 +366,36 @@
         return r.json()
 
     @_try_relogin
     def delete_skill(self, project: str, name: str):
         url = self.url + f'/api/projects/{project}/skills/{name}'
         r = self.session.delete(url)
         _raise_for_status(r)
+
+    # Knowledge Base operations.
+    @_try_relogin
+    def insert_files_into_knowledge_base(self, project: str, knowledge_base_name: str, file_names: List[str]):
+        r = self.session.put(
+            self.url + f'/api/projects/{project}/knowledge_bases/{knowledge_base_name}',
+            json={
+                'knowledge_base': {
+                    'files': file_names
+                }
+            }
+        )
+        _raise_for_status(r)
+
+        return r.json()
+
+    @_try_relogin
+    def insert_webpages_into_knowledge_base(self, project: str, knowledge_base_name: str, urls: List[str]):
+        r = self.session.put(
+            self.url + f'/api/projects/{project}/knowledge_bases/{knowledge_base_name}',
+            json={
+                'knowledge_base': {
+                    'urls': urls
+                }
+            }
+        )
+        _raise_for_status(r)
+
+        return r.json()
```

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/databases.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/databases.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/handlers.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/jobs.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/projects.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,163 +1,195 @@
-import datetime as dt
-from typing import Union, List
+from typing import  List
 
-import pandas as pd
-
-from mindsdb_sql.parser.dialects.mindsdb import CreateJob, DropJob
-from mindsdb_sql.parser.ast import Identifier, Star, Select
+from mindsdb_sql.parser.dialects.mindsdb import CreateDatabase
+from mindsdb_sql.parser.ast import DropDatabase
+from mindsdb_sql.parser.ast import Identifier, Delete
 
 from mindsdb_sdk.utils.sql import dict_to_binary_op
+
+from mindsdb_sdk.agents import Agents
+from mindsdb_sdk.databases import Databases
+from mindsdb_sdk.ml_engines import MLEngines
+from mindsdb_sdk.skills import Skills
 from mindsdb_sdk.utils.objects_collection import CollectionBase
 
+from .models import Models
+from .query import Query
+from .views import Views
+from .jobs import Jobs
+from .knowledge_bases import KnowledgeBases
+
+
+class Project:
+    """
+    Allows to work with project: to manage models and views inside of it or call raw queries inside of project
+
+    Server instance allows to manipulate project and databases (integration) on mindsdb server
+
+    Attributes for accessing to different objects:
+        - models, see :func:`~mindsdb_sdk.models.Models`
+        - views, see :func:`~mindsdb_sdk.views.Views`
+        - jobs, see :func:`~mindsdb_sdk.jobs.Jobs`
+
+    It is possible to cal queries from project context:
+
+    Making prediciton using sql:
+
+    >>> query = project.query('select * from database.table join model1')
+    >>> df = query.fetch()
+
+    Making time series prediction:
+
+    >>> df = project.query('''
+    ...      SELECT m.saledate as date, m.ma as forecast
+    ...     FROM mindsdb.house_sales_model as m
+    ...     JOIN example_db.demo_data.house_sales as t
+    ...     WHERE t.saledate > LATEST AND t.type = 'house'
+    ...     AND t.bedrooms=2
+    ...     LIMIT 4;
+    ...    ''').fetch()
+
+    """
+
+    def __init__(self, api, name, agents: Agents = None, skills: Skills = None, knowledge_bases: KnowledgeBases = None, databases: Databases = None, ml_engines: MLEngines = None):
+        self.name = name
+        self.api = api
+
+        self.models = Models(self, api)
+
+        # old api
+        self.get_model = self.models.get
+        self.list_models = self.models.list
+        self.create_model = self.models.create
+        self.drop_model = self.models.drop
+
+        self.views = Views(self, api)
+
+        # old api
+        self.get_view = self.views.get
+        self.list_views = self.views.list
+        self.create_view = self.views.create
+        self.drop_view = self.views.drop
+
+        self.jobs = Jobs(self, api)
+
+        # old api
+        self.get_job = self.jobs.get
+        self.list_jobs = self.jobs.list
+        self.create_job = self.jobs.create
+        self.drop_job = self.jobs.drop
+
+        self.databases = databases or Databases(api)
+        self.knowledge_bases = knowledge_bases or KnowledgeBases(self, api)
 
-class Job:
-    def __init__(self, project, data):
-        self.project = project
-        self.data = data
-        self._update(data)
-
-    def _update(self, data):
-        self.name = data['name']
-        self.query_str = data['query']
-        self.start_at = data['start_at']
-        self.end_at = data['end_at']
-        self.next_run_at = data['next_run_at']
-        self.schedule_str = data['schedule_str']
+        self.skills = skills or Skills(api, name)
+        self.agents = agents or Agents(api, name, self.knowledge_bases, self.databases, self.models, ml_engines, self.skills)
 
     def __repr__(self):
-        return f"{self.__class__.__name__}({self.name}, query='{self.query_str}')"
+        return f'{self.__class__.__name__}({self.name})'
 
-    def refresh(self):
+    def query(self, sql: str) -> Query:
         """
-        Retrieve job data from mindsdb server
+        Execute raw query inside of project
+
+        :param sql: sql query
+        :return: Query object
         """
-        job = self.project.get_job(self.name)
-        self._update(job.data)
+        return Query(self.api, sql, database=self.name)
+
 
-    def get_history(self) -> pd.DataFrame:
+    def drop_model_version(self, name: str, version: int):
         """
-        Get history of job execution
+        Drop version of the model
 
-        :return: dataframe with job executions
+        :param name: name of the model
+        :param version: version to drop
         """
-        ast_query = Select(
-            targets=[Star()],
-            from_table=Identifier('jobs_history'),
+        ast_query = Delete(
+            table=Identifier('models_versions'),
             where=dict_to_binary_op({
-                'name': self.name
+                'name': name,
+                'version': version
             })
         )
-        return self.project.api.sql_query(ast_query.to_string(), database=self.project.name)
+        self.query(ast_query.to_string()).fetch()
 
 
-class Jobs(CollectionBase):
-    def __init__(self, project, api):
-        self.project = project
-        self.api = api
 
-    def _list(self, name: str = None) -> List[Job]:
+class Projects(CollectionBase):
+    """
+    Projects
+    ----------
 
-        ast_query = Select(targets=[Star()], from_table=Identifier('jobs'))
+    list of projects
 
-        if name is not None:
-            ast_query.where = dict_to_binary_op({'name': name})
+    >>> projects.list()
 
-        df = self.api.sql_query(ast_query.to_string(), database=self.project.name)
+    create
 
-        # columns to lower case
-        cols_map = {i: i.lower() for i in df.columns}
-        df = df.rename(columns=cols_map)
+    >>> project = projects.create('proj')
 
-        return [
-            Job(self.project, item)
-            for item in df.to_dict('records')
-        ]
+    drop
 
-    def list(self) -> List[Job]:
-        """
-        Show list of jobs in project
+    >>> projects.drop('proj')
 
-        :return: list of Job objects
-        """
+    get existing
 
-        return self._list()
+    >>> projects.get('proj')
 
-    def get(self, name: str) -> Job:
-        """
-        Get job by name from project
+    by attribute
+    >>> projects.proj
 
-        :param name: name of the job
-        :return: Job object
-        """
+    """
+
+    def __init__(self, api):
+        self.api = api
 
-        jobs = self._list(name)
-        if len(jobs) == 1:
-            return jobs[0]
-        elif len(jobs) == 0:
-            raise AttributeError("Job doesn't exist")
-        else:
-            raise RuntimeError("Several jobs with the same name")
+    def _list_projects(self):
+        data = self.api.sql_query("select NAME from information_schema.databases where TYPE='project'")
+        return list(data.NAME)
 
-    def create(
-            self,
-            name: str,
-            query_str: str,
-            start_at: dt.datetime = None,
-            end_at: dt.datetime = None,
-            repeat_str: str = None,
-            repeat_min: int = None,
-        ) -> Union[Job, None]:
+    def list(self) -> List[Project]:
         """
-        Create new job in project and return it.
-
-        If it is not possible (job executed and not accessible anymore):
-           return None
+        Show list of project on server
 
-        More info: https://docs.mindsdb.com/sql/create/jobs
+        :return: list of Project objects
+        """
+        # select * from information_schema.databases where TYPE='project'
+        return [Project(self.api, name) for name in self._list_projects()]
 
-        :param name: name of the job
-        :param query_str: str, job's query (or list of queries with ';' delimiter) which job have to execute
-        :param start_at: datetime, first start of job,
-        :param end_at: datetime, when job have to be stopped,
-        :param repeat_str: str, optional, how to repeat job (e.g. '1 hour', '2 weeks', '3 min')
-        :param repeat_min: int, optional, period to repeat the job in minutes
-        :return: Job object or None
+    def get(self, name: str = 'mindsdb') -> Project:
         """
+        Get Project by name
 
-        if start_at is not None:
-            start_str = start_at.strftime("%Y-%m-%d %H:%M:%S")
-        else:
-            start_str = None
+        :param name: name of project
+        :return: Project object
+        """
+        if name not in self._list_projects():
+            raise AttributeError("Project doesn't exist")
+        return Project(self.api, name)
 
-        if end_at is not None:
-            end_str = end_at.strftime("%Y-%m-%d %H:%M:%S")
-        else:
-            end_str = None
+    def create(self, name: str) -> Project:
+        """
+        Create new project and return it
 
-        if repeat_min is not None:
-            repeat_str = f'{repeat_min} minutes'
+        :param name: name of the project
+        :return: Project object
+        """
 
-        ast_query = CreateJob(
+        ast_query = CreateDatabase(
             name=Identifier(name),
-            query_str=query_str,
-            start_str=start_str,
-            end_str=end_str,
-            repeat_str=repeat_str
+            engine='mindsdb',
+            parameters={}
         )
 
-        self.api.sql_query(ast_query.to_string(), database=self.project.name)
-
-        # job can be executed and remove it is not repeatable
-        jobs = self._list(name)
-        if len(jobs) == 1:
-            return jobs[0]
+        self.api.sql_query(ast_query.to_string())
+        return Project(self.api, name)
 
     def drop(self, name: str):
         """
-        Drop job from project
+        Drop project from server
 
-        :param name: name of the job
+        :param name: name of the project
         """
-        ast_query = DropJob(Identifier(name))
-
-        self.api.sql_query(ast_query.to_string(), database=self.project.name)
+        ast_query = DropDatabase(name=Identifier(name))
+        self.api.sql_query(ast_query.to_string())
```

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/knowledge_bases.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/knowledge_bases.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from typing import Union, List
 
 import pandas as pd
 
 from mindsdb_sql.parser.dialects.mindsdb import CreateKnowledgeBase, DropKnowledgeBase
 from mindsdb_sql.parser.ast import Identifier, Star, Select, BinaryOperation, Constant, Insert
 
-from mindsdb_sdk.utils.sql import dict_to_binary_op
+from mindsdb_sdk.utils.sql import dict_to_binary_op, query_to_native_query
 from mindsdb_sdk.utils.objects_collection import CollectionBase
+from mindsdb_sdk.utils.context import is_saving
 
 from .models import Model
 from .tables import Table
 from .query import Query
 from .databases import Database
 
 
@@ -27,18 +28,19 @@
 
     Query relevant results
 
     >>> df = kb.find('flats').fetch()
 
     """
 
-    def __init__(self, project, data: dict):
-
+    def __init__(self, api, project, data: dict):
+        self.api = api
         self.project = project
         self.name = data['name']
+        self.table_name = Identifier(parts=[self.project.name, self.name])
 
         self.storage = None
         if data['storage'] is not None:
             # if name contents '.' there could be errors
 
             parts = data['storage'].split('.')
             if len(parts) == 2:
@@ -65,18 +67,18 @@
 
         self.params = params
 
         # query behavior
         self._query = None
         self._limit = None
 
-        database = project.name
         self._update_query()
 
-        super().__init__(project.api, self.sql, database)
+        # empty database
+        super().__init__(project.api, self.sql, None)
 
     def __repr__(self):
         return f'{self.__class__.__name__}({self.project.name}.{self.name})'
 
     def find(self, query: str, limit: int = 100):
         """
 
@@ -100,28 +102,38 @@
 
         return kb
 
     def _update_query(self):
 
         ast_query = Select(
             targets=[Star()],
-            from_table=Identifier(parts=[
-                self.project.name, self.name
-            ])
+            from_table=self.table_name
         )
         if self._query is not None:
             ast_query.where = BinaryOperation(op='=', args=[
                 Identifier('content'),
                 Constant(self._query)
             ])
 
         if self._limit is not None:
             ast_query.limit = Constant(self._limit)
         self.sql = ast_query.to_string()
 
+    def insert_files(self, file_paths: List[str]):
+        """
+        Insert data from file to knowledge base
+        """
+        self.api.insert_files_into_knowledge_base(self.project.name, self.name, file_paths)
+
+    def insert_webpages(self, urls: List[str]):
+        """
+        Insert data from crawled URLs to knowledge base
+        """
+        self.api.insert_webpages_into_knowledge_base(self.project.name, self.name, urls)
+
     def insert(self, data: Union[pd.DataFrame, Query, dict]):
         """
         Insert data to knowledge base
 
         >>> # insert using query
         >>> my_kb.insert(server.databases.example_db.tables.houses_sales.filter(type='house'))
         >>> # using dataframe
@@ -139,28 +151,36 @@
             data = pd.DataFrame([data])
 
         if isinstance(data, pd.DataFrame):
             # insert data
             data_split = data.to_dict('split')
 
             ast_query = Insert(
-                table=Identifier(self.name),
+                table=Identifier(self.table_name),
                 columns=data_split['columns'],
                 values=data_split['data']
             )
-
             sql = ast_query.to_string()
-            self.api.sql_query(sql, self.database)
+
         else:
             # insert from select
-            table = Identifier(parts=[self.database, self.name])
-            self.api.sql_query(
-                f'INSERT INTO {table.to_string()} ({data.sql})',
-                database=data.database
-            )
+            if data.database is not None:
+                ast_query = Insert(
+                    table=Identifier(self.table_name),
+                    from_select=query_to_native_query(data)
+                )
+                sql = ast_query.to_string()
+            else:
+                sql = f'INSERT INTO {self.table_name.to_string()} ({data.sql})'
+
+        if is_saving():
+            # don't execute it right now, return query object
+            return Query(self, sql, self.database)
+
+        self.api.sql_query(sql, self.database)
 
 
 class KnowledgeBases(CollectionBase):
     """
     **Knowledge bases**
 
     Get list:
@@ -198,15 +218,15 @@
         df = self.api.sql_query(ast_query.to_string(), database=self.project.name)
 
         # columns to lower case
         cols_map = {i: i.lower() for i in df.columns}
         df = df.rename(columns=cols_map)
 
         return [
-            KnowledgeBase(self.project, item)
+            KnowledgeBase(self.api, self.project, item)
             for item in df.to_dict('records')
         ]
 
     def list(self) -> List[KnowledgeBase]:
         """
 
         Get list of knowledge bases inside of project:
@@ -237,15 +257,15 @@
         name: str,
         model: Model = None,
         storage: Table = None,
         metadata_columns: list = None,
         content_columns: list = None,
         id_column: str = None,
         params: dict = None,
-    ) -> KnowledgeBase:
+    ) -> Union[KnowledgeBase, Query]:
         """
 
         Create knowledge base:
 
         >>> kb = server.knowledge_bases.create(
         ...   'my_kb',
         ...   model=server.models.emb_model,
@@ -287,27 +307,35 @@
 
         if storage is not None:
             storage_name = Identifier(parts=[storage.db.name, storage.name])
         else:
             storage_name = None
 
         ast_query = CreateKnowledgeBase(
-            Identifier(name),
+            Identifier(parts=[self.project.name, name]),
             model=model_name,
             storage=storage_name,
             params=params_out
         )
+        sql = ast_query.to_string()
+
+        if is_saving():
+            return Query(self, sql)
 
-        self.api.sql_query(ast_query.to_string(), database=self.project.name)
+        self.api.sql_query(sql)
 
         return self.get(name)
 
     def drop(self, name: str):
         """
 
         :param name:
         :return:
         """
 
-        ast_query = DropKnowledgeBase(Identifier(name))
+        ast_query = DropKnowledgeBase(Identifier(parts=[self.project.name, name]))
+        sql = ast_query.to_string()
+
+        if is_saving():
+            return Query(self, sql)
 
-        self.api.sql_query(ast_query.to_string())
+        self.api.sql_query(sql)
```

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/ml_engines.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/ml_engines.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/models.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 
 import pandas as pd
 
 from mindsdb_sql.parser.dialects.mindsdb import CreatePredictor, DropPredictor
 from mindsdb_sql.parser.dialects.mindsdb import RetrainPredictor, FinetunePredictor
 from mindsdb_sql.parser.ast import Identifier, Select, Star, Join, Update, Describe, Constant
 from mindsdb_sql import parse_sql
+from mindsdb_sql.exceptions import ParsingException
 
 from .ml_engines import MLEngine
 
 from mindsdb_sdk.utils.objects_collection import CollectionBase
-from mindsdb_sdk.utils.sql import dict_to_binary_op
+from mindsdb_sdk.utils.sql import dict_to_binary_op, query_to_native_query
+from mindsdb_sdk.utils.context import is_saving
 
 from .query import Query
 
 
 class Model:
     """
 
@@ -101,23 +103,23 @@
         self.name = data['name']
         self.version = None
 
     def __repr__(self):
         version = ''
         if self.version is not None:
             version = f', version={self.version}'
-        return f'{self.__class__.__name__}({self.name}{version}, status={self.data["status"]})'
+        return f'{self.__class__.__name__}({self.name}{version}, status={self.data.get("status")})'
 
     def _get_identifier(self):
         parts = [self.project.name, self.name]
         if self.version is not None:
             parts.append(str(self.version))
         return Identifier(parts=parts)
 
-    def predict(self, data: Union[pd.DataFrame, Query, dict], params: dict = None) -> pd.DataFrame:
+    def predict(self, data: Union[pd.DataFrame, Query, dict], params: dict = None) -> Union[pd.DataFrame, Query]:
         """
         Make prediction using model
 
         if data is dataframe
           it uses /model/predict http method and sends dataframe over it
 
         if data is select query with one table
@@ -126,17 +128,21 @@
         if data is select from join other complex query it modifies query to:
           'select from (input query) join model' and sends it over sql/query http method
 
         :param data: dataframe or Query object as input to predictor
         :param params: parameters for predictor, optional
         :return: dataframe with result of prediction
         """
+
         if isinstance(data, Query):
             # create join from select if it is simple select
-            ast_query = parse_sql(data.sql, dialect='mindsdb')
+            try:
+                ast_query = parse_sql(data.sql, dialect='mindsdb')
+            except ParsingException:
+                ast_query = None
 
             # injection of join disabled yet
             # if isinstance(ast_query, Select) and isinstance(ast_query.from_table, Identifier):
             #     # inject aliases
             #     if ast_query.from_table.alias is None:
             #         alias = 't'
             #         ast_query.from_table.alias = Identifier(alias)
@@ -161,32 +167,53 @@
             #         right=model_identifier
             #     )
             #
             #     # select only model columns
             #     ast_query.targets = [Identifier(parts=['m', Star()])]
             #
 
-            # wrap query to subselect
             model_identifier = self._get_identifier()
             model_identifier.alias = Identifier('m')
 
-            ast_query.parentheses = True
-            ast_query.alias = Identifier('t')
-            upper_query = Select(
-                targets=[Identifier(parts=['m', Star()])],
-                from_table=Join(
-                    join_type='join',
-                    left=ast_query,
-                    right=model_identifier
+            if data.database is not None or ast_query is None or not isinstance(ast_query, Select):
+                # use native query
+                native_query = query_to_native_query(data)
+                native_query.parentheses = True
+                native_query.alias = Identifier('t')
+                upper_query = Select(
+                    targets=[Identifier(parts=['m', Star()])],
+                    from_table=Join(
+                        join_type='join',
+                        left=native_query,
+                        right=model_identifier
+                    )
+                )
+            else:
+                # wrap query to subselect
+                model_identifier = self._get_identifier()
+                model_identifier.alias = Identifier('m')
+
+                ast_query.parentheses = True
+                ast_query.alias = Identifier('t')
+                upper_query = Select(
+                    targets=[Identifier(parts=['m', Star()])],
+                    from_table=Join(
+                        join_type='join',
+                        left=ast_query,
+                        right=model_identifier
+                    )
                 )
-            )
             if params is not None:
                 upper_query.using = params
             # execute in query's database
-            return self.project.api.sql_query(upper_query.to_string(), database=data.database)
+            sql = upper_query.to_string()
+            if is_saving():
+                return Query(self, sql)
+
+            return self.project.api.sql_query(sql, database=None)
 
         elif isinstance(data, dict):
             data = pd.DataFrame([data])
             return self.project.api.model_predict(self.project.name, self.name, data,
                                                   params=params, version=self.version)
         elif isinstance(data, pd.DataFrame):
             return self.project.api.model_predict(self.project.name, self.name, data,
@@ -285,37 +312,46 @@
 
         ast_query = ast_class(
             name=self._get_identifier(),
             query_str=query,
             integration_name=database,
             using=options or None,
         )
+        sql = ast_query.to_string()
+
+        if is_saving():
+            return Query(self, sql)
 
-        data = self.project.query(ast_query.to_string()).fetch()
+        data = self.project.api.sql_query(sql)
         data = {k.lower(): v for k, v in data.items()}
 
         # return new instance
         base_class = self.__class__
         return base_class(self.project, data)
 
-    def describe(self, type: str = None) -> pd.DataFrame:
+    def describe(self, type: str = None) -> Union[pd.DataFrame, Query]:
         """
         Return description of the model
 
         :param type: describe type (for lightwood is models, ensemble, features), optional
         :return: dataframe with result of description
         """
         if self.version is not None:
             raise NotImplementedError
 
         identifier = self._get_identifier()
         if type is not None:
             identifier.parts.append(type)
         ast_query = Describe(identifier)
-        return self.project.query(ast_query.to_string()).fetch()
+
+        sql = ast_query.to_string()
+        if is_saving():
+            return Query(self, sql)
+
+        return self.project.api.sql_query(sql)
 
     def list_versions(self) -> List[ModelVersion]:
         """
         Show list of model versions
 
         :return: list ModelVersion objects
         """
@@ -349,24 +385,28 @@
     def set_active(self, version: int):
         """
         Change model active version
 
         :param version: version to set active
         """
         ast_query = Update(
-            table=Identifier('models_versions'),
+            table=Identifier(parts=[self.project.name, 'models_versions']),
             update_columns={
                 'active': Constant(1)
             },
             where=dict_to_binary_op({
                 'name': self.name,
                 'version': version
             })
         )
-        self.project.query(ast_query.to_string()).fetch()
+        sql = ast_query.to_string()
+        if is_saving():
+            return Query(self, sql)
+
+        self.project.api.sql_query(sql)
         self.refresh()
 
 
 class ModelVersion(Model):
     def __init__(self, project, data):
 
         super().__init__(project, data)
@@ -405,15 +445,15 @@
         name: str,
         predict: str = None,
         engine: Union[str, MLEngine] = None,
         query: Union[str, Query] = None,
         database: str = None,
         options: dict = None,
         timeseries_options: dict = None, **kwargs
-    ) -> Model:
+    ) -> Union[Model, Query]:
         """
         Create new model in project and return it
 
         If query/database is passed, it will be executed on mindsdb side
 
         Create, using params and qeury as string
 
@@ -461,15 +501,15 @@
 
         if predict is not None:
             targets = [Identifier(predict)]
         else:
             targets = None
 
         ast_query = CreatePredictor(
-            name=Identifier(name),
+            name=Identifier(parts=[self.project.name, name]),
             query_str=query,
             integration_name=database,
             targets=targets,
         )
 
         if timeseries_options is not None:
             # check ts options
@@ -497,15 +537,21 @@
 
         if engine is not None:
             if isinstance(engine, MLEngine):
                 engine = engine.name
 
             options['engine'] = engine
         ast_query.using = options
-        df = self.project.query(ast_query.to_string()).fetch()
+
+        sql = ast_query.to_string()
+
+        if is_saving():
+            return Query(self, sql)
+
+        df = self.project.api.sql_query(sql)
         if len(df) > 0:
             data = dict(df.iloc[0])
             # to lowercase
             data = {k.lower(): v for k,v in data.items()}
 
             return Model(self.project, data)
 
@@ -534,16 +580,20 @@
         """
         Drop model from project with all versions
 
         >>> models.drop('rentals_model')
 
         :param name: name of the model
         """
-        ast_query = DropPredictor(name=Identifier(name))
-        self.project.query(ast_query.to_string()).fetch()
+        ast_query = DropPredictor(name=Identifier(parts=[self.project.name, name]))
+        sql = ast_query.to_string()
+        if is_saving():
+            return Query(self, sql)
+
+        self.project.api.sql_query(sql)
 
 
     def list(self, with_versions: bool = False,
                     name: str = None,
                     version: int = None) -> List[Union[Model, ModelVersion]]:
         """
         List models (or model versions) in project
```

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/query.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/server.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
     """
 
     def __init__(self, api, skills: Skills = None, agents: Agents = None):
         # server is also mindsdb project
         project_name = 'mindsdb'
         self.databases = Databases(api)
-        super().__init__(api, project_name, skills=skills, agents=agents, databases=self.databases)
+        self.ml_engines = MLEngines(api)
+        super().__init__(api, project_name, skills=skills, agents=agents, databases=self.databases, ml_engines=self.ml_engines)
 
         self.projects = Projects(api)
 
         # old api
         self.get_project = self.projects.get
         self.list_projects = self.projects.list
         self.create_project = self.projects.create
@@ -42,15 +43,14 @@
 
         # old api
         self.get_database = self.databases.get
         self.list_databases = self.databases.list
         self.create_database = self.databases.create
         self.drop_database = self.databases.drop
 
-        self.ml_engines = MLEngines(self.api)
 
         self.ml_handlers = Handlers(self.api, 'ml')
         self.data_handlers = Handlers(self.api, 'data')
 
     def status(self) -> dict:
         """
         Get server information. It could content version
```

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/skills.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/skills.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     List all skills:
 
     >>> skills = skills.list()
 
     Create a new SQL skill:
 
-    >>> text_to_sql_skill = skills.create('text_to_sql', 'sql', { 'tables': ['my_table'], 'database': 'my_database' })
+    >>> text_to_sql_skill = skills.create('text_to_sql', 'sql', { 'tables': ['my_table'], 'database': 'my_database', 'description': 'my_description'})
 
     Update a skill:
 
     >>> skill.params = { 'tables': ['new_table'], 'database': 'new_database' }
     >>> updated_skill = skills.update('my_skill', skill)
 
     Delete a skill by name
@@ -46,38 +46,42 @@
         return self.params == other.params
 
     def __repr__(self):
         return f'{self.__class__.__name__}(name: {self.name})'
 
     @classmethod
     def from_json(cls, json: dict):
+        name = json['name']
+        type = json['type']
+        params = json['params']
         if json['type'] == 'sql':
-            return SQLSkill(json['name'], json['params']['tables'], json['params']['database'])
+            return SQLSkill(name, params['tables'], params['database'], params.get('description', ''))
         if json['type'] == 'retrieval':
-            return RetrievalSkill(json['name'], json['params']['knowledge_base'], json['params']['description'])
-        return Skill(json['name'], json['type'], json['params'])
+            return RetrievalSkill(name, params['source'], params.get('description', ''))
+        return Skill(name, type, params)
 
 
 class SQLSkill(Skill):
     """Represents a MindsDB skill for agents to interact with MindsDB databases"""
-    def __init__(self, name: str, tables: List[str], database: str):
+    def __init__(self, name: str, tables: List[str], database: str, description: str):
         params = {
             'database': database,
             'tables': tables,
+            'description': description
         }
         super().__init__(name, 'sql', params)
 
 class RetrievalSkill(Skill):
     """Represents a MindsDB skill for agents to interact with MindsDB data sources"""
     def __init__(self, name: str, knowledge_base: str, description: str):
         params = {
-            'knowledge_base': knowledge_base,
+            'source': knowledge_base,
             'description': description
         }
-        super().__init__(name, 'knowledge_base', params)
+        super().__init__(name, 'retrieval', params)
 
 
 class Skills(CollectionBase):
     """Collection for skills"""
     def __init__(self, api, project: str):
         self.api = api
         self.project = project
@@ -110,15 +114,15 @@
         :param type: Type of the skill to be created
         :param params: Parameters for the skill to be created
 
         :return: created skill object
         """
         _ = self.api.create_skill(self.project, name, type, params)
         if type == 'sql':
-            return SQLSkill(name, params['tables'], params['database'])
+            return SQLSkill(name, params['tables'], params['database'], params['description'])
         return Skill(name, type, params)
 
     def update(self, name: str, updated_skill: Skill) -> Skill:
         """
         Update a skill by name.
 
         param name: Name of the skill to be updated
```

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/tables.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/tables.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import copy
 from typing import Union
 from typing import List
 
 import pandas as pd
 
-from mindsdb_sql.parser.ast import DropTables
+from mindsdb_sql.parser.ast import DropTables, CreateTable
 from mindsdb_sql.parser.ast import Select, Star, Identifier, Constant, Delete, Insert, Update, Last, BinaryOperation
 
-from mindsdb_sdk.utils.sql import dict_to_binary_op, add_condition
+from mindsdb_sdk.utils.sql import dict_to_binary_op, add_condition, query_to_native_query
 from mindsdb_sdk.utils.objects_collection import CollectionBase
+from mindsdb_sdk.utils.context import is_saving
 
 from .query import Query
 
 
 class Table(Query):
     def __init__(self, db, name):
-        super().__init__(db.api, '', db.name)
+        # empty database
+        super().__init__(db.api, '', None)
         self.name = name
+        self.table_name = Identifier(parts=[db.name, name])
         self.db = db
         self._filters = {}
         self._limit = None
         self._track_column = None
         self._update_query()
 
     def _filters_repr(self):
@@ -33,15 +36,15 @@
             filters = ', ' + filters
         return filters
 
     def __repr__(self):
         limit_str = ''
         if self._limit is not None:
             limit_str = f'; limit={self._limit}'
-        return f'{self.__class__.__name__}({self.name}{self._filters_repr()}{limit_str})'
+        return f'{self.__class__.__name__}({self.table_name}{self._filters_repr()}{limit_str})'
 
     def filter(self, **kwargs):
         """
         Applies filters on table
         table.filter(a=1, b=2) adds where condition to table:
         'select * from table1 where a=1 and b=2'
 
@@ -93,15 +96,15 @@
         where = dict_to_binary_op(self._filters)
         if self._track_column is not None:
             condition = BinaryOperation(op='>', args=[Identifier(self._track_column), Last()])
             where = add_condition(where, condition)
 
         ast_query = Select(
             targets=[Star()],
-            from_table=Identifier(self.name),
+            from_table=self.table_name,
             where=where
         )
         if self._limit is not None:
             ast_query.limit = Constant(self._limit)
         self.sql = ast_query.to_string()
 
     def insert(self, query: Union[pd.DataFrame, Query]):
@@ -112,48 +115,60 @@
         """
 
         if isinstance(query, pd.DataFrame):
             # insert data
             data_split = query.to_dict('split')
 
             ast_query = Insert(
-                table=Identifier(self.name),
+                table=self.table_name,
                 columns=data_split['columns'],
                 values=data_split['data']
             )
 
             sql = ast_query.to_string()
-            self.api.sql_query(sql, self.database)
-        else:
+
+        elif isinstance(query, Query):
             # insert from select
-            table = Identifier(parts=[self.database, self.name])
-            self.api.sql_query(
-                f'INSERT INTO {table.to_string()} ({query.sql})',
-                database=query.database
-            )
+
+            if query.database is not None:
+                # use native query
+                ast_query = Insert(
+                    table=self.table_name,
+                    from_select=query_to_native_query(query)
+                )
+                sql = ast_query.to_string()
+            else:
+                sql = f'INSERT INTO {self.table_name.to_string()} ({query.sql})',
+        else:
+            raise ValueError(f'Invalid query type: {query}')
+
+        if is_saving():
+            return Query(self, sql)
+
+        self.api.sql_query(sql)
 
     def delete(self, **kwargs):
         """
         Deletes record from table using filters
 
         >>> table.delete(a=1, b=2)
 
         :param kwargs: filter
         """
-        identifier = Identifier(self.name)
-        # add database
-        identifier.parts.insert(0, self.database)
 
         ast_query = Delete(
-            table=identifier,
+            table=self.table_name,
             where=dict_to_binary_op(kwargs)
         )
-
         sql = ast_query.to_string()
-        self.api.sql_query(sql, 'mindsdb')
+
+        if is_saving():
+            return Query(self, sql)
+
+        self.api.sql_query(sql)
 
     def update(self, values: Union[dict, Query], on: list = None, filters: dict = None):
         '''
         Update table by condition of from other table.
 
         If 'values' is a dict:
           it will be an update by condition
@@ -173,41 +188,50 @@
 
         if isinstance(values, Query):
             # is update from select
             if on is None:
                 raise ValueError('"on" parameter is required for update from query')
 
             # insert from select
-            table = Identifier(parts=[self.database, self.name])
-            map_cols = ', '.join(on)
-            self.api.sql_query(
-                f'UPDATE {table.to_string()} ON {map_cols} FROM ({values.sql})',
-                database=values.database
-            )
+            if values.database is not None:
+                ast_query = Update(
+                    table=self.table_name,
+                    keys=[Identifier(col) for col in on],
+                    from_select=query_to_native_query(values)
+                )
+                sql = ast_query.to_string()
+            else:
+                map_cols = ', '.join(on)
+                sql = f'UPDATE {self.table_name.to_string()} ON {map_cols} FROM ({values.sql})'
+
         elif isinstance(values, dict):
             # is regular update
             if filters is None:
                 raise ValueError('"filters" parameter is required for update')
 
             update_columns = {
                 k: Constant(v)
                 for k, v in values.items()
             }
 
             ast_query = Update(
-                table=Identifier(self.name),
+                table=self.table_name,
                 update_columns=update_columns,
                 where=dict_to_binary_op(filters)
             )
 
             sql = ast_query.to_string()
-            self.api.sql_query(sql, self.database)
         else:
             raise NotImplementedError
 
+        if is_saving():
+            return Query(self, sql)
+
+        self.api.sql_query(sql)
+
 
 class Tables(CollectionBase):
     """
     Wortking with tables:
     Get table as Query object
 
     >>> table = tables.get('table1')
@@ -265,15 +289,15 @@
 
         :param name: name of table
         :return: Table object
         """
 
         return Table(self.database, name)
 
-    def create(self, name: str, query: Union[pd.DataFrame, Query], replace: bool = False) -> Table:
+    def create(self, name: str, query: Union[pd.DataFrame, Query], replace: bool = False) -> Union[Table, Query]:
         """
         Create new table and return it.
 
         On mindsdb server it executes command:
         `insert into a (select ...)`
 
         or if replace is True
@@ -309,31 +333,46 @@
         #     )
         # )
         # self.query(ast_query.to_string()).fetch()
 
         # call in query database
         table = Identifier(parts=[self.database.name, name])
 
-        replace_str = ''
-        if replace:
-            replace_str = ' or replace'
-
-        self.api.sql_query(
-            f'create{replace_str} table {table.to_string()} ({query.sql})',
-            database=query.database
-        )
+        if query.database is not None:
+            # use native query
+            ast_query = CreateTable(
+                name=table,
+                is_replace=replace,
+                from_select=query_to_native_query(query)
+            )
+            sql = ast_query.to_string()
+        else:
+            replace_str = ''
+            if replace:
+                replace_str = ' or replace'
+
+            sql = f'create{replace_str} table {table.to_string()} ({query.sql})'
+
+        if is_saving():
+            return Query(self, sql)
+
+        self.api.sql_query(sql)
 
         return Table(self.database, name)
 
     def drop(self, name: str):
         """
         Delete table
 
         :param name: name of table
         """
+        table = Identifier(parts=[self.database.name, name])
+
         ast_query = DropTables(
-            tables=[
-                Identifier(parts=[name])
-            ]
+            tables=[table]
         )
-        self.api.sql_query(ast_query.to_string(), database=self.database.name)
+        sql = ast_query.to_string()
+
+        if is_saving():
+            return Query(self, sql)
+        self.api.sql_query(sql)
```

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/utils/objects_collection.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/utils/objects_collection.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk/views.py` & `mindsdb_sdk-2.3.0/mindsdb_sdk/views.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/PKG-INFO` & `mindsdb_sdk-2.3.0/mindsdb_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindsdb-sdk
-Version: 2.2.1
+Version: 2.3.0
 Summary: MindsDB Python SDK, provides an SDK to use a remote mindsdb instance
 Home-page: https://github.com/mindsdb/mindsdb_python_sdk
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb-sdk/
 Description: # Python MindsDB SDK
```

### Comparing `mindsdb_sdk-2.2.1/mindsdb_sdk.egg-info/SOURCES.txt` & `mindsdb_sdk-2.3.0/mindsdb_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,9 +22,12 @@
 mindsdb_sdk.egg-info/SOURCES.txt
 mindsdb_sdk.egg-info/dependency_links.txt
 mindsdb_sdk.egg-info/requires.txt
 mindsdb_sdk.egg-info/top_level.txt
 mindsdb_sdk/connectors/__init__.py
 mindsdb_sdk/connectors/rest_api.py
 mindsdb_sdk/utils/__init__.py
+mindsdb_sdk/utils/context.py
 mindsdb_sdk/utils/objects_collection.py
-mindsdb_sdk/utils/sql.py
+mindsdb_sdk/utils/openai.py
+mindsdb_sdk/utils/sql.py
+mindsdb_sdk/utils/table_schema.py
```

### Comparing `mindsdb_sdk-2.2.1/setup.py` & `mindsdb_sdk-2.3.0/setup.py`

 * *Files identical despite different names*

