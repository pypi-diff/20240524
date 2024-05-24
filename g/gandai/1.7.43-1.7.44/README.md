# Comparing `tmp/gandai-1.7.43.tar.gz` & `tmp/gandai-1.7.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.43.tar", last modified: Thu May 23 23:22:48 2024, max compression
+gzip compressed data, was "gandai-1.7.44.tar", last modified: Thu May 23 23:35:03 2024, max compression
```

## Comparing `gandai-1.7.43.tar` & `gandai-1.7.44.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.082462 gandai-1.7.43/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.43/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:22:48.082251 gandai-1.7.43/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.076172 gandai-1.7.43/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.43/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.080259 gandai-1.7.43/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.43/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.43/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.43/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.43/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2600 2024-03-29 15:40:37.000000 gandai-1.7.43/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.43/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.43/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.43/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7026 2024-05-23 22:33:44.000000 gandai-1.7.43/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.43/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2564 2024-05-23 22:34:21.000000 gandai-1.7.43/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    15748 2024-05-23 23:22:20.000000 gandai-1.7.43/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.43/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    42225 2024-05-23 22:23:40.000000 gandai-1.7.43/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.43/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.43/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.43/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1695 2024-05-07 15:22:26.000000 gandai-1.7.43/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.43/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1674 2024-03-29 15:34:07.000000 gandai-1.7.43/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.43/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.43/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)     6384 2024-05-23 22:33:42.000000 gandai-1.7.43/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.43/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1204 2024-05-23 22:34:19.000000 gandai-1.7.43/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    11083 2024-05-23 23:22:18.000000 gandai-1.7.43/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.080814 gandai-1.7.43/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.43/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.081198 gandai-1.7.43/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.43/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.43/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.43/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.43/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.43/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.081884 gandai-1.7.43/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.43/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.43/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.43/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.43/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.43/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    28619 2024-05-23 22:23:38.000000 gandai-1.7.43/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.43/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1079 2024-05-06 22:42:54.000000 gandai-1.7.43/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.082054 gandai-1.7.43/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:22:48.000000 gandai-1.7.43/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-23 23:22:48.000000 gandai-1.7.43/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-23 23:22:48.000000 gandai-1.7.43/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-23 23:22:48.000000 gandai-1.7.43/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-23 23:22:29.000000 gandai-1.7.43/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-23 23:22:48.082501 gandai-1.7.43/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.43/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.777294 gandai-1.7.44/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.44/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:35:03.777106 gandai-1.7.44/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.767256 gandai-1.7.44/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.44/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.773867 gandai-1.7.44/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.44/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.44/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.44/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.44/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2600 2024-03-29 15:40:37.000000 gandai-1.7.44/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.44/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.44/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.44/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7026 2024-05-23 22:33:44.000000 gandai-1.7.44/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.44/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2564 2024-05-23 22:34:21.000000 gandai-1.7.44/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    15739 2024-05-23 23:34:14.000000 gandai-1.7.44/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.44/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    42225 2024-05-23 22:23:40.000000 gandai-1.7.44/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.44/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.44/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.44/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1695 2024-05-07 15:22:26.000000 gandai-1.7.44/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.44/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1674 2024-03-29 15:34:07.000000 gandai-1.7.44/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.44/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.44/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)     6384 2024-05-23 22:33:42.000000 gandai-1.7.44/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.44/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1204 2024-05-23 22:34:19.000000 gandai-1.7.44/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    11060 2024-05-23 23:34:12.000000 gandai-1.7.44/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.774798 gandai-1.7.44/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.44/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.775177 gandai-1.7.44/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.44/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.44/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.44/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.44/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.44/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.776663 gandai-1.7.44/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.44/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.44/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.44/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.44/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.44/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    28619 2024-05-23 22:23:38.000000 gandai-1.7.44/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.44/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1079 2024-05-06 22:42:54.000000 gandai-1.7.44/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.776919 gandai-1.7.44/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:35:03.000000 gandai-1.7.44/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-23 23:35:03.000000 gandai-1.7.44/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-23 23:35:03.000000 gandai-1.7.44/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-23 23:35:03.000000 gandai-1.7.44/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-23 23:34:32.000000 gandai-1.7.44/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-23 23:35:03.777332 gandai-1.7.44/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.44/setup.py
```

### Comparing `gandai-1.7.43/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xaacf4f66 (Thu May 23 23:22:18 2024 UTC)
-files sz: 11083
+moddate:  0x74d24f66 (Thu May 23 23:34:12 2024 UTC)
+files sz: 11060
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d005a000100640064026c016d025a020100640064
@@ -1269,15 +1269,15 @@
          firstlineno 174
          lnotab
             0x02011e014803020114fe0405020122fe0405020108fe0405020102fe04
             05020120fe04ef04173e013e0146011e013e01
       code
          argcount  : 1
          nlocals   : 5
