# Comparing `tmp/sqlitecloud-0.0.75.tar.gz` & `tmp/sqlitecloud-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlitecloud-0.0.75.tar", last modified: Wed May 22 13:34:25 2024, max compression
+gzip compressed data, was "sqlitecloud-0.0.77.tar", last modified: Fri May 24 18:01:42 2024, max compression
```

## Comparing `sqlitecloud-0.0.75.tar` & `sqlitecloud-0.0.77.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/README-PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/SqliteCloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-22 13:34:25.000000 sqlitecloud-0.0.75/SqliteCloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-22 13:34:25.000000 sqlitecloud-0.0.75/SqliteCloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:34:25.000000 sqlitecloud-0.0.75/SqliteCloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 13:34:25.000000 sqlitecloud-0.0.75/SqliteCloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 13:34:25.000000 sqlitecloud-0.0.75/SqliteCloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-22 13:34:22.000000 sqlitecloud-0.0.75/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/sqlitecloud/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/conn_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    33673 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/resultset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23341 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-24 18:01:39.000000 sqlitecloud-0.0.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/SqliteCloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-24 18:01:42.000000 sqlitecloud-0.0.77/SqliteCloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-24 18:01:42.000000 sqlitecloud-0.0.77/SqliteCloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:01:42.000000 sqlitecloud-0.0.77/SqliteCloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 18:01:42.000000 sqlitecloud-0.0.77/SqliteCloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 18:01:42.000000 sqlitecloud-0.0.77/SqliteCloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-24 18:01:39.000000 sqlitecloud-0.0.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/sqlitecloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33631 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/resultset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/sqlitecloud/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:42.644730 sqlitecloud-0.0.77/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23369 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-24 18:01:36.000000 sqlitecloud-0.0.77/tests/integration/test_upload.py
```

### Comparing `sqlitecloud-0.0.75/PKG-INFO` & `sqlitecloud-0.0.77/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SqliteCloud
-Version: 0.0.75
+Version: 0.0.77
 Summary: A Python package for working with SQLite databases in the cloud.
 Home-page: https://github.com/sqlitecloud/python
 Author: sqlitecloud.io
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,29 +12,41 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Requires-Dist: lz4==3.1.10
+Requires-Dist: lz4>=3.1.10
 
-# Python SDK for SqliteCloud
+# Python SDK for SQLite Cloud
 
