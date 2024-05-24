# Comparing `tmp/gandai-1.7.51.tar.gz` & `tmp/gandai-1.7.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.51.tar", last modified: Fri May 24 06:44:05 2024, max compression
+gzip compressed data, was "gandai-1.7.52.tar", last modified: Fri May 24 07:01:08 2024, max compression
```

## Comparing `gandai-1.7.51.tar` & `gandai-1.7.52.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.776359 gandai-1.7.51/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.51/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 06:44:05.776152 gandai-1.7.51/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.769453 gandai-1.7.51/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.51/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.773364 gandai-1.7.51/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.51/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.51/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.51/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.51/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2600 2024-05-24 00:47:47.000000 gandai-1.7.51/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.51/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.51/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.51/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7037 2024-05-23 23:56:05.000000 gandai-1.7.51/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.51/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-24 05:31:06.000000 gandai-1.7.51/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    16151 2024-05-24 06:42:01.000000 gandai-1.7.51/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.51/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    42420 2024-05-24 06:17:33.000000 gandai-1.7.51/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.51/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.51/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.51/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      836 2024-05-24 06:09:06.000000 gandai-1.7.51/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.51/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1674 2024-05-24 00:47:46.000000 gandai-1.7.51/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.51/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.51/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)     6395 2024-05-23 23:56:03.000000 gandai-1.7.51/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.51/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-24 05:31:04.000000 gandai-1.7.51/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    11300 2024-05-24 06:41:58.000000 gandai-1.7.51/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.773862 gandai-1.7.51/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.51/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.774227 gandai-1.7.51/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.51/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.51/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.51/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.51/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.51/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.775595 gandai-1.7.51/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.51/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.51/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.51/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.51/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.51/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    28730 2024-05-24 06:17:30.000000 gandai-1.7.51/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.51/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1056 2024-05-24 06:09:03.000000 gandai-1.7.51/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 06:44:05.775949 gandai-1.7.51/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 06:44:05.000000 gandai-1.7.51/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-24 06:44:05.000000 gandai-1.7.51/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-24 06:44:05.000000 gandai-1.7.51/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-24 06:44:05.000000 gandai-1.7.51/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-24 06:43:57.000000 gandai-1.7.51/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-24 06:44:05.776395 gandai-1.7.51/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.51/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:01:08.758267 gandai-1.7.52/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.52/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 07:01:08.758080 gandai-1.7.52/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:01:08.748149 gandai-1.7.52/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.52/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:01:08.754637 gandai-1.7.52/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.52/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.52/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.52/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.52/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2600 2024-05-24 00:47:47.000000 gandai-1.7.52/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.52/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.52/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.52/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7037 2024-05-23 23:56:05.000000 gandai-1.7.52/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.52/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-24 05:31:06.000000 gandai-1.7.52/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    15990 2024-05-24 06:59:26.000000 gandai-1.7.52/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.52/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    42429 2024-05-24 06:59:56.000000 gandai-1.7.52/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.52/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.52/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.52/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      836 2024-05-24 06:09:06.000000 gandai-1.7.52/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.52/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1674 2024-05-24 00:47:46.000000 gandai-1.7.52/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.52/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.52/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)     6395 2024-05-23 23:56:03.000000 gandai-1.7.52/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.52/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-24 05:31:04.000000 gandai-1.7.52/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    11376 2024-05-24 06:59:24.000000 gandai-1.7.52/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:01:08.755403 gandai-1.7.52/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.52/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:01:08.755835 gandai-1.7.52/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.52/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.52/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.52/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.52/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.52/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:01:08.757615 gandai-1.7.52/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.52/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.52/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.52/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.52/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.52/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    28739 2024-05-24 06:59:54.000000 gandai-1.7.52/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.52/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1056 2024-05-24 06:09:03.000000 gandai-1.7.52/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 07:01:08.757900 gandai-1.7.52/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 07:01:08.000000 gandai-1.7.52/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-24 07:01:08.000000 gandai-1.7.52/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-24 07:01:08.000000 gandai-1.7.52/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-24 07:01:08.000000 gandai-1.7.52/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-24 07:01:01.000000 gandai-1.7.52/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-24 07:01:08.758301 gandai-1.7.52/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.52/setup.py
```

### Comparing `gandai-1.7.51/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xb6365066 (Fri May 24 06:41:58 2024 UTC)
-files sz: 11300
+moddate:  0xcc3a5066 (Fri May 24 06:59:24 2024 UTC)
+files sz: 11376
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d025a020100640064
@@ -1490,74 +1490,71 @@
             000000000000007c027c03ac0aa6020000ab020000000000000000010064
             0053007c016a070000000000000000640d6b02000000007202640053007c
             016a070000000000000000640e6b02000000007202640053007c016a0700
             00000000000000640f6b020000000072237411000000000000000000007c
             01ac05a6010000ab01000000000000000001007415000000000000000000
             007c027c03ac0aa6020000ab0200000000000000000100640053007c016a
             07000000000000000064106b02000000007202640053007c016a07000000
-            000000000064116b020000000072127417000000000000000000007c01ac
+            000000000064116b020000000072127411000000000000000000007c01ac
             05a6010000ab0100000000000000000100640053007c016a070000000000
-            00000064126b020000000072387419000000000000000000007c016a0d00
-            000000000000006413190000000000000000006414190000000000000000
-            00a6010000ab01000000000000000064156b04000000007212741d000000
-            000000000000007c02ac16a6010000ab0100000000000000000100640053
-            00640053007c016a07000000000000000064176b02000000007213741f00
-            0000000000000000007c027c01ac18a6020000ab02000000000000000001
-            00640053007c016a07000000000000000064196b02000000007213742100
-            0000000000000000007c027c01ac18a6020000ab02000000000000000001
-            00640053007c016a070000000000000000641a6b02000000007222740200
-            0000000000000000006a020000000000000000a011000000000000000000
-            00000000000000000000007c01ac05a6010000ab01000000000000000001
-            00640053007c016a070000000000000000641b6b02000000007236740100
-            000000000000000000641ca6010000ab0100000000000000000100740200
+            00000064126b020000000072127417000000000000000000007c01ac05a6
+            010000ab0100000000000000000100640053007c016a0700000000000000
+            0064136b020000000072137419000000000000000000007c027c01ac14a6
+            020000ab0200000000000000000100640053007c016a0700000000000000
+            0064156b02000000007213741b000000000000000000007c027c01ac14a6
+            020000ab0200000000000000000100640053007c016a0700000000000000
+            0064166b020000000072227402000000000000000000006a020000000000
+            000000a00e00000000000000000000000000000000000000007c01ac05a6
+            010000ab0100000000000000000100640053007c016a0700000000000000
+            0064176b020000000072367401000000000000000000006418a6010000ab
+            01000000000000000001007402000000000000000000006a020000000000
+            000000a00f00000000000000000000000000000000000000007c026a1000
+            00000000000000ac19a6010000ab0100000000000000000100640053007c
+            016a070000000000000000641a6b02000000009001721f74010000000000
+            00000000007c01a6010000ab01000000000000000001007c016a11000000
+            0000000000641a190000000000000000007d047c016a1100000000000000
+            00641b190000000000000000007d057c04641c6b0200000000724c740200
             0000000000000000006a020000000000000000a012000000000000000000
