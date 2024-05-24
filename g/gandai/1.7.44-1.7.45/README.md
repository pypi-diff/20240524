# Comparing `tmp/gandai-1.7.44.tar.gz` & `tmp/gandai-1.7.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.44.tar", last modified: Thu May 23 23:35:03 2024, max compression
+gzip compressed data, was "gandai-1.7.45.tar", last modified: Fri May 24 03:39:48 2024, max compression
```

## Comparing `gandai-1.7.44.tar` & `gandai-1.7.45.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.777294 gandai-1.7.44/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.44/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:35:03.777106 gandai-1.7.44/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.767256 gandai-1.7.44/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.44/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.773867 gandai-1.7.44/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.44/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.44/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.44/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.44/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2600 2024-03-29 15:40:37.000000 gandai-1.7.44/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.44/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.44/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.44/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7026 2024-05-23 22:33:44.000000 gandai-1.7.44/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.44/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2564 2024-05-23 22:34:21.000000 gandai-1.7.44/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    15739 2024-05-23 23:34:14.000000 gandai-1.7.44/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.44/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    42225 2024-05-23 22:23:40.000000 gandai-1.7.44/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.44/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.44/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.44/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1695 2024-05-07 15:22:26.000000 gandai-1.7.44/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.44/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1674 2024-03-29 15:34:07.000000 gandai-1.7.44/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.44/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.44/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)     6384 2024-05-23 22:33:42.000000 gandai-1.7.44/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.44/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1204 2024-05-23 22:34:19.000000 gandai-1.7.44/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    11060 2024-05-23 23:34:12.000000 gandai-1.7.44/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.774798 gandai-1.7.44/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.44/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.775177 gandai-1.7.44/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.44/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.44/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.44/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.44/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.44/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.776663 gandai-1.7.44/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.44/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.44/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.44/gandai/migrations/sql/240523-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.44/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.44/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    28619 2024-05-23 22:23:38.000000 gandai-1.7.44/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.44/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1079 2024-05-06 22:42:54.000000 gandai-1.7.44/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:35:03.776919 gandai-1.7.44/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:35:03.000000 gandai-1.7.44/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-23 23:35:03.000000 gandai-1.7.44/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-23 23:35:03.000000 gandai-1.7.44/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-23 23:35:03.000000 gandai-1.7.44/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-23 23:34:32.000000 gandai-1.7.44/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-23 23:35:03.777332 gandai-1.7.44/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.44/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.689491 gandai-1.7.45/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.45/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 03:39:48.689278 gandai-1.7.45/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.679484 gandai-1.7.45/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.45/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.686157 gandai-1.7.45/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.45/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.45/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.45/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.45/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2600 2024-05-24 00:47:47.000000 gandai-1.7.45/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.45/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.45/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.45/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7037 2024-05-23 23:56:05.000000 gandai-1.7.45/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.45/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2564 2024-05-23 22:34:21.000000 gandai-1.7.45/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    15923 2024-05-24 03:37:15.000000 gandai-1.7.45/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.45/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    42286 2024-05-23 23:53:21.000000 gandai-1.7.45/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.45/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.45/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.45/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1695 2024-05-24 03:39:23.000000 gandai-1.7.45/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.45/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1674 2024-05-24 00:47:46.000000 gandai-1.7.45/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.45/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.45/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)     6395 2024-05-23 23:56:03.000000 gandai-1.7.45/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.45/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1204 2024-05-23 22:34:19.000000 gandai-1.7.45/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    11171 2024-05-24 03:37:12.000000 gandai-1.7.45/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.686894 gandai-1.7.45/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.45/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.687288 gandai-1.7.45/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.45/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.45/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.45/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.45/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.45/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.688817 gandai-1.7.45/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.45/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.45/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.45/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.45/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.45/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    28680 2024-05-23 23:53:18.000000 gandai-1.7.45/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.45/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1079 2024-05-24 03:39:21.000000 gandai-1.7.45/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-24 03:39:48.689090 gandai-1.7.45/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-24 03:39:48.000000 gandai-1.7.45/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-24 03:39:48.000000 gandai-1.7.45/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-24 03:39:48.000000 gandai-1.7.45/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-24 03:39:48.000000 gandai-1.7.45/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-24 03:39:30.000000 gandai-1.7.45/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-24 03:39:48.689529 gandai-1.7.45/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.45/setup.py
```

### Comparing `gandai-1.7.44/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x6fdf0666 (Fri Mar 29 15:34:07 2024 UTC)
+moddate:  0xb2e34f66 (Fri May 24 00:47:46 2024 UTC)
 files sz: 1674
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
```

### Comparing `gandai-1.7.44/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/gpt.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/gpt.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x46c44f66 (Thu May 23 22:33:42 2024 UTC)
-files sz: 6384
+moddate:  0x93d74f66 (Thu May 23 23:56:03 2024 UTC)
+files sz: 6395
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a02640064026c016d035a0301
@@ -58,30 +58,30 @@
                 98 LOAD_CONST               7 ('return')
                100 LOAD_NAME                0 (json)
                102 BUILD_TUPLE              4
                104 LOAD_CONST               8 (<code object ask_gpt4, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py", line 14>)
                106 MAKE_FUNCTION            4 (annotations)
                108 STORE_NAME               9 (ask_gpt4)
    
-    27         110 LOAD_CONST               9 ('\nTo update an attribute for a company you will create an event with the company\'s domain\nof type "update". This will update that company\'s meta field \n\nhere is an example update event\n\n{\n    "domain": "lol.com",\n    "actor_key": "chatgpt",\n    "type": "update",\n    "data": {\n        "contact_name": "Bob"\n    }\n}\n\nHere are all the fields you can use for event[\'data\']\n\nc.meta->>\'description\' as description, -- a description of the company for use by private equity research analyst to understand the company.\nc.meta->>\'employees\' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.\nc.meta->>\'ownership\' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] \nc.meta->>\'headquarters\' as headquarters,\nc.meta->>\'city\' as city,\nc.meta->>\'state\' as state,\nc.meta->>\'designation\' as designation,\nc.meta->>\'products\' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.\nc.meta->>\'services\' as services, -- services are intangible goods offered by the company. do not list products here.\nc.meta->>\'end_customer\' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.\nc.meta->>\'geographies\' as geographies, -- geographies are the areas where the company does business. \nc.meta->>\'year_founded\' as year_founded,\nc.meta->>\'linkedin\' as linkedin, -- linkedinUrl \nc.meta->>\'linkedin_range\' as linkedin_range,\nc.meta->>\'industry\' as industry,\nc.meta->>\'revenue_estimates\' as revenue_estimates,\nc.meta->>\'location_count\' as location_count,\nc.meta->>\'business_models\' as business_models,\nc.meta->>\'facility_size\' as facility_size,\nc.meta->>\'contact_name\' as contact_name,\nc.meta->>\'contact_title\' as contact_title,\nc.meta->>\'contact_email\' as contact_email,\nc.meta->>\'contact_phone\' as contact_phone,\nc.meta->>\'contact_address\' as contact_address,\n\nFor fields that are lists, you will use a csv string \nFor these lists, such as products or services, try to stick to top 5 or less areas of focus.\n\nYou will fill out the description field with a description of the company. \nThe description will be a comprehensive description of the company for use by private equity research analyst to understand the company.\n\nIf you are unsure, just leave that key out of the response data\n\n')
+    27         110 LOAD_CONST               9 ('\nTo update an attribute for a company you will create an event with the company\'s domain\nof type "update". This will update that company\'s meta field \n\nhere is an example update event\n\n{\n    "domain": "lol.com",\n    "actor_key": "chatgpt",\n    "type": "update",\n    "data": {\n        "contact_name": "Bob"\n    }\n}\n\nHere are all the fields you can use for event[\'data\']\n\nc.data->>\'gpt_description\' as gpt_description, -- a description of the company for use by private equity research analyst to understand the company.\n\nYou will fill out the description field with a description of the company. \nThe description will be a comprehensive description of the company for use \nby private equity research analyst to understand the company.\n\nc.data->>\'employees\' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.\nc.data->>\'ownership\' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] \nc.data->>\'headquarters\' as headquarters,\nc.data->>\'city\' as city,\nc.data->>\'state\' as state,\nc.data->>\'designation\' as designation,\nc.data->>\'products\' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.\nc.data->>\'services\' as services, -- services are intangible goods offered by the company. do not list products here.\nc.data->>\'end_customer\' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.\nc.data->>\'geographies\' as geographies, -- geographies are the areas where the company does business. \nc.data->>\'year_founded\' as year_founded,\nc.data->>\'linkedin\' as linkedin, -- linkedinUrl \nc.data->>\'linkedin_range\' as linkedin_range,\nc.data->>\'industry\' as industry,\nc.data->>\'revenue_estimates\' as revenue_estimates,\nc.data->>\'location_count\' as location_count,\nc.data->>\'business_models\' as business_models,\nc.data->>\'facility_size\' as facility_size,\nc.data->>\'contact_name\' as contact_name,\nc.data->>\'contact_title\' as contact_title,\nc.data->>\'contact_email\' as contact_email,\nc.data->>\'contact_phone\' as contact_phone,\nc.data->>\'contact_address\' as contact_address,\n\nFor fields that are lists, you will use a csv string \nFor these lists, such as products or services, try to stick to top 5 or less areas of focus.\n\n\nIf you are unsure, just leave that key out of the response data\n\n')
                112 STORE_NAME              10 (HOW_TO_ENRICH)
    
-    80         114 LOAD_CONST              10 ('\nYou will respond with an JSON object that looks like this:\n{\n    "events": List[Event],\n}\n')
+    83         114 LOAD_CONST              10 ('\nYou will respond with an JSON object that looks like this:\n{\n    "events": List[Event],\n}\n')
                116 STORE_NAME              11 (HOW_TO_RESPOND)
    
-    87         118 LOAD_CONST              11 ('\nTo search the Google Maps Places API\nYou will respond with this\n{"events": List[asdict(Event)]}\n\nUnless otherwise directed you will return 10 centroids\n\nThere are 20 results per centroid\nSo if the user asks for 100 results you will return the count divided by 20\n\nGive me the query strings you would use to search for \nEach query string should be small enough for a Google Maps search\n\nFor example to search throughout Dallas you might use:\ndentists in Dallas, TX\ndentists in Highland Park, TX\ndentists in Grapevine, TX\ndentists in Plano, TX\n\nNow give me the queries that you would use\n\nHere\'s some Event examples:\n[{\n    "type": "maps",\n    "search_uid": 1700,\n    "actor_key": "7138248581",\n    "data": {\n        "query": "dentists in Dallas, TX"\n    }\n}]\n\n')
+    90         118 LOAD_CONST              11 ('\nTo search the Google Maps Places API\nYou will respond with this\n{"events": List[asdict(Event)]}\n\nUnless otherwise directed you will return 10 centroids\n\nThere are 20 results per centroid\nSo if the user asks for 100 results you will return the count divided by 20\n\nGive me the query strings you would use to search for \nEach query string should be small enough for a Google Maps search\n\nFor example to search throughout Dallas you might use:\ndentists in Dallas, TX\ndentists in Highland Park, TX\ndentists in Grapevine, TX\ndentists in Plano, TX\n\nNow give me the queries that you would use\n\nHere\'s some Event examples:\n[{\n    "type": "maps",\n    "search_uid": 1700,\n    "actor_key": "7138248581",\n    "data": {\n        "query": "dentists in Dallas, TX"\n    }\n}]\n\n')
                120 STORE_NAME              12 (HOW_TO_GOOGLE_MAPS)
    
-   120         122 LOAD_CONST              12 ('\n// example Import(Event)\n{\n    "search_uid": 19696114,\n    "domain": null,\n    "actor_key": "4805705555",\n    "type": "import",\n    "data": {\n        "stage": "advance",\n        "domains": [\n            "buybits.com",\n            "lidoradio.com",\n            "rocklandcustomproducts.com",\n            "sigmasafety.ca",\n        ],\n    },\n}\n\nHere are the stages along with their labels:\nThe only valid stages are labelMap.keys()\nconst labelMap = {\n    "land": "Landing",\n    "create": "Inbox",\n    "advance": "Review",\n    "validate": "Validated",\n    "send": "Client Inbox",\n    "client_approve": "Client Approved",\n    "sync": "Synced",\n    "reject": "Reject",\n    "conflict": "Conflict",\n    "client_conflict": "Client Conflict",\n    "client_reject": "Client Reject"\n}\n')
+   123         122 LOAD_CONST              12 ('\n// example Import(Event)\n{\n    "search_uid": 19696114,\n    "domain": null,\n    "actor_key": "4805705555",\n    "type": "import",\n    "data": {\n        "stage": "advance",\n        "domains": [\n            "buybits.com",\n            "lidoradio.com",\n            "rocklandcustomproducts.com",\n            "sigmasafety.ca",\n        ],\n    },\n}\n\nHere are the stages along with their labels:\nThe only valid stages are labelMap.keys()\nconst labelMap = {\n    "land": "Landing",\n    "create": "Inbox",\n    "advance": "Review",\n    "validate": "Validated",\n    "send": "Client Inbox",\n    "client_approve": "Client Approved",\n    "sync": "Synced",\n    "reject": "Reject",\n    "conflict": "Conflict",\n    "client_conflict": "Client Conflict",\n    "client_reject": "Client Reject"\n}\n')
                124 STORE_NAME              13 (HOW_TO_IMPORT)
    
-   155         126 LOAD_CONST              13 ('\nTo move a target to a different stage you will create an event with the targets domain \nand the stage you want to move it to.\n\ndomain should include domain only, no subdomain or protocol\n\n// example Event\n{\n    "search_uid": 19696114,\n    "domain": "acme.com",\n    "actor_key": "5558248581",\n    "type": "send",\n    "data": {"key": "value"},\n}\n\n\nHere are the stages along with their labels:\nThe only valid event types are the labelMap.keys()\nconst labelMap = {\n    "land": "Landing",\n    "create": "Inbox",\n    "advance": "Review",\n    "validate": "Validated",\n    "send": "Client Inbox",\n    "client_approve": "Client Approved",\n    "sync": "Synced",\n    "reject": "Reject",\n    "conflict": "Conflict",\n    "client_conflict": "Client Conflict",\n    "client_reject": "Client Reject"\n}\n')
+   158         126 LOAD_CONST              13 ('\nTo move a target to a different stage you will create an event with the targets domain \nand the stage you want to move it to.\n\ndomain should include domain only, no subdomain or protocol\n\n// example Event\n{\n    "search_uid": 19696114,\n    "domain": "acme.com",\n    "actor_key": "5558248581",\n    "type": "send",\n    "data": {"key": "value"},\n}\n\n\nHere are the stages along with their labels:\nThe only valid event types are the labelMap.keys()\nconst labelMap = {\n    "land": "Landing",\n    "create": "Inbox",\n    "advance": "Review",\n    "validate": "Validated",\n    "send": "Client Inbox",\n    "client_approve": "Client Approved",\n    "sync": "Synced",\n    "reject": "Reject",\n    "conflict": "Conflict",\n    "client_conflict": "Client Conflict",\n    "client_reject": "Client Reject"\n}\n')
                128 STORE_NAME              14 (HOW_TO_TRANSITION)
    
-   188         130 LOAD_CONST              14 ('\n\nTo search Google, you will create an Event object.\n\n@dataclass\nclass Google(Event):\n    search_uid: int  # fk # add index\n    actor_key: str  # fk\n    type: str  \n    data: dict = field(default_factory=dict)\n    id: int = field(default=None)  # pk\n    # created: int = field(init=False)\n\nList[Event] examples asdict:\n\n[{\n  \'search_uid\': 200,\n  \'domain\': null,\n  \'actor_key\': \'3125740050\',\n  \'type\': \'google\',\n  \'data\': {\'q\': \'"golf cart" AND audio\'},\n  \'created\': 1697813193},\n{\n  \'search_uid\': 5255570,\n  \'domain\': null,\n  \'actor_key\': \'3102835279\',\n  \'type\': \'google\',\n  \'data\': {\'q\': \'"commercial" AND "door" AND ("repair" OR "maintenance" OR "replacement") AND "new York City"\'},\n  \'created\': 1697814555}]\n\nThe type is \'google\'\nYou will not set the id or created fields.\nThe default count is 10\n\n')
+   191         130 LOAD_CONST              14 ('\n\nTo search Google, you will create an Event object.\n\n@dataclass\nclass Google(Event):\n    search_uid: int  # fk # add index\n    actor_key: str  # fk\n    type: str  \n    data: dict = field(default_factory=dict)\n    id: int = field(default=None)  # pk\n    # created: int = field(init=False)\n\nList[Event] examples asdict:\n\n[{\n  \'search_uid\': 200,\n  \'domain\': null,\n  \'actor_key\': \'3125740050\',\n  \'type\': \'google\',\n  \'data\': {\'q\': \'"golf cart" AND audio\'},\n  \'created\': 1697813193},\n{\n  \'search_uid\': 5255570,\n  \'domain\': null,\n  \'actor_key\': \'3102835279\',\n  \'type\': \'google\',\n  \'data\': {\'q\': \'"commercial" AND "door" AND ("repair" OR "maintenance" OR "replacement") AND "new York City"\'},\n  \'created\': 1697814555}]\n\nThe type is \'google\'\nYou will not set the id or created fields.\nThe default count is 10\n\n')
                132 STORE_NAME              15 (HOW_TO_GOOGLE)
                134 LOAD_CONST               1 (None)
                136 RETURN_VALUE
    consts
       0
       None
       ('secrets',)
@@ -155,23 +155,23 @@
          varnames   ('messages', 'chat_completion')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py'
          name       'ask_gpt4'
          firstlineno 14
          lnotab 0x0201360102010202020106fb12082801
-      '\nTo update an attribute for a company you will create an event with the company\'s domain\nof type "update". This will update that company\'s meta field \n\nhere is an example update event\n\n{\n    "domain": "lol.com",\n    "actor_key": "chatgpt",\n    "type": "update",\n    "data": {\n        "contact_name": "Bob"\n    }\n}\n\nHere are all the fields you can use for event[\'data\']\n\nc.meta->>\'description\' as description, -- a description of the company for use by private equity research analyst to understand the company.\nc.meta->>\'employees\' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.\nc.meta->>\'ownership\' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] \nc.meta->>\'headquarters\' as headquarters,\nc.meta->>\'city\' as city,\nc.meta->>\'state\' as state,\nc.meta->>\'designation\' as designation,\nc.meta->>\'products\' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.\nc.meta->>\'services\' as services, -- services are intangible goods offered by the company. do not list products here.\nc.meta->>\'end_customer\' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.\nc.meta->>\'geographies\' as geographies, -- geographies are the areas where the company does business. \nc.meta->>\'year_founded\' as year_founded,\nc.meta->>\'linkedin\' as linkedin, -- linkedinUrl \nc.meta->>\'linkedin_range\' as linkedin_range,\nc.meta->>\'industry\' as industry,\nc.meta->>\'revenue_estimates\' as revenue_estimates,\nc.meta->>\'location_count\' as location_count,\nc.meta->>\'business_models\' as business_models,\nc.meta->>\'facility_size\' as facility_size,\nc.meta->>\'contact_name\' as contact_name,\nc.meta->>\'contact_title\' as contact_title,\nc.meta->>\'contact_email\' as contact_email,\nc.meta->>\'contact_phone\' as contact_phone,\nc.meta->>\'contact_address\' as contact_address,\n\nFor fields that are lists, you will use a csv string \nFor these lists, such as products or services, try to stick to top 5 or less areas of focus.\n\nYou will fill out the description field with a description of the company. \nThe description will be a comprehensive description of the company for use by private equity research analyst to understand the company.\n\nIf you are unsure, just leave that key out of the response data\n\n'
+      '\nTo update an attribute for a company you will create an event with the company\'s domain\nof type "update". This will update that company\'s meta field \n\nhere is an example update event\n\n{\n    "domain": "lol.com",\n    "actor_key": "chatgpt",\n    "type": "update",\n    "data": {\n        "contact_name": "Bob"\n    }\n}\n\nHere are all the fields you can use for event[\'data\']\n\nc.data->>\'gpt_description\' as gpt_description, -- a description of the company for use by private equity research analyst to understand the company.\n\nYou will fill out the description field with a description of the company. \nThe description will be a comprehensive description of the company for use \nby private equity research analyst to understand the company.\n\nc.data->>\'employees\' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.\nc.data->>\'ownership\' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] \nc.data->>\'headquarters\' as headquarters,\nc.data->>\'city\' as city,\nc.data->>\'state\' as state,\nc.data->>\'designation\' as designation,\nc.data->>\'products\' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.\nc.data->>\'services\' as services, -- services are intangible goods offered by the company. do not list products here.\nc.data->>\'end_customer\' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.\nc.data->>\'geographies\' as geographies, -- geographies are the areas where the company does business. \nc.data->>\'year_founded\' as year_founded,\nc.data->>\'linkedin\' as linkedin, -- linkedinUrl \nc.data->>\'linkedin_range\' as linkedin_range,\nc.data->>\'industry\' as industry,\nc.data->>\'revenue_estimates\' as revenue_estimates,\nc.data->>\'location_count\' as location_count,\nc.data->>\'business_models\' as business_models,\nc.data->>\'facility_size\' as facility_size,\nc.data->>\'contact_name\' as contact_name,\nc.data->>\'contact_title\' as contact_title,\nc.data->>\'contact_email\' as contact_email,\nc.data->>\'contact_phone\' as contact_phone,\nc.data->>\'contact_address\' as contact_address,\n\nFor fields that are lists, you will use a csv string \nFor these lists, such as products or services, try to stick to top 5 or less areas of focus.\n\n\nIf you are unsure, just leave that key out of the response data\n\n'
       '\nYou will respond with an JSON object that looks like this:\n{\n    "events": List[Event],\n}\n'
       '\nTo search the Google Maps Places API\nYou will respond with this\n{"events": List[asdict(Event)]}\n\nUnless otherwise directed you will return 10 centroids\n\nThere are 20 results per centroid\nSo if the user asks for 100 results you will return the count divided by 20\n\nGive me the query strings you would use to search for \nEach query string should be small enough for a Google Maps search\n\nFor example to search throughout Dallas you might use:\ndentists in Dallas, TX\ndentists in Highland Park, TX\ndentists in Grapevine, TX\ndentists in Plano, TX\n\nNow give me the queries that you would use\n\nHere\'s some Event examples:\n[{\n    "type": "maps",\n    "search_uid": 1700,\n    "actor_key": "7138248581",\n    "data": {\n        "query": "dentists in Dallas, TX"\n    }\n}]\n\n'
       '\n// example Import(Event)\n{\n    "search_uid": 19696114,\n    "domain": null,\n    "actor_key": "4805705555",\n    "type": "import",\n    "data": {\n        "stage": "advance",\n        "domains": [\n            "buybits.com",\n            "lidoradio.com",\n            "rocklandcustomproducts.com",\n            "sigmasafety.ca",\n        ],\n    },\n}\n\nHere are the stages along with their labels:\nThe only valid stages are labelMap.keys()\nconst labelMap = {\n    "land": "Landing",\n    "create": "Inbox",\n    "advance": "Review",\n    "validate": "Validated",\n    "send": "Client Inbox",\n    "client_approve": "Client Approved",\n    "sync": "Synced",\n    "reject": "Reject",\n    "conflict": "Conflict",\n    "client_conflict": "Client Conflict",\n    "client_reject": "Client Reject"\n}\n'
       '\nTo move a target to a different stage you will create an event with the targets domain \nand the stage you want to move it to.\n\ndomain should include domain only, no subdomain or protocol\n\n// example Event\n{\n    "search_uid": 19696114,\n    "domain": "acme.com",\n    "actor_key": "5558248581",\n    "type": "send",\n    "data": {"key": "value"},\n}\n\n\nHere are the stages along with their labels:\nThe only valid event types are the labelMap.keys()\nconst labelMap = {\n    "land": "Landing",\n    "create": "Inbox",\n    "advance": "Review",\n    "validate": "Validated",\n    "send": "Client Inbox",\n    "client_approve": "Client Approved",\n    "sync": "Synced",\n    "reject": "Reject",\n    "conflict": "Conflict",\n    "client_conflict": "Client Conflict",\n    "client_reject": "Client Reject"\n}\n'
       '\n\nTo search Google, you will create an Event object.\n\n@dataclass\nclass Google(Event):\n    search_uid: int  # fk # add index\n    actor_key: str  # fk\n    type: str  \n    data: dict = field(default_factory=dict)\n    id: int = field(default=None)  # pk\n    # created: int = field(init=False)\n\nList[Event] examples asdict:\n\n[{\n  \'search_uid\': 200,\n  \'domain\': null,\n  \'actor_key\': \'3125740050\',\n  \'type\': \'google\',\n  \'data\': {\'q\': \'"golf cart" AND audio\'},\n  \'created\': 1697813193},\n{\n  \'search_uid\': 5255570,\n  \'domain\': null,\n  \'actor_key\': \'3102835279\',\n  \'type\': \'google\',\n  \'data\': {\'q\': \'"commercial" AND "door" AND ("repair" OR "maintenance" OR "replacement") AND "new York City"\'},\n  \'created\': 1697814555}]\n\nThe type is \'google\'\nYou will not set the id or created fields.\nThe default count is 10\n\n'
    names      ('json', 'gandai', 'ts', 'secrets', 'openai', 'OpenAI', 'access_secret_version', 'client', 'list', 'ask_gpt4', 'HOW_TO_ENRICH', 'HOW_TO_RESPOND', 'HOW_TO_GOOGLE_MAPS', 'HOW_TO_IMPORT', 'HOW_TO_TRANSITION', 'HOW_TO_GOOGLE')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/gpt.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080208010c010c0204011eff1207100d043504070421042304
+      0x00ff0201080208010c010c0204011eff1207100d043804070421042304
       21
```

### Comparing `gandai-1.7.44/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/helpers.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,167 +1,167 @@
 magic:    0xa70d0d0a
-moddate:  0x74d24f66 (Thu May 23 23:34:12 2024 UTC)
-files sz: 11060
+moddate:  0x680b5066 (Fri May 24 03:37:12 2024 UTC)
+files sz: 11171
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
-      0x9700640064016c006d005a000100640064026c016d025a020100640064
-      036c036d045a040100640064046c055a06640565076602640684045a0864
-      0765066a0900000000000000006a0a000000000000000064056507640864
-      046606640984045a0b640765066a0900000000000000006a0a0000000000
-      000000640864046604640a84045a0c640765066a0900000000000000006a
-      0a0000000000000000640b65066a0900000000000000006a0d0000000000
-      000000640864046606640c84045a0e640765066a0900000000000000006a
-      0a0000000000000000640b65066a0900000000000000006a0d0000000000
-      000000640864046606640d84045a0f640b65066a0900000000000000006a
-      0d0000000000000000640864046604640e84045a10640f65066a09000000
-      00000000006a110000000000000000640864046604641084045a12640b65
-      066a0900000000000000006a0d0000000000000000640864046604641184
-      045a1364126514640864046604641384045a1564045300
+      0x9700640064016c006d015a010100640064026c026d025a020100640064
+      036c035a04640064046c056d065a060100640565076602640684045a0864
+      0765046a0900000000000000006a0a000000000000000064056507640864
+      036606640984045a0b640765046a0900000000000000006a0a0000000000
+      000000640864036604640a84045a0c640765046a0900000000000000006a
+      0a0000000000000000640b65046a0900000000000000006a0d0000000000
+      000000640864036606640c84045a0e640765046a0900000000000000006a
+      0a0000000000000000640b65046a0900000000000000006a0d0000000000
+      000000640864036606640d84045a0f640b65046a0900000000000000006a
+      0d0000000000000000640864036604640e84045a10640f65046a09000000
+      00000000006a110000000000000000640864036604641084045a12640b65
+      046a0900000000000000006a0d0000000000000000640864036604641184
+      045a1364126514640864036604641384045a1564035300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('time',))
-                 6 IMPORT_NAME              0 (time)
-                 8 IMPORT_FROM              0 (time)
-                10 STORE_NAME               0 (time)
+                 4 LOAD_CONST               1 (('asdict',))
+                 6 IMPORT_NAME              0 (dataclasses)
+                 8 IMPORT_FROM              1 (asdict)
+                10 STORE_NAME               1 (asdict)
                 12 POP_TOP
    
      2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('asdict',))
