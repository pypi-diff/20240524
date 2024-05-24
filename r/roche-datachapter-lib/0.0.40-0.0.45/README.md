# Comparing `tmp/roche_datachapter_lib-0.0.40.tar.gz` & `tmp/roche_datachapter_lib-0.0.45.tar.gz`

## Comparing `roche_datachapter_lib-0.0.40.tar` & `roche_datachapter_lib-0.0.45.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/requirements_for_build.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/requirements_for_test.txt
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/setup_build_upload.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/__domain__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/data_transformer.py
--rw-r--r--   0        0        0     7402 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/db_config.py
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/google_services.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/google_services_enums.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/job_manager.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/logger.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/query_manager.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/result_type.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/simple_test.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/test_db_config.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/test_google_services.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/test_job_manager.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/test_query_manager.py
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/queries/ej_godw.sql
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/queries/ej_rexis.sql
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/queries/ej_sap.sql
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/queries/ej_sql_server.sql
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/tests/queries/stock_sap.sql
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/LICENSE
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/pyproject.toml
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.40/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/requirements_for_build.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/requirements_for_test.txt
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/setup_build_upload.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/__domain__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/data_transformer.py
+-rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/db_config.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/google_services.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/google_services_enums.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/job_manager.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/logger.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/query_manager.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/result_type.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/tests/simple_test.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/tests/test_db_config.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/tests/test_google_services.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/tests/test_job_manager.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/tests/test_query_manager.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/tests/test_redshift_connection.py
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/tests/queries/ej_godw.sql
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/tests/queries/ej_rexis.sql
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/tests/queries/ej_sap.sql
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/tests/queries/ej_sql_server.sql
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/tests/queries/stock_sap.sql
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/LICENSE
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/README.md
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/pyproject.toml
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.45/PKG-INFO
```

### Comparing `roche_datachapter_lib-0.0.40/setup_build_upload.py` & `roche_datachapter_lib-0.0.45/setup_build_upload.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/__domain__.py` & `roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/__domain__.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/data_transformer.py` & `roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/data_transformer.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/db_config.py` & `roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/db_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """All Database configurations and methods"""
 from typing import List, Dict, Any
 from os import environ
 import pandas
+import psycopg
 from sqlalchemy import create_engine
 from sqlalchemy.sql import text
 from sqlalchemy.exc import OperationalError
 from .result_type import ResultType
 
 ENV_VAR_NAMES = ["SQLSERVER_SERVER", "SQLSERVER_USER", "SQLSERVER_PWD",
                  "SQLSERVER_LATAM_AR_DB", "SQLSERVER_LATAM_AR_DEV_DB",
                  "SQLSERVER_LATAM_AR_FARMADB_DB", "SQLSERVER_LATAM_AR_SAND_DB",
                  "SQLSERVER_LATAM_AR_STAGING_DB", "SQLSERVER_LATAM_UY_DB",
                  "SQLSERVER_LATAM_UY_STAGING_DB", "GODW_SERVER", "GODW_PORT",
                  "GODW_USER", "GODW_PASSWORD", "GODW_SERVICENAME", "GODW_ORACLE_INSTANT_CLIENT_PATH",
                  "SAPDWP06_SERVER", "SAPDWP06_PORT", "SAPDWP06_USER", "SAPDWP06_PASSWORD", "SAPDWP06_DB",
                  "REXIS_SALES_SERVER", "REXIS_SALES_DB", "REXIS_SERVICES_SERVER", "REXIS_SERVICES_DB",
-                 "NEXUS_HOST", "NEXUS_DB", "NEXUS_PORT", "NEXUS_USER", "NEXUS_PASSWORD"]
+                 "NEXUS_HOST", "NEXUS_DB", "NEXUS_PORT", "NEXUS_USER", "NEXUS_PASSWORD",
+                 "RDI_LATAM_AR_USER", "RDI_LATAM_AR_PASSWORD", "RDI_LATAM_AR_HOST",
+                 "RDI_LATAM_AR_PORT", "RDI_LATAM_AR_DB"]
 
 for env_var_name in ENV_VAR_NAMES:
     value = environ.get(env_var_name)
     if value is not None:
         globals()[env_var_name] = value
     else:
         raise EnvironmentError(
@@ -60,14 +63,30 @@
     @classmethod
     def __check_select_query__(cls, query: str = ''):
         if not query.lower().strip().startswith("select"):
             raise ValueError(f'NOT SELECT query: "{query[:100].strip().replace(
                 '\n', ' ').replace('\t', ' ').replace('  ', ' ')}..."')
 
     @classmethod