-            00000000000000000000007c026a130000000000000000ac1da6010000ab
-            0100000000000000000100640053007c016a070000000000000000641e6b
-            02000000009001721f7401000000000000000000007c01a6010000ab0100
-            0000000000000001007c016a0d0000000000000000641e19000000000000
-            0000007d047c016a0d0000000000000000641f190000000000000000007d
-            057c0464206b0200000000724c7402000000000000000000006a02000000
-            0000000000a0140000000000000000000000000000000000000000740200
-            0000000000000000006a150000000000000000a016000000000000000000
-            00000000000000000000007c026a130000000000000000640d7c037c016a
-            170000000000000000ac21a6040000ab040000000000000000a6010000ab
-            0100000000000000000100640053007c0464226b0200000000724c740200
-            0000000000000000006a020000000000000000a014000000000000000000
-            00000000000000000000007402000000000000000000006a150000000000
-            000000a01600000000000000000000000000000000000000007c026a1300
-            0000000000000064237c037c016a170000000000000000ac21a6040000ab
+            00000000000000000000007402000000000000000000006a130000000000
+            000000a01400000000000000000000000000000000000000007c026a1000
+            00000000000000640d7c037c016a150000000000000000ac1da6040000ab
             040000000000000000a6010000ab0100000000000000000100640053007c
-            0564247600724c7402000000000000000000006a020000000000000000a0
-            140000000000000000000000000000000000000000740200000000000000
-            0000006a150000000000000000a016000000000000000000000000000000
-            00000000007c026a13000000000000000064087c037c016a170000000000
-            000000ac21a6040000ab040000000000000000a6010000ab010000000000
-            000000010064005300640053007c016a07000000000000000064256b0200
-            00000072b97c0372817402000000000000000000006a0200000000000000
-            00a01800000000000000000000000000000000000000007c03a6010000ab
-            0100000000000000007d067c016a0d0000000000000000a0190000000000
-            0000000000000000000000000000006426a6010000ab0100000000000000
-            0072127c016a0d00000000000000006426190000000000000000007c065f
-            1a000000000000000069007c066a1b0000000000000000a5017c016a0d00
-            00000000000000a5017c065f1b0000000000000000740200000000000000
-            0000006a020000000000000000a01c000000000000000000000000000000
-            00000000007c06a6010000ab01000000000000000001006400530069007c
-            026a1b0000000000000000a5017c016a0d0000000000000000a5017c025f
-            1b00000000000000007402000000000000000000006a0200000000000000
-            00a01d00000000000000000000000000000000000000007c02a6010000ab
-            0100000000000000000100640053007c016a07000000000000000064276b
-            020000000072757c016a0d00000000000000006428190000000000000000
-            0044005d697d0374010000000000000000000064297c03a6020000ab0200
-            0000000000000001007402000000000000000000006a0200000000000000
-            00a014000000000000000000000000000000000000000074020000000000
-            00000000006a150000000000000000a01600000000000000000000000000
-            000000000000007c026a1300000000000000007c037c016a0d0000000000
-            000000642a190000000000000000007c016a170000000000000000ac2ba6
-            040000ab040000000000000000a6010000ab01000000000000000001008c
-            686400530064005300
+            04641e6b0200000000724c7402000000000000000000006a020000000000
+            000000a01200000000000000000000000000000000000000007402000000
+            000000000000006a130000000000000000a0140000000000000000000000
+            0000000000000000007c026a100000000000000000641f7c037c016a1500
+            00000000000000ac1da6040000ab040000000000000000a6010000ab0100
+            000000000000000100640053007c0564207600724c740200000000000000
+            0000006a020000000000000000a012000000000000000000000000000000
+            00000000007402000000000000000000006a130000000000000000a01400
+            000000000000000000000000000000000000007c026a1000000000000000
+            0064087c037c016a150000000000000000ac1da6040000ab040000000000
+            000000a6010000ab010000000000000000010064005300640053007c016a
+            07000000000000000064216b020000000072b97c03728174020000000000
+            00000000006a020000000000000000a01600000000000000000000000000
+            000000000000007c03a6010000ab0100000000000000007d067c016a1100
+            00000000000000a017000000000000000000000000000000000000000064
+            22a6010000ab01000000000000000072127c016a11000000000000000064
+            22190000000000000000007c065f18000000000000000069007c066a1900
+            00000000000000a5017c016a110000000000000000a5017c065f19000000
+            00000000007402000000000000000000006a020000000000000000a01a00
+            000000000000000000000000000000000000007c06a6010000ab01000000
+            000000000001006400530069007c026a190000000000000000a5017c016a
+            110000000000000000a5017c025f19000000000000000074020000000000
+            00000000006a020000000000000000a01b00000000000000000000000000
+            000000000000007c02a6010000ab0100000000000000000100640053007c
+            016a07000000000000000064236b020000000072757c016a110000000000
+            00000064241900000000000000000044005d697d03740100000000000000
+            00000064257c03a6020000ab020000000000000000010074020000000000
+            00000000006a020000000000000000a01200000000000000000000000000
+            000000000000007402000000000000000000006a130000000000000000a0
+            1400000000000000000000000000000000000000007c026a100000000000
+            0000007c037c016a1100000000000000006426190000000000000000007c
+            016a150000000000000000ac27a6040000ab040000000000000000a60100
+            00ab01000000000000000001008c686400530064005300
          232           0 RESUME                   0
          
          233           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('processing event...')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