-                18 IMPORT_NAME              1 (dataclasses)
-                20 IMPORT_FROM              2 (asdict)
-                22 STORE_NAME               2 (asdict)
+                16 LOAD_CONST               2 (('time',))
+                18 IMPORT_NAME              2 (time)
+                20 IMPORT_FROM              2 (time)
+                22 STORE_NAME               2 (time)
                 24 POP_TOP
    
-     3          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               3 (('from_dict',))
-                30 IMPORT_NAME              3 (dacite)
-                32 IMPORT_FROM              4 (from_dict)
-                34 STORE_NAME               4 (from_dict)
-                36 POP_TOP
+     4          26 LOAD_CONST               0 (0)
+                28 LOAD_CONST               3 (None)
+                30 IMPORT_NAME              3 (gandai)
+                32 STORE_NAME               4 (ts)
    
-     5          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               4 (None)
-                42 IMPORT_NAME              5 (gandai)
-                44 STORE_NAME               6 (ts)
+     5          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               4 (('from_dict',))
+                38 IMPORT_NAME              5 (dacite)
+                40 IMPORT_FROM              6 (from_dict)
+                42 STORE_NAME               6 (from_dict)
+                44 POP_TOP
    
      8          46 LOAD_CONST               5 ('domain')
                 48 LOAD_NAME                7 (str)
                 50 BUILD_TUPLE              2
                 52 LOAD_CONST               6 (<code object run_acquired_check, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 8>)
                 54 MAKE_FUNCTION            4 (annotations)
                 56 STORE_NAME               8 (run_acquired_check)
    
-    47          58 LOAD_CONST               7 ('search')
-                60 LOAD_NAME                6 (ts)
+    46          58 LOAD_CONST               7 ('search')
+                60 LOAD_NAME                4 (ts)
                 62 LOAD_ATTR                9 (models)
                 72 LOAD_ATTR               10 (Search)
                 82 LOAD_CONST               5 ('domain')
                 84 LOAD_NAME                7 (str)
                 86 LOAD_CONST               8 ('return')
-                88 LOAD_CONST               4 (None)
+                88 LOAD_CONST               3 (None)
                 90 BUILD_TUPLE              6
-                92 LOAD_CONST               9 (<code object run_similarity_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 47>)
+                92 LOAD_CONST               9 (<code object run_similarity_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 46>)
                 94 MAKE_FUNCTION            4 (annotations)
                 96 STORE_NAME              11 (run_similarity_search)
    
-    58          98 LOAD_CONST               7 ('search')
-               100 LOAD_NAME                6 (ts)
+    57          98 LOAD_CONST               7 ('search')
+               100 LOAD_NAME                4 (ts)
                102 LOAD_ATTR                9 (models)
                112 LOAD_ATTR               10 (Search)
                122 LOAD_CONST               8 ('return')
-               124 LOAD_CONST               4 (None)
+               124 LOAD_CONST               3 (None)
                126 BUILD_TUPLE              4
-               128 LOAD_CONST              10 (<code object run_criteria_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 58>)
+               128 LOAD_CONST              10 (<code object run_criteria_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 57>)
                130 MAKE_FUNCTION            4 (annotations)
                132 STORE_NAME              12 (run_criteria_search)
    
-    71         134 LOAD_CONST               7 ('search')
-               136 LOAD_NAME                6 (ts)
+    70         134 LOAD_CONST               7 ('search')
+               136 LOAD_NAME                4 (ts)
                138 LOAD_ATTR                9 (models)
                148 LOAD_ATTR               10 (Search)
                158 LOAD_CONST              11 ('event')
-               160 LOAD_NAME                6 (ts)
+               160 LOAD_NAME                4 (ts)
                162 LOAD_ATTR                9 (models)
                172 LOAD_ATTR               13 (Event)
                182 LOAD_CONST               8 ('return')
-               184 LOAD_CONST               4 (None)
+               184 LOAD_CONST               3 (None)
                186 BUILD_TUPLE              6
-               188 LOAD_CONST              12 (<code object run_maps_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 71>)
+               188 LOAD_CONST              12 (<code object run_maps_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 70>)
                190 MAKE_FUNCTION            4 (annotations)
                192 STORE_NAME              14 (run_maps_search)
    
-   116         194 LOAD_CONST               7 ('search')
-               196 LOAD_NAME                6 (ts)
+   115         194 LOAD_CONST               7 ('search')
+               196 LOAD_NAME                4 (ts)
                198 LOAD_ATTR                9 (models)
                208 LOAD_ATTR               10 (Search)
                218 LOAD_CONST              11 ('event')
-               220 LOAD_NAME                6 (ts)
+               220 LOAD_NAME                4 (ts)
                222 LOAD_ATTR                9 (models)
                232 LOAD_ATTR               13 (Event)
                242 LOAD_CONST               8 ('return')
-               244 LOAD_CONST               4 (None)
+               244 LOAD_CONST               3 (None)
                246 BUILD_TUPLE              6
-               248 LOAD_CONST              13 (<code object run_google_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 116>)
+               248 LOAD_CONST              13 (<code object run_google_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 115>)
                250 MAKE_FUNCTION            4 (annotations)
                252 STORE_NAME              15 (run_google_search)
    
-   131         254 LOAD_CONST              11 ('event')
-               256 LOAD_NAME                6 (ts)
+   130         254 LOAD_CONST              11 ('event')
+               256 LOAD_NAME                4 (ts)
                258 LOAD_ATTR                9 (models)
                268 LOAD_ATTR               13 (Event)
                278 LOAD_CONST               8 ('return')
-               280 LOAD_CONST               4 (None)
+               280 LOAD_CONST               3 (None)
                282 BUILD_TUPLE              4
-               284 LOAD_CONST              14 (<code object handle_prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 131>)
+               284 LOAD_CONST              14 (<code object handle_prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 130>)
                286 MAKE_FUNCTION            4 (annotations)
                288 STORE_NAME              16 (handle_prompt)
    
    174         290 LOAD_CONST              15 ('company')
-               292 LOAD_NAME                6 (ts)
+               292 LOAD_NAME                4 (ts)
                294 LOAD_ATTR                9 (models)
                304 LOAD_ATTR               17 (Company)
                314 LOAD_CONST               8 ('return')
-               316 LOAD_CONST               4 (None)
+               316 LOAD_CONST               3 (None)
                318 BUILD_TUPLE              4
                320 LOAD_CONST              16 (<code object enrich_with_gpt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 174>)
                322 MAKE_FUNCTION            4 (annotations)
                324 STORE_NAME              18 (enrich_with_gpt)
    
-   207         326 LOAD_CONST              11 ('event')
-               328 LOAD_NAME                6 (ts)
+   208         326 LOAD_CONST              11 ('event')
+               328 LOAD_NAME                4 (ts)
                330 LOAD_ATTR                9 (models)
                340 LOAD_ATTR               13 (Event)
                350 LOAD_CONST               8 ('return')
-               352 LOAD_CONST               4 (None)
+               352 LOAD_CONST               3 (None)
                354 BUILD_TUPLE              4
-               356 LOAD_CONST              17 (<code object run_enrichment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 207>)
+               356 LOAD_CONST              17 (<code object run_enrichment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 208>)
                358 MAKE_FUNCTION            4 (annotations)
                360 STORE_NAME              19 (run_enrichment)
    
-   224         362 LOAD_CONST              18 ('event_id')
+   228         362 LOAD_CONST              18 ('event_id')
                364 LOAD_NAME               20 (int)
                366 LOAD_CONST               8 ('return')
-               368 LOAD_CONST               4 (None)
+               368 LOAD_CONST               3 (None)
                370 BUILD_TUPLE              4
-               372 LOAD_CONST              19 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 224>)
+               372 LOAD_CONST              19 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 228>)
                374 MAKE_FUNCTION            4 (annotations)
                376 STORE_NAME              21 (process_event)
-               378 LOAD_CONST               4 (None)
+               378 LOAD_CONST               3 (None)
                380 RETURN_VALUE
    consts
       0
-      ('time',)
       ('asdict',)
-      ('from_dict',)
+      ('time',)
       None
+      ('from_dict',)
       'domain'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 8
          flags     : 3
          code
@@ -331,43 +331,43 @@
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007c017c00ac01a6020000ab0200
             000000000000007d027400000000000000000000006a0300000000000000
             00a00400000000000000000000000000000000000000007c027c006a0500
             00000000000000640264037c019b009d02ac04a6040000ab040000000000
             000000010064005300
-          47           0 RESUME                   0
+          46           0 RESUME                   0
          
-          48           2 LOAD_GLOBAL              0 (ts)
+          47           2 LOAD_GLOBAL              0 (ts)
                       14 LOAD_ATTR                1 (grata)
                       24 LOAD_METHOD              2 (find_similar)
                       46 LOAD_FAST                1 (domain)
                       48 LOAD_FAST                0 (search)
                       50 KW_NAMES                 1
                       52 PRECALL                  2
                       56 CALL                     2
                       66 STORE_FAST               2 (grata_companies)
          
-          49          68 LOAD_GLOBAL              0 (ts)
+          48          68 LOAD_GLOBAL              0 (ts)
                       80 LOAD_ATTR                3 (query)
                       90 LOAD_METHOD              4 (insert_companies_as_targets)
          
-          50         112 LOAD_FAST                2 (grata_companies)
+          49         112 LOAD_FAST                2 (grata_companies)
          
-          51         114 LOAD_FAST                0 (search)
+          50         114 LOAD_FAST                0 (search)
                      116 LOAD_ATTR                5 (uid)
          
-          52         126 LOAD_CONST               2 ('grata')
+          51         126 LOAD_CONST               2 ('grata')
          
-          54         128 LOAD_CONST               3 ('grata/')
+          53         128 LOAD_CONST               3 ('grata/')
                      130 LOAD_FAST                1 (domain)
                      132 FORMAT_VALUE             0
                      134 BUILD_STRING             2
          
-          49         136 KW_NAMES                 4
+          48         136 KW_NAMES                 4
                      138 PRECALL                  4
                      142 CALL                     4
                      152 POP_TOP
                      154 LOAD_CONST               0 (None)
                      156 RETURN_VALUE
          consts
             None
@@ -377,54 +377,54 @@
             ('companies', 'search_uid', 'actor_key', 'source')
          names      ('ts', 'grata', 'find_similar', 'query', 'insert_companies_as_targets', 'uid')
          varnames   ('search', 'domain', 'grata_companies')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_similarity_search'
-         firstlineno 47
+         firstlineno 46
          lnotab 0x020142012c0102010c01020208fb
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007c00a6010000ab010000000000
             0000007d017400000000000000000000006a030000000000000000a00400
             000000000000000000000000000000000000007c017c006a050000000000
             000000640164026401ac03a6050000ab0500000000000000000100640053
             00
-          58           0 RESUME                   0
+          57           0 RESUME                   0
          
