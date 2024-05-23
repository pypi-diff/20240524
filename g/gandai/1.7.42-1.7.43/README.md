# Comparing `tmp/gandai-1.7.42.tar.gz` & `tmp/gandai-1.7.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.42.tar", last modified: Thu May 23 23:15:02 2024, max compression
+gzip compressed data, was "gandai-1.7.43.tar", last modified: Thu May 23 23:22:48 2024, max compression
```

## Comparing `gandai-1.7.42.tar` & `gandai-1.7.43.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.588358 gandai-1.7.42/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.42/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:15:02.588137 gandai-1.7.42/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.578137 gandai-1.7.42/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.42/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.584892 gandai-1.7.42/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.42/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.42/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.42/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.42/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2600 2024-03-29 15:40:37.000000 gandai-1.7.42/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.42/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.42/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.42/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7026 2024-05-23 22:33:44.000000 gandai-1.7.42/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.42/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2564 2024-05-23 22:34:21.000000 gandai-1.7.42/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    19281 2024-05-23 22:32:08.000000 gandai-1.7.42/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.42/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    42225 2024-05-23 22:23:40.000000 gandai-1.7.42/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.42/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.42/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.42/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1695 2024-05-07 15:22:26.000000 gandai-1.7.42/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.42/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1674 2024-03-29 15:34:07.000000 gandai-1.7.42/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.42/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.42/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)     6384 2024-05-23 22:33:42.000000 gandai-1.7.42/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.42/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1204 2024-05-23 22:34:19.000000 gandai-1.7.42/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    14648 2024-05-23 22:32:05.000000 gandai-1.7.42/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.585851 gandai-1.7.42/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.42/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.586341 gandai-1.7.42/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.42/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.42/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.42/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.42/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.42/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.587636 gandai-1.7.42/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.42/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.42/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.42/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.42/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.42/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    28619 2024-05-23 22:23:38.000000 gandai-1.7.42/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.42/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1079 2024-05-06 22:42:54.000000 gandai-1.7.42/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.587915 gandai-1.7.42/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:15:02.000000 gandai-1.7.42/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-23 23:15:02.000000 gandai-1.7.42/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-23 23:15:02.000000 gandai-1.7.42/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-23 23:15:02.000000 gandai-1.7.42/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-23 23:14:45.000000 gandai-1.7.42/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-23 23:15:02.588397 gandai-1.7.42/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.42/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.082462 gandai-1.7.43/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.43/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:22:48.082251 gandai-1.7.43/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.076172 gandai-1.7.43/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.43/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.080259 gandai-1.7.43/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.43/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.43/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.43/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.43/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2600 2024-03-29 15:40:37.000000 gandai-1.7.43/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.43/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.43/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.43/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7026 2024-05-23 22:33:44.000000 gandai-1.7.43/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.43/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2564 2024-05-23 22:34:21.000000 gandai-1.7.43/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    15748 2024-05-23 23:22:20.000000 gandai-1.7.43/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.43/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    42225 2024-05-23 22:23:40.000000 gandai-1.7.43/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.43/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.43/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.43/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1695 2024-05-07 15:22:26.000000 gandai-1.7.43/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.43/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1674 2024-03-29 15:34:07.000000 gandai-1.7.43/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.43/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.43/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)     6384 2024-05-23 22:33:42.000000 gandai-1.7.43/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.43/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1204 2024-05-23 22:34:19.000000 gandai-1.7.43/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    11083 2024-05-23 23:22:18.000000 gandai-1.7.43/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.080814 gandai-1.7.43/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.43/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.081198 gandai-1.7.43/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.43/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.43/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.43/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.43/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.43/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.081884 gandai-1.7.43/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.43/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.43/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.43/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.43/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.43/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    28619 2024-05-23 22:23:38.000000 gandai-1.7.43/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.43/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1079 2024-05-06 22:42:54.000000 gandai-1.7.43/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:22:48.082054 gandai-1.7.43/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:22:48.000000 gandai-1.7.43/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-23 23:22:48.000000 gandai-1.7.43/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-23 23:22:48.000000 gandai-1.7.43/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-23 23:22:48.000000 gandai-1.7.43/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-23 23:22:29.000000 gandai-1.7.43/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-23 23:22:48.082501 gandai-1.7.43/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.43/setup.py
```

### Comparing `gandai-1.7.42/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/query.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.43/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/analytics.py` & `gandai-1.7.43/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/constants.py` & `gandai-1.7.43/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/db.py` & `gandai-1.7.43/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/google.py` & `gandai-1.7.43/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/gpt.py` & `gandai-1.7.43/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/grata.py` & `gandai-1.7.43/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/helpers.py` & `gandai-1.7.43/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/main.py` & `gandai-1.7.43/gandai/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import re
-from concurrent.futures import ThreadPoolExecutor
-from dataclasses import asdict, dataclass, field
+from time import time
+from dataclasses import asdict
+from dacite import from_dict
 
 import gandai as ts
