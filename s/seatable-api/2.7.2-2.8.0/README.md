# Comparing `tmp/seatable-api-2.7.2.tar.gz` & `tmp/seatable-api-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seatable-api-2.7.2.tar", last modified: Tue Apr 23 04:50:35 2024, max compression
+gzip compressed data, was "dist/seatable-api-2.8.0.tar", last modified: Fri May 24 03:47:25 2024, max compression
```

## Comparing `seatable-api-2.7.2.tar` & `seatable-api-2.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-23 04:50:35.569173 seatable-api-2.7.2/
--rw-r--r--   0 ranjiwei   (501) staff       (20)      733 2024-04-23 04:50:35.568797 seatable-api-2.7.2/PKG-INFO
--rw-r--r--   0 ranjiwei   (501) staff       (20)      300 2021-01-29 01:36:12.000000 seatable-api-2.7.2/README.md
-drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-23 04:50:35.553962 seatable-api-2.7.2/seatable_api/
--rw-r--r--   0 ranjiwei   (501) staff       (20)      171 2024-01-25 01:33:50.000000 seatable-api-2.7.2/seatable_api/__init__.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)    26437 2024-04-23 04:42:37.000000 seatable-api-2.7.2/seatable_api/api_gateway.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)    11418 2021-01-29 01:36:12.000000 seatable-api-2.7.2/seatable_api/column.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     1135 2021-12-15 04:05:31.000000 seatable-api-2.7.2/seatable_api/constants.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     1338 2024-01-25 01:33:50.000000 seatable-api-2.7.2/seatable_api/context.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)    29203 2024-01-25 01:33:50.000000 seatable-api-2.7.2/seatable_api/convert_airtable.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)    13988 2024-03-21 06:02:17.000000 seatable-api-2.7.2/seatable_api/date_utils.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)      235 2024-01-25 01:33:50.000000 seatable-api-2.7.2/seatable_api/exception.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)    49205 2024-04-23 04:41:04.000000 seatable-api-2.7.2/seatable_api/main.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     2876 2021-07-17 06:11:15.000000 seatable-api-2.7.2/seatable_api/message.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     3006 2021-01-13 04:11:42.000000 seatable-api-2.7.2/seatable_api/parsetab.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     9400 2021-02-24 08:59:41.000000 seatable-api-2.7.2/seatable_api/query.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     2744 2021-07-17 06:11:15.000000 seatable-api-2.7.2/seatable_api/socket_io.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     7276 2024-03-27 08:04:05.000000 seatable-api-2.7.2/seatable_api/utils.py
-drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-23 04:50:35.561065 seatable-api-2.7.2/seatable_api.egg-info/
--rw-r--r--   0 ranjiwei   (501) staff       (20)      733 2024-04-23 04:50:35.000000 seatable-api-2.7.2/seatable_api.egg-info/PKG-INFO
--rw-r--r--   0 ranjiwei   (501) staff       (20)      591 2024-04-23 04:50:35.000000 seatable-api-2.7.2/seatable_api.egg-info/SOURCES.txt
--rw-r--r--   0 ranjiwei   (501) staff       (20)        1 2024-04-23 04:50:35.000000 seatable-api-2.7.2/seatable_api.egg-info/dependency_links.txt
--rw-r--r--   0 ranjiwei   (501) staff       (20)       47 2024-04-23 04:50:35.000000 seatable-api-2.7.2/seatable_api.egg-info/requires.txt
--rw-r--r--   0 ranjiwei   (501) staff       (20)       19 2024-04-23 04:50:35.000000 seatable-api-2.7.2/seatable_api.egg-info/top_level.txt
--rw-r--r--   0 ranjiwei   (501) staff       (20)       38 2024-04-23 04:50:35.569305 seatable-api-2.7.2/setup.cfg
--rw-r--r--   0 ranjiwei   (501) staff       (20)      723 2024-04-23 04:49:39.000000 seatable-api-2.7.2/setup.py
-drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-04-23 04:50:35.567066 seatable-api-2.7.2/tests/
--rw-r--r--   0 ranjiwei   (501) staff       (20)        0 2023-04-14 03:49:39.000000 seatable-api-2.7.2/tests/__init__.py
--rw-r--r--   0 ranjiwei   (501) staff       (20)     5261 2023-04-14 03:49:39.000000 seatable-api-2.7.2/tests/dateutils_test.py
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-05-24 03:47:25.976000 seatable-api-2.8.0/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      733 2024-05-24 03:47:25.975677 seatable-api-2.8.0/PKG-INFO
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      300 2021-01-29 01:36:12.000000 seatable-api-2.8.0/README.md
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-05-24 03:47:25.961699 seatable-api-2.8.0/seatable_api/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      171 2024-01-25 01:33:50.000000 seatable-api-2.8.0/seatable_api/__init__.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    26505 2024-05-24 03:41:29.000000 seatable-api-2.8.0/seatable_api/api_gateway.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    11418 2021-01-29 01:36:12.000000 seatable-api-2.8.0/seatable_api/column.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     1135 2021-12-15 04:05:31.000000 seatable-api-2.8.0/seatable_api/constants.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     1338 2024-01-25 01:33:50.000000 seatable-api-2.8.0/seatable_api/context.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    29203 2024-01-25 01:33:50.000000 seatable-api-2.8.0/seatable_api/convert_airtable.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    13988 2024-03-21 06:02:17.000000 seatable-api-2.8.0/seatable_api/date_utils.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      235 2024-01-25 01:33:50.000000 seatable-api-2.8.0/seatable_api/exception.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)    49205 2024-05-24 03:37:02.000000 seatable-api-2.8.0/seatable_api/main.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     2876 2021-07-17 06:11:15.000000 seatable-api-2.8.0/seatable_api/message.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     3006 2021-01-13 04:11:42.000000 seatable-api-2.8.0/seatable_api/parsetab.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     9400 2021-02-24 08:59:41.000000 seatable-api-2.8.0/seatable_api/query.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     2744 2021-07-17 06:11:15.000000 seatable-api-2.8.0/seatable_api/socket_io.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     7276 2024-05-24 03:09:06.000000 seatable-api-2.8.0/seatable_api/utils.py
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-05-24 03:47:25.968170 seatable-api-2.8.0/seatable_api.egg-info/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      733 2024-05-24 03:47:25.000000 seatable-api-2.8.0/seatable_api.egg-info/PKG-INFO
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      591 2024-05-24 03:47:25.000000 seatable-api-2.8.0/seatable_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)        1 2024-05-24 03:47:25.000000 seatable-api-2.8.0/seatable_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)       47 2024-05-24 03:47:25.000000 seatable-api-2.8.0/seatable_api.egg-info/requires.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)       19 2024-05-24 03:47:25.000000 seatable-api-2.8.0/seatable_api.egg-info/top_level.txt
+-rw-r--r--   0 ranjiwei   (501) staff       (20)       38 2024-05-24 03:47:25.976144 seatable-api-2.8.0/setup.cfg
+-rw-r--r--   0 ranjiwei   (501) staff       (20)      723 2024-05-24 03:46:35.000000 seatable-api-2.8.0/setup.py
+drwxr-xr-x   0 ranjiwei   (501) staff       (20)        0 2024-05-24 03:47:25.974055 seatable-api-2.8.0/tests/
+-rw-r--r--   0 ranjiwei   (501) staff       (20)        0 2023-04-14 03:49:39.000000 seatable-api-2.8.0/tests/__init__.py
+-rw-r--r--   0 ranjiwei   (501) staff       (20)     5261 2023-04-14 03:49:39.000000 seatable-api-2.8.0/tests/dateutils_test.py
```

### Comparing `seatable-api-2.7.2/PKG-INFO` & `seatable-api-2.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.7.2
+Version: 2.8.0
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Description: # seatable-api-python
```

### Comparing `seatable-api-2.7.2/seatable_api/api_gateway.py` & `seatable-api-2.8.0/seatable_api/api_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,16 @@
         :param desc: boolean
         :param start: int
         :param limit: int
         :return: list
         """
         url = self._row_server_url()
         params = {
-            'table_name': table_name
+            'table_name': table_name,
+            'convert_keys': True
         }
 
         if like_table_id(table_name):
             params['table_id'] = table_name
         if view_name:
             params['view_name'] = view_name
         if order_by:
@@ -222,15 +223,16 @@
         """
         :param table_name: str
         :param row_id: str
         :return: dict
         """
         url = self._row_server_url() + row_id + '/'
         params = {
-            'table_name': table_name
+            'table_name': table_name,
+            'convert_keys': True
         }
 
         if like_table_id(table_name):
             params['table_id'] = table_name
         response = requests.get(url, params=params, headers=self.headers, timeout=self.timeout)
         data = parse_response(response)
         return data
```

### Comparing `seatable-api-2.7.2/seatable_api/column.py` & `seatable-api-2.8.0/seatable_api/column.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/seatable_api/constants.py` & `seatable-api-2.8.0/seatable_api/constants.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/seatable_api/context.py` & `seatable-api-2.8.0/seatable_api/context.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/seatable_api/convert_airtable.py` & `seatable-api-2.8.0/seatable_api/convert_airtable.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/seatable_api/date_utils.py` & `seatable-api-2.8.0/seatable_api/date_utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/seatable_api/main.py` & `seatable-api-2.8.0/seatable_api/main.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/seatable_api/message.py` & `seatable-api-2.8.0/seatable_api/message.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/seatable_api/parsetab.py` & `seatable-api-2.8.0/seatable_api/parsetab.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/seatable_api/query.py` & `seatable-api-2.8.0/seatable_api/query.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/seatable_api/socket_io.py` & `seatable-api-2.8.0/seatable_api/socket_io.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/seatable_api/utils.py` & `seatable-api-2.8.0/seatable_api/utils.py`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/seatable_api.egg-info/PKG-INFO` & `seatable-api-2.8.0/seatable_api.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatable-api
-Version: 2.7.2
+Version: 2.8.0
 Summary: Python client for SeaTable web api
 Home-page: https://github.com/seatable/seatable-api-python
 Author: seatable
 Author-email: support@seafile.com
 License: Apache Licence
 Description: # seatable-api-python
```

### Comparing `seatable-api-2.7.2/seatable_api.egg-info/SOURCES.txt` & `seatable-api-2.8.0/seatable_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seatable-api-2.7.2/setup.py` & `seatable-api-2.8.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '2.7.2'
+__version__ = '2.8.0'
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='seatable-api',
     version=__version__,
```

### Comparing `seatable-api-2.7.2/tests/dateutils_test.py` & `seatable-api-2.8.0/tests/dateutils_test.py`

 * *Files identical despite different names*

