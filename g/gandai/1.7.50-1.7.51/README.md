# Comparing `tmp/gandai-1.7.50.tar.gz` & `tmp/gandai-1.7.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.50.tar", last modified: Fri May 24 05:49:58 2024, max compression
+gzip compressed data, was "gandai-1.7.51.tar", last modified: Fri May 24 06:44:05 2024, max compression
```

## Comparing `gandai-1.7.50.tar` & `gandai-1.7.51.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:49:58.588800 gandai-1.7.50/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.50/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 05:49:58.588592 gandai-1.7.50/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:49:58.574646 gandai-1.7.50/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.50/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:49:58.585036 gandai-1.7.50/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.50/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.50/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.50/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.50/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2600 2024-05-24 00:47:47.000000 gandai-1.7.50/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.50/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.50/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.50/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7037 2024-05-23 23:56:05.000000 gandai-1.7.50/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.50/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-24 05:31:06.000000 gandai-1.7.50/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    16184 2024-05-24 05:45:46.000000 gandai-1.7.50/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.50/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    42390 2024-05-24 03:52:51.000000 gandai-1.7.50/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.50/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.50/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.50/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1550 2024-05-24 05:49:45.000000 gandai-1.7.50/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.50/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1674 2024-05-24 00:47:46.000000 gandai-1.7.50/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.50/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.50/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)     6395 2024-05-23 23:56:03.000000 gandai-1.7.50/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.50/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-24 05:31:04.000000 gandai-1.7.50/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    11334 2024-05-24 05:45:43.000000 gandai-1.7.50/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:49:58.585838 gandai-1.7.50/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.50/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:49:58.586227 gandai-1.7.50/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.50/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.50/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.50/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.50/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.50/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:49:58.588067 gandai-1.7.50/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.50/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.50/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.50/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.50/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.50/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    28700 2024-05-24 03:52:49.000000 gandai-1.7.50/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.50/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1057 2024-05-24 05:49:43.000000 gandai-1.7.50/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:49:58.588360 gandai-1.7.50/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 05:49:58.000000 gandai-1.7.50/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-24 05:49:58.000000 gandai-1.7.50/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-24 05:49:58.000000 gandai-1.7.50/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-24 05:49:58.000000 gandai-1.7.50/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-24 05:49:53.000000 gandai-1.7.50/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-24 05:49:58.588839 gandai-1.7.50/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.50/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.776359 gandai-1.7.51/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.51/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 06:44:05.776152 gandai-1.7.51/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.769453 gandai-1.7.51/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.51/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.773364 gandai-1.7.51/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.51/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.51/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.51/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.51/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2600 2024-05-24 00:47:47.000000 gandai-1.7.51/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.51/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.51/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.51/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7037 2024-05-23 23:56:05.000000 gandai-1.7.51/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.51/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-24 05:31:06.000000 gandai-1.7.51/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    16151 2024-05-24 06:42:01.000000 gandai-1.7.51/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.51/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    42420 2024-05-24 06:17:33.000000 gandai-1.7.51/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.51/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.51/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.51/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      836 2024-05-24 06:09:06.000000 gandai-1.7.51/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.51/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1674 2024-05-24 00:47:46.000000 gandai-1.7.51/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.51/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.51/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)     6395 2024-05-23 23:56:03.000000 gandai-1.7.51/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.51/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-24 05:31:04.000000 gandai-1.7.51/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    11300 2024-05-24 06:41:58.000000 gandai-1.7.51/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.773862 gandai-1.7.51/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.51/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.774227 gandai-1.7.51/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.51/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.51/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.51/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.51/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.51/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.775595 gandai-1.7.51/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.51/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.51/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.51/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.51/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.51/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    28730 2024-05-24 06:17:30.000000 gandai-1.7.51/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.51/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1056 2024-05-24 06:09:03.000000 gandai-1.7.51/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.775949 gandai-1.7.51/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 06:44:05.000000 gandai-1.7.51/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-24 06:44:05.000000 gandai-1.7.51/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-24 06:44:05.000000 gandai-1.7.51/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-24 06:44:05.000000 gandai-1.7.51/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-24 06:43:57.000000 gandai-1.7.51/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-24 06:44:05.776395 gandai-1.7.51/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.51/setup.py
```

### Comparing `gandai-1.7.50/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x87295066 (Fri May 24 05:45:43 2024 UTC)
-files sz: 11334
+moddate:  0xb6365066 (Fri May 24 06:41:58 2024 UTC)
+files sz: 11300
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d025a020100640064
@@ -138,20 +138,20 @@
                350 LOAD_CONST               8 ('return')
                352 LOAD_CONST               3 (None)
                354 BUILD_TUPLE              4
                356 LOAD_CONST              17 (<code object run_enrichment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 213>)
                358 MAKE_FUNCTION            4 (annotations)
                360 STORE_NAME              19 (run_enrichment)
    
-   233         362 LOAD_CONST              18 ('event_id')
+   232         362 LOAD_CONST              18 ('event_id')
                364 LOAD_NAME               20 (int)
                366 LOAD_CONST               8 ('return')
                368 LOAD_CONST               3 (None)
                370 BUILD_TUPLE              4
-               372 LOAD_CONST              19 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 233>)
+               372 LOAD_CONST              19 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 232>)
                374 MAKE_FUNCTION            4 (annotations)
                376 STORE_NAME              21 (process_event)
                378 LOAD_CONST               3 (None)
                380 RETURN_VALUE
    consts
       0
       ('asdict',)
@@ -1316,157 +1316,152 @@
          firstlineno 174
          lnotab
             0x02011e0102014c0112011e0116fe0805020114fe0405020122fe040502
             0108fe0405020102fe0405020120fe04ef04173e013e01180146011e013e
             01
       code
          argcount  : 1
-         nlocals   : 5
+         nlocals   : 4
          stacksize : 3
          flags     : 3
          code
-            0x97007c006a0000000000000000007d017c006a0100000000000000007d
-            027404000000000000000000006a030000000000000000a0040000000000
-            0000000000000000000000000000007c01a6010000ab0100000000000000
-            007d037c036a050000000000000000a00600000000000000000000000000
-            000000000000006401a6010000ab0100000000000000007210740f000000
-            000000000000006402a6010000ab01000000000000000001006e8e740400
-            0000000000000000006a080000000000000000a009000000000000000000
-            00000000000000000000007c036a000000000000000000a6010000ab0100
-            000000000000007d047c036a0a000000000000000070147c04a006000000
-            00000000000000000000000000000000006403a6010000ab010000000000
-            0000007c035f0a00000000000000007c04a0060000000000000000000000
-            0000000000000000006404a6010000ab0100000000000000007c035f0b00
-            0000000000000069007c036a050000000000000000a5017c04a5017c035f
-            0500000000000000007404000000000000000000006a0300000000000000
-            00a00c00000000000000000000000000000000000000007c03a6010000ab
-            01000000000000000001007c036a050000000000000000a0060000000000
-            0000000000000000000000000000006405a6010000ab0100000000000000
-            007211740f000000000000000000006406a6010000ab0100000000000000
-            00010064005300741b000000000000000000007c03ac07a6010000ab0100
-            00000000000000010064005300
+            0x97007c006a0000000000000000007d017402000000000000000000006a
+            020000000000000000a00300000000000000000000000000000000000000
+            007c01a6010000ab0100000000000000007d027c026a0400000000000000
+            00a00500000000000000000000000000000000000000006401a6010000ab
+            0100000000000000007210740d000000000000000000006402a6010000ab
+            01000000000000000001006e8e7402000000000000000000006a07000000
+            0000000000a00800000000000000000000000000000000000000007c026a
+            000000000000000000a6010000ab0100000000000000007d037c026a0900
+            0000000000000070147c03a0050000000000000000000000000000000000
+            0000006403a6010000ab0100000000000000007c025f0900000000000000
+            007c03a00500000000000000000000000000000000000000006404a60100
+            00ab0100000000000000007c025f0a000000000000000069007c026a0400
+            00000000000000a5017c03a5017c025f0400000000000000007402000000
+            000000000000006a020000000000000000a00b0000000000000000000000
+            0000000000000000007c02a6010000ab01000000000000000001007c026a
+            040000000000000000a00500000000000000000000000000000000000000
+            006405a6010000ab0100000000000000007211740d000000000000000000
+            006406a6010000ab01000000000000000001006400530074190000000000
+            00000000007c02ac07a6010000ab010000000000000000010064005300
          213           0 RESUME                   0
          
          214           2 LOAD_FAST                0 (event)
                        4 LOAD_ATTR                0 (domain)
                       14 STORE_FAST               1 (domain)
          
-         215          16 LOAD_FAST                0 (event)
-                      18 LOAD_ATTR                1 (search_uid)
-                      28 STORE_FAST               2 (search_uid)
-         
-         217          30 LOAD_GLOBAL              4 (ts)
-                      42 LOAD_ATTR                3 (query)
-                      52 LOAD_METHOD              4 (find_company_by_domain)
-                      74 LOAD_FAST                1 (domain)
-                      76 PRECALL                  1
-                      80 CALL                     1
-                      90 STORE_FAST               3 (company)
-         
-         218          92 LOAD_FAST                3 (company)
-                      94 LOAD_ATTR                5 (meta)
-                     104 LOAD_METHOD              6 (get)
-                     126 LOAD_CONST               1 ('company_uid')
-                     128 PRECALL                  1
-                     132 CALL                     1
-                     142 POP_JUMP_FORWARD_IF_FALSE    16 (to 176)
-         
-         219         144 LOAD_GLOBAL             15 (NULL + print)
-                     156 LOAD_CONST               2 ('company already exists. skipping enrichment...')
-                     158 PRECALL                  1
-                     162 CALL                     1
-                     172 POP_TOP
-                     174 JUMP_FORWARD           142 (to 460)
-         
-         221     >>  176 LOAD_GLOBAL              4 (ts)
-                     188 LOAD_ATTR                8 (grata)
-                     198 LOAD_METHOD              9 (enrich)
-                     220 LOAD_FAST                3 (company)
-                     222 LOAD_ATTR                0 (domain)
-                     232 PRECALL                  1
-                     236 CALL                     1
-                     246 STORE_FAST               4 (resp)
-         
-         222         248 LOAD_FAST                3 (company)
-                     250 LOAD_ATTR               10 (name)
-                     260 JUMP_IF_TRUE_OR_POP     20 (to 302)
-                     262 LOAD_FAST                4 (resp)
-                     264 LOAD_METHOD              6 (get)
-                     286 LOAD_CONST               3 ('name')
-                     288 PRECALL                  1
-                     292 CALL                     1
-                 >>  302 LOAD_FAST                3 (company)
-                     304 STORE_ATTR              10 (name)
-         
-         223         314 LOAD_FAST                4 (resp)
-                     316 LOAD_METHOD              6 (get)
-                     338 LOAD_CONST               4 ('description')
-                     340 PRECALL                  1
-                     344 CALL                     1
-                     354 LOAD_FAST                3 (company)
-                     356 STORE_ATTR              11 (description)
-         
-         224         366 BUILD_MAP                0
-                     368 LOAD_FAST                3 (company)
-                     370 LOAD_ATTR                5 (meta)
-                     380 DICT_UPDATE              1
-                     382 LOAD_FAST                4 (resp)
-                     384 DICT_UPDATE              1
-                     386 LOAD_FAST                3 (company)
-                     388 STORE_ATTR               5 (meta)
+         216          16 LOAD_GLOBAL              2 (ts)
+                      28 LOAD_ATTR                2 (query)
+                      38 LOAD_METHOD              3 (find_company_by_domain)
+                      60 LOAD_FAST                1 (domain)
+                      62 PRECALL                  1
+                      66 CALL                     1
+                      76 STORE_FAST               2 (company)
          
