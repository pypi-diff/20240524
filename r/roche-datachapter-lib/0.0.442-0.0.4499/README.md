# Comparing `tmp/roche_datachapter_lib-0.0.442.tar.gz` & `tmp/roche_datachapter_lib-0.0.4499.tar.gz`

## Comparing `roche_datachapter_lib-0.0.442.tar` & `roche_datachapter_lib-0.0.4499.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/requirements_for_build.txt
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/requirements_for_test.txt
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/setup_build_upload.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/__domain__.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/data_transformer.py
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/db_config.py
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/google_services.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/google_services_enums.py
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/job_manager.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/logger.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/query_manager.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/result_type.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/tests/simple_test.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/tests/test_db_config.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/tests/test_google_services.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/tests/test_job_manager.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/tests/test_query_manager.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/tests/test_redshift_connection.py
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/tests/queries/ej_godw.sql
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/tests/queries/ej_rexis.sql
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/tests/queries/ej_sap.sql
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/tests/queries/ej_sql_server.sql
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/tests/queries/stock_sap.sql
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/LICENSE
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/README.md
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/pyproject.toml
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.442/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/requirements_for_build.txt
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/requirements_for_test.txt
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/setup_build_upload.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/__domain__.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/data_transformer.py
+-rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/db_config.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/google_services.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/google_services_enums.py
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/job_manager.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/logger.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/query_manager.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/result_type.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/tests/simple_test.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/tests/test_db_config.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/tests/test_google_services.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/tests/test_job_manager.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/tests/test_query_manager.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/tests/test_redshift_connection.py
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/tests/queries/ej_godw.sql
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/tests/queries/ej_rexis.sql
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/tests/queries/ej_sap.sql
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/tests/queries/ej_sql_server.sql
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/tests/queries/stock_sap.sql
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/LICENSE
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/README.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/pyproject.toml
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 roche_datachapter_lib-0.0.4499/PKG-INFO
```

### Comparing `roche_datachapter_lib-0.0.442/setup_build_upload.py` & `roche_datachapter_lib-0.0.4499/setup_build_upload.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/__domain__.py` & `roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/__domain__.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/data_transformer.py` & `roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/data_transformer.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/db_config.py` & `roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/db_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
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
                  "NEXUS_HOST", "NEXUS_DB", "NEXUS_PORT", "NEXUS_USER", "NEXUS_PASSWORD",
-                 "RDI_LATAM_AR_USER", "RDI_LATAM_AR_PASSWORD", "RDI_LATAM_AR_HOST", "RDI_LATAM_AR_PORT", "RDI_LATAM_AR_DB"]
+                 "RDI_LATAM_AR_USER", "RDI_LATAM_AR_PASSWORD", "RDI_LATAM_AR_HOST",
+                 "RDI_LATAM_AR_PORT", "RDI_LATAM_AR_DB"]
 
 for env_var_name in ENV_VAR_NAMES:
     value = environ.get(env_var_name)
     if value is not None:
         globals()[env_var_name] = value
     else:
         raise EnvironmentError(
@@ -47,29 +49,44 @@
         'sqlserver_latam_ar_staging': f"{SQLSERVER_BASE}/{SQLSERVER_LATAM_AR_STAGING_DB}",  # pylint:disable=undefined-variable
         'sqlserver_latam_uy': f"{SQLSERVER_BASE}/{SQLSERVER_LATAM_UY_DB}",  # pylint:disable=undefined-variable
         'sqlserver_latam_uy_staging': f"{SQLSERVER_BASE}/{SQLSERVER_LATAM_UY_STAGING_DB}",  # pylint:disable=undefined-variable
         'godw': f"oracle+oracledb://{GODW_USER}:{GODW_PASSWORD}@{GODW_SERVER}:{GODW_PORT}/?service_name={GODW_SERVICENAME}",  # pylint:disable=undefined-variable
         'sapdwp06': f"hana+hdbcli://{SAPDWP06_USER}:{SAPDWP06_PASSWORD}@{SAPDWP06_SERVER}:{SAPDWP06_PORT}/{SAPDWP06_DB}?encrypt=true",  # pylint:disable=undefined-variable
         'rexis_sales': f"mssql+pymssql://@{REXIS_SALES_SERVER}/{REXIS_SALES_DB}",  # pylint:disable=undefined-variable
         'rexis_services': f"mssql+pymssql://@{REXIS_SERVICES_SERVER}/{REXIS_SERVICES_DB}",  # pylint:disable=undefined-variable
-        'nexus_prod': f"mysql+pymysql://{NEXUS_USER}:{NEXUS_PASSWORD}@{NEXUS_HOST}:{NEXUS_PORT}/{NEXUS_DB}",  # pylint:disable=undefined-variable
-        'rdi_latam_ar': f"postgresql+psycopg2://{RDI_LATAM_AR_USER}:{RDI_LATAM_AR_PASSWORD}@{RDI_LATAM_AR_HOST}:{RDI_LATAM_AR_PORT}/{RDI_LATAM_AR_DB}?sslmode=disable"  # pylint:disable=undefined-variable
+        'nexus_prod': f"mysql+pymysql://{NEXUS_USER}:{NEXUS_PASSWORD}@{NEXUS_HOST}:{NEXUS_PORT}/{NEXUS_DB}"  # pylint:disable=undefined-variable
     }
 
     @classmethod
     def __get_bind__(cls, bind: str = ''):
