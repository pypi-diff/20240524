# Comparing `tmp/train_traveler_api-0.1.0a1716562459.tar.gz` & `tmp/train_traveler_api-0.1.0a1716563972.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "train_traveler_api-0.1.0a1716562459.tar", last modified: Fri May 24 14:54:18 2024, max compression
+gzip compressed data, was "train_traveler_api-0.1.0a1716563972.tar", last modified: Fri May 24 15:19:32 2024, max compression
```

## Comparing `train_traveler_api-0.1.0a1716562459.tar` & `train_traveler_api-0.1.0a1716563972.tar`

### file list

```diff
@@ -1,11 +1,51 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 14:54:18.832209 train_traveler_api-0.1.0a1716562459/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2024-05-24 14:04:47.000000 train_traveler_api-0.1.0a1716562459/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4415 2024-05-24 14:54:18.832209 train_traveler_api-0.1.0a1716562459/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3997 2024-05-24 14:51:26.000000 train_traveler_api-0.1.0a1716562459/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-05-24 14:54:18.832209 train_traveler_api-0.1.0a1716562459/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      696 2024-05-24 14:53:45.000000 train_traveler_api-0.1.0a1716562459/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 14:54:18.832209 train_traveler_api-0.1.0a1716562459/train_traveler_api.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4415 2024-05-24 14:54:18.000000 train_traveler_api-0.1.0a1716562459/train_traveler_api.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      194 2024-05-24 14:54:18.000000 train_traveler_api-0.1.0a1716562459/train_traveler_api.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-24 14:54:18.000000 train_traveler_api-0.1.0a1716562459/train_traveler_api.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-24 14:54:18.000000 train_traveler_api-0.1.0a1716562459/train_traveler_api.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.460365 train_traveler_api-0.1.0a1716563972/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1073 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4432 2024-05-24 15:19:32.460365 train_traveler_api-0.1.0a1716563972/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4001 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-05-24 15:19:32.460365 train_traveler_api-0.1.0a1716563972/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      836 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/connections/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/connections/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      231 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/connections/connection_manager.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/entities/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1681 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/disruption_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      136 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/entity_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      621 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/information_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1749 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/journey_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      444 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/line_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      295 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/link_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      529 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/place_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      409 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/public_transport_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      762 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/stop_date_time_entity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      729 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/entities/stop_entity.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/models/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/models/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      191 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/models/area_model.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      295 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/models/journey_model.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      270 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/models/next_journey_model.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/repositories/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4395 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/disruption_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8339 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/journey_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1833 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/line_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1323 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/link_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1619 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/place_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2261 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/repository_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3637 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/stop_area_repository.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      392 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/repositories/stop_point_repository.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.450365 train_traveler_api-0.1.0a1716563972/sncf/services/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/services/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      449 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/services/area_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      379 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/services/info_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6944 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/services/journey_service.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       70 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/services/service_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9035 2024-05-24 15:16:19.000000 train_traveler_api-0.1.0a1716563972/sncf/train_traveler.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-24 15:19:32.460365 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4432 2024-05-24 15:19:32.000000 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1320 2024-05-24 15:19:32.000000 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-24 15:19:32.000000 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       60 2024-05-24 15:19:32.000000 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        5 2024-05-24 15:19:32.000000 train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/top_level.txt
```

### Comparing `train_traveler_api-0.1.0a1716562459/LICENSE` & `train_traveler_api-0.1.0a1716563972/LICENSE`

 * *Files identical despite different names*

### Comparing `train_traveler_api-0.1.0a1716562459/PKG-INFO` & `train_traveler_api-0.1.0a1716563972/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: train-traveler-api
-Version: 0.1.0a1716562459
-Summary: Train traveler is a backend for SNCF API
-Home-page: https://github.com/Matthyeux/train-traveler-api
-Author: Matthieu DURINDEL
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Train Traveler
 
 > **Warning**
 > 
 > **Train Traveler is currently under construction and is in alpha stage. Use at your own risk. Features and functionality may change.**
 
 