-          61           2 LOAD_GLOBAL              0 (ts)
+          60           2 LOAD_GLOBAL              0 (ts)
                       14 LOAD_ATTR                1 (grata)
                       24 LOAD_METHOD              2 (find_by_criteria)
                       46 LOAD_FAST                0 (search)
                       48 PRECALL                  1
                       52 CALL                     1
                       62 STORE_FAST               1 (grata_companies)
          
-          62          64 LOAD_GLOBAL              0 (ts)
+          61          64 LOAD_GLOBAL              0 (ts)
                       76 LOAD_ATTR                3 (query)
                       86 LOAD_METHOD              4 (insert_companies_as_targets)
          
-          63         108 LOAD_FAST                1 (grata_companies)
+          62         108 LOAD_FAST                1 (grata_companies)
          
-          64         110 LOAD_FAST                0 (search)
+          63         110 LOAD_FAST                0 (search)
                      112 LOAD_ATTR                5 (uid)
          
-          65         122 LOAD_CONST               1 ('grata')
+          64         122 LOAD_CONST               1 ('grata')
          
-          66         124 LOAD_CONST               2 (True)
+          65         124 LOAD_CONST               2 (True)
          
-          67         126 LOAD_CONST               1 ('grata')
+          66         126 LOAD_CONST               1 ('grata')
          
-          62         128 KW_NAMES                 3
+          61         128 KW_NAMES                 3
                      130 PRECALL                  5
                      134 CALL                     5
                      144 POP_TOP
                      146 LOAD_CONST               0 (None)
                      148 RETURN_VALUE
          consts
             None
@@ -433,15 +433,15 @@
             ('companies', 'search_uid', 'actor_key', 'force', 'source')
          names      ('ts', 'grata', 'find_by_criteria', 'query', 'insert_companies_as_targets', 'uid')
          varnames   ('search', 'grata_companies')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_criteria_search'
-         firstlineno 58
+         firstlineno 57
          lnotab 0x02033e012c0102010c010201020102fb
       'event'
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 6
          flags     : 3
@@ -458,92 +458,92 @@
             0100000000000000007d047417000000000000000000007c04a6010000ab
             01000000000000000001007c04640319000000000000000000a00c000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             0044005d0f7d0502007c027c057c00ac09a6020000ab0200000000000000
             0001008c1064005300
                        0 MAKE_CELL                6 (existing_search_domains)
          
-          71           2 RESUME                   0
+          70           2 RESUME                   0
          
-          72           4 LOAD_GLOBAL              0 (ts)
+          71           4 LOAD_GLOBAL              0 (ts)
                       16 LOAD_ATTR                1 (query)
                       26 LOAD_METHOD              2 (search_targets)
                       48 LOAD_FAST                0 (search)
                       50 LOAD_ATTR                3 (uid)
                       60 KW_NAMES                 1
                       62 PRECALL                  1
                       66 CALL                     1
          
-          73          76 LOAD_CONST               2 ('domain')
+          72          76 LOAD_CONST               2 ('domain')
          
-          72          78 BINARY_SUBSCR
+          71          78 BINARY_SUBSCR
          
-          74          88 LOAD_METHOD              4 (to_list)
+          73          88 LOAD_METHOD              4 (to_list)
                      110 PRECALL                  0
                      114 CALL                     0
          
-          72         124 STORE_DEREF              6 (existing_search_domains)
+          71         124 STORE_DEREF              6 (existing_search_domains)
          
-          76         126 LOAD_CONST               3 ('place_id')
+          75         126 LOAD_CONST               3 ('place_id')
                      128 LOAD_GLOBAL             10 (str)
                      140 LOAD_CONST               4 ('search')
                      142 LOAD_GLOBAL              0 (ts)
                      154 LOAD_ATTR                6 (models)
                      164 LOAD_ATTR                7 (Search)
                      174 LOAD_CONST               5 ('return')
                      176 LOAD_CONST               0 (None)
                      178 BUILD_TUPLE              6
                      180 LOAD_CLOSURE             6 (existing_search_domains)
                      182 BUILD_TUPLE              1
-                     184 LOAD_CONST               6 (<code object build_place, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 76>)
+                     184 LOAD_CONST               6 (<code object build_place, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 75>)
                      186 MAKE_FUNCTION           12 (annotations, closure)
                      188 STORE_FAST               2 (build_place)
          
-         107         190 LOAD_FAST                1 (event)
+         106         190 LOAD_FAST                1 (event)
                      192 LOAD_ATTR                8 (data)
                      202 LOAD_CONST               7 ('query')
                      204 BINARY_SUBSCR
                      214 STORE_FAST               3 (q)
          
-         108         216 LOAD_GLOBAL              0 (ts)
+         107         216 LOAD_GLOBAL              0 (ts)
                      228 LOAD_ATTR                9 (google)
                      238 LOAD_METHOD             10 (get_google_places)
                      260 LOAD_FAST                3 (q)
                      262 KW_NAMES                 8
                      264 PRECALL                  1
                      268 CALL                     1
                      278 STORE_FAST               4 (results)
          
-         109         280 LOAD_GLOBAL             23 (NULL + print)
+         108         280 LOAD_GLOBAL             23 (NULL + print)
                      292 LOAD_FAST                4 (results)
                      294 PRECALL                  1
                      298 CALL                     1
                      308 POP_TOP
          
-         112         310 LOAD_FAST                4 (results)
+         111         310 LOAD_FAST                4 (results)
                      312 LOAD_CONST               3 ('place_id')
                      314 BINARY_SUBSCR
                      324 LOAD_METHOD             12 (tolist)
                      346 PRECALL                  0
                      350 CALL                     0
                      360 GET_ITER
                  >>  362 FOR_ITER                15 (to 394)
                      364 STORE_FAST               5 (place)
          
-         113         366 PUSH_NULL
+         112         366 PUSH_NULL
                      368 LOAD_FAST                2 (build_place)
                      370 LOAD_FAST                5 (place)
                      372 LOAD_FAST                0 (search)
                      374 KW_NAMES                 9
                      376 PRECALL                  2
                      380 CALL                     2
                      390 POP_TOP
                      392 JUMP_BACKWARD           16 (to 362)
          
-         112     >>  394 LOAD_CONST               0 (None)
+         111     >>  394 LOAD_CONST               0 (None)
                      396 RETURN_VALUE
          consts
             None
             ('search_uid',)
             'domain'
             'place_id'
             'search'
@@ -574,131 +574,131 @@
                   000000000000007c016a0f0000000000000000640a7c066a0d0000000000
                   000000640b640c7c036901ac0da6050000ab0500000000000000007d0774
                   00000000000000000000006a0a0000000000000000a01000000000000000
                   000000000000000000000000007c07a6010000ab01000000000000000001
                   0064005300
                              0 COPY_FREE_VARS           1
                
-                76           2 RESUME                   0
+                75           2 RESUME                   0
                
-                77           4 LOAD_GLOBAL              0 (ts)
+                76           4 LOAD_GLOBAL              0 (ts)
                             16 LOAD_ATTR                1 (google)
                             26 LOAD_ATTR                2 (gmaps)
                             36 LOAD_METHOD              3 (place)
                
-                78          58 LOAD_FAST                0 (place_id)
+                77          58 LOAD_FAST                0 (place_id)
                             60 BUILD_LIST               0
                             62 LOAD_CONST               1 (('name', 'website', 'reviews'))
                             64 LIST_EXTEND              1
                
-                77          66 KW_NAMES                 2
+                76          66 KW_NAMES                 2
                             68 PRECALL                  2
                             72 CALL                     2
                             82 STORE_FAST               2 (resp)
                
-                80          84 LOAD_FAST                2 (resp)
+                79          84 LOAD_FAST                2 (resp)
                             86 LOAD_CONST               3 ('result')
                             88 BINARY_SUBSCR
                             98 STORE_FAST               3 (place)
                
-                81         100 LOAD_GLOBAL              0 (ts)
+                80         100 LOAD_GLOBAL              0 (ts)
                            112 LOAD_ATTR                4 (helpers)
                            122 LOAD_METHOD              5 (clean_domain)
                            144 LOAD_FAST                3 (place)
                            146 LOAD_METHOD              6 (get)
                            168 LOAD_CONST               4 ('website')
                            170 PRECALL                  1
                            174 CALL                     1
                            184 PRECALL                  1
                            188 CALL                     1
                            198 STORE_FAST               4 (domain)
                
-                82         200 LOAD_FAST                4 (domain)
+                81         200 LOAD_FAST                4 (domain)
                            202 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 208)
                
-                83         204 LOAD_CONST               0 (None)
+                82         204 LOAD_CONST               0 (None)
                            206 RETURN_VALUE
                
-                84     >>  208 LOAD_FAST                4 (domain)
+                83     >>  208 LOAD_FAST                4 (domain)
                            210 LOAD_DEREF               8 (existing_search_domains)
                            212 CONTAINS_OP              0
                            214 POP_JUMP_FORWARD_IF_FALSE    21 (to 258)
                
-                85         216 LOAD_GLOBAL             15 (NULL + print)
+                84         216 LOAD_GLOBAL             15 (NULL + print)
                            228 LOAD_CONST               5 ('domain ')
                            230 LOAD_FAST                4 (domain)
                            232 FORMAT_VALUE             0
                            234 LOAD_CONST               6 (' already in search. skipping...')
                            236 BUILD_STRING             3
                            238 PRECALL                  1
                            242 CALL                     1
                            252 POP_TOP
                
-                86         254 LOAD_CONST               0 (None)
+                85         254 LOAD_CONST               0 (None)
                            256 RETURN_VALUE
                
-                87     >>  258 LOAD_GLOBAL              0 (ts)
+                86     >>  258 LOAD_GLOBAL              0 (ts)
                            270 LOAD_ATTR                8 (models)
                            280 LOAD_METHOD              9 (Company)
                
-                88         302 LOAD_FAST                3 (place)
+                87         302 LOAD_FAST                3 (place)
                            304 LOAD_CONST               7 ('name')
                            306 BINARY_SUBSCR
                
-                89         316 LOAD_FAST                4 (domain)
+                88         316 LOAD_FAST                4 (domain)
                
-                90         318 LOAD_CONST               8 ('Map API')
+                89         318 LOAD_CONST               8 ('Map API')
                
-                87         320 KW_NAMES                 9
+                86         320 KW_NAMES                 9
                            322 PRECALL                  3
                            326 CALL                     3
                            336 STORE_FAST               5 (new_company)
                
-                92         338 LOAD_GLOBAL              0 (ts)
+                91         338 LOAD_GLOBAL              0 (ts)
                            350 LOAD_ATTR               10 (query)
                            360 LOAD_METHOD             11 (insert_company)
                            382 LOAD_FAST                5 (new_company)
                            384 PRECALL                  1
                            388 CALL                     1
                            398 POP_TOP
                
-                93         400 LOAD_GLOBAL              0 (ts)
+                92         400 LOAD_GLOBAL              0 (ts)
                            412 LOAD_ATTR               10 (query)
                            422 LOAD_METHOD             12 (find_company_by_domain)
                            444 LOAD_FAST                5 (new_company)
                            446 LOAD_ATTR               13 (domain)
                            456 PRECALL                  1
                            460 CALL                     1
                            470 STORE_FAST               6 (company)
                
-                95         472 LOAD_GLOBAL              0 (ts)
+                94         472 LOAD_GLOBAL              0 (ts)
                            484 LOAD_ATTR                8 (models)
                            494 LOAD_METHOD             14 (Event)
                
-                96         516 LOAD_FAST                1 (search)
+                95         516 LOAD_FAST                1 (search)
                            518 LOAD_ATTR               15 (uid)
                
-                97         528 LOAD_CONST              10 ('create')
+                96         528 LOAD_CONST              10 ('create')
                
-                98         530 LOAD_FAST                6 (company)
+                97         530 LOAD_FAST                6 (company)
                            532 LOAD_ATTR               13 (domain)
                
-                99         542 LOAD_CONST              11 ('google')
+                98         542 LOAD_CONST              11 ('google')
                
-               101         544 LOAD_CONST              12 ('place')
+               100         544 LOAD_CONST              12 ('place')
                            546 LOAD_FAST                3 (place)
                
-               100         548 BUILD_MAP                1
+                99         548 BUILD_MAP                1
                
-                95         550 KW_NAMES                13
+                94         550 KW_NAMES                13
                            552 PRECALL                  5
                            556 CALL                     5
                            566 STORE_FAST               7 (event)
                
-               105         568 LOAD_GLOBAL              0 (ts)
+               104         568 LOAD_GLOBAL              0 (ts)
                            580 LOAD_ATTR               10 (query)
                            590 LOAD_METHOD             16 (insert_event)
                            612 LOAD_FAST                7 (event)
                            614 PRECALL                  1
                            618 CALL                     1
                            628 POP_TOP
                            630 LOAD_CONST               0 (None)
@@ -720,28 +720,28 @@
                   ('search_uid', 'type', 'domain', 'actor_key', 'data')
                names      ('ts', 'google', 'gmaps', 'place', 'helpers', 'clean_domain', 'get', 'print', 'models', 'Company', 'query', 'insert_company', 'find_company_by_domain', 'domain', 'Event', 'uid', 'insert_event')
                varnames   ('place_id', 'search', 'resp', 'place', 'domain', 'new_company', 'company', 'event')
                freevars   ('existing_search_domains',)
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
                name       'build_place'
-               firstlineno 76
+               firstlineno 75
                lnotab
                   0x0401360108ff120310016401040104010801260104012c010e01020102
                   fd12053e0148022c010c0102010c01020204ff02fb120a
             'query'
             ('q',)
             ('place_id', 'search')
          names      ('ts', 'query', 'search_targets', 'uid', 'to_list', 'str', 'models', 'Search', 'data', 'google', 'get_google_places', 'print', 'tolist')
          varnames   ('search', 'event', 'build_place', 'q', 'results', 'place')
          freevars   ()
          cellvars   ('existing_search_domains',)
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_maps_search'
-         firstlineno 71
+         firstlineno 70
          lnotab 0x0401480102ff0a0224fe0204401f1a0140011e0338011cff
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 7
          flags     : 3
          code
@@ -758,36 +758,36 @@
             00ab0100000000000000007d037411000000000000000000007c03a60100
             00ab01000000000000000001007404000000000000000000006a09000000
             0000000000a00a00000000000000000000000000000000000000007c0364
             09640b670219000000000000000000a00b00000000000000000000000000
             00000000000000640dac0ea6010000ab0100000000000000007c016a0c00
             000000000000007c016a0d0000000000000000640fac10a6040000ab0400
             00000000000000010064005300
-         116           0 RESUME                   0
+         115           0 RESUME                   0
          
-         117           2 LOAD_FAST                1 (event)
+         116           2 LOAD_FAST                1 (event)
                        4 LOAD_ATTR                0 (data)
                       14 LOAD_CONST               1 ('q')
                       16 BINARY_SUBSCR
                       26 STORE_FAST               2 (q)
          
-         118          28 LOAD_GLOBAL              3 (NULL + len)
+         117          28 LOAD_GLOBAL              3 (NULL + len)
                       40 LOAD_FAST                2 (q)
                       42 PRECALL                  1
                       46 CALL                     1
                       56 LOAD_CONST               2 (0)
                       58 COMPARE_OP               4 (>)
                       64 POP_JUMP_FORWARD_IF_TRUE    10 (to 86)
                       66 LOAD_ASSERTION_ERROR
                       68 LOAD_CONST               3 ('q must be a non-empty string')
                       70 PRECALL                  0
                       74 CALL                     0
                       84 RAISE_VARARGS            1
          
-         119     >>   86 LOAD_GLOBAL              4 (ts)
+         118     >>   86 LOAD_GLOBAL              4 (ts)
                       98 LOAD_ATTR                3 (google)
                      108 LOAD_METHOD              4 (search)
                      130 LOAD_FAST                2 (q)
                      132 LOAD_FAST                1 (event)
                      134 LOAD_ATTR                0 (data)
                      144 LOAD_METHOD              5 (get)
                      166 LOAD_CONST               4 ('count')
@@ -795,66 +795,66 @@
                      170 PRECALL                  2
                      174 CALL                     2
                      184 KW_NAMES                 6
                      186 PRECALL                  2
                      190 CALL                     2
                      200 STORE_FAST               3 (results)
          
-         120         202 LOAD_FAST                3 (results)
+         119         202 LOAD_FAST                3 (results)
                      204 LOAD_CONST               7 ('link')
                      206 BINARY_SUBSCR
                      216 LOAD_METHOD              6 (apply)
-                     238 LOAD_CONST               8 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 120>)
+                     238 LOAD_CONST               8 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 119>)
                      240 MAKE_FUNCTION            0
                      242 PRECALL                  1
                      246 CALL                     1
                      256 LOAD_FAST                3 (results)
                      258 LOAD_CONST               9 ('domain')
                      260 STORE_SUBSCR
          
-         121         264 LOAD_FAST                3 (results)
+         120         264 LOAD_FAST                3 (results)
                      266 LOAD_METHOD              7 (rename)
                      288 LOAD_CONST              10 ('snippet')
                      290 LOAD_CONST              11 ('description')
                      292 BUILD_MAP                1
                      294 KW_NAMES                12
                      296 PRECALL                  1
                      300 CALL                     1
                      310 STORE_FAST               3 (results)
          
-         122         312 LOAD_GLOBAL             17 (NULL + print)
+         121         312 LOAD_GLOBAL             17 (NULL + print)
                      324 LOAD_FAST                3 (results)
                      326 PRECALL                  1
                      330 CALL                     1
                      340 POP_TOP
          
-         123         342 LOAD_GLOBAL              4 (ts)
+         122         342 LOAD_GLOBAL              4 (ts)
                      354 LOAD_ATTR                9 (query)
                      364 LOAD_METHOD             10 (insert_companies_as_targets)
          
-         124         386 LOAD_FAST                3 (results)
+         123         386 LOAD_FAST                3 (results)
                      388 LOAD_CONST               9 ('domain')
                      390 LOAD_CONST              11 ('description')
                      392 BUILD_LIST               2
                      394 BINARY_SUBSCR
                      404 LOAD_METHOD             11 (to_dict)
                      426 LOAD_CONST              13 ('records')
                      428 KW_NAMES                14
                      430 PRECALL                  1
                      434 CALL                     1
          
-         125         444 LOAD_FAST                1 (event)
+         124         444 LOAD_FAST                1 (event)
                      446 LOAD_ATTR               12 (search_uid)
          
-         126         456 LOAD_FAST                1 (event)
+         125         456 LOAD_FAST                1 (event)
                      458 LOAD_ATTR               13 (actor_key)
          
-         127         468 LOAD_CONST              15 ('Google')
+         126         468 LOAD_CONST              15 ('Google')
          
-         123         470 KW_NAMES                16
+         122         470 KW_NAMES                16
                      472 PRECALL                  4
                      476 CALL                     4
                      486 POP_TOP
                      488 LOAD_CONST               0 (None)
                      490 RETURN_VALUE
          consts
             None
@@ -870,15 +870,15 @@
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c00a6010000ab010000000000
                   0000005300
-               120           0 RESUME                   0
+               119           0 RESUME                   0
                              2 LOAD_GLOBAL              0 (ts)
                             14 LOAD_ATTR                1 (helpers)
                             24 LOAD_METHOD              2 (clean_domain)
                             46 LOAD_FAST                0 (x)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 RETURN_VALUE
@@ -886,15 +886,15 @@
                   None
                names      ('ts', 'helpers', 'clean_domain')
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
                name       '<lambda>'
-               firstlineno 120
+               firstlineno 119
                lnotab 0x
             'domain'
             'snippet'
             'description'
             ('columns',)
             'records'
             ('orient',)