@@ -1758,386 +1755,370 @@
                      856 POP_JUMP_FORWARD_IF_FALSE     2 (to 862)
          
          262         858 LOAD_CONST               0 (None)
                      860 RETURN_VALUE
          
          265     >>  862 LOAD_FAST                1 (event)
                      864 LOAD_ATTR                7 (type)
-                     874 LOAD_CONST              17 ('prompt')
+                     874 LOAD_CONST              17 ('enrich')
                      876 COMPARE_OP               2 (==)
                      882 POP_JUMP_FORWARD_IF_FALSE    18 (to 920)
          
-         266         884 LOAD_GLOBAL             23 (NULL + handle_prompt)
+         266         884 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      896 LOAD_FAST                1 (event)
                      898 KW_NAMES                 5
                      900 PRECALL                  1
                      904 CALL                     1
                      914 POP_TOP
                      916 LOAD_CONST               0 (None)
                      918 RETURN_VALUE
          
-         267     >>  920 LOAD_FAST                1 (event)
+         268     >>  920 LOAD_FAST                1 (event)
                      922 LOAD_ATTR                7 (type)
-                     932 LOAD_CONST              18 ('criteria')
+                     932 LOAD_CONST              18 ('prompt')
                      934 COMPARE_OP               2 (==)
-                     940 POP_JUMP_FORWARD_IF_FALSE    56 (to 1054)
+                     940 POP_JUMP_FORWARD_IF_FALSE    18 (to 978)
          
-         268         942 LOAD_GLOBAL             25 (NULL + len)
+         269         942 LOAD_GLOBAL             23 (NULL + handle_prompt)
                      954 LOAD_FAST                1 (event)
