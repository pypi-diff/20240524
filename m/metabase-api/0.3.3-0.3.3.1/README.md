# Comparing `tmp/metabase-api-0.3.3.tar.gz` & `tmp/metabase-api-0.3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabase-api-0.3.3.tar", last modified: Mon May 13 04:24:49 2024, max compression
+gzip compressed data, was "metabase-api-0.3.3.1.tar", last modified: Fri May 24 17:40:47 2024, max compression
```

## Comparing `metabase-api-0.3.3.tar` & `metabase-api-0.3.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 04:24:49.420837 metabase-api-0.3.3/
--rw-rw-rw-   0        0        0     1080 2024-05-13 00:48:54.000000 metabase-api-0.3.3/LICENSE
--rw-rw-rw-   0        0        0    13252 2024-05-13 04:24:49.420837 metabase-api-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    12638 2024-05-13 00:51:10.000000 metabase-api-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 04:24:49.404095 metabase-api-0.3.3/metabase_api/
--rw-rw-rw-   0        0        0       39 2024-05-13 00:48:54.000000 metabase-api-0.3.3/metabase_api/__init__.py
--rw-rw-rw-   0        0        0    12728 2024-05-13 00:48:54.000000 metabase-api-0.3.3/metabase_api/_helper_methods.py
--rw-rw-rw-   0        0        0     1108 2024-05-13 00:48:54.000000 metabase-api-0.3.3/metabase_api/_rest_methods.py
--rw-rw-rw-   0        0        0    17174 2024-05-13 00:48:54.000000 metabase-api-0.3.3/metabase_api/copy_methods.py
--rw-rw-rw-   0        0        0    11866 2024-05-13 00:48:54.000000 metabase-api-0.3.3/metabase_api/create_methods.py
--rw-rw-rw-   0        0        0    15325 2024-05-13 04:15:23.000000 metabase-api-0.3.3/metabase_api/metabase_api.py
-drwxrwxrwx   0        0        0        0 2024-05-13 04:24:49.414335 metabase-api-0.3.3/metabase_api.egg-info/
--rw-rw-rw-   0        0        0    13252 2024-05-13 04:24:49.000000 metabase-api-0.3.3/metabase_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-05-13 04:24:49.000000 metabase-api-0.3.3/metabase_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 04:24:49.000000 metabase-api-0.3.3/metabase_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-13 04:24:49.000000 metabase-api-0.3.3/metabase_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-13 04:24:49.000000 metabase-api-0.3.3/metabase_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 04:24:49.422020 metabase-api-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      687 2024-05-13 00:49:44.000000 metabase-api-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 04:24:49.418332 metabase-api-0.3.3/tests/
--rw-rw-rw-   0        0        0        1 2024-05-13 00:48:54.000000 metabase-api-0.3.3/tests/__init__.py
--rw-rw-rw-   0        0        0    11237 2024-05-13 04:15:59.000000 metabase-api-0.3.3/tests/test_metabase_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:40:47.082677 metabase-api-0.3.3.1/
+-rw-rw-rw-   0        0        0     1080 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/LICENSE
+-rw-rw-rw-   0        0        0    13254 2024-05-24 17:40:47.082677 metabase-api-0.3.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    12638 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 17:40:47.067045 metabase-api-0.3.3.1/metabase_api/
+-rw-rw-rw-   0        0        0       39 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/metabase_api/__init__.py
+-rw-rw-rw-   0        0        0    12728 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/metabase_api/_helper_methods.py
+-rw-rw-rw-   0        0        0     1108 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/metabase_api/_rest_methods.py
+-rw-rw-rw-   0        0        0    17174 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/metabase_api/copy_methods.py
+-rw-rw-rw-   0        0        0    11866 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/metabase_api/create_methods.py
+-rw-rw-rw-   0        0        0    15352 2024-05-24 17:37:54.000000 metabase-api-0.3.3.1/metabase_api/metabase_api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:40:47.082677 metabase-api-0.3.3.1/metabase_api.egg-info/
+-rw-rw-rw-   0        0        0    13254 2024-05-24 17:40:46.000000 metabase-api-0.3.3.1/metabase_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-05-24 17:40:46.000000 metabase-api-0.3.3.1/metabase_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 17:40:46.000000 metabase-api-0.3.3.1/metabase_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 17:40:46.000000 metabase-api-0.3.3.1/metabase_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-24 17:40:46.000000 metabase-api-0.3.3.1/metabase_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 17:40:47.082677 metabase-api-0.3.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      689 2024-05-24 17:32:18.000000 metabase-api-0.3.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 17:40:47.082677 metabase-api-0.3.3.1/tests/
+-rw-rw-rw-   0        0        0        1 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/tests/__init__.py
+-rw-rw-rw-   0        0        0    11231 2024-05-24 17:27:42.000000 metabase-api-0.3.3.1/tests/test_metabase_api.py
```

### Comparing `metabase-api-0.3.3/LICENSE` & `metabase-api-0.3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.3/PKG-INFO` & `metabase-api-0.3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api
-Version: 0.3.3
+Version: 0.3.3.1
 Summary: A Python Wrapper for Metabase API
 Home-page: https://github.com/vvaezian/metabase_api_python
 Author: Vahid Vaezian
 Author-email: vahid.vaezian@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `metabase-api-0.3.3/README.md` & `metabase-api-0.3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.3/metabase_api/_helper_methods.py` & `metabase-api-0.3.3.1/metabase_api/_helper_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.3/metabase_api/_rest_methods.py` & `metabase-api-0.3.3.1/metabase_api/_rest_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.3/metabase_api/copy_methods.py` & `metabase-api-0.3.3.1/metabase_api/copy_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.3/metabase_api/create_methods.py` & `metabase-api-0.3.3.1/metabase_api/create_methods.py`

 * *Files identical despite different names*

