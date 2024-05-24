# Comparing `tmp/gandai-1.7.45.tar.gz` & `tmp/gandai-1.7.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.45.tar", last modified: Fri May 24 03:39:48 2024, max compression
+gzip compressed data, was "gandai-1.7.46.tar", last modified: Fri May 24 04:22:31 2024, max compression
```

## Comparing `gandai-1.7.45.tar` & `gandai-1.7.46.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.689491 gandai-1.7.45/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.45/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 03:39:48.689278 gandai-1.7.45/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.679484 gandai-1.7.45/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.45/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.686157 gandai-1.7.45/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.45/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.45/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.45/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.45/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2600 2024-05-24 00:47:47.000000 gandai-1.7.45/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.45/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.45/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.45/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7037 2024-05-23 23:56:05.000000 gandai-1.7.45/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.45/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2564 2024-05-23 22:34:21.000000 gandai-1.7.45/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    15923 2024-05-24 03:37:15.000000 gandai-1.7.45/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.45/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    42286 2024-05-23 23:53:21.000000 gandai-1.7.45/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.45/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.45/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.45/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1695 2024-05-24 03:39:23.000000 gandai-1.7.45/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.45/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1674 2024-05-24 00:47:46.000000 gandai-1.7.45/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.45/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.45/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)     6395 2024-05-23 23:56:03.000000 gandai-1.7.45/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.45/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1204 2024-05-23 22:34:19.000000 gandai-1.7.45/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    11171 2024-05-24 03:37:12.000000 gandai-1.7.45/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.686894 gandai-1.7.45/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.45/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.687288 gandai-1.7.45/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.45/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.45/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.45/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.45/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.45/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.688817 gandai-1.7.45/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.45/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.45/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.45/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.45/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.45/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    28680 2024-05-23 23:53:18.000000 gandai-1.7.45/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.45/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1079 2024-05-24 03:39:21.000000 gandai-1.7.45/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.689090 gandai-1.7.45/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 03:39:48.000000 gandai-1.7.45/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-24 03:39:48.000000 gandai-1.7.45/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-24 03:39:48.000000 gandai-1.7.45/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-24 03:39:48.000000 gandai-1.7.45/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-24 03:39:30.000000 gandai-1.7.45/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-24 03:39:48.689529 gandai-1.7.45/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.45/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 04:22:31.876515 gandai-1.7.46/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.46/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 04:22:31.876311 gandai-1.7.46/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 04:22:31.865461 gandai-1.7.46/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.46/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 04:22:31.873105 gandai-1.7.46/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.46/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.46/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.46/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.46/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2600 2024-05-24 00:47:47.000000 gandai-1.7.46/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.46/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.46/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.46/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7037 2024-05-23 23:56:05.000000 gandai-1.7.46/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.46/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2564 2024-05-23 22:34:21.000000 gandai-1.7.46/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    16137 2024-05-24 04:21:00.000000 gandai-1.7.46/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.46/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    42390 2024-05-24 03:52:51.000000 gandai-1.7.46/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.46/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.46/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.46/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1550 2024-05-24 03:50:42.000000 gandai-1.7.46/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.46/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1674 2024-05-24 00:47:46.000000 gandai-1.7.46/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.46/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.46/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)     6395 2024-05-23 23:56:03.000000 gandai-1.7.46/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.46/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1204 2024-05-23 22:34:19.000000 gandai-1.7.46/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    11281 2024-05-24 04:20:57.000000 gandai-1.7.46/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 04:22:31.873953 gandai-1.7.46/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.46/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 04:22:31.874367 gandai-1.7.46/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.46/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.46/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.46/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.46/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.46/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 04:22:31.875813 gandai-1.7.46/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.46/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.46/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.46/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.46/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.46/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    28700 2024-05-24 03:52:49.000000 gandai-1.7.46/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.46/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1057 2024-05-24 03:50:40.000000 gandai-1.7.46/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 04:22:31.876101 gandai-1.7.46/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 04:22:31.000000 gandai-1.7.46/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-24 04:22:31.000000 gandai-1.7.46/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-24 04:22:31.000000 gandai-1.7.46/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-24 04:22:31.000000 gandai-1.7.46/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-24 04:22:15.000000 gandai-1.7.46/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-24 04:22:31.876549 gandai-1.7.46/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.46/setup.py
```

### Comparing `gandai-1.7.45/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x680b5066 (Fri May 24 03:37:12 2024 UTC)
-files sz: 11171
+moddate:  0xa9155066 (Fri May 24 04:20:57 2024 UTC)
+files sz: 11281
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d025a020100640064
@@ -127,31 +127,31 @@
                314 LOAD_CONST               8 ('return')
                316 LOAD_CONST               3 (None)
                318 BUILD_TUPLE              4
                320 LOAD_CONST              16 (<code object enrich_with_gpt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 174>)
                322 MAKE_FUNCTION            4 (annotations)
                324 STORE_NAME              18 (enrich_with_gpt)
    
-   208         326 LOAD_CONST              11 ('event')
+   212         326 LOAD_CONST              11 ('event')
                328 LOAD_NAME                4 (ts)
                330 LOAD_ATTR                9 (models)
                340 LOAD_ATTR               13 (Event)
                350 LOAD_CONST               8 ('return')
                352 LOAD_CONST               3 (None)
                354 BUILD_TUPLE              4
-               356 LOAD_CONST              17 (<code object run_enrichment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 208>)
+               356 LOAD_CONST              17 (<code object run_enrichment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 212>)
                358 MAKE_FUNCTION            4 (annotations)
                360 STORE_NAME              19 (run_enrichment)
    
-   228         362 LOAD_CONST              18 ('event_id')
+   232         362 LOAD_CONST              18 ('event_id')
                364 LOAD_NAME               20 (int)
                366 LOAD_CONST               8 ('return')
                368 LOAD_CONST               3 (None)
                370 BUILD_TUPLE              4
-               372 LOAD_CONST              19 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 228>)
+               372 LOAD_CONST              19 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 232>)
                374 MAKE_FUNCTION            4 (annotations)
                376 STORE_NAME              21 (process_event)
                378 LOAD_CONST               3 (None)
                380 RETURN_VALUE
    consts
       0
       ('asdict',)
@@ -1107,173 +1107,214 @@
          lnotab
             0x02012003020120fe0405020120fe0405020120fe0405020120fe040502
             0120fe0405020112fe0405020112fe04041ee3041f3e021e01140120013e
             011e012a0140fb
       'company'
       code
          argcount  : 1
-         nlocals   : 5
+         nlocals   : 6
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
-            0001007402000000000000000000006a020000000000000000a003000000
-            00000000000000000000000000000000007c006a040000000000000000a6
-            010000ab0100000000000000007d01640264037c006a0500000000000000
-            009b0064049d0364059c0264026406740d000000000000000000007c00a6
-            010000ab0100000000000000009b009d0264059c02640264077c019b009d
-            0264059c026402640864059c0264097402000000000000000000006a0700
-            000000000000006a08000000000000000064059c0267057d027402000000
-            000000000000006a070000000000000000a0090000000000000000000000
-            0000000000000000007c02a6010000ab0100000000000000007d03741500
-            0000000000000000007402000000000000000000006a0b00000000000000
-            006a0c00000000000000007c03a6020000ab0200000000000000007d0474
-            1b00000000000000000000741d00000000000000000000a6000000ab0000
-            00000000000000a6010000ab0100000000000000007c046a0f0000000000
-            000000640a3c0000007401000000000000000000007c04a6010000ab0100
-            0000000000000001007402000000000000000000006a1000000000000000
-            00a01100000000000000000000000000000000000000007c04a6010000ab
-            01000000000000000001007c035300
+            00010009007402000000000000000000006a020000000000000000a00300
+            000000000000000000000000000000000000007c006a0400000000000000
+            00a6010000ab0100000000000000007d016e282300740a00000000000000
+            0000002400721b7d027401000000000000000000007c02a6010000ab0100
+            00000000000000010064027d01590064007d027e026e0864007d027e0277
+            017700780359007701640364047c006a0600000000000000009b0064059d
+            0364069c0264036407740f000000000000000000007c00a6010000ab0100
+            000000000000009b009d0264069c02640364087c019b009d0264069c0264
+            03640964069c02640a7402000000000000000000006a0800000000000000
+            006a09000000000000000064069c0267057d037402000000000000000000
+            006a080000000000000000a00a0000000000000000000000000000000000
+            0000007c03a6010000ab0100000000000000007d04741700000000000000
+            0000007402000000000000000000006a0c00000000000000006a0d000000
+            00000000007c04a6020000ab0200000000000000007d05741d0000000000
+            0000000000741f00000000000000000000a6000000ab0000000000000000
+            00a6010000ab0100000000000000007c056a100000000000000000640b3c
+            0000007401000000000000000000007c05a6010000ab0100000000000000
+            0001007402000000000000000000006a110000000000000000a012000000
+            00000000000000000000000000000000007c05a6010000ab010000000000
+            00000001007c045300
          174           0 RESUME                   0
          
          175           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('enriching with gpt...')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-         176          32 LOAD_GLOBAL              2 (ts)