-         225         398 LOAD_GLOBAL              4 (ts)
-                     410 LOAD_ATTR                3 (query)
-                     420 LOAD_METHOD             12 (update_company)
-                     442 LOAD_FAST                3 (company)
-                     444 PRECALL                  1
-                     448 CALL                     1
-                     458 POP_TOP
-         
-         227     >>  460 LOAD_FAST                3 (company)
-                     462 LOAD_ATTR                5 (meta)
-                     472 LOAD_METHOD              6 (get)
-                     494 LOAD_CONST               5 ('gpt_description')
-                     496 PRECALL                  1
-                     500 CALL                     1
-                     510 POP_JUMP_FORWARD_IF_FALSE    17 (to 546)
+         217          78 LOAD_FAST                2 (company)
+                      80 LOAD_ATTR                4 (meta)
+                      90 LOAD_METHOD              5 (get)
+                     112 LOAD_CONST               1 ('company_uid')
+                     114 PRECALL                  1
+                     118 CALL                     1
+                     128 POP_JUMP_FORWARD_IF_FALSE    16 (to 162)
+         
+         218         130 LOAD_GLOBAL             13 (NULL + print)
+                     142 LOAD_CONST               2 ('company already exists. skipping enrichment...')
+                     144 PRECALL                  1
+                     148 CALL                     1
+                     158 POP_TOP
+                     160 JUMP_FORWARD           142 (to 446)
+         
+         220     >>  162 LOAD_GLOBAL              2 (ts)
+                     174 LOAD_ATTR                7 (grata)
+                     184 LOAD_METHOD              8 (enrich)
+                     206 LOAD_FAST                2 (company)
+                     208 LOAD_ATTR                0 (domain)
+                     218 PRECALL                  1
+                     222 CALL                     1
+                     232 STORE_FAST               3 (resp)
+         
+         221         234 LOAD_FAST                2 (company)
+                     236 LOAD_ATTR                9 (name)
+                     246 JUMP_IF_TRUE_OR_POP     20 (to 288)
+                     248 LOAD_FAST                3 (resp)
+                     250 LOAD_METHOD              5 (get)
+                     272 LOAD_CONST               3 ('name')
+                     274 PRECALL                  1
+                     278 CALL                     1
+                 >>  288 LOAD_FAST                2 (company)
+                     290 STORE_ATTR               9 (name)
+         
+         222         300 LOAD_FAST                3 (resp)
+                     302 LOAD_METHOD              5 (get)
+                     324 LOAD_CONST               4 ('description')
+                     326 PRECALL                  1
+                     330 CALL                     1
+                     340 LOAD_FAST                2 (company)
+                     342 STORE_ATTR              10 (description)
          
-         228         512 LOAD_GLOBAL             15 (NULL + print)
-                     524 LOAD_CONST               6 ('company already enriched with gpt. skipping...')
-                     526 PRECALL                  1
-                     530 CALL                     1
-                     540 POP_TOP
-                     542 LOAD_CONST               0 (None)
-                     544 RETURN_VALUE
+         223         352 BUILD_MAP                0
+                     354 LOAD_FAST                2 (company)
+                     356 LOAD_ATTR                4 (meta)
+                     366 DICT_UPDATE              1
+                     368 LOAD_FAST                3 (resp)
+                     370 DICT_UPDATE              1
+                     372 LOAD_FAST                2 (company)
+                     374 STORE_ATTR               4 (meta)
+         
+         224         384 LOAD_GLOBAL              2 (ts)
+                     396 LOAD_ATTR                2 (query)
+                     406 LOAD_METHOD             11 (update_company)
+                     428 LOAD_FAST                2 (company)
+                     430 PRECALL                  1
+                     434 CALL                     1
+                     444 POP_TOP
          
-         230     >>  546 LOAD_GLOBAL             27 (NULL + enrich_with_gpt)
-                     558 LOAD_FAST                3 (company)
-                     560 KW_NAMES                 7
-                     562 PRECALL                  1
-                     566 CALL                     1
-                     576 POP_TOP
-                     578 LOAD_CONST               0 (None)
-                     580 RETURN_VALUE
+         226     >>  446 LOAD_FAST                2 (company)
+                     448 LOAD_ATTR                4 (meta)
+                     458 LOAD_METHOD              5 (get)
+                     480 LOAD_CONST               5 ('gpt_description')
+                     482 PRECALL                  1
+                     486 CALL                     1
+                     496 POP_JUMP_FORWARD_IF_FALSE    17 (to 532)
+         
+         227         498 LOAD_GLOBAL             13 (NULL + print)
+                     510 LOAD_CONST               6 ('company already enriched with gpt. skipping...')
+                     512 PRECALL                  1
+                     516 CALL                     1
+                     526 POP_TOP
+                     528 LOAD_CONST               0 (None)
+                     530 RETURN_VALUE
+         
+         229     >>  532 LOAD_GLOBAL             25 (NULL + enrich_with_gpt)
+                     544 LOAD_FAST                2 (company)
+                     546 KW_NAMES                 7
+                     548 PRECALL                  1
+                     552 CALL                     1
+                     562 POP_TOP
+                     564 LOAD_CONST               0 (None)
+                     566 RETURN_VALUE
          consts
             None
             'company_uid'
             'company already exists. skipping enrichment...'
             'name'
             'description'
             'gpt_description'
             'company already enriched with gpt. skipping...'
             ('company',)