-         stacksize : 4
+         stacksize : 3
          flags     : 3
          code
             0x97007c006a0000000000000000007d017c006a0100000000000000007d
             027404000000000000000000006a030000000000000000a0040000000000
             0000000000000000000000000000007c01a6010000ab0100000000000000
             007d037c036a050000000000000000a00600000000000000000000000000
             000000000000006401a6010000ab0100000000000000007210740f000000
@@ -1287,16 +1287,16 @@
             000000000000007d047c036a0a000000000000000070147c04a006000000
             00000000000000000000000000000000006403a6010000ab010000000000
             0000007c035f0a00000000000000007c04a0060000000000000000000000
             0000000000000000006404a6010000ab0100000000000000007c035f0b00
             0000000000000069007c036a050000000000000000a5017c04a5017c035f
             0500000000000000007404000000000000000000006a0300000000000000
             00a00c00000000000000000000000000000000000000007c03a6010000ab
-            0100000000000000000100741b000000000000000000007c037c02ac05a6
-            020000ab020000000000000000010064005300
+            0100000000000000000100741b000000000000000000007c03ac05a60100
+            00ab010000000000000000010064005300
          207           0 RESUME                   0
          
          208           2 LOAD_FAST                0 (event)
                        4 LOAD_ATTR                0 (domain)
                       14 STORE_FAST               1 (domain)
          
          209          16 LOAD_FAST                0 (event)
@@ -1369,28 +1369,27 @@
                      442 LOAD_FAST                3 (company)
                      444 PRECALL                  1
                      448 CALL                     1
                      458 POP_TOP
          
          221     >>  460 LOAD_GLOBAL             27 (NULL + enrich_with_gpt)
                      472 LOAD_FAST                3 (company)
-                     474 LOAD_FAST                2 (search_uid)
-                     476 KW_NAMES                 5
-                     478 PRECALL                  2
-                     482 CALL                     2
-                     492 POP_TOP
-                     494 LOAD_CONST               0 (None)
-                     496 RETURN_VALUE
+                     474 KW_NAMES                 5
+                     476 PRECALL                  1
+                     480 CALL                     1
+                     490 POP_TOP
+                     492 LOAD_CONST               0 (None)
+                     494 RETURN_VALUE
          consts
             None
             'company_uid'
             'company already exists. skipping enrichment...'
             'name'
             'description'
-            ('company', 'search_uid')
+            ('company',)
          names      ('domain', 'search_uid', 'ts', 'query', 'find_company_by_domain', 'meta', 'get', 'print', 'grata', 'enrich', 'name', 'description', 'update_company', 'enrich_with_gpt')
          varnames   ('event', 'domain', 'search_uid', 'company', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_enrichment'
          firstlineno 207
```

### Comparing `gandai-1.7.43/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.44/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/analytics.py` & `gandai-1.7.44/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/constants.py` & `gandai-1.7.44/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/db.py` & `gandai-1.7.44/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/google.py` & `gandai-1.7.44/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/gpt.py` & `gandai-1.7.44/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/grata.py` & `gandai-1.7.44/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/helpers.py` & `gandai-1.7.44/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/main.py` & `gandai-1.7.44/gandai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     else:
         resp = ts.grata.enrich(company.domain)
         company.name = company.name or resp.get("name")
         company.description = resp.get("description")
         company.meta = {**company.meta, **resp}
         ts.query.update_company(company)
 
-    enrich_with_gpt(company=company, search_uid=search_uid)
+    enrich_with_gpt(company=company)
 
 
 def process_event(event_id: int) -> None:
     print("processing event...")
     event: ts.models.Event = ts.query.find_event_by_id(event_id)
     print("event_id", event_id)
     print(event)
```

### Comparing `gandai-1.7.43/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.44/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/migrations/db_seed.py` & `gandai-1.7.44/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/migrations/dealcloud.py` & `gandai-1.7.44/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.44/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/migrations/sql/schema.sql` & `gandai-1.7.44/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/models.py` & `gandai-1.7.44/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/query.py` & `gandai-1.7.44/gandai/query.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/secrets.py` & `gandai-1.7.44/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai/tasks.py` & `gandai-1.7.44/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.43/gandai.egg-info/SOURCES.txt` & `gandai-1.7.44/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

