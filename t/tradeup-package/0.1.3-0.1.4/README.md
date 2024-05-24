# Comparing `tmp/tradeup_package-0.1.3.tar.gz` & `tmp/tradeup_package-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradeup_package-0.1.3.tar", last modified: Thu May  9 15:36:54 2024, max compression
+gzip compressed data, was "tradeup_package-0.1.4.tar", last modified: Fri May 24 18:49:54 2024, max compression
```

## Comparing `tradeup_package-0.1.3.tar` & `tradeup_package-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-09 15:36:54.686897 tradeup_package-0.1.3/
--rw-rw-r--   0 script.master  (1001) script.master  (1001)     1068 2024-04-26 19:46:29.000000 tradeup_package-0.1.3/LICENSE
--rw-r--r--   0 script.master  (1001) script.master  (1001)      281 2024-05-09 15:36:54.686897 tradeup_package-0.1.3/PKG-INFO
--rw-rw-r--   0 script.master  (1001) script.master  (1001)     1131 2024-05-09 15:33:22.000000 tradeup_package-0.1.3/README.md
--rw-rw-r--   0 script.master  (1001) script.master  (1001)      323 2024-05-09 15:31:52.000000 tradeup_package-0.1.3/pyproject.toml
--rw-rw-r--   0 script.master  (1001) script.master  (1001)       38 2024-05-09 15:36:54.686897 tradeup_package-0.1.3/setup.cfg
-drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-09 15:36:54.686897 tradeup_package-0.1.3/tradeup/
--rw-rw-r--   0 script.master  (1001) script.master  (1001)     6193 2024-05-08 13:36:19.000000 tradeup_package-0.1.3/tradeup/Public.py
--rw-rw-r--   0 script.master  (1001) script.master  (1001)       21 2023-10-04 18:16:32.000000 tradeup_package-0.1.3/tradeup/__init__.py
-drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-09 15:36:54.686897 tradeup_package-0.1.3/tradeup_package.egg-info/
--rw-r--r--   0 script.master  (1001) script.master  (1001)      281 2024-05-09 15:36:54.000000 tradeup_package-0.1.3/tradeup_package.egg-info/PKG-INFO
--rw-rw-r--   0 script.master  (1001) script.master  (1001)      226 2024-05-09 15:36:54.000000 tradeup_package-0.1.3/tradeup_package.egg-info/SOURCES.txt
--rw-rw-r--   0 script.master  (1001) script.master  (1001)        1 2024-05-09 15:36:54.000000 tradeup_package-0.1.3/tradeup_package.egg-info/dependency_links.txt
--rw-rw-r--   0 script.master  (1001) script.master  (1001)        8 2024-05-09 15:36:54.000000 tradeup_package-0.1.3/tradeup_package.egg-info/top_level.txt
+drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-24 18:49:54.552498 tradeup_package-0.1.4/
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)     1068 2024-04-26 19:46:29.000000 tradeup_package-0.1.4/LICENSE
+-rw-r--r--   0 script.master  (1001) script.master  (1001)      281 2024-05-24 18:49:54.552498 tradeup_package-0.1.4/PKG-INFO
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)     1241 2024-05-24 18:48:56.000000 tradeup_package-0.1.4/README.md
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)      323 2024-05-24 18:49:01.000000 tradeup_package-0.1.4/pyproject.toml
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)       38 2024-05-24 18:49:54.552498 tradeup_package-0.1.4/setup.cfg
+drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-24 18:49:54.548498 tradeup_package-0.1.4/tradeup/
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)     6555 2024-05-24 18:43:42.000000 tradeup_package-0.1.4/tradeup/Public.py
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)       21 2023-10-04 18:16:32.000000 tradeup_package-0.1.4/tradeup/__init__.py
+drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-24 18:49:54.552498 tradeup_package-0.1.4/tradeup_package.egg-info/
+-rw-r--r--   0 script.master  (1001) script.master  (1001)      281 2024-05-24 18:49:54.000000 tradeup_package-0.1.4/tradeup_package.egg-info/PKG-INFO
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)      226 2024-05-24 18:49:54.000000 tradeup_package-0.1.4/tradeup_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)        1 2024-05-24 18:49:54.000000 tradeup_package-0.1.4/tradeup_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)        8 2024-05-24 18:49:54.000000 tradeup_package-0.1.4/tradeup_package.egg-info/top_level.txt
```

### Comparing `tradeup_package-0.1.3/LICENSE` & `tradeup_package-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tradeup_package-0.1.3/README.md` & `tradeup_package-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,8 +19,11 @@
 Release note 0.1.1   2024/05/02 10:59
 Defined all functions under class Amazon as static method, no need to include argument 'self' when calling functions
 
 Release note 0.1.2   2024/05/02 15:20
 Excluded all 'self' under class amazon
 
 ## Release note 0.1.3   2024/05/09 11:32
-Minor bug fix, correct typos in check_holiday()
+Minor bug fix, correct typos in check_holiday()
+
+## Release note 0.1.4   2024/05/24 14:46
+Based on use cases, assign individual connection to check_holiday()
```

### Comparing `tradeup_package-0.1.3/tradeup/Public.py` & `tradeup_package-0.1.4/tradeup/Public.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,22 +120,29 @@
         except ClientError as e:
             raise e
     
         password = get_secret_value_response['SecretString']
         return password    
     
     @staticmethod
-    def check_holiday(date_obj, con, which='NYSE_Holiday'):
+    def check_holiday(date_obj, which='NYSE_Holiday'):
+        connection = ast.literal_eval(amazon.get_secret(secret_name = "tradeup-redshift-prod", region_name = 'us-east-1'))
         date_str = date_obj.strftime("%Y-%m-%d")
-        df = wr.redshift.read_sql_query(
-            sql=f"""
-                SELECT "{which}" FROM holiday.holiday WHERE date ='{date_str}'
-                """,
-            con=con
-        )
+        with redshift_connector.connect(
+            host= connection['host'],
+            database='tradeup_eod',
+            user=connection['username'],
+            password=connection['password']
+        ) as con:  
+            df = wr.redshift.read_sql_query(
+                sql=f"""
+                    SELECT "{which}" FROM holiday.holiday WHERE date ='{date_str}'
+                    """,
+                con=con
+            )
         
         # not in holiday list
         if len(df) == 0:
             return False
         
         # in holiday list and decide
         if df.iloc[0,0] == 1:
```