-                     956 LOAD_ATTR               13 (data)
-                     966 LOAD_CONST              19 ('inclusion')
-                     968 BINARY_SUBSCR
-                     978 LOAD_CONST              20 ('keywords')
-                     980 BINARY_SUBSCR
-                     990 PRECALL                  1
-                     994 CALL                     1
-                    1004 LOAD_CONST              21 (0)
-                    1006 COMPARE_OP               4 (>)
-                    1012 POP_JUMP_FORWARD_IF_FALSE    18 (to 1050)
-         
-         269        1014 LOAD_GLOBAL             29 (NULL + run_criteria_search)
-                    1026 LOAD_FAST                2 (search)
-                    1028 KW_NAMES                22
-                    1030 PRECALL                  1
-                    1034 CALL                     1
-                    1044 POP_TOP
-                    1046 LOAD_CONST               0 (None)
-                    1048 RETURN_VALUE
-         
-         268     >> 1050 LOAD_CONST               0 (None)
-                    1052 RETURN_VALUE
-         
-         270     >> 1054 LOAD_FAST                1 (event)
-                    1056 LOAD_ATTR                7 (type)
-                    1066 LOAD_CONST              23 ('maps')
-                    1068 COMPARE_OP               2 (==)
-                    1074 POP_JUMP_FORWARD_IF_FALSE    19 (to 1114)
-         
-         271        1076 LOAD_GLOBAL             31 (NULL + run_maps_search)
-                    1088 LOAD_FAST                2 (search)
-                    1090 LOAD_FAST                1 (event)
-                    1092 KW_NAMES                24
-                    1094 PRECALL                  2
-                    1098 CALL                     2
-                    1108 POP_TOP
-                    1110 LOAD_CONST               0 (None)
-                    1112 RETURN_VALUE
-         
-         272     >> 1114 LOAD_FAST                1 (event)
-                    1116 LOAD_ATTR                7 (type)
-                    1126 LOAD_CONST              25 ('google')
-                    1128 COMPARE_OP               2 (==)
-                    1134 POP_JUMP_FORWARD_IF_FALSE    19 (to 1174)
-         
-         273        1136 LOAD_GLOBAL             33 (NULL + run_google_search)
-                    1148 LOAD_FAST                2 (search)
-                    1150 LOAD_FAST                1 (event)
-                    1152 KW_NAMES                24
-                    1154 PRECALL                  2
-                    1158 CALL                     2
-                    1168 POP_TOP
-                    1170 LOAD_CONST               0 (None)
-                    1172 RETURN_VALUE
-         
-         275     >> 1174 LOAD_FAST                1 (event)
-                    1176 LOAD_ATTR                7 (type)
-                    1186 LOAD_CONST              26 ('import')
-                    1188 COMPARE_OP               2 (==)
-                    1194 POP_JUMP_FORWARD_IF_FALSE    34 (to 1264)
-         
-         276        1196 LOAD_GLOBAL              2 (ts)
-                    1208 LOAD_ATTR                2 (query)
-                    1218 LOAD_METHOD             17 (important_targets_from_event)
-                    1240 LOAD_FAST                1 (event)
-                    1242 KW_NAMES                 5
-                    1244 PRECALL                  1
-                    1248 CALL                     1
-                    1258 POP_TOP
-                    1260 LOAD_CONST               0 (None)
-                    1262 RETURN_VALUE
-         
-         278     >> 1264 LOAD_FAST                1 (event)
-                    1266 LOAD_ATTR                7 (type)
-                    1276 LOAD_CONST              27 ('reset')
-                    1278 COMPARE_OP               2 (==)
-                    1284 POP_JUMP_FORWARD_IF_FALSE    54 (to 1394)
-         
-         279        1286 LOAD_GLOBAL              1 (NULL + print)
-                    1298 LOAD_CONST              28 ('💣 Resetting Inbox...')
-                    1300 PRECALL                  1
-                    1304 CALL                     1
-                    1314 POP_TOP
-         
-         280        1316 LOAD_GLOBAL              2 (ts)
-                    1328 LOAD_ATTR                2 (query)
-                    1338 LOAD_METHOD             18 (reset_inbox)
-                    1360 LOAD_FAST                2 (search)
-                    1362 LOAD_ATTR               19 (uid)
-                    1372 KW_NAMES                29
-                    1374 PRECALL                  1
-                    1378 CALL                     1
-                    1388 POP_TOP
-                    1390 LOAD_CONST               0 (None)
-                    1392 RETURN_VALUE
-         
-         282     >> 1394 LOAD_FAST                1 (event)
-                    1396 LOAD_ATTR                7 (type)
-                    1406 LOAD_CONST              30 ('rating')
-                    1408 COMPARE_OP               2 (==)
-                    1414 EXTENDED_ARG             1
-                    1416 POP_JUMP_FORWARD_IF_FALSE   287 (to 1992)
-         
-         284        1418 LOAD_GLOBAL              1 (NULL + print)
-                    1430 LOAD_FAST                1 (event)
-                    1432 PRECALL                  1
-                    1436 CALL                     1
-                    1446 POP_TOP
-         
-         285        1448 LOAD_FAST                1 (event)
-                    1450 LOAD_ATTR               13 (data)
-                    1460 LOAD_CONST              30 ('rating')
-                    1462 BINARY_SUBSCR
-                    1472 STORE_FAST               4 (rating)
-         
-         286        1474 LOAD_FAST                1 (event)
-                    1476 LOAD_ATTR               13 (data)
-                    1486 LOAD_CONST              31 ('currentView')
-                    1488 BINARY_SUBSCR
-                    1498 STORE_FAST               5 (from_stage)
-         
-         287        1500 LOAD_FAST                4 (rating)
-                    1502 LOAD_CONST              32 (1)
-                    1504 COMPARE_OP               2 (==)
-                    1510 POP_JUMP_FORWARD_IF_FALSE    76 (to 1664)
-         
-         288        1512 LOAD_GLOBAL              2 (ts)
-                    1524 LOAD_ATTR                2 (query)
-                    1534 LOAD_METHOD             20 (insert_event)
-         
-         289        1556 LOAD_GLOBAL              2 (ts)
-                    1568 LOAD_ATTR               21 (models)
-                    1578 LOAD_METHOD             22 (Event)
-         
-         290        1600 LOAD_FAST                2 (search)
-                    1602 LOAD_ATTR               19 (uid)
-         
-         291        1612 LOAD_CONST              13 ('reject')
-         
-         292        1614 LOAD_FAST                3 (domain)
-         
-         293        1616 LOAD_FAST                1 (event)
-                    1618 LOAD_ATTR               23 (actor_key)
-         
-         289        1628 KW_NAMES                33
-                    1630 PRECALL                  4
-                    1634 CALL                     4
-         
-         288        1644 PRECALL                  1
-                    1648 CALL                     1
-                    1658 POP_TOP
-                    1660 LOAD_CONST               0 (None)
-                    1662 RETURN_VALUE
-         
-         296     >> 1664 LOAD_FAST                4 (rating)
-                    1666 LOAD_CONST              34 (2)
-                    1668 COMPARE_OP               2 (==)
-                    1674 POP_JUMP_FORWARD_IF_FALSE    76 (to 1828)
-         
-         297        1676 LOAD_GLOBAL              2 (ts)
-                    1688 LOAD_ATTR                2 (query)
-                    1698 LOAD_METHOD             20 (insert_event)
-         
-         298        1720 LOAD_GLOBAL              2 (ts)
-                    1732 LOAD_ATTR               21 (models)
-                    1742 LOAD_METHOD             22 (Event)
-         
-         299        1764 LOAD_FAST                2 (search)
-                    1766 LOAD_ATTR               19 (uid)
-         
-         300        1776 LOAD_CONST              35 ('hold')
-         
-         301        1778 LOAD_FAST                3 (domain)
-         
-         302        1780 LOAD_FAST                1 (event)
-                    1782 LOAD_ATTR               23 (actor_key)
-         
-         298        1792 KW_NAMES                33
-                    1794 PRECALL                  4
-                    1798 CALL                     4
-         
-         297        1808 PRECALL                  1
-                    1812 CALL                     1
-                    1822 POP_TOP
-                    1824 LOAD_CONST               0 (None)
-                    1826 RETURN_VALUE
-         
-         305     >> 1828 LOAD_FAST                5 (from_stage)
-                    1830 LOAD_CONST              36 (('land', 'create', 'advance', 'hold'))
-                    1832 CONTAINS_OP              0
-                    1834 POP_JUMP_FORWARD_IF_FALSE    76 (to 1988)
-         
-         306        1836 LOAD_GLOBAL              2 (ts)
-                    1848 LOAD_ATTR                2 (query)
-                    1858 LOAD_METHOD             20 (insert_event)
-         
-         307        1880 LOAD_GLOBAL              2 (ts)
-                    1892 LOAD_ATTR               21 (models)
-                    1902 LOAD_METHOD             22 (Event)
-         
-         308        1924 LOAD_FAST                2 (search)
-                    1926 LOAD_ATTR               19 (uid)
-         
-         309        1936 LOAD_CONST               8 ('validate')
-         
-         310        1938 LOAD_FAST                3 (domain)
-         
-         311        1940 LOAD_FAST                1 (event)
-                    1942 LOAD_ATTR               23 (actor_key)
-         
-         307        1952 KW_NAMES                33
-                    1954 PRECALL                  4
-                    1958 CALL                     4
-         
-         306        1968 PRECALL                  1
-                    1972 CALL                     1
-                    1982 POP_TOP
-                    1984 LOAD_CONST               0 (None)
-                    1986 RETURN_VALUE
-         
-         305     >> 1988 LOAD_CONST               0 (None)
-                    1990 RETURN_VALUE
-         
-         315     >> 1992 LOAD_FAST                1 (event)
-                    1994 LOAD_ATTR                7 (type)
-                    2004 LOAD_CONST              37 ('update')
-                    2006 COMPARE_OP               2 (==)
-                    2012 POP_JUMP_FORWARD_IF_FALSE   185 (to 2384)
-         
-         316        2014 LOAD_FAST                3 (domain)
-                    2016 POP_JUMP_FORWARD_IF_FALSE   129 (to 2276)
-         
-         317        2018 LOAD_GLOBAL              2 (ts)
-                    2030 LOAD_ATTR                2 (query)
-                    2040 LOAD_METHOD             24 (find_company_by_domain)
-                    2062 LOAD_FAST                3 (domain)
-                    2064 PRECALL                  1
-                    2068 CALL                     1
-                    2078 STORE_FAST               6 (company)
-         
-         318        2080 LOAD_FAST                1 (event)
-                    2082 LOAD_ATTR               13 (data)
-                    2092 LOAD_METHOD             25 (get)
-                    2114 LOAD_CONST              38 ('name')
-                    2116 PRECALL                  1
-                    2120 CALL                     1
-                    2130 POP_JUMP_FORWARD_IF_FALSE    18 (to 2168)
-         
-         319        2132 LOAD_FAST                1 (event)
-                    2134 LOAD_ATTR               13 (data)
-                    2144 LOAD_CONST              38 ('name')
-                    2146 BINARY_SUBSCR
-                    2156 LOAD_FAST                6 (company)
-                    2158 STORE_ATTR              26 (name)
-         
-         325     >> 2168 BUILD_MAP                0
-                    2170 LOAD_FAST                6 (company)
-                    2172 LOAD_ATTR               27 (meta)
-                    2182 DICT_UPDATE              1
-                    2184 LOAD_FAST                1 (event)
-                    2186 LOAD_ATTR               13 (data)
-                    2196 DICT_UPDATE              1
-                    2198 LOAD_FAST                6 (company)
-                    2200 STORE_ATTR              27 (meta)
-         
-         326        2210 LOAD_GLOBAL              2 (ts)
-                    2222 LOAD_ATTR                2 (query)
-                    2232 LOAD_METHOD             28 (update_company)
-                    2254 LOAD_FAST                6 (company)
-                    2256 PRECALL                  1
-                    2260 CALL                     1
-                    2270 POP_TOP
-                    2272 LOAD_CONST               0 (None)
-                    2274 RETURN_VALUE
-         
-         328     >> 2276 BUILD_MAP                0
-                    2278 LOAD_FAST                2 (search)
-                    2280 LOAD_ATTR               27 (meta)
-                    2290 DICT_UPDATE              1
-                    2292 LOAD_FAST                1 (event)
-                    2294 LOAD_ATTR               13 (data)
-                    2304 DICT_UPDATE              1
-                    2306 LOAD_FAST                2 (search)
-                    2308 STORE_ATTR              27 (meta)
-         
-         329        2318 LOAD_GLOBAL              2 (ts)
-                    2330 LOAD_ATTR                2 (query)
-                    2340 LOAD_METHOD             29 (update_search)
-                    2362 LOAD_FAST                2 (search)
-                    2364 PRECALL                  1
-                    2368 CALL                     1
-                    2378 POP_TOP
-                    2380 LOAD_CONST               0 (None)
-                    2382 RETURN_VALUE
-         
-         331     >> 2384 LOAD_FAST                1 (event)
-                    2386 LOAD_ATTR                7 (type)
-                    2396 LOAD_CONST              39 ('move')
-                    2398 COMPARE_OP               2 (==)
-                    2404 POP_JUMP_FORWARD_IF_FALSE   117 (to 2640)
-         
-         333        2406 LOAD_FAST                1 (event)
-                    2408 LOAD_ATTR               13 (data)
-                    2418 LOAD_CONST              40 ('domains')
-                    2420 BINARY_SUBSCR
-                    2430 GET_ITER
-                 >> 2432 FOR_ITER               105 (to 2644)
-                    2434 STORE_FAST               3 (domain)
-         
-         334        2436 LOAD_GLOBAL              1 (NULL + print)
-                    2448 LOAD_CONST              41 ('moving domain:')
-                    2450 LOAD_FAST                3 (domain)
-                    2452 PRECALL                  2
-                    2456 CALL                     2
-                    2466 POP_TOP
-         
-         335        2468 LOAD_GLOBAL              2 (ts)
-                    2480 LOAD_ATTR                2 (query)
-                    2490 LOAD_METHOD             20 (insert_event)
-         
-         336        2512 LOAD_GLOBAL              2 (ts)
-                    2524 LOAD_ATTR               21 (models)
-                    2534 LOAD_METHOD             22 (Event)
-         
-         337        2556 LOAD_FAST                2 (search)
-                    2558 LOAD_ATTR               19 (uid)
-         
-         338        2568 LOAD_FAST                3 (domain)
-         
-         339        2570 LOAD_FAST                1 (event)
-                    2572 LOAD_ATTR               13 (data)
-                    2582 LOAD_CONST              42 ('stage')
-                    2584 BINARY_SUBSCR
-         
-         340        2594 LOAD_FAST                1 (event)
-                    2596 LOAD_ATTR               23 (actor_key)
-         
-         336        2606 KW_NAMES                43
-                    2608 PRECALL                  4
-                    2612 CALL                     4
-         
-         335        2622 PRECALL                  1
-                    2626 CALL                     1
-                    2636 POP_TOP
-                    2638 JUMP_BACKWARD          104 (to 2432)
+                     956 KW_NAMES                 5
+                     958 PRECALL                  1
+                     962 CALL                     1
+                     972 POP_TOP
+                     974 LOAD_CONST               0 (None)
+                     976 RETURN_VALUE
+         
+         273     >>  978 LOAD_FAST                1 (event)
+                     980 LOAD_ATTR                7 (type)
+                     990 LOAD_CONST              19 ('maps')
+                     992 COMPARE_OP               2 (==)
+                     998 POP_JUMP_FORWARD_IF_FALSE    19 (to 1038)
+         
+         274        1000 LOAD_GLOBAL             25 (NULL + run_maps_search)
+                    1012 LOAD_FAST                2 (search)
+                    1014 LOAD_FAST                1 (event)
+                    1016 KW_NAMES                20
+                    1018 PRECALL                  2
+                    1022 CALL                     2
+                    1032 POP_TOP
+                    1034 LOAD_CONST               0 (None)
+                    1036 RETURN_VALUE
+         
+         275     >> 1038 LOAD_FAST                1 (event)
+                    1040 LOAD_ATTR                7 (type)
+                    1050 LOAD_CONST              21 ('google')
+                    1052 COMPARE_OP               2 (==)
+                    1058 POP_JUMP_FORWARD_IF_FALSE    19 (to 1098)
+         
+         276        1060 LOAD_GLOBAL             27 (NULL + run_google_search)
+                    1072 LOAD_FAST                2 (search)
+                    1074 LOAD_FAST                1 (event)
+                    1076 KW_NAMES                20
+                    1078 PRECALL                  2
+                    1082 CALL                     2
+                    1092 POP_TOP
+                    1094 LOAD_CONST               0 (None)
+                    1096 RETURN_VALUE
+         
+         278     >> 1098 LOAD_FAST                1 (event)
+                    1100 LOAD_ATTR                7 (type)
+                    1110 LOAD_CONST              22 ('import')
+                    1112 COMPARE_OP               2 (==)
+                    1118 POP_JUMP_FORWARD_IF_FALSE    34 (to 1188)
+         
+         279        1120 LOAD_GLOBAL              2 (ts)
+                    1132 LOAD_ATTR                2 (query)
+                    1142 LOAD_METHOD             14 (important_targets_from_event)
+                    1164 LOAD_FAST                1 (event)
+                    1166 KW_NAMES                 5
+                    1168 PRECALL                  1
+                    1172 CALL                     1
+                    1182 POP_TOP
+                    1184 LOAD_CONST               0 (None)
+                    1186 RETURN_VALUE
+         
+         281     >> 1188 LOAD_FAST                1 (event)
+                    1190 LOAD_ATTR                7 (type)
+                    1200 LOAD_CONST              23 ('reset')
+                    1202 COMPARE_OP               2 (==)
+                    1208 POP_JUMP_FORWARD_IF_FALSE    54 (to 1318)
+         
+         282        1210 LOAD_GLOBAL              1 (NULL + print)
+                    1222 LOAD_CONST              24 ('💣 Resetting Inbox...')
+                    1224 PRECALL                  1
+                    1228 CALL                     1
+                    1238 POP_TOP
+         
+         283        1240 LOAD_GLOBAL              2 (ts)
+                    1252 LOAD_ATTR                2 (query)
+                    1262 LOAD_METHOD             15 (reset_inbox)
+                    1284 LOAD_FAST                2 (search)
+                    1286 LOAD_ATTR               16 (uid)
+                    1296 KW_NAMES                25
+                    1298 PRECALL                  1
+                    1302 CALL                     1
+                    1312 POP_TOP
+                    1314 LOAD_CONST               0 (None)
+                    1316 RETURN_VALUE
+         
+         285     >> 1318 LOAD_FAST                1 (event)
+                    1320 LOAD_ATTR                7 (type)
+                    1330 LOAD_CONST              26 ('rating')
+                    1332 COMPARE_OP               2 (==)
+                    1338 EXTENDED_ARG             1
+                    1340 POP_JUMP_FORWARD_IF_FALSE   287 (to 1916)
+         
+         287        1342 LOAD_GLOBAL              1 (NULL + print)
+                    1354 LOAD_FAST                1 (event)
+                    1356 PRECALL                  1
+                    1360 CALL                     1
+                    1370 POP_TOP
+         
+         288        1372 LOAD_FAST                1 (event)
+                    1374 LOAD_ATTR               17 (data)
+                    1384 LOAD_CONST              26 ('rating')
+                    1386 BINARY_SUBSCR
+                    1396 STORE_FAST               4 (rating)
+         
+         289        1398 LOAD_FAST                1 (event)
+                    1400 LOAD_ATTR               17 (data)
+                    1410 LOAD_CONST              27 ('currentView')
+                    1412 BINARY_SUBSCR
+                    1422 STORE_FAST               5 (from_stage)
+         
+         290        1424 LOAD_FAST                4 (rating)
+                    1426 LOAD_CONST              28 (1)
+                    1428 COMPARE_OP               2 (==)
+                    1434 POP_JUMP_FORWARD_IF_FALSE    76 (to 1588)
+         
+         291        1436 LOAD_GLOBAL              2 (ts)
+                    1448 LOAD_ATTR                2 (query)
+                    1458 LOAD_METHOD             18 (insert_event)
+         
+         292        1480 LOAD_GLOBAL              2 (ts)
+                    1492 LOAD_ATTR               19 (models)
+                    1502 LOAD_METHOD             20 (Event)
+         
+         293        1524 LOAD_FAST                2 (search)
+                    1526 LOAD_ATTR               16 (uid)
+         
+         294        1536 LOAD_CONST              13 ('reject')
+         
+         295        1538 LOAD_FAST                3 (domain)
+         
+         296        1540 LOAD_FAST                1 (event)
+                    1542 LOAD_ATTR               21 (actor_key)
+         
+         292        1552 KW_NAMES                29
+                    1554 PRECALL                  4
+                    1558 CALL                     4
+         
+         291        1568 PRECALL                  1
+                    1572 CALL                     1
+                    1582 POP_TOP
+                    1584 LOAD_CONST               0 (None)
+                    1586 RETURN_VALUE
+         
+         299     >> 1588 LOAD_FAST                4 (rating)
+                    1590 LOAD_CONST              30 (2)
+                    1592 COMPARE_OP               2 (==)
+                    1598 POP_JUMP_FORWARD_IF_FALSE    76 (to 1752)
+         
+         300        1600 LOAD_GLOBAL              2 (ts)
+                    1612 LOAD_ATTR                2 (query)
+                    1622 LOAD_METHOD             18 (insert_event)
+         
+         301        1644 LOAD_GLOBAL              2 (ts)
+                    1656 LOAD_ATTR               19 (models)
+                    1666 LOAD_METHOD             20 (Event)
+         
+         302        1688 LOAD_FAST                2 (search)
+                    1690 LOAD_ATTR               16 (uid)
+         
+         303        1700 LOAD_CONST              31 ('hold')
+         
+         304        1702 LOAD_FAST                3 (domain)
+         
+         305        1704 LOAD_FAST                1 (event)
+                    1706 LOAD_ATTR               21 (actor_key)
+         
+         301        1716 KW_NAMES                29
+                    1718 PRECALL                  4
+                    1722 CALL                     4
+         
+         300        1732 PRECALL                  1
+                    1736 CALL                     1
+                    1746 POP_TOP
+                    1748 LOAD_CONST               0 (None)
+                    1750 RETURN_VALUE
+         
+         308     >> 1752 LOAD_FAST                5 (from_stage)
+                    1754 LOAD_CONST              32 (('land', 'create', 'advance', 'hold'))
+                    1756 CONTAINS_OP              0
+                    1758 POP_JUMP_FORWARD_IF_FALSE    76 (to 1912)
+         
+         309        1760 LOAD_GLOBAL              2 (ts)
+                    1772 LOAD_ATTR                2 (query)
+                    1782 LOAD_METHOD             18 (insert_event)
+         
+         310        1804 LOAD_GLOBAL              2 (ts)
+                    1816 LOAD_ATTR               19 (models)
+                    1826 LOAD_METHOD             20 (Event)
+         
+         311        1848 LOAD_FAST                2 (search)
+                    1850 LOAD_ATTR               16 (uid)
+         
+         312        1860 LOAD_CONST               8 ('validate')
+         
+         313        1862 LOAD_FAST                3 (domain)
+         
+         314        1864 LOAD_FAST                1 (event)
+                    1866 LOAD_ATTR               21 (actor_key)
+         
+         310        1876 KW_NAMES                29
+                    1878 PRECALL                  4
+                    1882 CALL                     4
+         
+         309        1892 PRECALL                  1
+                    1896 CALL                     1
+                    1906 POP_TOP
+                    1908 LOAD_CONST               0 (None)
+                    1910 RETURN_VALUE
+         
+         308     >> 1912 LOAD_CONST               0 (None)
+                    1914 RETURN_VALUE
+         
+         318     >> 1916 LOAD_FAST                1 (event)
+                    1918 LOAD_ATTR                7 (type)
+                    1928 LOAD_CONST              33 ('update')
+                    1930 COMPARE_OP               2 (==)
+                    1936 POP_JUMP_FORWARD_IF_FALSE   185 (to 2308)
+         
+         319        1938 LOAD_FAST                3 (domain)
+                    1940 POP_JUMP_FORWARD_IF_FALSE   129 (to 2200)
+         
+         320        1942 LOAD_GLOBAL              2 (ts)
+                    1954 LOAD_ATTR                2 (query)
+                    1964 LOAD_METHOD             22 (find_company_by_domain)
+                    1986 LOAD_FAST                3 (domain)
+                    1988 PRECALL                  1
+                    1992 CALL                     1
+                    2002 STORE_FAST               6 (company)
+         
+         321        2004 LOAD_FAST                1 (event)
+                    2006 LOAD_ATTR               17 (data)
+                    2016 LOAD_METHOD             23 (get)
+                    2038 LOAD_CONST              34 ('name')
+                    2040 PRECALL                  1
+                    2044 CALL                     1
+                    2054 POP_JUMP_FORWARD_IF_FALSE    18 (to 2092)
+         
+         322        2056 LOAD_FAST                1 (event)
+                    2058 LOAD_ATTR               17 (data)
+                    2068 LOAD_CONST              34 ('name')
+                    2070 BINARY_SUBSCR
+                    2080 LOAD_FAST                6 (company)
+                    2082 STORE_ATTR              24 (name)
+         
+         328     >> 2092 BUILD_MAP                0
+                    2094 LOAD_FAST                6 (company)
+                    2096 LOAD_ATTR               25 (meta)
+                    2106 DICT_UPDATE              1
+                    2108 LOAD_FAST                1 (event)
+                    2110 LOAD_ATTR               17 (data)
+                    2120 DICT_UPDATE              1
+                    2122 LOAD_FAST                6 (company)
+                    2124 STORE_ATTR              25 (meta)
+         
+         329        2134 LOAD_GLOBAL              2 (ts)
+                    2146 LOAD_ATTR                2 (query)
+                    2156 LOAD_METHOD             26 (update_company)
+                    2178 LOAD_FAST                6 (company)
+                    2180 PRECALL                  1
+                    2184 CALL                     1
+                    2194 POP_TOP
+                    2196 LOAD_CONST               0 (None)
+                    2198 RETURN_VALUE
+         
+         331     >> 2200 BUILD_MAP                0
+                    2202 LOAD_FAST                2 (search)
+                    2204 LOAD_ATTR               25 (meta)
+                    2214 DICT_UPDATE              1
+                    2216 LOAD_FAST                1 (event)
+                    2218 LOAD_ATTR               17 (data)
+                    2228 DICT_UPDATE              1
+                    2230 LOAD_FAST                2 (search)
+                    2232 STORE_ATTR              25 (meta)
+         
+         332        2242 LOAD_GLOBAL              2 (ts)
+                    2254 LOAD_ATTR                2 (query)
+                    2264 LOAD_METHOD             27 (update_search)
+                    2286 LOAD_FAST                2 (search)
+                    2288 PRECALL                  1
+                    2292 CALL                     1
+                    2302 POP_TOP
+                    2304 LOAD_CONST               0 (None)
+                    2306 RETURN_VALUE
+         
+         334     >> 2308 LOAD_FAST                1 (event)
+                    2310 LOAD_ATTR                7 (type)
+                    2320 LOAD_CONST              35 ('move')
+                    2322 COMPARE_OP               2 (==)
+                    2328 POP_JUMP_FORWARD_IF_FALSE   117 (to 2564)
+         
+         336        2330 LOAD_FAST                1 (event)
+                    2332 LOAD_ATTR               17 (data)
+                    2342 LOAD_CONST              36 ('domains')
+                    2344 BINARY_SUBSCR
+                    2354 GET_ITER
+                 >> 2356 FOR_ITER               105 (to 2568)
+                    2358 STORE_FAST               3 (domain)
+         
+         337        2360 LOAD_GLOBAL              1 (NULL + print)
+                    2372 LOAD_CONST              37 ('moving domain:')
+                    2374 LOAD_FAST                3 (domain)
+                    2376 PRECALL                  2
+                    2380 CALL                     2
+                    2390 POP_TOP
+         
+         338        2392 LOAD_GLOBAL              2 (ts)
+                    2404 LOAD_ATTR                2 (query)
+                    2414 LOAD_METHOD             18 (insert_event)
+         
+         339        2436 LOAD_GLOBAL              2 (ts)
+                    2448 LOAD_ATTR               19 (models)
+                    2458 LOAD_METHOD             20 (Event)
+         
+         340        2480 LOAD_FAST                2 (search)
+                    2482 LOAD_ATTR               16 (uid)
+         
+         341        2492 LOAD_FAST                3 (domain)
+         
+         342        2494 LOAD_FAST                1 (event)
+                    2496 LOAD_ATTR               17 (data)
+                    2506 LOAD_CONST              38 ('stage')
+                    2508 BINARY_SUBSCR
+         
+         343        2518 LOAD_FAST                1 (event)
+                    2520 LOAD_ATTR               21 (actor_key)
+         
+         339        2530 KW_NAMES                39
+                    2532 PRECALL                  4
+                    2536 CALL                     4
+         
+         338        2546 PRECALL                  1
+                    2550 CALL                     1
+                    2560 POP_TOP
+                    2562 JUMP_BACKWARD          104 (to 2356)
          