@@ -902,15 +902,15 @@
             ('companies', 'search_uid', 'actor_key', 'source')
          names      ('data', 'len', 'ts', 'google', 'search', 'get', 'apply', 'rename', 'print', 'query', 'insert_companies_as_targets', 'to_dict', 'search_uid', 'actor_key')
          varnames   ('search', 'event', 'q', 'results')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_google_search'
-         firstlineno 116
+         firstlineno 115
          lnotab 0x02011a013a0174013e0130011e012c013a010c010c0102fc
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 10
          flags     : 3
          code
@@ -932,163 +932,163 @@
             007419000000000000000000007402000000000000000000006a0d000000
             00000000006a0e00000000000000007c03a6020000ab0200000000000000
             007d047401000000000000000000007c04a6010000ab0100000000000000
             0001007c006a0a00000000000000006407190000000000000000007c046a
             0a000000000000000064073c0000007402000000000000000000006a0f00
             00000000000000a01000000000000000000000000000000000000000007c
             04a6010000ab01000000000000000001008c7564005300
-         131           0 RESUME                   0
+         130           0 RESUME                   0
          
-         132           2 LOAD_GLOBAL              1 (NULL + print)
+         131           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('prompt event:')
                       16 LOAD_FAST                0 (event)
                       18 PRECALL                  2
                       22 CALL                     2
                       32 POP_TOP
          
-         135          34 LOAD_CONST               2 ('system')
+         134          34 LOAD_CONST               2 ('system')
          
-         136          36 LOAD_GLOBAL              2 (ts)
+         135          36 LOAD_GLOBAL              2 (ts)
                       48 LOAD_ATTR                2 (gpt)
                       58 LOAD_ATTR                3 (HOW_TO_RESPOND)
          
-         134          68 LOAD_CONST               3 (('role', 'content'))
+         133          68 LOAD_CONST               3 (('role', 'content'))
                       70 BUILD_CONST_KEY_MAP      2
          
-         139          72 LOAD_CONST               2 ('system')
+         138          72 LOAD_CONST               2 ('system')
          
-         140          74 LOAD_GLOBAL              2 (ts)
+         139          74 LOAD_GLOBAL              2 (ts)
                       86 LOAD_ATTR                2 (gpt)
                       96 LOAD_ATTR                4 (HOW_TO_IMPORT)
          
-         138         106 LOAD_CONST               3 (('role', 'content'))
+         137         106 LOAD_CONST               3 (('role', 'content'))
                      108 BUILD_CONST_KEY_MAP      2
          
-         143         110 LOAD_CONST               2 ('system')
+         142         110 LOAD_CONST               2 ('system')
          
-         144         112 LOAD_GLOBAL              2 (ts)
+         143         112 LOAD_GLOBAL              2 (ts)
                      124 LOAD_ATTR                2 (gpt)
                      134 LOAD_ATTR                5 (HOW_TO_TRANSITION)
          
-         142         144 LOAD_CONST               3 (('role', 'content'))
+         141         144 LOAD_CONST               3 (('role', 'content'))
                      146 BUILD_CONST_KEY_MAP      2
          
-         147         148 LOAD_CONST               2 ('system')
+         146         148 LOAD_CONST               2 ('system')
          
-         148         150 LOAD_GLOBAL              2 (ts)
+         147         150 LOAD_GLOBAL              2 (ts)
                      162 LOAD_ATTR                2 (gpt)
                      172 LOAD_ATTR                6 (HOW_TO_GOOGLE)
          
-         146         182 LOAD_CONST               3 (('role', 'content'))
+         145         182 LOAD_CONST               3 (('role', 'content'))
                      184 BUILD_CONST_KEY_MAP      2
          
-         151         186 LOAD_CONST               2 ('system')
+         150         186 LOAD_CONST               2 ('system')
          
-         152         188 LOAD_GLOBAL              2 (ts)
+         151         188 LOAD_GLOBAL              2 (ts)
                      200 LOAD_ATTR                2 (gpt)
                      210 LOAD_ATTR                7 (HOW_TO_GOOGLE_MAPS)
          
-         150         220 LOAD_CONST               3 (('role', 'content'))
+         149         220 LOAD_CONST               3 (('role', 'content'))
                      222 BUILD_CONST_KEY_MAP      2
          
-         155         224 LOAD_CONST               2 ('system')
+         154         224 LOAD_CONST               2 ('system')
          
-         156         226 LOAD_CONST               4 ('the search_uid is ')
+         155         226 LOAD_CONST               4 ('the search_uid is ')
                      228 LOAD_FAST                0 (event)
                      230 LOAD_ATTR                8 (search_uid)
                      240 FORMAT_VALUE             0
                      242 BUILD_STRING             2
          
-         154         244 LOAD_CONST               3 (('role', 'content'))
+         153         244 LOAD_CONST               3 (('role', 'content'))
                      246 BUILD_CONST_KEY_MAP      2
          
-         159         248 LOAD_CONST               2 ('system')
+         158         248 LOAD_CONST               2 ('system')
          
-         160         250 LOAD_CONST               5 ('the actor_key is ')
+         159         250 LOAD_CONST               5 ('the actor_key is ')
                      252 LOAD_FAST                0 (event)
                      254 LOAD_ATTR                9 (actor_key)
                      264 FORMAT_VALUE             0
                      266 BUILD_STRING             2
          
-         158         268 LOAD_CONST               3 (('role', 'content'))
+         157         268 LOAD_CONST               3 (('role', 'content'))
                      270 BUILD_CONST_KEY_MAP      2
          
-         162         272 LOAD_CONST               6 ('user')
+         161         272 LOAD_CONST               6 ('user')
                      274 LOAD_FAST                0 (event)
                      276 LOAD_ATTR               10 (data)
                      286 LOAD_CONST               7 ('prompt')
                      288 BINARY_SUBSCR
                      298 LOAD_CONST               3 (('role', 'content'))
                      300 BUILD_CONST_KEY_MAP      2
          
-         133         302 BUILD_LIST               8
+         132         302 BUILD_LIST               8
                      304 STORE_FAST               1 (messages)
          
-         164         306 LOAD_GLOBAL              2 (ts)
+         163         306 LOAD_GLOBAL              2 (ts)
                      318 LOAD_ATTR                2 (gpt)
                      328 LOAD_METHOD             11 (ask_gpt4)
                      350 LOAD_FAST                1 (messages)
                      352 PRECALL                  1
                      356 CALL                     1
                      366 STORE_FAST               2 (resp)
          
-         166         368 LOAD_GLOBAL              1 (NULL + print)
+         165         368 LOAD_GLOBAL              1 (NULL + print)
                      380 LOAD_FAST                2 (resp)
                      382 PRECALL                  1
                      386 CALL                     1
                      396 POP_TOP
          
-         167         398 LOAD_FAST                2 (resp)
+         166         398 LOAD_FAST                2 (resp)
                      400 LOAD_CONST               8 ('events')
                      402 BINARY_SUBSCR
                      412 GET_ITER
                  >>  414 FOR_ITER               116 (to 648)
                      416 STORE_FAST               3 (new_event)
          
-         168         418 LOAD_GLOBAL              1 (NULL + print)
+         167         418 LOAD_GLOBAL              1 (NULL + print)
                      430 LOAD_CONST               9 ('new event:')
                      432 LOAD_FAST                3 (new_event)
                      434 PRECALL                  2
                      438 CALL                     2
                      448 POP_TOP
          
-         169         450 LOAD_GLOBAL             25 (NULL + from_dict)
+         168         450 LOAD_GLOBAL             25 (NULL + from_dict)
                      462 LOAD_GLOBAL              2 (ts)
                      474 LOAD_ATTR               13 (models)
                      484 LOAD_ATTR               14 (Event)
                      494 LOAD_FAST                3 (new_event)
                      496 PRECALL                  2
                      500 CALL                     2
                      510 STORE_FAST               4 (e)
          
-         170         512 LOAD_GLOBAL              1 (NULL + print)
+         169         512 LOAD_GLOBAL              1 (NULL + print)
                      524 LOAD_FAST                4 (e)
                      526 PRECALL                  1
                      530 CALL                     1
                      540 POP_TOP
          
-         171         542 LOAD_FAST                0 (event)
+         170         542 LOAD_FAST                0 (event)
                      544 LOAD_ATTR               10 (data)
                      554 LOAD_CONST               7 ('prompt')
                      556 BINARY_SUBSCR
                      566 LOAD_FAST                4 (e)
                      568 LOAD_ATTR               10 (data)
                      578 LOAD_CONST               7 ('prompt')
                      580 STORE_SUBSCR
          
-         172         584 LOAD_GLOBAL              2 (ts)
+         171         584 LOAD_GLOBAL              2 (ts)
                      596 LOAD_ATTR               15 (query)
                      606 LOAD_METHOD             16 (insert_event)
                      628 LOAD_FAST                4 (e)
                      630 PRECALL                  1
                      634 CALL                     1
                      644 POP_TOP
                      646 JUMP_BACKWARD          117 (to 414)
          
-         167     >>  648 LOAD_CONST               0 (None)
+         166     >>  648 LOAD_CONST               0 (None)
                      650 RETURN_VALUE
          consts
             None
             'prompt event:'
             'system'
             ('role', 'content')
             'the search_uid is '
@@ -1099,15 +1099,15 @@
             'new event:'
          names      ('print', 'ts', 'gpt', 'HOW_TO_RESPOND', 'HOW_TO_IMPORT', 'HOW_TO_TRANSITION', 'HOW_TO_GOOGLE', 'HOW_TO_GOOGLE_MAPS', 'search_uid', 'actor_key', 'data', 'ask_gpt4', 'from_dict', 'models', 'Event', 'query', 'insert_event')
          varnames   ('event', 'messages', 'resp', 'new_event', 'e')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'handle_prompt'
-         firstlineno 131
+         firstlineno 130
          lnotab
             0x02012003020120fe0405020120fe0405020120fe0405020120fe040502
             0120fe0405020112fe0405020112fe04041ee3041f3e021e01140120013e
             011e012a0140fb
       'company'
       code
          argcount  : 1
@@ -1287,117 +1287,138 @@
             000000000000007d047c036a0a000000000000000070147c04a006000000
             00000000000000000000000000000000006403a6010000ab010000000000
             0000007c035f0a00000000000000007c04a0060000000000000000000000
             0000000000000000006404a6010000ab0100000000000000007c035f0b00
             0000000000000069007c036a050000000000000000a5017c04a5017c035f
             0500000000000000007404000000000000000000006a0300000000000000
             00a00c00000000000000000000000000000000000000007c03a6010000ab
-            0100000000000000000100741b000000000000000000007c03ac05a60100
-            00ab010000000000000000010064005300
-         207           0 RESUME                   0
+            01000000000000000001007c036a050000000000000000a0060000000000
+            0000000000000000000000000000006405a6010000ab0100000000000000
+            007211740f000000000000000000006406a6010000ab0100000000000000
+            00010064005300741b000000000000000000007c03ac07a6010000ab0100
+            00000000000000010064005300
+         208           0 RESUME                   0
          
-         208           2 LOAD_FAST                0 (event)
+         209           2 LOAD_FAST                0 (event)
                        4 LOAD_ATTR                0 (domain)
                       14 STORE_FAST               1 (domain)
          
-         209          16 LOAD_FAST                0 (event)
+         210          16 LOAD_FAST                0 (event)
                       18 LOAD_ATTR                1 (search_uid)
                       28 STORE_FAST               2 (search_uid)
          
-         211          30 LOAD_GLOBAL              4 (ts)
+         212          30 LOAD_GLOBAL              4 (ts)
                       42 LOAD_ATTR                3 (query)
                       52 LOAD_METHOD              4 (find_company_by_domain)
                       74 LOAD_FAST                1 (domain)
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               3 (company)
          
-         212          92 LOAD_FAST                3 (company)
+         213          92 LOAD_FAST                3 (company)
                       94 LOAD_ATTR                5 (meta)
                      104 LOAD_METHOD              6 (get)
                      126 LOAD_CONST               1 ('company_uid')
                      128 PRECALL                  1
                      132 CALL                     1
                      142 POP_JUMP_FORWARD_IF_FALSE    16 (to 176)
          
-         213         144 LOAD_GLOBAL             15 (NULL + print)
+         214         144 LOAD_GLOBAL             15 (NULL + print)
                      156 LOAD_CONST               2 ('company already exists. skipping enrichment...')
                      158 PRECALL                  1
                      162 CALL                     1
                      172 POP_TOP
                      174 JUMP_FORWARD           142 (to 460)
          
-         215     >>  176 LOAD_GLOBAL              4 (ts)
+         216     >>  176 LOAD_GLOBAL              4 (ts)
                      188 LOAD_ATTR                8 (grata)
                      198 LOAD_METHOD              9 (enrich)
                      220 LOAD_FAST                3 (company)
                      222 LOAD_ATTR                0 (domain)
                      232 PRECALL                  1
                      236 CALL                     1
                      246 STORE_FAST               4 (resp)
          
-         216         248 LOAD_FAST                3 (company)
+         217         248 LOAD_FAST                3 (company)
                      250 LOAD_ATTR               10 (name)
                      260 JUMP_IF_TRUE_OR_POP     20 (to 302)
                      262 LOAD_FAST                4 (resp)
                      264 LOAD_METHOD              6 (get)
                      286 LOAD_CONST               3 ('name')
                      288 PRECALL                  1
                      292 CALL                     1
                  >>  302 LOAD_FAST                3 (company)
                      304 STORE_ATTR              10 (name)
          
-         217         314 LOAD_FAST                4 (resp)
+         218         314 LOAD_FAST                4 (resp)
                      316 LOAD_METHOD              6 (get)
                      338 LOAD_CONST               4 ('description')
                      340 PRECALL                  1
                      344 CALL                     1
                      354 LOAD_FAST                3 (company)
                      356 STORE_ATTR              11 (description)
          
-         218         366 BUILD_MAP                0
+         219         366 BUILD_MAP                0
                      368 LOAD_FAST                3 (company)
                      370 LOAD_ATTR                5 (meta)
                      380 DICT_UPDATE              1
                      382 LOAD_FAST                4 (resp)
                      384 DICT_UPDATE              1
                      386 LOAD_FAST                3 (company)
                      388 STORE_ATTR               5 (meta)
          
-         219         398 LOAD_GLOBAL              4 (ts)
+         220         398 LOAD_GLOBAL              4 (ts)
                      410 LOAD_ATTR                3 (query)
                      420 LOAD_METHOD             12 (update_company)
                      442 LOAD_FAST                3 (company)
                      444 PRECALL                  1
                      448 CALL                     1
                      458 POP_TOP
          
-         221     >>  460 LOAD_GLOBAL             27 (NULL + enrich_with_gpt)
-                     472 LOAD_FAST                3 (company)
-                     474 KW_NAMES                 5
-                     476 PRECALL                  1
-                     480 CALL                     1
-                     490 POP_TOP
-                     492 LOAD_CONST               0 (None)
-                     494 RETURN_VALUE
+         222     >>  460 LOAD_FAST                3 (company)
+                     462 LOAD_ATTR                5 (meta)
+                     472 LOAD_METHOD              6 (get)
+                     494 LOAD_CONST               5 ('gpt')
+                     496 PRECALL                  1
+                     500 CALL                     1
+                     510 POP_JUMP_FORWARD_IF_FALSE    17 (to 546)
+         
+         223         512 LOAD_GLOBAL             15 (NULL + print)
+                     524 LOAD_CONST               6 ('company already enriched with gpt. skipping...')
+                     526 PRECALL                  1
+                     530 CALL                     1
+                     540 POP_TOP
+                     542 LOAD_CONST               0 (None)
+                     544 RETURN_VALUE
+         
+         225     >>  546 LOAD_GLOBAL             27 (NULL + enrich_with_gpt)
+                     558 LOAD_FAST                3 (company)
+                     560 KW_NAMES                 7
+                     562 PRECALL                  1
+                     566 CALL                     1
+                     576 POP_TOP
+                     578 LOAD_CONST               0 (None)
+                     580 RETURN_VALUE
          consts
             None
             'company_uid'
             'company already exists. skipping enrichment...'
             'name'
             'description'