-![Build Status](https://github.com/sqlitecloud/python/actions/workflows/deploy.yaml/badge.svg "Build Status") ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=plastic&logo=jupyter&logoColor=white)
+<p align="center">
+  <img src="https://sqlitecloud.io/social/logo.png" height="300" alt="SQLite Cloud logo">
+</p>
 
-SQLiteCloud is a powerful Python package that allows you to interact with the SQLite Cloud backend server seamlessly. It provides methods for various database operations. This package is designed to simplify database operations in Python applications, making it easier than ever to work with SQLite Cloud.
+![Build Status](https://github.com/sqlitecloud/python/actions/workflows/deploy.yaml/badge.svg "Build Status")
+[![codecov](https://codecov.io/github/sqlitecloud/python/graph/badge.svg?token=38G6FGOWKP)](https://codecov.io/github/sqlitecloud/python)
+![PyPI - Version](https://img.shields.io/pypi/v/sqlitecloud?link=https%3A%2F%2Fpypi.org%2Fproject%2FSqliteCloud%2F)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/sqlitecloud?link=https%3A%2F%2Fpypi.org%2Fproject%2FSqliteCloud%2F)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sqlitecloud?link=https%3A%2F%2Fpypi.org%2Fproject%2FSqliteCloud%2F)
 
 
+[SQLiteCloud](https://sqlitecloud.io) is a powerful Python package that allows you to interact with the SQLite Cloud backend server seamlessly. It provides methods for various database operations. This package is designed to simplify database operations in Python applications, making it easier than ever to work with SQLite Cloud.
+
+- Site: [https://sqlitecloud.io](https://sqlitecloud.io/developers)
+- Documentation: https://..._coming!_
+- Source: [https://github.com/sqlitecloud/python](https://github.com/sqlitecloud/python)
+
 ## Installation
 
 You can install SqliteCloud Package using Python Package Index (PYPI):
 
 ```bash
-$ pip install SqliteCloud
+$ pip install sqlitecloud
 ```
 
 ## Usage
 <hr>
 
 ```python
 from sqlitecloud.client import SqliteCloudClient
@@ -50,15 +62,15 @@
 client = SqliteCloudClient(cloud_account=account)
 conn = client.open_connection()
 ```
 
 #### _Using string configuration_
 
 ```python
-account = SqliteCloudAccount("sqlitecloud://user:pass@host.com:port/dbname?timeout=10&key2=value2&key3=value3")
+account = SqliteCloudAccount("sqlitecloud://user:pass@host.com:port/dbname?apikey=myapikey")
 client = SqliteCloudClient(cloud_account=account)
 conn = client.open_connection()
 ```
 
 ### _Execute a query_
 You can bind values to parametric queries: you can pass parameters as positional values in an array
 ```python
@@ -71,12 +83,22 @@
 ### _Iterate result_
 result is an iterable object
 ```python
 for row in result:
     print(row)
 ```
 
+### _Specific value_
+```python
+result.get_value(0, 0)
+```
+
+### _Column name_
+```python
+result.get_name(0)
+```
+
 ### _Close connection_
 
-```python 
+```python
 client.disconnect(conn)
 ```
```

### Comparing `sqlitecloud-0.0.75/SqliteCloud.egg-info/PKG-INFO` & `sqlitecloud-0.0.77/SqliteCloud.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SqliteCloud
-Version: 0.0.75
+Version: 0.0.77
 Summary: A Python package for working with SQLite databases in the cloud.
 Home-page: https://github.com/sqlitecloud/python
 Author: sqlitecloud.io
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,29 +12,41 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Requires-Dist: lz4==3.1.10
+Requires-Dist: lz4>=3.1.10
 
-# Python SDK for SqliteCloud
+# Python SDK for SQLite Cloud
 
-![Build Status](https://github.com/sqlitecloud/python/actions/workflows/deploy.yaml/badge.svg "Build Status") ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=plastic&logo=jupyter&logoColor=white)
+<p align="center">
+  <img src="https://sqlitecloud.io/social/logo.png" height="300" alt="SQLite Cloud logo">
+</p>
 
-SQLiteCloud is a powerful Python package that allows you to interact with the SQLite Cloud backend server seamlessly. It provides methods for various database operations. This package is designed to simplify database operations in Python applications, making it easier than ever to work with SQLite Cloud.
+![Build Status](https://github.com/sqlitecloud/python/actions/workflows/deploy.yaml/badge.svg "Build Status")
+[![codecov](https://codecov.io/github/sqlitecloud/python/graph/badge.svg?token=38G6FGOWKP)](https://codecov.io/github/sqlitecloud/python)
+![PyPI - Version](https://img.shields.io/pypi/v/sqlitecloud?link=https%3A%2F%2Fpypi.org%2Fproject%2FSqliteCloud%2F)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/sqlitecloud?link=https%3A%2F%2Fpypi.org%2Fproject%2FSqliteCloud%2F)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/sqlitecloud?link=https%3A%2F%2Fpypi.org%2Fproject%2FSqliteCloud%2F)
 
 
+[SQLiteCloud](https://sqlitecloud.io) is a powerful Python package that allows you to interact with the SQLite Cloud backend server seamlessly. It provides methods for various database operations. This package is designed to simplify database operations in Python applications, making it easier than ever to work with SQLite Cloud.
+
+- Site: [https://sqlitecloud.io](https://sqlitecloud.io/developers)
+- Documentation: https://..._coming!_
+- Source: [https://github.com/sqlitecloud/python](https://github.com/sqlitecloud/python)
+
 ## Installation
 
 You can install SqliteCloud Package using Python Package Index (PYPI):
 
 ```bash
-$ pip install SqliteCloud
+$ pip install sqlitecloud
 ```
 
 ## Usage
 <hr>
 
 ```python
 from sqlitecloud.client import SqliteCloudClient
@@ -50,15 +62,15 @@
 client = SqliteCloudClient(cloud_account=account)
 conn = client.open_connection()
 ```
 
 #### _Using string configuration_
 
 ```python
-account = SqliteCloudAccount("sqlitecloud://user:pass@host.com:port/dbname?timeout=10&key2=value2&key3=value3")
+account = SqliteCloudAccount("sqlitecloud://user:pass@host.com:port/dbname?apikey=myapikey")
 client = SqliteCloudClient(cloud_account=account)
 conn = client.open_connection()
 ```
 
 ### _Execute a query_
 You can bind values to parametric queries: you can pass parameters as positional values in an array
 ```python
@@ -71,12 +83,22 @@
 ### _Iterate result_
 result is an iterable object
 ```python
 for row in result:
     print(row)
 ```
 
+### _Specific value_
+```python
+result.get_value(0, 0)
+```
+
+### _Column name_
+```python
+result.get_name(0)
+```
+
 ### _Close connection_
 
-```python 
+```python
 client.disconnect(conn)
 ```
```

### Comparing `sqlitecloud-0.0.75/SqliteCloud.egg-info/SOURCES.txt` & `sqlitecloud-0.0.77/SqliteCloud.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 MANIFEST.in
-README-PYPI.md
+README.md
 setup.py
 SqliteCloud.egg-info/PKG-INFO
 SqliteCloud.egg-info/SOURCES.txt
 SqliteCloud.egg-info/dependency_links.txt
 SqliteCloud.egg-info/requires.txt
 SqliteCloud.egg-info/top_level.txt
 sqlitecloud/__init__.py
 sqlitecloud/client.py
-sqlitecloud/conn_info.py
 sqlitecloud/download.py
 sqlitecloud/driver.py
 sqlitecloud/pubsub.py
 sqlitecloud/resultset.py
 sqlitecloud/types.py
 sqlitecloud/upload.py
 tests/__init__.py
```

### Comparing `sqlitecloud-0.0.75/sqlitecloud/client.py` & `sqlitecloud-0.0.77/sqlitecloud/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 """
 from typing import Optional
 from urllib import parse
 
 from sqlitecloud.driver import Driver
 from sqlitecloud.resultset import SqliteCloudResultSet
 from sqlitecloud.types import (
+    SQCLOUD_DEFAULT,
     SQCloudConfig,
     SQCloudConnect,
     SQCloudException,
     SqliteCloudAccount,
 )
 
 
 class SqliteCloudClient:
     """
     Client to interact with Sqlite Cloud
     """
 
-    SQLITE_DEFAULT_PORT = 8860
-
     def __init__(
         self,
         cloud_account: Optional[SqliteCloudAccount] = None,
         connection_str: Optional[str] = None,
     ) -> None:
         """Initializes a new instance of the class with connection information.
 
         Args:
-            cloud_account (SqliteCloudAccount): The account information for the SQlite Cloud database.
+            cloud_account (SqliteCloudAccount): The account information for the
+                SQlite Cloud database.
             connection_str (str): The connection string for the SQlite Cloud database.
                 Eg: sqlitecloud://user:pass@host.com:port/dbname?timeout=10&apikey=abcd123
 
         """
         self._driver = Driver()
 
         self.config = SQCloudConfig()
@@ -45,15 +45,16 @@
         else:
             raise SQCloudException("Missing connection parameters")
 
     def open_connection(self) -> SQCloudConnect:
         """Opens a connection to the SQCloud server.
 
         Returns:
-            SQCloudConnect: An instance of the SQCloudConnect class representing the connection to the SQCloud server.
+            SQCloudConnect: An instance of the SQCloudConnect class representing
+                the connection to the SQCloud server.
 
         Raises:
             SQCloudException: If an error occurs while opening the connection.
         """
         connection = self._driver.connect(
             self.config.account.hostname, self.config.account.port, self.config
         )
@@ -71,17 +72,15 @@
             conn (SQCloudConnect): The connection to the database.
 
         Returns:
             bool: True if the connection is open, False otherwise.
         """
         return self._driver.is_connected(conn)
 
-    def exec_query(
-        self, query: str, conn: SQCloudConnect
-    ) -> SqliteCloudResultSet:
+    def exec_query(self, query: str, conn: SQCloudConnect) -> SqliteCloudResultSet:
         """Executes a SQL query on the SQLite Cloud database.
 
         Args:
             query (str): The SQL query to be executed.
 
         Returns:
             SqliteCloudResultSet: The result set of the executed query.
@@ -144,15 +143,15 @@
             path = params.path
             database = path.strip("/")
             if database:
                 config.account.dbname = database
 
             config.account.hostname = params.hostname
             config.account.port = (
-                int(params.port) if params.port else self.SQLITE_DEFAULT_PORT
+                int(params.port) if params.port else SQCLOUD_DEFAULT.PORT.value
             )
 
             return config
         except Exception as e:
             raise SQCloudException(
                 f"Invalid connection string {connection_string}"
             ) from e
```

### Comparing `sqlitecloud-0.0.75/sqlitecloud/download.py` & `sqlitecloud-0.0.77/sqlitecloud/download.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from io import BufferedWriter
 import logging
+from io import BufferedWriter
 
 from sqlitecloud.driver import Driver
 from sqlitecloud.types import SQCloudConnect
 
 
 def xCallback(
     fd: BufferedWriter, data: bytes, blen: int, ntot: int, nprogress: int
```

### Comparing `sqlitecloud-0.0.75/sqlitecloud/driver.py` & `sqlitecloud-0.0.77/sqlitecloud/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from io import BufferedReader, BufferedWriter
 import logging
 import select
+import socket
 import ssl
 import threading
+from io import BufferedReader, BufferedWriter
 from typing import Callable, Optional, Union
+
 import lz4.block
+
 from sqlitecloud.resultset import SQCloudResult, SqliteCloudResultSet
 from sqlitecloud.types import (
     SQCLOUD_CMD,
     SQCLOUD_DEFAULT,
     SQCLOUD_INTERNAL_ERRCODE,
     SQCLOUD_RESULT_TYPE,
     SQCLOUD_ROWSET,
     SQCloudConfig,
     SQCloudConnect,
     SQCloudException,
     SQCloudNumber,
     SQCloudRowsetSignature,
     SQCloudValue,
 )
-import socket
 
 
 class Driver:
     SQCLOUD_DEFAULT_UPLOAD_SIZE = 512 * 1024
 
     def __init__(self) -> None:
         # Used while parsing chunked rowset
@@ -61,16 +63,14 @@
         Disconnect from the SQLite Cloud server.
         """
         try:
             if conn.socket:
                 conn.socket.close()
             if not only_main_socket and conn.pubsub_socket:
                 conn.pubsub_socket.close()
-        except Exception:
-            pass
         finally:
             conn.socket = None
             if not only_main_socket:
                 conn.pubsub_socket = None
 
     def execute(self, command: str, connection: SQCloudConnect) -> SQCloudResult:
         """
@@ -127,15 +127,15 @@
                 context.verify_mode = ssl.CERT_NONE
 
             sock = context.wrap_socket(sock, server_hostname=hostname)
 
         try:
             sock.connect((hostname, port))
         except Exception as e:
-            errmsg = f"An error occurred while initializing the socket."
+            errmsg = "An error occurred while initializing the socket."
             raise SQCloudException(errmsg) from e
 
         return sock
 
     def _internal_reconnect(self, buffer: bytes) -> bool:
         return True
 
@@ -182,20 +182,20 @@
                         logging.info("PubSub socket dismissed.")
                         break
 
                     # wait for the socket to be readable (no timeout)
                     ready_to_read, _, errors = select.select(
                         [connection.pubsub_socket], [], []
                     )
-                    # eg, no data to read
-                    if len(ready_to_read) == 0:
-                        continue
                     # eg, if the socket is closed
                     if len(errors) > 0:
                         break
+                    # eg, no data to read
+                    if len(ready_to_read) == 0:
+                        continue
 
                     data = connection.pubsub_socket.recv(blen)
                     if not data:
                         logging.info("PubSub connection closed.")
                         break
                 except Exception as e:
                     logging.error(
```

### Comparing `sqlitecloud-0.0.75/sqlitecloud/pubsub.py` & `sqlitecloud-0.0.77/sqlitecloud/pubsub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import socket
-from sqlite3 import connect
 from typing import Callable, Optional
+
 from sqlitecloud.driver import Driver
 from sqlitecloud.resultset import SqliteCloudResultSet
 from sqlitecloud.types import SQCLOUD_PUBSUB_SUBJECT, SQCloudConnect
 
 
 class SqliteCloudPubSub:
     def __init__(self) -> None:
```

### Comparing `sqlitecloud-0.0.75/sqlitecloud/resultset.py` & `sqlitecloud-0.0.77/sqlitecloud/resultset.py`

 * *Files identical despite different names*

### Comparing `sqlitecloud-0.0.75/sqlitecloud/types.py` & `sqlitecloud-0.0.77/sqlitecloud/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
+import types
 from asyncio import AbstractEventLoop
 from enum import Enum
-from threading import Thread
-import types
 from typing import Callable, Optional
-from enum import Enum
 
 
 class SQCLOUD_DEFAULT(Enum):
     PORT = 8860
     TIMEOUT = 12
     UPLOAD_SIZE = 512 * 1024
 
@@ -95,17 +93,17 @@
 
 
 class SqliteCloudAccount:
     def __init__(
         self,
         username: Optional[str] = "",
         password: Optional[str] = "",
-        hostname: Optional[str] = "",
+        hostname: str = "",
         dbname: Optional[str] = "",
-        port: Optional[int] = SQCLOUD_DEFAULT.PORT.value,
+        port: int = SQCLOUD_DEFAULT.PORT.value,
         apikey: Optional[str] = "",
     ) -> None:
         # User name is required unless connectionstring is provided
         self.username = username
         # Password is required unless connection string is provided
         self.password = password
         # Password is hashed
```

### Comparing `sqlitecloud-0.0.75/sqlitecloud/upload.py` & `sqlitecloud-0.0.77/sqlitecloud/upload.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from io import BufferedReader
+import logging
 import os
+from io import BufferedReader
 from typing import Optional
+
 from sqlitecloud.driver import Driver
 from sqlitecloud.types import SQCloudConnect
-import logging
+
 
 def xCallback(fd: BufferedReader, blen: int, ntot: int, nprogress: int) -> bytes:
     """
     Callback function used for uploading data.
 
     Args:
         fd (BufferedReader): The file descriptor to read data from.
@@ -41,19 +43,19 @@
         key (Optional[str]): The encryption key for the database. If None, no encryption is used.
         filename (str): The path to the SQLite database file to be uploaded.
 
     Raises:
         SQCloudException: If an error occurs while uploading the database.
 
     """
-    
+
     # Create a driver object
     driver = Driver()
 
-    with open(filename, 'rb') as fd:
+    with open(filename, "rb") as fd:
         dbsize = os.path.getsize(filename)
 
         driver.upload_database(
             connection,
             dbname,
             key,
             False,
```

### Comparing `sqlitecloud-0.0.75/tests/conftest.py` & `sqlitecloud-0.0.77/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import os
+
 import pytest
 from dotenv import load_dotenv
 
 from sqlitecloud.client import SqliteCloudClient
 from sqlitecloud.types import SQCloudConnect, SqliteCloudAccount
 
+
 @pytest.fixture(autouse=True)
 def load_env_vars():
     load_dotenv(".env")
 
+
 @pytest.fixture()
 def sqlitecloud_connection():
     account = SqliteCloudAccount()
     account.username = os.getenv("SQLITE_USER")
     account.password = os.getenv("SQLITE_PASSWORD")
     account.dbname = os.getenv("SQLITE_DB")
     account.hostname = os.getenv("SQLITE_HOST")
-    account.port = 8860
+    account.port = int(os.getenv("SQLITE_PORT"))
 
     client = SqliteCloudClient(cloud_account=account)
 
     connection = client.open_connection()
     assert isinstance(connection, SQCloudConnect)
     assert client.is_connected(connection)
 
     yield (connection, client)
 
-    client.disconnect(connection)
+    client.disconnect(connection)
```

### Comparing `sqlitecloud-0.0.75/tests/integration/test_client.py` & `sqlitecloud-0.0.77/tests/integration/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import json
-from multiprocessing import connection
 import os
-import sqlite3
-import tempfile
 import time
 
 import pytest
+
 from sqlitecloud.client import SqliteCloudClient
 from sqlitecloud.types import (
     SQCLOUD_ERRCODE,
     SQCLOUD_INTERNAL_ERRCODE,
     SQCLOUD_RESULT_TYPE,
     SQCloudConnect,
     SQCloudException,
@@ -26,39 +24,39 @@
 
     def test_connection_with_credentials(self):
         account = SqliteCloudAccount()
         account.username = os.getenv("SQLITE_USER")
         account.password = os.getenv("SQLITE_PASSWORD")
         account.dbname = os.getenv("SQLITE_DB")
         account.hostname = os.getenv("SQLITE_HOST")
-        account.port = 8860
+        account.port = int(os.getenv("SQLITE_PORT"))
 
         client = SqliteCloudClient(cloud_account=account)
         conn = client.open_connection()
         assert isinstance(conn, SQCloudConnect)
 
         client.disconnect(conn)
 
     def test_connection_with_apikey(self):
         account = SqliteCloudAccount()
         account.username = os.getenv("SQLITE_API_KEY")
         account.hostname = os.getenv("SQLITE_HOST")
-        account.port = 8860
+        account.port = int(os.getenv("SQLITE_PORT"))
 
         client = SqliteCloudClient(cloud_account=account)
         conn = client.open_connection()
         assert isinstance(conn, SQCloudConnect)
 
         client.disconnect(conn)
 
     def test_connection_without_credentials_and_apikey(self):
         account = SqliteCloudAccount()
         account.dbname = os.getenv("SQLITE_DB")
         account.hostname = os.getenv("SQLITE_HOST")
-        account.port = 8860
+        account.port = int(os.getenv("SQLITE_PORT"))
 
         client = SqliteCloudClient(cloud_account=account)
 
         with pytest.raises(SQCloudException):
             client.open_connection()
 
     def test_connect_with_string(self):
@@ -81,49 +79,49 @@
 
         client.disconnect(conn)
 
     def test_is_connected(self):
         account = SqliteCloudAccount()
         account.username = os.getenv("SQLITE_API_KEY")
         account.hostname = os.getenv("SQLITE_HOST")
-        account.port = 8860
+        account.port = int(os.getenv("SQLITE_PORT"))
 
         client = SqliteCloudClient(cloud_account=account)
 
         conn = client.open_connection()
-        assert client.is_connected(conn) == True
+        assert client.is_connected(conn)
 
         client.disconnect(conn)
-        assert client.is_connected(conn) == False
+        assert not client.is_connected(conn)
 
     def test_disconnect(self):
         account = SqliteCloudAccount()
         account.username = os.getenv("SQLITE_API_KEY")
         account.hostname = os.getenv("SQLITE_HOST")
-        account.port = 8860
+        account.port = int(os.getenv("SQLITE_PORT"))
 
         client = SqliteCloudClient(cloud_account=account)
 
         conn = client.open_connection()
-        assert client.is_connected(conn) == True
+        assert client.is_connected(conn)
 
         client.disconnect(conn)
-        assert client.is_connected(conn) == False
+        assert not client.is_connected(conn)
         assert conn.socket is None
         assert conn.pubsub_socket is None
 
         # disconnecting a second time should not raise an exception
         client.disconnect(conn)
 
     def test_select(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
         result = client.exec_query("SELECT 'Hello'", connection)
 
-        assert False == result.is_result
+        assert not result.is_result
         assert 1 == result.nrows
         assert 1 == result.ncols
         assert "Hello" == result.get_value(0, 0)
 
     def test_column_not_found(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         with pytest.raises(SQCloudException) as e:
@@ -235,15 +233,15 @@
 
         assert "PONG" == result.get_result()
 
     def test_json(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST JSON", connection)
 
-        assert SQCLOUD_RESULT_TYPE.RESULT_JSON == result.tag 
+        assert SQCLOUD_RESULT_TYPE.RESULT_JSON == result.tag
         assert {
             "msg-from": {"class": "soldier", "name": "Wixilav"},
             "msg-to": {"class": "supreme-commander", "name": "[Redacted]"},
             "msg-type": ["0xdeadbeef", "irc log"],
             "msg-log": [
                 "soldier: Boss there is a slight problem with the piece offering to humans",
                 "supreme-commander: Explain yourself soldier!",
@@ -289,15 +287,15 @@
         )
 
     def test_array(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST ARRAY", connection)
 
         result_array = result.get_result()
-        
+
         assert SQCLOUD_RESULT_TYPE.RESULT_ARRAY == result.tag
         assert isinstance(result_array, list)
         assert len(result_array) == 5
         assert result_array[0] == "Hello World"
         assert result_array[1] == "123456"
         assert result_array[2] == "3.1415"
         assert result_array[3] is None
@@ -328,15 +326,14 @@
 
         client.disconnect(connection)
 
         # maxrows cannot be tested at this level.
         # just expect everything is ok
         assert rowset.nrows > 100
 
-
     def test_max_rowset_option_to_fail_when_rowset_is_bigger(self):
         account = SqliteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = os.getenv("SQLITE_DB")
         account.apikey = os.getenv("SQLITE_API_KEY")
 
         client = SqliteCloudClient(cloud_account=account)
@@ -348,15 +345,14 @@
             client.exec_query("SELECT * FROM albums", connection)
 
         client.disconnect(connection)
 
         assert SQCLOUD_ERRCODE.INTERNAL.value == e.value.errcode
         assert "RowSet too big to be sent (limit set to 1024 bytes)." == e.value.errmsg
 
-
     def test_max_rowset_option_to_succeed_when_rowset_is_lighter(self):
         account = SqliteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = os.getenv("SQLITE_DB")
         account.apikey = os.getenv("SQLITE_API_KEY")
 
         client = SqliteCloudClient(cloud_account=account)
@@ -435,15 +431,15 @@
                 WITH RECURSIVE r(i) AS (
                     VALUES(0)
                     UNION ALL
                     SELECT i FROM r
                     LIMIT 10000000
                 )
                 SELECT i FROM r WHERE i = 1;""",
-                connection
+                connection,
             )
 
         client.disconnect(connection)
 
         assert e.value.errcode == SQCLOUD_INTERNAL_ERRCODE.NETWORK
         assert e.value.errmsg == "An error occurred while reading data from the socket."
 
@@ -641,15 +637,16 @@
         client = SqliteCloudClient(cloud_account=account)
         client.config.compression = True
 
         connection = client.open_connection()
 
         # min compression size for rowset set by default to 20400 bytes
         rowset = client.exec_query(
-            "SELECT * from albums inner join albums a2 on albums.AlbumId = a2.AlbumId", connection
+            "SELECT * from albums inner join albums a2 on albums.AlbumId = a2.AlbumId",
+            connection,
         )
 
         client.disconnect(connection)
 
         assert rowset.nrows > 0
         assert rowset.ncols > 0
         assert rowset.get_name(0) == "AlbumId"
```

### Comparing `sqlitecloud-0.0.75/tests/integration/test_pubsub.py` & `sqlitecloud-0.0.77/tests/integration/test_pubsub.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from time import sleep
-import time
+import threading
+import uuid
 
 import pytest
 
 from sqlitecloud.pubsub import SqliteCloudPubSub
 from sqlitecloud.resultset import SqliteCloudResultSet
 from sqlitecloud.types import (
     SQCLOUD_ERRCODE,
@@ -14,43 +14,46 @@
 
 
 class TestPubSub:
     def test_listen_channel_and_notify(self, sqlitecloud_connection):
         connection, _ = sqlitecloud_connection
 
         callback_called = False
+        flag = threading.Event()
 
         def assert_callback(conn, result, data):
             nonlocal callback_called
+            nonlocal flag
 
             if isinstance(result, SqliteCloudResultSet):
                 assert result.tag == SQCLOUD_RESULT_TYPE.RESULT_JSON
                 assert data == ["somedata"]
                 callback_called = True
+                flag.set()
 
         pubsub = SqliteCloudPubSub()
         type = SQCLOUD_PUBSUB_SUBJECT.CHANNEL
-        channel = "channel" + str(int(time.time()))
+        channel = "channel" + str(uuid.uuid4())
 
         pubsub.create_channel(connection, channel)
         pubsub.listen(connection, type, channel, assert_callback, ["somedata"])
 
         pubsub.notify_channel(connection, channel, "somedata2")
 
         # wait for callback to be called
-        sleep(1)
+        flag.wait(30)
 
         assert callback_called
 
     def test_unlisten_channel(self, sqlitecloud_connection):
         connection, _ = sqlitecloud_connection
 
         pubsub = SqliteCloudPubSub()
         type = SQCLOUD_PUBSUB_SUBJECT.CHANNEL
-        channel_name = "channel" + str(int(time.time()))
+        channel_name = "channel" + str(uuid.uuid4())
 
         pubsub.create_channel(connection, channel_name)
         pubsub.listen(connection, type, channel_name, lambda conn, result, data: None)
 
         result = pubsub.list_connections(connection)
         assert channel_name in result.data
 
@@ -62,15 +65,15 @@
         assert connection.pubsub_callback is None
         assert connection.pubsub_data is None
 
     def test_create_channel_to_fail_if_exists(self, sqlitecloud_connection):
         connection, _ = sqlitecloud_connection
 
         pubsub = SqliteCloudPubSub()
-        channel_name = "channel" + str(int(time.time()))
+        channel_name = "channel" + str(uuid.uuid4())
 
         pubsub.create_channel(connection, channel_name, if_not_exists=True)
 
         with pytest.raises(SQCloudException) as e:
             pubsub.create_channel(connection, channel_name, if_not_exists=False)
 
         assert (
@@ -79,77 +82,90 @@
         )
         assert e.value.errcode == SQCLOUD_ERRCODE.GENERIC.value
 
     def test_is_connected(self, sqlitecloud_connection):
         connection, _ = sqlitecloud_connection
 
         pubsub = SqliteCloudPubSub()
-        channel_name = "channel" + str(int(time.time()))
+        channel_name = "channel" + str(uuid.uuid4())
 
         assert not pubsub.is_connected(connection)
 
         pubsub.create_channel(connection, channel_name, if_not_exists=True)
-        pubsub.listen(connection, SQCLOUD_PUBSUB_SUBJECT.CHANNEL, channel_name, lambda conn, result, data: None)
+        pubsub.listen(
+            connection,
+            SQCLOUD_PUBSUB_SUBJECT.CHANNEL,
+            channel_name,
+            lambda conn, result, data: None,
+        )
 
         assert pubsub.is_connected(connection)
 
     def test_set_pubsub_only(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
         callback_called = False
+        flag = threading.Event()
 
         def assert_callback(conn, result, data):
             nonlocal callback_called
+            nonlocal flag
 
             if isinstance(result, SqliteCloudResultSet):
                 assert result.get_result() is not None
                 callback_called = True
+                flag.set()
 
         pubsub = SqliteCloudPubSub()
         type = SQCLOUD_PUBSUB_SUBJECT.CHANNEL
-        channel = "channel" + str(int(time.time()))
+        channel = "channel" + str(uuid.uuid4())
 
         pubsub.create_channel(connection, channel, if_not_exists=True)
         pubsub.listen(connection, type, channel, assert_callback)
 
         pubsub.set_pubsub_only(connection)
 
         assert not client.is_connected(connection)
         assert pubsub.is_connected(connection)
 
         connection2 = client.open_connection()
         pubsub2 = SqliteCloudPubSub()
         pubsub2.notify_channel(connection2, channel, "message-in-a-bottle")
 
+        client.disconnect(connection2)
+
         # wait for callback to be called
-        sleep(2)
+        flag.wait(30)
 
         assert callback_called
 
-        client.disconnect(connection2)
-
     def test_listen_table_for_update(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
         callback_called = False
+        flag = threading.Event()
 
         def assert_callback(conn, result, data):
             nonlocal callback_called
+            nonlocal flag
 
             if isinstance(result, SqliteCloudResultSet):
                 assert result.tag == SQCLOUD_RESULT_TYPE.RESULT_JSON
                 assert new_name in result.get_result()
                 assert data == ["somedata"]
                 callback_called = True
+                flag.set()
 
         pubsub = SqliteCloudPubSub()
         type = SQCLOUD_PUBSUB_SUBJECT.TABLE
-        new_name = "Rock"+ str(int(time.time()))
+        new_name = "Rock" + str(uuid.uuid4())
 
         pubsub.listen(connection, type, "genres", assert_callback, ["somedata"])
 
-        client.exec_query(f"UPDATE genres SET Name = '{new_name}' WHERE GenreId = 1;", connection)
+        client.exec_query(
+            f"UPDATE genres SET Name = '{new_name}' WHERE GenreId = 1;", connection
+        )
 
         # wait for callback to be called
-        sleep(1)
+        flag.wait(30)
 
-        assert callback_called
+        assert callback_called
```

### Comparing `sqlitecloud-0.0.75/tests/integration/test_upload.py` & `sqlitecloud-0.0.77/tests/integration/test_upload.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os
 import uuid
-import pytest
-from sqlitecloud.client import SqliteCloudClient
-from sqlitecloud.types import SQCloudConnect, SqliteCloudAccount
+
 from sqlitecloud.upload import upload_db
 
 
 class TestUpload:
     def test_upload_db(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
```

