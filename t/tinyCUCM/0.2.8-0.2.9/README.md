# Comparing `tmp/tinycucm-0.2.8.tar.gz` & `tmp/tinycucm-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinycucm-0.2.8.tar", last modified: Thu May 16 07:10:11 2024, max compression
+gzip compressed data, was "tinycucm-0.2.9.tar", last modified: Fri May 24 06:33:57 2024, max compression
```

## Comparing `tinycucm-0.2.8.tar` & `tinycucm-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-05-16 07:10:11.576629 tinycucm-0.2.8/
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     1065 2023-12-14 09:02:09.000000 tinycucm-0.2.8/LICENSE
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    53461 2024-05-16 07:10:11.575101 tinycucm-0.2.8/PKG-INFO
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    52886 2024-05-16 06:59:40.000000 tinycucm-0.2.8/README.md
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      655 2024-05-08 16:58:24.000000 tinycucm-0.2.8/pyproject.toml
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)       38 2024-05-16 07:10:11.576779 tinycucm-0.2.8/setup.cfg
-drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-05-16 07:10:11.556349 tinycucm-0.2.8/src/
-drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-05-16 07:10:11.568370 tinycucm-0.2.8/src/tinyCUCM/
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      102 2024-03-06 09:24:29.000000 tinycucm-0.2.8/src/tinyCUCM/__init__.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     1011 2024-03-06 11:07:28.000000 tinycucm-0.2.8/src/tinyCUCM/ccs_models.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    61188 2024-05-16 06:59:40.000000 tinycucm-0.2.8/src/tinyCUCM/client.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     3812 2024-04-27 06:18:56.000000 tinycucm-0.2.8/src/tinyCUCM/decorators.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      811 2023-12-14 16:21:28.000000 tinycucm-0.2.8/src/tinyCUCM/exceptions.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     1152 2024-03-06 11:07:52.000000 tinycucm-0.2.8/src/tinyCUCM/ris_models.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     7822 2024-04-05 07:35:16.000000 tinycucm-0.2.8/src/tinyCUCM/settings.py
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)     4856 2024-03-18 16:33:58.000000 tinycucm-0.2.8/src/tinyCUCM/sql_models.py
-drwxr-xr-x   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        0 2024-05-16 07:10:11.573711 tinycucm-0.2.8/src/tinyCUCM.egg-info/
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)    53461 2024-05-16 07:10:11.000000 tinycucm-0.2.8/src/tinyCUCM.egg-info/PKG-INFO
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)      419 2024-05-16 07:10:11.000000 tinycucm-0.2.8/src/tinyCUCM.egg-info/SOURCES.txt
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        1 2024-05-16 07:10:11.000000 tinycucm-0.2.8/src/tinyCUCM.egg-info/dependency_links.txt
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)       28 2024-05-16 07:10:11.000000 tinycucm-0.2.8/src/tinyCUCM.egg-info/requires.txt
--rw-r--r--   0 ruaute2  (1475392673) RAIFFEISEN\Domain Users (608140329)        9 2024-05-16 07:10:11.000000 tinycucm-0.2.8/src/tinyCUCM.egg-info/top_level.txt
+drwxr-xr-x   0 ruaute2  (1475392673) 608140329        0 2024-05-24 06:33:57.631868 tinycucm-0.2.9/
+-rw-r--r--   0 ruaute2  (1475392673) 608140329     1065 2023-12-14 09:02:09.000000 tinycucm-0.2.9/LICENSE
+-rw-r--r--   0 ruaute2  (1475392673) 608140329    53461 2024-05-24 06:33:57.630618 tinycucm-0.2.9/PKG-INFO
+-rw-r--r--   0 ruaute2  (1475392673) 608140329    52886 2024-05-16 06:59:40.000000 tinycucm-0.2.9/README.md
+-rw-r--r--   0 ruaute2  (1475392673) 608140329      655 2024-05-24 06:29:03.000000 tinycucm-0.2.9/pyproject.toml
+-rw-r--r--   0 ruaute2  (1475392673) 608140329       38 2024-05-24 06:33:57.632019 tinycucm-0.2.9/setup.cfg
+drwxr-xr-x   0 ruaute2  (1475392673) 608140329        0 2024-05-24 06:33:57.609481 tinycucm-0.2.9/src/
+drwxr-xr-x   0 ruaute2  (1475392673) 608140329        0 2024-05-24 06:33:57.620933 tinycucm-0.2.9/src/tinyCUCM/
+-rw-r--r--   0 ruaute2  (1475392673) 608140329      102 2024-03-06 09:24:29.000000 tinycucm-0.2.9/src/tinyCUCM/__init__.py
+-rw-r--r--   0 ruaute2  (1475392673) 608140329     1011 2024-03-06 11:07:28.000000 tinycucm-0.2.9/src/tinyCUCM/ccs_models.py
+-rw-r--r--   0 ruaute2  (1475392673) 608140329    61333 2024-05-24 06:29:03.000000 tinycucm-0.2.9/src/tinyCUCM/client.py
+-rw-r--r--   0 ruaute2  (1475392673) 608140329     3812 2024-04-27 06:18:56.000000 tinycucm-0.2.9/src/tinyCUCM/decorators.py
+-rw-r--r--   0 ruaute2  (1475392673) 608140329      811 2023-12-14 16:21:28.000000 tinycucm-0.2.9/src/tinyCUCM/exceptions.py
+-rw-r--r--   0 ruaute2  (1475392673) 608140329     1152 2024-03-06 11:07:52.000000 tinycucm-0.2.9/src/tinyCUCM/ris_models.py
+-rw-r--r--   0 ruaute2  (1475392673) 608140329     7822 2024-04-05 07:35:16.000000 tinycucm-0.2.9/src/tinyCUCM/settings.py
+-rw-r--r--   0 ruaute2  (1475392673) 608140329     4856 2024-03-18 16:33:58.000000 tinycucm-0.2.9/src/tinyCUCM/sql_models.py
+drwxr-xr-x   0 ruaute2  (1475392673) 608140329        0 2024-05-24 06:33:57.629200 tinycucm-0.2.9/src/tinyCUCM.egg-info/
+-rw-r--r--   0 ruaute2  (1475392673) 608140329    53461 2024-05-24 06:33:57.000000 tinycucm-0.2.9/src/tinyCUCM.egg-info/PKG-INFO
+-rw-r--r--   0 ruaute2  (1475392673) 608140329      419 2024-05-24 06:33:57.000000 tinycucm-0.2.9/src/tinyCUCM.egg-info/SOURCES.txt
+-rw-r--r--   0 ruaute2  (1475392673) 608140329        1 2024-05-24 06:33:57.000000 tinycucm-0.2.9/src/tinyCUCM.egg-info/dependency_links.txt
+-rw-r--r--   0 ruaute2  (1475392673) 608140329       28 2024-05-24 06:33:57.000000 tinycucm-0.2.9/src/tinyCUCM.egg-info/requires.txt
+-rw-r--r--   0 ruaute2  (1475392673) 608140329        9 2024-05-24 06:33:57.000000 tinycucm-0.2.9/src/tinyCUCM.egg-info/top_level.txt
```

### Comparing `tinycucm-0.2.8/LICENSE` & `tinycucm-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tinycucm-0.2.8/PKG-INFO` & `tinycucm-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyCUCM
-Version: 0.2.8
+Version: 0.2.9
 Summary: Cisco Unified Call Manager AXL Methods Collection.
 Author-email: Luarvick <lu.luarvick@gmail.com>
 Project-URL: Homepage, https://github.com/luarvick/tinyCUCM
 Project-URL: Issues, https://github.com/luarvick/tinyCUCM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyCUCM Version: 0.2.8 Summary: Cisco Unified Call