+    def __execute_select_query_on_rdi__(cls, query: str = '') -> pandas.DataFrame:
+        df = pandas.DataFrame()
+        try:
+            str_conn = f"dbname='{RDI_LATAM_AR_DB}' user='{RDI_LATAM_AR_USER}' password='{RDI_LATAM_AR_PASSWORD}' host='{
+                RDI_LATAM_AR_HOST}' port='{RDI_LATAM_AR_PORT}'"  # pylint:disable=undefined-variable
+            with psycopg.connect(str_conn, options='-c client_encoding=UTF8') as conn:
+                with conn.cursor() as cursor:
+                    cursor.execute(query)
+                    result = cursor.fetchall()
+                    colnames = [desc[0] for desc in cursor.description]
+                    df = pandas.DataFrame(result, columns=colnames)
+        except psycopg.Error as e:
+            print(f"Error al ejecutar la consulta en RDI: {e}")
+        return df
+
+    @classmethod
     def validate_bind(cls, bind: str = ''):
         """Bind validation"""
         if bind in cls.SQLALCHEMY_BINDS:
             return bind
         available_binds = ', '.join(
             f"{key}" for key in cls.SQLALCHEMY_BINDS)
         raise ValueError(
@@ -84,22 +103,25 @@
             return False
         return False
 
     @classmethod
     def execute_custom_select_query(cls, query: str, p_bind: str, result_set_as: ResultType = ResultType.PANDAS_DATA_FRAME) -> pandas.DataFrame | List[Dict[str, Any]]:
         """Execute SQL SELECT query on specific bind and return result set as a pandas DataFrame"""
         cls.__check_select_query__(query)
-        df = pandas.DataFrame()
-        engine = create_engine(cls.__get_bind__(p_bind))
-        with engine.connect() as connection:
-            result = connection.execute(text(query))
-            all_rows = result.fetchall()
-            if len(all_rows) > 0:
-                df = pandas.DataFrame.from_records(
-                    all_rows, columns=result.keys())
+        if p_bind.lower() == 'rdi_latam_ar':
+            df = cls.__execute_select_query_on_rdi__(query)
+        else:
+            df = pandas.DataFrame()
+            engine = create_engine(cls.__get_bind__(p_bind))
+            with engine.connect() as connection:
+                result = connection.execute(text(query))
+                all_rows = result.fetchall()
+                if len(all_rows) > 0:
+                    df = pandas.DataFrame.from_records(
+                        all_rows, columns=result.keys())
         if result_set_as == ResultType.JSON_LIST:
             df = df.to_dict(orient='records')
         return df
 
     @classmethod
     def execute_stored_procedure(cls, sp_name: str, sp_params: dict = None, p_bind: str = 'sqlserver_master'):
         """Execute SQL query on specific bind and return result set as a dictionary"""
@@ -121,17 +143,17 @@
                         print(type(valor))
                         input(valor)
                         raise ValueError(
                             "sp_params only accept dict of int, float, bool or str")
                 sql_string += ', '.join(params)
             connection.execute(text(sql_string))
             connection.commit()
-            
+
     @classmethod
-    def truncate_table(cls, p_bind: str, schema: str, table:str):
+    def truncate_table(cls, p_bind: str, schema: str, table: str):
         """Truncate specific table from specific bind"""
         engine = create_engine(cls.__get_bind__(p_bind))
         with engine.connect() as connection:
             sql_string = f"TRUNCATE TABLE [{str(schema)}].[{str(table)}]"
             connection.execute(text(sql_string))
             connection.commit()
             return True
```

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/google_services.py` & `roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/google_services.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/job_manager.py` & `roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/job_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/logger.py` & `roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/logger.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/src/roche_datachapter_lib/query_manager.py` & `roche_datachapter_lib-0.0.45/src/roche_datachapter_lib/query_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/test_google_services.py` & `roche_datachapter_lib-0.0.45/tests/test_google_services.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/test_job_manager.py` & `roche_datachapter_lib-0.0.45/tests/test_job_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/queries/ej_godw.sql` & `roche_datachapter_lib-0.0.45/tests/queries/ej_godw.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/queries/ej_sap.sql` & `roche_datachapter_lib-0.0.45/tests/queries/ej_sap.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/queries/ej_sql_server.sql` & `roche_datachapter_lib-0.0.45/tests/queries/ej_sql_server.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/tests/queries/stock_sap.sql` & `roche_datachapter_lib-0.0.45/tests/queries/stock_sap.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/.gitignore` & `roche_datachapter_lib-0.0.45/.gitignore`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/LICENSE` & `roche_datachapter_lib-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/README.md` & `roche_datachapter_lib-0.0.45/README.md`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.40/PKG-INFO` & `roche_datachapter_lib-0.0.45/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: roche_datachapter_lib
-Version: 0.0.40
+Version: 0.0.45
 Summary: Esta biblioteca de código esta pensada para compartir funcionalidades entre todos los procesos ETL que desarrollemos con Python
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Lucas Frías <lucasmatiasfrias@live.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,18 +15,23 @@
 Requires-Dist: flask==2.3.1
 Requires-Dist: google-api-python-client==2.99.0
 Requires-Dist: google-auth-httplib2==0.1.1
 Requires-Dist: google-auth-oauthlib==1.1.0
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: oracledb==2.0.0
 Requires-Dist: pandas==2.1.3
+Requires-Dist: psycopg
+Requires-Dist: psycopg-binary
+Requires-Dist: psycopg-c
 Requires-Dist: pymssql
 Requires-Dist: pymysql==1.1.0
 Requires-Dist: pyodbc==5.0.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: sqlalchemy-hana==1.1.1
+Requires-Dist: sqlalchemy==2.0.30
 Description-Content-Type: text/markdown
 
 # Roche Data Chapeter LIB
 
 ## Description
 It contains the base structure that includes the configuration parameters of the different databases using environment variables on the server, a static data_transformer class to perform the data transformation and another static class to perform connection to Google services through the Google REST API.
```

