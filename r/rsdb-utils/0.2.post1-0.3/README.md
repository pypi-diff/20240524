# Comparing `tmp/rsdb_utils-0.2.post1.tar.gz` & `tmp/rsdb_utils-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsdb_utils-0.2.post1.tar", last modified: Wed May 22 15:32:41 2024, max compression
+gzip compressed data, was "rsdb_utils-0.3.tar", last modified: Fri May 24 15:27:56 2024, max compression
```

## Comparing `rsdb_utils-0.2.post1.tar` & `rsdb_utils-0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 15:32:41.957956 rsdb_utils-0.2.post1/
--rw-rw-r--   0 romain    (1000) romain    (1000)    35149 2023-06-19 14:21:45.000000 rsdb_utils-0.2.post1/LICENCE.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       54 2024-05-22 13:30:20.000000 rsdb_utils-0.2.post1/MANIFEST.in
--rw-r--r--   0 romain    (1000) romain    (1000)    45207 2024-05-22 15:32:41.957956 rsdb_utils-0.2.post1/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)     3602 2024-05-22 15:30:17.000000 rsdb_utils-0.2.post1/README.md
--rw-rw-r--   0 romain    (1000) romain    (1000)     1252 2024-05-22 15:32:31.000000 rsdb_utils-0.2.post1/pyproject.toml
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 15:32:41.957956 rsdb_utils-0.2.post1/rsdb_utils/
--rw-rw-r--   0 romain    (1000) romain    (1000)      279 2024-05-22 11:43:31.000000 rsdb_utils-0.2.post1/rsdb_utils/__init__.py
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 15:32:41.957956 rsdb_utils-0.2.post1/rsdb_utils/rsdb-schema/
--rw-rw-r--   0 romain    (1000) romain    (1000)    26502 2024-05-22 13:26:55.000000 rsdb_utils-0.2.post1/rsdb_utils/rsdb-schema/case_study_schema.json
--rw-rw-r--   0 romain    (1000) romain    (1000)     7324 2024-05-22 14:32:36.000000 rsdb_utils-0.2.post1/rsdb_utils/utils.py
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 15:32:41.957956 rsdb_utils-0.2.post1/rsdb_utils.egg-info/
--rw-r--r--   0 romain    (1000) romain    (1000)    45207 2024-05-22 15:32:41.000000 rsdb_utils-0.2.post1/rsdb_utils.egg-info/PKG-INFO
--rw-rw-r--   0 romain    (1000) romain    (1000)      321 2024-05-22 15:32:41.000000 rsdb_utils-0.2.post1/rsdb_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)        1 2024-05-22 15:32:41.000000 rsdb_utils-0.2.post1/rsdb_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       69 2024-05-22 15:32:41.000000 rsdb_utils-0.2.post1/rsdb_utils.egg-info/requires.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       11 2024-05-22 15:32:41.000000 rsdb_utils-0.2.post1/rsdb_utils.egg-info/top_level.txt
--rw-rw-r--   0 romain    (1000) romain    (1000)       38 2024-05-22 15:32:41.957956 rsdb_utils-0.2.post1/setup.cfg
-drwxrwxr-x   0 romain    (1000) romain    (1000)        0 2024-05-22 15:32:41.957956 rsdb_utils-0.2.post1/tests/
--rw-rw-r--   0 romain    (1000) romain    (1000)     3230 2024-05-22 11:43:22.000000 rsdb_utils-0.2.post1/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:27:56.569709 rsdb_utils-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-24 15:27:51.000000 rsdb_utils-0.3/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 15:27:51.000000 rsdb_utils-0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    45410 2024-05-24 15:27:56.569709 rsdb_utils-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-24 15:27:51.000000 rsdb_utils-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-24 15:27:51.000000 rsdb_utils-0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:27:56.569709 rsdb_utils-0.3/rsdb_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-24 15:27:51.000000 rsdb_utils-0.3/rsdb_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:27:56.569709 rsdb_utils-0.3/rsdb_utils/rsdb-schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    26474 2024-05-24 15:27:51.000000 rsdb_utils-0.3/rsdb_utils/rsdb-schema/case_study_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11717 2024-05-24 15:27:51.000000 rsdb_utils-0.3/rsdb_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:27:56.569709 rsdb_utils-0.3/rsdb_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45410 2024-05-24 15:27:56.000000 rsdb_utils-0.3/rsdb_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-24 15:27:56.000000 rsdb_utils-0.3/rsdb_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:27:56.000000 rsdb_utils-0.3/rsdb_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-24 15:27:56.000000 rsdb_utils-0.3/rsdb_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 15:27:56.000000 rsdb_utils-0.3/rsdb_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:27:56.569709 rsdb_utils-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:27:56.569709 rsdb_utils-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-24 15:27:51.000000 rsdb_utils-0.3/tests/tests.py
```

### Comparing `rsdb_utils-0.2.post1/LICENCE.txt` & `rsdb_utils-0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `rsdb_utils-0.2.post1/PKG-INFO` & `rsdb_utils-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsdb-utils
-Version: 0.2.post1
+Version: 0.3
 Summary: Utils to process the Regime Shifts DataBase CSV and parquet files
 Author-email: Romain Thomas <romain.thomas@su.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,14 +703,15 @@
 Utils to process the Regime Shifts DataBase CSV and parquet files.
 
 Functionalities:
 
   - Import the database from a CSV or parquet file in a pandas DataFrame
   - Save the database in a CSV or parquet file from a pandas DataFrame
   - Check the database (a DataFrame) with the json schema or the Regime Shifts DataBase
+  - From the JSON schema, generate a CSV with the list of enums values ([`tests/list_of_enums_from_json_schema`](https://github.com/regimeshifts/rsdb-utils/blob/main/tests/list_of_enums_from_json_schema.csv))
 
 Code repository: [https://github.com/regimeshifts/rsdb-utils](https://github.com/regimeshifts/rsdb-utils)
 
 Licence: GNU General Public License v3 (GPLv3)
 
 ## Installation
```