-         331     >> 2640 LOAD_CONST               0 (None)
-                    2642 RETURN_VALUE
+         334     >> 2564 LOAD_CONST               0 (None)
+                    2566 RETURN_VALUE
          
-         333     >> 2644 LOAD_CONST               0 (None)
-                    2646 RETURN_VALUE
+         336     >> 2568 LOAD_CONST               0 (None)
+                    2570 RETURN_VALUE
          consts
             None
             'processing event...'
             'event_id'
             ('uid',)
             'land'
             ('event',)
@@ -2148,20 +2129,16 @@
             ('search', 'domain')
             'send'
             'client_approve'
             'reject'
             'client_reject'
             'conflict'
             'client_conflict'
+            'enrich'
             'prompt'
-            'criteria'
-            'inclusion'
-            'keywords'
-            0
-            ('search',)
             'maps'
             ('search', 'event')
             'google'
             'import'
             'reset'
             '💣 Resetting Inbox...'
             ('search_uid',)
@@ -2175,29 +2152,29 @@
             'update'
             'name'
             'move'
             'domains'
             'moving domain:'
             'stage'
             ('search_uid', 'domain', 'type', 'actor_key')
-         names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'len', 'data', 'run_criteria_search', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'reset_inbox', 'uid', 'insert_event', 'models', 'Event', 'actor_key', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
+         names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'reset_inbox', 'uid', 'data', 'insert_event', 'models', 'Event', 'actor_key', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
          varnames   ('event_id', 'event', 'search', 'domain', 'rating', 'from_stage', 'company')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_event'
          firstlineno 232
          lnotab
             0x02011e013e0120011e014a010e01160124011601240116012401160120
             012001260116012401160120012601160104011601040116012001260116