-                      44 LOAD_ATTR                2 (helpers)
-                      54 LOAD_METHOD              3 (get_homepage_text)
-                      76 LOAD_FAST                0 (company)
-                      78 LOAD_ATTR                4 (domain)
-                      88 PRECALL                  1
-                      92 CALL                     1
-                     102 STORE_FAST               1 (homepage_text)
-         
-         179         104 LOAD_CONST               2 ('system')
-         
-         180         106 LOAD_CONST               3 ('You will help us evaluate ')
-                     108 LOAD_FAST                0 (company)
-                     110 LOAD_ATTR                5 (name)
-                     120 FORMAT_VALUE             0
-                     122 LOAD_CONST               4 (' for acquisition.')
-                     124 BUILD_STRING             3
-         
-         178         126 LOAD_CONST               5 (('role', 'content'))
-                     128 BUILD_CONST_KEY_MAP      2
-         
-         183         130 LOAD_CONST               2 ('system')
-         
-         184         132 LOAD_CONST               6 ('You will consider this existing information: ')
-                     134 LOAD_GLOBAL             13 (NULL + asdict)
-                     146 LOAD_FAST                0 (company)
-                     148 PRECALL                  1
-                     152 CALL                     1
-                     162 FORMAT_VALUE             0
-                     164 BUILD_STRING             2
-         
-         182         166 LOAD_CONST               5 (('role', 'content'))
-                     168 BUILD_CONST_KEY_MAP      2
-         
-         187         170 LOAD_CONST               2 ('system')
-         
-         188         172 LOAD_CONST               7 ('You will consider this copy from the company homepage as the most up to date. homepage_text: ')
-                     174 LOAD_FAST                1 (homepage_text)
-                     176 FORMAT_VALUE             0
-                     178 BUILD_STRING             2
-         
-         186         180 LOAD_CONST               5 (('role', 'content'))
-                     182 BUILD_CONST_KEY_MAP      2
-         
-         191         184 LOAD_CONST               2 ('system')
-         
-         192         186 LOAD_CONST               8 ('You will respond with only the JSON object.')
-         
-         190         188 LOAD_CONST               5 (('role', 'content'))
-                     190 BUILD_CONST_KEY_MAP      2
-         
-         195         192 LOAD_CONST               9 ('user')
-         
-         196         194 LOAD_GLOBAL              2 (ts)
-                     206 LOAD_ATTR                7 (gpt)
-                     216 LOAD_ATTR                8 (HOW_TO_ENRICH)
-         
-         194         226 LOAD_CONST               5 (('role', 'content'))
-                     228 BUILD_CONST_KEY_MAP      2
-         
-         177         230 BUILD_LIST               5
-                     232 STORE_FAST               2 (messages)
-         
-         200         234 LOAD_GLOBAL              2 (ts)
-                     246 LOAD_ATTR                7 (gpt)
-                     256 LOAD_METHOD              9 (ask_gpt4)
-                     278 LOAD_FAST                2 (messages)
-                     280 PRECALL                  1
-                     284 CALL                     1
-                     294 STORE_FAST               3 (resp)
-         
-         201         296 LOAD_GLOBAL             21 (NULL + from_dict)
-                     308 LOAD_GLOBAL              2 (ts)
-                     320 LOAD_ATTR               11 (models)
-                     330 LOAD_ATTR               12 (Event)
-                     340 LOAD_FAST                3 (resp)
-                     342 PRECALL                  2
-                     346 CALL                     2
-                     356 STORE_FAST               4 (update_event)
-         
-         202         358 LOAD_GLOBAL             27 (NULL + int)
-                     370 LOAD_GLOBAL             29 (NULL + time)
-                     382 PRECALL                  0
-                     386 CALL                     0
-                     396 PRECALL                  1
-                     400 CALL                     1
-                     410 LOAD_FAST                4 (update_event)
-                     412 LOAD_ATTR               15 (data)
-                     422 LOAD_CONST              10 ('gpt')
-                     424 STORE_SUBSCR
-         
-         203         428 LOAD_GLOBAL              1 (NULL + print)
-                     440 LOAD_FAST                4 (update_event)
-                     442 PRECALL                  1
-                     446 CALL                     1
-                     456 POP_TOP
-         
-         204         458 LOAD_GLOBAL              2 (ts)
-                     470 LOAD_ATTR               16 (query)
-                     480 LOAD_METHOD             17 (insert_event)
-                     502 LOAD_FAST                4 (update_event)
-                     504 PRECALL                  1
-                     508 CALL                     1
-                     518 POP_TOP
+         176          32 NOP
+         
+         177          34 LOAD_GLOBAL              2 (ts)
+                      46 LOAD_ATTR                2 (helpers)
+                      56 LOAD_METHOD              3 (get_homepage_text)
+                      78 LOAD_FAST                0 (company)
+                      80 LOAD_ATTR                4 (domain)
+                      90 PRECALL                  1
+                      94 CALL                     1
+                     104 STORE_FAST               1 (homepage_text)
+                     106 JUMP_FORWARD            40 (to 188)
+                 >>  108 PUSH_EXC_INFO
+         
+         178         110 LOAD_GLOBAL             10 (Exception)
+                     122 CHECK_EXC_MATCH
+                     124 POP_JUMP_FORWARD_IF_FALSE    27 (to 180)
+                     126 STORE_FAST               2 (e)
+         
+         179         128 LOAD_GLOBAL              1 (NULL + print)
+                     140 LOAD_FAST                2 (e)
+                     142 PRECALL                  1
+                     146 CALL                     1
+                     156 POP_TOP
+         
+         180         158 LOAD_CONST               2 ('<could not fetch homepage>')
+                     160 STORE_FAST               1 (homepage_text)
+                     162 POP_EXCEPT
+                     164 LOAD_CONST               0 (None)
+                     166 STORE_FAST               2 (e)
+                     168 DELETE_FAST              2 (e)
+                     170 JUMP_FORWARD             8 (to 188)
+                 >>  172 LOAD_CONST               0 (None)
+                     174 STORE_FAST               2 (e)
+                     176 DELETE_FAST              2 (e)
+                     178 RERAISE                  1
+         
+         178     >>  180 RERAISE                  0
+                 >>  182 COPY                     3
+                     184 POP_EXCEPT
+                     186 RERAISE                  1
+         
+         183     >>  188 LOAD_CONST               3 ('system')
+         
+         184         190 LOAD_CONST               4 ('You will help us evaluate ')
+                     192 LOAD_FAST                0 (company)
+                     194 LOAD_ATTR                6 (name)
+                     204 FORMAT_VALUE             0
+                     206 LOAD_CONST               5 (' for acquisition.')
+                     208 BUILD_STRING             3
+         
+         182         210 LOAD_CONST               6 (('role', 'content'))
+                     212 BUILD_CONST_KEY_MAP      2
+         
+         187         214 LOAD_CONST               3 ('system')
+         
+         188         216 LOAD_CONST               7 ('You will consider this existing information: ')
+                     218 LOAD_GLOBAL             15 (NULL + asdict)
+                     230 LOAD_FAST                0 (company)
+                     232 PRECALL                  1
+                     236 CALL                     1
+                     246 FORMAT_VALUE             0
+                     248 BUILD_STRING             2
+         
+         186         250 LOAD_CONST               6 (('role', 'content'))
+                     252 BUILD_CONST_KEY_MAP      2
+         
+         191         254 LOAD_CONST               3 ('system')
+         
+         192         256 LOAD_CONST               8 ('You will consider this copy from the company homepage as the most up to date. homepage_text: ')
+                     258 LOAD_FAST                1 (homepage_text)
+                     260 FORMAT_VALUE             0
+                     262 BUILD_STRING             2
+         
+         190         264 LOAD_CONST               6 (('role', 'content'))
+                     266 BUILD_CONST_KEY_MAP      2
+         
+         195         268 LOAD_CONST               3 ('system')
+         
+         196         270 LOAD_CONST               9 ('You will respond with only the JSON object.')
+         
+         194         272 LOAD_CONST               6 (('role', 'content'))
+                     274 BUILD_CONST_KEY_MAP      2
+         
+         199         276 LOAD_CONST              10 ('user')
+         
+         200         278 LOAD_GLOBAL              2 (ts)
+                     290 LOAD_ATTR                8 (gpt)
+                     300 LOAD_ATTR                9 (HOW_TO_ENRICH)
+         
+         198         310 LOAD_CONST               6 (('role', 'content'))
+                     312 BUILD_CONST_KEY_MAP      2
+         
+         181         314 BUILD_LIST               5
+                     316 STORE_FAST               3 (messages)
+         
+         204         318 LOAD_GLOBAL              2 (ts)
+                     330 LOAD_ATTR                8 (gpt)
+                     340 LOAD_METHOD             10 (ask_gpt4)
+                     362 LOAD_FAST                3 (messages)
+                     364 PRECALL                  1
+                     368 CALL                     1
+                     378 STORE_FAST               4 (resp)
+         
+         205         380 LOAD_GLOBAL             23 (NULL + from_dict)
+                     392 LOAD_GLOBAL              2 (ts)
+                     404 LOAD_ATTR               12 (models)
+                     414 LOAD_ATTR               13 (Event)
+                     424 LOAD_FAST                4 (resp)
+                     426 PRECALL                  2
+                     430 CALL                     2
+                     440 STORE_FAST               5 (update_event)
+         
+         206         442 LOAD_GLOBAL             29 (NULL + int)
+                     454 LOAD_GLOBAL             31 (NULL + time)
+                     466 PRECALL                  0
+                     470 CALL                     0
+                     480 PRECALL                  1
+                     484 CALL                     1
+                     494 LOAD_FAST                5 (update_event)
+                     496 LOAD_ATTR               16 (data)
+                     506 LOAD_CONST              11 ('gpt')
+                     508 STORE_SUBSCR
+         
+         207         512 LOAD_GLOBAL              1 (NULL + print)
+                     524 LOAD_FAST                5 (update_event)
+                     526 PRECALL                  1
+                     530 CALL                     1
+                     540 POP_TOP
          
