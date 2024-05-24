# Comparing `tmp/database_mysql_local-0.0.324.tar.gz` & `tmp/database_mysql_local-0.0.325.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.324.tar", last modified: Thu May 23 18:04:12 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.325.tar", last modified: Fri May 24 07:23:55 2024, max compression
```

## Comparing `database_mysql_local-0.0.324.tar` & `database_mysql_local-0.0.325.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:12.444633 database_mysql_local-0.0.324/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 18:04:12.444633 database_mysql_local-0.0.324/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:12.440633 database_mysql_local-0.0.324/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:12.444633 database_mysql_local-0.0.324/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53208 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30337 2024-05-23 18:03:40.000000 database_mysql_local-0.0.324/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/table_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)   630215 2024-05-23 18:03:38.000000 database_mysql_local-0.0.324/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-23 18:03:13.000000 database_mysql_local-0.0.324/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:04:12.444633 database_mysql_local-0.0.324/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 18:04:12.000000 database_mysql_local-0.0.324/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-23 18:04:12.000000 database_mysql_local-0.0.324/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:04:12.000000 database_mysql_local-0.0.324/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-23 18:04:12.000000 database_mysql_local-0.0.324/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 18:04:12.000000 database_mysql_local-0.0.324/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 18:03:40.000000 database_mysql_local-0.0.324/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:04:12.444633 database_mysql_local-0.0.324/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 18:03:40.000000 database_mysql_local-0.0.324/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:23:55.921397 database_mysql_local-0.0.325/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-24 07:23:55.921397 database_mysql_local-0.0.325/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:23:55.913397 database_mysql_local-0.0.325/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:23:55.921397 database_mysql_local-0.0.325/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53663 2024-05-24 07:23:21.000000 database_mysql_local-0.0.325/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30337 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238517 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/database_mysql_local/src/table_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   630215 2024-05-24 07:23:21.000000 database_mysql_local-0.0.325/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-05-24 07:23:21.000000 database_mysql_local-0.0.325/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:23:55.921397 database_mysql_local-0.0.325/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-24 07:23:55.000000 database_mysql_local-0.0.325/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-24 07:23:55.000000 database_mysql_local-0.0.325/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:23:55.000000 database_mysql_local-0.0.325/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-24 07:23:55.000000 database_mysql_local-0.0.325/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 07:23:55.000000 database_mysql_local-0.0.325/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-24 07:22:55.000000 database_mysql_local-0.0.325/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 07:23:55.921397 database_mysql_local-0.0.325/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-24 07:23:21.000000 database_mysql_local-0.0.325/setup.py
```

### Comparing `database_mysql_local-0.0.324/PKG-INFO` & `database_mysql_local-0.0.325/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.324
+Version: 0.0.325
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.324/README.md` & `database_mysql_local-0.0.325/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.325/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.325/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.325/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.325/database_mysql_local/src/generic_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,27 +220,35 @@
         finally:
             self.default_schema_name = old_schema_name
             self.logger.debug(object=locals())
         return table_id
 
     def _get_existing_duplicate_id(self, schema_name: str, table_name: str, error: Exception) -> int or None:
         """Error examples:
-        - Duplicate entry 'test@gmail.com' for key 'email_address_table.email_address.unique'
         - Duplicate entry '1' for key 'test_mysql_table.PRIMARY'
-        - Duplicate entry '7263200721327371865' for key 'test_mysql_table.number_UNIQUE"""
+        - Duplicate entry '7263200721327371865' for key 'test_mysql_table.number_UNIQUE
+        - Duplicate entry 'test@gmail.com' for key 'email_address_table.email_address.unique'
+        - 1062 (23000): Duplicate entry 'tal@circlez.ai' for key 'person_table.person_table.main_email_person.unique'"""
+        # When inserting a deleted entity and insert_is_undelete=false, we should null all the unique fields of the deleted entity
+
         pattern = r'Duplicate entry \'(.+?)\' for key \'(.+?)\''
         match = re.search(pattern, str(error))
         if not match:  # a different error
             raise error
         duplicate_value = match.group(1)
-        duplicate_column_name = match.group(2).split('.')[1]
-        if duplicate_column_name == "PRIMARY":
+        key = match.group(2)
+        if key.endswith("PRIMARY"):
             return int(duplicate_value)
-        if duplicate_column_name.endswith("_UNIQUE"):
-            duplicate_column_name = duplicate_column_name.split('_')[0]
+        elif key.endswith("_UNIQUE"):
+            duplicate_column_name = key.split(".")[-1].split('_')[0]
+        elif key.count(".") > 1:
+            duplicate_column_name = key.split(".")[-2]
+        else:
+            raise Exception(f"GenericCRUD._get_existing_duplicate_id: please report the following error,"
+                            f" so we can add support to this case: insert error: {error}")
 
         column_name = self.get_primary_key(schema_name=schema_name, table_name=table_name)
         if not column_name:
             raise error  # Column name for constraint not found
         select_query = f"SELECT {column_name} FROM `{schema_name}`.`{table_name}` WHERE {duplicate_column_name} = %s LIMIT 1;"
         self.connection.commit()
         self.cursor.execute(select_query, (duplicate_value,))
@@ -713,15 +721,15 @@
             if arg_name in ("self", "__class__"):
                 continue
             elif arg_name in required_args and not arg_value:
                 message = f"Invalid value for {arg_name}: {arg_value}"
             elif arg_name == "table_name":
                 validate_none_select_table_name(arg_value)
             elif arg_name == "view_table_name":
-                validate_select_table_name(database_object_name=arg_value, is_test_data=self.is_test_data)
+                validate_select_table_name(database_object_name=arg_value)
 
             # data_dict values are allowed to contain ';', as we use them with %s (TODO: unless it's ToSQLInterface)
             if ((arg_name.startswith("data_") and arg_value and any(
                     ";" in str(x) for x in arg_value.keys())) or  # check columns
                     (not arg_name.startswith("data_") and arg_name != "params" and ";" in str(arg_value))):
                 message = f"Invalid value for {arg_name}: {arg_value} (contains ';')"
```

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.325/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.325/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/point.py` & `database_mysql_local-0.0.325/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.325/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.325/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/table_columns.py` & `database_mysql_local-0.0.325/database_mysql_local/src/table_columns.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.325/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.325/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.325/database_mysql_local/src/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from url_remote.environment_name_enum import EnvironmentName
 
 from .table_columns import table_columns
 from .table_definition import table_definition
 from .to_sql_interface import ToSQLInterface
 
 
-def validate_select_table_name(database_object_name: str, is_test_data: bool = False) -> None:
+def validate_select_table_name(database_object_name: str) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
-            and not database_object_name.endswith("_view") and not is_test_data):
+            and not database_object_name.endswith("_view")):
         raise Exception(
             f"View name must end with '_view' in this environment (got {database_object_name})")
 
 
 def validate_none_select_table_name(database_object_name: str) -> None:
     if (get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value)
             and not database_object_name.endswith("_table")):
```

### Comparing `database_mysql_local-0.0.324/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.325/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.324
+Version: 0.0.325
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.324/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.325/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/pyproject.toml` & `database_mysql_local-0.0.325/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.324/setup.py` & `database_mysql_local-0.0.325/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.324',
+    version='0.0.325',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

