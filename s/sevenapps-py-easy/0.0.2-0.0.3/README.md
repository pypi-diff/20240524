# Comparing `tmp/sevenapps_py_easy-0.0.2.tar.gz` & `tmp/sevenapps_py_easy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sevenapps_py_easy-0.0.2.tar", last modified: Thu May 23 22:56:53 2024, max compression
+gzip compressed data, was "sevenapps_py_easy-0.0.3.tar", last modified: Fri May 24 20:55:03 2024, max compression
```

## Comparing `sevenapps_py_easy-0.0.2.tar` & `sevenapps_py_easy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-23 22:56:53.574802 sevenapps_py_easy-0.0.2/
--rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.2/LICENSE
--rw-r--r--   0 jjimenez   (502) staff       (20)      316 2024-05-23 22:56:53.574739 sevenapps_py_easy-0.0.2/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      117 2024-05-23 21:49:37.000000 sevenapps_py_easy-0.0.2/README.md
--rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-23 22:56:53.575044 sevenapps_py_easy-0.0.2/setup.cfg
--rw-r--r--   0 jjimenez   (502) staff       (20)      395 2024-05-23 22:56:49.000000 sevenapps_py_easy-0.0.2/setup.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-23 22:56:53.574560 sevenapps_py_easy-0.0.2/sevenapps_py_easy.egg-info/
--rw-r--r--   0 jjimenez   (502) staff       (20)      316 2024-05-23 22:56:53.000000 sevenapps_py_easy-0.0.2/sevenapps_py_easy.egg-info/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      240 2024-05-23 22:56:53.000000 sevenapps_py_easy-0.0.2/sevenapps_py_easy.egg-info/SOURCES.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-23 22:56:53.000000 sevenapps_py_easy-0.0.2/sevenapps_py_easy.egg-info/dependency_links.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)        6 2024-05-23 22:56:53.000000 sevenapps_py_easy-0.0.2/sevenapps_py_easy.egg-info/top_level.txt
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-23 22:56:53.574305 sevenapps_py_easy-0.0.2/utils/
--rw-r--r--   0 jjimenez   (502) staff       (20)       25 2024-05-23 22:56:42.000000 sevenapps_py_easy-0.0.2/utils/__init__.py
--rw-r--r--   0 jjimenez   (502) staff       (20)     1517 2024-05-16 15:30:33.000000 sevenapps_py_easy-0.0.2/utils/file_manager.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 20:55:03.393181 sevenapps_py_easy-0.0.3/
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.3/LICENSE
+-rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-24 20:55:03.393110 sevenapps_py_easy-0.0.3/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      117 2024-05-23 21:49:37.000000 sevenapps_py_easy-0.0.3/README.md
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 20:55:03.390756 sevenapps_py_easy-0.0.3/services/
+-rw-r--r--   0 jjimenez   (502) staff       (20)       84 2024-05-24 08:17:24.000000 sevenapps_py_easy-0.0.3/services/__init__.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     2615 2024-05-23 23:36:20.000000 sevenapps_py_easy-0.0.3/services/google_firestore_connector.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     2648 2024-05-24 08:15:19.000000 sevenapps_py_easy-0.0.3/services/google_services_connector.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     3201 2024-05-23 10:01:03.000000 sevenapps_py_easy-0.0.3/services/selenium_connector.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-24 20:55:03.393397 sevenapps_py_easy-0.0.3/setup.cfg
+-rw-r--r--   0 jjimenez   (502) staff       (20)      484 2024-05-24 08:17:54.000000 sevenapps_py_easy-0.0.3/setup.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 20:55:03.392792 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/
+-rw-r--r--   0 jjimenez   (502) staff       (20)      384 2024-05-24 20:55:03.000000 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      409 2024-05-24 20:55:03.000000 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/SOURCES.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-24 20:55:03.000000 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/dependency_links.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)       38 2024-05-24 20:55:03.000000 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/requires.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)       15 2024-05-24 20:55:03.000000 sevenapps_py_easy-0.0.3/sevenapps_py_easy.egg-info/top_level.txt
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-24 20:55:03.392240 sevenapps_py_easy-0.0.3/utils/
+-rw-r--r--   0 jjimenez   (502) staff       (20)       25 2024-05-23 22:56:42.000000 sevenapps_py_easy-0.0.3/utils/__init__.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1517 2024-05-16 15:30:33.000000 sevenapps_py_easy-0.0.3/utils/file_manager.py
```

### Comparing `sevenapps_py_easy-0.0.2/LICENSE` & `sevenapps_py_easy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sevenapps_py_easy-0.0.2/utils/file_manager.py` & `sevenapps_py_easy-0.0.3/utils/file_manager.py`

 * *Files identical despite different names*

