# Comparing `tmp/smartsheet-dataframe-0.2.0.tar.gz` & `tmp/smartsheet_dataframe-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\there\PycharmProjects\Smartsheet-DataFrame\dist\tmp8mz4ffvy\smartsheet-dataframe-0.2.0.tar", last modified: Tue Jun  8 01:36:59 2021, max compression
+gzip compressed data, was "smartsheet_dataframe-0.3.0.tar", last modified: Fri May 24 01:07:36 2024, max compression
```

## Comparing `smartsheet-dataframe-0.2.0.tar` & `smartsheet_dataframe-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-06-08 01:36:59.000000 smartsheet-dataframe-0.2.0/
--rw-rw-rw-   0        0        0     1089 2021-05-14 22:01:29.000000 smartsheet-dataframe-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      703 2021-06-08 01:36:59.000000 smartsheet-dataframe-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2429 2021-05-26 00:15:34.000000 smartsheet-dataframe-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2021-06-08 01:36:59.000000 smartsheet-dataframe-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      958 2021-05-26 22:58:08.000000 smartsheet-dataframe-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-08 01:36:59.000000 smartsheet-dataframe-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2021-06-08 01:36:59.000000 smartsheet-dataframe-0.2.0/src/smartsheet_dataframe/
--rw-rw-rw-   0        0        0       91 2021-05-26 23:23:30.000000 smartsheet-dataframe-0.2.0/src/smartsheet_dataframe/__init__.py
--rw-rw-rw-   0        0        0    13589 2021-06-02 03:19:27.000000 smartsheet-dataframe-0.2.0/src/smartsheet_dataframe/smartsheet_dataframe.py
-drwxrwxrwx   0        0        0        0 2021-06-08 01:36:59.000000 smartsheet-dataframe-0.2.0/src/smartsheet_dataframe.egg-info/
--rw-rw-rw-   0        0        0      703 2021-06-08 01:36:59.000000 smartsheet-dataframe-0.2.0/src/smartsheet_dataframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2021-06-08 01:36:59.000000 smartsheet-dataframe-0.2.0/src/smartsheet_dataframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-08 01:36:59.000000 smartsheet-dataframe-0.2.0/src/smartsheet_dataframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2021-06-08 01:36:59.000000 smartsheet-dataframe-0.2.0/src/smartsheet_dataframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2021-06-08 01:36:59.000000 smartsheet-dataframe-0.2.0/src/smartsheet_dataframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 01:07:36.349950 smartsheet_dataframe-0.3.0/
+-rw-rw-rw-   0        0        0     1089 2021-05-14 22:01:29.000000 smartsheet_dataframe-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3196 2024-05-24 01:07:36.348950 smartsheet_dataframe-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2429 2021-05-26 00:15:34.000000 smartsheet_dataframe-0.3.0/README.md
+-rw-rw-rw-   0        0        0      965 2024-05-24 01:05:39.000000 smartsheet_dataframe-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 01:07:36.349950 smartsheet_dataframe-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 01:07:36.326949 smartsheet_dataframe-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 01:07:36.334949 smartsheet_dataframe-0.3.0/src/smartsheet_dataframe/
+-rw-rw-rw-   0        0        0       80 2023-12-22 22:09:07.000000 smartsheet_dataframe-0.3.0/src/smartsheet_dataframe/__init__.py
+-rw-rw-rw-   0        0        0     9666 2023-12-22 22:09:17.000000 smartsheet_dataframe-0.3.0/src/smartsheet_dataframe/smartsheet_dataframe.py
+drwxrwxrwx   0        0        0        0 2024-05-24 01:07:36.346951 smartsheet_dataframe-0.3.0/src/smartsheet_dataframe.egg-info/
+-rw-rw-rw-   0        0        0     3196 2024-05-24 01:07:36.000000 smartsheet_dataframe-0.3.0/src/smartsheet_dataframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-05-24 01:07:36.000000 smartsheet_dataframe-0.3.0/src/smartsheet_dataframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 01:07:36.000000 smartsheet_dataframe-0.3.0/src/smartsheet_dataframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-24 01:07:36.000000 smartsheet_dataframe-0.3.0/src/smartsheet_dataframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-24 01:07:36.000000 smartsheet_dataframe-0.3.0/src/smartsheet_dataframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 01:07:36.344950 smartsheet_dataframe-0.3.0/tests/
+-rw-rw-rw-   0        0        0     2344 2021-05-26 22:40:36.000000 smartsheet_dataframe-0.3.0/tests/tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `smartsheet-dataframe-0.2.0/LICENSE` & `smartsheet_dataframe-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartsheet-dataframe-0.2.0/README.md` & `smartsheet_dataframe-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `smartsheet-dataframe-0.2.0/src/smartsheet_dataframe/smartsheet_dataframe.py` & `smartsheet_dataframe-0.3.0/src/smartsheet_dataframe/smartsheet_dataframe.py`

 * *Files 22% similar despite different names*

```diff
@@ -165,14 +165,19 @@
 
     if include_parent_id:
         columns_list.insert(0, "parent_id")
     if include_row_id:
         columns_list.insert(0, "row_id")
 
     rows_list = []
+    
+	# Handle empty sheet condition
+    if not object_dict.get('rows', None):
+        return pd.DataFrame(columns=columns_list)
+    
     for row in object_dict['rows']:
         cells_list = []
         if include_row_id:
             cells_list.append(int(row['id']))
         if include_parent_id:
             cells_list.append(int(row['parentId'])) if 'parentId' in row else cells_list.append('')
 