### Comparing `rsdb_utils-0.2.post1/README.md` & `rsdb_utils-0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Utils to process the Regime Shifts DataBase CSV and parquet files.
 
 Functionalities:
 
   - Import the database from a CSV or parquet file in a pandas DataFrame
   - Save the database in a CSV or parquet file from a pandas DataFrame
   - Check the database (a DataFrame) with the json schema or the Regime Shifts DataBase
+  - From the JSON schema, generate a CSV with the list of enums values ([`tests/list_of_enums_from_json_schema`](https://github.com/regimeshifts/rsdb-utils/blob/main/tests/list_of_enums_from_json_schema.csv))
 
 Code repository: [https://github.com/regimeshifts/rsdb-utils](https://github.com/regimeshifts/rsdb-utils)
 
 Licence: GNU General Public License v3 (GPLv3)
 
 ## Installation
```

### Comparing `rsdb_utils-0.2.post1/pyproject.toml` & `rsdb_utils-0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rsdb-utils"
-version = "0.2.post1"
+version = "0.3"
 description = "Utils to process the Regime Shifts DataBase CSV and parquet files"
 readme = "README.md"
 authors = [{ name = "Romain Thomas", email = "romain.thomas@su.se" }]
 license = {file = "LICENCE.txt"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `rsdb_utils-0.2.post1/rsdb_utils/rsdb-schema/case_study_schema.json` & `rsdb_utils-0.3/rsdb_utils/rsdb-schema/case_study_schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999834656084655%*

 * *Differences: {"'defs'": "{'regime_shift_type': {'then': {'properties': {'other': {delete: ['minLength']}}}}}"}*

```diff
@@ -517,15 +517,14 @@
             "required": [
                 "value"
             ],
             "then": {
                 "properties": {
                     "other": {
                         "maxLength": 100,
-                        "minLength": 1,
                         "type": [
                             "string",
                             "null"
                         ]
                     }
                 }
             },
```

### Comparing `rsdb_utils-0.2.post1/rsdb_utils.egg-info/PKG-INFO` & `rsdb_utils-0.3/rsdb_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsdb-utils
-Version: 0.2.post1
+Version: 0.3
 Summary: Utils to process the Regime Shifts DataBase CSV and parquet files
 Author-email: Romain Thomas <romain.thomas@su.se>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -703,14 +703,15 @@
 Utils to process the Regime Shifts DataBase CSV and parquet files.
 
 Functionalities:
 
   - Import the database from a CSV or parquet file in a pandas DataFrame
   - Save the database in a CSV or parquet file from a pandas DataFrame
   - Check the database (a DataFrame) with the json schema or the Regime Shifts DataBase
+  - From the JSON schema, generate a CSV with the list of enums values ([`tests/list_of_enums_from_json_schema`](https://github.com/regimeshifts/rsdb-utils/blob/main/tests/list_of_enums_from_json_schema.csv))
 
 Code repository: [https://github.com/regimeshifts/rsdb-utils](https://github.com/regimeshifts/rsdb-utils)
 
 Licence: GNU General Public License v3 (GPLv3)
 
 ## Installation
```

