# Comparing `tmp/gandai-1.7.47.tar.gz` & `tmp/gandai-1.7.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.47.tar", last modified: Fri May 24 05:35:23 2024, max compression
+gzip compressed data, was "gandai-1.7.48.tar", last modified: Fri May 24 05:36:21 2024, max compression
```

## Comparing `gandai-1.7.47.tar` & `gandai-1.7.48.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:35:23.786568 gandai-1.7.47/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.47/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 05:35:23.786367 gandai-1.7.47/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:35:23.779281 gandai-1.7.47/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.47/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:35:23.783974 gandai-1.7.47/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.47/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.47/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.47/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.47/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2600 2024-05-24 00:47:47.000000 gandai-1.7.47/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.47/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.47/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.47/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7037 2024-05-23 23:56:05.000000 gandai-1.7.47/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.47/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-24 05:31:06.000000 gandai-1.7.47/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    16150 2024-05-24 05:32:50.000000 gandai-1.7.47/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.47/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    42390 2024-05-24 03:52:51.000000 gandai-1.7.47/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.47/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.47/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.47/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      836 2024-05-24 05:34:43.000000 gandai-1.7.47/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.47/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1674 2024-05-24 00:47:46.000000 gandai-1.7.47/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.47/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.47/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)     6395 2024-05-23 23:56:03.000000 gandai-1.7.47/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.47/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-24 05:31:04.000000 gandai-1.7.47/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    11293 2024-05-24 05:32:48.000000 gandai-1.7.47/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:35:23.784414 gandai-1.7.47/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.47/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:35:23.784755 gandai-1.7.47/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.47/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.47/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.47/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.47/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.47/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:35:23.785908 gandai-1.7.47/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.47/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.47/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.47/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.47/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.47/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    28700 2024-05-24 03:52:49.000000 gandai-1.7.47/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.47/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1056 2024-05-24 05:34:41.000000 gandai-1.7.47/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:35:23.786180 gandai-1.7.47/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 05:35:23.000000 gandai-1.7.47/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-24 05:35:23.000000 gandai-1.7.47/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-24 05:35:23.000000 gandai-1.7.47/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-24 05:35:23.000000 gandai-1.7.47/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-24 05:35:10.000000 gandai-1.7.47/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-24 05:35:23.786600 gandai-1.7.47/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.47/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:36:21.634535 gandai-1.7.48/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.48/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 05:36:21.634343 gandai-1.7.48/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:36:21.629350 gandai-1.7.48/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.48/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:36:21.632609 gandai-1.7.48/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.48/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.48/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.48/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.48/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2600 2024-05-24 00:47:47.000000 gandai-1.7.48/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.48/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.48/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.48/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7037 2024-05-23 23:56:05.000000 gandai-1.7.48/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.48/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2703 2024-05-24 05:31:06.000000 gandai-1.7.48/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    16150 2024-05-24 05:32:50.000000 gandai-1.7.48/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.48/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    42390 2024-05-24 03:52:51.000000 gandai-1.7.48/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.48/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.48/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.48/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1550 2024-05-24 05:36:08.000000 gandai-1.7.48/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.48/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1674 2024-05-24 00:47:46.000000 gandai-1.7.48/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.48/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.48/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)     6395 2024-05-23 23:56:03.000000 gandai-1.7.48/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.48/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1283 2024-05-24 05:31:04.000000 gandai-1.7.48/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    11293 2024-05-24 05:32:48.000000 gandai-1.7.48/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:36:21.633129 gandai-1.7.48/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.48/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:36:21.633382 gandai-1.7.48/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.48/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.48/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.48/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.48/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.48/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:36:21.633944 gandai-1.7.48/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.48/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.48/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.48/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.48/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.48/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    28700 2024-05-24 03:52:49.000000 gandai-1.7.48/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.48/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1057 2024-05-24 05:36:06.000000 gandai-1.7.48/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 05:36:21.634142 gandai-1.7.48/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 05:36:21.000000 gandai-1.7.48/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-24 05:36:21.000000 gandai-1.7.48/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-24 05:36:21.000000 gandai-1.7.48/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-24 05:36:21.000000 gandai-1.7.48/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-24 05:36:13.000000 gandai-1.7.48/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-24 05:36:21.634574 gandai-1.7.48/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.48/setup.py
```

### Comparing `gandai-1.7.47/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.48/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/analytics.py` & `gandai-1.7.48/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/constants.py` & `gandai-1.7.48/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/db.py` & `gandai-1.7.48/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/google.py` & `gandai-1.7.48/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/gpt.py` & `gandai-1.7.48/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/grata.py` & `gandai-1.7.48/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/helpers.py` & `gandai-1.7.48/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/main.py` & `gandai-1.7.48/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.48/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/migrations/db_seed.py` & `gandai-1.7.48/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/migrations/dealcloud.py` & `gandai-1.7.48/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.48/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/migrations/sql/schema.sql` & `gandai-1.7.48/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/models.py` & `gandai-1.7.48/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/query.py` & `gandai-1.7.48/gandai/query.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/secrets.py` & `gandai-1.7.48/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.47/gandai/tasks.py` & `gandai-1.7.48/gandai/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import gandai as ts
 from gandai import main
 from google.cloud import tasks_v2
 
 
 def trigger_process_event(event_id: int) -> None:
-    if True:
+    if False:
         main.process_event(event_id=event_id)
         # Thread(target=main.process_event, kwargs={"event_id": event_id}).start()
     else:
         client = tasks_v2.CloudTasksClient()
         parent = client.queue_path(
             project=os.getenv("GOOGLE_CLOUD_PROJECT", "targetselect-staging"),
             location="us-central1",
```

### Comparing `gandai-1.7.47/gandai.egg-info/SOURCES.txt` & `gandai-1.7.48/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

