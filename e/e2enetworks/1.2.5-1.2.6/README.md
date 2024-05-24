# Comparing `tmp/e2enetworks-1.2.5.tar.gz` & `tmp/e2enetworks-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-1.2.5.tar", last modified: Thu May 23 06:58:59 2024, max compression
+gzip compressed data, was "e2enetworks-1.2.6.tar", last modified: Fri May 24 10:20:08 2024, max compression
```

## Comparing `e2enetworks-1.2.5.tar` & `e2enetworks-1.2.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.895915 e2enetworks-1.2.5/
--rw-r--r--   0 aman       (501) staff       (20)    10786 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/LICENSE.txt
--rw-r--r--   0 aman       (501) staff       (20)     1160 2024-05-23 06:58:59.895574 e2enetworks-1.2.5/PKG-INFO
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/README.rst
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.884729 e2enetworks-1.2.5/e2enetworks/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/__init__.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.886582 e2enetworks-1.2.5/e2enetworks/cloud/
--rw-r--r--   0 aman       (501) staff       (20)        0 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)      147 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/test.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.893726 e2enetworks-1.2.5/e2enetworks/cloud/tir/
--rw-r--r--   0 aman       (501) staff       (20)     2390 2024-05-01 12:23:40.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)     9305 2024-04-23 09:50:02.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/api_client.py
--rw-r--r--   0 aman       (501) staff       (20)     2794 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/apitoken.py
--rw-r--r--   0 aman       (501) staff       (20)     9394 2024-05-01 11:52:21.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/client.py
--rw-r--r--   0 aman       (501) staff       (20)     8779 2024-05-02 06:03:17.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/constants.py
--rw-r--r--   0 aman       (501) staff       (20)     5630 2024-05-01 11:21:31.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/datasets.py
--rw-r--r--   0 aman       (501) staff       (20)    13823 2023-12-15 09:21:32.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/endpoints.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.894758 e2enetworks-1.2.5/e2enetworks/cloud/tir/finetuning/
--rw-r--r--   0 aman       (501) staff       (20)        0 2024-04-30 09:51:50.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/finetuning/__init__.py
--rw-r--r--   0 aman       (501) staff       (20)      382 2024-05-01 09:25:21.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/finetuning/constants.py
--rw-r--r--   0 aman       (501) staff       (20)     9809 2024-05-22 10:54:24.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/finetuning/finetuner.py
--rw-r--r--   0 aman       (501) staff       (20)     3057 2024-05-22 10:54:35.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/helpers.py
--rw-r--r--   0 aman       (501) staff       (20)     1368 2023-11-28 07:27:23.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/images.py
--rw-r--r--   0 aman       (501) staff       (20)     2105 2024-04-23 09:50:02.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/minio_service.py
--rw-r--r--   0 aman       (501) staff       (20)     6934 2024-05-23 06:01:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/models.py
--rw-r--r--   0 aman       (501) staff       (20)     6022 2023-12-15 09:21:32.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/notebook.py
--rw-r--r--   0 aman       (501) staff       (20)     9999 2023-12-15 09:21:32.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/pipelines.py
--rw-r--r--   0 aman       (501) staff       (20)     2849 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/projects.py
--rw-r--r--   0 aman       (501) staff       (20)     4268 2024-05-01 10:15:57.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/skus.py
--rw-r--r--   0 aman       (501) staff       (20)     2391 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/teams.py
--rw-r--r--   0 aman       (501) staff       (20)     1059 2024-05-02 06:16:05.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/utils.py
--rw-r--r--   0 aman       (501) staff       (20)       23 2023-11-21 11:03:20.000000 e2enetworks-1.2.5/e2enetworks/cloud/tir/version.py
--rw-r--r--   0 aman       (501) staff       (20)     1566 2024-05-22 11:49:33.000000 e2enetworks-1.2.5/e2enetworks/constants.py
-drwxr-xr-x   0 aman       (501) staff       (20)        0 2024-05-23 06:58:59.886151 e2enetworks-1.2.5/e2enetworks.egg-info/
--rw-r--r--   0 aman       (501) staff       (20)     1160 2024-05-23 06:58:59.000000 e2enetworks-1.2.5/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 aman       (501) staff       (20)     1051 2024-05-23 06:58:59.000000 e2enetworks-1.2.5/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 aman       (501) staff       (20)        1 2024-05-23 06:58:59.000000 e2enetworks-1.2.5/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 aman       (501) staff       (20)       40 2024-05-23 06:58:59.000000 e2enetworks-1.2.5/e2enetworks.egg-info/requires.txt
--rw-r--r--   0 aman       (501) staff       (20)       12 2024-05-23 06:58:59.000000 e2enetworks-1.2.5/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 aman       (501) staff       (20)       38 2024-05-23 06:58:59.895998 e2enetworks-1.2.5/setup.cfg
--rw-r--r--   0 aman       (501) staff       (20)     1710 2024-05-23 06:02:59.000000 e2enetworks-1.2.5/setup.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-05-24 10:20:08.912353 e2enetworks-1.2.6/
+-rw-r--r--   0 jagga      (501) staff       (20)    10786 2024-04-15 09:47:56.000000 e2enetworks-1.2.6/LICENSE.txt
+-rw-r--r--   0 jagga      (501) staff       (20)     1275 2024-05-24 10:20:08.912083 e2enetworks-1.2.6/PKG-INFO
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.6/README.rst
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-05-24 10:20:08.906999 e2enetworks-1.2.6/e2enetworks/
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.6/e2enetworks/__init__.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-05-24 10:20:08.907956 e2enetworks-1.2.6/e2enetworks/cloud/
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.6/e2enetworks/cloud/__init__.py
+-rw-r--r--   0 jagga      (501) staff       (20)      147 2024-04-15 09:47:56.000000 e2enetworks-1.2.6/e2enetworks/cloud/test.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-05-24 10:20:08.911180 e2enetworks-1.2.6/e2enetworks/cloud/tir/
+-rw-r--r--   0 jagga      (501) staff       (20)     2390 2024-05-10 09:46:13.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/__init__.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9509 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/api_client.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2794 2024-04-15 09:47:56.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/apitoken.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9393 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/client.py
+-rw-r--r--   0 jagga      (501) staff       (20)     8779 2024-05-10 09:46:13.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/constants.py
+-rw-r--r--   0 jagga      (501) staff       (20)     6087 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/datasets.py
+-rw-r--r--   0 jagga      (501) staff       (20)    23432 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/endpoints.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-05-24 10:20:08.911577 e2enetworks-1.2.6/e2enetworks/cloud/tir/finetuning/
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-05-10 09:46:13.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/finetuning/__init__.py
+-rw-r--r--   0 jagga      (501) staff       (20)      382 2024-05-10 09:46:13.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/finetuning/constants.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9809 2024-05-10 09:46:13.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/finetuning/finetuner.py
+-rw-r--r--   0 jagga      (501) staff       (20)     3545 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/helpers.py
+-rw-r--r--   0 jagga      (501) staff       (20)     1457 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/images.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2480 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/minio_service.py
+-rw-r--r--   0 jagga      (501) staff       (20)     8031 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/models.py
+-rw-r--r--   0 jagga      (501) staff       (20)    11967 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/notebook.py
+-rw-r--r--   0 jagga      (501) staff       (20)    10164 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/pipelines.py
+-rw-r--r--   0 jagga      (501) staff       (20)     3209 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/projects.py
+-rw-r--r--   0 jagga      (501) staff       (20)     5187 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/skus.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2391 2024-04-15 09:47:56.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/teams.py
+-rw-r--r--   0 jagga      (501) staff       (20)     1142 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/utils.py
+-rw-r--r--   0 jagga      (501) staff       (20)       23 2024-04-15 09:47:56.000000 e2enetworks-1.2.6/e2enetworks/cloud/tir/version.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2518 2024-05-24 10:18:45.000000 e2enetworks-1.2.6/e2enetworks/constants.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-05-24 10:20:08.911815 e2enetworks-1.2.6/e2enetworks.egg-info/
+-rw-r--r--   0 jagga      (501) staff       (20)     1275 2024-05-24 10:20:08.000000 e2enetworks-1.2.6/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 jagga      (501) staff       (20)     1051 2024-05-24 10:20:08.000000 e2enetworks-1.2.6/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 jagga      (501) staff       (20)        1 2024-05-24 10:20:08.000000 e2enetworks-1.2.6/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 jagga      (501) staff       (20)       40 2024-05-24 10:20:08.000000 e2enetworks-1.2.6/e2enetworks.egg-info/requires.txt
+-rw-r--r--   0 jagga      (501) staff       (20)       12 2024-05-24 10:20:08.000000 e2enetworks-1.2.6/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 jagga      (501) staff       (20)       38 2024-05-24 10:20:08.912404 e2enetworks-1.2.6/setup.cfg
+-rw-r--r--   0 jagga      (501) staff       (20)     1710 2024-05-24 10:19:00.000000 e2enetworks-1.2.6/setup.py
```

### Comparing `e2enetworks-1.2.5/LICENSE.txt` & `e2enetworks-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.5/PKG-INFO` & `e2enetworks-1.2.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 1.2.5
+Version: 1.2.6
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
@@ -23,7 +23,12 @@
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: urllib3
+Requires-Dist: minio
+Requires-Dist: prettytable
+Requires-Dist: tqdm
```

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/__init__.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/__init__.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/api_client.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from e2enetworks.cloud.tir import client
 from e2enetworks.cloud.tir.constants import MODEL_NAME_TO_URL_PATH_MAPPING, LANGUAGES_SUPPORTED_BY_WHISPER,REQUIRED_PARAMETERS_WHISPER,ALLOWED_TIMESTAMPS_VALUE_WHISPER
 from e2enetworks.cloud.tir.helpers import (get_formated_data_for_model,
                                            get_model_url, get_random_string)
 from e2enetworks.cloud.tir.minio_service import MinioService
 from e2enetworks.cloud.tir.utils import prepare_object
 from e2enetworks.constants import (BASE_GPU_URL, BUCKET_TYPES, MANAGED_STORAGE,
-                                   MODEL_TYPES, headers,WHISPER_LARGE_V3,WHISPER_DATA_LIMIT_BYTES)
+                                   MODEL_TYPES, headers,WHISPER_LARGE_V3,STABLE_DIFFUSION_2_1,WHISPER_DATA_LIMIT_BYTES)
 
 
 class ModelAPIClient:
     def __init__(self, team: Optional[str] = "", project: Optional[str] = ""):
         client_not_ready = (
             "Client is not ready. Please initiate client by:"
             "\n- Using e2enetworks.cloud.tir.init(...)"
@@ -31,14 +31,17 @@
             client.Default.set_team(team)
 
     def infer(self, model_name, data):
         
         if model_name == WHISPER_LARGE_V3 :
             return self.__whisper_infer(data)
         
+        if model_name == STABLE_DIFFUSION_2_1 and (not data.get('generator') or data.get('generator')=='null') :
+            raise ValueError('generator should not be null')
+        
         namespace = "p-" + str(client.Default.project())
         try:
             url_status, url = get_model_url(model_name, namespace)
             if not url_status:
                 raise Exception(f"Invalid input Error {url} model not present")
             data_status, payload = get_formated_data_for_model(model_name, data)
             if not data_status:
```

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/apitoken.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/apitoken.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/client.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     def set_team(self, team):
         self._team = team
 
     def gpu_projects_path(self, project=None):
         if not project:
             project = self.project()
         