-         names      ('domain', 'search_uid', 'ts', 'query', 'find_company_by_domain', 'meta', 'get', 'print', 'grata', 'enrich', 'name', 'description', 'update_company', 'enrich_with_gpt')
-         varnames   ('event', 'domain', 'search_uid', 'company', 'resp')
+         names      ('domain', 'ts', 'query', 'find_company_by_domain', 'meta', 'get', 'print', 'grata', 'enrich', 'name', 'description', 'update_company', 'enrich_with_gpt')
+         varnames   ('event', 'domain', 'company', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_enrichment'
          firstlineno 213
-         lnotab 0x02010e010e023e013401200248014201340120013e0234012202
+         lnotab 0x02010e023e013401200248014201340120013e0234012202
       'event_id'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 9
          flags     : 3
          code
@@ -1555,593 +1550,593 @@
             0000000000000001007402000000000000000000006a0200000000000000
             00a014000000000000000000000000000000000000000074020000000000
             00000000006a150000000000000000a01600000000000000000000000000
             000000000000007c026a1300000000000000007c037c016a0d0000000000
             000000642a190000000000000000007c016a170000000000000000ac2ba6
             040000ab040000000000000000a6010000ab01000000000000000001008c
             686400530064005300
-         233           0 RESUME                   0
+         232           0 RESUME                   0
          
-         234           2 LOAD_GLOBAL              1 (NULL + print)
+         233           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('processing event...')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-         235          32 LOAD_GLOBAL              2 (ts)
+         234          32 LOAD_GLOBAL              2 (ts)
                       44 LOAD_ATTR                2 (query)
                       54 LOAD_METHOD              3 (find_event_by_id)
                       76 LOAD_FAST                0 (event_id)
                       78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               1 (event)
          
-         236          94 LOAD_GLOBAL              1 (NULL + print)
+         235          94 LOAD_GLOBAL              1 (NULL + print)
                      106 LOAD_CONST               2 ('event_id')
                      108 LOAD_FAST                0 (event_id)
                      110 PRECALL                  2
                      114 CALL                     2
                      124 POP_TOP
          
-         237         126 LOAD_GLOBAL              1 (NULL + print)
+         236         126 LOAD_GLOBAL              1 (NULL + print)
                      138 LOAD_FAST                1 (event)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 POP_TOP
          
-         238         156 LOAD_GLOBAL              2 (ts)
+         237         156 LOAD_GLOBAL              2 (ts)
                      168 LOAD_ATTR                2 (query)
                      178 LOAD_METHOD              4 (find_search)
                      200 LOAD_FAST                1 (event)
                      202 LOAD_ATTR                5 (search_uid)
                      212 KW_NAMES                 3
                      214 PRECALL                  1
                      218 CALL                     1
                      228 STORE_FAST               2 (search)
          
-         239         230 LOAD_FAST                1 (event)
+         238         230 LOAD_FAST                1 (event)
                      232 LOAD_ATTR                6 (domain)
                      242 STORE_FAST               3 (domain)
          
-         240         244 LOAD_FAST                1 (event)
+         239         244 LOAD_FAST                1 (event)
                      246 LOAD_ATTR                7 (type)
                      256 LOAD_CONST               4 ('land')
                      258 COMPARE_OP               2 (==)
                      264 POP_JUMP_FORWARD_IF_FALSE    18 (to 302)
          
-         241         266 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         240         266 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      278 LOAD_FAST                1 (event)
                      280 KW_NAMES                 5
                      282 PRECALL                  1
                      286 CALL                     1
                      296 POP_TOP
                      298 LOAD_CONST               0 (None)
                      300 RETURN_VALUE
          
-         242     >>  302 LOAD_FAST                1 (event)
+         241     >>  302 LOAD_FAST                1 (event)
                      304 LOAD_ATTR                7 (type)
                      314 LOAD_CONST               6 ('create')
                      316 COMPARE_OP               2 (==)
                      322 POP_JUMP_FORWARD_IF_FALSE    18 (to 360)
          
-         243         324 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         242         324 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      336 LOAD_FAST                1 (event)
                      338 KW_NAMES                 5
                      340 PRECALL                  1
                      344 CALL                     1
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
          
-         244     >>  360 LOAD_FAST                1 (event)
+         243     >>  360 LOAD_FAST                1 (event)
                      362 LOAD_ATTR                7 (type)
                      372 LOAD_CONST               7 ('advance')
                      374 COMPARE_OP               2 (==)
                      380 POP_JUMP_FORWARD_IF_FALSE    18 (to 418)
          
-         245         382 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         244         382 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      394 LOAD_FAST                1 (event)
                      396 KW_NAMES                 5
                      398 PRECALL                  1
                      402 CALL                     1
                      412 POP_TOP
                      414 LOAD_CONST               0 (None)
                      416 RETURN_VALUE
          
-         246     >>  418 LOAD_FAST                1 (event)
+         245     >>  418 LOAD_FAST                1 (event)
                      420 LOAD_ATTR                7 (type)
                      430 LOAD_CONST               8 ('validate')
                      432 COMPARE_OP               2 (==)
                      438 POP_JUMP_FORWARD_IF_FALSE    51 (to 542)
          
-         247         440 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         246         440 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      452 LOAD_FAST                1 (event)
                      454 KW_NAMES                 5
                      456 PRECALL                  1
                      460 CALL                     1
                      470 POP_TOP
          
-         248         472 LOAD_GLOBAL             19 (NULL + run_acquired_check)
+         247         472 LOAD_GLOBAL             19 (NULL + run_acquired_check)
                      484 LOAD_FAST                3 (domain)
                      486 KW_NAMES                 9
                      488 PRECALL                  1
                      492 CALL                     1
                      502 POP_TOP
          
-         249         504 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         248         504 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      516 LOAD_FAST                2 (search)
                      518 LOAD_FAST                3 (domain)
                      520 KW_NAMES                10
                      522 PRECALL                  2
                      526 CALL                     2
                      536 POP_TOP
                      538 LOAD_CONST               0 (None)
                      540 RETURN_VALUE
          
-         250     >>  542 LOAD_FAST                1 (event)
+         249     >>  542 LOAD_FAST                1 (event)
                      544 LOAD_ATTR                7 (type)
                      554 LOAD_CONST              11 ('send')
                      556 COMPARE_OP               2 (==)
                      562 POP_JUMP_FORWARD_IF_FALSE    18 (to 600)
          
-         251         564 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         250         564 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      576 LOAD_FAST                1 (event)
                      578 KW_NAMES                 5
                      580 PRECALL                  1
                      584 CALL                     1
                      594 POP_TOP
                      596 LOAD_CONST               0 (None)
                      598 RETURN_VALUE
          
-         252     >>  600 LOAD_FAST                1 (event)
+         251     >>  600 LOAD_FAST                1 (event)
                      602 LOAD_ATTR                7 (type)
                      612 LOAD_CONST              12 ('client_approve')
                      614 COMPARE_OP               2 (==)
                      620 POP_JUMP_FORWARD_IF_FALSE    35 (to 692)
          
-         253         622 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         252         622 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      634 LOAD_FAST                1 (event)
                      636 KW_NAMES                 5
                      638 PRECALL                  1
                      642 CALL                     1
                      652 POP_TOP
          
-         254         654 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         253         654 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      666 LOAD_FAST                2 (search)
                      668 LOAD_FAST                3 (domain)
                      670 KW_NAMES                10
                      672 PRECALL                  2
                      676 CALL                     2
                      686 POP_TOP
                      688 LOAD_CONST               0 (None)
                      690 RETURN_VALUE
          
-         255     >>  692 LOAD_FAST                1 (event)
+         254     >>  692 LOAD_FAST                1 (event)
                      694 LOAD_ATTR                7 (type)
                      704 LOAD_CONST              13 ('reject')
                      706 COMPARE_OP               2 (==)
                      712 POP_JUMP_FORWARD_IF_FALSE     2 (to 718)
          
-         256         714 LOAD_CONST               0 (None)
+         255         714 LOAD_CONST               0 (None)
                      716 RETURN_VALUE
          
-         257     >>  718 LOAD_FAST                1 (event)
+         256     >>  718 LOAD_FAST                1 (event)
                      720 LOAD_ATTR                7 (type)
                      730 LOAD_CONST              14 ('client_reject')
                      732 COMPARE_OP               2 (==)
                      738 POP_JUMP_FORWARD_IF_FALSE     2 (to 744)
          
-         258         740 LOAD_CONST               0 (None)
+         257         740 LOAD_CONST               0 (None)
                      742 RETURN_VALUE
          
-         259     >>  744 LOAD_FAST                1 (event)
+         258     >>  744 LOAD_FAST                1 (event)
                      746 LOAD_ATTR                7 (type)
                      756 LOAD_CONST              15 ('conflict')
                      758 COMPARE_OP               2 (==)
                      764 POP_JUMP_FORWARD_IF_FALSE    35 (to 836)
          
-         260         766 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         259         766 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      778 LOAD_FAST                1 (event)
                      780 KW_NAMES                 5
                      782 PRECALL                  1
                      786 CALL                     1
                      796 POP_TOP
          
-         261         798 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         260         798 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      810 LOAD_FAST                2 (search)
                      812 LOAD_FAST                3 (domain)
                      814 KW_NAMES                10
                      816 PRECALL                  2
                      820 CALL                     2
                      830 POP_TOP
                      832 LOAD_CONST               0 (None)
                      834 RETURN_VALUE
          
-         262     >>  836 LOAD_FAST                1 (event)
+         261     >>  836 LOAD_FAST                1 (event)
                      838 LOAD_ATTR                7 (type)
                      848 LOAD_CONST              16 ('client_conflict')
                      850 COMPARE_OP               2 (==)
                      856 POP_JUMP_FORWARD_IF_FALSE     2 (to 862)
          
-         263         858 LOAD_CONST               0 (None)
+         262         858 LOAD_CONST               0 (None)
                      860 RETURN_VALUE
          
-         266     >>  862 LOAD_FAST                1 (event)
+         265     >>  862 LOAD_FAST                1 (event)
                      864 LOAD_ATTR                7 (type)
                      874 LOAD_CONST              17 ('prompt')
                      876 COMPARE_OP               2 (==)
                      882 POP_JUMP_FORWARD_IF_FALSE    18 (to 920)
          
-         267         884 LOAD_GLOBAL             23 (NULL + handle_prompt)
+         266         884 LOAD_GLOBAL             23 (NULL + handle_prompt)
                      896 LOAD_FAST                1 (event)
                      898 KW_NAMES                 5
                      900 PRECALL                  1
                      904 CALL                     1
                      914 POP_TOP
                      916 LOAD_CONST               0 (None)
                      918 RETURN_VALUE
          
-         268     >>  920 LOAD_FAST                1 (event)
+         267     >>  920 LOAD_FAST                1 (event)
                      922 LOAD_ATTR                7 (type)
                      932 LOAD_CONST              18 ('criteria')
                      934 COMPARE_OP               2 (==)
                      940 POP_JUMP_FORWARD_IF_FALSE    56 (to 1054)
          
-         269         942 LOAD_GLOBAL             25 (NULL + len)
+         268         942 LOAD_GLOBAL             25 (NULL + len)
                      954 LOAD_FAST                1 (event)
                      956 LOAD_ATTR               13 (data)
                      966 LOAD_CONST              19 ('inclusion')
                      968 BINARY_SUBSCR
                      978 LOAD_CONST              20 ('keywords')
                      980 BINARY_SUBSCR
                      990 PRECALL                  1
                      994 CALL                     1
                     1004 LOAD_CONST              21 (0)
                     1006 COMPARE_OP               4 (>)
                     1012 POP_JUMP_FORWARD_IF_FALSE    18 (to 1050)
          
-         270        1014 LOAD_GLOBAL             29 (NULL + run_criteria_search)
+         269        1014 LOAD_GLOBAL             29 (NULL + run_criteria_search)
                     1026 LOAD_FAST                2 (search)
                     1028 KW_NAMES                22
                     1030 PRECALL                  1
                     1034 CALL                     1
                     1044 POP_TOP
                     1046 LOAD_CONST               0 (None)
                     1048 RETURN_VALUE
          
-         269     >> 1050 LOAD_CONST               0 (None)
+         268     >> 1050 LOAD_CONST               0 (None)
                     1052 RETURN_VALUE
          
-         271     >> 1054 LOAD_FAST                1 (event)
+         270     >> 1054 LOAD_FAST                1 (event)
                     1056 LOAD_ATTR                7 (type)
                     1066 LOAD_CONST              23 ('maps')
                     1068 COMPARE_OP               2 (==)
                     1074 POP_JUMP_FORWARD_IF_FALSE    19 (to 1114)
          
-         272        1076 LOAD_GLOBAL             31 (NULL + run_maps_search)
+         271        1076 LOAD_GLOBAL             31 (NULL + run_maps_search)
                     1088 LOAD_FAST                2 (search)
                     1090 LOAD_FAST                1 (event)
                     1092 KW_NAMES                24
                     1094 PRECALL                  2
                     1098 CALL                     2
                     1108 POP_TOP
                     1110 LOAD_CONST               0 (None)
                     1112 RETURN_VALUE
          
-         273     >> 1114 LOAD_FAST                1 (event)
+         272     >> 1114 LOAD_FAST                1 (event)
                     1116 LOAD_ATTR                7 (type)
                     1126 LOAD_CONST              25 ('google')
                     1128 COMPARE_OP               2 (==)
                     1134 POP_JUMP_FORWARD_IF_FALSE    19 (to 1174)
          
-         274        1136 LOAD_GLOBAL             33 (NULL + run_google_search)
+         273        1136 LOAD_GLOBAL             33 (NULL + run_google_search)
                     1148 LOAD_FAST                2 (search)
                     1150 LOAD_FAST                1 (event)
                     1152 KW_NAMES                24
                     1154 PRECALL                  2
                     1158 CALL                     2
                     1168 POP_TOP
                     1170 LOAD_CONST               0 (None)
                     1172 RETURN_VALUE
          
-         276     >> 1174 LOAD_FAST                1 (event)
+         275     >> 1174 LOAD_FAST                1 (event)
                     1176 LOAD_ATTR                7 (type)
                     1186 LOAD_CONST              26 ('import')
                     1188 COMPARE_OP               2 (==)
                     1194 POP_JUMP_FORWARD_IF_FALSE    34 (to 1264)
          
-         277        1196 LOAD_GLOBAL              2 (ts)
+         276        1196 LOAD_GLOBAL              2 (ts)
                     1208 LOAD_ATTR                2 (query)
                     1218 LOAD_METHOD             17 (important_targets_from_event)
                     1240 LOAD_FAST                1 (event)
                     1242 KW_NAMES                 5
                     1244 PRECALL                  1
                     1248 CALL                     1
                     1258 POP_TOP
                     1260 LOAD_CONST               0 (None)
                     1262 RETURN_VALUE
          
-         279     >> 1264 LOAD_FAST                1 (event)
+         278     >> 1264 LOAD_FAST                1 (event)
                     1266 LOAD_ATTR                7 (type)
                     1276 LOAD_CONST              27 ('reset')
                     1278 COMPARE_OP               2 (==)
                     1284 POP_JUMP_FORWARD_IF_FALSE    54 (to 1394)
          
-         280        1286 LOAD_GLOBAL              1 (NULL + print)
+         279        1286 LOAD_GLOBAL              1 (NULL + print)
                     1298 LOAD_CONST              28 ('💣 Resetting Inbox...')
                     1300 PRECALL                  1
                     1304 CALL                     1
                     1314 POP_TOP
          
-         281        1316 LOAD_GLOBAL              2 (ts)
+         280        1316 LOAD_GLOBAL              2 (ts)
                     1328 LOAD_ATTR                2 (query)
                     1338 LOAD_METHOD             18 (reset_inbox)
                     1360 LOAD_FAST                2 (search)
                     1362 LOAD_ATTR               19 (uid)
                     1372 KW_NAMES                29
                     1374 PRECALL                  1
                     1378 CALL                     1
                     1388 POP_TOP
                     1390 LOAD_CONST               0 (None)
                     1392 RETURN_VALUE
          
-         283     >> 1394 LOAD_FAST                1 (event)
+         282     >> 1394 LOAD_FAST                1 (event)
                     1396 LOAD_ATTR                7 (type)
                     1406 LOAD_CONST              30 ('rating')
                     1408 COMPARE_OP               2 (==)
                     1414 EXTENDED_ARG             1
                     1416 POP_JUMP_FORWARD_IF_FALSE   287 (to 1992)
          
-         285        1418 LOAD_GLOBAL              1 (NULL + print)
+         284        1418 LOAD_GLOBAL              1 (NULL + print)
                     1430 LOAD_FAST                1 (event)
                     1432 PRECALL                  1
                     1436 CALL                     1
                     1446 POP_TOP
          
-         286        1448 LOAD_FAST                1 (event)
+         285        1448 LOAD_FAST                1 (event)
                     1450 LOAD_ATTR               13 (data)
                     1460 LOAD_CONST              30 ('rating')
                     1462 BINARY_SUBSCR
                     1472 STORE_FAST               4 (rating)
          
-         287        1474 LOAD_FAST                1 (event)
+         286        1474 LOAD_FAST                1 (event)
                     1476 LOAD_ATTR               13 (data)
                     1486 LOAD_CONST              31 ('currentView')
                     1488 BINARY_SUBSCR
                     1498 STORE_FAST               5 (from_stage)
          
-         288        1500 LOAD_FAST                4 (rating)
+         287        1500 LOAD_FAST                4 (rating)
                     1502 LOAD_CONST              32 (1)
                     1504 COMPARE_OP               2 (==)
                     1510 POP_JUMP_FORWARD_IF_FALSE    76 (to 1664)
          
-         289        1512 LOAD_GLOBAL              2 (ts)
+         288        1512 LOAD_GLOBAL              2 (ts)
                     1524 LOAD_ATTR                2 (query)
                     1534 LOAD_METHOD             20 (insert_event)
          
-         290        1556 LOAD_GLOBAL              2 (ts)
+         289        1556 LOAD_GLOBAL              2 (ts)
                     1568 LOAD_ATTR               21 (models)
                     1578 LOAD_METHOD             22 (Event)
          
-         291        1600 LOAD_FAST                2 (search)
+         290        1600 LOAD_FAST                2 (search)
                     1602 LOAD_ATTR               19 (uid)
          
-         292        1612 LOAD_CONST              13 ('reject')
+         291        1612 LOAD_CONST              13 ('reject')
          
-         293        1614 LOAD_FAST                3 (domain)
+         292        1614 LOAD_FAST                3 (domain)
          
-         294        1616 LOAD_FAST                1 (event)
+         293        1616 LOAD_FAST                1 (event)
                     1618 LOAD_ATTR               23 (actor_key)
          
-         290        1628 KW_NAMES                33
+         289        1628 KW_NAMES                33
                     1630 PRECALL                  4
                     1634 CALL                     4
          
-         289        1644 PRECALL                  1
+         288        1644 PRECALL                  1
                     1648 CALL                     1
                     1658 POP_TOP
                     1660 LOAD_CONST               0 (None)
                     1662 RETURN_VALUE
          
-         297     >> 1664 LOAD_FAST                4 (rating)
+         296     >> 1664 LOAD_FAST                4 (rating)
                     1666 LOAD_CONST              34 (2)
                     1668 COMPARE_OP               2 (==)
                     1674 POP_JUMP_FORWARD_IF_FALSE    76 (to 1828)
          
-         298        1676 LOAD_GLOBAL              2 (ts)
+         297        1676 LOAD_GLOBAL              2 (ts)
                     1688 LOAD_ATTR                2 (query)
                     1698 LOAD_METHOD             20 (insert_event)
          
-         299        1720 LOAD_GLOBAL              2 (ts)
+         298        1720 LOAD_GLOBAL              2 (ts)
                     1732 LOAD_ATTR               21 (models)
                     1742 LOAD_METHOD             22 (Event)
          
-         300        1764 LOAD_FAST                2 (search)
+         299        1764 LOAD_FAST                2 (search)
                     1766 LOAD_ATTR               19 (uid)
          
-         301        1776 LOAD_CONST              35 ('hold')
+         300        1776 LOAD_CONST              35 ('hold')
          
-         302        1778 LOAD_FAST                3 (domain)
+         301        1778 LOAD_FAST                3 (domain)
          
-         303        1780 LOAD_FAST                1 (event)
+         302        1780 LOAD_FAST                1 (event)
                     1782 LOAD_ATTR               23 (actor_key)
          
-         299        1792 KW_NAMES                33
+         298        1792 KW_NAMES                33
                     1794 PRECALL                  4
                     1798 CALL                     4
          
-         298        1808 PRECALL                  1
+         297        1808 PRECALL                  1
                     1812 CALL                     1
                     1822 POP_TOP
                     1824 LOAD_CONST               0 (None)
                     1826 RETURN_VALUE
          
-         306     >> 1828 LOAD_FAST                5 (from_stage)
+         305     >> 1828 LOAD_FAST                5 (from_stage)
                     1830 LOAD_CONST              36 (('land', 'create', 'advance', 'hold'))
                     1832 CONTAINS_OP              0
                     1834 POP_JUMP_FORWARD_IF_FALSE    76 (to 1988)
          
-         307        1836 LOAD_GLOBAL              2 (ts)
+         306        1836 LOAD_GLOBAL              2 (ts)
                     1848 LOAD_ATTR                2 (query)
                     1858 LOAD_METHOD             20 (insert_event)
          
-         308        1880 LOAD_GLOBAL              2 (ts)
+         307        1880 LOAD_GLOBAL              2 (ts)
                     1892 LOAD_ATTR               21 (models)
                     1902 LOAD_METHOD             22 (Event)
          
-         309        1924 LOAD_FAST                2 (search)
+         308        1924 LOAD_FAST                2 (search)
                     1926 LOAD_ATTR               19 (uid)
          
-         310        1936 LOAD_CONST               8 ('validate')
+         309        1936 LOAD_CONST               8 ('validate')
          
-         311        1938 LOAD_FAST                3 (domain)
+         310        1938 LOAD_FAST                3 (domain)
          
-         312        1940 LOAD_FAST                1 (event)
+         311        1940 LOAD_FAST                1 (event)
                     1942 LOAD_ATTR               23 (actor_key)
          
-         308        1952 KW_NAMES                33
+         307        1952 KW_NAMES                33
                     1954 PRECALL                  4
                     1958 CALL                     4
          
-         307        1968 PRECALL                  1
+         306        1968 PRECALL                  1
                     1972 CALL                     1
                     1982 POP_TOP
                     1984 LOAD_CONST               0 (None)
                     1986 RETURN_VALUE
          
-         306     >> 1988 LOAD_CONST               0 (None)
+         305     >> 1988 LOAD_CONST               0 (None)
                     1990 RETURN_VALUE
          
-         316     >> 1992 LOAD_FAST                1 (event)
+         315     >> 1992 LOAD_FAST                1 (event)
                     1994 LOAD_ATTR                7 (type)
                     2004 LOAD_CONST              37 ('update')
                     2006 COMPARE_OP               2 (==)
                     2012 POP_JUMP_FORWARD_IF_FALSE   185 (to 2384)
          
-         317        2014 LOAD_FAST                3 (domain)
+         316        2014 LOAD_FAST                3 (domain)
                     2016 POP_JUMP_FORWARD_IF_FALSE   129 (to 2276)
          
-         318        2018 LOAD_GLOBAL              2 (ts)
+         317        2018 LOAD_GLOBAL              2 (ts)
                     2030 LOAD_ATTR                2 (query)
                     2040 LOAD_METHOD             24 (find_company_by_domain)
                     2062 LOAD_FAST                3 (domain)
                     2064 PRECALL                  1
                     2068 CALL                     1
                     2078 STORE_FAST               6 (company)
          
-         319        2080 LOAD_FAST                1 (event)
+         318        2080 LOAD_FAST                1 (event)
                     2082 LOAD_ATTR               13 (data)
                     2092 LOAD_METHOD             25 (get)
                     2114 LOAD_CONST              38 ('name')
                     2116 PRECALL                  1
                     2120 CALL                     1
                     2130 POP_JUMP_FORWARD_IF_FALSE    18 (to 2168)
          
-         320        2132 LOAD_FAST                1 (event)
+         319        2132 LOAD_FAST                1 (event)
                     2134 LOAD_ATTR               13 (data)
                     2144 LOAD_CONST              38 ('name')
                     2146 BINARY_SUBSCR
                     2156 LOAD_FAST                6 (company)
                     2158 STORE_ATTR              26 (name)
          
-         326     >> 2168 BUILD_MAP                0
+         325     >> 2168 BUILD_MAP                0
                     2170 LOAD_FAST                6 (company)
                     2172 LOAD_ATTR               27 (meta)
                     2182 DICT_UPDATE              1
                     2184 LOAD_FAST                1 (event)
                     2186 LOAD_ATTR               13 (data)
                     2196 DICT_UPDATE              1
                     2198 LOAD_FAST                6 (company)
                     2200 STORE_ATTR              27 (meta)
          
-         327        2210 LOAD_GLOBAL              2 (ts)
+         326        2210 LOAD_GLOBAL              2 (ts)
                     2222 LOAD_ATTR                2 (query)
                     2232 LOAD_METHOD             28 (update_company)
                     2254 LOAD_FAST                6 (company)
                     2256 PRECALL                  1
                     2260 CALL                     1
                     2270 POP_TOP
                     2272 LOAD_CONST               0 (None)
                     2274 RETURN_VALUE
          
-         329     >> 2276 BUILD_MAP                0
+         328     >> 2276 BUILD_MAP                0
                     2278 LOAD_FAST                2 (search)
                     2280 LOAD_ATTR               27 (meta)
                     2290 DICT_UPDATE              1
                     2292 LOAD_FAST                1 (event)
                     2294 LOAD_ATTR               13 (data)
                     2304 DICT_UPDATE              1
                     2306 LOAD_FAST                2 (search)
                     2308 STORE_ATTR              27 (meta)
          
-         330        2318 LOAD_GLOBAL              2 (ts)
+         329        2318 LOAD_GLOBAL              2 (ts)
                     2330 LOAD_ATTR                2 (query)
                     2340 LOAD_METHOD             29 (update_search)
                     2362 LOAD_FAST                2 (search)
                     2364 PRECALL                  1
                     2368 CALL                     1
                     2378 POP_TOP
                     2380 LOAD_CONST               0 (None)
                     2382 RETURN_VALUE
          
-         332     >> 2384 LOAD_FAST                1 (event)
+         331     >> 2384 LOAD_FAST                1 (event)
                     2386 LOAD_ATTR                7 (type)
                     2396 LOAD_CONST              39 ('move')
                     2398 COMPARE_OP               2 (==)
                     2404 POP_JUMP_FORWARD_IF_FALSE   117 (to 2640)
          
-         334        2406 LOAD_FAST                1 (event)
+         333        2406 LOAD_FAST                1 (event)
                     2408 LOAD_ATTR               13 (data)
                     2418 LOAD_CONST              40 ('domains')
                     2420 BINARY_SUBSCR
                     2430 GET_ITER
                  >> 2432 FOR_ITER               105 (to 2644)
                     2434 STORE_FAST               3 (domain)
          
-         335        2436 LOAD_GLOBAL              1 (NULL + print)
+         334        2436 LOAD_GLOBAL              1 (NULL + print)
                     2448 LOAD_CONST              41 ('moving domain:')
                     2450 LOAD_FAST                3 (domain)
                     2452 PRECALL                  2
                     2456 CALL                     2
                     2466 POP_TOP
          
-         336        2468 LOAD_GLOBAL              2 (ts)
+         335        2468 LOAD_GLOBAL              2 (ts)
                     2480 LOAD_ATTR                2 (query)
                     2490 LOAD_METHOD             20 (insert_event)
          
-         337        2512 LOAD_GLOBAL              2 (ts)
+         336        2512 LOAD_GLOBAL              2 (ts)
                     2524 LOAD_ATTR               21 (models)
                     2534 LOAD_METHOD             22 (Event)
          
-         338        2556 LOAD_FAST                2 (search)
+         337        2556 LOAD_FAST                2 (search)
                     2558 LOAD_ATTR               19 (uid)
          
-         339        2568 LOAD_FAST                3 (domain)
+         338        2568 LOAD_FAST                3 (domain)
          
-         340        2570 LOAD_FAST                1 (event)
+         339        2570 LOAD_FAST                1 (event)
                     2572 LOAD_ATTR               13 (data)
                     2582 LOAD_CONST              42 ('stage')
                     2584 BINARY_SUBSCR
          
-         341        2594 LOAD_FAST                1 (event)
+         340        2594 LOAD_FAST                1 (event)
                     2596 LOAD_ATTR               23 (actor_key)
          
-         337        2606 KW_NAMES                43
+         336        2606 KW_NAMES                43
                     2608 PRECALL                  4
                     2612 CALL                     4
          
-         336        2622 PRECALL                  1
+         335        2622 PRECALL                  1
                     2626 CALL                     1
                     2636 POP_TOP
                     2638 JUMP_BACKWARD          104 (to 2432)
          
-         332     >> 2640 LOAD_CONST               0 (None)
+         331     >> 2640 LOAD_CONST               0 (None)
                     2642 RETURN_VALUE
          
-         334     >> 2644 LOAD_CONST               0 (None)
+         333     >> 2644 LOAD_CONST               0 (None)
                     2646 RETURN_VALUE
          consts
             None
             'processing event...'
             'event_id'
             ('uid',)
             'land'
@@ -2186,15 +2181,15 @@
             ('search_uid', 'domain', 'type', 'actor_key')
          names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'len', 'data', 'run_criteria_search', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'reset_inbox', 'uid', 'insert_event', 'models', 'Event', 'actor_key', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
          varnames   ('event_id', 'event', 'search', 'domain', 'rating', 'from_stage', 'company')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_event'
-         firstlineno 233
+         firstlineno 232
          lnotab
             0x02011e013e0120011e014a010e01160124011601240116012401160120
             012001260116012401160120012601160104011601040116012001260116
             010403160124011601480124ff040216012601160126021601440216011e
             014e0218021e011a011a010c012c012c010c01020102010cfc10ff14080c
             012c012c010c01020102010cfc10ff140808012c012c010c01020102010c
             fc10ff14ff040a160104013e01340124062a0142022a01420216021e0120
@@ -2202,8 +2197,8 @@
    names      ('dataclasses', 'asdict', 'time', 'gandai', 'ts', 'dacite', 'from_dict', 'str', 'run_acquired_check', 'models', 'Search', 'run_similarity_search', 'run_criteria_search', 'Event', 'run_maps_search', 'run_google_search', 'handle_prompt', 'Company', 'enrich_with_gpt', 'run_enrichment', 'int', 'process_event')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c0208010c030c26280b240d3c2d3c0f242c24272414
+   lnotab 0x00ff02010c010c0208010c030c26280b240d3c2d3c0f242c24272413
```

### Comparing `gandai-1.7.50/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x110f5066 (Fri May 24 03:52:49 2024 UTC)
-files sz: 28700
+moddate:  0xfa305066 (Fri May 24 06:17:30 2024 UTC)
+files sz: 28730
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -271,145 +271,145 @@
    478         474 LOAD_CONST              22 ('search_uid')
                476 LOAD_NAME               33 (int)
                478 BUILD_TUPLE              2
                480 LOAD_CONST              34 (<code object search_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 478>)
                482 MAKE_FUNCTION            4 (annotations)
                484 STORE_NAME              45 (search_targets)
    
-   611         486 LOAD_CONST              22 ('search_uid')
+   612         486 LOAD_CONST              22 ('search_uid')
                488 LOAD_NAME               33 (int)
                490 LOAD_CONST              11 ('return')
                492 LOAD_NAME                9 (pd)
                494 LOAD_ATTR               37 (DataFrame)
                504 BUILD_TUPLE              4
-               506 LOAD_CONST              35 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 611>)
+               506 LOAD_CONST              35 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 612>)
                508 MAKE_FUNCTION            4 (annotations)
                510 STORE_NAME              46 (search_comments)
    