+            'gpt'
+            'company already enriched with gpt. skipping...'
             ('company',)
          names      ('domain', 'search_uid', 'ts', 'query', 'find_company_by_domain', 'meta', 'get', 'print', 'grata', 'enrich', 'name', 'description', 'update_company', 'enrich_with_gpt')
          varnames   ('event', 'domain', 'search_uid', 'company', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_enrichment'
-         firstlineno 207
-         lnotab 0x02010e010e023e013401200248014201340120013e02
+         firstlineno 208
+         lnotab 0x02010e010e023e013401200248014201340120013e0234012202
       'event_id'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 9
          flags     : 3
          code
@@ -1486,593 +1507,593 @@
             0000000000000001007402000000000000000000006a0200000000000000
             00a014000000000000000000000000000000000000000074020000000000
             00000000006a150000000000000000a01600000000000000000000000000
             000000000000007c026a1300000000000000007c037c016a0d0000000000
             000000642a190000000000000000007c016a170000000000000000ac2ba6
             040000ab040000000000000000a6010000ab01000000000000000001008c
             686400530064005300
-         224           0 RESUME                   0
+         228           0 RESUME                   0
          
-         225           2 LOAD_GLOBAL              1 (NULL + print)
+         229           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('processing event...')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-         226          32 LOAD_GLOBAL              2 (ts)
+         230          32 LOAD_GLOBAL              2 (ts)
                       44 LOAD_ATTR                2 (query)
                       54 LOAD_METHOD              3 (find_event_by_id)
                       76 LOAD_FAST                0 (event_id)
                       78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               1 (event)
          
-         227          94 LOAD_GLOBAL              1 (NULL + print)
+         231          94 LOAD_GLOBAL              1 (NULL + print)
                      106 LOAD_CONST               2 ('event_id')
                      108 LOAD_FAST                0 (event_id)
                      110 PRECALL                  2
                      114 CALL                     2
                      124 POP_TOP
          
-         228         126 LOAD_GLOBAL              1 (NULL + print)
+         232         126 LOAD_GLOBAL              1 (NULL + print)
                      138 LOAD_FAST                1 (event)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 POP_TOP
          
-         229         156 LOAD_GLOBAL              2 (ts)
+         233         156 LOAD_GLOBAL              2 (ts)
                      168 LOAD_ATTR                2 (query)
                      178 LOAD_METHOD              4 (find_search)
                      200 LOAD_FAST                1 (event)
                      202 LOAD_ATTR                5 (search_uid)
                      212 KW_NAMES                 3
                      214 PRECALL                  1
                      218 CALL                     1
                      228 STORE_FAST               2 (search)
          
-         230         230 LOAD_FAST                1 (event)
+         234         230 LOAD_FAST                1 (event)
                      232 LOAD_ATTR                6 (domain)
                      242 STORE_FAST               3 (domain)
          
-         231         244 LOAD_FAST                1 (event)
+         235         244 LOAD_FAST                1 (event)
                      246 LOAD_ATTR                7 (type)
                      256 LOAD_CONST               4 ('land')
                      258 COMPARE_OP               2 (==)
                      264 POP_JUMP_FORWARD_IF_FALSE    18 (to 302)
          
-         232         266 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         236         266 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      278 LOAD_FAST                1 (event)
                      280 KW_NAMES                 5
                      282 PRECALL                  1
                      286 CALL                     1
                      296 POP_TOP
                      298 LOAD_CONST               0 (None)
                      300 RETURN_VALUE
          
-         233     >>  302 LOAD_FAST                1 (event)
+         237     >>  302 LOAD_FAST                1 (event)
                      304 LOAD_ATTR                7 (type)
                      314 LOAD_CONST               6 ('create')
                      316 COMPARE_OP               2 (==)
                      322 POP_JUMP_FORWARD_IF_FALSE    18 (to 360)
          
-         234         324 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         238         324 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      336 LOAD_FAST                1 (event)
                      338 KW_NAMES                 5
                      340 PRECALL                  1
                      344 CALL                     1
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
          
-         235     >>  360 LOAD_FAST                1 (event)
+         239     >>  360 LOAD_FAST                1 (event)
                      362 LOAD_ATTR                7 (type)
                      372 LOAD_CONST               7 ('advance')
                      374 COMPARE_OP               2 (==)
                      380 POP_JUMP_FORWARD_IF_FALSE    18 (to 418)
          
-         236         382 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         240         382 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      394 LOAD_FAST                1 (event)
                      396 KW_NAMES                 5
                      398 PRECALL                  1
                      402 CALL                     1
                      412 POP_TOP
                      414 LOAD_CONST               0 (None)
                      416 RETURN_VALUE
          
-         237     >>  418 LOAD_FAST                1 (event)
+         241     >>  418 LOAD_FAST                1 (event)
                      420 LOAD_ATTR                7 (type)
                      430 LOAD_CONST               8 ('validate')
                      432 COMPARE_OP               2 (==)
                      438 POP_JUMP_FORWARD_IF_FALSE    51 (to 542)
          
-         238         440 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         242         440 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      452 LOAD_FAST                1 (event)
                      454 KW_NAMES                 5
                      456 PRECALL                  1
                      460 CALL                     1
                      470 POP_TOP
          
-         239         472 LOAD_GLOBAL             19 (NULL + run_acquired_check)
+         243         472 LOAD_GLOBAL             19 (NULL + run_acquired_check)
                      484 LOAD_FAST                3 (domain)
                      486 KW_NAMES                 9
                      488 PRECALL                  1
                      492 CALL                     1
                      502 POP_TOP
          
-         240         504 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         244         504 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      516 LOAD_FAST                2 (search)
                      518 LOAD_FAST                3 (domain)
                      520 KW_NAMES                10
                      522 PRECALL                  2
                      526 CALL                     2
                      536 POP_TOP
                      538 LOAD_CONST               0 (None)
                      540 RETURN_VALUE
          
-         241     >>  542 LOAD_FAST                1 (event)
+         245     >>  542 LOAD_FAST                1 (event)
                      544 LOAD_ATTR                7 (type)
                      554 LOAD_CONST              11 ('send')
                      556 COMPARE_OP               2 (==)
                      562 POP_JUMP_FORWARD_IF_FALSE    18 (to 600)
          
-         242         564 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         246         564 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      576 LOAD_FAST                1 (event)
                      578 KW_NAMES                 5
                      580 PRECALL                  1
                      584 CALL                     1
                      594 POP_TOP
                      596 LOAD_CONST               0 (None)
                      598 RETURN_VALUE
          
-         243     >>  600 LOAD_FAST                1 (event)
+         247     >>  600 LOAD_FAST                1 (event)
                      602 LOAD_ATTR                7 (type)
                      612 LOAD_CONST              12 ('client_approve')
                      614 COMPARE_OP               2 (==)
                      620 POP_JUMP_FORWARD_IF_FALSE    35 (to 692)
          
-         244         622 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         248         622 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      634 LOAD_FAST                1 (event)
                      636 KW_NAMES                 5
                      638 PRECALL                  1
                      642 CALL                     1
                      652 POP_TOP
          
-         245         654 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         249         654 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      666 LOAD_FAST                2 (search)
                      668 LOAD_FAST                3 (domain)
                      670 KW_NAMES                10
                      672 PRECALL                  2
                      676 CALL                     2
                      686 POP_TOP
                      688 LOAD_CONST               0 (None)
                      690 RETURN_VALUE
          
-         246     >>  692 LOAD_FAST                1 (event)
+         250     >>  692 LOAD_FAST                1 (event)
                      694 LOAD_ATTR                7 (type)
                      704 LOAD_CONST              13 ('reject')
                      706 COMPARE_OP               2 (==)
                      712 POP_JUMP_FORWARD_IF_FALSE     2 (to 718)
          
-         247         714 LOAD_CONST               0 (None)
+         251         714 LOAD_CONST               0 (None)
                      716 RETURN_VALUE
          
-         248     >>  718 LOAD_FAST                1 (event)
+         252     >>  718 LOAD_FAST                1 (event)
                      720 LOAD_ATTR                7 (type)
                      730 LOAD_CONST              14 ('client_reject')
                      732 COMPARE_OP               2 (==)
                      738 POP_JUMP_FORWARD_IF_FALSE     2 (to 744)
          
-         249         740 LOAD_CONST               0 (None)
+         253         740 LOAD_CONST               0 (None)
                      742 RETURN_VALUE
          
-         250     >>  744 LOAD_FAST                1 (event)
+         254     >>  744 LOAD_FAST                1 (event)
                      746 LOAD_ATTR                7 (type)
                      756 LOAD_CONST              15 ('conflict')
                      758 COMPARE_OP               2 (==)
                      764 POP_JUMP_FORWARD_IF_FALSE    35 (to 836)
          
-         251         766 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         255         766 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      778 LOAD_FAST                1 (event)
                      780 KW_NAMES                 5
                      782 PRECALL                  1
                      786 CALL                     1
                      796 POP_TOP
          
-         252         798 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         256         798 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      810 LOAD_FAST                2 (search)
                      812 LOAD_FAST                3 (domain)
                      814 KW_NAMES                10
                      816 PRECALL                  2
                      820 CALL                     2
                      830 POP_TOP
                      832 LOAD_CONST               0 (None)
                      834 RETURN_VALUE
          
-         253     >>  836 LOAD_FAST                1 (event)
+         257     >>  836 LOAD_FAST                1 (event)
                      838 LOAD_ATTR                7 (type)
                      848 LOAD_CONST              16 ('client_conflict')
                      850 COMPARE_OP               2 (==)
                      856 POP_JUMP_FORWARD_IF_FALSE     2 (to 862)
          
-         254         858 LOAD_CONST               0 (None)
+         258         858 LOAD_CONST               0 (None)
                      860 RETURN_VALUE
          
-         257     >>  862 LOAD_FAST                1 (event)
+         261     >>  862 LOAD_FAST                1 (event)
                      864 LOAD_ATTR                7 (type)
                      874 LOAD_CONST              17 ('prompt')
                      876 COMPARE_OP               2 (==)
                      882 POP_JUMP_FORWARD_IF_FALSE    18 (to 920)
          
-         258         884 LOAD_GLOBAL             23 (NULL + handle_prompt)
+         262         884 LOAD_GLOBAL             23 (NULL + handle_prompt)
                      896 LOAD_FAST                1 (event)
                      898 KW_NAMES                 5
                      900 PRECALL                  1
                      904 CALL                     1
                      914 POP_TOP
                      916 LOAD_CONST               0 (None)
                      918 RETURN_VALUE
          
-         259     >>  920 LOAD_FAST                1 (event)
+         263     >>  920 LOAD_FAST                1 (event)
                      922 LOAD_ATTR                7 (type)
                      932 LOAD_CONST              18 ('criteria')
                      934 COMPARE_OP               2 (==)
                      940 POP_JUMP_FORWARD_IF_FALSE    56 (to 1054)
          
-         260         942 LOAD_GLOBAL             25 (NULL + len)
+         264         942 LOAD_GLOBAL             25 (NULL + len)
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
          
-         261        1014 LOAD_GLOBAL             29 (NULL + run_criteria_search)
+         265        1014 LOAD_GLOBAL             29 (NULL + run_criteria_search)
                     1026 LOAD_FAST                2 (search)
                     1028 KW_NAMES                22
                     1030 PRECALL                  1
                     1034 CALL                     1
                     1044 POP_TOP
                     1046 LOAD_CONST               0 (None)
                     1048 RETURN_VALUE
          
-         260     >> 1050 LOAD_CONST               0 (None)
+         264     >> 1050 LOAD_CONST               0 (None)
                     1052 RETURN_VALUE
          
-         262     >> 1054 LOAD_FAST                1 (event)
+         266     >> 1054 LOAD_FAST                1 (event)
                     1056 LOAD_ATTR                7 (type)
                     1066 LOAD_CONST              23 ('maps')
                     1068 COMPARE_OP               2 (==)
                     1074 POP_JUMP_FORWARD_IF_FALSE    19 (to 1114)
          
-         263        1076 LOAD_GLOBAL             31 (NULL + run_maps_search)
+         267        1076 LOAD_GLOBAL             31 (NULL + run_maps_search)
                     1088 LOAD_FAST                2 (search)
                     1090 LOAD_FAST                1 (event)
                     1092 KW_NAMES                24
                     1094 PRECALL                  2
                     1098 CALL                     2
                     1108 POP_TOP
                     1110 LOAD_CONST               0 (None)
                     1112 RETURN_VALUE
          
-         264     >> 1114 LOAD_FAST                1 (event)
+         268     >> 1114 LOAD_FAST                1 (event)
                     1116 LOAD_ATTR                7 (type)
                     1126 LOAD_CONST              25 ('google')
                     1128 COMPARE_OP               2 (==)
                     1134 POP_JUMP_FORWARD_IF_FALSE    19 (to 1174)
          
-         265        1136 LOAD_GLOBAL             33 (NULL + run_google_search)
+         269        1136 LOAD_GLOBAL             33 (NULL + run_google_search)
                     1148 LOAD_FAST                2 (search)
                     1150 LOAD_FAST                1 (event)
                     1152 KW_NAMES                24
                     1154 PRECALL                  2
                     1158 CALL                     2
                     1168 POP_TOP
                     1170 LOAD_CONST               0 (None)
                     1172 RETURN_VALUE
          
-         267     >> 1174 LOAD_FAST                1 (event)
+         271     >> 1174 LOAD_FAST                1 (event)
                     1176 LOAD_ATTR                7 (type)
                     1186 LOAD_CONST              26 ('import')
                     1188 COMPARE_OP               2 (==)
                     1194 POP_JUMP_FORWARD_IF_FALSE    34 (to 1264)
          
-         268        1196 LOAD_GLOBAL              2 (ts)
+         272        1196 LOAD_GLOBAL              2 (ts)
                     1208 LOAD_ATTR                2 (query)
                     1218 LOAD_METHOD             17 (important_targets_from_event)
                     1240 LOAD_FAST                1 (event)
                     1242 KW_NAMES                 5
                     1244 PRECALL                  1
                     1248 CALL                     1
                     1258 POP_TOP
                     1260 LOAD_CONST               0 (None)
                     1262 RETURN_VALUE
          
-         270     >> 1264 LOAD_FAST                1 (event)
+         274     >> 1264 LOAD_FAST                1 (event)
                     1266 LOAD_ATTR                7 (type)
                     1276 LOAD_CONST              27 ('reset')
                     1278 COMPARE_OP               2 (==)
                     1284 POP_JUMP_FORWARD_IF_FALSE    54 (to 1394)
          
-         271        1286 LOAD_GLOBAL              1 (NULL + print)
+         275        1286 LOAD_GLOBAL              1 (NULL + print)
                     1298 LOAD_CONST              28 ('💣 Resetting Inbox...')
                     1300 PRECALL                  1
                     1304 CALL                     1
                     1314 POP_TOP
          
-         272        1316 LOAD_GLOBAL              2 (ts)
+         276        1316 LOAD_GLOBAL              2 (ts)
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
          
-         274     >> 1394 LOAD_FAST                1 (event)
+         278     >> 1394 LOAD_FAST                1 (event)
                     1396 LOAD_ATTR                7 (type)
                     1406 LOAD_CONST              30 ('rating')
                     1408 COMPARE_OP               2 (==)
                     1414 EXTENDED_ARG             1
                     1416 POP_JUMP_FORWARD_IF_FALSE   287 (to 1992)
          
-         276        1418 LOAD_GLOBAL              1 (NULL + print)
+         280        1418 LOAD_GLOBAL              1 (NULL + print)
                     1430 LOAD_FAST                1 (event)
                     1432 PRECALL                  1
                     1436 CALL                     1
                     1446 POP_TOP
          
-         277        1448 LOAD_FAST                1 (event)
+         281        1448 LOAD_FAST                1 (event)
                     1450 LOAD_ATTR               13 (data)
                     1460 LOAD_CONST              30 ('rating')
                     1462 BINARY_SUBSCR
                     1472 STORE_FAST               4 (rating)
          
-         278        1474 LOAD_FAST                1 (event)
+         282        1474 LOAD_FAST                1 (event)
                     1476 LOAD_ATTR               13 (data)
                     1486 LOAD_CONST              31 ('currentView')
                     1488 BINARY_SUBSCR
                     1498 STORE_FAST               5 (from_stage)
          
-         279        1500 LOAD_FAST                4 (rating)
+         283        1500 LOAD_FAST                4 (rating)
                     1502 LOAD_CONST              32 (1)
                     1504 COMPARE_OP               2 (==)
                     1510 POP_JUMP_FORWARD_IF_FALSE    76 (to 1664)
          
-         280        1512 LOAD_GLOBAL              2 (ts)
+         284        1512 LOAD_GLOBAL              2 (ts)
                     1524 LOAD_ATTR                2 (query)
                     1534 LOAD_METHOD             20 (insert_event)
          
-         281        1556 LOAD_GLOBAL              2 (ts)
+         285        1556 LOAD_GLOBAL              2 (ts)
                     1568 LOAD_ATTR               21 (models)
                     1578 LOAD_METHOD             22 (Event)
          
-         282        1600 LOAD_FAST                2 (search)
+         286        1600 LOAD_FAST                2 (search)
                     1602 LOAD_ATTR               19 (uid)
          
-         283        1612 LOAD_CONST              13 ('reject')
+         287        1612 LOAD_CONST              13 ('reject')
          
-         284        1614 LOAD_FAST                3 (domain)
+         288        1614 LOAD_FAST                3 (domain)
          
-         285        1616 LOAD_FAST                1 (event)
+         289        1616 LOAD_FAST                1 (event)
                     1618 LOAD_ATTR               23 (actor_key)
          
-         281        1628 KW_NAMES                33
+         285        1628 KW_NAMES                33
                     1630 PRECALL                  4
                     1634 CALL                     4
          
-         280        1644 PRECALL                  1
+         284        1644 PRECALL                  1
                     1648 CALL                     1
                     1658 POP_TOP
                     1660 LOAD_CONST               0 (None)
                     1662 RETURN_VALUE
          
-         288     >> 1664 LOAD_FAST                4 (rating)
+         292     >> 1664 LOAD_FAST                4 (rating)
                     1666 LOAD_CONST              34 (2)
                     1668 COMPARE_OP               2 (==)
                     1674 POP_JUMP_FORWARD_IF_FALSE    76 (to 1828)
          
-         289        1676 LOAD_GLOBAL              2 (ts)
+         293        1676 LOAD_GLOBAL              2 (ts)
                     1688 LOAD_ATTR                2 (query)
                     1698 LOAD_METHOD             20 (insert_event)
          
-         290        1720 LOAD_GLOBAL              2 (ts)
+         294        1720 LOAD_GLOBAL              2 (ts)
                     1732 LOAD_ATTR               21 (models)
                     1742 LOAD_METHOD             22 (Event)
          
-         291        1764 LOAD_FAST                2 (search)
+         295        1764 LOAD_FAST                2 (search)
                     1766 LOAD_ATTR               19 (uid)
          
-         292        1776 LOAD_CONST              35 ('hold')
+         296        1776 LOAD_CONST              35 ('hold')
          
-         293        1778 LOAD_FAST                3 (domain)
+         297        1778 LOAD_FAST                3 (domain)
          
-         294        1780 LOAD_FAST                1 (event)
+         298        1780 LOAD_FAST                1 (event)
                     1782 LOAD_ATTR               23 (actor_key)
          
-         290        1792 KW_NAMES                33
+         294        1792 KW_NAMES                33
                     1794 PRECALL                  4
                     1798 CALL                     4
          
-         289        1808 PRECALL                  1
+         293        1808 PRECALL                  1
                     1812 CALL                     1
                     1822 POP_TOP
                     1824 LOAD_CONST               0 (None)
                     1826 RETURN_VALUE
          
-         297     >> 1828 LOAD_FAST                5 (from_stage)
+         301     >> 1828 LOAD_FAST                5 (from_stage)
                     1830 LOAD_CONST              36 (('land', 'create', 'advance', 'hold'))
                     1832 CONTAINS_OP              0
                     1834 POP_JUMP_FORWARD_IF_FALSE    76 (to 1988)
          
-         298        1836 LOAD_GLOBAL              2 (ts)
+         302        1836 LOAD_GLOBAL              2 (ts)
                     1848 LOAD_ATTR                2 (query)
                     1858 LOAD_METHOD             20 (insert_event)
          
-         299        1880 LOAD_GLOBAL              2 (ts)
+         303        1880 LOAD_GLOBAL              2 (ts)
                     1892 LOAD_ATTR               21 (models)
                     1902 LOAD_METHOD             22 (Event)
          
-         300        1924 LOAD_FAST                2 (search)
+         304        1924 LOAD_FAST                2 (search)
                     1926 LOAD_ATTR               19 (uid)
          
-         301        1936 LOAD_CONST               8 ('validate')
+         305        1936 LOAD_CONST               8 ('validate')
          
-         302        1938 LOAD_FAST                3 (domain)
+         306        1938 LOAD_FAST                3 (domain)
          
-         303        1940 LOAD_FAST                1 (event)
+         307        1940 LOAD_FAST                1 (event)
                     1942 LOAD_ATTR               23 (actor_key)
          
-         299        1952 KW_NAMES                33
+         303        1952 KW_NAMES                33
                     1954 PRECALL                  4
                     1958 CALL                     4
          
-         298        1968 PRECALL                  1
+         302        1968 PRECALL                  1
                     1972 CALL                     1
                     1982 POP_TOP
                     1984 LOAD_CONST               0 (None)
                     1986 RETURN_VALUE
          
-         297     >> 1988 LOAD_CONST               0 (None)
+         301     >> 1988 LOAD_CONST               0 (None)
                     1990 RETURN_VALUE
          
-         307     >> 1992 LOAD_FAST                1 (event)
+         311     >> 1992 LOAD_FAST                1 (event)
                     1994 LOAD_ATTR                7 (type)
                     2004 LOAD_CONST              37 ('update')
                     2006 COMPARE_OP               2 (==)
                     2012 POP_JUMP_FORWARD_IF_FALSE   185 (to 2384)
          
-         308        2014 LOAD_FAST                3 (domain)
+         312        2014 LOAD_FAST                3 (domain)
                     2016 POP_JUMP_FORWARD_IF_FALSE   129 (to 2276)
          
-         309        2018 LOAD_GLOBAL              2 (ts)
+         313        2018 LOAD_GLOBAL              2 (ts)
                     2030 LOAD_ATTR                2 (query)
                     2040 LOAD_METHOD             24 (find_company_by_domain)
                     2062 LOAD_FAST                3 (domain)
                     2064 PRECALL                  1
                     2068 CALL                     1
                     2078 STORE_FAST               6 (company)
          
-         310        2080 LOAD_FAST                1 (event)
+         314        2080 LOAD_FAST                1 (event)
                     2082 LOAD_ATTR               13 (data)
                     2092 LOAD_METHOD             25 (get)
                     2114 LOAD_CONST              38 ('name')
                     2116 PRECALL                  1
                     2120 CALL                     1
                     2130 POP_JUMP_FORWARD_IF_FALSE    18 (to 2168)
          
-         311        2132 LOAD_FAST                1 (event)
+         315        2132 LOAD_FAST                1 (event)
                     2134 LOAD_ATTR               13 (data)
                     2144 LOAD_CONST              38 ('name')
                     2146 BINARY_SUBSCR
                     2156 LOAD_FAST                6 (company)
                     2158 STORE_ATTR              26 (name)
          
-         317     >> 2168 BUILD_MAP                0
+         321     >> 2168 BUILD_MAP                0
                     2170 LOAD_FAST                6 (company)
                     2172 LOAD_ATTR               27 (meta)
                     2182 DICT_UPDATE              1
                     2184 LOAD_FAST                1 (event)
                     2186 LOAD_ATTR               13 (data)
                     2196 DICT_UPDATE              1
                     2198 LOAD_FAST                6 (company)
                     2200 STORE_ATTR              27 (meta)
          
-         318        2210 LOAD_GLOBAL              2 (ts)
+         322        2210 LOAD_GLOBAL              2 (ts)
                     2222 LOAD_ATTR                2 (query)
                     2232 LOAD_METHOD             28 (update_company)
                     2254 LOAD_FAST                6 (company)
                     2256 PRECALL                  1
                     2260 CALL                     1
                     2270 POP_TOP
                     2272 LOAD_CONST               0 (None)
                     2274 RETURN_VALUE
          
-         320     >> 2276 BUILD_MAP                0
+         324     >> 2276 BUILD_MAP                0
                     2278 LOAD_FAST                2 (search)
                     2280 LOAD_ATTR               27 (meta)
                     2290 DICT_UPDATE              1
                     2292 LOAD_FAST                1 (event)
                     2294 LOAD_ATTR               13 (data)
                     2304 DICT_UPDATE              1
                     2306 LOAD_FAST                2 (search)
                     2308 STORE_ATTR              27 (meta)
          
-         321        2318 LOAD_GLOBAL              2 (ts)
+         325        2318 LOAD_GLOBAL              2 (ts)
                     2330 LOAD_ATTR                2 (query)
                     2340 LOAD_METHOD             29 (update_search)
                     2362 LOAD_FAST                2 (search)
                     2364 PRECALL                  1
                     2368 CALL                     1
                     2378 POP_TOP
                     2380 LOAD_CONST               0 (None)
                     2382 RETURN_VALUE
          
-         323     >> 2384 LOAD_FAST                1 (event)
+         327     >> 2384 LOAD_FAST                1 (event)
                     2386 LOAD_ATTR                7 (type)
                     2396 LOAD_CONST              39 ('move')
                     2398 COMPARE_OP               2 (==)
                     2404 POP_JUMP_FORWARD_IF_FALSE   117 (to 2640)
          
-         325        2406 LOAD_FAST                1 (event)
+         329        2406 LOAD_FAST                1 (event)
                     2408 LOAD_ATTR               13 (data)
                     2418 LOAD_CONST              40 ('domains')
                     2420 BINARY_SUBSCR
                     2430 GET_ITER
                  >> 2432 FOR_ITER               105 (to 2644)
                     2434 STORE_FAST               3 (domain)
          
-         326        2436 LOAD_GLOBAL              1 (NULL + print)
+         330        2436 LOAD_GLOBAL              1 (NULL + print)
                     2448 LOAD_CONST              41 ('moving domain:')
                     2450 LOAD_FAST                3 (domain)
                     2452 PRECALL                  2
                     2456 CALL                     2
                     2466 POP_TOP
          
-         327        2468 LOAD_GLOBAL              2 (ts)
+         331        2468 LOAD_GLOBAL              2 (ts)
                     2480 LOAD_ATTR                2 (query)
                     2490 LOAD_METHOD             20 (insert_event)
          
-         328        2512 LOAD_GLOBAL              2 (ts)
+         332        2512 LOAD_GLOBAL              2 (ts)
                     2524 LOAD_ATTR               21 (models)
                     2534 LOAD_METHOD             22 (Event)
          
-         329        2556 LOAD_FAST                2 (search)
+         333        2556 LOAD_FAST                2 (search)
                     2558 LOAD_ATTR               19 (uid)
          
-         330        2568 LOAD_FAST                3 (domain)
+         334        2568 LOAD_FAST                3 (domain)
          
-         331        2570 LOAD_FAST                1 (event)
+         335        2570 LOAD_FAST                1 (event)
                     2572 LOAD_ATTR               13 (data)
                     2582 LOAD_CONST              42 ('stage')
                     2584 BINARY_SUBSCR
          
-         332        2594 LOAD_FAST                1 (event)
+         336        2594 LOAD_FAST                1 (event)
                     2596 LOAD_ATTR               23 (actor_key)
          
-         328        2606 KW_NAMES                43
+         332        2606 KW_NAMES                43
                     2608 PRECALL                  4
                     2612 CALL                     4
          
-         327        2622 PRECALL                  1
+         331        2622 PRECALL                  1
                     2626 CALL                     1
                     2636 POP_TOP
                     2638 JUMP_BACKWARD          104 (to 2432)
          
-         323     >> 2640 LOAD_CONST               0 (None)
+         327     >> 2640 LOAD_CONST               0 (None)
                     2642 RETURN_VALUE
          
-         325     >> 2644 LOAD_CONST               0 (None)
+         329     >> 2644 LOAD_CONST               0 (None)
                     2646 RETURN_VALUE
          consts
             None
             'processing event...'
             'event_id'
             ('uid',)
             'land'
@@ -2117,24 +2138,24 @@
             ('search_uid', 'domain', 'type', 'actor_key')
          names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'len', 'data', 'run_criteria_search', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'reset_inbox', 'uid', 'insert_event', 'models', 'Event', 'actor_key', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
          varnames   ('event_id', 'event', 'search', 'domain', 'rating', 'from_stage', 'company')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_event'
-         firstlineno 224
+         firstlineno 228
          lnotab
             0x02011e013e0120011e014a010e01160124011601240116012401160120
             012001260116012401160120012601160104011601040116012001260116
             010403160124011601480124ff040216012601160126021601440216011e
             014e0218021e011a011a010c012c012c010c01020102010cfc10ff14080c
             012c012c010c01020102010cfc10ff140808012c012c010c01020102010c
             fc10ff14ff040a160104013e01340124062a0142022a01420216021e0120
             012c012c010c01020118010cfc10ff12fc0402
-   names      ('time', 'dataclasses', 'asdict', 'dacite', 'from_dict', 'gandai', 'ts', 'str', 'run_acquired_check', 'models', 'Search', 'run_similarity_search', 'run_criteria_search', 'Event', 'run_maps_search', 'run_google_search', 'handle_prompt', 'Company', 'enrich_with_gpt', 'run_enrichment', 'int', 'process_event')
+   names      ('dataclasses', 'asdict', 'time', 'gandai', 'ts', 'dacite', 'from_dict', 'str', 'run_acquired_check', 'models', 'Search', 'run_similarity_search', 'run_criteria_search', 'Event', 'run_maps_search', 'run_google_search', 'handle_prompt', 'Company', 'enrich_with_gpt', 'run_enrichment', 'int', 'process_event')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c010c0208030c27280b240d3c2d3c0f242b24212411
+   lnotab 0x00ff02010c010c0208010c030c26280b240d3c2d3c0f242c24222414
```

### Comparing `gandai-1.7.44/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xeac14f66 (Thu May 23 22:23:38 2024 UTC)
-files sz: 28619
+moddate:  0xeed64f66 (Thu May 23 23:53:18 2024 UTC)
+files sz: 28680
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
    
-   610         486 LOAD_CONST              22 ('search_uid')
+   611         486 LOAD_CONST              22 ('search_uid')
                488 LOAD_NAME               33 (int)
                490 LOAD_CONST              11 ('return')
                492 LOAD_NAME                9 (pd)
                494 LOAD_ATTR               37 (DataFrame)
                504 BUILD_TUPLE              4
-               506 LOAD_CONST              35 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 610>)
+               506 LOAD_CONST              35 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 611>)
                508 MAKE_FUNCTION            4 (annotations)
                510 STORE_NAME              46 (search_comments)
    
