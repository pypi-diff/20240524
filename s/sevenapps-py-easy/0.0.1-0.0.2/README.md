# Comparing `tmp/sevenapps_py_easy-0.0.1.tar.gz` & `tmp/sevenapps_py_easy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sevenapps_py_easy-0.0.1.tar", last modified: Thu May 23 22:45:25 2024, max compression
+gzip compressed data, was "sevenapps_py_easy-0.0.2.tar", last modified: Thu May 23 22:56:53 2024, max compression
```

## Comparing `sevenapps_py_easy-0.0.1.tar` & `sevenapps_py_easy-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-23 22:45:25.679971 sevenapps_py_easy-0.0.1/
--rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.1/LICENSE
--rw-r--r--   0 jjimenez   (502) staff       (20)      316 2024-05-23 22:45:25.679916 sevenapps_py_easy-0.0.1/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      117 2024-05-23 21:49:37.000000 sevenapps_py_easy-0.0.1/README.md
--rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-23 22:45:25.680215 sevenapps_py_easy-0.0.1/setup.cfg
--rw-r--r--   0 jjimenez   (502) staff       (20)      395 2024-05-23 22:42:28.000000 sevenapps_py_easy-0.0.1/setup.py
-drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-23 22:45:25.679727 sevenapps_py_easy-0.0.1/sevenapps_py_easy.egg-info/
--rw-r--r--   0 jjimenez   (502) staff       (20)      316 2024-05-23 22:45:25.000000 sevenapps_py_easy-0.0.1/sevenapps_py_easy.egg-info/PKG-INFO
--rw-r--r--   0 jjimenez   (502) staff       (20)      200 2024-05-23 22:45:25.000000 sevenapps_py_easy-0.0.1/sevenapps_py_easy.egg-info/SOURCES.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-23 22:45:25.000000 sevenapps_py_easy-0.0.1/sevenapps_py_easy.egg-info/dependency_links.txt
--rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-23 22:45:25.000000 sevenapps_py_easy-0.0.1/sevenapps_py_easy.egg-info/top_level.txt
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-23 22:56:53.574802 sevenapps_py_easy-0.0.2/
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1066 2024-05-23 21:53:57.000000 sevenapps_py_easy-0.0.2/LICENSE
+-rw-r--r--   0 jjimenez   (502) staff       (20)      316 2024-05-23 22:56:53.574739 sevenapps_py_easy-0.0.2/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      117 2024-05-23 21:49:37.000000 sevenapps_py_easy-0.0.2/README.md
+-rw-r--r--   0 jjimenez   (502) staff       (20)       79 2024-05-23 22:56:53.575044 sevenapps_py_easy-0.0.2/setup.cfg
+-rw-r--r--   0 jjimenez   (502) staff       (20)      395 2024-05-23 22:56:49.000000 sevenapps_py_easy-0.0.2/setup.py
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-23 22:56:53.574560 sevenapps_py_easy-0.0.2/sevenapps_py_easy.egg-info/
+-rw-r--r--   0 jjimenez   (502) staff       (20)      316 2024-05-23 22:56:53.000000 sevenapps_py_easy-0.0.2/sevenapps_py_easy.egg-info/PKG-INFO
+-rw-r--r--   0 jjimenez   (502) staff       (20)      240 2024-05-23 22:56:53.000000 sevenapps_py_easy-0.0.2/sevenapps_py_easy.egg-info/SOURCES.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)        1 2024-05-23 22:56:53.000000 sevenapps_py_easy-0.0.2/sevenapps_py_easy.egg-info/dependency_links.txt
+-rw-r--r--   0 jjimenez   (502) staff       (20)        6 2024-05-23 22:56:53.000000 sevenapps_py_easy-0.0.2/sevenapps_py_easy.egg-info/top_level.txt
+drwxr-xr-x   0 jjimenez   (502) staff       (20)        0 2024-05-23 22:56:53.574305 sevenapps_py_easy-0.0.2/utils/
+-rw-r--r--   0 jjimenez   (502) staff       (20)       25 2024-05-23 22:56:42.000000 sevenapps_py_easy-0.0.2/utils/__init__.py
+-rw-r--r--   0 jjimenez   (502) staff       (20)     1517 2024-05-16 15:30:33.000000 sevenapps_py_easy-0.0.2/utils/file_manager.py
```

### Comparing `sevenapps_py_easy-0.0.1/LICENSE` & `sevenapps_py_easy-0.0.2/LICENSE`

 * *Files identical despite different names*