-         205         520 LOAD_FAST                3 (resp)
-                     522 RETURN_VALUE
+         208         542 LOAD_GLOBAL              2 (ts)
+                     554 LOAD_ATTR               17 (query)
+                     564 LOAD_METHOD             18 (insert_event)
+                     586 LOAD_FAST                5 (update_event)
+                     588 PRECALL                  1
+                     592 CALL                     1
+                     602 POP_TOP
+         
+         209         604 LOAD_FAST                4 (resp)
+                     606 RETURN_VALUE
+         ExceptionTable:
+           34 to 104 -> 108 [0]
+           108 to 126 -> 182 [1] lasti
+           128 to 160 -> 172 [1] lasti
+           172 to 180 -> 182 [1] lasti
          consts
             None
             'enriching with gpt...'
+            '<could not fetch homepage>'
             'system'
             'You will help us evaluate '
             ' for acquisition.'
             ('role', 'content')
             'You will consider this existing information: '
             'You will consider this copy from the company homepage as the most up to date. homepage_text: '
             'You will respond with only the JSON object.'
             'user'
             'gpt'
-         names      ('print', 'ts', 'helpers', 'get_homepage_text', 'domain', 'name', 'asdict', 'gpt', 'HOW_TO_ENRICH', 'ask_gpt4', 'from_dict', 'models', 'Event', 'int', 'time', 'data', 'query', 'insert_event')
-         varnames   ('company', 'homepage_text', 'messages', 'resp', 'update_event')
+         names      ('print', 'ts', 'helpers', 'get_homepage_text', 'domain', 'Exception', 'name', 'asdict', 'gpt', 'HOW_TO_ENRICH', 'ask_gpt4', 'from_dict', 'models', 'Event', 'int', 'time', 'data', 'query', 'insert_event')
+         varnames   ('company', 'homepage_text', 'e', 'messages', 'resp', 'update_event')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'enrich_with_gpt'
          firstlineno 174
          lnotab
-            0x02011e014803020114fe0405020122fe0405020108fe0405020102fe04
-            05020120fe04ef04173e013e0146011e013e01
+            0x02011e0102014c0112011e0116fe0805020114fe0405020122fe040502
+            0108fe0405020102fe0405020120fe04ef04173e013e0146011e013e01
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 3
          flags     : 3
          code
             0x97007c006a0000000000000000007d017c006a0100000000000000007d
@@ -1292,109 +1333,109 @@
             0500000000000000007404000000000000000000006a0300000000000000
             00a00c00000000000000000000000000000000000000007c03a6010000ab
             01000000000000000001007c036a050000000000000000a0060000000000
             0000000000000000000000000000006405a6010000ab0100000000000000
             007211740f000000000000000000006406a6010000ab0100000000000000
             00010064005300741b000000000000000000007c03ac07a6010000ab0100
             00000000000000010064005300
-         208           0 RESUME                   0
+         212           0 RESUME                   0
          
-         209           2 LOAD_FAST                0 (event)
+         213           2 LOAD_FAST                0 (event)
                        4 LOAD_ATTR                0 (domain)
                       14 STORE_FAST               1 (domain)
          
-         210          16 LOAD_FAST                0 (event)
+         214          16 LOAD_FAST                0 (event)
                       18 LOAD_ATTR                1 (search_uid)
                       28 STORE_FAST               2 (search_uid)
          
-         212          30 LOAD_GLOBAL              4 (ts)
+         216          30 LOAD_GLOBAL              4 (ts)
                       42 LOAD_ATTR                3 (query)
                       52 LOAD_METHOD              4 (find_company_by_domain)
                       74 LOAD_FAST                1 (domain)
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               3 (company)
          
-         213          92 LOAD_FAST                3 (company)
+         217          92 LOAD_FAST                3 (company)
                       94 LOAD_ATTR                5 (meta)
                      104 LOAD_METHOD              6 (get)
                      126 LOAD_CONST               1 ('company_uid')
                      128 PRECALL                  1
                      132 CALL                     1
                      142 POP_JUMP_FORWARD_IF_FALSE    16 (to 176)
          
-         214         144 LOAD_GLOBAL             15 (NULL + print)
+         218         144 LOAD_GLOBAL             15 (NULL + print)
                      156 LOAD_CONST               2 ('company already exists. skipping enrichment...')
                      158 PRECALL                  1
                      162 CALL                     1
                      172 POP_TOP
                      174 JUMP_FORWARD           142 (to 460)
          
-         216     >>  176 LOAD_GLOBAL              4 (ts)
+         220     >>  176 LOAD_GLOBAL              4 (ts)
                      188 LOAD_ATTR                8 (grata)
                      198 LOAD_METHOD              9 (enrich)
                      220 LOAD_FAST                3 (company)
                      222 LOAD_ATTR                0 (domain)
                      232 PRECALL                  1
                      236 CALL                     1
                      246 STORE_FAST               4 (resp)
          
-         217         248 LOAD_FAST                3 (company)
+         221         248 LOAD_FAST                3 (company)
                      250 LOAD_ATTR               10 (name)
                      260 JUMP_IF_TRUE_OR_POP     20 (to 302)
                      262 LOAD_FAST                4 (resp)
                      264 LOAD_METHOD              6 (get)
                      286 LOAD_CONST               3 ('name')
                      288 PRECALL                  1
                      292 CALL                     1
                  >>  302 LOAD_FAST                3 (company)
                      304 STORE_ATTR              10 (name)
          
-         218         314 LOAD_FAST                4 (resp)
+         222         314 LOAD_FAST                4 (resp)
                      316 LOAD_METHOD              6 (get)
                      338 LOAD_CONST               4 ('description')
                      340 PRECALL                  1
                      344 CALL                     1
                      354 LOAD_FAST                3 (company)
                      356 STORE_ATTR              11 (description)
          
-         219         366 BUILD_MAP                0
+         223         366 BUILD_MAP                0
                      368 LOAD_FAST                3 (company)
                      370 LOAD_ATTR                5 (meta)
                      380 DICT_UPDATE              1
                      382 LOAD_FAST                4 (resp)
                      384 DICT_UPDATE              1
                      386 LOAD_FAST                3 (company)
                      388 STORE_ATTR               5 (meta)
          
-         220         398 LOAD_GLOBAL              4 (ts)
+         224         398 LOAD_GLOBAL              4 (ts)
                      410 LOAD_ATTR                3 (query)
                      420 LOAD_METHOD             12 (update_company)
                      442 LOAD_FAST                3 (company)
                      444 PRECALL                  1
                      448 CALL                     1
                      458 POP_TOP
          
-         222     >>  460 LOAD_FAST                3 (company)
+         226     >>  460 LOAD_FAST                3 (company)
                      462 LOAD_ATTR                5 (meta)
                      472 LOAD_METHOD              6 (get)
                      494 LOAD_CONST               5 ('gpt')
                      496 PRECALL                  1
                      500 CALL                     1
                      510 POP_JUMP_FORWARD_IF_FALSE    17 (to 546)
          
-         223         512 LOAD_GLOBAL             15 (NULL + print)
+         227         512 LOAD_GLOBAL             15 (NULL + print)
                      524 LOAD_CONST               6 ('company already enriched with gpt. skipping...')
                      526 PRECALL                  1
                      530 CALL                     1
                      540 POP_TOP
                      542 LOAD_CONST               0 (None)
                      544 RETURN_VALUE
          
-         225     >>  546 LOAD_GLOBAL             27 (NULL + enrich_with_gpt)
+         229     >>  546 LOAD_GLOBAL             27 (NULL + enrich_with_gpt)
                      558 LOAD_FAST                3 (company)
                      560 KW_NAMES                 7
                      562 PRECALL                  1
                      566 CALL                     1
                      576 POP_TOP
                      578 LOAD_CONST               0 (None)
                      580 RETURN_VALUE