-   632         512 LOAD_CONST              22 ('search_uid')
+   633         512 LOAD_CONST              22 ('search_uid')
                514 LOAD_NAME               33 (int)
                516 LOAD_CONST              11 ('return')
                518 LOAD_NAME                9 (pd)
                520 LOAD_ATTR               37 (DataFrame)
                530 BUILD_TUPLE              4
-               532 LOAD_CONST              36 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 632>)
+               532 LOAD_CONST              36 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 633>)
                534 MAKE_FUNCTION            4 (annotations)
                536 STORE_NAME              47 (event)
    
-   644         538 LOAD_CONST              22 ('search_uid')
+   645         538 LOAD_CONST              22 ('search_uid')
                540 LOAD_NAME               33 (int)
                542 LOAD_CONST              11 ('return')
                544 LOAD_NAME                9 (pd)
                546 LOAD_ATTR               37 (DataFrame)
                556 BUILD_TUPLE              4
-               558 LOAD_CONST              37 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 644>)
+               558 LOAD_CONST              37 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 645>)
                560 MAKE_FUNCTION            4 (annotations)
                562 STORE_NAME              48 (event_history)
    
-   674         564 LOAD_CONST              22 ('search_uid')
+   675         564 LOAD_CONST              22 ('search_uid')
                566 LOAD_NAME               33 (int)
                568 LOAD_CONST              11 ('return')
                570 LOAD_NAME                9 (pd)
                572 LOAD_ATTR               37 (DataFrame)
                582 BUILD_TUPLE              4
-               584 LOAD_CONST              38 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 674>)
+               584 LOAD_CONST              38 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 675>)
                586 MAKE_FUNCTION            4 (annotations)
                588 STORE_NAME              49 (search_criteria_history)
    
-   703         590 LOAD_CONST              39 ('uid')
+   704         590 LOAD_CONST              39 ('uid')
                592 LOAD_NAME               33 (int)
                594 LOAD_CONST              11 ('return')
                596 LOAD_NAME               16 (ts)
                598 LOAD_ATTR               28 (models)
                608 LOAD_ATTR               25 (Search)
                618 BUILD_TUPLE              4
-               620 LOAD_CONST              40 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 703>)
+               620 LOAD_CONST              40 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 704>)
                622 MAKE_FUNCTION            4 (annotations)
                624 STORE_NAME              50 (find_search)
    
-   731         626 LOAD_CONST              41 ('searchToken')
+   732         626 LOAD_CONST              41 ('searchToken')
                628 LOAD_NAME               34 (str)
                630 LOAD_CONST              11 ('return')
                632 LOAD_NAME               16 (ts)
                634 LOAD_ATTR               28 (models)
                644 LOAD_ATTR               25 (Search)
                654 BUILD_TUPLE              4
-               656 LOAD_CONST              42 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 731>)
+               656 LOAD_CONST              42 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 732>)
                658 MAKE_FUNCTION            4 (annotations)
                660 STORE_NAME              51 (find_search_by_token)
    
-   740         662 LOAD_CONST              43 ('domain')
+   741         662 LOAD_CONST              43 ('domain')
                664 LOAD_NAME               34 (str)
                666 LOAD_CONST              11 ('return')
                668 LOAD_NAME               22 (Company)
                670 BUILD_TUPLE              4
-               672 LOAD_CONST              44 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 740>)
+               672 LOAD_CONST              44 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 741>)
                674 MAKE_FUNCTION            4 (annotations)
                676 STORE_NAME              52 (find_company_by_domain)
    
-   756         678 LOAD_CONST              45 ('email')
+   757         678 LOAD_CONST              45 ('email')
                680 LOAD_NAME               34 (str)
                682 LOAD_CONST              11 ('return')
                684 LOAD_NAME               22 (Company)
                686 BUILD_TUPLE              4
-               688 LOAD_CONST              46 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 756>)
+               688 LOAD_CONST              46 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 757>)
                690 MAKE_FUNCTION            4 (annotations)
                692 STORE_NAME              53 (find_actor_by_email)
    
-   772         694 LOAD_CONST              47 ('event_id')
+   773         694 LOAD_CONST              47 ('event_id')
                696 LOAD_NAME               33 (int)
                698 LOAD_CONST              11 ('return')
                700 LOAD_NAME               23 (Event)
                702 BUILD_TUPLE              4
-               704 LOAD_CONST              48 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 772>)
+               704 LOAD_CONST              48 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 773>)
                706 MAKE_FUNCTION            4 (annotations)
                708 STORE_NAME              54 (find_event_by_id)
    
-   791         710 LOAD_CONST              13 ('company')
+   792         710 LOAD_CONST              13 ('company')
                712 LOAD_NAME               22 (Company)
                714 LOAD_CONST              11 ('return')
                716 LOAD_CONST               1 (None)
                718 BUILD_TUPLE              4
-               720 LOAD_CONST              49 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 791>)
+               720 LOAD_CONST              49 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 792>)
                722 MAKE_FUNCTION            4 (annotations)
                724 STORE_NAME              55 (update_company)
    
-   820         726 LOAD_CONST              17 ('search')
+   821         726 LOAD_CONST              17 ('search')
                728 LOAD_NAME               25 (Search)
                730 LOAD_CONST              11 ('return')
                732 LOAD_CONST               1 (None)
                734 BUILD_TUPLE              4
-               736 LOAD_CONST              50 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 820>)
+               736 LOAD_CONST              50 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 821>)
                738 MAKE_FUNCTION            4 (annotations)
                740 STORE_NAME              56 (update_search)
    
-   843         742 LOAD_CONST              47 ('event_id')
+   844         742 LOAD_CONST              47 ('event_id')
                744 LOAD_NAME               33 (int)
                746 LOAD_CONST              11 ('return')
                748 LOAD_CONST               1 (None)
                750 BUILD_TUPLE              4
-               752 LOAD_CONST              51 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 843>)
+               752 LOAD_CONST              51 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 844>)
                754 MAKE_FUNCTION            4 (annotations)
                756 STORE_NAME              57 (mute_event)
    
-   866         758 LOAD_CONST              52 ('comment_id')
+   867         758 LOAD_CONST              52 ('comment_id')
                760 LOAD_NAME               33 (int)
                762 LOAD_CONST              11 ('return')
                764 LOAD_CONST               1 (None)
                766 BUILD_TUPLE              4
-               768 LOAD_CONST              53 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 866>)
+               768 LOAD_CONST              53 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 867>)
                770 MAKE_FUNCTION            4 (annotations)
                772 STORE_NAME              58 (delete_comment)
    
-   877         774 LOAD_CONST              22 ('search_uid')
+   878         774 LOAD_CONST              22 ('search_uid')
                776 LOAD_NAME               33 (int)
                778 LOAD_CONST              11 ('return')
                780 LOAD_CONST               1 (None)
                782 BUILD_TUPLE              4
-               784 LOAD_CONST              54 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 877>)
+               784 LOAD_CONST              54 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 878>)
                786 MAKE_FUNCTION            4 (annotations)
                788 STORE_NAME              59 (reset_inbox)
                790 LOAD_CONST               1 (None)
                792 RETURN_VALUE
    consts
       0
       None
@@ -2604,57 +2604,57 @@
             010000ab0100000000000000007c04640d3c0000007c04a00a0000000000
             0000000000000000000000000000007c08640eac0fa6020000ab02000000
             00000000007c0464103c0000007c04a00a00000000000000000000000000
             000000000000007c09640eac0fa6020000ab0200000000000000007c0464
             113c0000007c045300
          478           0 RESUME                   0
          
-         481           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        c.description as grata_description,\n        c.meta->>'description' as description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n    ;\n    ")
+         481           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         543           6 LOAD_GLOBAL              0 (db)
+         544           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         544          58 LOAD_FAST                2 (conn)
+         545          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         545          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         546          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         546         120 LOAD_CONST               2 ('search_uid')
+         547         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         544         126 PRECALL                  2
+         545         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         548         142 LOAD_GLOBAL             11 (NULL + pd)
+         549         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         543         258 LOAD_CONST               0 (None)
+         544         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2665,139 +2665,139 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         550     >>  304 LOAD_CONST               4 ('return')
+         551     >>  304 LOAD_CONST               4 ('return')
                      306 LOAD_GLOBAL             18 (str)
                      318 BUILD_TUPLE              2
-                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 550>)
+                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 551>)
                      322 MAKE_FUNCTION            4 (annotations)
                      324 STORE_FAST               5 (list_to_csv)
          
-         562         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 562>)
+         563         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 563>)
                      328 MAKE_FUNCTION            0
                      330 STORE_FAST               6 (get_employees)
          
-         574         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 574>)
+         575         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 575>)
                      334 MAKE_FUNCTION            0
                      336 STORE_FAST               7 (get_ownership)
          
-         582         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 582>)
+         583         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 583>)
                      340 MAKE_FUNCTION            0
                      342 STORE_FAST               8 (get_state)
          
-         592         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 592>)
+         593         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 593>)
                      346 MAKE_FUNCTION            0
                      348 STORE_FAST               9 (get_city)
          
-         601         350 LOAD_FAST                4 (df)
+         602         350 LOAD_FAST                4 (df)
                      352 LOAD_CONST              10 ('end_customer')
                      354 BINARY_SUBSCR
                      364 LOAD_METHOD             10 (apply)
                      386 LOAD_FAST                5 (list_to_csv)
                      388 PRECALL                  1
                      392 CALL                     1
                      402 LOAD_FAST                4 (df)
                      404 LOAD_CONST              10 ('end_customer')
                      406 STORE_SUBSCR
          
-         602         410 LOAD_FAST                4 (df)
+         603         410 LOAD_FAST                4 (df)
                      412 LOAD_CONST              11 ('meta')
                      414 BINARY_SUBSCR
                      424 LOAD_METHOD             10 (apply)
                      446 LOAD_FAST                6 (get_employees)
                      448 PRECALL                  1
                      452 CALL                     1
                      462 LOAD_FAST                4 (df)
                      464 LOAD_CONST              12 ('employees')
                      466 STORE_SUBSCR
          
-         603         470 LOAD_FAST                4 (df)
+         604         470 LOAD_FAST                4 (df)
                      472 LOAD_CONST              13 ('ownership')
                      474 BINARY_SUBSCR
                      484 LOAD_METHOD             10 (apply)
                      506 LOAD_FAST                7 (get_ownership)
                      508 PRECALL                  1
                      512 CALL                     1
                      522 LOAD_FAST                4 (df)
                      524 LOAD_CONST              13 ('ownership')
                      526 STORE_SUBSCR
          
-         604         530 LOAD_FAST                4 (df)
+         605         530 LOAD_FAST                4 (df)
                      532 LOAD_METHOD             10 (apply)
                      554 LOAD_FAST                8 (get_state)
                      556 LOAD_CONST              14 (1)
                      558 KW_NAMES                15
                      560 PRECALL                  2
                      564 CALL                     2
                      574 LOAD_FAST                4 (df)
                      576 LOAD_CONST              16 ('state')
                      578 STORE_SUBSCR
          
-         605         582 LOAD_FAST                4 (df)
+         606         582 LOAD_FAST                4 (df)
                      584 LOAD_METHOD             10 (apply)
                      606 LOAD_FAST                9 (get_city)
                      608 LOAD_CONST              14 (1)
                      610 KW_NAMES                15
                      612 PRECALL                  2
                      616 CALL                     2
                      626 LOAD_FAST                4 (df)
                      628 LOAD_CONST              17 ('city')
                      630 STORE_SUBSCR
          
-         607         634 LOAD_FAST                4 (df)
+         608         634 LOAD_FAST                4 (df)
                      636 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