@@ -185,140 +190,51 @@
                 cells_list.append('')
         else:
             rows_list.append(cells_list)
 
     return pd.DataFrame(rows_list, columns=columns_list)
 
 
-def _do_request(url: str, method: str = 'GET', options: dict = None,
-                data: dict = None, json=None, token: str = None, retries: int = 3) -> requests.Response:
-    if not (options or token):
-        raise ValueError("Neither 'options' nor 'token' were provided. One of these is required")
-    elif options and not token:
-        if not options.get("Authorization"):
-            raise ValueError("'Authorization' missing from options.")
-    elif options and token:
-        if not options.get("Authorization"):
-            options.update({"Authorization": f"Bearer {token}"})
-    elif token:
-        options = {"Authorization": f"Bearer {token}"}
-
+def _do_request(url: str, options: dict, retries: int = 3) -> requests.Response:
     i = 0
-    response = None
     for i in range(retries):
         try:
-            response = requests.request(method=method.upper(), url=url, headers=options, json=json, data=data)
+            response = requests.get(url, headers=options)
             response_json = response.json()
 
             if response.status_code != 200:
                 if response_json['errorCode'] == 1002 or response_json['errorCode'] == 1003 or \
                         response_json['errorCode'] == 1004:
                     raise AuthenticationError("Could not connect using the supplied auth token \n" +
                                               response.text)
                 elif response_json['errorCode'] == 4004:
                     logger.debug(f"Rate limit exceeded. Waiting and trying again... {i}")
                     time.sleep(5 + (i * 5))
                     continue
                 else:
                     warnings.warn("An unhandled status_code was returned by the Smartsheet API: \n" +
                                   response.text)
+                    return
         except AuthenticationError:
             logger.exception("Smartsheet returned an error status code")
             break
         except:
             logger.exception(f"Not able to retrieve get response. Retrying... {i}")
             time.sleep(5 + (i * 5))
             continue
         break
     else:
         raise Exception(f"Could not retrieve request after retrying {i} times")
 
     return response
 
 
-def set_as_df(df: pd.DataFrame,
-              sheet_id: int,
-              token: str = None,
-              smartsheet_client: Any = None,
-              erase_sheet: bool = False,
-              insert_columns: bool = False,
-              column_mapping: dict = None) -> None:
-    """
-    Set values in a Smartsheet from a Pandas DataFrame
-    ..................................................
-
-    One of 'token' or 'smartsheet_client' parameters must be supplied
-
-    :param df: Pandas DataFrame to copy into sheet
-    :param sheet_id: ID of destination sheet
-    :param token: Smartsheet Authentication Token
-    :param smartsheet_client: smartsheet-python-sdk authentication object
-    :param erase_sheet: If True, will erase all values in a sheet before inserting DataFrame
-    :param insert_columns: If True, columns not found in the sheet will be inserted
-    :param column_mapping: Mapping for Pandas Columns to Dict containing key-value source:destination pairs.
-            This should look like: {'pandas df column name': 'smartsheet_column_name'}
-
-    :return: None
-    """
-
-    sheet = None
-    if token:
-        if smartsheet_client:
-            logging.debug("Both 'token' and 'smartsheet_client' were given in function parameters. \n" +
-                          "'smartsheet_client' will be ignored")
-
-        sheet = _get_from_request(token=token, id_=sheet_id, type_='sheet')
-    elif smartsheet_client:
-        sheet = smartsheet_client.Sheets.get_sheet(sheet_id).to_dict()
-
-    columns_dict = _get_columns_dict(sheet)  # {col['title']: col['id'] for col in sheet['columns']}
-    row_ids_list = [str(row['id']) for row in sheet['rows']]
-
-    if erase_sheet:
-        if row_ids_list:
-            logging.debug("Deleting rows from sheet")
-            if smartsheet_client:
-                smartsheet_client.Sheets.delete_rows(sheet_id, row_ids_list)
-            elif token:
-                _do_request(f"https://api.smartsheet.com/2.0/sheets/{sheet_id}/rows?ids={','.join(row_ids_list)}&ignoreRowsNotFound=true",
-                            token=token, method='DELETE')
-
-    add_columns_list = []
-    if insert_columns:
-        for col in df.columns.tolist():
-            if col != 'row_id' and col != 'parent_id':
-                if not columns_dict.get(col):
-                    # TODO: Create function to guess column type
-                    add_columns_list.append({'title': col, 'type': "TEXT_NUMBER", "index": len(columns_dict)})
-        else:
-            if add_columns_list:
-                if smartsheet_client:
-                    import smartsheet.models
-                    add_smartsheet_cols = [smartsheet.models.Column(col) for col in add_columns_list]
-                    smartsheet_client.Sheets.add_columns(sheet_id, add_smartsheet_cols)
-                elif token:
-                    _do_request(f"https://api.smartsheet.com/2.0/sheets/{sheet_id}/columns",
-                                token=token, method='POST', json=add_columns_list,
-                                options={"Content-Type": "application/json"})
-
-    for index, row in df.iterrows():
-        pass
-
-    print("pause")
-
-
 def _handle_object_value(object_value: dict) -> str:
     email_list_string: str = ""
     if object_value['objectType'].upper() == "MULTI_CONTACT":
         email_list_string = ', '.join(obj['email'] for obj in object_value['values'])
 
     return email_list_string
 
 
-def _get_columns_dict(sheet: dict) -> dict:
-    return {col['title']: {'id': col['id'],
-                           'type': col['type'],
-                           'index': col['index']} for col in sheet['columns']}
-
-
 class AuthenticationError(Exception):
     pass
```