-import requests
-from bs4 import BeautifulSoup
-from dacite import from_dict
 
 
 def run_acquired_check(domain: str):
     company = ts.query.find_company_by_domain(domain)
     q = f"{company.name} was acquired"
     google_page_one = ts.google.search(q)  # top 10 results, could extend?
     messages = [
@@ -42,124 +39,14 @@
     updates: dict = ts.gpt.ask_gpt4(messages)
     print(updates)
     company.meta = {**company.meta, **updates}
     # this is where I could also make a comment
     ts.query.update_company(company)
 
 
-def enrich_with_gpt(company: ts.models.Company, search_uid: int) -> None:
-
-    HOW_TO_ENRICH = """
-    To update an attribute for a company you will create an event with the company's domain
-    of type "update". This will update that company's meta field 
-    here is an example 
-
-    {
-		"search_uid": 1,
-		"domain": "lol.com",
-		"actor_key": "chatgpt",
-		"type": "update",
-		"data": {
-			"contact_name": "Bob"
-		}
-	}
-
-    Here are all the fields you can 
-
-    c.meta->>'description' as description, -- a description of the company for use by private equity research analyst to understand the company.
-    c.meta->>'employees' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.
-    c.meta->>'ownership' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] 
-    c.meta->>'headquarters' as headquarters,
-    c.meta->>'city' as city,
-    c.meta->>'state' as state,
-    c.meta->>'designation' as designation,
-    c.meta->>'products' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.
-    c.meta->>'services' as services, -- services are intangible goods offered by the company. do not list products here.
-    c.meta->>'end_customer' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.
-    c.meta->>'geographies' as geographies, -- geographies are the areas where the company does business. 
-    c.meta->>'year_founded' as year_founded,
-    c.meta->>'linkedin' as linkedin, -- linkedinUrl 
-    c.meta->>'linkedin_range' as linkedin_range,
-    c.meta->>'industry' as industry,
-    c.meta->>'revenue_estimates' as revenue_estimates,
-    c.meta->>'location_count' as location_count,
-    c.meta->>'business_models' as business_models,
-    c.meta->>'facility_size' as facility_size,
-    c.meta->>'contact_name' as contact_name,
-    c.meta->>'contact_title' as contact_title,
-    c.meta->>'contact_email' as contact_email,
-    c.meta->>'contact_phone' as contact_phone,
-    c.meta->>'contact_address' as contact_address,
-
-    For fields that are lists, you will use a csv string 
-    For these lists, such as products or services, try to stick to top 5 or less areas of focus.
-
-    You will fill out the description field with a description of the company.
-    
-    If you are unsure, just leave that key out of the response data
-
-    """
-
-    HEADERS = {
-        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15",
-        "Accept": "text/html",
-        "Referer": "https://www.google.com",
-    }
-
-    def get_homepage_text(domain: str) -> str:
-        HEADERS = {
-            "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15",
-            "Accept": "text/html",
-            "Referer": "https://www.google.com",
-        }
-        try:
-            resp = requests.get(f"http://www.{domain}", headers=HEADERS)
-        except:
-            print(f"failed on www.{domain}\ntrying without www")
-            resp = requests.get(f"http://{domain}", headers=HEADERS)
-
-        soup = BeautifulSoup(resp.text, "html.parser")
-        homepage_text = soup.text.strip()
-        homepage_text = re.sub(r"\s+", " ", homepage_text)
-        print(homepage_text)
-        return homepage_text
-
-    homepage_text = get_homepage_text(company.domain)
-
-    messages = [
-        {
-            "role": "system",
-            "content": f"You will help us evaluate {company.name} for acquisition.",
-        },
-        {
-            "role": "system",
-            "content": f"You will consider this existing information: {asdict(company)}",  # the existing (and grata) data
-        },
-        {
-            "role": "system",
-            "content": f"You will consider this copy from the company homepage as the most up to date. homepage_text: {homepage_text}",
-        },
-        {
-            "role": "system",
-            "content": "You will respond with only the JSON object.",
-        },
-        {
-            "role": "user",
-            "content": HOW_TO_ENRICH,
-        },
-    ]
-
-    resp = ts.gpt.ask_gpt4(messages)
-    update_event = from_dict(ts.models.Event, resp)
-    update_event.search_uid = search_uid
-    print(update_event)
-    # ts.query.insert_event(update_event)
-
-    return resp
-
 
 def run_similarity_search(search: ts.models.Search, domain: str) -> None:
     grata_companies = ts.grata.find_similar(domain=domain, search=search)
     ts.query.insert_companies_as_targets(
         companies=grata_companies,
         search_uid=search.uid,
         actor_key="grata",
@@ -280,24 +167,55 @@
     for new_event in resp["events"]:
         print("new event:", new_event)
         e = from_dict(ts.models.Event, new_event)
         print(e)
         e.data["prompt"] = event.data["prompt"]
         ts.query.insert_event(e)
 
+def enrich_with_gpt(company: ts.models.Company) -> None:
+    print("enriching with gpt...")
+    homepage_text = ts.helpers.get_homepage_text(company.domain)
+    messages = [
+        {
+            "role": "system",
+            "content": f"You will help us evaluate {company.name} for acquisition.",
+        },
+        {
+            "role": "system",
+            "content": f"You will consider this existing information: {asdict(company)}",  # the existing (and grata) data
+        },
+        {
+            "role": "system",
+            "content": f"You will consider this copy from the company homepage as the most up to date. homepage_text: {homepage_text}",
+        },
+        {
+            "role": "system",
+            "content": "You will respond with only the JSON object.",
+        },
+        {
+            "role": "user",
+            "content": ts.gpt.HOW_TO_ENRICH,
+        },
+    ]
+
+    resp = ts.gpt.ask_gpt4(messages)
+    update_event = from_dict(ts.models.Event, resp)
+    update_event.data["gpt"] = int(time())
+    print(update_event)
+    ts.query.insert_event(update_event)
+    return resp
 
 def run_enrichment(event: ts.models.Event) -> None:
     domain = event.domain
     search_uid = event.search_uid
 
     company = ts.query.find_company_by_domain(domain)
     if company.meta.get("company_uid"):
         print("company already exists. skipping enrichment...")
     else:
-
         resp = ts.grata.enrich(company.domain)
         company.name = company.name or resp.get("name")
         company.description = resp.get("description")
         company.meta = {**company.meta, **resp}
         ts.query.update_company(company)
 
     enrich_with_gpt(company=company, search_uid=search_uid)
```

### Comparing `gandai-1.7.42/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.43/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/migrations/db_seed.py` & `gandai-1.7.43/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/migrations/dealcloud.py` & `gandai-1.7.43/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.43/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/migrations/sql/schema.sql` & `gandai-1.7.43/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/models.py` & `gandai-1.7.43/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/query.py` & `gandai-1.7.43/gandai/query.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/secrets.py` & `gandai-1.7.43/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai/tasks.py` & `gandai-1.7.43/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.42/gandai.egg-info/SOURCES.txt` & `gandai-1.7.43/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