+Metadata-Version: 2.1 Name: tinyCUCM Version: 0.2.9 Summary: Cisco Unified Call
 Manager AXL Methods Collection. Author-email: Luarvick
 gmail.com> Project-URL: Homepage, https://github.com/luarvick/tinyCUCM Project-
 URL: Issues, https://github.com/luarvick/tinyCUCM/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 zeep==4.2.1 Requires-Dist: pydantic==2.6.3
```

### Comparing `tinycucm-0.2.8/README.md` & `tinycucm-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `tinycucm-0.2.8/pyproject.toml` & `tinycucm-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tinyCUCM"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Luarvick", email="lu.luarvick@gmail.com" },
 ]
 description = "Cisco Unified Call Manager AXL Methods Collection."
 readme = "README.md"
 dependencies = [
     "zeep==4.2.1",
```

### Comparing `tinycucm-0.2.8/src/tinyCUCM/ccs_models.py` & `tinycucm-0.2.9/src/tinyCUCM/ccs_models.py`

 * *Files identical despite different names*

### Comparing `tinycucm-0.2.8/src/tinyCUCM/client.py` & `tinycucm-0.2.9/src/tinyCUCM/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1395,14 +1395,15 @@
 
         validated_data = CucmSqlSearchCallPickupGroupModel(**kwargs).model_dump()
         sql_query = """SELECT cpg.pkid,
                               cpg.name,
                               npg.description,
                               npg.dnorpattern AS pattern,
                               rpg.name AS partition,
+                              npm.pkid AS line_pkid,
                               npm.dnorpattern AS line,
                               rpm.name AS line_partition,
                               npm.description AS line_description
                          FROM pickupgroup cpg
                     LEFT JOIN numplan npg ON npg.pkid = cpg.fknumplan_pickup
                     LEFT JOIN routepartition rpg ON rpg.pkid = npg.fkroutepartition
                     LEFT JOIN pickupgrouplinemap pglm ON pglm.fkpickupgroup = cpg.pkid
@@ -1427,24 +1428,25 @@
         """
 
         validated_data = CucmSqlSearchDeviceModel(**kwargs).model_dump()
         sql_query = """SELECT d.pkid,
                               d.name,
                               d.description,
                               dp.name AS device_pool,
+                              np.pkid AS line_pkid,
                               np.dnorpattern AS line,
                               dnpm.numplanindex AS line_index,
                               rp.name AS line_partition,
                               np.description AS line_description,
                               tc.name AS class,
                               tm.name AS model,
-                              eu.pkid AS pkid_end_user,
+                              eu.pkid AS end_user_pkid,
                               eu.userid, 
                               eu.displayname AS display_name,
-                              eu_rdp.pkid AS pkid_end_user_rdp,
+                              eu_rdp.pkid AS end_user_rdp_pkid,
                               eu_rdp.userid AS userid_rdp,
                               eu_rdp.displayname AS display_name_rdp
                          FROM device d
                     LEFT JOIN devicenumplanmap dnpm ON dnpm.fkdevice = d.pkid
                     LEFT JOIN numplan np ON np.pkid = dnpm.fknumplan
                     LEFT JOIN routepartition rp ON rp.pkid = np.fkroutepartition
                     LEFT JOIN devicepool dp ON dp.pkid = d.fkdevicepool
@@ -1502,14 +1504,15 @@
         :return:
         """
 
         validated_data = CucmSqlSearchLineGroupModel(**kwargs).model_dump()
         sql_query = """SELECT lg.pkid,
                               lg.name,
                               tda.name AS algorithm,
+                              np.pkid AS line_pkid,
                               np.dnorpattern AS line,
                               rp.name AS line_partition,
                               np.description AS line_description,
                               lgnpm.lineselectionorder AS line_index
                          FROM linegroup lg
                     LEFT JOIN linegroupnumplanmap lgnpm ON lgnpm.fklinegroup = lg.pkid
                     LEFT JOIN typedistributealgorithm tda ON tda.enum = lg.tkdistributealgorithm
@@ -1611,18 +1614,18 @@
         """
 
         sql_query = """SELECT d.pkid AS device_pkid,
                               d.name AS device,
                               d.description AS device_description,
                               tc.name AS device_class,
                               tm.name AS device_model,
-                              np.pkid AS pattern_pkid,
-                              np.dnorpattern AS pattern,
-                              np.description AS pattern_description,
-                              rp.name AS pattern_partition,
+                              np.pkid AS line_pkid,
+                              np.dnorpattern AS line,
+                              np.description AS line_description,
+                              rp.name AS line_partition,
                               np.tkpatternusage AS pattern_usage,
                               tpu.name AS pattern_type
                          FROM device d
                     LEFT JOIN devicenumplanmap dnpm ON dnpm.fkdevice = d.pkid
                     LEFT JOIN numplan np ON np.pkid = dnpm.fknumplan
                     LEFT JOIN routepartition rp ON rp.pkid = np.fkroutepartition
                     LEFT JOIN typepatternusage tpu ON tpu.enum = np.tkpatternusage
```

### Comparing `tinycucm-0.2.8/src/tinyCUCM/decorators.py` & `tinycucm-0.2.9/src/tinyCUCM/decorators.py`

 * *Files identical despite different names*

### Comparing `tinycucm-0.2.8/src/tinyCUCM/exceptions.py` & `tinycucm-0.2.9/src/tinyCUCM/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinycucm-0.2.8/src/tinyCUCM/ris_models.py` & `tinycucm-0.2.9/src/tinyCUCM/ris_models.py`

 * *Files identical despite different names*

### Comparing `tinycucm-0.2.8/src/tinyCUCM/settings.py` & `tinycucm-0.2.9/src/tinyCUCM/settings.py`

 * *Files identical despite different names*

### Comparing `tinycucm-0.2.8/src/tinyCUCM/sql_models.py` & `tinycucm-0.2.9/src/tinyCUCM/sql_models.py`

 * *Files identical despite different names*

### Comparing `tinycucm-0.2.8/src/tinyCUCM.egg-info/PKG-INFO` & `tinycucm-0.2.9/src/tinyCUCM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyCUCM
-Version: 0.2.8
+Version: 0.2.9
 Summary: Cisco Unified Call Manager AXL Methods Collection.
 Author-email: Luarvick <lu.luarvick@gmail.com>
 Project-URL: Homepage, https://github.com/luarvick/tinyCUCM
 Project-URL: Issues, https://github.com/luarvick/tinyCUCM/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyCUCM Version: 0.2.8 Summary: Cisco Unified Call
+Metadata-Version: 2.1 Name: tinyCUCM Version: 0.2.9 Summary: Cisco Unified Call
 Manager AXL Methods Collection. Author-email: Luarvick
 gmail.com> Project-URL: Homepage, https://github.com/luarvick/tinyCUCM Project-
 URL: Issues, https://github.com/luarvick/tinyCUCM/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 zeep==4.2.1 Requires-Dist: pydantic==2.6.3
```

