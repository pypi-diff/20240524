# Comparing `tmp/pih-plb_db-0.20.2.tar.gz` & `tmp/pih-plb_db-0.20.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_db-0.20.2.tar", last modified: Fri May 24 15:05:15 2024, max compression
+gzip compressed data, was "pih-plb_db-0.20.3.tar", last modified: Fri May 24 15:19:40 2024, max compression
```

## Comparing `pih-plb_db-0.20.2.tar` & `pih-plb_db-0.20.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 15:05:15.851422 pih-plb_db-0.20.2/
--rw-rw-rw-   0        0        0      282 2024-05-24 15:05:15.820173 pih-plb_db-0.20.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-24 15:05:15.424459 pih-plb_db-0.20.2/PolibaseDatabaseService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.20.2/PolibaseDatabaseService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.20.2/PolibaseDatabaseService/__main__.py
--rw-rw-rw-   0        0        0    11337 2024-05-24 15:04:47.000000 pih-plb_db-0.20.2/PolibaseDatabaseService/api.py
--rw-rw-rw-   0        0        0     1082 2024-05-24 15:04:55.000000 pih-plb_db-0.20.2/PolibaseDatabaseService/const.py
--rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.20.2/PolibaseDatabaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-24 15:05:15.773306 pih-plb_db-0.20.2/pih_plb_db.egg-info/
--rw-rw-rw-   0        0        0      282 2024-05-24 15:05:14.000000 pih-plb_db-0.20.2/pih_plb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-24 15:05:14.000000 pih-plb_db-0.20.2/pih_plb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 15:05:14.000000 pih-plb_db-0.20.2/pih_plb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-24 15:05:14.000000 pih-plb_db-0.20.2/pih_plb_db.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-24 15:05:14.000000 pih-plb_db-0.20.2/pih_plb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-24 15:05:14.000000 pih-plb_db-0.20.2/pih_plb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 15:05:15.851422 pih-plb_db-0.20.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 15:19:40.805482 pih-plb_db-0.20.3/
+-rw-rw-rw-   0        0        0      282 2024-05-24 15:19:40.774233 pih-plb_db-0.20.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-24 15:19:40.428403 pih-plb_db-0.20.3/PolibaseDatabaseService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.20.3/PolibaseDatabaseService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.20.3/PolibaseDatabaseService/__main__.py
+-rw-rw-rw-   0        0        0    12197 2024-05-24 15:18:06.000000 pih-plb_db-0.20.3/PolibaseDatabaseService/api.py
+-rw-rw-rw-   0        0        0     1082 2024-05-24 15:18:50.000000 pih-plb_db-0.20.3/PolibaseDatabaseService/const.py
+-rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.20.3/PolibaseDatabaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:19:40.742963 pih-plb_db-0.20.3/pih_plb_db.egg-info/
+-rw-rw-rw-   0        0        0      282 2024-05-24 15:19:40.000000 pih-plb_db-0.20.3/pih_plb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-24 15:19:40.000000 pih-plb_db-0.20.3/pih_plb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 15:19:40.000000 pih-plb_db-0.20.3/pih_plb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-24 15:19:40.000000 pih-plb_db-0.20.3/pih_plb_db.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-24 15:19:40.000000 pih-plb_db-0.20.3/pih_plb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-24 15:19:40.000000 pih-plb_db-0.20.3/pih_plb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 15:19:40.805482 pih-plb_db-0.20.3/setup.cfg
```

### Comparing `pih-plb_db-0.20.2/PolibaseDatabaseService/api.py` & `pih-plb_db-0.20.3/PolibaseDatabaseService/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -170,57 +170,72 @@
                 "-p",
                 esc(A.D_V_E.value("POLIBASE_DATABASE_ARCHIVE_PASSWORD")),
             )
         )
         compression_level: int | None = A.S.get(
             A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL
         )
-        os.system(
+        A.L.debug_bot(
             js(
                 (
-                    archiver_program_path,
-                    (
-                        (
-                            js(
+                    "arch:",
+                    os.system(
+                        js(
+                            (
+                                archiver_program_path,
                                 (
-                                    j(("a -t", ARCHIVE_TYPE)),
                                     (
-                                        None
-                                        if n(compression_level)
-                                        else j(
+                                        js(
                                             (
-                                                "-mx",
-                                                A.S.get(
-                                                    A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL
+                                                j(("a -t", ARCHIVE_TYPE)),
+                                                (
+                                                    None
+                                                    if n(compression_level)
+                                                    else j(
+                                                        (
+                                                            "-mx",
+                                                            A.S.get(
+                                                                A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL
+                                                            ),
+                                                        )
+                                                    )
                                                 ),
+                                                password_parameter,
                                             )
                                         )
-                                    ),
-                                    password_parameter,
-                                )
+                                    )
+                                    if n(archive_creation_parameters)
+                                    else js(
+                                        (
+                                            archive_creation_parameters,
+                                            password_parameter,
+                                        )
+                                    )
+                                ),
+                                file_out_name,
+                                file_database_dump_name_out,
                             )
                         )
-                        if n(archive_creation_parameters)
-                        else js((archive_creation_parameters, password_parameter))
                     ),
-                    file_out_name,
-                    file_database_dump_name_out,
                 )
             )
         )
 
         A.E.backup_notify_about_polibase_creation_archived_db_dumb_complete(
             os.path.getsize(A.PTH.join(polibase_folder_path, file_out_name)), not test
         )
 
         # step 4
         A.E.backup_notify_about_polibase_coping_archived_db_dumb_start(
             A.CT_H.NAS.ALIAS.upper()
         )
-        os.system(nas_copy_command)
+         A.L.debug_bot(
+            js(
+                (
+                    "nas_copy_command:",os.system(nas_copy_command), nas_copy_command)))
         A.E.backup_notify_about_polibase_coping_archived_db_dumb_complete(
             A.CT_H.NAS.ALIAS.upper()
         )
 
         # step 5
         A.E.backup_notify_about_polibase_coping_db_dumb_start(
             A.CT_H.POLIBASE2.ALIAS.upper()
```

### Comparing `pih-plb_db-0.20.2/PolibaseDatabaseService/const.py` & `pih-plb_db-0.20.3/PolibaseDatabaseService/const.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "PolibaseDatabase"
 
 HOST = A.CT_H.POLIBASE
 
-VERSION: str = "0.20.2"
+VERSION: str = "0.20.3"
 
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     host=HOST.NAME,
     description="Polibase database service",
     commands=("create_polibase_database_backup",),
```

### Comparing `pih-plb_db-0.20.2/PolibaseDatabaseService/service.py` & `pih-plb_db-0.20.3/PolibaseDatabaseService/service.py`

 * *Files identical despite different names*