### Comparing `metabase-api-0.3.3/metabase_api/metabase_api.py` & `metabase-api-0.3.3.1/metabase_api/metabase_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 
 class Metabase_API():
 
     def __init__(self, domain, email=None, password=None, api_key=None, basic_auth=False, is_admin=True):
         assert email is not None or api_key is not None
         self.domain = domain.rstrip('/')
         self.email = email
-        self.auth = (self.email, self.password) if basic_auth and email else None
+        self.auth = None
         if email:
             self.password = getpass.getpass(prompt='Please enter your password: ') if password is None else password
             self.session_id = None
             self.header = None
+            if basic_auth:
+                self.auth = (self.email, self.password) 
             self.authenticate()
         else:
             self.header = {"X-API-KEY": api_key}
         self.is_admin = is_admin
         if not self.is_admin:
             print('''
                 Ask your Metabase admin to disable "Friendly Table and Field Names" (in Admin Panel > Settings > General).
```

### Comparing `metabase-api-0.3.3/metabase_api.egg-info/PKG-INFO` & `metabase-api-0.3.3.1/metabase_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-api
-Version: 0.3.3
+Version: 0.3.3.1
 Summary: A Python Wrapper for Metabase API
 Home-page: https://github.com/vvaezian/metabase_api_python
 Author: Vahid Vaezian
 Author-email: vahid.vaezian@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `metabase-api-0.3.3/setup.py` & `metabase-api-0.3.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="metabase-api",
-    version="0.3.3",
+    version="0.3.3.1",
     author="Vahid Vaezian",
     author_email="vahid.vaezian@gmail.com",
     description="A Python Wrapper for Metabase API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vvaezian/metabase_api_python",
     packages=setuptools.find_packages(),
```

### Comparing `metabase-api-0.3.3/tests/test_metabase_api.py` & `metabase-api-0.3.3.1/tests/test_metabase_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,18 +261,18 @@
     self.assertEqual(res, json_data)
 
     # csv
     res = mb.get_card_data(card_id=1, data_format='csv')
     csv_data = 'col1,col2\nrow1 cell1,1\n,2\nrow3 cell1,\n,\nrow5 cell1,5\n'
     self.assertEqual(res, csv_data)
 
-    # # filtered data
-    # res = mb.get_card_data(card_id=2, parameters=[{"type":"string/=","value":['row1 cell1', 'row3 cell1'],"target":["dimension",["template-tag","test_filter"]]}])
-    # filtered_data = [{'col1': 'row1 cell1', 'col2': 1}, {'col1': 'row3 cell1', 'col2': None}]
-    # self.assertEqual(res, filtered_data)
+    # filtered data
+    res = mb.get_card_data(card_id=2, parameters=[{"type":"string/=","value":['row1 cell1', 'row3 cell1'],"target":["dimension",["template-tag","test_filter"]]}])
+    filtered_data = [{'col1': 'row1 cell1', 'col2': '1'}, {'col1': 'row3 cell1', 'col2': None}]
+    self.assertEqual(res, filtered_data)
 
 
 
   def test_clone_card(self):
     # native question
     res = mb.clone_card(2, 9, 10, new_card_name='test_clone_native', new_card_collection_id=1, return_card=True)
     # simple/custom question
```

