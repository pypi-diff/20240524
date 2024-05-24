# Comparing `tmp/wizata_dsapi-1.0.5.tar.gz` & `tmp/wizata-dsapi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata_dsapi-1.0.5.tar", last modified: Mon May 20 09:39:27 2024, max compression
+gzip compressed data, was "wizata-dsapi-1.0.6.tar", last modified: Fri May 24 08:55:28 2024, max compression
```

## Comparing `wizata_dsapi-1.0.5.tar` & `wizata-dsapi-1.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-20 09:39:27.549099 wizata_dsapi-1.0.5/
--rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata_dsapi-1.0.5/LICENSE.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1284 2024-05-20 09:39:27.548886 wizata_dsapi-1.0.5/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata_dsapi-1.0.5/README.rst
--rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2024-05-20 09:39:27.549142 wizata_dsapi-1.0.5/setup.cfg
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1445 2024-05-20 09:38:32.000000 wizata_dsapi-1.0.5/setup.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-20 09:39:27.546465 wizata_dsapi-1.0.5/wizata_dsapi/
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1557 2024-05-16 13:17:14.000000 wizata_dsapi-1.0.5/wizata_dsapi/__init__.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3875 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/api_config.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1172 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/api_dto.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     9270 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/api_interface.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4151 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/business_label.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10084 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/context.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     8472 2024-05-16 13:17:14.000000 wizata_dsapi-1.0.5/wizata_dsapi/dataframe_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10822 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/datapoint.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2089 2024-03-06 07:51:32.000000 wizata_dsapi-1.0.5/wizata_dsapi/ds_dataframe.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata_dsapi-1.0.5/wizata_dsapi/dsapi_json_encoder.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12777 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/execution.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4355 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/experiment.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      807 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/ilogger.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    14587 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/mlmodel.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1551 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/model_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1150 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/paged_query_result.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    28788 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/pipeline.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2355 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/plot.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    19308 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12710 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/script.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     7625 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/solution_component.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12451 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/template.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4769 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/trigger.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     6291 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/twin.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12865 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/twinregistration.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)       22 2024-05-20 09:38:32.000000 wizata_dsapi-1.0.5/wizata_dsapi/version.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      942 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/wizard_function.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3762 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/wizard_request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    68678 2024-05-07 11:09:47.000000 wizata_dsapi-1.0.5/wizata_dsapi/wizata_dsapi_client.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1535 2024-03-20 11:49:55.000000 wizata_dsapi-1.0.5/wizata_dsapi/words.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-20 09:39:27.548143 wizata_dsapi-1.0.5/wizata_dsapi.egg-info/
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1284 2024-05-20 09:39:27.000000 wizata_dsapi-1.0.5/wizata_dsapi.egg-info/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1037 2024-05-20 09:39:27.000000 wizata_dsapi-1.0.5/wizata_dsapi.egg-info/SOURCES.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2024-05-20 09:39:27.000000 wizata_dsapi-1.0.5/wizata_dsapi.egg-info/dependency_links.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      586 2024-05-20 09:39:27.000000 wizata_dsapi-1.0.5/wizata_dsapi.egg-info/requires.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2024-05-20 09:39:27.000000 wizata_dsapi-1.0.5/wizata_dsapi.egg-info/top_level.txt
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-24 08:55:28.865453 wizata-dsapi-1.0.6/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-1.0.6/LICENSE.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-05-24 08:55:28.865324 wizata-dsapi-1.0.6/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-1.0.6/README.rst
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2024-05-24 08:55:28.865504 wizata-dsapi-1.0.6/setup.cfg
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1450 2024-05-22 09:08:26.000000 wizata-dsapi-1.0.6/setup.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-24 08:55:28.864428 wizata-dsapi-1.0.6/wizata_dsapi/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1557 2024-05-16 13:17:14.000000 wizata-dsapi-1.0.6/wizata_dsapi/__init__.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3875 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/api_config.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1172 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/api_dto.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     9270 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/api_interface.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4151 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/business_label.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    10084 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/context.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     8472 2024-05-16 13:17:14.000000 wizata-dsapi-1.0.6/wizata_dsapi/dataframe_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    10822 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/datapoint.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2089 2024-03-06 07:51:32.000000 wizata-dsapi-1.0.6/wizata_dsapi/ds_dataframe.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-1.0.6/wizata_dsapi/dsapi_json_encoder.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    13229 2024-05-24 08:38:26.000000 wizata-dsapi-1.0.6/wizata_dsapi/execution.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4355 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/experiment.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      807 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/ilogger.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    14587 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/mlmodel.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1551 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/model_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1150 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/paged_query_result.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    28788 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/pipeline.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2355 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/plot.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    19308 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12710 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/script.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     7625 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/solution_component.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12451 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/template.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4769 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/trigger.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     6291 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/twin.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12865 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/twinregistration.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       22 2024-05-24 08:55:26.000000 wizata-dsapi-1.0.6/wizata_dsapi/version.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      942 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/wizard_function.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3762 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/wizard_request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    68678 2024-05-07 11:09:47.000000 wizata-dsapi-1.0.6/wizata_dsapi/wizata_dsapi_client.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1535 2024-03-20 11:49:55.000000 wizata-dsapi-1.0.6/wizata_dsapi/words.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-05-24 08:55:28.865126 wizata-dsapi-1.0.6/wizata_dsapi.egg-info/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-05-24 08:55:28.000000 wizata-dsapi-1.0.6/wizata_dsapi.egg-info/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1037 2024-05-24 08:55:28.000000 wizata-dsapi-1.0.6/wizata_dsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2024-05-24 08:55:28.000000 wizata-dsapi-1.0.6/wizata_dsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      591 2024-05-24 08:55:28.000000 wizata-dsapi-1.0.6/wizata_dsapi.egg-info/requires.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2024-05-24 08:55:28.000000 wizata-dsapi-1.0.6/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata_dsapi-1.0.5/LICENSE.txt` & `wizata-dsapi-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/setup.py` & `wizata-dsapi-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,37 +11,37 @@
     name='wizata-dsapi',
     version=main_ns['__version__'],
     description='Wizata Data Science Toolkit',
     author='Wizata S.A.',
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
-        'requests==2.29.0',
-        'dill>=0.3.8',
-        'pandas>=2.2.2',
-        'numpy>=1.26.4',
-        'matplotlib>=3.9.0',
-        'protobuf>=3.20.3',
-        "tensorflow==2.16.1; sys_platform != 'darwin' or platform_machine != 'arm64'",
-        "tensorflow-macos==2.16.1; sys_platform == 'darwin' and platform_machine == 'arm64'",
-        "keras==3.3.3; sys_platform != 'darwin' or platform_machine != 'arm64'",
-        "keras==3.3.3; sys_platform == 'darwin' and platform_machine == 'arm64'",
-        'tensorflow_probability>=0.24.0',
-        'scikit-learn>=1.4.2',
-        'scipy>=1.13.0',
-        'plotly>=5.22.0',
-        'adtk>=0.6.2',
-        'xgboost>=2.0.3',
-        'joblib>=1.4.2',
-        'explainerdashboard>=0.4.7',
-        'ipywidgets>=8.1.2',
-        'kaleido>=0.2.1',
-        'pytest>=8.2.1',
-        'pytest-cov>=5.0.0',
-        'shapely>=2.0.4',
-        'pyodbc>=5.1.0',
+        'dill==0.3.6',
+        'pandas==1.5.3',
+        'numpy==1.23.5',
+        'matplotlib==3.7.1',
+        'protobuf==3.20.3',
+        "tensorflow==2.15.0; sys_platform != 'darwin' or platform_machine != 'arm64'",
+        "tensorflow-macos==2.15.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
+        "keras==2.15.0; sys_platform != 'darwin' or platform_machine != 'arm64'",
+        "keras==2.15.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
+        'tensorflow_probability==0.15.0',
+        'scikit-learn==1.2.2',
+        'plotly==5.13.1',
+        'adtk==0.6.2',
+        'scipy==1.10.1',
+        'xgboost==1.7.4',
+        'joblib==1.2.0',
+        'requests==2.28.2',
+        'setuptools==67.6.0',
+        'explainerdashboard==0.4.2.1',
+        'ipywidgets==8.0.4',
+        'kaleido==0.2.1',
+        'pytest==7.2.2',
+        'pytest-cov==4.0.0',
+        'shapely==2.0.1',
+        'pyodbc==4.0.35',
         'msal>=1.24.0',