@@ -67,15 +55,15 @@
 from sncf.services.journey_service import JourneyService
 
 
 # Initialize the client with your API key
 # url = https://api.sncf.com/v1
 # api_key = your api key
 # region = sncf
-client = ApiConnectionManager(url, api_key, region)
+connection = ApiConnectionManager(url, api_key, region)
 
 # Initiatlize journey_service
 journey_service = JourneyService(
     stop_area_repository=ApiStopAreaRepository(connection),
     journey_repository=ApiJourneyRepository(connection),
     disruption_repository=ApiDisruptionRepository(connection)
 )
@@ -126,8 +114,8 @@
     Create your feature branch (git checkout -b feature/AmazingFeature)
     Commit your changes (git commit -m 'Add some AmazingFeature')
     Push to the branch (git push origin feature/AmazingFeature)
     Open a Pull Request
 
 ## License
 
-Distributed under the MIT License. See LICENSE for more information.
+Distributed under the MIT License. See LICENSE for more information.
```

### Comparing `train_traveler_api-0.1.0a1716562459/README.md` & `train_traveler_api-0.1.0a1716563972/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: train-traveler-api
+Version: 0.1.0a1716563972
+Summary: Train traveler is a backend for SNCF API
+Home-page: https://github.com/Matthyeux/train-traveler-api
+Author: Matthieu DURINDEL
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Train Traveler
 
 > **Warning**
 > 
 > **Train Traveler is currently under construction and is in alpha stage. Use at your own risk. Features and functionality may change.**
 
 
@@ -55,15 +68,15 @@
 from sncf.services.journey_service import JourneyService
 
 
 # Initialize the client with your API key
 # url = https://api.sncf.com/v1
 # api_key = your api key
 # region = sncf
-client = ApiConnectionManager(url, api_key, region)
+connection = ApiConnectionManager(url, api_key, region)
 
 # Initiatlize journey_service
 journey_service = JourneyService(
     stop_area_repository=ApiStopAreaRepository(connection),
     journey_repository=ApiJourneyRepository(connection),
     disruption_repository=ApiDisruptionRepository(connection)
 )
@@ -114,8 +127,8 @@
     Create your feature branch (git checkout -b feature/AmazingFeature)
     Commit your changes (git commit -m 'Add some AmazingFeature')
     Push to the branch (git push origin feature/AmazingFeature)
     Open a Pull Request
 
 ## License
 
-Distributed under the MIT License. See LICENSE for more information.
+Distributed under the MIT License. See LICENSE for more information.
```

### Comparing `train_traveler_api-0.1.0a1716562459/setup.py` & `train_traveler_api-0.1.0a1716563972/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 setup(
     name="train-traveler-api",
     version=f"0.1.0-alpha.{int(round(datetime.timestamp(datetime.now())))}",
     author="Matthieu DURINDEL",
     description="Train traveler is a backend for SNCF API",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    license="MIT",
     url="https://github.com/Matthyeux/train-traveler-api",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-    ]
+    ],
+    entry_points={
+        'console_scripts': [
+            'train-traveler=sncf.train_traveler:main',
+        ],
+    }
 )
```

### Comparing `train_traveler_api-0.1.0a1716562459/train_traveler_api.egg-info/PKG-INFO` & `train_traveler_api-0.1.0a1716563972/train_traveler_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: train-traveler-api
-Version: 0.1.0a1716562459
+Version: 0.1.0a1716563972
 Summary: Train traveler is a backend for SNCF API
 Home-page: https://github.com/Matthyeux/train-traveler-api
 Author: Matthieu DURINDEL
+License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Train Traveler
@@ -67,15 +68,15 @@
 from sncf.services.journey_service import JourneyService
 
 
 # Initialize the client with your API key
 # url = https://api.sncf.com/v1
 # api_key = your api key
 # region = sncf
-client = ApiConnectionManager(url, api_key, region)
+connection = ApiConnectionManager(url, api_key, region)
 
 # Initiatlize journey_service
 journey_service = JourneyService(
     stop_area_repository=ApiStopAreaRepository(connection),
     journey_repository=ApiJourneyRepository(connection),
     disruption_repository=ApiDisruptionRepository(connection)
 )
```