-            010403160124011601480124ff040216012601160126021601440216011e
-            014e0218021e011a011a010c012c012c010c01020102010cfc10ff14080c
-            012c012c010c01020102010cfc10ff140808012c012c010c01020102010c
-            fc10ff14ff040a160104013e01340124062a0142022a01420216021e0120
-            012c012c010c01020118010cfc10ff12fc0402
+            010403160124021601240416012601160126021601440216011e014e0218
+            021e011a011a010c012c012c010c01020102010cfc10ff14080c012c012c
+            010c01020102010cfc10ff140808012c012c010c01020102010cfc10ff14
+            ff040a160104013e01340124062a0142022a01420216021e0120012c012c
+            010c01020118010cfc10ff12fc0402
    names      ('dataclasses', 'asdict', 'time', 'gandai', 'ts', 'dacite', 'from_dict', 'str', 'run_acquired_check', 'models', 'Search', 'run_similarity_search', 'run_criteria_search', 'Event', 'run_maps_search', 'run_google_search', 'handle_prompt', 'Company', 'enrich_with_gpt', 'run_enrichment', 'int', 'process_event')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
    name       '<module>'
    firstlineno 1
```

### Comparing `gandai-1.7.51/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xfa305066 (Fri May 24 06:17:30 2024 UTC)
-files sz: 28730
+moddate:  0xea3a5066 (Fri May 24 06:59:54 2024 UTC)
+files sz: 28739
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -2613,15 +2613,15 @@
             010000ab0100000000000000007c04640d3c0000007c04a00a0000000000
             0000000000000000000000000000007c08640eac0fa6020000ab02000000
             00000000007c0464103c0000007c04a00a00000000000000000000000000
             000000000000007c09640eac0fa6020000ab0200000000000000007c0464
             113c0000007c045300
          478           0 RESUME                   0
          