-        'u8darts>=0.29.0',
-        'optuna>=3.6.1',
-        'sqlalchemy>=2.0.30'
+        'u8darts==0.25.0',
+        'optuna==3.3.0'
     ]
 )
```

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/__init__.py` & `wizata-dsapi-1.0.6/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/api_config.py` & `wizata-dsapi-1.0.6/wizata_dsapi/api_config.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/api_dto.py` & `wizata-dsapi-1.0.6/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/api_interface.py` & `wizata-dsapi-1.0.6/wizata_dsapi/api_interface.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/business_label.py` & `wizata-dsapi-1.0.6/wizata_dsapi/business_label.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/context.py` & `wizata-dsapi-1.0.6/wizata_dsapi/context.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-1.0.6/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/datapoint.py` & `wizata-dsapi-1.0.6/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-1.0.6/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-1.0.6/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/execution.py` & `wizata-dsapi-1.0.6/wizata_dsapi/execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     """
     execution keeps all information on time, status and results of a specific pipeline manual or automatic run.
 
     :ivar uuid.UUID execution_id: technical id of execution.
     :ivar int execution_time: duration of the execution from started.
     :ivar uuid.UUID experiment_id: experiment id used in experiment mode.
     :ivar uuid.UUID pipeline_id: pipeline id executed or to execute.
+    :ivar uuid.UUID pipeline_image_id: pipeline image package to use instead of current pipeline.
     :ivar dict properties: configuration, parameters and variables (only accessible from front-end to DS api).
     :ivar int queued_date: timestamp on which execution is queued, if none use createdDate
     :ivar int started_date: timestamp on which execution is started.
     :ivar wizata_dsapi.ExecutionStatus status: execution status.
     :ivar uuid.UUID template_id: template id linked to the pipeline.
     :ivar uuid.UUID trigger_id: trigger id used if automatic run.
     :ivar uuid.UUID twin_id: twin id registered on the template to run pipeline on.
@@ -159,14 +160,15 @@
         return obj
 
     def __init__(self,
                  execution_id=None,
                  properties: dict = None,
                  pipeline: Pipeline = None,
                  pipeline_id: uuid.UUID = None,
+                 pipeline_image_id: str = None,
                  experiment: Experiment = None,
                  experiment_id: uuid.UUID = None,
                  twin_id: uuid.UUID = None,
                  template_id: uuid.UUID = None,
                  trigger_id: uuid.UUID = None):
 
         # Id
@@ -186,14 +188,15 @@
         self.template_id = template_id
 
         # Pipeline
         if pipeline is not None:
             self.pipeline_id = pipeline.pipeline_id
         else:
             self.pipeline_id = pipeline_id
+        self.pipeline_image_id = pipeline_image_id
 
         # Status and info
         self.status = None
         self.queued_date = None
         self.started_date = None
         self.execution_time = None
         self.waiting_time = None
@@ -229,14 +232,16 @@
         # Experiment
         if self.experiment_id is not None:
             obj["experimentId"] = str(self.experiment_id)
 
         # Pipeline
         if self.pipeline_id is not None:
             obj["pipelineId"] = str(self.pipeline_id)
+        if self.pipeline_image_id is not None:
+            obj["pipelineImageId"] = str(self.pipeline_image_id)
 
         # Trigger , Twin & Template
         if self.trigger_id is not None:
             obj["executionTriggerId"] = str(self.trigger_id)
         if self.template_id is not None:
             obj["templateId"] = str(self.template_id)
         if self.twin_id is not None:
@@ -279,14 +284,16 @@
         # Experiment
         if "experimentId" in obj.keys() and obj["experimentId"] is not None:
             self.experiment_id = uuid.UUID(obj["experimentId"])
 
         # Pipeline
         if "pipelineId" in obj.keys() and obj["pipelineId"] is not None:
             self.pipeline_id = uuid.UUID(obj["pipelineId"])
+        if "pipelineImageId" in obj.keys() and obj["pipelineImageId"] is not None:
+            self.pipeline_image_id = obj["pipelineImageId"]
 
         # Trigger , Twin & Template
         if "twinId" in obj.keys() and obj["twinId"] is not None:
             self.twin_id = uuid.UUID(obj["twinId"])
         if "templateId" in obj.keys() and obj["templateId"] is not None:
             self.template_id = uuid.UUID(obj["templateId"])
         if "executionTriggerId" in obj.keys() and obj["executionTriggerId"] is not None:
```

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/experiment.py` & `wizata-dsapi-1.0.6/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/ilogger.py` & `wizata-dsapi-1.0.6/wizata_dsapi/ilogger.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/mlmodel.py` & `wizata-dsapi-1.0.6/wizata_dsapi/mlmodel.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-1.0.6/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/paged_query_result.py` & `wizata-dsapi-1.0.6/wizata_dsapi/paged_query_result.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/pipeline.py` & `wizata-dsapi-1.0.6/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/plot.py` & `wizata-dsapi-1.0.6/wizata_dsapi/plot.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/request.py` & `wizata-dsapi-1.0.6/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/script.py` & `wizata-dsapi-1.0.6/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/solution_component.py` & `wizata-dsapi-1.0.6/wizata_dsapi/solution_component.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/template.py` & `wizata-dsapi-1.0.6/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/trigger.py` & `wizata-dsapi-1.0.6/wizata_dsapi/trigger.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/twin.py` & `wizata-dsapi-1.0.6/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/twinregistration.py` & `wizata-dsapi-1.0.6/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/wizard_function.py` & `wizata-dsapi-1.0.6/wizata_dsapi/wizard_function.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/wizard_request.py` & `wizata-dsapi-1.0.6/wizata_dsapi/wizard_request.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-1.0.6/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi/words.py` & `wizata-dsapi-1.0.6/wizata_dsapi/words.py`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-1.0.6/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata_dsapi-1.0.5/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-1.0.6/wizata_dsapi.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-requests==2.29.0
-dill>=0.3.8
-pandas>=2.2.2
-numpy>=1.26.4
-matplotlib>=3.9.0
-protobuf>=3.20.3
-tensorflow_probability>=0.24.0
-scikit-learn>=1.4.2
-scipy>=1.13.0
-plotly>=5.22.0
-adtk>=0.6.2
-xgboost>=2.0.3
-joblib>=1.4.2
-explainerdashboard>=0.4.7
-ipywidgets>=8.1.2
-kaleido>=0.2.1
-pytest>=8.2.1
-pytest-cov>=5.0.0
-shapely>=2.0.4
-pyodbc>=5.1.0
+dill==0.3.6
+pandas==1.5.3
+numpy==1.23.5
+matplotlib==3.7.1
+protobuf==3.20.3
+tensorflow_probability==0.15.0
+scikit-learn==1.2.2
+plotly==5.13.1
+adtk==0.6.2
+scipy==1.10.1
+xgboost==1.7.4
+joblib==1.2.0
+requests==2.28.2
+setuptools==67.6.0
+explainerdashboard==0.4.2.1
+ipywidgets==8.0.4
+kaleido==0.2.1
+pytest==7.2.2
+pytest-cov==4.0.0
+shapely==2.0.1
+pyodbc==4.0.35
 msal>=1.24.0
-u8darts>=0.29.0
-optuna>=3.6.1
-sqlalchemy>=2.0.30
+u8darts==0.25.0
+optuna==3.3.0
 
 [:sys_platform != "darwin" or platform_machine != "arm64"]
-tensorflow==2.16.1
-keras==3.3.3
+tensorflow==2.15.0
+keras==2.15.0
 
 [:sys_platform == "darwin" and platform_machine == "arm64"]
-tensorflow-macos==2.16.1
-keras==3.3.3
+tensorflow-macos==2.15.0
+keras==2.15.0
```

