# Comparing `tmp/sevenapps_py_easy-0.0.3.tar.gz` & `tmp/sevenapps_py_easy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sevenapps_py_easy-0.0.3.tar", last modified: Fri May 24 20:55:03 2024, max compression
+gzip compressed data, was "sevenapps_py_easy-0.0.4.tar", last modified: Fri May 24 21:44:16 2024, max compression
```

## Comparing `sevenapps_py_easy-0.0.3.tar` & `sevenapps_py_easy-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 20:55:03.393181 sevenapps_py_easy-0.0.3/
--rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.3/LICENSE
--rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-24 20:55:03.393110 sevenapps_py_easy-0.0.3/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      117 2024-05-23 21:49:37.000000 sevenapps_py_easy-0.0.3/README.md
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 20:55:03.390756 sevenapps_py_easy-0.0.3/services/
--rw-r--r--   0 jjimenez   (502) staff       (20)       84 2024-05-24 08:17:24.000000 sevenapps_py_easy-0.0.3/services/__init__.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     2615 2024-05-23 23:36:20.000000 sevenapps_py_easy-0.0.3/services/google_firestore_connector.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     2648 2024-05-24 08:15:19.000000 sevenapps_py_easy-0.0.3/services/google_services_connector.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     3201 2024-05-23 10:01:03.000000 sevenapps_py_easy-0.0.3/services/selenium_connector.py
--rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-24 20:55:03.393397 sevenapps_py_easy-0.0.3/setup.cfg
--rw-r--r--   0 jjimenez   (502) staff       (20)      484 2024-05-24 08:17:54.000000 sevenapps_py_easy-0.0.3/setup.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 20:55:03.392792 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/
--rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-24 20:55:03.000000 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      409 2024-05-24 20:55:03.000000 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/SOURCES.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-24 20:55:03.000000 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/dependency_links.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)       38 2024-05-24 20:55:03.000000 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/requires.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)       15 2024-05-24 20:55:03.000000 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/top_level.txt
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 20:55:03.392240 sevenapps_py_easy-0.0.3/utils/
--rw-r--r--   0 jjimenez   (502) staff       (20)       25 2024-05-23 22:56:42.000000 sevenapps_py_easy-0.0.3/utils/__init__.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     1517 2024-05-16 15:30:33.000000 sevenapps_py_easy-0.0.3/utils/file_manager.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:44:16.227084 sevenapps_py_easy-0.0.4/
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.4/LICENSE
+-rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-24 21:44:16.227025 sevenapps_py_easy-0.0.4/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      162 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.4/README.md
+-rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-24 21:44:16.227261 sevenapps_py_easy-0.0.4/setup.cfg
+-rw-r--r--   0 jjimenez   (502) staff       (20)      484 2024-05-24 21:44:13.000000 sevenapps_py_easy-0.0.4/setup.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:44:16.224974 sevenapps_py_easy-0.0.4/sevenapps/
+-rw-r--r--   0 jjimenez   (502) staff       (20)       42 2024-05-24 21:42:35.000000 sevenapps_py_easy-0.0.4/sevenapps/__init__.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:44:16.225575 sevenapps_py_easy-0.0.4/sevenapps/services/
+-rw-r--r--   0 jjimenez   (502) staff       (20)      117 2024-05-24 21:43:32.000000 sevenapps_py_easy-0.0.4/sevenapps/services/__init__.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     2615 2024-05-23 23:36:20.000000 sevenapps_py_easy-0.0.4/sevenapps/services/google_firestore_connector.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     2658 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.4/sevenapps/services/google_services_connector.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     3211 2024-05-24 21:23:17.000000 sevenapps_py_easy-0.0.4/sevenapps/services/selenium_connector.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:44:16.225829 sevenapps_py_easy-0.0.4/sevenapps/utils/
+-rw-r--r--   0 jjimenez   (502) staff       (20)       27 2024-05-24 21:42:57.000000 sevenapps_py_easy-0.0.4/sevenapps/utils/__init__.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1517 2024-05-16 15:30:33.000000 sevenapps_py_easy-0.0.4/sevenapps/utils/file_manager.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 21:44:16.226768 sevenapps_py_easy-0.0.4/sevenapps_py_easy.egg-info/
+-rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-24 21:44:16.000000 sevenapps_py_easy-0.0.4/sevenapps_py_easy.egg-info/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      491 2024-05-24 21:44:16.000000 sevenapps_py_easy-0.0.4/sevenapps_py_easy.egg-info/SOURCES.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-24 21:44:16.000000 sevenapps_py_easy-0.0.4/sevenapps_py_easy.egg-info/dependency_links.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)       38 2024-05-24 21:44:16.000000 sevenapps_py_easy-0.0.4/sevenapps_py_easy.egg-info/requires.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)       10 2024-05-24 21:44:16.000000 sevenapps_py_easy-0.0.4/sevenapps_py_easy.egg-info/top_level.txt
```

### Comparing `sevenapps_py_easy-0.0.3/LICENSE` & `sevenapps_py_easy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.3/services/google_firestore_connector.py` & `sevenapps_py_easy-0.0.4/sevenapps/services/google_firestore_connector.py`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.3/services/google_services_connector.py` & `sevenapps_py_easy-0.0.4/sevenapps/services/google_services_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from googleapiclient.discovery import build
 from googleapiclient.http import MediaFileUpload
 from google.oauth2.service_account import Credentials
 import gspread
-from utils.file_manager import *
+from sevenapps.utils.file_manager import *
 
 
 class GoogleServicesConnector:
 
     def __init__(self, config, credentials_file_path):
         self.credentials_file_path = credentials_file_path
         self.gspread_client = None
```

### Comparing `sevenapps_py_easy-0.0.3/services/selenium_connector.py` & `sevenapps_py_easy-0.0.4/sevenapps/services/selenium_connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from utils.file_manager import *
+from sevenapps.utils.file_manager import *
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.action_chains import ActionChains
```

### Comparing `sevenapps_py_easy-0.0.3/utils/file_manager.py` & `sevenapps_py_easy-0.0.4/sevenapps/utils/file_manager.py`

 * *Files identical despite different names*