-         481           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    ")
+         481           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute','enrich')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
          545           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
@@ -2760,15 +2760,15 @@
                      636 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
-            "\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    "
+            "\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute','enrich')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        -- c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n        AND e.domain != ''\n    ;\n    "
             'search_uid'
             ('columns',)
             'return'
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
```

### Comparing `gandai-1.7.51/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.52/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/analytics.py` & `gandai-1.7.52/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/constants.py` & `gandai-1.7.52/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/db.py` & `gandai-1.7.52/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/google.py` & `gandai-1.7.52/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/gpt.py` & `gandai-1.7.52/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/grata.py` & `gandai-1.7.52/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/helpers.py` & `gandai-1.7.52/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/main.py` & `gandai-1.7.52/gandai/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,20 +257,23 @@
         pass
     elif event.type == "conflict":
         run_enrichment(event=event)
         run_similarity_search(search=search, domain=domain)
     elif event.type == "client_conflict":
         pass
 
+
+    elif event.type == "enrich":
+        run_enrichment(event=event)
     ## actions
     elif event.type == "prompt":
         handle_prompt(event=event)
-    elif event.type == "criteria":
-        if len(event.data["inclusion"]["keywords"]) > 0:
-            run_criteria_search(search=search)
+    # elif event.type == "criteria":
+    #     if len(event.data["inclusion"]["keywords"]) > 0:
+    #         run_criteria_search(search=search)
     elif event.type == "maps":
         run_maps_search(search=search, event=event)
     elif event.type == "google":
         run_google_search(search=search, event=event)
 
     elif event.type == "import":
         ts.query.important_targets_from_event(event=event)
```

### Comparing `gandai-1.7.51/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.52/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/migrations/db_seed.py` & `gandai-1.7.52/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/migrations/dealcloud.py` & `gandai-1.7.52/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.52/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/migrations/sql/schema.sql` & `gandai-1.7.52/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/models.py` & `gandai-1.7.52/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/query.py` & `gandai-1.7.52/gandai/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -482,15 +482,15 @@
     WITH RankedEvents AS (
         SELECT *,
             ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn
         FROM event
         WHERE 
             domain is not null
             AND search_uid = :search_uid
-            AND type NOT IN ('comment','rating','criteria','update','review','mute')
+            AND type NOT IN ('comment','rating','criteria','update','review','mute','enrich')
     )
     SELECT 
         e.search_uid, 
         e.domain, 
         e.type as stage, 
         e.created as updated, 
         to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,
```

### Comparing `gandai-1.7.51/gandai/secrets.py` & `gandai-1.7.52/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai/tasks.py` & `gandai-1.7.52/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.51/gandai.egg-info/SOURCES.txt` & `gandai-1.7.52/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

