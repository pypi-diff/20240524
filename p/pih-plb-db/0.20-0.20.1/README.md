# Comparing `tmp/pih-plb_db-0.20.tar.gz` & `tmp/pih-plb_db-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_db-0.20.tar", last modified: Mon May 20 23:11:58 2024, max compression
+gzip compressed data, was "pih-plb_db-0.20.1.tar", last modified: Fri May 24 14:57:58 2024, max compression
```

## Comparing `pih-plb_db-0.20.tar` & `pih-plb_db-0.20.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 23:11:58.464148 pih-plb_db-0.20/
--rw-rw-rw-   0        0        0      280 2024-05-20 23:11:58.429873 pih-plb_db-0.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 23:11:57.721544 pih-plb_db-0.20/PolibaseDatabaseService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.20/PolibaseDatabaseService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.20/PolibaseDatabaseService/__main__.py
--rw-rw-rw-   0        0        0    10898 2024-05-20 22:38:27.000000 pih-plb_db-0.20/PolibaseDatabaseService/api.py
--rw-rw-rw-   0        0        0     1052 2024-05-20 22:38:38.000000 pih-plb_db-0.20/PolibaseDatabaseService/const.py
--rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.20/PolibaseDatabaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-20 23:11:58.398626 pih-plb_db-0.20/pih_plb_db.egg-info/
--rw-rw-rw-   0        0        0      280 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-20 23:11:57.000000 pih-plb_db-0.20/pih_plb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 23:11:58.466147 pih-plb_db-0.20/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 14:57:58.630343 pih-plb_db-0.20.1/
+-rw-rw-rw-   0        0        0      282 2024-05-24 14:57:58.599092 pih-plb_db-0.20.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 14:57:58.223055 pih-plb_db-0.20.1/PolibaseDatabaseService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.20.1/PolibaseDatabaseService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.20.1/PolibaseDatabaseService/__main__.py
+-rw-rw-rw-   0        0        0    10928 2024-05-24 14:56:42.000000 pih-plb_db-0.20.1/PolibaseDatabaseService/api.py
+-rw-rw-rw-   0        0        0     1082 2024-05-24 14:57:08.000000 pih-plb_db-0.20.1/PolibaseDatabaseService/const.py
+-rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.20.1/PolibaseDatabaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-24 14:57:58.552223 pih-plb_db-0.20.1/pih_plb_db.egg-info/
+-rw-rw-rw-   0        0        0      282 2024-05-24 14:57:57.000000 pih-plb_db-0.20.1/pih_plb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-24 14:57:57.000000 pih-plb_db-0.20.1/pih_plb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 14:57:57.000000 pih-plb_db-0.20.1/pih_plb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-24 14:57:57.000000 pih-plb_db-0.20.1/pih_plb_db.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-24 14:57:57.000000 pih-plb_db-0.20.1/pih_plb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-24 14:57:57.000000 pih-plb_db-0.20.1/pih_plb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 14:57:58.630343 pih-plb_db-0.20.1/setup.cfg
```

### Comparing `pih-plb_db-0.20/PolibaseDatabaseService/api.py` & `pih-plb_db-0.20.1/PolibaseDatabaseService/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,24 +42,24 @@
             file_name, DATABASE_DUMP.FILE_EXTENSION
         )
         if test:
             polibase_folder_path_src: str = polibase_folder_path
             polibase_folder_path = A.PTH.for_windows(
                 A.PTH.join(polibase_folder_path, TEST_NAME)
             )
-            os.system(
+            A.L.debug_bot(js(("test:", os.system(
                 js(
                     (
                         "robocopy",
                         A.PTH.join(polibase_folder_path_src, STUB_DIRECTORY_NAME),
                         polibase_folder_path,
                         file_database_dump_name_out,
                     )
                 )
-            )
+            ))))
         polibase2_folder_path: str = A.PTH.for_windows(
             A.PTH.join(A.CT_H.POLIBASE2.NAME, local_polibase_database_dump_folder_name)
         )
 
         archiver_program_path: str = 'C:/"Program Files"/7-Zip/7z'
 
         file_out_name = A.PTH.add_extension(file_name, ARCHIVE_TYPE)
```

### Comparing `pih-plb_db-0.20/PolibaseDatabaseService/const.py` & `pih-plb_db-0.20.1/PolibaseDatabaseService/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "PolibaseDatabase"
 
 HOST = A.CT_H.POLIBASE
 
-VERSION: str = "0.20"
+VERSION: str = "0.20.1"
 
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     host=HOST.NAME,
     description="Polibase database service",
     commands=("create_polibase_database_backup",),
     version=VERSION,
     use_standalone=True,
     standalone_name="plb_db",
+    host_changeable=False,
     run_from_system_account=True,
     python_executable_path=CONST.UNKNOWN_VALUE,
 )
 
 TEST_NAME: str = "test"
 STUB_DIRECTORY_NAME: str = "stub"
 #
```

### Comparing `pih-plb_db-0.20/PolibaseDatabaseService/service.py` & `pih-plb_db-0.20.1/PolibaseDatabaseService/service.py`

 * *Files identical despite different names*