-   633         512 LOAD_CONST              22 ('search_uid')
+   634         512 LOAD_CONST              22 ('search_uid')
                514 LOAD_NAME               33 (int)
                516 LOAD_CONST              11 ('return')
                518 LOAD_NAME                9 (pd)
                520 LOAD_ATTR               37 (DataFrame)
                530 BUILD_TUPLE              4
-               532 LOAD_CONST              36 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 633>)
+               532 LOAD_CONST              36 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 634>)
                534 MAKE_FUNCTION            4 (annotations)
                536 STORE_NAME              47 (event)
    
-   645         538 LOAD_CONST              22 ('search_uid')
+   646         538 LOAD_CONST              22 ('search_uid')
                540 LOAD_NAME               33 (int)
                542 LOAD_CONST              11 ('return')
                544 LOAD_NAME                9 (pd)
                546 LOAD_ATTR               37 (DataFrame)
                556 BUILD_TUPLE              4
-               558 LOAD_CONST              37 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 645>)
+               558 LOAD_CONST              37 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 646>)
                560 MAKE_FUNCTION            4 (annotations)
                562 STORE_NAME              48 (event_history)
    
-   675         564 LOAD_CONST              22 ('search_uid')
+   676         564 LOAD_CONST              22 ('search_uid')
                566 LOAD_NAME               33 (int)
                568 LOAD_CONST              11 ('return')
                570 LOAD_NAME                9 (pd)
                572 LOAD_ATTR               37 (DataFrame)
                582 BUILD_TUPLE              4