-            "\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        c.description as grata_description,\n        c.meta->>'description' as description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n    ;\n    "
+            "\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        c.description as grata_description,\n        c.meta->>'description' as grata_description,\n        c.meta->>'gpt_description' as gpt_description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n    ;\n    "
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
-               550           0 RESUME                   0
+               551           0 RESUME                   0
                
-               552           2 NOP
+               553           2 NOP
                
-               553           4 LOAD_GLOBAL              1 (NULL + json)
+               554           4 LOAD_GLOBAL              1 (NULL + json)
                             16 LOAD_ATTR                1 (loads)
                             26 LOAD_FAST                0 (list_str)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               1 (list_data)
                
-               556          44 LOAD_CONST               1 (', ')
+               557          44 LOAD_CONST               1 (', ')
                             46 LOAD_METHOD              2 (join)
                             68 LOAD_FAST                1 (list_data)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 STORE_FAST               2 (csv_str)
                
-               558          86 LOAD_FAST                2 (csv_str)
+               559          86 LOAD_FAST                2 (csv_str)
                             88 RETURN_VALUE
                        >>   90 PUSH_EXC_INFO
                
-               559          92 POP_TOP
+               560          92 POP_TOP
                
-               560          94 POP_EXCEPT
+               561          94 POP_EXCEPT
                             96 LOAD_CONST               2 ('')
                             98 RETURN_VALUE
                        >>  100 COPY                     3
                            102 POP_EXCEPT
                            104 RERAISE                  1
                ExceptionTable:
                  4 to 86 -> 90 [0]
@@ -2808,75 +2808,75 @@
                   ''
                names      ('json', 'loads', 'join')
                varnames   ('list_str', 'list_data', 'csv_str')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'list_to_csv'
-               firstlineno 550
+               firstlineno 551
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
-               562           0 RESUME                   0
+               563           0 RESUME                   0
                
-               563           2 LOAD_FAST                0 (meta)
+               564           2 LOAD_FAST                0 (meta)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('employees')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    30 (to 104)
                
-               565          44 NOP
+               566          44 NOP
                
-               566          46 LOAD_GLOBAL              3 (NULL + int)
+               567          46 LOAD_GLOBAL              3 (NULL + int)
                             58 LOAD_FAST                0 (meta)
                             60 LOAD_CONST               1 ('employees')
                             62 BINARY_SUBSCR
                             72 PRECALL                  1
                             76 CALL                     1
                             86 RETURN_VALUE
                        >>   88 PUSH_EXC_INFO
                
-               567          90 POP_TOP
+               568          90 POP_TOP
                
-               568          92 POP_EXCEPT
+               569          92 POP_EXCEPT
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                        >>   98 COPY                     3
                            100 POP_EXCEPT
                            102 RERAISE                  1
                
-               569     >>  104 LOAD_FAST                0 (meta)
+               570     >>  104 LOAD_FAST                0 (meta)
                            106 LOAD_METHOD              0 (get)
                            128 LOAD_CONST               2 ('grata_employee_estimates')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 POP_JUMP_FORWARD_IF_FALSE    27 (to 200)
                
-               570         146 LOAD_FAST                0 (meta)
+               571         146 LOAD_FAST                0 (meta)
                            148 LOAD_CONST               2 ('grata_employee_estimates')
                            150 BINARY_SUBSCR
                            160 LOAD_METHOD              0 (get)
                            182 LOAD_CONST               3 ('count')
                            184 PRECALL                  1
                            188 CALL                     1
                            198 RETURN_VALUE
                
-               572     >>  200 LOAD_CONST               0 (None)
+               573     >>  200 LOAD_CONST               0 (None)
                            202 RETURN_VALUE
                ExceptionTable:
                  46 to 84 -> 88 [0]
                  88 to 90 -> 98 [1] lasti
                consts
                   None
                   'employees'