@@ -1409,15 +1450,15 @@
             ('company',)
          names      ('domain', 'search_uid', 'ts', 'query', 'find_company_by_domain', 'meta', 'get', 'print', 'grata', 'enrich', 'name', 'description', 'update_company', 'enrich_with_gpt')
          varnames   ('event', 'domain', 'search_uid', 'company', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_enrichment'
-         firstlineno 208
+         firstlineno 212
          lnotab 0x02010e010e023e013401200248014201340120013e0234012202
       'event_id'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 9
          flags     : 3
@@ -1507,593 +1548,593 @@
             0000000000000001007402000000000000000000006a0200000000000000
             00a014000000000000000000000000000000000000000074020000000000
             00000000006a150000000000000000a01600000000000000000000000000
             000000000000007c026a1300000000000000007c037c016a0d0000000000
             000000642a190000000000000000007c016a170000000000000000ac2ba6
             040000ab040000000000000000a6010000ab01000000000000000001008c
             686400530064005300
-         228           0 RESUME                   0
+         232           0 RESUME                   0
          
-         229           2 LOAD_GLOBAL              1 (NULL + print)
+         233           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('processing event...')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-         230          32 LOAD_GLOBAL              2 (ts)
+         234          32 LOAD_GLOBAL              2 (ts)
                       44 LOAD_ATTR                2 (query)
                       54 LOAD_METHOD              3 (find_event_by_id)
                       76 LOAD_FAST                0 (event_id)
                       78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               1 (event)
          
-         231          94 LOAD_GLOBAL              1 (NULL + print)
+         235          94 LOAD_GLOBAL              1 (NULL + print)
                      106 LOAD_CONST               2 ('event_id')
                      108 LOAD_FAST                0 (event_id)
                      110 PRECALL                  2
                      114 CALL                     2
                      124 POP_TOP
          
-         232         126 LOAD_GLOBAL              1 (NULL + print)
+         236         126 LOAD_GLOBAL              1 (NULL + print)
                      138 LOAD_FAST                1 (event)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 POP_TOP
          
-         233         156 LOAD_GLOBAL              2 (ts)
+         237         156 LOAD_GLOBAL              2 (ts)
                      168 LOAD_ATTR                2 (query)
                      178 LOAD_METHOD              4 (find_search)
                      200 LOAD_FAST                1 (event)
                      202 LOAD_ATTR                5 (search_uid)
                      212 KW_NAMES                 3
                      214 PRECALL                  1
                      218 CALL                     1
                      228 STORE_FAST               2 (search)
          
-         234         230 LOAD_FAST                1 (event)
+         238         230 LOAD_FAST                1 (event)
                      232 LOAD_ATTR                6 (domain)
                      242 STORE_FAST               3 (domain)
          
-         235         244 LOAD_FAST                1 (event)
+         239         244 LOAD_FAST                1 (event)
                      246 LOAD_ATTR                7 (type)
                      256 LOAD_CONST               4 ('land')
                      258 COMPARE_OP               2 (==)
                      264 POP_JUMP_FORWARD_IF_FALSE    18 (to 302)
          
-         236         266 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         240         266 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      278 LOAD_FAST                1 (event)
                      280 KW_NAMES                 5
                      282 PRECALL                  1
                      286 CALL                     1
                      296 POP_TOP
                      298 LOAD_CONST               0 (None)
                      300 RETURN_VALUE
          
-         237     >>  302 LOAD_FAST                1 (event)
+         241     >>  302 LOAD_FAST                1 (event)
                      304 LOAD_ATTR                7 (type)
                      314 LOAD_CONST               6 ('create')
                      316 COMPARE_OP               2 (==)
                      322 POP_JUMP_FORWARD_IF_FALSE    18 (to 360)
          
-         238         324 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         242         324 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      336 LOAD_FAST                1 (event)
                      338 KW_NAMES                 5
                      340 PRECALL                  1
                      344 CALL                     1
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
          
-         239     >>  360 LOAD_FAST                1 (event)
+         243     >>  360 LOAD_FAST                1 (event)
                      362 LOAD_ATTR                7 (type)
                      372 LOAD_CONST               7 ('advance')
                      374 COMPARE_OP               2 (==)
                      380 POP_JUMP_FORWARD_IF_FALSE    18 (to 418)
          
-         240         382 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         244         382 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      394 LOAD_FAST                1 (event)
                      396 KW_NAMES                 5
                      398 PRECALL                  1
                      402 CALL                     1
                      412 POP_TOP
                      414 LOAD_CONST               0 (None)
                      416 RETURN_VALUE
          
-         241     >>  418 LOAD_FAST                1 (event)
+         245     >>  418 LOAD_FAST                1 (event)
                      420 LOAD_ATTR                7 (type)
                      430 LOAD_CONST               8 ('validate')
                      432 COMPARE_OP               2 (==)
                      438 POP_JUMP_FORWARD_IF_FALSE    51 (to 542)
          
-         242         440 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         246         440 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      452 LOAD_FAST                1 (event)
                      454 KW_NAMES                 5
                      456 PRECALL                  1
                      460 CALL                     1
                      470 POP_TOP
          
-         243         472 LOAD_GLOBAL             19 (NULL + run_acquired_check)
+         247         472 LOAD_GLOBAL             19 (NULL + run_acquired_check)
                      484 LOAD_FAST                3 (domain)
                      486 KW_NAMES                 9
                      488 PRECALL                  1
                      492 CALL                     1
                      502 POP_TOP
          
-         244         504 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         248         504 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      516 LOAD_FAST                2 (search)
                      518 LOAD_FAST                3 (domain)
                      520 KW_NAMES                10
                      522 PRECALL                  2
                      526 CALL                     2
                      536 POP_TOP
                      538 LOAD_CONST               0 (None)
                      540 RETURN_VALUE
          
-         245     >>  542 LOAD_FAST                1 (event)
+         249     >>  542 LOAD_FAST                1 (event)
                      544 LOAD_ATTR                7 (type)
                      554 LOAD_CONST              11 ('send')
                      556 COMPARE_OP               2 (==)
                      562 POP_JUMP_FORWARD_IF_FALSE    18 (to 600)
          
-         246         564 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         250         564 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      576 LOAD_FAST                1 (event)
                      578 KW_NAMES                 5
                      580 PRECALL                  1
                      584 CALL                     1
                      594 POP_TOP
                      596 LOAD_CONST               0 (None)
                      598 RETURN_VALUE
          
-         247     >>  600 LOAD_FAST                1 (event)
+         251     >>  600 LOAD_FAST                1 (event)
                      602 LOAD_ATTR                7 (type)
                      612 LOAD_CONST              12 ('client_approve')
                      614 COMPARE_OP               2 (==)
                      620 POP_JUMP_FORWARD_IF_FALSE    35 (to 692)
          
-         248         622 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         252         622 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      634 LOAD_FAST                1 (event)
                      636 KW_NAMES                 5
                      638 PRECALL                  1
                      642 CALL                     1
                      652 POP_TOP
          
-         249         654 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         253         654 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      666 LOAD_FAST                2 (search)
                      668 LOAD_FAST                3 (domain)
                      670 KW_NAMES                10
                      672 PRECALL                  2
                      676 CALL                     2
                      686 POP_TOP
                      688 LOAD_CONST               0 (None)
                      690 RETURN_VALUE
          
-         250     >>  692 LOAD_FAST                1 (event)
+         254     >>  692 LOAD_FAST                1 (event)
                      694 LOAD_ATTR                7 (type)
                      704 LOAD_CONST              13 ('reject')
                      706 COMPARE_OP               2 (==)
                      712 POP_JUMP_FORWARD_IF_FALSE     2 (to 718)
          
-         251         714 LOAD_CONST               0 (None)
+         255         714 LOAD_CONST               0 (None)
                      716 RETURN_VALUE
          
-         252     >>  718 LOAD_FAST                1 (event)
+         256     >>  718 LOAD_FAST                1 (event)
                      720 LOAD_ATTR                7 (type)
                      730 LOAD_CONST              14 ('client_reject')
                      732 COMPARE_OP               2 (==)
                      738 POP_JUMP_FORWARD_IF_FALSE     2 (to 744)
          
-         253         740 LOAD_CONST               0 (None)
+         257         740 LOAD_CONST               0 (None)
                      742 RETURN_VALUE
          
-         254     >>  744 LOAD_FAST                1 (event)
+         258     >>  744 LOAD_FAST                1 (event)
                      746 LOAD_ATTR                7 (type)
                      756 LOAD_CONST              15 ('conflict')
                      758 COMPARE_OP               2 (==)
                      764 POP_JUMP_FORWARD_IF_FALSE    35 (to 836)
          
-         255         766 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         259         766 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      778 LOAD_FAST                1 (event)
                      780 KW_NAMES                 5
                      782 PRECALL                  1
                      786 CALL                     1
                      796 POP_TOP
          
-         256         798 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         260         798 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      810 LOAD_FAST                2 (search)
                      812 LOAD_FAST                3 (domain)
                      814 KW_NAMES                10
                      816 PRECALL                  2
                      820 CALL                     2
                      830 POP_TOP
                      832 LOAD_CONST               0 (None)
                      834 RETURN_VALUE
          
-         257     >>  836 LOAD_FAST                1 (event)
+         261     >>  836 LOAD_FAST                1 (event)
                      838 LOAD_ATTR                7 (type)
                      848 LOAD_CONST              16 ('client_conflict')
                      850 COMPARE_OP               2 (==)
                      856 POP_JUMP_FORWARD_IF_FALSE     2 (to 862)
          
-         258         858 LOAD_CONST               0 (None)
+         262         858 LOAD_CONST               0 (None)
                      860 RETURN_VALUE
          
-         261     >>  862 LOAD_FAST                1 (event)
+         265     >>  862 LOAD_FAST                1 (event)
                      864 LOAD_ATTR                7 (type)
                      874 LOAD_CONST              17 ('prompt')
                      876 COMPARE_OP               2 (==)
                      882 POP_JUMP_FORWARD_IF_FALSE    18 (to 920)
          
-         262         884 LOAD_GLOBAL             23 (NULL + handle_prompt)
+         266         884 LOAD_GLOBAL             23 (NULL + handle_prompt)
                      896 LOAD_FAST                1 (event)
                      898 KW_NAMES                 5
                      900 PRECALL                  1
                      904 CALL                     1
                      914 POP_TOP
                      916 LOAD_CONST               0 (None)
                      918 RETURN_VALUE
          
-         263     >>  920 LOAD_FAST                1 (event)
+         267     >>  920 LOAD_FAST                1 (event)
                      922 LOAD_ATTR                7 (type)
                      932 LOAD_CONST              18 ('criteria')
                      934 COMPARE_OP               2 (==)
                      940 POP_JUMP_FORWARD_IF_FALSE    56 (to 1054)
          
-         264         942 LOAD_GLOBAL             25 (NULL + len)
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
          
-         265        1014 LOAD_GLOBAL             29 (NULL + run_criteria_search)
+         269        1014 LOAD_GLOBAL             29 (NULL + run_criteria_search)
                     1026 LOAD_FAST                2 (search)
                     1028 KW_NAMES                22
                     1030 PRECALL                  1
                     1034 CALL                     1
                     1044 POP_TOP
                     1046 LOAD_CONST               0 (None)
                     1048 RETURN_VALUE
          
-         264     >> 1050 LOAD_CONST               0 (None)
+         268     >> 1050 LOAD_CONST               0 (None)
                     1052 RETURN_VALUE
          
-         266     >> 1054 LOAD_FAST                1 (event)
+         270     >> 1054 LOAD_FAST                1 (event)
                     1056 LOAD_ATTR                7 (type)
                     1066 LOAD_CONST              23 ('maps')
                     1068 COMPARE_OP               2 (==)
                     1074 POP_JUMP_FORWARD_IF_FALSE    19 (to 1114)
          
-         267        1076 LOAD_GLOBAL             31 (NULL + run_maps_search)
+         271        1076 LOAD_GLOBAL             31 (NULL + run_maps_search)
                     1088 LOAD_FAST                2 (search)
                     1090 LOAD_FAST                1 (event)
                     1092 KW_NAMES                24
                     1094 PRECALL                  2
                     1098 CALL                     2
                     1108 POP_TOP
                     1110 LOAD_CONST               0 (None)
                     1112 RETURN_VALUE
          
-         268     >> 1114 LOAD_FAST                1 (event)
+         272     >> 1114 LOAD_FAST                1 (event)
                     1116 LOAD_ATTR                7 (type)
                     1126 LOAD_CONST              25 ('google')
                     1128 COMPARE_OP               2 (==)
                     1134 POP_JUMP_FORWARD_IF_FALSE    19 (to 1174)
          
-         269        1136 LOAD_GLOBAL             33 (NULL + run_google_search)
+         273        1136 LOAD_GLOBAL             33 (NULL + run_google_search)
                     1148 LOAD_FAST                2 (search)
                     1150 LOAD_FAST                1 (event)
                     1152 KW_NAMES                24
                     1154 PRECALL                  2
                     1158 CALL                     2
                     1168 POP_TOP
                     1170 LOAD_CONST               0 (None)
                     1172 RETURN_VALUE
          
-         271     >> 1174 LOAD_FAST                1 (event)
+         275     >> 1174 LOAD_FAST                1 (event)
                     1176 LOAD_ATTR                7 (type)
                     1186 LOAD_CONST              26 ('import')
                     1188 COMPARE_OP               2 (==)
                     1194 POP_JUMP_FORWARD_IF_FALSE    34 (to 1264)
          
-         272        1196 LOAD_GLOBAL              2 (ts)
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
          
-         274     >> 1264 LOAD_FAST                1 (event)
+         278     >> 1264 LOAD_FAST                1 (event)
                     1266 LOAD_ATTR                7 (type)
                     1276 LOAD_CONST              27 ('reset')
                     1278 COMPARE_OP               2 (==)
                     1284 POP_JUMP_FORWARD_IF_FALSE    54 (to 1394)
          
-         275        1286 LOAD_GLOBAL              1 (NULL + print)
+         279        1286 LOAD_GLOBAL              1 (NULL + print)
                     1298 LOAD_CONST              28 ('💣 Resetting Inbox...')
                     1300 PRECALL                  1
                     1304 CALL                     1
                     1314 POP_TOP
          
-         276        1316 LOAD_GLOBAL              2 (ts)
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
          
-         278     >> 1394 LOAD_FAST                1 (event)
+         282     >> 1394 LOAD_FAST                1 (event)
                     1396 LOAD_ATTR                7 (type)
                     1406 LOAD_CONST              30 ('rating')
                     1408 COMPARE_OP               2 (==)
                     1414 EXTENDED_ARG             1
                     1416 POP_JUMP_FORWARD_IF_FALSE   287 (to 1992)
          
-         280        1418 LOAD_GLOBAL              1 (NULL + print)
+         284        1418 LOAD_GLOBAL              1 (NULL + print)
                     1430 LOAD_FAST                1 (event)
                     1432 PRECALL                  1
                     1436 CALL                     1
                     1446 POP_TOP
          
-         281        1448 LOAD_FAST                1 (event)
+         285        1448 LOAD_FAST                1 (event)
                     1450 LOAD_ATTR               13 (data)
                     1460 LOAD_CONST              30 ('rating')
                     1462 BINARY_SUBSCR
                     1472 STORE_FAST               4 (rating)
          
-         282        1474 LOAD_FAST                1 (event)
+         286        1474 LOAD_FAST                1 (event)
                     1476 LOAD_ATTR               13 (data)
                     1486 LOAD_CONST              31 ('currentView')
                     1488 BINARY_SUBSCR
                     1498 STORE_FAST               5 (from_stage)
          
-         283        1500 LOAD_FAST                4 (rating)
+         287        1500 LOAD_FAST                4 (rating)
                     1502 LOAD_CONST              32 (1)
                     1504 COMPARE_OP               2 (==)
                     1510 POP_JUMP_FORWARD_IF_FALSE    76 (to 1664)
          
-         284        1512 LOAD_GLOBAL              2 (ts)
+         288        1512 LOAD_GLOBAL              2 (ts)
                     1524 LOAD_ATTR                2 (query)
                     1534 LOAD_METHOD             20 (insert_event)
          
-         285        1556 LOAD_GLOBAL              2 (ts)
+         289        1556 LOAD_GLOBAL              2 (ts)
                     1568 LOAD_ATTR               21 (models)
                     1578 LOAD_METHOD             22 (Event)
          
-         286        1600 LOAD_FAST                2 (search)
+         290        1600 LOAD_FAST                2 (search)
                     1602 LOAD_ATTR               19 (uid)
          
-         287        1612 LOAD_CONST              13 ('reject')
+         291        1612 LOAD_CONST              13 ('reject')
          
-         288        1614 LOAD_FAST                3 (domain)
+         292        1614 LOAD_FAST                3 (domain)
          
-         289        1616 LOAD_FAST                1 (event)
+         293        1616 LOAD_FAST                1 (event)
                     1618 LOAD_ATTR               23 (actor_key)
          
-         285        1628 KW_NAMES                33
+         289        1628 KW_NAMES                33
                     1630 PRECALL                  4
                     1634 CALL                     4
          
-         284        1644 PRECALL                  1
+         288        1644 PRECALL                  1
                     1648 CALL                     1
                     1658 POP_TOP
                     1660 LOAD_CONST               0 (None)
                     1662 RETURN_VALUE
          
-         292     >> 1664 LOAD_FAST                4 (rating)
+         296     >> 1664 LOAD_FAST                4 (rating)
                     1666 LOAD_CONST              34 (2)
                     1668 COMPARE_OP               2 (==)
                     1674 POP_JUMP_FORWARD_IF_FALSE    76 (to 1828)
          
-         293        1676 LOAD_GLOBAL              2 (ts)
+         297        1676 LOAD_GLOBAL              2 (ts)
                     1688 LOAD_ATTR                2 (query)
                     1698 LOAD_METHOD             20 (insert_event)
          
-         294        1720 LOAD_GLOBAL              2 (ts)
+         298        1720 LOAD_GLOBAL              2 (ts)
                     1732 LOAD_ATTR               21 (models)
                     1742 LOAD_METHOD             22 (Event)
          
-         295        1764 LOAD_FAST                2 (search)
+         299        1764 LOAD_FAST                2 (search)
                     1766 LOAD_ATTR               19 (uid)
          
-         296        1776 LOAD_CONST              35 ('hold')
+         300        1776 LOAD_CONST              35 ('hold')
          
-         297        1778 LOAD_FAST                3 (domain)
+         301        1778 LOAD_FAST                3 (domain)
          
-         298        1780 LOAD_FAST                1 (event)
+         302        1780 LOAD_FAST                1 (event)
                     1782 LOAD_ATTR               23 (actor_key)
          
-         294        1792 KW_NAMES                33
+         298        1792 KW_NAMES                33
                     1794 PRECALL                  4
                     1798 CALL                     4
          
-         293        1808 PRECALL                  1
+         297        1808 PRECALL                  1
                     1812 CALL                     1
                     1822 POP_TOP
                     1824 LOAD_CONST               0 (None)
                     1826 RETURN_VALUE
          
-         301     >> 1828 LOAD_FAST                5 (from_stage)
+         305     >> 1828 LOAD_FAST                5 (from_stage)
                     1830 LOAD_CONST              36 (('land', 'create', 'advance', 'hold'))
                     1832 CONTAINS_OP              0
                     1834 POP_JUMP_FORWARD_IF_FALSE    76 (to 1988)
          
-         302        1836 LOAD_GLOBAL              2 (ts)
+         306        1836 LOAD_GLOBAL              2 (ts)
                     1848 LOAD_ATTR                2 (query)
                     1858 LOAD_METHOD             20 (insert_event)
          
-         303        1880 LOAD_GLOBAL              2 (ts)
+         307        1880 LOAD_GLOBAL              2 (ts)
                     1892 LOAD_ATTR               21 (models)
                     1902 LOAD_METHOD             22 (Event)
          
-         304        1924 LOAD_FAST                2 (search)
+         308        1924 LOAD_FAST                2 (search)
                     1926 LOAD_ATTR               19 (uid)
          
-         305        1936 LOAD_CONST               8 ('validate')
+         309        1936 LOAD_CONST               8 ('validate')
          
-         306        1938 LOAD_FAST                3 (domain)
+         310        1938 LOAD_FAST                3 (domain)
          
-         307        1940 LOAD_FAST                1 (event)
+         311        1940 LOAD_FAST                1 (event)
                     1942 LOAD_ATTR               23 (actor_key)
          
-         303        1952 KW_NAMES                33
+         307        1952 KW_NAMES                33
                     1954 PRECALL                  4
                     1958 CALL                     4
          
-         302        1968 PRECALL                  1
+         306        1968 PRECALL                  1
                     1972 CALL                     1
                     1982 POP_TOP
                     1984 LOAD_CONST               0 (None)
                     1986 RETURN_VALUE
          
-         301     >> 1988 LOAD_CONST               0 (None)
+         305     >> 1988 LOAD_CONST               0 (None)
                     1990 RETURN_VALUE
          
-         311     >> 1992 LOAD_FAST                1 (event)
+         315     >> 1992 LOAD_FAST                1 (event)
                     1994 LOAD_ATTR                7 (type)
                     2004 LOAD_CONST              37 ('update')
                     2006 COMPARE_OP               2 (==)
                     2012 POP_JUMP_FORWARD_IF_FALSE   185 (to 2384)
          
-         312        2014 LOAD_FAST                3 (domain)
+         316        2014 LOAD_FAST                3 (domain)
                     2016 POP_JUMP_FORWARD_IF_FALSE   129 (to 2276)
          
-         313        2018 LOAD_GLOBAL              2 (ts)
+         317        2018 LOAD_GLOBAL              2 (ts)
                     2030 LOAD_ATTR                2 (query)
                     2040 LOAD_METHOD             24 (find_company_by_domain)
                     2062 LOAD_FAST                3 (domain)
                     2064 PRECALL                  1
                     2068 CALL                     1
                     2078 STORE_FAST               6 (company)
          
-         314        2080 LOAD_FAST                1 (event)
+         318        2080 LOAD_FAST                1 (event)
                     2082 LOAD_ATTR               13 (data)
                     2092 LOAD_METHOD             25 (get)
                     2114 LOAD_CONST              38 ('name')
                     2116 PRECALL                  1
                     2120 CALL                     1
                     2130 POP_JUMP_FORWARD_IF_FALSE    18 (to 2168)
          
-         315        2132 LOAD_FAST                1 (event)
+         319        2132 LOAD_FAST                1 (event)
                     2134 LOAD_ATTR               13 (data)
                     2144 LOAD_CONST              38 ('name')
                     2146 BINARY_SUBSCR
                     2156 LOAD_FAST                6 (company)
                     2158 STORE_ATTR              26 (name)
          
-         321     >> 2168 BUILD_MAP                0
+         325     >> 2168 BUILD_MAP                0
                     2170 LOAD_FAST                6 (company)
                     2172 LOAD_ATTR               27 (meta)
                     2182 DICT_UPDATE              1
                     2184 LOAD_FAST                1 (event)
                     2186 LOAD_ATTR               13 (data)
                     2196 DICT_UPDATE              1
                     2198 LOAD_FAST                6 (company)
                     2200 STORE_ATTR              27 (meta)
          
-         322        2210 LOAD_GLOBAL              2 (ts)
+         326        2210 LOAD_GLOBAL              2 (ts)
                     2222 LOAD_ATTR                2 (query)
                     2232 LOAD_METHOD             28 (update_company)
                     2254 LOAD_FAST                6 (company)
                     2256 PRECALL                  1
                     2260 CALL                     1
                     2270 POP_TOP
                     2272 LOAD_CONST               0 (None)
                     2274 RETURN_VALUE
          
-         324     >> 2276 BUILD_MAP                0
+         328     >> 2276 BUILD_MAP                0
                     2278 LOAD_FAST                2 (search)
                     2280 LOAD_ATTR               27 (meta)
                     2290 DICT_UPDATE              1
                     2292 LOAD_FAST                1 (event)
                     2294 LOAD_ATTR               13 (data)
                     2304 DICT_UPDATE              1
                     2306 LOAD_FAST                2 (search)
                     2308 STORE_ATTR              27 (meta)
          
-         325        2318 LOAD_GLOBAL              2 (ts)
+         329        2318 LOAD_GLOBAL              2 (ts)
                     2330 LOAD_ATTR                2 (query)
                     2340 LOAD_METHOD             29 (update_search)
                     2362 LOAD_FAST                2 (search)
                     2364 PRECALL                  1
                     2368 CALL                     1
                     2378 POP_TOP
                     2380 LOAD_CONST               0 (None)
                     2382 RETURN_VALUE
          
-         327     >> 2384 LOAD_FAST                1 (event)
+         331     >> 2384 LOAD_FAST                1 (event)
                     2386 LOAD_ATTR                7 (type)
                     2396 LOAD_CONST              39 ('move')
                     2398 COMPARE_OP               2 (==)
                     2404 POP_JUMP_FORWARD_IF_FALSE   117 (to 2640)
          
-         329        2406 LOAD_FAST                1 (event)
+         333        2406 LOAD_FAST                1 (event)
                     2408 LOAD_ATTR               13 (data)
                     2418 LOAD_CONST              40 ('domains')
                     2420 BINARY_SUBSCR
                     2430 GET_ITER
                  >> 2432 FOR_ITER               105 (to 2644)
                     2434 STORE_FAST               3 (domain)
          
-         330        2436 LOAD_GLOBAL              1 (NULL + print)
+         334        2436 LOAD_GLOBAL              1 (NULL + print)
                     2448 LOAD_CONST              41 ('moving domain:')
                     2450 LOAD_FAST                3 (domain)
                     2452 PRECALL                  2
                     2456 CALL                     2
                     2466 POP_TOP
          
-         331        2468 LOAD_GLOBAL              2 (ts)
+         335        2468 LOAD_GLOBAL              2 (ts)
                     2480 LOAD_ATTR                2 (query)
                     2490 LOAD_METHOD             20 (insert_event)
          
-         332        2512 LOAD_GLOBAL              2 (ts)
+         336        2512 LOAD_GLOBAL              2 (ts)
                     2524 LOAD_ATTR               21 (models)
                     2534 LOAD_METHOD             22 (Event)
          
-         333        2556 LOAD_FAST                2 (search)
+         337        2556 LOAD_FAST                2 (search)
                     2558 LOAD_ATTR               19 (uid)
          
-         334        2568 LOAD_FAST                3 (domain)
+         338        2568 LOAD_FAST                3 (domain)
          
-         335        2570 LOAD_FAST                1 (event)
+         339        2570 LOAD_FAST                1 (event)
                     2572 LOAD_ATTR               13 (data)
                     2582 LOAD_CONST              42 ('stage')
                     2584 BINARY_SUBSCR
          
-         336        2594 LOAD_FAST                1 (event)
+         340        2594 LOAD_FAST                1 (event)
                     2596 LOAD_ATTR               23 (actor_key)
          
-         332        2606 KW_NAMES                43
+         336        2606 KW_NAMES                43
                     2608 PRECALL                  4
                     2612 CALL                     4
          
-         331        2622 PRECALL                  1
+         335        2622 PRECALL                  1
                     2626 CALL                     1
                     2636 POP_TOP
                     2638 JUMP_BACKWARD          104 (to 2432)
          
-         327     >> 2640 LOAD_CONST               0 (None)
+         331     >> 2640 LOAD_CONST               0 (None)
                     2642 RETURN_VALUE
          
-         329     >> 2644 LOAD_CONST               0 (None)
+         333     >> 2644 LOAD_CONST               0 (None)
                     2646 RETURN_VALUE
          consts
             None
             'processing event...'
             'event_id'
             ('uid',)
             'land'
@@ -2138,15 +2179,15 @@
             ('search_uid', 'domain', 'type', 'actor_key')
          names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'len', 'data', 'run_criteria_search', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'reset_inbox', 'uid', 'insert_event', 'models', 'Event', 'actor_key', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
          varnames   ('event_id', 'event', 'search', 'domain', 'rating', 'from_stage', 'company')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_event'
-         firstlineno 228
+         firstlineno 232
          lnotab
             0x02011e013e0120011e014a010e01160124011601240116012401160120
             012001260116012401160120012601160104011601040116012001260116
             010403160124011601480124ff040216012601160126021601440216011e
             014e0218021e011a011a010c012c012c010c01020102010cfc10ff14080c
             012c012c010c01020102010cfc10ff140808012c012c010c01020102010c
             fc10ff14ff040a160104013e01340124062a0142022a01420216021e0120
@@ -2154,8 +2195,8 @@
    names      ('dataclasses', 'asdict', 'time', 'gandai', 'ts', 'dacite', 'from_dict', 'str', 'run_acquired_check', 'models', 'Search', 'run_similarity_search', 'run_criteria_search', 'Event', 'run_maps_search', 'run_google_search', 'handle_prompt', 'Company', 'enrich_with_gpt', 'run_enrichment', 'int', 'process_event')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c0208010c030c26280b240d3c2d3c0f242c24222414
+   lnotab 0x00ff02010c010c0208010c030c26280b240d3c2d3c0f242c24262414
```

### Comparing `gandai-1.7.45/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xeed64f66 (Thu May 23 23:53:18 2024 UTC)
-files sz: 28680
+moddate:  0x110f5066 (Fri May 24 03:52:49 2024 UTC)
+files sz: 28700
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -922,41 +922,43 @@
             0000006403a6010000ab0100000000000000006404190000000000000000
             00a0050000000000000000000000000000000000000000a6000000ab0000
             000000000000008a0c880c6601640584087d037c006a0000000000000000
             006406190000000000000000007d0467007d05740c000000000000000000
             00a0070000000000000000000000000000000000000000a6000000ab0000
             0000000000000035007d067c06a008000000000000000000000000000000
             0000000000a6000000ab000000000000000000350001007c04440090015d
-            3b7d077412000000000000000000006a0a0000000000000000a00b000000
+            677d077412000000000000000000006a0a0000000000000000a00b000000
             00000000000000000000000000000000007c07a6010000ab010000000000
             0000007d077c06a00c000000000000000000000000000000000000000074
             1b000000000000000000006a0e00000000000000006407a6010000ab0100
             000000000000007c077c0164089c02a6020000ab02000000000000000001
             007c06a00c0000000000000000000000000000000000000000741b000000
             000000000000006a0e00000000000000006409a6010000ab010000000000
             0000007c006a0300000000000000007c006a0f00000000000000007c077c
             006a000000000000000000a0010000000000000000000000000000000000
             0000006404640aa6020000ab020000000000000000640b9c04a6020000ab
             0200000000000000007d087c08a010000000000000000000000000000000
             0000000000a6000000ab0000000000000000007d097c0981157c05a01100
             000000000000000000000000000000000000007c09a6010000ab01000000
             00000000000100890ca00100000000000000000000000000000000000000
-            007c07a6010000ab010000000000000000815e7412000000000000000000
+            007c07a6010000ab010000000000000000818a7412000000000000000000
             006a120000000000000000a0130000000000000000000000000000000000
             0000007c006a0300000000000000007c006a0f00000000000000007c0764
-            0c640c640d7c079b00640e02007c037c07a6010000ab0100000000000000
-            009b009d046901ac0fa6050000ab0500000000000000007d0a7412000000
-            000000000000006a140000000000000000a0150000000000000000000000
-            0000000000000000007c0aa6010000ab010000000000000000010090018c
-            3d0900640064006400a6020000ab02000000000000000001006e0b230031
-            00730477027803590077010100590001000100640064006400a6020000ab
-            02000000000000000001006e0b2300310073047702780359007701010059
-            00010001007c0544005d177d0b7413000000000000000000006a16000000
-            00000000007c0bac10a6010000ab01000000000000000001008c18640053
-            00
+            0c640c02007c037c07a6010000ab0100000000000000009b00640d741200
+            0000000000000000006a1400000000000000006a1500000000000000007c
+            006a000000000000000000a0010000000000000000000000000000000000
+            0000006404a6010000ab010000000000000000190000000000000000009b
+            009d036901ac0ea6050000ab0500000000000000007d0a74120000000000
+            00000000006a160000000000000000a01700000000000000000000000000
+            000000000000007c0aa6010000ab010000000000000000010090018c6909
+            00640064006400a6020000ab02000000000000000001006e0b2300310073
+            0477027803590077010100590001000100640064006400a6020000ab0200
+            0000000000000001006e0b23003100730477027803590077010100590001
+            0001007c0544005d177d0b7413000000000000000000006a180000000000
+            0000007c0bac0fa6010000ab01000000000000000001008c1864005300
                        0 MAKE_CELL               12 (stage_dict)
          
          100           2 RESUME                   0
          
          102           4 LOAD_FAST                0 (event)
                        6 LOAD_ATTR                0 (data)
                       16 LOAD_METHOD              1 (get)
@@ -1013,15 +1015,15 @@
                      308 CALL                     0
                      318 BEFORE_WITH
                      320 POP_TOP
          
          115         322 LOAD_FAST                4 (domains)
                      324 GET_ITER
                  >>  326 EXTENDED_ARG             1
-                     328 FOR_ITER               315 (to 960)
+                     328 FOR_ITER               359 (to 1048)
                      330 STORE_FAST               7 (domain)
          
          117         332 LOAD_GLOBAL             18 (ts)
                      344 LOAD_ATTR               10 (helpers)
                      354 LOAD_METHOD             11 (clean_domain)
                      376 LOAD_FAST                7 (domain)
                      378 PRECALL                  1
@@ -1099,15 +1101,15 @@
                      724 POP_TOP
          
          150     >>  726 LOAD_DEREF              12 (stage_dict)
                      728 LOAD_METHOD              1 (get)
                      750 LOAD_FAST                7 (domain)
                      752 PRECALL                  1
                      756 CALL                     1
-                     766 POP_JUMP_FORWARD_IF_NONE    94 (to 956)
+                     766 POP_JUMP_FORWARD_IF_NONE   138 (to 1044)
          
          151         768 LOAD_GLOBAL             18 (ts)
                      780 LOAD_ATTR               18 (models)
                      790 LOAD_METHOD             19 (Event)
          
          152         812 LOAD_FAST                0 (event)
                      814 LOAD_ATTR                3 (search_uid)
@@ -1116,109 +1118,117 @@
                      826 LOAD_ATTR               15 (actor_key)
          
          154         836 LOAD_FAST                7 (domain)
          
          155         838 LOAD_CONST              12 ('comment')
          
          157         840 LOAD_CONST              12 ('comment')
-                     842 LOAD_CONST              13 ('imported ')
-                     844 LOAD_FAST                7 (domain)
-                     846 FORMAT_VALUE             0
-                     848 LOAD_CONST              14 ('. Was in stage: ')
-                     850 PUSH_NULL
-                     852 LOAD_FAST                3 (get_stage)
-                     854 LOAD_FAST                7 (domain)
-                     856 PRECALL                  1
-                     860 CALL                     1
-                     870 FORMAT_VALUE             0
-                     872 BUILD_STRING             4
-         
-         156         874 BUILD_MAP                1
-         
-         151         876 KW_NAMES                15
-                     878 PRECALL                  5
-                     882 CALL                     5
-                     892 STORE_FAST              10 (comment)
-         
-         160         894 LOAD_GLOBAL             18 (ts)
-                     906 LOAD_ATTR               20 (query)
-                     916 LOAD_METHOD             21 (insert_event)
-                     938 LOAD_FAST               10 (comment)
-                     940 PRECALL                  1
-                     944 CALL                     1
-                     954 POP_TOP
-                 >>  956 EXTENDED_ARG             1
-                     958 JUMP_BACKWARD          317 (to 326)
-         
-         115     >>  960 NOP
-         
-         114         962 LOAD_CONST               0 (None)
-                     964 LOAD_CONST               0 (None)
-                     966 LOAD_CONST               0 (None)
-                     968 PRECALL                  2
-                     972 CALL                     2
-                     982 POP_TOP
-                     984 JUMP_FORWARD            11 (to 1008)
-                 >>  986 PUSH_EXC_INFO
-                     988 WITH_EXCEPT_START
-                     990 POP_JUMP_FORWARD_IF_TRUE     4 (to 1000)
-                     992 RERAISE                  2
-                 >>  994 COPY                     3
-                     996 POP_EXCEPT
-                     998 RERAISE                  1
-                 >> 1000 POP_TOP
-                    1002 POP_EXCEPT
-                    1004 POP_TOP
-                    1006 POP_TOP
-         
-         113     >> 1008 LOAD_CONST               0 (None)
-                    1010 LOAD_CONST               0 (None)
-                    1012 LOAD_CONST               0 (None)
-                    1014 PRECALL                  2
-                    1018 CALL                     2
-                    1028 POP_TOP
-                    1030 JUMP_FORWARD            11 (to 1054)
-                 >> 1032 PUSH_EXC_INFO
-                    1034 WITH_EXCEPT_START
-                    1036 POP_JUMP_FORWARD_IF_TRUE     4 (to 1046)
-                    1038 RERAISE                  2
-                 >> 1040 COPY                     3
-                    1042 POP_EXCEPT
-                    1044 RERAISE                  1
-                 >> 1046 POP_TOP
-                    1048 POP_EXCEPT
-                    1050 POP_TOP
-                    1052 POP_TOP
-         
-         162     >> 1054 LOAD_FAST                5 (new_event_ids)
-                    1056 GET_ITER
-                 >> 1058 FOR_ITER                23 (to 1106)
-                    1060 STORE_FAST              11 (event_id)
-         
-         163        1062 LOAD_GLOBAL             19 (NULL + ts)
-                    1074 LOAD_ATTR               22 (trigger_process_event)
-                    1084 LOAD_FAST               11 (event_id)
-                    1086 KW_NAMES                16
-                    1088 PRECALL                  1
-                    1092 CALL                     1
-                    1102 POP_TOP
-                    1104 JUMP_BACKWARD           24 (to 1058)
+                     842 PUSH_NULL
+                     844 LOAD_FAST                3 (get_stage)
+                     846 LOAD_FAST                7 (domain)
+                     848 PRECALL                  1
+                     852 CALL                     1
+                     862 FORMAT_VALUE             0
+                     864 LOAD_CONST              13 (' → ')
+                     866 LOAD_GLOBAL             18 (ts)
+                     878 LOAD_ATTR               20 (constants)
+                     888 LOAD_ATTR               21 (LABEL_MAP)
+                     898 LOAD_FAST                0 (event)
+                     900 LOAD_ATTR                0 (data)
+                     910 LOAD_METHOD              1 (get)
+                     932 LOAD_CONST               4 ('stage')
+                     934 PRECALL                  1
+                     938 CALL                     1
+                     948 BINARY_SUBSCR
+                     958 FORMAT_VALUE             0
+                     960 BUILD_STRING             3
+         
+         156         962 BUILD_MAP                1
+         
+         151         964 KW_NAMES                14
+                     966 PRECALL                  5
+                     970 CALL                     5
+                     980 STORE_FAST              10 (comment)
+         
+         160         982 LOAD_GLOBAL             18 (ts)
+                     994 LOAD_ATTR               22 (query)
+                    1004 LOAD_METHOD             23 (insert_event)
+                    1026 LOAD_FAST               10 (comment)
+                    1028 PRECALL                  1
+                    1032 CALL                     1
+                    1042 POP_TOP
+                 >> 1044 EXTENDED_ARG             1
+                    1046 JUMP_BACKWARD          361 (to 326)
+         
+         115     >> 1048 NOP
+         
+         114        1050 LOAD_CONST               0 (None)
+                    1052 LOAD_CONST               0 (None)
+                    1054 LOAD_CONST               0 (None)
+                    1056 PRECALL                  2
+                    1060 CALL                     2
+                    1070 POP_TOP
+                    1072 JUMP_FORWARD            11 (to 1096)
+                 >> 1074 PUSH_EXC_INFO
+                    1076 WITH_EXCEPT_START
+                    1078 POP_JUMP_FORWARD_IF_TRUE     4 (to 1088)
+                    1080 RERAISE                  2
+                 >> 1082 COPY                     3
+                    1084 POP_EXCEPT
+                    1086 RERAISE                  1
+                 >> 1088 POP_TOP
+                    1090 POP_EXCEPT
+                    1092 POP_TOP
+                    1094 POP_TOP
+         
+         113     >> 1096 LOAD_CONST               0 (None)
+                    1098 LOAD_CONST               0 (None)
+                    1100 LOAD_CONST               0 (None)
+                    1102 PRECALL                  2
+                    1106 CALL                     2
+                    1116 POP_TOP
+                    1118 JUMP_FORWARD            11 (to 1142)
+                 >> 1120 PUSH_EXC_INFO
+                    1122 WITH_EXCEPT_START
+                    1124 POP_JUMP_FORWARD_IF_TRUE     4 (to 1134)
+                    1126 RERAISE                  2
+                 >> 1128 COPY                     3
+                    1130 POP_EXCEPT
+                    1132 RERAISE                  1
+                 >> 1134 POP_TOP
+                    1136 POP_EXCEPT
+                    1138 POP_TOP
+                    1140 POP_TOP
+         
+         162     >> 1142 LOAD_FAST                5 (new_event_ids)
+                    1144 GET_ITER
+                 >> 1146 FOR_ITER                23 (to 1194)
+                    1148 STORE_FAST              11 (event_id)
+         
+         163        1150 LOAD_GLOBAL             19 (NULL + ts)
+                    1162 LOAD_ATTR               24 (trigger_process_event)
+                    1172 LOAD_FAST               11 (event_id)
+                    1174 KW_NAMES                15
+                    1176 PRECALL                  1
+                    1180 CALL                     1
+                    1190 POP_TOP
+                    1192 JUMP_BACKWARD           24 (to 1146)
          
-         162     >> 1106 LOAD_CONST               0 (None)
-                    1108 RETURN_VALUE
+         162     >> 1194 LOAD_CONST               0 (None)
+                    1196 RETURN_VALUE
          ExceptionTable:
-           278 to 318 -> 1032 [1] lasti
-           320 to 958 -> 986 [2] lasti
-           962 to 984 -> 1032 [1] lasti
-           986 to 992 -> 994 [4] lasti
-           994 to 998 -> 1032 [1] lasti
-           1000 to 1000 -> 994 [4] lasti
-           1002 to 1006 -> 1032 [1] lasti
-           1032 to 1038 -> 1040 [3] lasti
-           1046 to 1046 -> 1040 [3] lasti
+           278 to 318 -> 1120 [1] lasti
+           320 to 1046 -> 1074 [2] lasti
+           1050 to 1072 -> 1120 [1] lasti
+           1074 to 1080 -> 1082 [4] lasti
+           1082 to 1086 -> 1120 [1] lasti
+           1088 to 1088 -> 1082 [4] lasti
+           1090 to 1094 -> 1120 [1] lasti
+           1120 to 1126 -> 1128 [3] lasti
+           1134 to 1134 -> 1128 [3] lasti
          consts
             None
             'source'
             ('search_uid',)
             'domain'
             'stage'
             code
@@ -1267,29 +1277,28 @@
             'domains'
             '\n                        INSERT INTO company (domain, source) \n                        VALUES(:domain, :source)\n                        ON CONFLICT DO NOTHING\n                        '
             ('domain', 'source')
             '\n                        INSERT INTO event (search_uid, domain, actor_key, type) \n                        VALUES(:search_uid, :domain, :actor_key, :type)\n                        ON CONFLICT DO NOTHING\n                        RETURNING id\n                        '
             'create'
             ('search_uid', 'actor_key', 'domain', 'type')
             'comment'
-            'imported '
-            '. Was in stage: '
+            ' → '
             ('search_uid', 'actor_key', 'domain', 'type', 'data')
             ('event_id',)
-         names      ('data', 'get', 'search_targets', 'search_uid', 'set_index', 'to_dict', 'db', 'connect', 'begin', 'ts', 'helpers', 'clean_domain', 'execute', 'sqlalchemy', 'text', 'actor_key', 'scalar_one', 'append', 'models', 'Event', 'query', 'insert_event', 'trigger_process_event')
+         names      ('data', 'get', 'search_targets', 'search_uid', 'set_index', 'to_dict', 'db', 'connect', 'begin', 'ts', 'helpers', 'clean_domain', 'execute', 'sqlalchemy', 'text', 'actor_key', 'scalar_one', 'append', 'models', 'Event', 'constants', 'LABEL_MAP', 'query', 'insert_event', 'trigger_process_event')
          varnames   ('event', 'source', 'targets', 'get_stage', 'domains', 'new_event_ids', 'con', 'domain', 'result', 'new_event_id', 'comment', 'event_id')
          freevars   ()
          cellvars   ('stage_dict',)
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'important_targets_from_event'
          firstlineno 100
          lnotab
             0x040234012a015a020a041a02040134012a010a023e011801160102ff0e
             0708f8100b1801160102ff0e090c010c01020134fc04f71011280104012a
-            022a012c010c010c010201020222ff02fb120942d302ff2eff2e3108012c
+            022a012c010c010c01020102027aff02fb120942d302ff2eff2e3108012c
             ff
       False
       'companies'
       'search_uid'
       'actor_key'
       'force'
       'source'
```

### Comparing `gandai-1.7.45/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.46/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/analytics.py` & `gandai-1.7.46/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/constants.py` & `gandai-1.7.46/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/db.py` & `gandai-1.7.46/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/google.py` & `gandai-1.7.46/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/gpt.py` & `gandai-1.7.46/gandai/gpt.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/grata.py` & `gandai-1.7.46/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/helpers.py` & `gandai-1.7.46/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/main.py` & `gandai-1.7.46/gandai/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,19 @@
         print(e)
         e.data["prompt"] = event.data["prompt"]
         ts.query.insert_event(e)
 
 
 def enrich_with_gpt(company: ts.models.Company) -> None:
     print("enriching with gpt...")
-    homepage_text = ts.helpers.get_homepage_text(company.domain)
+    try:
+        homepage_text = ts.helpers.get_homepage_text(company.domain)
+    except Exception as e:
+        print(e)
+        homepage_text = "<could not fetch homepage>"
     messages = [
         {
             "role": "system",
             "content": f"You will help us evaluate {company.name} for acquisition.",
         },
         {
             "role": "system",
```

### Comparing `gandai-1.7.45/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.46/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/migrations/db_seed.py` & `gandai-1.7.46/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/migrations/dealcloud.py` & `gandai-1.7.46/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.46/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/migrations/sql/schema.sql` & `gandai-1.7.46/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/models.py` & `gandai-1.7.46/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/query.py` & `gandai-1.7.46/gandai/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                 if stage_dict.get(domain) is not None:
                     comment = ts.models.Event(
                         search_uid=event.search_uid,
                         actor_key=event.actor_key,  # todo this should be the system
                         domain=domain,
                         type="comment",
                         data={
-                            "comment": f"imported {domain}. Was in stage: {get_stage(domain)}",
+                            "comment": f"{get_stage(domain)} → {ts.constants.LABEL_MAP[event.data.get('stage')]}"
                         },
                     )
                     ts.query.insert_event(comment)
 
     for event_id in new_event_ids:
         ts.trigger_process_event(event_id=event_id)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gandai-1.7.45/gandai/secrets.py` & `gandai-1.7.46/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.45/gandai/tasks.py` & `gandai-1.7.46/gandai/tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import gandai as ts
 from gandai import main
 from google.cloud import tasks_v2
 
 
 def trigger_process_event(event_id: int) -> None:
-    if os.getenv("ENV") == "local":
+    if False:
         main.process_event(event_id=event_id)
         # Thread(target=main.process_event, kwargs={"event_id": event_id}).start()
     else:
         client = tasks_v2.CloudTasksClient()
         parent = client.queue_path(
             project=os.getenv("GOOGLE_CLOUD_PROJECT", "targetselect-staging"),
             location="us-central1",
```

### Comparing `gandai-1.7.45/gandai.egg-info/SOURCES.txt` & `gandai-1.7.46/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