-               584 LOAD_CONST              38 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 675>)
+               584 LOAD_CONST              38 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 676>)
                586 MAKE_FUNCTION            4 (annotations)
                588 STORE_NAME              49 (search_criteria_history)
    
-   704         590 LOAD_CONST              39 ('uid')
+   705         590 LOAD_CONST              39 ('uid')
                592 LOAD_NAME               33 (int)
                594 LOAD_CONST              11 ('return')
                596 LOAD_NAME               16 (ts)
                598 LOAD_ATTR               28 (models)
                608 LOAD_ATTR               25 (Search)
                618 BUILD_TUPLE              4
-               620 LOAD_CONST              40 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 704>)
+               620 LOAD_CONST              40 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 705>)
                622 MAKE_FUNCTION            4 (annotations)
                624 STORE_NAME              50 (find_search)
    
-   732         626 LOAD_CONST              41 ('searchToken')
+   733         626 LOAD_CONST              41 ('searchToken')
                628 LOAD_NAME               34 (str)
                630 LOAD_CONST              11 ('return')
                632 LOAD_NAME               16 (ts)
                634 LOAD_ATTR               28 (models)
                644 LOAD_ATTR               25 (Search)
                654 BUILD_TUPLE              4
-               656 LOAD_CONST              42 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 732>)
+               656 LOAD_CONST              42 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 733>)
                658 MAKE_FUNCTION            4 (annotations)
                660 STORE_NAME              51 (find_search_by_token)
    
-   741         662 LOAD_CONST              43 ('domain')
+   742         662 LOAD_CONST              43 ('domain')
                664 LOAD_NAME               34 (str)
                666 LOAD_CONST              11 ('return')
                668 LOAD_NAME               22 (Company)
                670 BUILD_TUPLE              4
-               672 LOAD_CONST              44 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 741>)
+               672 LOAD_CONST              44 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 742>)
                674 MAKE_FUNCTION            4 (annotations)
                676 STORE_NAME              52 (find_company_by_domain)
    
-   757         678 LOAD_CONST              45 ('email')
+   758         678 LOAD_CONST              45 ('email')
                680 LOAD_NAME               34 (str)
                682 LOAD_CONST              11 ('return')
                684 LOAD_NAME               22 (Company)
                686 BUILD_TUPLE              4
-               688 LOAD_CONST              46 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 757>)
+               688 LOAD_CONST              46 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 758>)
                690 MAKE_FUNCTION            4 (annotations)
                692 STORE_NAME              53 (find_actor_by_email)
    
-   773         694 LOAD_CONST              47 ('event_id')
+   774         694 LOAD_CONST              47 ('event_id')
                696 LOAD_NAME               33 (int)
                698 LOAD_CONST              11 ('return')
                700 LOAD_NAME               23 (Event)
                702 BUILD_TUPLE              4
-               704 LOAD_CONST              48 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 773>)
+               704 LOAD_CONST              48 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 774>)
                706 MAKE_FUNCTION            4 (annotations)
                708 STORE_NAME              54 (find_event_by_id)
    
-   792         710 LOAD_CONST              13 ('company')
+   793         710 LOAD_CONST              13 ('company')
                712 LOAD_NAME               22 (Company)
                714 LOAD_CONST              11 ('return')
                716 LOAD_CONST               1 (None)
                718 BUILD_TUPLE              4
-               720 LOAD_CONST              49 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 792>)
+               720 LOAD_CONST              49 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 793>)
                722 MAKE_FUNCTION            4 (annotations)
                724 STORE_NAME              55 (update_company)
    
-   821         726 LOAD_CONST              17 ('search')
+   822         726 LOAD_CONST              17 ('search')
                728 LOAD_NAME               25 (Search)
                730 LOAD_CONST              11 ('return')
                732 LOAD_CONST               1 (None)
                734 BUILD_TUPLE              4
-               736 LOAD_CONST              50 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 821>)
+               736 LOAD_CONST              50 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 822>)
                738 MAKE_FUNCTION            4 (annotations)
                740 STORE_NAME              56 (update_search)
    
-   844         742 LOAD_CONST              47 ('event_id')
+   845         742 LOAD_CONST              47 ('event_id')
                744 LOAD_NAME               33 (int)
                746 LOAD_CONST              11 ('return')
                748 LOAD_CONST               1 (None)
                750 BUILD_TUPLE              4
-               752 LOAD_CONST              51 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 844>)
+               752 LOAD_CONST              51 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 845>)
                754 MAKE_FUNCTION            4 (annotations)
                756 STORE_NAME              57 (mute_event)
    
-   867         758 LOAD_CONST              52 ('comment_id')
+   868         758 LOAD_CONST              52 ('comment_id')
                760 LOAD_NAME               33 (int)
                762 LOAD_CONST              11 ('return')
                764 LOAD_CONST               1 (None)
                766 BUILD_TUPLE              4
-               768 LOAD_CONST              53 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 867>)
+               768 LOAD_CONST              53 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 868>)
                770 MAKE_FUNCTION            4 (annotations)
                772 STORE_NAME              58 (delete_comment)
    
-   878         774 LOAD_CONST              22 ('search_uid')
+   879         774 LOAD_CONST              22 ('search_uid')
                776 LOAD_NAME               33 (int)
                778 LOAD_CONST              11 ('return')
                780 LOAD_CONST               1 (None)
                782 BUILD_TUPLE              4
-               784 LOAD_CONST              54 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 878>)
+               784 LOAD_CONST              54 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 879>)
                786 MAKE_FUNCTION            4 (annotations)
                788 STORE_NAME              59 (reset_inbox)
                790 LOAD_CONST               1 (None)
                792 RETURN_VALUE
    consts
       0
       None
@@ -2613,57 +2613,57 @@
             010000ab0100000000000000007c04640d3c0000007c04a00a0000000000
             0000000000000000000000000000007c08640eac0fa6020000ab02000000
             00000000007c0464103c0000007c04a00a00000000000000000000000000
             000000000000007c09640eac0fa6020000ab0200000000000000007c0464
             113c0000007c045300
          478           0 RESUME                   0
          
-         481           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n    ;\n    ")
+         481           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         544           6 LOAD_GLOBAL              0 (db)
+         545           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         545          58 LOAD_FAST                2 (conn)
+         546          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         546          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         547          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         547         120 LOAD_CONST               2 ('search_uid')
+         548         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         545         126 PRECALL                  2
+         546         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         549         142 LOAD_GLOBAL             11 (NULL + pd)
+         550         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         544         258 LOAD_CONST               0 (None)
+         545         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2674,139 +2674,139 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         551     >>  304 LOAD_CONST               4 ('return')
+         552     >>  304 LOAD_CONST               4 ('return')
                      306 LOAD_GLOBAL             18 (str)
                      318 BUILD_TUPLE              2
-                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 551>)
+                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 552>)
                      322 MAKE_FUNCTION            4 (annotations)
                      324 STORE_FAST               5 (list_to_csv)
          
-         563         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 563>)
+         564         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 564>)
                      328 MAKE_FUNCTION            0
                      330 STORE_FAST               6 (get_employees)
          
-         575         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 575>)
+         576         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 576>)
                      334 MAKE_FUNCTION            0
                      336 STORE_FAST               7 (get_ownership)
          
-         583         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 583>)
+         584         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 584>)
                      340 MAKE_FUNCTION            0
                      342 STORE_FAST               8 (get_state)
          
-         593         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 593>)
+         594         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 594>)
                      346 MAKE_FUNCTION            0
                      348 STORE_FAST               9 (get_city)
          
-         602         350 LOAD_FAST                4 (df)
+         603         350 LOAD_FAST                4 (df)
                      352 LOAD_CONST              10 ('end_customer')
                      354 BINARY_SUBSCR
                      364 LOAD_METHOD             10 (apply)
                      386 LOAD_FAST                5 (list_to_csv)
                      388 PRECALL                  1
                      392 CALL                     1
                      402 LOAD_FAST                4 (df)
                      404 LOAD_CONST              10 ('end_customer')
                      406 STORE_SUBSCR
          
-         603         410 LOAD_FAST                4 (df)
+         604         410 LOAD_FAST                4 (df)
                      412 LOAD_CONST              11 ('meta')
                      414 BINARY_SUBSCR
                      424 LOAD_METHOD             10 (apply)
                      446 LOAD_FAST                6 (get_employees)
                      448 PRECALL                  1
                      452 CALL                     1
                      462 LOAD_FAST                4 (df)
                      464 LOAD_CONST              12 ('employees')
                      466 STORE_SUBSCR
          
-         604         470 LOAD_FAST                4 (df)
+         605         470 LOAD_FAST                4 (df)
                      472 LOAD_CONST              13 ('ownership')
                      474 BINARY_SUBSCR
                      484 LOAD_METHOD             10 (apply)
                      506 LOAD_FAST                7 (get_ownership)
                      508 PRECALL                  1
                      512 CALL                     1
                      522 LOAD_FAST                4 (df)
                      524 LOAD_CONST              13 ('ownership')
                      526 STORE_SUBSCR
          
-         605         530 LOAD_FAST                4 (df)
+         606         530 LOAD_FAST                4 (df)
                      532 LOAD_METHOD             10 (apply)
                      554 LOAD_FAST                8 (get_state)
                      556 LOAD_CONST              14 (1)
                      558 KW_NAMES                15
                      560 PRECALL                  2
                      564 CALL                     2
                      574 LOAD_FAST                4 (df)
                      576 LOAD_CONST              16 ('state')
                      578 STORE_SUBSCR
          
-         606         582 LOAD_FAST                4 (df)
+         607         582 LOAD_FAST                4 (df)
                      584 LOAD_METHOD             10 (apply)
                      606 LOAD_FAST                9 (get_city)
                      608 LOAD_CONST              14 (1)
                      610 KW_NAMES                15
                      612 PRECALL                  2
                      616 CALL                     2
                      626 LOAD_FAST                4 (df)
                      628 LOAD_CONST              17 ('city')
                      630 STORE_SUBSCR
          
-         608         634 LOAD_FAST                4 (df)
+         609         634 LOAD_FAST                4 (df)
                      636 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
-            "\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n    ;\n    "
+            "\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    "
             'search_uid'
             ('columns',)
             'return'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 19
                code
                   0x970009007401000000000000000000006a0100000000000000007c00a6
                   010000ab0100000000000000007d016401a0020000000000000000000000
                   0000000000000000007c01a6010000ab0100000000000000007d027c0253
                   0023000100590064025300780359007701
-               551           0 RESUME                   0
+               552           0 RESUME                   0
                
-               553           2 NOP
+               554           2 NOP
                
-               554           4 LOAD_GLOBAL              1 (NULL + json)
+               555           4 LOAD_GLOBAL              1 (NULL + json)
                             16 LOAD_ATTR                1 (loads)
                             26 LOAD_FAST                0 (list_str)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               1 (list_data)
                
-               557          44 LOAD_CONST               1 (', ')
+               558          44 LOAD_CONST               1 (', ')
                             46 LOAD_METHOD              2 (join)
                             68 LOAD_FAST                1 (list_data)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 STORE_FAST               2 (csv_str)
                
-               559          86 LOAD_FAST                2 (csv_str)
+               560          86 LOAD_FAST                2 (csv_str)
                             88 RETURN_VALUE
                        >>   90 PUSH_EXC_INFO
                
-               560          92 POP_TOP
+               561          92 POP_TOP
                
-               561          94 POP_EXCEPT
+               562          94 POP_EXCEPT
                             96 LOAD_CONST               2 ('')
                             98 RETURN_VALUE
                        >>  100 COPY                     3
                            102 POP_EXCEPT
                            104 RERAISE                  1
                ExceptionTable:
                  4 to 86 -> 90 [0]
@@ -2817,75 +2817,75 @@
                   ''
                names      ('json', 'loads', 'join')
                varnames   ('list_str', 'list_data', 'csv_str')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'list_to_csv'
-               firstlineno 551
+               firstlineno 552
                lnotab 0x0202020128032a0206010201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 19
                code
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab010000000000000000721e09007403000000000000000000007c
                   00640119000000000000000000a6010000ab010000000000000000530023
                   0001005900640053007803590077017c00a0000000000000000000000000
                   0000000000000000006402a6010000ab010000000000000000721b7c0064
                   0219000000000000000000a0000000000000000000000000000000000000
                   0000006403a6010000ab010000000000000000530064005300
-               563           0 RESUME                   0
+               564           0 RESUME                   0
                
