# Comparing `tmp/saphira-0.0.8.tar.gz` & `tmp/saphira-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saphira-0.0.8.tar", last modified: Mon Apr 29 15:58:40 2024, max compression
+gzip compressed data, was "saphira-0.0.9.tar", last modified: Fri May 24 01:29:05 2024, max compression
```

## Comparing `saphira-0.0.8.tar` & `saphira-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-29 15:58:40.316375 saphira-0.0.8/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2023-12-22 05:35:11.000000 saphira-0.0.8/LICENSE
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-29 15:58:40.314785 saphira-0.0.8/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2023-12-19 02:46:29.000000 saphira-0.0.8/README.md
--rw-r--r--   0 akshaychalana   (501) staff       (20)      718 2024-04-29 15:57:58.000000 saphira-0.0.8/pyproject.toml
--rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2024-04-29 15:58:40.316511 saphira-0.0.8/setup.cfg
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-29 15:58:40.287562 saphira-0.0.8/src/
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-29 15:58:40.296326 saphira-0.0.8/src/saphira/
--rw-r--r--   0 akshaychalana   (501) staff       (20)       45 2024-04-29 15:57:44.000000 saphira-0.0.8/src/saphira/__init__.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)     3898 2024-04-28 08:11:22.000000 saphira-0.0.8/src/saphira/saphira.py
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-29 15:58:40.313184 saphira-0.0.8/src/saphira.egg-info/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-29 15:58:40.000000 saphira-0.0.8/src/saphira.egg-info/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)      373 2024-04-29 15:58:40.000000 saphira-0.0.8/src/saphira.egg-info/SOURCES.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2024-04-29 15:58:40.000000 saphira-0.0.8/src/saphira.egg-info/dependency_links.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)       53 2024-04-29 15:58:40.000000 saphira-0.0.8/src/saphira.egg-info/requires.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2024-04-29 15:58:40.000000 saphira-0.0.8/src/saphira.egg-info/top_level.txt
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-29 15:58:40.311064 saphira-0.0.8/tests/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1743 2024-04-27 00:19:40.000000 saphira-0.0.8/tests/test_battery_capacity.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)      660 2024-04-09 06:41:30.000000 saphira-0.0.8/tests/test_energy_density.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)      596 2023-11-18 02:00:44.000000 saphira-0.0.8/tests/test_jama_server.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)      782 2024-04-28 17:31:20.000000 saphira-0.0.8/tests/test_radar_state_machine.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-05-24 01:29:05.049921 saphira-0.0.9/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2024-05-07 19:37:46.000000 saphira-0.0.9/LICENSE
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-05-24 01:29:05.049313 saphira-0.0.9/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2024-05-07 19:37:46.000000 saphira-0.0.9/README.md
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      718 2024-05-24 01:28:48.000000 saphira-0.0.9/pyproject.toml
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2024-05-24 01:29:05.050023 saphira-0.0.9/setup.cfg
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-05-24 01:29:05.033858 saphira-0.0.9/src/
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-05-24 01:29:05.037861 saphira-0.0.9/src/saphira/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       45 2024-05-24 01:28:40.000000 saphira-0.0.9/src/saphira/__init__.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     4446 2024-05-24 01:10:38.000000 saphira-0.0.9/src/saphira/saphira.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-05-24 01:29:05.048103 saphira-0.0.9/src/saphira.egg-info/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-05-24 01:29:05.000000 saphira-0.0.9/src/saphira.egg-info/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      373 2024-05-24 01:29:05.000000 saphira-0.0.9/src/saphira.egg-info/SOURCES.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2024-05-24 01:29:05.000000 saphira-0.0.9/src/saphira.egg-info/dependency_links.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       53 2024-05-24 01:29:05.000000 saphira-0.0.9/src/saphira.egg-info/requires.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2024-05-24 01:29:05.000000 saphira-0.0.9/src/saphira.egg-info/top_level.txt
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-05-24 01:29:05.047322 saphira-0.0.9/tests/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1743 2024-05-07 19:37:46.000000 saphira-0.0.9/tests/test_battery_capacity.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      660 2024-05-07 19:37:46.000000 saphira-0.0.9/tests/test_energy_density.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1671 2024-05-08 20:18:08.000000 saphira-0.0.9/tests/test_jama_server.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      782 2024-05-07 19:37:46.000000 saphira-0.0.9/tests/test_radar_state_machine.py
```

### Comparing `saphira-0.0.8/LICENSE` & `saphira-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `saphira-0.0.8/PKG-INFO` & `saphira-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.8
+Version: 0.0.9
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `saphira-0.0.8/pyproject.toml` & `saphira-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saphira"
-version = "0.0.8"
+version = "0.0.9"
 description = "Access parameters from the Saphira.ai SysEng SSoT"
 readme = "README.md"
 authors = [{ name = "Saphira AI", email = "contact@saphira.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `saphira-0.0.8/src/saphira/saphira.py` & `saphira-0.0.9/src/saphira/saphira.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+from numbers import Number
 import os
 import re
 import requests
 import subprocess
 import traceback
 from typing import Any, Optional
 import multiprocessing
@@ -50,19 +51,18 @@
             upload_resp = requests.post(upload_url, files=files, headers=HEADERS)
             print(f"{upload_url} responded with status code {upload_resp.status_code}")
             if upload_resp.status_code != 200:
                 print(f"Upload failed with {upload_resp.text}")
 
     return result
 
-# TODO: Alternatively support Exception input
 def update_test_status(project: str, requirement: str, passing: bool = False, test_result: Optional[TestResult] = None, exception: Exception = None):
     stack = inspect.stack()
     test = stack[-1].filename.split('/')[-1]
-    # TODO: Extract failure information from test_result (also include errors, not just failures)
+    # Extract failure information from test_result (also include errors, not just failures)
     failure = ''
     if test_result:
         passing = test_result.wasSuccessful()
         if len(test_result.failures) > 0:
             # TODO: Add safety here
             failure = test_result.failures[0][1].split('\n')[-3].split('(')[1].split(" ")[0]
             # TODO: Traverse AST for source of this variable instead
@@ -81,8 +81,18 @@
     print(f"failure: {failure}")
 
     resp = requests.post(f'{SAPHIRA_URL}/update_test_status', json={'key': requirement, 
                                                                     'passing': passing, 
                                                                     'project': project, 
                                                                     'test': test,
                                                                     'failure': failure}, headers=HEADERS)
-    print(resp.text)
+    print(resp.text)
+
+def create_or_update(project: str, key: str, value: Any, unit: str, description: str, parents: str) -> str:
+    resp = requests.post(f'{SAPHIRA_URL}/add_requirement?projectUuid={project}', 
+                         json={'key': key, 
+                               'requirement_type': 'numerical' if isinstance(value, Number) else 'text', 
+                               'value': value,
+                               'unit': unit,
+                               'reason': description, 
+                               'parents': parents}, headers=HEADERS)
+    return resp
```

### Comparing `saphira-0.0.8/src/saphira.egg-info/PKG-INFO` & `saphira-0.0.9/src/saphira.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.8
+Version: 0.0.9
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `saphira-0.0.8/tests/test_battery_capacity.py` & `saphira-0.0.9/tests/test_battery_capacity.py`

 * *Files identical despite different names*

### Comparing `saphira-0.0.8/tests/test_energy_density.py` & `saphira-0.0.9/tests/test_energy_density.py`

 * *Files identical despite different names*

### Comparing `saphira-0.0.8/tests/test_radar_state_machine.py` & `saphira-0.0.9/tests/test_radar_state_machine.py`

 * *Files identical despite different names*