@@ -2884,57 +2884,57 @@
                   'count'
                names      ('get', 'int')
                varnames   ('meta',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_employees'
-               firstlineno 562
+               firstlineno 563
                lnotab 0x02012a0202012c0102010c012a013602
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 19
                code
                   0x97007c0064016b02000000007202640253007c0064036b020000000072
                   02640453007c005300
-               574           0 RESUME                   0
+               575           0 RESUME                   0
                
-               575           2 LOAD_FAST                0 (ownership)
+               576           2 LOAD_FAST                0 (ownership)
                              4 LOAD_CONST               1 ('Bootstrapped')
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE     2 (to 18)
                
-               576          14 LOAD_CONST               2 ('Private')
+               577          14 LOAD_CONST               2 ('Private')
                             16 RETURN_VALUE
                
-               577     >>   18 LOAD_FAST                0 (ownership)
+               578     >>   18 LOAD_FAST                0 (ownership)
                             20 LOAD_CONST               3 ('Investor Backed')
                             22 COMPARE_OP               2 (==)
                             28 POP_JUMP_FORWARD_IF_FALSE     2 (to 34)
                
-               578          30 LOAD_CONST               4 ('Venture Capital')
+               579          30 LOAD_CONST               4 ('Venture Capital')
                             32 RETURN_VALUE
                
-               580     >>   34 LOAD_FAST                0 (ownership)
+               581     >>   34 LOAD_FAST                0 (ownership)
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
-               firstlineno 574
+               firstlineno 575
                lnotab 0x02010c0104010c010402
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 19
                code
@@ -2944,78 +2944,78 @@
                   00ab010000000000000000725a7c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017406000000
                   000000000000006a0400000000000000006a050000000000000000a00000
                   000000000000000000000000000000000000007c016405a6020000ab0200
                   000000000000007d027c02530064005300
-               582           0 RESUME                   0
+               583           0 RESUME                   0
                
-               583           2 LOAD_FAST                0 (row)
+               584           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('state')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               584          44 LOAD_FAST                0 (row)
+               585          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('state')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               585     >>   60 LOAD_FAST                0 (row)
+               586     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    90 (to 282)
                
-               586         102 LOAD_FAST                0 (row)
+               587         102 LOAD_FAST                0 (row)
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
                
-               587         204 LOAD_GLOBAL              6 (ts)
+               588         204 LOAD_GLOBAL              6 (ts)
                            216 LOAD_ATTR                4 (constants)
                            226 LOAD_ATTR                5 (STATE_NAMES)
                            236 LOAD_METHOD              0 (get)
                            258 LOAD_FAST                1 (state_name)
                            260 LOAD_CONST               5 ('')
                            262 PRECALL                  2
                            266 CALL                     2
                            276 STORE_FAST               2 (state_code)
                
-               588         278 LOAD_FAST                2 (state_code)
+               589         278 LOAD_FAST                2 (state_code)
                            280 RETURN_VALUE
                
-               590     >>  282 LOAD_CONST               0 (None)
+               591     >>  282 LOAD_CONST               0 (None)
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
-               firstlineno 582
+               firstlineno 583
                lnotab 0x02012a0110012a0166014a010402
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
@@ -3023,67 +3023,67 @@
                   010000ab01000000000000000072087c0064011900000000000000000053
                   007c00a00000000000000000000000000000000000000000006402a60100
                   00ab01000000000000000072357c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017c01530064
                   005300
-               592           0 RESUME                   0
+               593           0 RESUME                   0
                
-               593           2 LOAD_FAST                0 (row)
+               594           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('city')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               594          44 LOAD_FAST                0 (row)
+               595          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('city')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               595     >>   60 LOAD_FAST                0 (row)
+               596     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    53 (to 208)
                
-               596         102 LOAD_FAST                0 (row)
+               597         102 LOAD_FAST                0 (row)
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
                
-               597         204 LOAD_FAST                1 (city_name)
+               598         204 LOAD_FAST                1 (city_name)
                            206 RETURN_VALUE
                
-               599     >>  208 LOAD_CONST               0 (None)
+               600     >>  208 LOAD_CONST               0 (None)
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
-               firstlineno 592
+               firstlineno 593
                lnotab 0x02012a0110012a0166010402
             'end_customer'
             'meta'
             'employees'
             'ownership'
             1
             ('axis',)
@@ -3093,15 +3093,15 @@
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df', 'list_to_csv', 'get_employees', 'get_ownership', 'get_state', 'get_city')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_targets'
          firstlineno 478
          lnotab
-            0x0203043e34011801260106fe100474fb2e07160c060c0608060a06093c
+            0x0203043f34011801260106fe100474fb2e07160c060c0608060a06093c
             013c013c0134013402
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3112,59 +3112,59 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         610           0 RESUME                   0
+         611           0 RESUME                   0
          
-         611           2 LOAD_CONST               1 ("\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    ")
+         612           2 LOAD_CONST               1 ("\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    ")
                        4 STORE_FAST               1 (statement)
          
-         623           6 LOAD_GLOBAL              0 (db)
+         624           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         624          58 LOAD_FAST                2 (conn)
+         625          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         625          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         626          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         626         120 LOAD_CONST               2 ('search_uid')
+         627         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         624         126 PRECALL                  2
+         625         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         628         142 LOAD_GLOBAL             11 (NULL + pd)
+         629         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         623         258 LOAD_CONST               0 (None)
+         624         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3175,15 +3175,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         629     >>  304 LOAD_FAST                4 (df)
+         630     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3192,15 +3192,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_comments'
-         firstlineno 610
+         firstlineno 611
          lnotab 0x0201040c34011801260106fe100474fb2e06
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3211,56 +3211,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         632           0 RESUME                   0
+         633           0 RESUME                   0
          
-         633           2 LOAD_GLOBAL              0 (db)
+         634           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         634          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         635          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         639          58 LOAD_FAST                1 (conn)
+         640          58 LOAD_FAST                1 (conn)
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
          
-         640         142 LOAD_GLOBAL             11 (NULL + pd)
+         641         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         633         258 LOAD_CONST               0 (None)
+         634         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3271,15 +3271,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         641     >>  304 LOAD_FAST                4 (df)
+         642     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3288,15 +3288,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 632
+         firstlineno 633
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3308,65 +3308,65 @@
             007c01a6010000ab01000000000000000064027c006901a6020000ab0200
             000000000000007d03740f000000000000000000006a0800000000000000
             007c03a0090000000000000000000000000000000000000000a6000000ab
             0000000000000000007c03a00a0000000000000000000000000000000000
             000000a6000000ab000000000000000000ac03a6020000ab020000000000
             0000007d04640064006400a6020000ab02000000000000000001006e0b23
             0031007304770278035900770101005900010001007c045300
-         644           0 RESUME                   0
+         645           0 RESUME                   0
          
-         645           2 LOAD_GLOBAL              1 (NULL + isinstance)
+         646           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (search_uid)
                       16 LOAD_GLOBAL              2 (int)
                       28 PRECALL                  2
                       32 CALL                     2
                       42 POP_JUMP_FORWARD_IF_TRUE     2 (to 48)
                       44 LOAD_ASSERTION_ERROR
                       46 RAISE_VARARGS            1
          
-         646     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
+         647     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
                       50 STORE_FAST               1 (statement)
          
-         668          52 LOAD_GLOBAL              4 (db)
+         669          52 LOAD_GLOBAL              4 (db)
                       64 LOAD_METHOD              3 (connect)
                       86 PRECALL                  0
                       90 CALL                     0
                      100 BEFORE_WITH
                      102 STORE_FAST               2 (conn)
          
-         669         104 LOAD_FAST                2 (conn)
+         670         104 LOAD_FAST                2 (conn)
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
          
-         670         188 LOAD_GLOBAL             15 (NULL + pd)
+         671         188 LOAD_GLOBAL             15 (NULL + pd)
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
          
-         668         304 LOAD_CONST               0 (None)
+         669         304 LOAD_CONST               0 (None)
                      306 LOAD_CONST               0 (None)
                      308 LOAD_CONST               0 (None)
                      310 PRECALL                  2
                      314 CALL                     2
                      324 POP_TOP
                      326 JUMP_FORWARD            11 (to 350)
                  >>  328 PUSH_EXC_INFO
@@ -3377,15 +3377,15 @@
                      338 POP_EXCEPT
                      340 RERAISE                  1
                  >>  342 POP_TOP
                      344 POP_EXCEPT
                      346 POP_TOP
                      348 POP_TOP
          
-         671     >>  350 LOAD_FAST                4 (df)
+         672     >>  350 LOAD_FAST                4 (df)
                      352 RETURN_VALUE
          ExceptionTable:
            102 to 302 -> 328 [1] lasti
            328 to 334 -> 336 [3] lasti
            342 to 342 -> 336 [3] lasti
          consts
             None
@@ -3394,15 +3394,15 @@
             ('columns',)
          names      ('isinstance', 'int', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event_history'
-         firstlineno 644
+         firstlineno 645
          lnotab 0x02012e0104163401540174fe2e03
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3413,56 +3413,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         674           0 RESUME                   0
+         675           0 RESUME                   0
          
-         676           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
+         677           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         694           6 LOAD_GLOBAL              0 (db)
+         695           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         695          58 LOAD_FAST                2 (conn)
+         696          58 LOAD_FAST                2 (conn)
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
          
-         696         142 LOAD_GLOBAL             11 (NULL + pd)
+         697         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         694         258 LOAD_CONST               0 (None)
+         695         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3473,15 +3473,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         697     >>  304 LOAD_FAST                4 (df)
+         698     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3490,15 +3490,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_criteria_history'
-         firstlineno 674
+         firstlineno 675
          lnotab 0x020204123401540174fe2e03
       'uid'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 7
          flags     : 3
@@ -3516,96 +3516,96 @@
             000000000000007d05741300000000000000000000741400000000000000
             0000006a0b00000000000000006a0c00000000000000007c05a6020000ab
             0200000000000000007d067c066a0d0000000000000000a00e0000000000
             0000000000000000000000000000006403a6010000ab0100000000000000
             006404190000000000000000007c066a0f000000000000000064053c0000
             00640064006400a6020000ab02000000000000000001006e0b2300310073
             04770278035900770101005900010001007c065300
-         703           0 RESUME                   0
+         704           0 RESUME                   0
          
-         704           2 LOAD_GLOBAL              0 (db)
+         705           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         705          54 LOAD_CONST               1 ("\n            SELECT \n                uid, \n                label, \n                meta, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            ")
+         706          54 LOAD_CONST               1 ("\n            SELECT \n                uid, \n                label, \n                meta, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            ")
                       56 STORE_FAST               2 (statement)
          
-         718          58 LOAD_FAST                1 (conn)
+         719          58 LOAD_FAST                1 (conn)
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
          
-         720         142 LOAD_FAST                3 (result)
+         721         142 LOAD_FAST                3 (result)
                      144 LOAD_METHOD              5 (fetchone)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 STORE_FAST               4 (row)
          
-         721         182 LOAD_FAST                4 (row)
+         722         182 LOAD_FAST                4 (row)
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 214)
          
-         722         186 NOP
+         723         186 NOP
          
-         704         188 LOAD_CONST               0 (None)
+         705         188 LOAD_CONST               0 (None)
                      190 LOAD_CONST               0 (None)
                      192 LOAD_CONST               0 (None)
                      194 PRECALL                  2
                      198 CALL                     2
                      208 POP_TOP
                      210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         724     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         725     >>  214 LOAD_GLOBAL             13 (NULL + dict)
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
          
-         725         308 LOAD_GLOBAL             19 (NULL + from_dict)
+         726         308 LOAD_GLOBAL             19 (NULL + from_dict)
                      320 LOAD_GLOBAL             20 (ts)
                      332 LOAD_ATTR               11 (models)
                      342 LOAD_ATTR               12 (Search)
                      352 LOAD_FAST                5 (obj)
                      354 PRECALL                  2
                      358 CALL                     2
                      368 STORE_FAST               6 (search)
          
-         726         370 LOAD_FAST                6 (search)
+         727         370 LOAD_FAST                6 (search)
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
          
-         704         450 LOAD_CONST               0 (None)
+         705         450 LOAD_CONST               0 (None)
                      452 LOAD_CONST               0 (None)
                      454 LOAD_CONST               0 (None)
                      456 PRECALL                  2
                      460 CALL                     2
                      470 POP_TOP
                      472 JUMP_FORWARD            11 (to 496)
                  >>  474 PUSH_EXC_INFO
@@ -3616,15 +3616,15 @@
                      484 POP_EXCEPT
                      486 RERAISE                  1
                  >>  488 POP_TOP
                      490 POP_EXCEPT
                      492 POP_TOP
                      494 POP_TOP
          
-         728     >>  496 LOAD_FAST                6 (search)
+         729     >>  496 LOAD_FAST                6 (search)
                      498 RETURN_VALUE
          ExceptionTable:
            52 to 186 -> 474 [1] lasti
            214 to 448 -> 474 [1] lasti
            474 to 480 -> 482 [3] lasti
            488 to 488 -> 482 [3] lasti
          consts
@@ -3636,52 +3636,52 @@
             'client'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'fetchone', 'dict', 'zip', 'keys', 'from_dict', 'ts', 'models', 'Search', 'label', 'split', 'meta')
          varnames   ('uid', 'conn', 'statement', 'result', 'row', 'obj', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search'
-         firstlineno 703
+         firstlineno 704
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
-         731           0 RESUME                   0
+         732           0 RESUME                   0
          
-         732           2 LOAD_GLOBAL              1 (NULL + searches_query)
+         733           2 LOAD_GLOBAL              1 (NULL + searches_query)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (searches)
          
-         733          30 LOAD_FAST                1 (searches)
+         734          30 LOAD_FAST                1 (searches)
                       32 LOAD_FAST                1 (searches)
                       34 LOAD_CONST               1 ('searchToken')
                       36 BINARY_SUBSCR
                       46 LOAD_FAST                0 (searchToken)
                       48 COMPARE_OP               2 (==)
                       54 BINARY_SUBSCR
                       64 STORE_FAST               2 (search)
          
-         734          66 LOAD_FAST                2 (search)
+         735          66 LOAD_FAST                2 (search)
                       68 LOAD_ATTR                1 (empty)
                       78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
          
-         735          80 LOAD_CONST               0 (None)
+         736          80 LOAD_CONST               0 (None)
                       82 RETURN_VALUE
          
-         737     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
+         738     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
                       96 LOAD_FAST                2 (search)
                       98 LOAD_ATTR                3 (iloc)
                      108 LOAD_CONST               2 (0)
                      110 BINARY_SUBSCR
                      120 LOAD_CONST               3 ('uid')
                      122 BINARY_SUBSCR
                      132 PRECALL                  1
@@ -3694,15 +3694,15 @@
             'uid'
          names      ('searches_query', 'empty', 'find_search', 'iloc')
          varnames   ('searchToken', 'searches', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_token'
-         firstlineno 731
+         firstlineno 732
          lnotab 0x02011c0124010e010402
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3716,41 +3716,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         740           0 RESUME                   0
+         741           0 RESUME                   0
          
-         741           2 LOAD_GLOBAL              0 (db)
+         742           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         742          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         743          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         747          58 LOAD_FAST                1 (conn)
+         748          58 LOAD_FAST                1 (conn)
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
          
-         741         142 LOAD_CONST               0 (None)
+         742         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3761,24 +3761,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         749     >>  188 LOAD_FAST                3 (result)
+         750     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         750         210 LOAD_CONST               0 (None)
+         751         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         752     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         753     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3786,15 +3786,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         753         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         754         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3807,15 +3807,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 740
+         firstlineno 741
          lnotab 0x02013401040554fa2e08160104028201
       'email'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3830,41 +3830,41 @@
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000006a0c00000000000000006a0d00000000000000007c
             04a6020000ab0200000000000000005300
-         756           0 RESUME                   0
+         757           0 RESUME                   0
          
-         757           2 LOAD_GLOBAL              0 (db)
+         758           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         758          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
+         759          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
                       56 STORE_FAST               2 (statement)
          
-         763          58 LOAD_FAST                1 (conn)
+         764          58 LOAD_FAST                1 (conn)
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
          
-         757         142 LOAD_CONST               0 (None)
+         758         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3875,24 +3875,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         765     >>  188 LOAD_FAST                3 (result)
+         766     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         766         210 LOAD_CONST               0 (None)
+         767         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         768     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         769     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3900,15 +3900,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         769         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         770         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (ts)
                      368 LOAD_ATTR               12 (models)
                      378 LOAD_ATTR               13 (Actor)
                      388 LOAD_FAST                4 (obj)
                      390 PRECALL                  2
                      394 CALL                     2
                      404 RETURN_VALUE
@@ -3923,15 +3923,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'ts', 'models', 'Actor')
          varnames   ('email', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_actor_by_email'
-         firstlineno 756
+         firstlineno 757
          lnotab 0x02013401040554fa2e08160104028201
       'event_id'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3945,41 +3945,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         772           0 RESUME                   0
+         773           0 RESUME                   0
          
-         773           2 LOAD_GLOBAL              0 (db)
+         774           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         774          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+         775          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         779          58 LOAD_FAST                1 (conn)
+         780          58 LOAD_FAST                1 (conn)
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
          
-         773         142 LOAD_CONST               0 (None)
+         774         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3990,24 +3990,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         781     >>  188 LOAD_FAST                3 (result)
+         782     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         782         210 LOAD_CONST               0 (None)
+         783         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         784     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         785     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -4015,15 +4015,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         785         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         786         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Event)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -4036,15 +4036,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
          varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
-         firstlineno 772
+         firstlineno 773
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 12
          flags     : 3
          code
@@ -4056,71 +4056,71 @@
             000000000000007c006a0800000000000000007c006a0900000000000000
             007415000000000000000000006a0b00000000000000007c006a0c000000
             0000000000a6010000ab01000000000000000064029c06a6020000ab0200
             0000000000000001007c01a00d0000000000000000000000000000000000
             000000a6000000ab0000000000000000000100640064006400a6020000ab
             020000000000000000010064005300230031007304770278035900770101
             0059000100010064005300
-         791           0 RESUME                   0
+         792           0 RESUME                   0
          
-         792           2 LOAD_GLOBAL              0 (db)
+         793           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         793          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
+         794          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         805          58 LOAD_FAST                1 (conn)
+         806          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         806          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         807          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         808         120 LOAD_FAST                0 (company)
+         809         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (uid)
          
-         809         132 LOAD_FAST                0 (company)
+         810         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (name)
          
-         810         144 LOAD_FAST                0 (company)
+         811         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (description)
          
-         811         156 LOAD_FAST                0 (company)
+         812         156 LOAD_FAST                0 (company)
                      158 LOAD_ATTR                8 (domain)
          
-         812         168 LOAD_FAST                0 (company)
+         813         168 LOAD_FAST                0 (company)
                      170 LOAD_ATTR                9 (source)
          
-         813         180 LOAD_GLOBAL             21 (NULL + json)
+         814         180 LOAD_GLOBAL             21 (NULL + json)
                      192 LOAD_ATTR               11 (dumps)
                      202 LOAD_FAST                0 (company)
                      204 LOAD_ATTR               12 (meta)
                      214 PRECALL                  1
                      218 CALL                     1
          
-         807         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
+         808         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
                      230 BUILD_CONST_KEY_MAP      6
          
-         805         232 PRECALL                  2
+         806         232 PRECALL                  2
                      236 CALL                     2
                      246 POP_TOP
          
-         817         248 LOAD_FAST                1 (conn)
+         818         248 LOAD_FAST                1 (conn)
                      250 LOAD_METHOD             13 (commit)
                      272 PRECALL                  0
                      276 CALL                     0
                      286 POP_TOP
          
-         792         288 LOAD_CONST               0 (None)
+         793         288 LOAD_CONST               0 (None)
                      290 LOAD_CONST               0 (None)
                      292 LOAD_CONST               0 (None)
                      294 PRECALL                  2
                      298 CALL                     2
                      308 POP_TOP
                      310 LOAD_CONST               0 (None)
                      312 RETURN_VALUE
@@ -4147,15 +4147,15 @@
             ('uid', 'name', 'description', 'domain', 'source', 'meta')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'uid', 'name', 'description', 'domain', 'source', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 791
+         firstlineno 792
          lnotab 0x02013401040c180126020c010c010c010c010c0130fa04fe100c28e7
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
@@ -4165,58 +4165,58 @@
             006a0400000000000000006401a6010000ab010000000000000000740b00
             0000000000000000006a0600000000000000007c006a0700000000000000
             00a6010000ab0100000000000000007c006a08000000000000000064029c
             02a6020000ab02000000000000000001007c01a009000000000000000000
             0000000000000000000000a6000000ab0000000000000000000100640064
             006400a6020000ab02000000000000000001006400530023003100730477
             02780359007701010059000100010064005300
-         820           0 RESUME                   0
+         821           0 RESUME                   0
          
-         821           2 LOAD_GLOBAL              0 (db)
+         822           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         822          54 LOAD_FAST                1 (conn)
+         823          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         823          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         824          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         824         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
+         825         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
          
-         823         102 PRECALL                  1
+         824         102 PRECALL                  1
                      106 CALL                     1
          
-         833         116 LOAD_GLOBAL             11 (NULL + json)
+         834         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (meta)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         834         164 LOAD_FAST                0 (search)
+         835         164 LOAD_FAST                0 (search)
                      166 LOAD_ATTR                8 (uid)
          
-         832         176 LOAD_CONST               2 (('meta', 'uid'))
+         833         176 LOAD_CONST               2 (('meta', 'uid'))
                      178 BUILD_CONST_KEY_MAP      2
          
-         822         180 PRECALL                  2
+         823         180 PRECALL                  2
                      184 CALL                     2
                      194 POP_TOP
          
-         837         196 LOAD_FAST                1 (conn)
+         838         196 LOAD_FAST                1 (conn)
                      198 LOAD_METHOD              9 (commit)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 POP_TOP
          
-         821         236 LOAD_CONST               0 (None)
+         822         236 LOAD_CONST               0 (None)
                      238 LOAD_CONST               0 (None)
                      240 LOAD_CONST               0 (None)
                      242 PRECALL                  2
                      246 CALL                     2
                      256 POP_TOP
                      258 LOAD_CONST               0 (None)
                      260 RETURN_VALUE
@@ -4243,15 +4243,15 @@
             ('meta', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'meta', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 820
+         firstlineno 821
          lnotab 0x020134011801160102ff0e0a30010cfe04f6100f28f0
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4262,61 +4262,61 @@
             006901a6020000ab02000000000000000001007c01a00200000000000000
             000000000000000000000000007407000000000000000000006a04000000
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00500000000000000000000000000000000000000
             00a6000000ab0000000000000000000100640064006400a6020000ab0200
             000000000000000100640053002300310073047702780359007701010059
             000100010064005300
-         843           0 RESUME                   0
+         844           0 RESUME                   0
          
-         845           2 LOAD_GLOBAL              0 (db)
+         846           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         846          54 LOAD_FAST                1 (conn)
+         847          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         847          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         848          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         848         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
+         849         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
          
-         847         102 PRECALL                  1
+         848         102 PRECALL                  1
                      106 CALL                     1
          
-         856         116 LOAD_CONST               2 ('event_id')
+         857         116 LOAD_CONST               2 ('event_id')
                      118 LOAD_FAST                0 (event_id)
          
-         855         120 BUILD_MAP                1
+         856         120 BUILD_MAP                1
          
-         846         122 PRECALL                  2
+         847         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         859         138 LOAD_FAST                1 (conn)
+         860         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         860         216 LOAD_FAST                1 (conn)
+         861         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              5 (commit)
                      240 PRECALL                  0
                      244 CALL                     0
                      254 POP_TOP
          
-         845         256 LOAD_CONST               0 (None)
+         846         256 LOAD_CONST               0 (None)
                      258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 PRECALL                  2
                      266 CALL                     2
                      276 POP_TOP
                      278 LOAD_CONST               0 (None)
                      280 RETURN_VALUE
@@ -4344,15 +4344,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('event_id', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'mute_event'
-         firstlineno 843
+         firstlineno 844
          lnotab 0x020234011801160102ff0e0904ff02f7100d4e0128f1
       'comment_id'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -4364,58 +4364,58 @@
             0064027c006901a6020000ab02000000000000000001007c01a002000000
             00000000000000000000000000000000007407000000000000000000006a
             0400000000000000006403a6010000ab010000000000000000a6010000ab
             01000000000000000001007c01a005000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-         866           0 RESUME                   0
+         867           0 RESUME                   0
          
-         867           2 LOAD_GLOBAL              0 (db)
+         868           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         868          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
+         869          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         872          58 LOAD_FAST                1 (conn)
+         873          58 LOAD_FAST                1 (conn)
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
          
-         873         142 LOAD_FAST                1 (conn)
+         874         142 LOAD_FAST                1 (conn)
                      144 LOAD_METHOD              2 (execute)
                      166 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      178 LOAD_ATTR                4 (text)
                      188 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      190 PRECALL                  1
                      194 CALL                     1
                      204 PRECALL                  1
                      208 CALL                     1
                      218 POP_TOP
          
-         874         220 LOAD_FAST                1 (conn)
+         875         220 LOAD_FAST                1 (conn)
                      222 LOAD_METHOD              5 (commit)
                      244 PRECALL                  0
                      248 CALL                     0
                      258 POP_TOP
          
-         867         260 LOAD_CONST               0 (None)
+         868         260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 LOAD_CONST               0 (None)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 POP_TOP
                      282 LOAD_CONST               0 (None)
                      284 RETURN_VALUE
@@ -4443,15 +4443,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('comment_id', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'delete_comment'
-         firstlineno 866
+         firstlineno 867
          lnotab 0x02013401040454014e0128f9
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4464,71 +4464,71 @@
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00200000000000000000000000000000000000000
             007407000000000000000000006a0400000000000000006404a6010000ab
             010000000000000000a6010000ab01000000000000000001007c01a00500
             00000000000000000000000000000000000000a6000000ab000000000000
             0000000100640064006400a6020000ab0200000000000000000100640053
             002300310073047702780359007701010059000100010064005300
-         877           0 RESUME                   0
+         878           0 RESUME                   0
          
-         881           2 LOAD_GLOBAL              0 (db)
+         882           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         882          54 LOAD_FAST                1 (conn)
+         883          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         883          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         884          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         884         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
+         885         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
          
-         883         102 PRECALL                  1
+         884         102 PRECALL                  1
                      106 CALL                     1
          
-         890         116 LOAD_CONST               2 ('search_uid')
+         891         116 LOAD_CONST               2 ('search_uid')
                      118 LOAD_FAST                0 (search_uid)
                      120 BUILD_MAP                1
          
-         882         122 PRECALL                  2
+         883         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         892         138 LOAD_FAST                1 (conn)
+         893         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         893         216 LOAD_FAST                1 (conn)
+         894         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              2 (execute)
                      240 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      252 LOAD_ATTR                4 (text)
                      262 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW rating')
                      264 PRECALL                  1
                      268 CALL                     1
                      278 PRECALL                  1
                      282 CALL                     1
                      292 POP_TOP
          
-         896         294 LOAD_FAST                1 (conn)
+         897         294 LOAD_FAST                1 (conn)
                      296 LOAD_METHOD              5 (commit)
                      318 PRECALL                  0
                      322 CALL                     0
                      332 POP_TOP
          
-         881         334 LOAD_CONST               0 (None)
+         882         334 LOAD_CONST               0 (None)
                      336 LOAD_CONST               0 (None)
                      338 LOAD_CONST               0 (None)
                      340 PRECALL                  2
                      344 CALL                     2
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
@@ -4557,22 +4557,22 @@
             'REFRESH MATERIALIZED VIEW rating'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('search_uid', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'reset_inbox'
-         firstlineno 877
+         firstlineno 878
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
-      7f00051a161a0c1a1e1a1d241c2409101010101013101d10171017100b
+      7f00061a161a0c1a1e1a1d241c2409101010101013101d10171017100b
```

### Comparing `gandai-1.7.44/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.45/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xee5c3966 (Mon May  6 22:42:54 2024 UTC)
+moddate:  0xe90b5066 (Fri May 24 03:39:21 2024 UTC)
 files sz: 1079
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `gandai-1.7.44/gandai/analytics.py` & `gandai-1.7.45/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/constants.py` & `gandai-1.7.45/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/db.py` & `gandai-1.7.45/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/google.py` & `gandai-1.7.45/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/gpt.py` & `gandai-1.7.45/gandai/gpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,44 +37,47 @@
     "data": {
         "contact_name": "Bob"
     }
 }
 
 Here are all the fields you can use for event['data']
 
-c.meta->>'description' as description, -- a description of the company for use by private equity research analyst to understand the company.
-c.meta->>'employees' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.
-c.meta->>'ownership' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] 
-c.meta->>'headquarters' as headquarters,
-c.meta->>'city' as city,
-c.meta->>'state' as state,
-c.meta->>'designation' as designation,
-c.meta->>'products' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.
-c.meta->>'services' as services, -- services are intangible goods offered by the company. do not list products here.
-c.meta->>'end_customer' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.
-c.meta->>'geographies' as geographies, -- geographies are the areas where the company does business. 
-c.meta->>'year_founded' as year_founded,
-c.meta->>'linkedin' as linkedin, -- linkedinUrl 
-c.meta->>'linkedin_range' as linkedin_range,
-c.meta->>'industry' as industry,
-c.meta->>'revenue_estimates' as revenue_estimates,
-c.meta->>'location_count' as location_count,
-c.meta->>'business_models' as business_models,
-c.meta->>'facility_size' as facility_size,
-c.meta->>'contact_name' as contact_name,
-c.meta->>'contact_title' as contact_title,
-c.meta->>'contact_email' as contact_email,
-c.meta->>'contact_phone' as contact_phone,
-c.meta->>'contact_address' as contact_address,
+c.data->>'gpt_description' as gpt_description, -- a description of the company for use by private equity research analyst to understand the company.
+
+You will fill out the description field with a description of the company. 
+The description will be a comprehensive description of the company for use 
+by private equity research analyst to understand the company.
+
+c.data->>'employees' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.
+c.data->>'ownership' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] 
+c.data->>'headquarters' as headquarters,
+c.data->>'city' as city,
+c.data->>'state' as state,
+c.data->>'designation' as designation,
+c.data->>'products' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.
+c.data->>'services' as services, -- services are intangible goods offered by the company. do not list products here.
+c.data->>'end_customer' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.
+c.data->>'geographies' as geographies, -- geographies are the areas where the company does business. 
+c.data->>'year_founded' as year_founded,
+c.data->>'linkedin' as linkedin, -- linkedinUrl 
+c.data->>'linkedin_range' as linkedin_range,
+c.data->>'industry' as industry,
+c.data->>'revenue_estimates' as revenue_estimates,
+c.data->>'location_count' as location_count,
+c.data->>'business_models' as business_models,
+c.data->>'facility_size' as facility_size,
+c.data->>'contact_name' as contact_name,
+c.data->>'contact_title' as contact_title,
+c.data->>'contact_email' as contact_email,
+c.data->>'contact_phone' as contact_phone,
+c.data->>'contact_address' as contact_address,
 
 For fields that are lists, you will use a csv string 
 For these lists, such as products or services, try to stick to top 5 or less areas of focus.
 
-You will fill out the description field with a description of the company. 
-The description will be a comprehensive description of the company for use by private equity research analyst to understand the company.
 
 If you are unsure, just leave that key out of the response data
 
 """
 
 
 HOW_TO_RESPOND = """
```

### Comparing `gandai-1.7.44/gandai/grata.py` & `gandai-1.7.45/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/helpers.py` & `gandai-1.7.45/gandai/helpers.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/main.py` & `gandai-1.7.45/gandai/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from time import time
 from dataclasses import asdict
-from dacite import from_dict
+from time import time
 
 import gandai as ts
+from dacite import from_dict
 
 
 def run_acquired_check(domain: str):
     company = ts.query.find_company_by_domain(domain)
     q = f"{company.name} was acquired"
     google_page_one = ts.google.search(q)  # top 10 results, could extend?
     messages = [
@@ -39,15 +39,14 @@
     updates: dict = ts.gpt.ask_gpt4(messages)
     print(updates)
     company.meta = {**company.meta, **updates}
     # this is where I could also make a comment
     ts.query.update_company(company)
 
 
-
 def run_similarity_search(search: ts.models.Search, domain: str) -> None:
     grata_companies = ts.grata.find_similar(domain=domain, search=search)
     ts.query.insert_companies_as_targets(
         companies=grata_companies,
         search_uid=search.uid,
         actor_key="grata",
         # force=True # ok
@@ -167,14 +166,15 @@
     for new_event in resp["events"]:
         print("new event:", new_event)
         e = from_dict(ts.models.Event, new_event)
         print(e)
         e.data["prompt"] = event.data["prompt"]
         ts.query.insert_event(e)
 
+
 def enrich_with_gpt(company: ts.models.Company) -> None:
     print("enriching with gpt...")
     homepage_text = ts.helpers.get_homepage_text(company.domain)
     messages = [
         {
             "role": "system",
             "content": f"You will help us evaluate {company.name} for acquisition.",
@@ -200,29 +200,33 @@
     resp = ts.gpt.ask_gpt4(messages)
     update_event = from_dict(ts.models.Event, resp)
     update_event.data["gpt"] = int(time())
     print(update_event)
     ts.query.insert_event(update_event)
     return resp
 
+
 def run_enrichment(event: ts.models.Event) -> None:
     domain = event.domain
     search_uid = event.search_uid
 
     company = ts.query.find_company_by_domain(domain)
     if company.meta.get("company_uid"):
         print("company already exists. skipping enrichment...")
     else:
         resp = ts.grata.enrich(company.domain)
         company.name = company.name or resp.get("name")
         company.description = resp.get("description")
         company.meta = {**company.meta, **resp}
         ts.query.update_company(company)
 
-    enrich_with_gpt(company=company)
+    if company.meta.get("gpt"):
+        print("company already enriched with gpt. skipping...")
+    else:
+        enrich_with_gpt(company=company)
 
 
 def process_event(event_id: int) -> None:
     print("processing event...")
     event: ts.models.Event = ts.query.find_event_by_id(event_id)
     print("event_id", event_id)
     print(event)
```

### Comparing `gandai-1.7.44/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.45/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/migrations/db_seed.py` & `gandai-1.7.45/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/migrations/dealcloud.py` & `gandai-1.7.45/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.45/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/migrations/sql/schema.sql` & `gandai-1.7.45/gandai/migrations/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/models.py` & `gandai-1.7.45/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/query.py` & `gandai-1.7.45/gandai/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,15 +493,16 @@
         e.domain, 
         e.type as stage, 
         e.created as updated, 
         to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,
         a.name as updated_by, 
         c.name, 
         c.description as grata_description,
-        c.meta->>'description' as description,
+        c.meta->>'description' as grata_description,
+        c.meta->>'gpt_description' as gpt_description,
         c.source,
         -- uh is this necessary?
         c.meta->>'ownership' as ownership, 
         c.meta->>'headquarters' as headquarters,
         c.meta->>'city' as city,
         c.meta->>'state' as state,
         c.meta->>'designation' as designation,
```

### Comparing `gandai-1.7.44/gandai/secrets.py` & `gandai-1.7.45/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai/tasks.py` & `gandai-1.7.45/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.44/gandai.egg-info/SOURCES.txt` & `gandai-1.7.45/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