-               564           2 LOAD_FAST                0 (meta)
+               565           2 LOAD_FAST                0 (meta)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('employees')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    30 (to 104)
                
-               566          44 NOP
+               567          44 NOP
                
-               567          46 LOAD_GLOBAL              3 (NULL + int)
+               568          46 LOAD_GLOBAL              3 (NULL + int)
                             58 LOAD_FAST                0 (meta)
                             60 LOAD_CONST               1 ('employees')
                             62 BINARY_SUBSCR
                             72 PRECALL                  1
                             76 CALL                     1
                             86 RETURN_VALUE
                        >>   88 PUSH_EXC_INFO
                
-               568          90 POP_TOP
+               569          90 POP_TOP
                
-               569          92 POP_EXCEPT
+               570          92 POP_EXCEPT
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                        >>   98 COPY                     3
                            100 POP_EXCEPT
                            102 RERAISE                  1
                
-               570     >>  104 LOAD_FAST                0 (meta)
+               571     >>  104 LOAD_FAST                0 (meta)
                            106 LOAD_METHOD              0 (get)
                            128 LOAD_CONST               2 ('grata_employee_estimates')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 POP_JUMP_FORWARD_IF_FALSE    27 (to 200)
                
-               571         146 LOAD_FAST                0 (meta)
+               572         146 LOAD_FAST                0 (meta)
                            148 LOAD_CONST               2 ('grata_employee_estimates')
                            150 BINARY_SUBSCR
                            160 LOAD_METHOD              0 (get)
                            182 LOAD_CONST               3 ('count')
                            184 PRECALL                  1
                            188 CALL                     1
                            198 RETURN_VALUE
                
-               573     >>  200 LOAD_CONST               0 (None)
+               574     >>  200 LOAD_CONST               0 (None)
                            202 RETURN_VALUE
                ExceptionTable:
                  46 to 84 -> 88 [0]
                  88 to 90 -> 98 [1] lasti
                consts
                   None
                   'employees'