-        return cls.SQLALCHEMY_BINDS[cls.validate_bind(bind.lower())]
+        return cls.SQLALCHEMY_BINDS[cls.validate_bind(bind)]
 
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
@@ -86,22 +103,25 @@
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
```

### Comparing `roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/google_services.py` & `roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/google_services.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/job_manager.py` & `roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/job_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/logger.py` & `roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/logger.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/src/roche_datachapter_lib/query_manager.py` & `roche_datachapter_lib-0.0.4499/src/roche_datachapter_lib/query_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/tests/test_google_services.py` & `roche_datachapter_lib-0.0.4499/tests/test_google_services.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/tests/test_job_manager.py` & `roche_datachapter_lib-0.0.4499/tests/test_job_manager.py`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/tests/test_redshift_connection.py` & `roche_datachapter_lib-0.0.4499/tests/test_redshift_connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import os
 from sqlalchemy import create_engine
+import sqlalchemy as sa
+from sqlalchemy.engine.url import URL
+import os
 
 # Cargar las variables de entorno
 USER = os.getenv('RDI_LATAM_AR_USER')
 PASSWORD = os.getenv('RDI_LATAM_AR_PASSWORD')
 HOST = os.getenv('RDI_LATAM_AR_HOST')
 PORT = os.getenv('RDI_LATAM_AR_PORT')
 DB = os.getenv('RDI_LATAM_AR_DB')
 
+
+
 # Crear la cadena de conexión con sslmode deshabilitado
 connection_string = f'redshift+psycopg2://{USER}:{PASSWORD}@{HOST}:{PORT}/{DB}?sslmode=disable'
-DATABASE_URL = f"postgresql+psycopg2://{USER}:{PASSWORD}@{HOST}:{PORT}/{DB}?sslmode=disable"
+DATABASE_URL = f"redshift+psycopg2://{USER}:{PASSWORD}@{HOST}:{PORT}/{DB}"
 # Crear el motor de SQLAlchemy
-engine = create_engine(DATABASE_URL)
+engine = create_engine(DATABASE_URL,connect_args={
+        "sslmode": "require",
+        "iam": True,
+    })
 
 # Probar la conexión (opcional)
 try:
     with engine.connect() as connection:
         result = connection.execute("SELECT * FROM gtm_latam_arg.stg_oceo.oceo_omuser_latest")
         for row in result:
             print(row)
```

### Comparing `roche_datachapter_lib-0.0.442/tests/queries/ej_godw.sql` & `roche_datachapter_lib-0.0.4499/tests/queries/ej_godw.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/tests/queries/ej_sap.sql` & `roche_datachapter_lib-0.0.4499/tests/queries/ej_sap.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/tests/queries/ej_sql_server.sql` & `roche_datachapter_lib-0.0.4499/tests/queries/ej_sql_server.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/tests/queries/stock_sap.sql` & `roche_datachapter_lib-0.0.4499/tests/queries/stock_sap.sql`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/.gitignore` & `roche_datachapter_lib-0.0.4499/.gitignore`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/LICENSE` & `roche_datachapter_lib-0.0.4499/LICENSE`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/README.md` & `roche_datachapter_lib-0.0.4499/README.md`

 * *Files identical despite different names*

### Comparing `roche_datachapter_lib-0.0.442/PKG-INFO` & `roche_datachapter_lib-0.0.4499/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.3
 Name: roche_datachapter_lib
-Version: 0.0.442
+Version: 0.0.4499
 Summary: Esta biblioteca de código esta pensada para compartir funcionalidades entre todos los procesos ETL que desarrollemos con Python
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Lucas Frías <lucasmatiasfrias@live.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Requires-Dist: chardet==5.2.0
 Requires-Dist: flask-sqlalchemy==3.0.3
-Requires-Dist: flask==3.0.3
+Requires-Dist: flask==2.3.1
 Requires-Dist: google-api-python-client==2.99.0
 Requires-Dist: google-auth-httplib2==0.1.1
 Requires-Dist: google-auth-oauthlib==1.1.0
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: oracledb==2.0.0
 Requires-Dist: pandas==2.1.3
-Requires-Dist: pkginfo
-Requires-Dist: psycopg2==2.9.9
-Requires-Dist: pymssql==2.3.0
-Requires-Dist: pymysql==1.1.1
+Requires-Dist: psycopg
+Requires-Dist: pymssql
+Requires-Dist: pymysql==1.1.0
 Requires-Dist: pyodbc==5.0.1
-Requires-Dist: setuptools
+Requires-Dist: requests==2.31.0
 Requires-Dist: sqlalchemy-hana==1.1.1
-Requires-Dist: sqlalchemy==2.0.0
+Requires-Dist: sqlalchemy==2.0.30
 Description-Content-Type: text/markdown
 
 # Roche Data Chapeter LIB
 
 ## Description
 It contains the base structure that includes the configuration parameters of the different databases using environment variables on the server, a static data_transformer class to perform the data transformation and another static class to perform connection to Google services through the Google REST API.
```