-        return "{api_host}/api/v1/gpu/projects/{project}".format(api_host=self.api_host(), project=project)
+        return "{api_host}api/v1/gpu/projects/{project}".format(api_host=self.api_host(), project=project)
     
     def project(self):
         if self._project:
             return self._project
         
         project_not_set = (
             "Project ID not set. Please provide a project ID by:"
```

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/constants.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/constants.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/datasets.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from typing import Optional
 
 import requests
+import os
 
 from e2enetworks.cloud.tir import client
 from e2enetworks.cloud.tir.minio_service import MinioService
 from e2enetworks.cloud.tir.utils import prepare_object
 from e2enetworks.constants import BASE_GPU_URL, BUCKET_TYPES, headers
 
 
@@ -24,15 +25,22 @@
 
         if project:
             client.Default.set_project(project)
 
         if team:
             client.Default.set_team(team)
 
-    def create(self, name, bucket_name=None, bucket_type='managed', description=""):
+    def create(self, name=None, bucket_name=None, bucket_type="managed", description=""):
+        if bucket_type!="managed":
+            if not bucket_name:
+                raise ValueError("please specify a valid bucket_name")
+            
+            if not bucket_type:
+                raise ValueError("please specify a valid bucket_type")
+
         payload = json.dumps({
             "type": bucket_type,
             "name": name,
             "bucket_name": bucket_name,
             "description": description,
         })
         headers['Authorization'] = f'Bearer {client.Default.access_token()}'
@@ -65,16 +73,19 @@
         dataset = self.get(dataset_id) if dataset_id else None
         if not dataset:
             raise ValueError("invalid dataset_id parameter")
         access_key = dataset.access_key.access_key
         secret_key = dataset.access_key.secret_key
         try:
             minio_service = MinioService(access_key=access_key, secret_key=secret_key)
-            minio_service.upload_directory_recursive(bucket_name=dataset.bucket.bucket_name,
+            if os.path.isdir(dataset_path):
+                minio_service.upload_directory_recursive(bucket_name=dataset.bucket.bucket_name,
                                                     source_directory=dataset_path, prefix=prefix)
+            else:
+                minio_service.upload_file(bucket_name=dataset.bucket.bucket_name, file_path=dataset_path, prefix=prefix)
             print("Dataset Pushed Successfully")
         except Exception as e:
             print(e)
 
         return dataset
 
     def download_dataset(self, dataset_id, local_path, prefix=""):
```

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/finetuning/finetuner.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/finetuning/finetuner.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/helpers.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,29 +11,42 @@
 
 def cpu_plan_short_code(sku):
     return f"{sku.get('series')}-{sku.get('sku_type').split('-')[0]}-{sku.get('cpu')}-" \
            f"{sku.get('memory')}-{sku.get('gpu') if sku.get('gpu') else 0}"
 
 
 def gpu_plan_short_code(sku):
-    return f"{sku.get('series')}-{sku.get('sku_type').split('.')[1]}-{sku.get('cpu')}-" \
+    #in split function "-" should be used instead of "."
+    return f"{sku.get('series')}-{sku.get('sku_type').split('-')[0]}-{sku.get('cpu')}-" \
            f"{sku.get('memory')}-{sku.get('gpu') if sku.get('gpu') else 0}"
 
 
 def plan_to_sku_id(skus, plan):
     if plan.startswith("CPU"):
         for sku in skus["CPU"]:
             if cpu_plan_short_code(sku) == plan:
                 return sku.get("sku_id")
     else:
         for sku in skus["GPU"]:
             if gpu_plan_short_code(sku) == plan:
                 return sku.get("sku_id")
     return False
 
+def plan_name_to_sku_id(skus, sku_unique_name):
+    if sku_unique_name.startswith("CPU"):
+        for sku in skus["CPU"]:
+            if not sku["is_free"] and cpu_plan_short_code(sku) == sku_unique_name:
+                return sku.get("sku_id")
+    else:
+        for sku in skus["GPU"]:
+            if not sku["is_free"] and gpu_plan_short_code(sku) == sku_unique_name:
+                return sku.get("sku_id")
+    return False
+
+
 
 def plan_name_to_sku_item_price_id(skus, sku_unique_name):
     if sku_unique_name.startswith("CPU"):
         for sku in skus["CPU"]:
             if not sku["is_free"] and cpu_plan_short_code(sku) == sku_unique_name:
                 for plan in sku["plans"]:
                     if plan["committed_days"] == 0:
```

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/images.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/images.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,17 +17,18 @@
     def list(self):
         url = f"{BASE_GPU_URL}gpu_service/image/"
         req = requests.Request('GET', url)
         response = client.Default.make_request(req)
         if response.status_code == 200:
             images = response.json()["data"]
             images_table = PrettyTable()
-            images_table.field_names = ['Name', 'version', 'image_id']
+            images_table.field_names = ['Name', 'version', 'image_id','image_version_id']
             for image in images:
-                images_table.add_row([image.get('name'), image.get('version'), image.get('id')])
+                for v in image["versions"]:
+                    images_table.add_row([image.get('name'), v["version"],  image.get('image_id'), v['image_version_id']])
             return images_table
 
 
     @staticmethod
     def help():
         print("Images Class Help")
         print("\t\t================")
```

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/minio_service.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/minio_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,14 +20,21 @@
                 file_path = os.path.join(root, file)
                 object_name = os.path.join(prefix, os.path.relpath(file_path, source_directory))
                 try:
                     self.client.fput_object(bucket_name, object_name, file_path)
                     print(f"Uploaded {object_name}")
                 except S3Error as e:
                     print(f"Error uploading {object_name}: {e}")
+
+    def upload_file(self, bucket_name, file_path, prefix=""):
+        object_name = f"{prefix}{os.path.basename(file_path)}" if prefix.endswith('/') else f"{prefix}/{os.path.basename(file_path)}"
+        try:
+            self.client.fput_object(bucket_name, object_name, file_path)
+        except Exception as err:
+            print(f"Error uploading {object_name}: {err}")
                
 
     def download_directory_recursive(self, bucket_name, local_path, prefix=""):
         objects = self.client.list_objects(bucket_name=bucket_name, prefix=prefix, recursive=True)
         for obj in objects:
             object_name = obj.object_name
             try:
```

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/models.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 
 import requests
+import os
 
 from typing import Optional
 from e2enetworks.constants import BASE_GPU_URL, BUCKET_TYPES, MODEL_TYPES, headers, MANAGED_STORAGE
 from e2enetworks.cloud.tir import client
 from e2enetworks.cloud.tir.utils import prepare_object
 from e2enetworks.cloud.tir.minio_service import MinioService
 from e2enetworks.cloud.tir.helpers import get_random_string
@@ -25,49 +26,53 @@
 
         if project:
             client.Default.set_project(project)
 
         if team:
             client.Default.set_team(team)
 
-    def create(self, name, model_type, job_id=None, score={}, storage_type=MANAGED_STORAGE, bucket_name=None):
+    def create(self, name, model_type='custom', storage_type=MANAGED_STORAGE, bucket_name=None, access_key=None, secret_key= None):
         try:
             payload = json.dumps({
                 "name": name,
                 "model_type": model_type,
                 "bucket_name": bucket_name,
                 "storage_type": storage_type,
-                "finetuning_id": job_id,
-                "score": score
+                "access_key": access_key,
+                "secret_key": secret_key
             })
         except Exception as e:
             raise Exception(f"Input Error {e}")
         headers['Authorization'] = f'Bearer {client.Default.access_token()}'
         url = f"{BASE_GPU_URL}teams/{client.Default.team()}/projects/{client.Default.project()}/serving/model/?" \
               f"apikey={client.Default.api_key()}"
         response = requests.post(url=url, headers=headers, data=payload)
         response = prepare_object(response)
         return response
 
-    def push_model(self, model_path, prefix="", model_id=None, job_id=None, score={}, model_type="custom", use_caching=False):
+    def push_model(self, model_path, prefix="", model_id=None, model_type="custom", use_caching=False):
         if model_id:
             model = self.get(model_id)
             if not model:
                 raise ValueError("invalid model_id parameter")
         else:
             model_name = f"model{get_random_string(6)}"
-            model = self.create(name=model_name, model_type=model_type, job_id=job_id, score=score, storage_type=MANAGED_STORAGE, bucket_name=None)
+            model = self.create(name=model_name, model_type=model_type, storage_type=MANAGED_STORAGE, bucket_name=None)
             if not model:
                 raise ValueError("failed to create a new model")
         
         access_key = model.access_key.access_key
         secret_key = model.access_key.secret_key
         minio_service = MinioService(access_key=access_key, secret_key=secret_key)
-        minio_service.upload_directory_recursive(bucket_name=model.bucket.bucket_name,
-                                                 source_directory=model_path, prefix=prefix)
+        if os.path.isdir(model_path):
+            minio_service.upload_directory_recursive(bucket_name=model.bucket.bucket_name,
+                                                    source_directory=model_path, prefix=prefix)
+        else :
+            minio_service.upload_file(bucket_name=model.bucket.bucket_name,
+                                                    file_path=model_path, prefix=prefix)
         if use_caching: 
             minio_service.update_cache_file(bucket_name=model.bucket.bucket_name)
         print("Model Pushed Successfully")
         if not model_id:
             return model
 
     def download_model(self, model_id, local_path, prefix=""):
@@ -81,14 +86,31 @@
             secret_key = model.access_key.secret_key
             minio_service = MinioService(access_key=access_key, secret_key=secret_key)
             minio_service.download_directory_recursive(bucket_name=model.bucket.bucket_name, local_path=local_path, prefix=prefix)
             print("Model downloaded successfully")
         except Exception as e:
             print(e)
             raise ValueError("invalid model id")
+    
+    def list_bucket_data(self, model_id, prefix=""):
+        if not model_id:
+            raise ValueError("model id is mandatory")
+        model = self.get(model_id)
+        if not model:
+            raise ValueError("Invalid model id")
+        
+        headers['Authorization'] = f'Bearer {client.Default.access_token()}'
+        url = f"{BASE_GPU_URL}teams/{client.Default.team()}/projects/{client.Default.project()}/serving/model/" \
+              f"{model_id}/bucket/?apikey={client.Default.api_key()}&prefix={prefix}"
+        response = requests.get(url=url, headers=headers)
+        response = prepare_object(response)
+        for i in response:
+            print(i.name)
+        return response
+
 
     def _update_repo(self, model_id, score={}):
         if type(model_id) != int:
             raise ValueError(model_id)
         payload = {
             "score": score
         }
@@ -137,23 +159,25 @@
             "\t\t1. __init__(team, project): Initializes a Models instance with the specified team and project "
             "IDs.")
         print("\t\t2. create(name, model_type, storage_type, bucket_name): Creates a new model with the provided "
               "details.")
         print("\t\t3. push_model(model_path, prefix, model_id, job_id, score, model_type, use_caching): Creates a new model with the provided "
               "details.")
         print("\t\t4. download_model(model_id, local_path, prefix)")
-        print("\t\t get(model_id): Retrieves information about a specific model using its ID.")
-        print("\t\t list(): Lists all models associated with the team and project.")
-        print("\t\t6. delete(model_id): Deletes a model with the given ID.")
-        print("\t\t7. help(): Displays this help message.")
+        print("\t\t5. list_bucket_data(model_id, prefix): to list the content of bucket")
+        print("\t\t6. get(model_id): Retrieves information about a specific model using its ID.")
+        print("\t\t7. list(): Lists all models associated with the team and project.")
+        print("\t\t8. delete(model_id): Deletes a model with the given ID.")
+        print("\t\t9. help(): Displays this help message.")
 
         # Example usages
         print("\t\tExample usages:")
         print("\t\tmodels = Models(123, 456)")
         print(f"\t\tmodels.create(name='Test Dataset', model_type={MODEL_TYPES}, , storage_type={BUCKET_TYPES}, "
               f"bucket_name='dataset-bucket'")
         print(f"\t\tmodels.push_model(model_path, prefix='', model_id=None, model_type='custom')")
         print(f"\t\tmodels.download_model(model_id=<model id>, local_path=<path of local directory>,"
               f" prefix=<prefix in the bucket>)")
+        print(f"\t\tmodels.list_bucket_data(model_id=<model id>, prefix='')")
         print("\t\tmodels.get(789)")
         print("\t\tmodels.list()")
         print("\t\tmodels.delete(789)")
```

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/pipelines.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/pipelines.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from typing import Dict, Optional
 
 import requests
+import json
 
+from e2enetworks.constants import headers
+from e2enetworks.constants import BASE_GPU_URL
 from e2enetworks.cloud.tir.constants import ARGUMENT_IS_MANDATORY
 from e2enetworks.cloud.tir.helpers import plan_name_to_sku_item_price_id
 from e2enetworks.cloud.tir.skus import Plans, client
 from e2enetworks.constants import PIPELINE
 from e2enetworks.cloud.tir.utils import prepare_object
 
 
@@ -88,15 +91,15 @@
 
         file = open(file_path, 'rb')
         files = [
             ('uploadfile',
              (file.name, file, 'application/octet-stream'))
         ]
         url = f"{client.Default.gpu_projects_path()}/pipelines/upload/?name={name}&description={description}&" \
-              f"pipeline_id={pipeline_id}"
+              f"pipeline_id={pipeline_id}&"
         req = requests.Request('POST', url, files=files)
         response = client.Default.make_request(req)
         return prepare_object(response)
 
     def list_pipeline_version(
             self,
             pipeline_id: str = ''
@@ -156,28 +159,28 @@
 
     def get_experiment(
         self,
         experiment_id: str = '',
     ):
         if not experiment_id:
             raise ValueError(f"EXPERIMENT_ID {ARGUMENT_IS_MANDATORY}")
-        url = f"{client.Default.gpu_projects_path()}/pipelines/experiment/{experiment_id}/"
+        url = f"{client.Default.gpu_projects_path()}/pipelines/experiments/{experiment_id}/"
         req = requests.Request('GET', url)
         response = client.Default.make_request(req)
         return prepare_object(response)
 
     def delete_experiment(
         self,
         experiment_id: str = '',
     ):
 
         if not experiment_id:
             raise ValueError(f"EXPERIMENT_ID {ARGUMENT_IS_MANDATORY}")
 
-        url = f"{client.Default.gpu_projects_path()}/pipelines/experiment/{experiment_id}/"
+        url = f"{client.Default.gpu_projects_path()}/pipelines/experiments/{experiment_id}/"
         req = requests.Request('DELETE', url)
         response = client.Default.make_request(req)
         return prepare_object(response)
 
     def create_run(
         self,
         name: str,
@@ -187,43 +190,43 @@
         pipeline_version_id: str = '',
     ):
         if not plan_name:
             return ValueError(f"plan_name is necessary")
         if not name or not experiment_id or not pipeline_version_id:
             raise ValueError(f"name, experiment_id, pipeline_version_id {ARGUMENT_IS_MANDATORY}")
         skus, skus_table = Plans().get_plans_list(PIPELINE)
-        payloads = {"name": name,
+        payloads = json.dumps({"name": name,
                     "description": description,
                     "experiment_id": experiment_id,
                     "sku_item_price_id": plan_name_to_sku_item_price_id(skus, plan_name),
-                    "pipeline_version_id": pipeline_version_id}
-        url = f"{client.Default.gpu_projects_path()}/pipelines/runs/"
-        req = requests.Request(method='POST', url=url, data=payloads)
-        response = client.Default.make_request(req)
-        return prepare_object(response)
+                    "pipeline_version_id": pipeline_version_id})
+        headers['Authorization'] = f'Bearer {client.Default.access_token()}'
+        url = f"{client.Default.gpu_projects_path()}/pipelines/runs/?apikey={client.Default.api_key()}"
+        response = requests.post(url=url, headers=headers, data=payloads)
+        return response
 
     def list_runs(self):
         url = f"{client.Default.gpu_projects_path()}/pipelines/runs/"
         req = requests.Request('GET', url)
         response = client.Default.make_request(req)
         return prepare_object(response)
 
     def get_run(self, run_id):
         if not run_id:
             raise ValueError(f"RUN_ID {ARGUMENT_IS_MANDATORY}")
-        url = f"{client.Default.gpu_projects_path()}/pipelines/run/{run_id}/"
+        url = f"{client.Default.gpu_projects_path()}/pipelines/runs/{run_id}/"
         req = requests.Request('GET', url)
         response = client.Default.make_request(req)
         return prepare_object(response)
 
     def delete_run(self, run_id):
         if not run_id:
             raise ValueError(f"RUN_ID {ARGUMENT_IS_MANDATORY}")
 
-        url = f"{client.Default.gpu_projects_path()}/pipelines/run/{run_id}/"
+        url = f"{client.Default.gpu_projects_path()}/pipelines/runs/{run_id}/"
         req = requests.Request('DELETE', url)
         response = client.Default.make_request(req)
         return prepare_object(response)
 
     @staticmethod
     def help():
         help_text = """
```

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/projects.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/projects.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import requests
+import json
 
+from typing import Dict
 from typing import Optional
 from e2enetworks.constants import BASE_GPU_URL
 from e2enetworks.cloud.tir import client
 from e2enetworks.cloud.tir.utils import prepare_object
+from e2enetworks.constants import headers
 
 
 class Projects:
     def __init__(
             self,
             team: Optional[str] = ""
     ):
@@ -18,21 +21,28 @@
         if not client.Default.ready():
             raise ValueError(client_not_ready)
 
         if team:
             client.Default.set_team(team)
 
     def create(self, project_name):
-        payload = {
-            "project_name": project_name,
-        }
-        url = f"{BASE_GPU_URL}teams/{client.Default.team()}/projects/"
-        req = requests.Request('POST', url, data=payload)
-        response = client.Default.make_request(req)
+        try:
+            payload = json.dumps({
+                "project_name": project_name
+            })
+        except Exception as e:
+            raise Exception(f"Input Error {e}")
+        headers['Authorization'] = f'Bearer {client.Default.access_token()}'
+        url = f"{BASE_GPU_URL}teams/{client.Default.team()}/projects/?apikey={client.Default.api_key()}"
+        response = requests.post(url=url, headers=headers, data=payload)
+        if response.status_code == 201:
+            print("Created successfully")
         return prepare_object(response)
+         
+
 
     def get(self, project_id):
 
         if type(project_id) != int:
             raise ValueError(project_id)
 
         url = f"{BASE_GPU_URL}teams/{client.Default.team()}/projects/{project_id}/"
```

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/skus.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/skus.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,64 +13,83 @@
         client_not_ready = (
             "Client is not ready. Please initiate client by:"
             "\n- Using e2enetworks.cloud.tir.init(...)"
         )
         if not client.Default.ready():
             raise ValueError(client_not_ready)
 
-    def list_endpoint_plans(self):
-        skus = self.list(INFERENCE)
+    def list_endpoint_plans(self,framework=None):
+        skus = self.list(INFERENCE,framework=framework)
 
         for sku in skus["CPU"]:
             if sku.get("is_inventory_available") and not sku["is_free"]:
                 print(cpu_plan_short_code(sku))
         for sku in skus["GPU"]:
             if sku.get("is_inventory_available") and not sku["is_free"]:
                 print(gpu_plan_short_code(sku))
 
-    def list(self, service, image=None):
+    def list(self, service, image_version_id=None, model_id=None, framework=None):
 
         if type(service) != str:
             print(f"Service - {service} Should be String")
             return
+        
+        Attributes = [NOTEBOOK,PIPELINE,INFERENCE]
+        if service not in Attributes :
+            raise ValueError("service must be in %s" % Attributes)
 
-        if service == NOTEBOOK and type(image) != str:
-            print(f"Image ID - {image} Should be String")
+        if service == NOTEBOOK and image_version_id and type(image_version_id) != int:
+            print(f"Image ID - {image_version_id} Should be Integer")
             return
-        image = image if image else ""
-        url = f"{BASE_GPU_URL}gpu_service/sku/?image_id={image}&service={service}&"
+
+        if service == PIPELINE and model_id and type(model_id) != int:
+            print(f"Image ID - {image_version_id} Should be Integer")
+            return
+
+        if service == INFERENCE and not framework :
+            raise ValueError("framework is required")
+        
+        if service == INFERENCE and type(framework) != str:
+            print(f"Image ID - {framework} Should be String")
+            return
+        
+        url = f"{BASE_GPU_URL}gpu_service/sku/"
+        
+        if service == INFERENCE :
+            url = f"{BASE_GPU_URL}gpu_service/sku/?framework={framework}&service={service}&"
+        
+        if service == NOTEBOOK :
+            image_version_id = image_version_id if image_version_id else ""
+            url = f"{BASE_GPU_URL}gpu_service/sku/?image_version_id={image_version_id}&service={service}&"
+
+        if service == PIPELINE :
+            model_id = model_id if model_id else ""
+            url = f"{BASE_GPU_URL}gpu_service/sku/?model_id={model_id}&service={service}&"
+        
         req = requests.Request('GET', url)
         response = client.Default.make_request(req)
         skus = {}
         if response.status_code == 200:
             skus = response.json()["data"]
         return skus
 
-    def get_skus_list(self, service, image=None):
-        image = image if image else ""
-        url = f"{BASE_GPU_URL}gpu_service/sku/?image_id={image}&service={service}&"
-        req = requests.Request('GET', url)
-        response = client.Default.make_request(req)
-        return response.json()["data"] if response.status_code == 200 else prepare_object(response)
+    def get_skus_list(self, service, image_version_id=None, model_id=None, framework=None):
+        return self.list(service, image_version_id, model_id, framework)
 
-    def get_plans_name(self, service, image=None):
-            if service not in [INFERENCE, NOTEBOOK, PIPELINE]:
-                raise ValueError("Invalid service name")
-            image = str(image) if image else ""
-            plans = self.list(service, image)
+    def get_plans_name(self, service, image_version_id=None, model_id=None, framework=None):
+            plans = self.list(service, image_version_id, model_id, framework)
             for sku in plans["CPU"]:
                 if sku.get("is_inventory_available") and not sku["is_free"]:
                     print(cpu_plan_short_code(sku))
             for sku in plans["GPU"]:
                 if sku.get("is_inventory_available") and not sku["is_free"]:
                     print(gpu_plan_short_code(sku))
 
-    def get_plans_list(self, service, image=None):
-        image = str(image) if image else ""
-        plans = self.list(service, image)
+    def get_plans_list(self, service, image_version_id=None, model_id=None, framework=None):
+        plans = self.list(service, image_version_id, model_id, framework)
         cpu_skus, gpu_skus = plans["CPU"], plans["GPU"]
         plans_table = PrettyTable()
         plans_table.field_names = ['name', 'series', 'cpu', 'gpu', 'memory',
                                    'sku_item_price_id', 'sku_type', 'committed_days', 'unit_price']
         self.insert_plans_in_table(cpu_skus, plans_table)
         self.insert_plans_in_table(gpu_skus, plans_table)
         return plans, plans_table
```

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/teams.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/teams.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.5/e2enetworks/cloud/tir/utils.py` & `e2enetworks-1.2.6/e2enetworks/cloud/tir/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 
 def prepare_object(response: Response):
     if not response.ok:
         try:
             output = response.json()
         except:
             output = response.reason
-        print("failed to load response:", output)
-        return None
+        print("ERROR:", output.get('errors'))
+        return response.json().get('errors')
+    
+    flag = response.json().get('data')
     response = load_json(response.content, object_hook=lambda d: SimpleNamespace(**d))
-    return response.data if hasattr(response, "data") else response
+    return response.data if hasattr(response, "data") and flag  else response.message
 
 
 def prepare_response(response: Response) -> Dict:
     if response.ok:
         return load_json(response.content)
 
     # logger.error("")
```

### Comparing `e2enetworks-1.2.5/e2enetworks/constants.py` & `e2enetworks-1.2.6/e2enetworks/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 BASE_URL_MODEL_API_CLIENT = os.environ.get("MODEL_API_CLIENT_HOST", "https://infer.e2enetworks.net/")
-MY_ACCOUNT_LB_URL = os.environ.get("E2E_TIR_API_HOST", "https://api-thor.e2enetworks.net/myaccount/")
+MY_ACCOUNT_LB_URL = os.environ.get("E2E_TIR_API_HOST", "https://api.e2enetworks.com/myaccount/")
 
 GPU_URL = "api/v1/gpu/"
 BASE_GPU_URL = f"{MY_ACCOUNT_LB_URL}{GPU_URL}"
 VALIDATED_SUCCESSFULLY = "Validated Successfully"
 INVALID_CREDENTIALS = "Validation Failed, Invalid APIkey or Token"
 headers = {
     'Connection': 'keep-alive',
@@ -23,23 +23,47 @@
     MANAGED_STORAGE: "To Create New Bucket",
     E2E_OBJECT_STORAGE: " To Use Existing Bucket"
 }
 NOTEBOOK = "notebook"
 INFERENCE = "inference_service"
 PIPELINE = "pipeline"
 
+PRIVATE = "private"
+CUSTOM = "custom"
+REGISTRY = "registry.e2enetworks.net"
 FREE_USAGE = "free_usage"
 PAID_USAGE = "paid_usage"
 INSTANCE_TYPE = [FREE_USAGE, PAID_USAGE]
 TRITON = "triton"
+TENSORRT = "tensorrt"
 PYTORCH = "pytorch"
 MODEL_TYPES = ['pytorch', 'triton', 'custom']
 S3_ENDPOINT = "objectstore.e2enetworks.net"
 
 WHISPER_DATA_LIMIT_BYTES = 50000000
 WHISPER_LARGE_V3 = "whisper-large-v3"
 LLAMA_2_13B_CHAT = "llama-2-13b-chat"
 STABLE_DIFFUSION_2_1 = "stable-diffusion-2-1"
 MIXTRAL_8X7B_INSTRUCT = "mixtral-8x7b-instruct"
 CODELLAMA_13B_INSTRUCT = "codellama-13b-instruct"
 E5_MISTRAL_7B_INSTRUCT = "e5-mistral-7b-instruct"
-LLAMA_3_8B_INSTRUCT = "llama-3-8b-instruct"
+AUTO_RENEW_STATUS = 'auto_renew'
+AUTO_TERMINATE_STATUS = 'auto_terminate'
+CONVERT_TO_HOURLY_BILLING = 'convert_to_hourly_billing'
+LLAMA_3_8B_INSTRUCT = "llama-3-8b-instruct"
+LLMA = "llma"
+STABLE_DIFFUSION = "stable_diffusion"
+MPT = "mpt"
+CODE_LLAMA = "codellama"
+FINETUNED = "finetuned"
+MIXTRAL8X7B = 'mixtral8x7b'
+MIXTRAL7B = 'mixtral7b'
+MIXTRAL7B_INSTRUCT = "mistral-7b-instruct"
+MIXTRAL8X7B_INSTRUCT = "mixtral-8x7b-instruct"
+GEMMA_7B_IT = "gemma-7b-it"
+GEMMA_7B = "gemma-7b"
+GEMMA_2B = "gemma-2b"
+GEMMA_2B_IT = "gemma-2b-it"
+PHI_3_MINI_128K_INSTRUCT = "Phi-3-mini-128k-instruct"
+STARCODER2_7B = "starcoder2-7b"
+VLLM = "vllm"
+TIR_CUSTOM_FRAMEWORKS = [LLMA, STABLE_DIFFUSION, MPT, CODE_LLAMA, MIXTRAL7B, MIXTRAL8X7B, MIXTRAL7B_INSTRUCT, MIXTRAL8X7B_INSTRUCT, GEMMA_7B_IT, GEMMA_7B, GEMMA_2B, GEMMA_2B_IT, TENSORRT, PYTORCH, TRITON, LLAMA_3_8B_INSTRUCT, VLLM, STARCODER2_7B, PHI_3_MINI_128K_INSTRUCT]
```

### Comparing `e2enetworks-1.2.5/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-1.2.6/e2enetworks.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 1.2.5
+Version: 1.2.6
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: System Administrators
@@ -23,7 +23,12 @@
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: urllib3
+Requires-Dist: minio
+Requires-Dist: prettytable
+Requires-Dist: tqdm
```

### Comparing `e2enetworks-1.2.5/e2enetworks.egg-info/SOURCES.txt` & `e2enetworks-1.2.6/e2enetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.5/setup.py` & `e2enetworks-1.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "1.2.5"
+version = "1.2.6"
 install_requires = [
     "requests",
     "urllib3",
     "minio",
     "prettytable",
     "tqdm"
 ]
```