@@ -2893,57 +2893,57 @@
                   'count'
                names      ('get', 'int')
                varnames   ('meta',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_employees'
-               firstlineno 563
+               firstlineno 564
                lnotab 0x02012a0202012c0102010c012a013602
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 19
                code
                   0x97007c0064016b02000000007202640253007c0064036b020000000072
                   02640453007c005300
-               575           0 RESUME                   0
+               576           0 RESUME                   0
                
-               576           2 LOAD_FAST                0 (ownership)
+               577           2 LOAD_FAST                0 (ownership)
                              4 LOAD_CONST               1 ('Bootstrapped')
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE     2 (to 18)
                
-               577          14 LOAD_CONST               2 ('Private')
+               578          14 LOAD_CONST               2 ('Private')
                             16 RETURN_VALUE
                
-               578     >>   18 LOAD_FAST                0 (ownership)
+               579     >>   18 LOAD_FAST                0 (ownership)
                             20 LOAD_CONST               3 ('Investor Backed')
                             22 COMPARE_OP               2 (==)
                             28 POP_JUMP_FORWARD_IF_FALSE     2 (to 34)
                
-               579          30 LOAD_CONST               4 ('Venture Capital')
+               580          30 LOAD_CONST               4 ('Venture Capital')
                             32 RETURN_VALUE
                
-               581     >>   34 LOAD_FAST                0 (ownership)
+               582     >>   34 LOAD_FAST                0 (ownership)
                             36 RETURN_VALUE
                consts
                   None
                   'Bootstrapped'
                   'Private'
                   'Investor Backed'
                   'Venture Capital'
                names      ()
                varnames   ('ownership',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_ownership'
-               firstlineno 575
+               firstlineno 576
                lnotab 0x02010c0104010c010402
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 19
                code
@@ -2953,78 +2953,78 @@
                   00ab010000000000000000725a7c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017406000000
                   000000000000006a0400000000000000006a050000000000000000a00000
                   000000000000000000000000000000000000007c016405a6020000ab0200
                   000000000000007d027c02530064005300
-               583           0 RESUME                   0
+               584           0 RESUME                   0
                
-               584           2 LOAD_FAST                0 (row)
+               585           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('state')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               585          44 LOAD_FAST                0 (row)
+               586          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('state')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               586     >>   60 LOAD_FAST                0 (row)
+               587     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    90 (to 282)
                
-               587         102 LOAD_FAST                0 (row)
+               588         102 LOAD_FAST                0 (row)
                            104 LOAD_CONST               2 ('headquarters')
                            106 BINARY_SUBSCR
                            116 LOAD_METHOD              1 (split)
                            138 LOAD_CONST               3 (',')
                            140 PRECALL                  1
                            144 CALL                     1
                            154 LOAD_CONST               4 (-1)
                            156 BINARY_SUBSCR
                            166 LOAD_METHOD              2 (strip)
                            188 PRECALL                  0
                            192 CALL                     0
                            202 STORE_FAST               1 (state_name)
                
-               588         204 LOAD_GLOBAL              6 (ts)
+               589         204 LOAD_GLOBAL              6 (ts)
                            216 LOAD_ATTR                4 (constants)
                            226 LOAD_ATTR                5 (STATE_NAMES)
                            236 LOAD_METHOD              0 (get)
                            258 LOAD_FAST                1 (state_name)
                            260 LOAD_CONST               5 ('')
                            262 PRECALL                  2
                            266 CALL                     2
                            276 STORE_FAST               2 (state_code)
                
-               589         278 LOAD_FAST                2 (state_code)
+               590         278 LOAD_FAST                2 (state_code)
                            280 RETURN_VALUE
                
-               591     >>  282 LOAD_CONST               0 (None)
+               592     >>  282 LOAD_CONST               0 (None)
                            284 RETURN_VALUE
                consts
                   None
                   'state'
                   'headquarters'
                   ','
                   -1
                   ''
                names      ('get', 'split', 'strip', 'ts', 'constants', 'STATE_NAMES')
                varnames   ('row', 'state_name', 'state_code')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_state'
-               firstlineno 583
+               firstlineno 584
                lnotab 0x02012a0110012a0166014a010402
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
@@ -3032,67 +3032,67 @@
                   010000ab01000000000000000072087c0064011900000000000000000053
                   007c00a00000000000000000000000000000000000000000006402a60100
                   00ab01000000000000000072357c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017c01530064
                   005300
-               593           0 RESUME                   0
+               594           0 RESUME                   0
                
-               594           2 LOAD_FAST                0 (row)
+               595           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('city')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               595          44 LOAD_FAST                0 (row)
+               596          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('city')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               596     >>   60 LOAD_FAST                0 (row)
+               597     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    53 (to 208)
                
-               597         102 LOAD_FAST                0 (row)
+               598         102 LOAD_FAST                0 (row)
                            104 LOAD_CONST               2 ('headquarters')
                            106 BINARY_SUBSCR
                            116 LOAD_METHOD              1 (split)
                            138 LOAD_CONST               3 (',')
                            140 PRECALL                  1
                            144 CALL                     1
                            154 LOAD_CONST               4 (0)
                            156 BINARY_SUBSCR
                            166 LOAD_METHOD              2 (strip)
                            188 PRECALL                  0
                            192 CALL                     0
                            202 STORE_FAST               1 (city_name)
                
-               598         204 LOAD_FAST                1 (city_name)
+               599         204 LOAD_FAST                1 (city_name)
                            206 RETURN_VALUE
                
-               600     >>  208 LOAD_CONST               0 (None)
+               601     >>  208 LOAD_CONST               0 (None)
                            210 RETURN_VALUE
                consts
                   None
                   'city'
                   'headquarters'
                   ','
                   0
                names      ('get', 'split', 'strip')
                varnames   ('row', 'city_name')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_city'
-               firstlineno 593
+               firstlineno 594
                lnotab 0x02012a0110012a0166010402
             'end_customer'
             'meta'
             'employees'
             'ownership'
             1
             ('axis',)
@@ -3102,15 +3102,15 @@
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df', 'list_to_csv', 'get_employees', 'get_ownership', 'get_state', 'get_city')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_targets'
          firstlineno 478
          lnotab
-            0x0203043f34011801260106fe100474fb2e07160c060c0608060a06093c
+            0x0203044034011801260106fe100474fb2e07160c060c0608060a06093c
             013c013c0134013402
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3121,59 +3121,59 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         611           0 RESUME                   0
+         612           0 RESUME                   0
          
-         612           2 LOAD_CONST               1 ("\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    ")
+         613           2 LOAD_CONST               1 ("\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    ")
                        4 STORE_FAST               1 (statement)
          
-         624           6 LOAD_GLOBAL              0 (db)
+         625           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         625          58 LOAD_FAST                2 (conn)
+         626          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         626          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         627          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         627         120 LOAD_CONST               2 ('search_uid')
+         628         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         625         126 PRECALL                  2
+         626         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         629         142 LOAD_GLOBAL             11 (NULL + pd)
+         630         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         624         258 LOAD_CONST               0 (None)
+         625         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3184,15 +3184,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         630     >>  304 LOAD_FAST                4 (df)
+         631     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3201,15 +3201,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_comments'
-         firstlineno 611
+         firstlineno 612
          lnotab 0x0201040c34011801260106fe100474fb2e06
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3220,56 +3220,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         633           0 RESUME                   0
+         634           0 RESUME                   0
          
-         634           2 LOAD_GLOBAL              0 (db)
+         635           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         635          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         636          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         640          58 LOAD_FAST                1 (conn)
+         641          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         641         142 LOAD_GLOBAL             11 (NULL + pd)
+         642         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         634         258 LOAD_CONST               0 (None)
+         635         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3280,15 +3280,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         642     >>  304 LOAD_FAST                4 (df)
+         643     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3297,15 +3297,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 633
+         firstlineno 634
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3317,65 +3317,65 @@
             007c01a6010000ab01000000000000000064027c006901a6020000ab0200
             000000000000007d03740f000000000000000000006a0800000000000000
             007c03a0090000000000000000000000000000000000000000a6000000ab
             0000000000000000007c03a00a0000000000000000000000000000000000
             000000a6000000ab000000000000000000ac03a6020000ab020000000000
             0000007d04640064006400a6020000ab02000000000000000001006e0b23
             0031007304770278035900770101005900010001007c045300
-         645           0 RESUME                   0
+         646           0 RESUME                   0
          
-         646           2 LOAD_GLOBAL              1 (NULL + isinstance)
+         647           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (search_uid)
                       16 LOAD_GLOBAL              2 (int)
                       28 PRECALL                  2
                       32 CALL                     2
                       42 POP_JUMP_FORWARD_IF_TRUE     2 (to 48)
                       44 LOAD_ASSERTION_ERROR
                       46 RAISE_VARARGS            1
          
-         647     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
+         648     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
                       50 STORE_FAST               1 (statement)
          
-         669          52 LOAD_GLOBAL              4 (db)
+         670          52 LOAD_GLOBAL              4 (db)
                       64 LOAD_METHOD              3 (connect)
                       86 PRECALL                  0
                       90 CALL                     0
                      100 BEFORE_WITH
                      102 STORE_FAST               2 (conn)
          
-         670         104 LOAD_FAST                2 (conn)
+         671         104 LOAD_FAST                2 (conn)
                      106 LOAD_METHOD              4 (execute)
                      128 LOAD_GLOBAL             11 (NULL + sqlalchemy)
                      140 LOAD_ATTR                6 (text)
                      150 LOAD_FAST                1 (statement)
                      152 PRECALL                  1
                      156 CALL                     1
                      166 LOAD_CONST               2 ('search_uid')
                      168 LOAD_FAST                0 (search_uid)
                      170 BUILD_MAP                1
                      172 PRECALL                  2
                      176 CALL                     2
                      186 STORE_FAST               3 (result)
          
-         671         188 LOAD_GLOBAL             15 (NULL + pd)
+         672         188 LOAD_GLOBAL             15 (NULL + pd)
                      200 LOAD_ATTR                8 (DataFrame)
                      210 LOAD_FAST                3 (result)
                      212 LOAD_METHOD              9 (fetchall)
                      234 PRECALL                  0
                      238 CALL                     0
                      248 LOAD_FAST                3 (result)
                      250 LOAD_METHOD             10 (keys)
                      272 PRECALL                  0
                      276 CALL                     0
                      286 KW_NAMES                 3
                      288 PRECALL                  2
                      292 CALL                     2
                      302 STORE_FAST               4 (df)
          
-         669         304 LOAD_CONST               0 (None)
+         670         304 LOAD_CONST               0 (None)
                      306 LOAD_CONST               0 (None)
                      308 LOAD_CONST               0 (None)
                      310 PRECALL                  2
                      314 CALL                     2
                      324 POP_TOP
                      326 JUMP_FORWARD            11 (to 350)
                  >>  328 PUSH_EXC_INFO
@@ -3386,15 +3386,15 @@
                      338 POP_EXCEPT
                      340 RERAISE                  1
                  >>  342 POP_TOP
                      344 POP_EXCEPT
                      346 POP_TOP
                      348 POP_TOP
          
-         672     >>  350 LOAD_FAST                4 (df)
+         673     >>  350 LOAD_FAST                4 (df)
                      352 RETURN_VALUE
          ExceptionTable:
            102 to 302 -> 328 [1] lasti
            328 to 334 -> 336 [3] lasti
            342 to 342 -> 336 [3] lasti
          consts
             None
@@ -3403,15 +3403,15 @@
             ('columns',)
          names      ('isinstance', 'int', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event_history'
-         firstlineno 645
+         firstlineno 646
          lnotab 0x02012e0104163401540174fe2e03
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3422,56 +3422,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         675           0 RESUME                   0
+         676           0 RESUME                   0
          
-         677           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
+         678           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         695           6 LOAD_GLOBAL              0 (db)
+         696           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         696          58 LOAD_FAST                2 (conn)
+         697          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         697         142 LOAD_GLOBAL             11 (NULL + pd)
+         698         142 LOAD_GLOBAL             11 (NULL + pd)
                      154 LOAD_ATTR                6 (DataFrame)
                      164 LOAD_FAST                3 (result)
                      166 LOAD_METHOD              7 (fetchall)
                      188 PRECALL                  0
                      192 CALL                     0
                      202 LOAD_FAST                3 (result)
                      204 LOAD_METHOD              8 (keys)
                      226 PRECALL                  0
                      230 CALL                     0
                      240 KW_NAMES                 3
                      242 PRECALL                  2
                      246 CALL                     2
                      256 STORE_FAST               4 (df)
          
-         695         258 LOAD_CONST               0 (None)
+         696         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3482,15 +3482,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         698     >>  304 LOAD_FAST                4 (df)
+         699     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3499,15 +3499,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_criteria_history'
-         firstlineno 675
+         firstlineno 676
          lnotab 0x020204123401540174fe2e03
       'uid'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 7
          flags     : 3
@@ -3525,96 +3525,96 @@
             000000000000007d05741300000000000000000000741400000000000000
             0000006a0b00000000000000006a0c00000000000000007c05a6020000ab
             0200000000000000007d067c066a0d0000000000000000a00e0000000000
             0000000000000000000000000000006403a6010000ab0100000000000000
             006404190000000000000000007c066a0f000000000000000064053c0000
             00640064006400a6020000ab02000000000000000001006e0b2300310073
             04770278035900770101005900010001007c065300
-         704           0 RESUME                   0
+         705           0 RESUME                   0
          
-         705           2 LOAD_GLOBAL              0 (db)
+         706           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         706          54 LOAD_CONST               1 ("\n            SELECT \n                uid, \n                label, \n                meta, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            ")
+         707          54 LOAD_CONST               1 ("\n            SELECT \n                uid, \n                label, \n                meta, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            ")
                       56 STORE_FAST               2 (statement)
          
-         719          58 LOAD_FAST                1 (conn)
+         720          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('uid')
                      122 LOAD_FAST                0 (uid)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         721         142 LOAD_FAST                3 (result)
+         722         142 LOAD_FAST                3 (result)
                      144 LOAD_METHOD              5 (fetchone)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 STORE_FAST               4 (row)
          
-         722         182 LOAD_FAST                4 (row)
+         723         182 LOAD_FAST                4 (row)
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 214)
          
-         723         186 NOP
+         724         186 NOP
          
-         705         188 LOAD_CONST               0 (None)
+         706         188 LOAD_CONST               0 (None)
                      190 LOAD_CONST               0 (None)
                      192 LOAD_CONST               0 (None)
                      194 PRECALL                  2
                      198 CALL                     2
                      208 POP_TOP
                      210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         725     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         726     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                4 (row)
                      278 PRECALL                  2
                      282 CALL                     2
                      292 PRECALL                  1
                      296 CALL                     1
                      306 STORE_FAST               5 (obj)
          
-         726         308 LOAD_GLOBAL             19 (NULL + from_dict)
+         727         308 LOAD_GLOBAL             19 (NULL + from_dict)
                      320 LOAD_GLOBAL             20 (ts)
                      332 LOAD_ATTR               11 (models)
                      342 LOAD_ATTR               12 (Search)
                      352 LOAD_FAST                5 (obj)
                      354 PRECALL                  2
                      358 CALL                     2
                      368 STORE_FAST               6 (search)
          
-         727         370 LOAD_FAST                6 (search)
+         728         370 LOAD_FAST                6 (search)
                      372 LOAD_ATTR               13 (label)
                      382 LOAD_METHOD             14 (split)
                      404 LOAD_CONST               3 (' - ')
                      406 PRECALL                  1
                      410 CALL                     1
                      420 LOAD_CONST               4 (0)
                      422 BINARY_SUBSCR
                      432 LOAD_FAST                6 (search)
                      434 LOAD_ATTR               15 (meta)
                      444 LOAD_CONST               5 ('client')
                      446 STORE_SUBSCR
          
-         705         450 LOAD_CONST               0 (None)
+         706         450 LOAD_CONST               0 (None)
                      452 LOAD_CONST               0 (None)
                      454 LOAD_CONST               0 (None)
                      456 PRECALL                  2
                      460 CALL                     2
                      470 POP_TOP
                      472 JUMP_FORWARD            11 (to 496)
                  >>  474 PUSH_EXC_INFO
@@ -3625,15 +3625,15 @@
                      484 POP_EXCEPT
                      486 RERAISE                  1
                  >>  488 POP_TOP
                      490 POP_EXCEPT
                      492 POP_TOP
                      494 POP_TOP
          
-         729     >>  496 LOAD_FAST                6 (search)
+         730     >>  496 LOAD_FAST                6 (search)
                      498 RETURN_VALUE
          ExceptionTable:
            52 to 186 -> 474 [1] lasti
            214 to 448 -> 474 [1] lasti
            474 to 480 -> 482 [3] lasti
            488 to 488 -> 482 [3] lasti
          consts
@@ -3645,52 +3645,52 @@
             'client'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'fetchone', 'dict', 'zip', 'keys', 'from_dict', 'ts', 'models', 'Search', 'label', 'split', 'meta')
          varnames   ('uid', 'conn', 'statement', 'result', 'row', 'obj', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search'
-         firstlineno 704
+         firstlineno 705
          lnotab 0x02013401040d54022801040102ee1a145e013e0150ea2e18
       'searchToken'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
             017c017c016401190000000000000000007c006b02000000001900000000
             00000000007d027c026a0100000000000000007202640053007405000000
             000000000000007c026a0300000000000000006402190000000000000000
             00640319000000000000000000a6010000ab0100000000000000005300
-         732           0 RESUME                   0
+         733           0 RESUME                   0
          
-         733           2 LOAD_GLOBAL              1 (NULL + searches_query)
+         734           2 LOAD_GLOBAL              1 (NULL + searches_query)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (searches)
          
-         734          30 LOAD_FAST                1 (searches)
+         735          30 LOAD_FAST                1 (searches)
                       32 LOAD_FAST                1 (searches)
                       34 LOAD_CONST               1 ('searchToken')
                       36 BINARY_SUBSCR
                       46 LOAD_FAST                0 (searchToken)
                       48 COMPARE_OP               2 (==)
                       54 BINARY_SUBSCR
                       64 STORE_FAST               2 (search)
          
-         735          66 LOAD_FAST                2 (search)
+         736          66 LOAD_FAST                2 (search)
                       68 LOAD_ATTR                1 (empty)
                       78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
          
-         736          80 LOAD_CONST               0 (None)
+         737          80 LOAD_CONST               0 (None)
                       82 RETURN_VALUE
          
-         738     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
+         739     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
                       96 LOAD_FAST                2 (search)
                       98 LOAD_ATTR                3 (iloc)
                      108 LOAD_CONST               2 (0)
                      110 BINARY_SUBSCR
                      120 LOAD_CONST               3 ('uid')
                      122 BINARY_SUBSCR
                      132 PRECALL                  1
@@ -3703,15 +3703,15 @@
             'uid'
          names      ('searches_query', 'empty', 'find_search', 'iloc')
          varnames   ('searchToken', 'searches', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_token'
-         firstlineno 732
+         firstlineno 733
          lnotab 0x02011c0124010e010402
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3725,41 +3725,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         741           0 RESUME                   0
+         742           0 RESUME                   0
          
-         742           2 LOAD_GLOBAL              0 (db)
+         743           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         743          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         744          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         748          58 LOAD_FAST                1 (conn)
+         749          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('domain')
                      122 LOAD_FAST                0 (domain)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         742         142 LOAD_CONST               0 (None)
+         743         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3770,24 +3770,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         750     >>  188 LOAD_FAST                3 (result)
+         751     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         751         210 LOAD_CONST               0 (None)
+         752         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         753     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         754     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3795,15 +3795,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         754         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         755         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3816,15 +3816,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 741
+         firstlineno 742
          lnotab 0x02013401040554fa2e08160104028201
       'email'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3839,41 +3839,41 @@
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000006a0c00000000000000006a0d00000000000000007c
             04a6020000ab0200000000000000005300
-         757           0 RESUME                   0
+         758           0 RESUME                   0
          
-         758           2 LOAD_GLOBAL              0 (db)
+         759           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         759          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
+         760          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
                       56 STORE_FAST               2 (statement)
          
-         764          58 LOAD_FAST                1 (conn)
+         765          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('email')
                      122 LOAD_FAST                0 (email)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         758         142 LOAD_CONST               0 (None)
+         759         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3884,24 +3884,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         766     >>  188 LOAD_FAST                3 (result)
+         767     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         767         210 LOAD_CONST               0 (None)
+         768         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         769     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         770     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3909,15 +3909,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         770         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         771         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (ts)
                      368 LOAD_ATTR               12 (models)
                      378 LOAD_ATTR               13 (Actor)
                      388 LOAD_FAST                4 (obj)
                      390 PRECALL                  2
                      394 CALL                     2
                      404 RETURN_VALUE
@@ -3932,15 +3932,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'ts', 'models', 'Actor')
          varnames   ('email', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_actor_by_email'
-         firstlineno 757
+         firstlineno 758
          lnotab 0x02013401040554fa2e08160104028201
       'event_id'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3954,41 +3954,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         773           0 RESUME                   0
+         774           0 RESUME                   0
          
-         774           2 LOAD_GLOBAL              0 (db)
+         775           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         775          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+         776          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         780          58 LOAD_FAST                1 (conn)
+         781          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('event_id')
                      122 LOAD_FAST                0 (event_id)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         774         142 LOAD_CONST               0 (None)
+         775         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3999,24 +3999,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         782     >>  188 LOAD_FAST                3 (result)
+         783     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         783         210 LOAD_CONST               0 (None)
+         784         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         785     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         786     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -4024,15 +4024,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         786         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         787         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Event)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -4045,15 +4045,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
          varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
-         firstlineno 773
+         firstlineno 774
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 12
          flags     : 3
          code
@@ -4065,71 +4065,71 @@
             000000000000007c006a0800000000000000007c006a0900000000000000
             007415000000000000000000006a0b00000000000000007c006a0c000000
             0000000000a6010000ab01000000000000000064029c06a6020000ab0200
             0000000000000001007c01a00d0000000000000000000000000000000000
             000000a6000000ab0000000000000000000100640064006400a6020000ab
             020000000000000000010064005300230031007304770278035900770101
             0059000100010064005300
-         792           0 RESUME                   0
+         793           0 RESUME                   0
          
-         793           2 LOAD_GLOBAL              0 (db)
+         794           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         794          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
+         795          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         806          58 LOAD_FAST                1 (conn)
+         807          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         807          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         808          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         809         120 LOAD_FAST                0 (company)
+         810         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (uid)
          
-         810         132 LOAD_FAST                0 (company)
+         811         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (name)
          
-         811         144 LOAD_FAST                0 (company)
+         812         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (description)
          
-         812         156 LOAD_FAST                0 (company)
+         813         156 LOAD_FAST                0 (company)
                      158 LOAD_ATTR                8 (domain)
          
-         813         168 LOAD_FAST                0 (company)
+         814         168 LOAD_FAST                0 (company)
                      170 LOAD_ATTR                9 (source)
          
-         814         180 LOAD_GLOBAL             21 (NULL + json)
+         815         180 LOAD_GLOBAL             21 (NULL + json)
                      192 LOAD_ATTR               11 (dumps)
                      202 LOAD_FAST                0 (company)
                      204 LOAD_ATTR               12 (meta)
                      214 PRECALL                  1
                      218 CALL                     1
          
-         808         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
+         809         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
                      230 BUILD_CONST_KEY_MAP      6
          
-         806         232 PRECALL                  2
+         807         232 PRECALL                  2
                      236 CALL                     2
                      246 POP_TOP
          
-         818         248 LOAD_FAST                1 (conn)
+         819         248 LOAD_FAST                1 (conn)
                      250 LOAD_METHOD             13 (commit)
                      272 PRECALL                  0
                      276 CALL                     0
                      286 POP_TOP
          
-         793         288 LOAD_CONST               0 (None)
+         794         288 LOAD_CONST               0 (None)
                      290 LOAD_CONST               0 (None)
                      292 LOAD_CONST               0 (None)
                      294 PRECALL                  2
                      298 CALL                     2
                      308 POP_TOP
                      310 LOAD_CONST               0 (None)
                      312 RETURN_VALUE
@@ -4156,15 +4156,15 @@
             ('uid', 'name', 'description', 'domain', 'source', 'meta')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'uid', 'name', 'description', 'domain', 'source', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 792
+         firstlineno 793
          lnotab 0x02013401040c180126020c010c010c010c010c0130fa04fe100c28e7
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
@@ -4174,58 +4174,58 @@
             006a0400000000000000006401a6010000ab010000000000000000740b00
             0000000000000000006a0600000000000000007c006a0700000000000000
             00a6010000ab0100000000000000007c006a08000000000000000064029c
             02a6020000ab02000000000000000001007c01a009000000000000000000
             0000000000000000000000a6000000ab0000000000000000000100640064
             006400a6020000ab02000000000000000001006400530023003100730477
             02780359007701010059000100010064005300
-         821           0 RESUME                   0
+         822           0 RESUME                   0
          
-         822           2 LOAD_GLOBAL              0 (db)
+         823           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         823          54 LOAD_FAST                1 (conn)
+         824          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         824          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         825          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         825         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
+         826         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
          
-         824         102 PRECALL                  1
+         825         102 PRECALL                  1
                      106 CALL                     1
          
-         834         116 LOAD_GLOBAL             11 (NULL + json)
+         835         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (meta)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         835         164 LOAD_FAST                0 (search)
+         836         164 LOAD_FAST                0 (search)
                      166 LOAD_ATTR                8 (uid)
          
-         833         176 LOAD_CONST               2 (('meta', 'uid'))
+         834         176 LOAD_CONST               2 (('meta', 'uid'))
                      178 BUILD_CONST_KEY_MAP      2
          
-         823         180 PRECALL                  2
+         824         180 PRECALL                  2
                      184 CALL                     2
                      194 POP_TOP
          
-         838         196 LOAD_FAST                1 (conn)
+         839         196 LOAD_FAST                1 (conn)
                      198 LOAD_METHOD              9 (commit)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 POP_TOP
          
-         822         236 LOAD_CONST               0 (None)
+         823         236 LOAD_CONST               0 (None)
                      238 LOAD_CONST               0 (None)
                      240 LOAD_CONST               0 (None)
                      242 PRECALL                  2
                      246 CALL                     2
                      256 POP_TOP
                      258 LOAD_CONST               0 (None)
                      260 RETURN_VALUE
@@ -4252,15 +4252,15 @@
             ('meta', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'meta', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 821
+         firstlineno 822
          lnotab 0x020134011801160102ff0e0a30010cfe04f6100f28f0
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4271,61 +4271,61 @@
             006901a6020000ab02000000000000000001007c01a00200000000000000
             000000000000000000000000007407000000000000000000006a04000000
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00500000000000000000000000000000000000000
             00a6000000ab0000000000000000000100640064006400a6020000ab0200
             000000000000000100640053002300310073047702780359007701010059
             000100010064005300
-         844           0 RESUME                   0
+         845           0 RESUME                   0
          
-         846           2 LOAD_GLOBAL              0 (db)
+         847           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         847          54 LOAD_FAST                1 (conn)
+         848          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         848          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         849          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         849         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
+         850         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
          
-         848         102 PRECALL                  1
+         849         102 PRECALL                  1
                      106 CALL                     1
          
-         857         116 LOAD_CONST               2 ('event_id')
+         858         116 LOAD_CONST               2 ('event_id')
                      118 LOAD_FAST                0 (event_id)
          
-         856         120 BUILD_MAP                1
+         857         120 BUILD_MAP                1
          
-         847         122 PRECALL                  2
+         848         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         860         138 LOAD_FAST                1 (conn)
+         861         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         861         216 LOAD_FAST                1 (conn)
+         862         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              5 (commit)
                      240 PRECALL                  0
                      244 CALL                     0
                      254 POP_TOP
          
-         846         256 LOAD_CONST               0 (None)
+         847         256 LOAD_CONST               0 (None)
                      258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 PRECALL                  2
                      266 CALL                     2
                      276 POP_TOP
                      278 LOAD_CONST               0 (None)
                      280 RETURN_VALUE
@@ -4353,15 +4353,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('event_id', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'mute_event'
-         firstlineno 844
+         firstlineno 845
          lnotab 0x020234011801160102ff0e0904ff02f7100d4e0128f1
       'comment_id'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -4373,58 +4373,58 @@
             0064027c006901a6020000ab02000000000000000001007c01a002000000
             00000000000000000000000000000000007407000000000000000000006a
             0400000000000000006403a6010000ab010000000000000000a6010000ab
             01000000000000000001007c01a005000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-         867           0 RESUME                   0
+         868           0 RESUME                   0
          
-         868           2 LOAD_GLOBAL              0 (db)
+         869           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         869          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
+         870          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         873          58 LOAD_FAST                1 (conn)
+         874          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 LOAD_CONST               2 ('comment_id')
                      122 LOAD_FAST                0 (comment_id)
                      124 BUILD_MAP                1
                      126 PRECALL                  2
                      130 CALL                     2
                      140 POP_TOP
          
-         874         142 LOAD_FAST                1 (conn)
+         875         142 LOAD_FAST                1 (conn)
                      144 LOAD_METHOD              2 (execute)
                      166 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      178 LOAD_ATTR                4 (text)
                      188 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      190 PRECALL                  1
                      194 CALL                     1
                      204 PRECALL                  1
                      208 CALL                     1
                      218 POP_TOP
          
-         875         220 LOAD_FAST                1 (conn)
+         876         220 LOAD_FAST                1 (conn)
                      222 LOAD_METHOD              5 (commit)
                      244 PRECALL                  0
                      248 CALL                     0
                      258 POP_TOP
          
-         868         260 LOAD_CONST               0 (None)
+         869         260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 LOAD_CONST               0 (None)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 POP_TOP
                      282 LOAD_CONST               0 (None)
                      284 RETURN_VALUE
@@ -4452,15 +4452,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('comment_id', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'delete_comment'
-         firstlineno 867
+         firstlineno 868
          lnotab 0x02013401040454014e0128f9
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4473,71 +4473,71 @@
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00200000000000000000000000000000000000000
             007407000000000000000000006a0400000000000000006404a6010000ab
             010000000000000000a6010000ab01000000000000000001007c01a00500
             00000000000000000000000000000000000000a6000000ab000000000000
             0000000100640064006400a6020000ab0200000000000000000100640053
             002300310073047702780359007701010059000100010064005300
-         878           0 RESUME                   0
+         879           0 RESUME                   0
          
-         882           2 LOAD_GLOBAL              0 (db)
+         883           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         883          54 LOAD_FAST                1 (conn)
+         884          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         884          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         885          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         885         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
+         886         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
          
-         884         102 PRECALL                  1
+         885         102 PRECALL                  1
                      106 CALL                     1
          
-         891         116 LOAD_CONST               2 ('search_uid')
+         892         116 LOAD_CONST               2 ('search_uid')
                      118 LOAD_FAST                0 (search_uid)
                      120 BUILD_MAP                1
          
-         883         122 PRECALL                  2
+         884         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         893         138 LOAD_FAST                1 (conn)
+         894         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         894         216 LOAD_FAST                1 (conn)
+         895         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              2 (execute)
                      240 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      252 LOAD_ATTR                4 (text)
                      262 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW rating')
                      264 PRECALL                  1
                      268 CALL                     1
                      278 PRECALL                  1
                      282 CALL                     1
                      292 POP_TOP
          
-         897         294 LOAD_FAST                1 (conn)
+         898         294 LOAD_FAST                1 (conn)
                      296 LOAD_METHOD              5 (commit)
                      318 PRECALL                  0
                      322 CALL                     0
                      332 POP_TOP
          
-         882         334 LOAD_CONST               0 (None)
+         883         334 LOAD_CONST               0 (None)
                      336 LOAD_CONST               0 (None)
                      338 LOAD_CONST               0 (None)
                      340 PRECALL                  2
                      344 CALL                     2
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
@@ -4566,22 +4566,22 @@
             'REFRESH MATERIALIZED VIEW rating'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('search_uid', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'reset_inbox'
-         firstlineno 878
+         firstlineno 879
          lnotab 0x020434011801160102ff0e0706f8100a4e014e0328f1
       (False, None)
    names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'important_targets_from_event', 'int', 'str', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'average_rating_per_search_query', 'validation_history', 'searches_comment_counts', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'search_comments', 'event', 'event_history', 'search_criteria_history', 'find_search', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010c010c011002080108010c010c02140208010c010c
       011c021406101e240e100f1010244c020102fb04010eff020202fe020302
       fd020402fc020502fb020602fa08601620060c162b0614061b160e163e0c
-      7f00061a161a0c1a1e1a1d241c2409101010101013101d10171017100b
+      7f00071a161a0c1a1e1a1d241c2409101010101013101d10171017100b
```

### Comparing `gandai-1.7.50/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.51/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/analytics.py` & `gandai-1.7.51/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/constants.py` & `gandai-1.7.51/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/db.py` & `gandai-1.7.51/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/google.py` & `gandai-1.7.51/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/gpt.py` & `gandai-1.7.51/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/grata.py` & `gandai-1.7.51/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/helpers.py` & `gandai-1.7.51/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/main.py` & `gandai-1.7.51/gandai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,14 @@
     print(update_event)
     ts.query.insert_event(update_event)
     return resp
 
 
 def run_enrichment(event: ts.models.Event) -> None:
     domain = event.domain
-    search_uid = event.search_uid
 
     company = ts.query.find_company_by_domain(domain)
     if company.meta.get("company_uid"):
         print("company already exists. skipping enrichment...")
     else:
         resp = ts.grata.enrich(company.domain)
         company.name = company.name or resp.get("name")
```

### Comparing `gandai-1.7.50/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.51/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/migrations/db_seed.py` & `gandai-1.7.51/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/migrations/dealcloud.py` & `gandai-1.7.51/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.51/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/migrations/sql/schema.sql` & `gandai-1.7.51/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/models.py` & `gandai-1.7.51/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/query.py` & `gandai-1.7.51/gandai/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -492,15 +492,15 @@
         e.search_uid, 
         e.domain, 
         e.type as stage, 
         e.created as updated, 
         to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,
         a.name as updated_by, 
         c.name, 
-        c.description as grata_description,
+        -- c.description as grata_description,
         c.meta->>'description' as grata_description,
         c.meta->>'gpt_description' as gpt_description,
         c.source,
         -- uh is this necessary?
         c.meta->>'ownership' as ownership, 
         c.meta->>'headquarters' as headquarters,
         c.meta->>'city' as city,
@@ -534,14 +534,15 @@
     LEFT JOIN actor a ON e.actor_key = a.key
     LEFT JOIN company c ON e.domain = c.domain
     LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain
     LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain
     
     WHERE 
         e.rn = 1
+        AND e.domain != ''
     ;
     """
 
     with db.connect() as conn:
         result = conn.execute(
             sqlalchemy.text(statement),
             {"search_uid": search_uid},
```

### Comparing `gandai-1.7.50/gandai/secrets.py` & `gandai-1.7.51/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.50/gandai/tasks.py` & `gandai-1.7.51/gandai/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import gandai as ts
 from gandai import main
 from google.cloud import tasks_v2
 
 
 def trigger_process_event(event_id: int) -> None:
-    if False:
+    if True:
         main.process_event(event_id=event_id)
         # Thread(target=main.process_event, kwargs={"event_id": event_id}).start()
     else:
         client = tasks_v2.CloudTasksClient()
         parent = client.queue_path(
             project=os.getenv("GOOGLE_CLOUD_PROJECT", "targetselect-staging"),
             location="us-central1",
```

### Comparing `gandai-1.7.50/gandai.egg-info/SOURCES.txt` & `gandai-1.7.51/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

