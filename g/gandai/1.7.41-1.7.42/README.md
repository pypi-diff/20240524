# Comparing `tmp/gandai-1.7.41.tar.gz` & `tmp/gandai-1.7.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.7.41.tar", last modified: Mon May  6 21:58:41 2024, max compression
+gzip compressed data, was "gandai-1.7.42.tar", last modified: Thu May 23 23:15:02 2024, max compression
```

## Comparing `gandai-1.7.41.tar` & `gandai-1.7.42.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 21:58:41.827045 gandai-1.7.41/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.41/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-06 21:58:41.826853 gandai-1.7.41/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 21:58:41.818615 gandai-1.7.41/gandai/
--rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.41/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 21:58:41.824355 gandai-1.7.41/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.41/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.41/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.41/gandai/__pycache__/analytics.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.41/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2600 2024-03-29 15:40:37.000000 gandai-1.7.41/gandai/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.41/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.41/gandai/__pycache__/db.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.41/gandai/__pycache__/google.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5002 2024-05-06 16:10:12.000000 gandai-1.7.41/gandai/__pycache__/gpt.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.41/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1394 2024-03-29 15:42:35.000000 gandai-1.7.41/gandai/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    19242 2024-05-06 21:55:03.000000 gandai-1.7.41/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    10448 2024-05-06 20:32:25.000000 gandai-1.7.41/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    41771 2024-05-06 21:57:41.000000 gandai-1.7.41/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.41/gandai/__pycache__/secrets.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.41/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.41/gandai/__pycache__/sources.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1695 2024-05-06 21:58:10.000000 gandai-1.7.41/gandai/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.41/gandai/analytics.py
--rw-r--r--   0 parker     (501) staff       (20)     1674 2024-03-29 15:34:07.000000 gandai-1.7.41/gandai/constants.py
--rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.41/gandai/db.py
--rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.41/gandai/google.py
--rw-r--r--   0 parker     (501) staff       (20)     4216 2024-05-06 16:10:07.000000 gandai-1.7.41/gandai/gpt.py
--rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.41/gandai/grata.py
--rw-r--r--   0 parker     (501) staff       (20)      452 2024-03-29 15:34:07.000000 gandai-1.7.41/gandai/helpers.py
--rw-r--r--   0 parker     (501) staff       (20)    14528 2024-05-06 21:54:59.000000 gandai-1.7.41/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 21:58:41.825196 gandai-1.7.41/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.41/gandai/migrations/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 21:58:41.825569 gandai-1.7.41/gandai/migrations/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.41/gandai/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.41/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.41/gandai/migrations/db_create.py
--rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.41/gandai/migrations/db_seed.py
--rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.41/gandai/migrations/dealcloud.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 21:58:41.826355 gandai-1.7.41/gandai/migrations/sql/
--rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.41/gandai/migrations/sql/2305023-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.41/gandai/migrations/sql/230818-alter.sql
--rw-r--r--   0 parker     (501) staff       (20)     3342 2024-03-29 15:34:07.000000 gandai-1.7.41/gandai/migrations/sql/schema.sql
--rw-r--r--   0 parker     (501) staff       (20)     4381 2024-05-06 20:32:23.000000 gandai-1.7.41/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    28386 2024-05-06 21:57:39.000000 gandai-1.7.41/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.41/gandai/secrets.py
--rw-r--r--   0 parker     (501) staff       (20)     1079 2024-05-06 21:58:08.000000 gandai-1.7.41/gandai/tasks.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-06 21:58:41.826659 gandai-1.7.41/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-06 21:58:41.000000 gandai-1.7.41/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1478 2024-05-06 21:58:41.000000 gandai-1.7.41/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-06 21:58:41.000000 gandai-1.7.41/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-06 21:58:41.000000 gandai-1.7.41/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-06 21:58:35.000000 gandai-1.7.41/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-06 21:58:41.827082 gandai-1.7.41/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.41/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.588358 gandai-1.7.42/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-23 11:45:31.000000 gandai-1.7.42/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:15:02.588137 gandai-1.7.42/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.578137 gandai-1.7.42/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)      429 2023-11-27 12:36:32.000000 gandai-1.7.42/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.584892 gandai-1.7.42/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      750 2023-11-27 12:36:32.000000 gandai-1.7.42/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.7.42/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     8783 2024-03-29 15:43:44.000000 gandai-1.7.42/gandai/__pycache__/analytics.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4305 2023-07-27 20:57:55.000000 gandai-1.7.42/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2600 2024-03-29 15:40:37.000000 gandai-1.7.42/gandai/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4039 2023-06-06 18:24:16.000000 gandai-1.7.42/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2014 2024-03-29 15:42:35.000000 gandai-1.7.42/gandai/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2168 2023-11-20 15:35:11.000000 gandai-1.7.42/gandai/__pycache__/google.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7026 2024-05-23 22:33:44.000000 gandai-1.7.42/gandai/__pycache__/gpt.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5730 2023-11-29 03:59:25.000000 gandai-1.7.42/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2564 2024-05-23 22:34:21.000000 gandai-1.7.42/gandai/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    19281 2024-05-23 22:32:08.000000 gandai-1.7.42/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    10484 2024-05-23 19:36:53.000000 gandai-1.7.42/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    42225 2024-05-23 22:23:40.000000 gandai-1.7.42/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     2237 2023-11-20 15:35:11.000000 gandai-1.7.42/gandai/__pycache__/secrets.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.7.42/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    13620 2023-11-15 17:26:28.000000 gandai-1.7.42/gandai/__pycache__/sources.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1695 2024-05-07 15:22:26.000000 gandai-1.7.42/gandai/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5714 2024-03-29 15:34:07.000000 gandai-1.7.42/gandai/analytics.py
+-rw-r--r--   0 parker     (501) staff       (20)     1674 2024-03-29 15:34:07.000000 gandai-1.7.42/gandai/constants.py
+-rw-r--r--   0 parker     (501) staff       (20)     1202 2024-03-29 15:34:07.000000 gandai-1.7.42/gandai/db.py
+-rw-r--r--   0 parker     (501) staff       (20)     1036 2023-11-17 19:29:48.000000 gandai-1.7.42/gandai/google.py
+-rw-r--r--   0 parker     (501) staff       (20)     6384 2024-05-23 22:33:42.000000 gandai-1.7.42/gandai/gpt.py
+-rw-r--r--   0 parker     (501) staff       (20)     3969 2023-11-29 03:58:56.000000 gandai-1.7.42/gandai/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1204 2024-05-23 22:34:19.000000 gandai-1.7.42/gandai/helpers.py
+-rw-r--r--   0 parker     (501) staff       (20)    14648 2024-05-23 22:32:05.000000 gandai-1.7.42/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.585851 gandai-1.7.42/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.7.42/gandai/migrations/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.586341 gandai-1.7.42/gandai/migrations/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      190 2023-05-13 21:27:35.000000 gandai-1.7.42/gandai/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     6432 2023-05-23 12:06:36.000000 gandai-1.7.42/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      412 2023-07-17 18:25:43.000000 gandai-1.7.42/gandai/migrations/db_create.py
+-rw-r--r--   0 parker     (501) staff       (20)     1653 2023-07-17 18:25:43.000000 gandai-1.7.42/gandai/migrations/db_seed.py
+-rw-r--r--   0 parker     (501) staff       (20)     3258 2023-07-17 18:25:43.000000 gandai-1.7.42/gandai/migrations/dealcloud.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.587636 gandai-1.7.42/gandai/migrations/sql/
+-rw-r--r--   0 parker     (501) staff       (20)      168 2023-06-07 16:12:27.000000 gandai-1.7.42/gandai/migrations/sql/2305023-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1720 2023-09-05 16:26:02.000000 gandai-1.7.42/gandai/migrations/sql/230818-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)      136 2024-05-23 23:10:21.000000 gandai-1.7.42/gandai/migrations/sql/240523-alter.sql
+-rw-r--r--   0 parker     (501) staff       (20)     3355 2024-05-23 22:41:05.000000 gandai-1.7.42/gandai/migrations/sql/schema.sql
+-rw-r--r--   0 parker     (501) staff       (20)     4501 2024-05-23 19:36:50.000000 gandai-1.7.42/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    28619 2024-05-23 22:23:38.000000 gandai-1.7.42/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     1129 2023-11-17 19:29:48.000000 gandai-1.7.42/gandai/secrets.py
+-rw-r--r--   0 parker     (501) staff       (20)     1079 2024-05-06 22:42:54.000000 gandai-1.7.42/gandai/tasks.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2024-05-23 23:15:02.587915 gandai-1.7.42/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2024-05-23 23:15:02.000000 gandai-1.7.42/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1517 2024-05-23 23:15:02.000000 gandai-1.7.42/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2024-05-23 23:15:02.000000 gandai-1.7.42/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2024-05-23 23:15:02.000000 gandai-1.7.42/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      384 2024-05-23 23:14:45.000000 gandai-1.7.42/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2024-05-23 23:15:02.588397 gandai-1.7.42/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      157 2023-07-17 18:25:43.000000 gandai-1.7.42/setup.py
```

### Comparing `gandai-1.7.41/gandai/__pycache__/__init__.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/analytics.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/analytics.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/constants.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/db.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/db.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/google.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/google.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/main.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xb3513966 (Mon May  6 21:54:59 2024 UTC)
-files sz: 14528
+moddate:  0xe5c34f66 (Thu May 23 22:32:05 2024 UTC)
+files sz: 14648
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -87,96 +87,96 @@
                122 LOAD_CONST              10 ('return')
                124 LOAD_CONST               1 (None)
                126 BUILD_TUPLE              6
                128 LOAD_CONST              11 (<code object enrich_with_gpt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 49>)
                130 MAKE_FUNCTION            4 (annotations)
                132 STORE_NAME              19 (enrich_with_gpt)
    
-   157         134 LOAD_CONST              12 ('search')
+   160         134 LOAD_CONST              12 ('search')
                136 LOAD_NAME                8 (ts)
                138 LOAD_ATTR               16 (models)
                148 LOAD_ATTR               20 (Search)
                158 LOAD_CONST               6 ('domain')
                160 LOAD_NAME               14 (str)
                162 LOAD_CONST              10 ('return')
                164 LOAD_CONST               1 (None)
                166 BUILD_TUPLE              6
-               168 LOAD_CONST              13 (<code object run_similarity_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 157>)
+               168 LOAD_CONST              13 (<code object run_similarity_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 160>)
                170 MAKE_FUNCTION            4 (annotations)
                172 STORE_NAME              21 (run_similarity_search)
    
-   168         174 LOAD_CONST              12 ('search')
+   171         174 LOAD_CONST              12 ('search')
                176 LOAD_NAME                8 (ts)
                178 LOAD_ATTR               16 (models)
                188 LOAD_ATTR               20 (Search)
                198 LOAD_CONST              10 ('return')
                200 LOAD_CONST               1 (None)
                202 BUILD_TUPLE              4
-               204 LOAD_CONST              14 (<code object run_criteria_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 168>)
+               204 LOAD_CONST              14 (<code object run_criteria_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 171>)
                206 MAKE_FUNCTION            4 (annotations)
                208 STORE_NAME              22 (run_criteria_search)
    
-   181         210 LOAD_CONST              12 ('search')
+   184         210 LOAD_CONST              12 ('search')
                212 LOAD_NAME                8 (ts)
                214 LOAD_ATTR               16 (models)
                224 LOAD_ATTR               20 (Search)
                234 LOAD_CONST              15 ('event')
                236 LOAD_NAME                8 (ts)
                238 LOAD_ATTR               16 (models)
                248 LOAD_ATTR               23 (Event)
                258 LOAD_CONST              10 ('return')
                260 LOAD_CONST               1 (None)
                262 BUILD_TUPLE              6
-               264 LOAD_CONST              16 (<code object run_maps_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 181>)
+               264 LOAD_CONST              16 (<code object run_maps_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 184>)
                266 MAKE_FUNCTION            4 (annotations)
                268 STORE_NAME              24 (run_maps_search)
    
-   226         270 LOAD_CONST              12 ('search')
+   229         270 LOAD_CONST              12 ('search')
                272 LOAD_NAME                8 (ts)
                274 LOAD_ATTR               16 (models)
                284 LOAD_ATTR               20 (Search)
                294 LOAD_CONST              15 ('event')
                296 LOAD_NAME                8 (ts)
                298 LOAD_ATTR               16 (models)
                308 LOAD_ATTR               23 (Event)
                318 LOAD_CONST              10 ('return')
                320 LOAD_CONST               1 (None)
                322 BUILD_TUPLE              6
-               324 LOAD_CONST              17 (<code object run_google_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 226>)
+               324 LOAD_CONST              17 (<code object run_google_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 229>)
                326 MAKE_FUNCTION            4 (annotations)
                328 STORE_NAME              25 (run_google_search)
    
-   241         330 LOAD_CONST              15 ('event')
+   244         330 LOAD_CONST              15 ('event')
                332 LOAD_NAME                8 (ts)
                334 LOAD_ATTR               16 (models)
                344 LOAD_ATTR               23 (Event)
                354 LOAD_CONST              10 ('return')
                356 LOAD_CONST               1 (None)
                358 BUILD_TUPLE              4
-               360 LOAD_CONST              18 (<code object handle_prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 241>)
+               360 LOAD_CONST              18 (<code object handle_prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 244>)
                362 MAKE_FUNCTION            4 (annotations)
                364 STORE_NAME              26 (handle_prompt)
    
-   285         366 LOAD_CONST              15 ('event')
+   288         366 LOAD_CONST              15 ('event')
                368 LOAD_NAME                8 (ts)
                370 LOAD_ATTR               16 (models)
                380 LOAD_ATTR               23 (Event)
                390 LOAD_CONST              10 ('return')
                392 LOAD_CONST               1 (None)
                394 BUILD_TUPLE              4
-               396 LOAD_CONST              19 (<code object run_enrichment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 285>)
+               396 LOAD_CONST              19 (<code object run_enrichment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 288>)
                398 MAKE_FUNCTION            4 (annotations)
                400 STORE_NAME              27 (run_enrichment)
    
-   303         402 LOAD_CONST              20 ('event_id')
+   306         402 LOAD_CONST              20 ('event_id')
                404 LOAD_NAME               18 (int)
                406 LOAD_CONST              10 ('return')
                408 LOAD_CONST               1 (None)
                410 BUILD_TUPLE              4
-               412 LOAD_CONST              21 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 303>)
+               412 LOAD_CONST              21 (<code object process_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 306>)
                414 MAKE_FUNCTION            4 (annotations)
                416 STORE_NAME              28 (process_event)
                418 LOAD_CONST               1 (None)
                420 RETURN_VALUE
    consts
       0
       None
@@ -362,136 +362,132 @@
             0a7c006a0200000000000000009b00640b9d03640c9c026409640d740700
             0000000000000000007c00a6010000ab0100000000000000009b009d0264
             0c9c026409640e7c059b009d02640c9c026409640f640c9c0264107c0264
             0c9c0267057d067408000000000000000000006a050000000000000000a0
             0600000000000000000000000000000000000000007c06a6010000ab0100
             000000000000007d07740f00000000000000000000740800000000000000
             0000006a0800000000000000006a0900000000000000007c07a6020000ab
-            0200000000000000007d087c017c085f0a00000000000000007408000000
-            000000000000006a0b0000000000000000a00c0000000000000000000000
-            0000000000000000007c08a6010000ab01000000000000000001007c0753
-            00
+            0200000000000000007d087c017c085f0a00000000000000007417000000
+            000000000000007c08a6010000ab01000000000000000001007c075300
           49           0 RESUME                   0
          
-          51           2 LOAD_CONST               1 ('\n    To update an attribute for a company you will create an event with the company\'s domain\n    of type "update". This will update that company\'s meta field \n    here is an example \n\n    {\n\t\t"search_uid": 1,\n\t\t"domain": "lol.com",\n\t\t"actor_key": "chatgpt",\n\t\t"type": "update",\n\t\t"data": {\n\t\t\t"contact_name": "Bob"\n\t\t}\n\t}\n\n    Here are all the fields you can \n\n    c.meta->>\'description\' as description, -- a description of the company for use by private equity research analyst to understand the company.\n    c.meta->>\'employees\' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.\n    c.meta->>\'ownership\' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] \n    c.meta->>\'headquarters\' as headquarters,\n    c.meta->>\'city\' as city,\n    c.meta->>\'state\' as state,\n    c.meta->>\'designation\' as designation,\n    c.meta->>\'products\' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.\n    c.meta->>\'services\' as services, -- services are intangible goods offered by the company. do not list products here.\n    c.meta->>\'end_customer\' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.\n    c.meta->>\'geographies\' as geographies, -- geographies are the areas where the company does business. \n    c.meta->>\'year_founded\' as year_founded,\n    c.meta->>\'linkedin\' as linkedin, -- linkedinUrl \n    c.meta->>\'linkedin_range\' as linkedin_range,\n    c.meta->>\'industry\' as industry,\n    c.meta->>\'revenue_estimates\' as revenue_estimates,\n    c.meta->>\'location_count\' as location_count,\n    c.meta->>\'business_models\' as business_models,\n    c.meta->>\'facility_size\' as facility_size,\n    c.meta->>\'contact_name\' as contact_name,\n    c.meta->>\'contact_title\' as contact_title,\n    c.meta->>\'contact_email\' as contact_email,\n    c.meta->>\'contact_phone\' as contact_phone,\n    c.meta->>\'contact_address\' as contact_address,\n\n    For fields that are lists, you will use a csv string \n    For these lists, such as products or services, try to stick to top 5 or less areas of focus.\n\n    If you are unsure, just leave that key out of the response data\n\n    ')
+          51           2 LOAD_CONST               1 ('\n    To update an attribute for a company you will create an event with the company\'s domain\n    of type "update". This will update that company\'s meta field \n    here is an example \n\n    {\n\t\t"search_uid": 1,\n\t\t"domain": "lol.com",\n\t\t"actor_key": "chatgpt",\n\t\t"type": "update",\n\t\t"data": {\n\t\t\t"contact_name": "Bob"\n\t\t}\n\t}\n\n    Here are all the fields you can \n\n    c.meta->>\'description\' as description, -- a description of the company for use by private equity research analyst to understand the company.\n    c.meta->>\'employees\' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.\n    c.meta->>\'ownership\' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] \n    c.meta->>\'headquarters\' as headquarters,\n    c.meta->>\'city\' as city,\n    c.meta->>\'state\' as state,\n    c.meta->>\'designation\' as designation,\n    c.meta->>\'products\' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.\n    c.meta->>\'services\' as services, -- services are intangible goods offered by the company. do not list products here.\n    c.meta->>\'end_customer\' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.\n    c.meta->>\'geographies\' as geographies, -- geographies are the areas where the company does business. \n    c.meta->>\'year_founded\' as year_founded,\n    c.meta->>\'linkedin\' as linkedin, -- linkedinUrl \n    c.meta->>\'linkedin_range\' as linkedin_range,\n    c.meta->>\'industry\' as industry,\n    c.meta->>\'revenue_estimates\' as revenue_estimates,\n    c.meta->>\'location_count\' as location_count,\n    c.meta->>\'business_models\' as business_models,\n    c.meta->>\'facility_size\' as facility_size,\n    c.meta->>\'contact_name\' as contact_name,\n    c.meta->>\'contact_title\' as contact_title,\n    c.meta->>\'contact_email\' as contact_email,\n    c.meta->>\'contact_phone\' as contact_phone,\n    c.meta->>\'contact_address\' as contact_address,\n\n    For fields that are lists, you will use a csv string \n    For these lists, such as products or services, try to stick to top 5 or less areas of focus.\n\n    You will fill out the description field with a description of the company.\n    \n    If you are unsure, just leave that key out of the response data\n\n    ')
                        4 STORE_FAST               2 (HOW_TO_ENRICH)
          
-         101           6 LOAD_CONST               2 ('Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15')
+         103           6 LOAD_CONST               2 ('Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15')
          
-         102           8 LOAD_CONST               3 ('text/html')
+         104           8 LOAD_CONST               3 ('text/html')
          
-         103          10 LOAD_CONST               4 ('https://www.google.com')
+         105          10 LOAD_CONST               4 ('https://www.google.com')
          
-         100          12 LOAD_CONST               5 (('User-Agent', 'Accept', 'Referer'))
+         102          12 LOAD_CONST               5 (('User-Agent', 'Accept', 'Referer'))
                       14 BUILD_CONST_KEY_MAP      3
                       16 STORE_FAST               3 (HEADERS)
          
-         106          18 LOAD_CONST               6 ('domain')
+         108          18 LOAD_CONST               6 ('domain')
                       20 LOAD_GLOBAL              0 (str)
                       32 LOAD_CONST               7 ('return')
                       34 LOAD_GLOBAL              0 (str)
                       46 BUILD_TUPLE              4
-                      48 LOAD_CONST               8 (<code object get_homepage_text, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 106>)
+                      48 LOAD_CONST               8 (<code object get_homepage_text, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 108>)
                       50 MAKE_FUNCTION            4 (annotations)
                       52 STORE_FAST               4 (get_homepage_text)
          
-         124          54 PUSH_NULL
+         126          54 PUSH_NULL
                       56 LOAD_FAST                4 (get_homepage_text)
                       58 LOAD_FAST                0 (company)
                       60 LOAD_ATTR                1 (domain)
                       70 PRECALL                  1
                       74 CALL                     1
                       84 STORE_FAST               5 (homepage_text)
          
-         128          86 LOAD_CONST               9 ('system')
+         130          86 LOAD_CONST               9 ('system')
          
-         129          88 LOAD_CONST              10 ('You will help us evaluate ')
+         131          88 LOAD_CONST              10 ('You will help us evaluate ')
                       90 LOAD_FAST                0 (company)
                       92 LOAD_ATTR                2 (name)
                      102 FORMAT_VALUE             0
                      104 LOAD_CONST              11 (' for acquisition.')
                      106 BUILD_STRING             3
          
-         127         108 LOAD_CONST              12 (('role', 'content'))
+         129         108 LOAD_CONST              12 (('role', 'content'))
                      110 BUILD_CONST_KEY_MAP      2
          
-         132         112 LOAD_CONST               9 ('system')
+         134         112 LOAD_CONST               9 ('system')
          
-         133         114 LOAD_CONST              13 ('You will consider this existing information: ')
+         135         114 LOAD_CONST              13 ('You will consider this existing information: ')
                      116 LOAD_GLOBAL              7 (NULL + asdict)
                      128 LOAD_FAST                0 (company)
                      130 PRECALL                  1
                      134 CALL                     1
                      144 FORMAT_VALUE             0
                      146 BUILD_STRING             2
          
-         131         148 LOAD_CONST              12 (('role', 'content'))
+         133         148 LOAD_CONST              12 (('role', 'content'))
                      150 BUILD_CONST_KEY_MAP      2
          
-         136         152 LOAD_CONST               9 ('system')
+         138         152 LOAD_CONST               9 ('system')
          
-         137         154 LOAD_CONST              14 ('You will consider this copy from the company homepage as the most up to date. homepage_text: ')
+         139         154 LOAD_CONST              14 ('You will consider this copy from the company homepage as the most up to date. homepage_text: ')
                      156 LOAD_FAST                5 (homepage_text)
                      158 FORMAT_VALUE             0
                      160 BUILD_STRING             2
          
-         135         162 LOAD_CONST              12 (('role', 'content'))
+         137         162 LOAD_CONST              12 (('role', 'content'))
                      164 BUILD_CONST_KEY_MAP      2
          
-         140         166 LOAD_CONST               9 ('system')
+         142         166 LOAD_CONST               9 ('system')
          
-         141         168 LOAD_CONST              15 ('You will respond with only the JSON object.')
+         143         168 LOAD_CONST              15 ('You will respond with only the JSON object.')
          
-         139         170 LOAD_CONST              12 (('role', 'content'))
+         141         170 LOAD_CONST              12 (('role', 'content'))
                      172 BUILD_CONST_KEY_MAP      2
          
-         144         174 LOAD_CONST              16 ('user')
+         146         174 LOAD_CONST              16 ('user')
          
-         145         176 LOAD_FAST                2 (HOW_TO_ENRICH)
+         147         176 LOAD_FAST                2 (HOW_TO_ENRICH)
          
-         143         178 LOAD_CONST              12 (('role', 'content'))
+         145         178 LOAD_CONST              12 (('role', 'content'))
                      180 BUILD_CONST_KEY_MAP      2
          
-         126         182 BUILD_LIST               5
+         128         182 BUILD_LIST               5
                      184 STORE_FAST               6 (messages)
          
-         149         186 LOAD_GLOBAL              8 (ts)
+         151         186 LOAD_GLOBAL              8 (ts)
                      198 LOAD_ATTR                5 (gpt)
                      208 LOAD_METHOD              6 (ask_gpt4)
                      230 LOAD_FAST                6 (messages)
                      232 PRECALL                  1
                      236 CALL                     1
                      246 STORE_FAST               7 (resp)
          
-         150         248 LOAD_GLOBAL             15 (NULL + from_dict)
+         152         248 LOAD_GLOBAL             15 (NULL + from_dict)
                      260 LOAD_GLOBAL              8 (ts)
                      272 LOAD_ATTR                8 (models)
                      282 LOAD_ATTR                9 (Event)
                      292 LOAD_FAST                7 (resp)
                      294 PRECALL                  2
                      298 CALL                     2
                      308 STORE_FAST               8 (update_event)
          
-         151         310 LOAD_FAST                1 (search_uid)
+         153         310 LOAD_FAST                1 (search_uid)
                      312 LOAD_FAST                8 (update_event)
                      314 STORE_ATTR              10 (search_uid)
          
-         152         324 LOAD_GLOBAL              8 (ts)
-                     336 LOAD_ATTR               11 (query)
-                     346 LOAD_METHOD             12 (insert_event)
-                     368 LOAD_FAST                8 (update_event)
-                     370 PRECALL                  1
-                     374 CALL                     1
-                     384 POP_TOP
+         154         324 LOAD_GLOBAL             23 (NULL + print)
+                     336 LOAD_FAST                8 (update_event)
+                     338 PRECALL                  1
+                     342 CALL                     1
+                     352 POP_TOP
          
-         154         386 LOAD_FAST                7 (resp)
-                     388 RETURN_VALUE
+         157         354 LOAD_FAST                7 (resp)
+                     356 RETURN_VALUE
          consts
             None
-            '\n    To update an attribute for a company you will create an event with the company\'s domain\n    of type "update". This will update that company\'s meta field \n    here is an example \n\n    {\n\t\t"search_uid": 1,\n\t\t"domain": "lol.com",\n\t\t"actor_key": "chatgpt",\n\t\t"type": "update",\n\t\t"data": {\n\t\t\t"contact_name": "Bob"\n\t\t}\n\t}\n\n    Here are all the fields you can \n\n    c.meta->>\'description\' as description, -- a description of the company for use by private equity research analyst to understand the company.\n    c.meta->>\'employees\' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.\n    c.meta->>\'ownership\' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] \n    c.meta->>\'headquarters\' as headquarters,\n    c.meta->>\'city\' as city,\n    c.meta->>\'state\' as state,\n    c.meta->>\'designation\' as designation,\n    c.meta->>\'products\' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.\n    c.meta->>\'services\' as services, -- services are intangible goods offered by the company. do not list products here.\n    c.meta->>\'end_customer\' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.\n    c.meta->>\'geographies\' as geographies, -- geographies are the areas where the company does business. \n    c.meta->>\'year_founded\' as year_founded,\n    c.meta->>\'linkedin\' as linkedin, -- linkedinUrl \n    c.meta->>\'linkedin_range\' as linkedin_range,\n    c.meta->>\'industry\' as industry,\n    c.meta->>\'revenue_estimates\' as revenue_estimates,\n    c.meta->>\'location_count\' as location_count,\n    c.meta->>\'business_models\' as business_models,\n    c.meta->>\'facility_size\' as facility_size,\n    c.meta->>\'contact_name\' as contact_name,\n    c.meta->>\'contact_title\' as contact_title,\n    c.meta->>\'contact_email\' as contact_email,\n    c.meta->>\'contact_phone\' as contact_phone,\n    c.meta->>\'contact_address\' as contact_address,\n\n    For fields that are lists, you will use a csv string \n    For these lists, such as products or services, try to stick to top 5 or less areas of focus.\n\n    If you are unsure, just leave that key out of the response data\n\n    '
+            '\n    To update an attribute for a company you will create an event with the company\'s domain\n    of type "update". This will update that company\'s meta field \n    here is an example \n\n    {\n\t\t"search_uid": 1,\n\t\t"domain": "lol.com",\n\t\t"actor_key": "chatgpt",\n\t\t"type": "update",\n\t\t"data": {\n\t\t\t"contact_name": "Bob"\n\t\t}\n\t}\n\n    Here are all the fields you can \n\n    c.meta->>\'description\' as description, -- a description of the company for use by private equity research analyst to understand the company.\n    c.meta->>\'employees\' as employees, -- the INTEGER number of employees at the company. prefer the grata estimate. this is an integer.\n    c.meta->>\'ownership\' as ownership, -- one of ["bootstrapped","investor_backed","public","public_subsidiary","private_subsidiary","private_equity","private_equity_add_on"] \n    c.meta->>\'headquarters\' as headquarters,\n    c.meta->>\'city\' as city,\n    c.meta->>\'state\' as state,\n    c.meta->>\'designation\' as designation,\n    c.meta->>\'products\' as products, -- products are physical goods sold by the company. do not list services here. A brand is not a product, do not list brands here.\n    c.meta->>\'services\' as services, -- services are intangible goods offered by the company. do not list products here.\n    c.meta->>\'end_customer\' as end_customer, -- what types of customers does the company serve. If commercial, what industry(s). do not list specific customers here.\n    c.meta->>\'geographies\' as geographies, -- geographies are the areas where the company does business. \n    c.meta->>\'year_founded\' as year_founded,\n    c.meta->>\'linkedin\' as linkedin, -- linkedinUrl \n    c.meta->>\'linkedin_range\' as linkedin_range,\n    c.meta->>\'industry\' as industry,\n    c.meta->>\'revenue_estimates\' as revenue_estimates,\n    c.meta->>\'location_count\' as location_count,\n    c.meta->>\'business_models\' as business_models,\n    c.meta->>\'facility_size\' as facility_size,\n    c.meta->>\'contact_name\' as contact_name,\n    c.meta->>\'contact_title\' as contact_title,\n    c.meta->>\'contact_email\' as contact_email,\n    c.meta->>\'contact_phone\' as contact_phone,\n    c.meta->>\'contact_address\' as contact_address,\n\n    For fields that are lists, you will use a csv string \n    For these lists, such as products or services, try to stick to top 5 or less areas of focus.\n\n    You will fill out the description field with a description of the company.\n    \n    If you are unsure, just leave that key out of the response data\n\n    '
             'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15'
             'text/html'
             'https://www.google.com'
             ('User-Agent', 'Accept', 'Referer')
             'domain'
             'return'
             code
@@ -508,55 +504,55 @@
                   0200000000000000007d0259006e03780359007701740700000000000000
                   0000007c026a040000000000000000640aa6020000ab0200000000000000
                   007d037c036a040000000000000000a00500000000000000000000000000
                   00000000000000a6000000ab0000000000000000007d04740d0000000000
                   00000000006a070000000000000000640b640c7c04a6030000ab03000000
                   00000000007d047405000000000000000000007c04a6010000ab01000000
                   000000000001007c045300
-               106           0 RESUME                   0
+               108           0 RESUME                   0
                
-               108           2 LOAD_CONST               1 ('Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15')
+               110           2 LOAD_CONST               1 ('Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15')
                
-               109           4 LOAD_CONST               2 ('text/html')
+               111           4 LOAD_CONST               2 ('text/html')
                
-               110           6 LOAD_CONST               3 ('https://www.google.com')
+               112           6 LOAD_CONST               3 ('https://www.google.com')
                
-               107           8 LOAD_CONST               4 (('User-Agent', 'Accept', 'Referer'))
+               109           8 LOAD_CONST               4 (('User-Agent', 'Accept', 'Referer'))
                             10 BUILD_CONST_KEY_MAP      3
                             12 STORE_FAST               1 (HEADERS)
                
-               112          14 NOP
+               114          14 NOP
                
-               113          16 LOAD_GLOBAL              1 (NULL + requests)
+               115          16 LOAD_GLOBAL              1 (NULL + requests)
                             28 LOAD_ATTR                1 (get)
                             38 LOAD_CONST               5 ('http://www.')
                             40 LOAD_FAST                0 (domain)
                             42 FORMAT_VALUE             0
                             44 BUILD_STRING             2
                             46 LOAD_FAST                1 (HEADERS)
                             48 KW_NAMES                 6
                             50 PRECALL                  2
                             54 CALL                     2
                             64 STORE_FAST               2 (resp)
                             66 JUMP_FORWARD            51 (to 170)
                        >>   68 PUSH_EXC_INFO
                
-               114          70 POP_TOP
+               116          70 POP_TOP
                
-               115          72 LOAD_GLOBAL              5 (NULL + print)
+               117          72 LOAD_GLOBAL              5 (NULL + print)
                             84 LOAD_CONST               7 ('failed on www.')
                             86 LOAD_FAST                0 (domain)
                             88 FORMAT_VALUE             0
                             90 LOAD_CONST               8 ('\ntrying without www')
                             92 BUILD_STRING             3
                             94 PRECALL                  1
                             98 CALL                     1
                            108 POP_TOP
                
-               116         110 LOAD_GLOBAL              1 (NULL + requests)
+               118         110 LOAD_GLOBAL              1 (NULL + requests)
                            122 LOAD_ATTR                1 (get)
                            132 LOAD_CONST               9 ('http://')
                            134 LOAD_FAST                0 (domain)
                            136 FORMAT_VALUE             0
                            138 BUILD_STRING             2
                            140 LOAD_FAST                1 (HEADERS)
                            142 KW_NAMES                 6
@@ -565,45 +561,45 @@
                            158 STORE_FAST               2 (resp)
                            160 POP_EXCEPT
                            162 JUMP_FORWARD             3 (to 170)
                        >>  164 COPY                     3
                            166 POP_EXCEPT
                            168 RERAISE                  1
                
-               118     >>  170 LOAD_GLOBAL              7 (NULL + BeautifulSoup)
+               120     >>  170 LOAD_GLOBAL              7 (NULL + BeautifulSoup)
                            182 LOAD_FAST                2 (resp)
                            184 LOAD_ATTR                4 (text)
                            194 LOAD_CONST              10 ('html.parser')
                            196 PRECALL                  2
                            200 CALL                     2
                            210 STORE_FAST               3 (soup)
                
-               119         212 LOAD_FAST                3 (soup)
+               121         212 LOAD_FAST                3 (soup)
                            214 LOAD_ATTR                4 (text)
                            224 LOAD_METHOD              5 (strip)
                            246 PRECALL                  0
                            250 CALL                     0
                            260 STORE_FAST               4 (homepage_text)
                
-               120         262 LOAD_GLOBAL             13 (NULL + re)
+               122         262 LOAD_GLOBAL             13 (NULL + re)
                            274 LOAD_ATTR                7 (sub)
                            284 LOAD_CONST              11 ('\\s+')
                            286 LOAD_CONST              12 (' ')
                            288 LOAD_FAST                4 (homepage_text)
                            290 PRECALL                  3
                            294 CALL                     3
                            304 STORE_FAST               4 (homepage_text)
                
-               121         306 LOAD_GLOBAL              5 (NULL + print)
+               123         306 LOAD_GLOBAL              5 (NULL + print)
                            318 LOAD_FAST                4 (homepage_text)
                            320 PRECALL                  1
                            324 CALL                     1
                            334 POP_TOP
                
-               122         336 LOAD_FAST                4 (homepage_text)
+               124         336 LOAD_FAST                4 (homepage_text)
                            338 RETURN_VALUE
                ExceptionTable:
                  16 to 64 -> 68 [0]
                  68 to 158 -> 164 [1] lasti
                consts
                   None
                   'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15'
@@ -620,76 +616,76 @@
                   ' '
                names      ('requests', 'get', 'print', 'BeautifulSoup', 'text', 'strip', 're', 'sub')
                varnames   ('domain', 'HEADERS', 'resp', 'soup', 'homepage_text')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
                name       'get_homepage_text'
-               firstlineno 106
+               firstlineno 108
                lnotab 0x02020201020102fd060502013601020126013c022a0132012c011e01
             'system'
             'You will help us evaluate '
             ' for acquisition.'
             ('role', 'content')
             'You will consider this existing information: '
             'You will consider this copy from the company homepage as the most up to date. homepage_text: '
             'You will respond with only the JSON object.'
             'user'
-         names      ('str', 'domain', 'name', 'asdict', 'ts', 'gpt', 'ask_gpt4', 'from_dict', 'models', 'Event', 'search_uid', 'query', 'insert_event')
+         names      ('str', 'domain', 'name', 'asdict', 'ts', 'gpt', 'ask_gpt4', 'from_dict', 'models', 'Event', 'search_uid', 'print')
          varnames   ('company', 'search_uid', 'HOW_TO_ENRICH', 'HEADERS', 'get_homepage_text', 'homepage_text', 'messages', 'resp', 'update_event')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'enrich_with_gpt'
          firstlineno 49
          lnotab
-            0x020204320201020102fd060624122004020114fe0405020122fe040502
-            0108fe0405020102fe0405020102fe04ef04173e013e010e013e02
+            0x020204340201020102fd060624122004020114fe0405020122fe040502
+            0108fe0405020102fe0405020102fe04ef04173e013e010e011e03
       'search'
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 7
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007c017c00ac01a6020000ab0200
             000000000000007d027400000000000000000000006a0300000000000000
             00a00400000000000000000000000000000000000000007c027c006a0500
             00000000000000640264037c019b009d02ac04a6040000ab040000000000
             000000010064005300
-         157           0 RESUME                   0
+         160           0 RESUME                   0
          
-         158           2 LOAD_GLOBAL              0 (ts)
+         161           2 LOAD_GLOBAL              0 (ts)
                       14 LOAD_ATTR                1 (grata)
                       24 LOAD_METHOD              2 (find_similar)
                       46 LOAD_FAST                1 (domain)
                       48 LOAD_FAST                0 (search)
                       50 KW_NAMES                 1
                       52 PRECALL                  2
                       56 CALL                     2
                       66 STORE_FAST               2 (grata_companies)
          
-         159          68 LOAD_GLOBAL              0 (ts)
+         162          68 LOAD_GLOBAL              0 (ts)
                       80 LOAD_ATTR                3 (query)
                       90 LOAD_METHOD              4 (insert_companies_as_targets)
          
-         160         112 LOAD_FAST                2 (grata_companies)
+         163         112 LOAD_FAST                2 (grata_companies)
          
-         161         114 LOAD_FAST                0 (search)
+         164         114 LOAD_FAST                0 (search)
                      116 LOAD_ATTR                5 (uid)
          
-         162         126 LOAD_CONST               2 ('grata')
+         165         126 LOAD_CONST               2 ('grata')
          
-         164         128 LOAD_CONST               3 ('grata/')
+         167         128 LOAD_CONST               3 ('grata/')
                      130 LOAD_FAST                1 (domain)
                      132 FORMAT_VALUE             0
                      134 BUILD_STRING             2
          
-         159         136 KW_NAMES                 4
+         162         136 KW_NAMES                 4
                      138 PRECALL                  4
                      142 CALL                     4
                      152 POP_TOP
                      154 LOAD_CONST               0 (None)
                      156 RETURN_VALUE
          consts
             None
@@ -699,54 +695,54 @@
             ('companies', 'search_uid', 'actor_key', 'source')
          names      ('ts', 'grata', 'find_similar', 'query', 'insert_companies_as_targets', 'uid')
          varnames   ('search', 'domain', 'grata_companies')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_similarity_search'
-         firstlineno 157
+         firstlineno 160
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
-         168           0 RESUME                   0
+         171           0 RESUME                   0
          
-         171           2 LOAD_GLOBAL              0 (ts)
+         174           2 LOAD_GLOBAL              0 (ts)
                       14 LOAD_ATTR                1 (grata)
                       24 LOAD_METHOD              2 (find_by_criteria)
                       46 LOAD_FAST                0 (search)
                       48 PRECALL                  1
                       52 CALL                     1
                       62 STORE_FAST               1 (grata_companies)
          
-         172          64 LOAD_GLOBAL              0 (ts)
+         175          64 LOAD_GLOBAL              0 (ts)
                       76 LOAD_ATTR                3 (query)
                       86 LOAD_METHOD              4 (insert_companies_as_targets)
          
-         173         108 LOAD_FAST                1 (grata_companies)
+         176         108 LOAD_FAST                1 (grata_companies)
          
-         174         110 LOAD_FAST                0 (search)
+         177         110 LOAD_FAST                0 (search)
                      112 LOAD_ATTR                5 (uid)
          
-         175         122 LOAD_CONST               1 ('grata')
+         178         122 LOAD_CONST               1 ('grata')
          
-         176         124 LOAD_CONST               2 (True)
+         179         124 LOAD_CONST               2 (True)
          
-         177         126 LOAD_CONST               1 ('grata')
+         180         126 LOAD_CONST               1 ('grata')
          
-         172         128 KW_NAMES                 3
+         175         128 KW_NAMES                 3
                      130 PRECALL                  5
                      134 CALL                     5
                      144 POP_TOP
                      146 LOAD_CONST               0 (None)
                      148 RETURN_VALUE
          consts
             None
@@ -755,15 +751,15 @@
             ('companies', 'search_uid', 'actor_key', 'force', 'source')
          names      ('ts', 'grata', 'find_by_criteria', 'query', 'insert_companies_as_targets', 'uid')
          varnames   ('search', 'grata_companies')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_criteria_search'
-         firstlineno 168
+         firstlineno 171
          lnotab 0x02033e012c0102010c010201020102fb
       'event'
       code
          argcount  : 2
          nlocals   : 6
          stacksize : 6
          flags     : 3
@@ -780,92 +776,92 @@
             0100000000000000007d047417000000000000000000007c04a6010000ab
             01000000000000000001007c04640319000000000000000000a00c000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             0044005d0f7d0502007c027c057c00ac09a6020000ab0200000000000000
             0001008c1064005300
                        0 MAKE_CELL                6 (existing_search_domains)
          
-         181           2 RESUME                   0
+         184           2 RESUME                   0
          
-         182           4 LOAD_GLOBAL              0 (ts)
+         185           4 LOAD_GLOBAL              0 (ts)
                       16 LOAD_ATTR                1 (query)
                       26 LOAD_METHOD              2 (search_targets)
                       48 LOAD_FAST                0 (search)
                       50 LOAD_ATTR                3 (uid)
                       60 KW_NAMES                 1
                       62 PRECALL                  1
                       66 CALL                     1
          
-         183          76 LOAD_CONST               2 ('domain')
+         186          76 LOAD_CONST               2 ('domain')
          
-         182          78 BINARY_SUBSCR
+         185          78 BINARY_SUBSCR
          
-         184          88 LOAD_METHOD              4 (to_list)
+         187          88 LOAD_METHOD              4 (to_list)
                      110 PRECALL                  0
                      114 CALL                     0
          
-         182         124 STORE_DEREF              6 (existing_search_domains)
+         185         124 STORE_DEREF              6 (existing_search_domains)
          
-         186         126 LOAD_CONST               3 ('place_id')
+         189         126 LOAD_CONST               3 ('place_id')
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
-                     184 LOAD_CONST               6 (<code object build_place, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 186>)
+                     184 LOAD_CONST               6 (<code object build_place, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 189>)
                      186 MAKE_FUNCTION           12 (annotations, closure)
                      188 STORE_FAST               2 (build_place)
          
-         217         190 LOAD_FAST                1 (event)
+         220         190 LOAD_FAST                1 (event)
                      192 LOAD_ATTR                8 (data)
                      202 LOAD_CONST               7 ('query')
                      204 BINARY_SUBSCR
                      214 STORE_FAST               3 (q)
          
-         218         216 LOAD_GLOBAL              0 (ts)
+         221         216 LOAD_GLOBAL              0 (ts)
                      228 LOAD_ATTR                9 (google)
                      238 LOAD_METHOD             10 (get_google_places)
                      260 LOAD_FAST                3 (q)
                      262 KW_NAMES                 8
                      264 PRECALL                  1
                      268 CALL                     1
                      278 STORE_FAST               4 (results)
          
-         219         280 LOAD_GLOBAL             23 (NULL + print)
+         222         280 LOAD_GLOBAL             23 (NULL + print)
                      292 LOAD_FAST                4 (results)
                      294 PRECALL                  1
                      298 CALL                     1
                      308 POP_TOP
          
-         222         310 LOAD_FAST                4 (results)
+         225         310 LOAD_FAST                4 (results)
                      312 LOAD_CONST               3 ('place_id')
                      314 BINARY_SUBSCR
                      324 LOAD_METHOD             12 (tolist)
                      346 PRECALL                  0
                      350 CALL                     0
                      360 GET_ITER
                  >>  362 FOR_ITER                15 (to 394)
                      364 STORE_FAST               5 (place)
          
-         223         366 PUSH_NULL
+         226         366 PUSH_NULL
                      368 LOAD_FAST                2 (build_place)
                      370 LOAD_FAST                5 (place)
                      372 LOAD_FAST                0 (search)
                      374 KW_NAMES                 9
                      376 PRECALL                  2
                      380 CALL                     2
                      390 POP_TOP
                      392 JUMP_BACKWARD           16 (to 362)
          
-         222     >>  394 LOAD_CONST               0 (None)
+         225     >>  394 LOAD_CONST               0 (None)
                      396 RETURN_VALUE
          consts
             None
             ('search_uid',)
             'domain'
             'place_id'
             'search'
@@ -896,131 +892,131 @@
                   000000000000007c016a0f0000000000000000640a7c066a0d0000000000
                   000000640b640c7c036901ac0da6050000ab0500000000000000007d0774
                   00000000000000000000006a0a0000000000000000a01000000000000000
                   000000000000000000000000007c07a6010000ab01000000000000000001
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               186           2 RESUME                   0
+               189           2 RESUME                   0
                
-               187           4 LOAD_GLOBAL              0 (ts)
+               190           4 LOAD_GLOBAL              0 (ts)
                             16 LOAD_ATTR                1 (google)
                             26 LOAD_ATTR                2 (gmaps)
                             36 LOAD_METHOD              3 (place)
                
-               188          58 LOAD_FAST                0 (place_id)
+               191          58 LOAD_FAST                0 (place_id)
                             60 BUILD_LIST               0
                             62 LOAD_CONST               1 (('name', 'website', 'reviews'))
                             64 LIST_EXTEND              1
                
-               187          66 KW_NAMES                 2
+               190          66 KW_NAMES                 2
                             68 PRECALL                  2
                             72 CALL                     2
                             82 STORE_FAST               2 (resp)
                
-               190          84 LOAD_FAST                2 (resp)
+               193          84 LOAD_FAST                2 (resp)
                             86 LOAD_CONST               3 ('result')
                             88 BINARY_SUBSCR
                             98 STORE_FAST               3 (place)
                
-               191         100 LOAD_GLOBAL              0 (ts)
+               194         100 LOAD_GLOBAL              0 (ts)
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
                
-               192         200 LOAD_FAST                4 (domain)
+               195         200 LOAD_FAST                4 (domain)
                            202 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 208)
                
-               193         204 LOAD_CONST               0 (None)
+               196         204 LOAD_CONST               0 (None)
                            206 RETURN_VALUE
                
-               194     >>  208 LOAD_FAST                4 (domain)
+               197     >>  208 LOAD_FAST                4 (domain)
                            210 LOAD_DEREF               8 (existing_search_domains)
                            212 CONTAINS_OP              0
                            214 POP_JUMP_FORWARD_IF_FALSE    21 (to 258)
                
-               195         216 LOAD_GLOBAL             15 (NULL + print)
+               198         216 LOAD_GLOBAL             15 (NULL + print)
                            228 LOAD_CONST               5 ('domain ')
                            230 LOAD_FAST                4 (domain)
                            232 FORMAT_VALUE             0
                            234 LOAD_CONST               6 (' already in search. skipping...')
                            236 BUILD_STRING             3
                            238 PRECALL                  1
                            242 CALL                     1
                            252 POP_TOP
                
-               196         254 LOAD_CONST               0 (None)
+               199         254 LOAD_CONST               0 (None)
                            256 RETURN_VALUE
                
-               197     >>  258 LOAD_GLOBAL              0 (ts)
+               200     >>  258 LOAD_GLOBAL              0 (ts)
                            270 LOAD_ATTR                8 (models)
                            280 LOAD_METHOD              9 (Company)
                
-               198         302 LOAD_FAST                3 (place)
+               201         302 LOAD_FAST                3 (place)
                            304 LOAD_CONST               7 ('name')
                            306 BINARY_SUBSCR
                
-               199         316 LOAD_FAST                4 (domain)
+               202         316 LOAD_FAST                4 (domain)
                
-               200         318 LOAD_CONST               8 ('Map API')
+               203         318 LOAD_CONST               8 ('Map API')
                
-               197         320 KW_NAMES                 9
+               200         320 KW_NAMES                 9
                            322 PRECALL                  3
                            326 CALL                     3
                            336 STORE_FAST               5 (new_company)
                
-               202         338 LOAD_GLOBAL              0 (ts)
+               205         338 LOAD_GLOBAL              0 (ts)
                            350 LOAD_ATTR               10 (query)
                            360 LOAD_METHOD             11 (insert_company)
                            382 LOAD_FAST                5 (new_company)
                            384 PRECALL                  1
                            388 CALL                     1
                            398 POP_TOP
                
-               203         400 LOAD_GLOBAL              0 (ts)
+               206         400 LOAD_GLOBAL              0 (ts)
                            412 LOAD_ATTR               10 (query)
                            422 LOAD_METHOD             12 (find_company_by_domain)
                            444 LOAD_FAST                5 (new_company)
                            446 LOAD_ATTR               13 (domain)
                            456 PRECALL                  1
                            460 CALL                     1
                            470 STORE_FAST               6 (company)
                
-               205         472 LOAD_GLOBAL              0 (ts)
+               208         472 LOAD_GLOBAL              0 (ts)
                            484 LOAD_ATTR                8 (models)
                            494 LOAD_METHOD             14 (Event)
                
-               206         516 LOAD_FAST                1 (search)
+               209         516 LOAD_FAST                1 (search)
                            518 LOAD_ATTR               15 (uid)
                
-               207         528 LOAD_CONST              10 ('create')
+               210         528 LOAD_CONST              10 ('create')
                
-               208         530 LOAD_FAST                6 (company)
+               211         530 LOAD_FAST                6 (company)
                            532 LOAD_ATTR               13 (domain)
                
-               209         542 LOAD_CONST              11 ('google')
+               212         542 LOAD_CONST              11 ('google')
                
-               211         544 LOAD_CONST              12 ('place')
+               214         544 LOAD_CONST              12 ('place')
                            546 LOAD_FAST                3 (place)
                
-               210         548 BUILD_MAP                1
+               213         548 BUILD_MAP                1
                
-               205         550 KW_NAMES                13
+               208         550 KW_NAMES                13
                            552 PRECALL                  5
                            556 CALL                     5
                            566 STORE_FAST               7 (event)
                
-               215         568 LOAD_GLOBAL              0 (ts)
+               218         568 LOAD_GLOBAL              0 (ts)
                            580 LOAD_ATTR               10 (query)
                            590 LOAD_METHOD             16 (insert_event)
                            612 LOAD_FAST                7 (event)
                            614 PRECALL                  1
                            618 CALL                     1
                            628 POP_TOP
                            630 LOAD_CONST               0 (None)
@@ -1042,28 +1038,28 @@
                   ('search_uid', 'type', 'domain', 'actor_key', 'data')
                names      ('ts', 'google', 'gmaps', 'place', 'helpers', 'clean_domain', 'get', 'print', 'models', 'Company', 'query', 'insert_company', 'find_company_by_domain', 'domain', 'Event', 'uid', 'insert_event')
                varnames   ('place_id', 'search', 'resp', 'place', 'domain', 'new_company', 'company', 'event')
                freevars   ('existing_search_domains',)
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
                name       'build_place'
-               firstlineno 186
+               firstlineno 189
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
-         firstlineno 181
+         firstlineno 184
          lnotab 0x0401480102ff0a0224fe0204401f1a0140011e0338011cff
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 7
          flags     : 3
          code
@@ -1080,36 +1076,36 @@
             00ab0100000000000000007d037411000000000000000000007c03a60100
             00ab01000000000000000001007404000000000000000000006a09000000
             0000000000a00a00000000000000000000000000000000000000007c0364
             09640b670219000000000000000000a00b00000000000000000000000000
             00000000000000640dac0ea6010000ab0100000000000000007c016a0c00
             000000000000007c016a0d0000000000000000640fac10a6040000ab0400
             00000000000000010064005300
-         226           0 RESUME                   0
+         229           0 RESUME                   0
          
-         227           2 LOAD_FAST                1 (event)
+         230           2 LOAD_FAST                1 (event)
                        4 LOAD_ATTR                0 (data)
                       14 LOAD_CONST               1 ('q')
                       16 BINARY_SUBSCR
                       26 STORE_FAST               2 (q)
          
-         228          28 LOAD_GLOBAL              3 (NULL + len)
+         231          28 LOAD_GLOBAL              3 (NULL + len)
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
          
-         229     >>   86 LOAD_GLOBAL              4 (ts)
+         232     >>   86 LOAD_GLOBAL              4 (ts)
                       98 LOAD_ATTR                3 (google)
                      108 LOAD_METHOD              4 (search)
                      130 LOAD_FAST                2 (q)
                      132 LOAD_FAST                1 (event)
                      134 LOAD_ATTR                0 (data)
                      144 LOAD_METHOD              5 (get)
                      166 LOAD_CONST               4 ('count')
@@ -1117,66 +1113,66 @@
                      170 PRECALL                  2
                      174 CALL                     2
                      184 KW_NAMES                 6
                      186 PRECALL                  2
                      190 CALL                     2
                      200 STORE_FAST               3 (results)
          
-         230         202 LOAD_FAST                3 (results)
+         233         202 LOAD_FAST                3 (results)
                      204 LOAD_CONST               7 ('link')
                      206 BINARY_SUBSCR
                      216 LOAD_METHOD              6 (apply)
-                     238 LOAD_CONST               8 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 230>)
+                     238 LOAD_CONST               8 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py", line 233>)
                      240 MAKE_FUNCTION            0
                      242 PRECALL                  1
                      246 CALL                     1
                      256 LOAD_FAST                3 (results)
                      258 LOAD_CONST               9 ('domain')
                      260 STORE_SUBSCR
          
-         231         264 LOAD_FAST                3 (results)
+         234         264 LOAD_FAST                3 (results)
                      266 LOAD_METHOD              7 (rename)
                      288 LOAD_CONST              10 ('snippet')
                      290 LOAD_CONST              11 ('description')
                      292 BUILD_MAP                1
                      294 KW_NAMES                12
                      296 PRECALL                  1
                      300 CALL                     1
                      310 STORE_FAST               3 (results)
          
-         232         312 LOAD_GLOBAL             17 (NULL + print)
+         235         312 LOAD_GLOBAL             17 (NULL + print)
                      324 LOAD_FAST                3 (results)
                      326 PRECALL                  1
                      330 CALL                     1
                      340 POP_TOP
          
-         233         342 LOAD_GLOBAL              4 (ts)
+         236         342 LOAD_GLOBAL              4 (ts)
                      354 LOAD_ATTR                9 (query)
                      364 LOAD_METHOD             10 (insert_companies_as_targets)
          
-         234         386 LOAD_FAST                3 (results)
+         237         386 LOAD_FAST                3 (results)
                      388 LOAD_CONST               9 ('domain')
                      390 LOAD_CONST              11 ('description')
                      392 BUILD_LIST               2
                      394 BINARY_SUBSCR
                      404 LOAD_METHOD             11 (to_dict)
                      426 LOAD_CONST              13 ('records')
                      428 KW_NAMES                14
                      430 PRECALL                  1
                      434 CALL                     1
          
-         235         444 LOAD_FAST                1 (event)
+         238         444 LOAD_FAST                1 (event)
                      446 LOAD_ATTR               12 (search_uid)
          
-         236         456 LOAD_FAST                1 (event)
+         239         456 LOAD_FAST                1 (event)
                      458 LOAD_ATTR               13 (actor_key)
          
-         237         468 LOAD_CONST              15 ('Google')
+         240         468 LOAD_CONST              15 ('Google')
          
-         233         470 KW_NAMES                16
+         236         470 KW_NAMES                16
                      472 PRECALL                  4
                      476 CALL                     4
                      486 POP_TOP
                      488 LOAD_CONST               0 (None)
                      490 RETURN_VALUE
          consts
             None
@@ -1192,15 +1188,15 @@
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c00a6010000ab010000000000
                   0000005300
-               230           0 RESUME                   0
+               233           0 RESUME                   0
                              2 LOAD_GLOBAL              0 (ts)
                             14 LOAD_ATTR                1 (helpers)
                             24 LOAD_METHOD              2 (clean_domain)
                             46 LOAD_FAST                0 (x)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 RETURN_VALUE
@@ -1208,15 +1204,15 @@
                   None
                names      ('ts', 'helpers', 'clean_domain')
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
                name       '<lambda>'
-               firstlineno 230
+               firstlineno 233
                lnotab 0x
             'domain'
             'snippet'
             'description'
             ('columns',)
             'records'
             ('orient',)
@@ -1224,15 +1220,15 @@
             ('companies', 'search_uid', 'actor_key', 'source')
          names      ('data', 'len', 'ts', 'google', 'search', 'get', 'apply', 'rename', 'print', 'query', 'insert_companies_as_targets', 'to_dict', 'search_uid', 'actor_key')
          varnames   ('search', 'event', 'q', 'results')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_google_search'
-         firstlineno 226
+         firstlineno 229
          lnotab 0x02011a013a0174013e0130011e012c013a010c010c0102fc
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 10
          flags     : 3
          code
@@ -1254,163 +1250,163 @@
             007419000000000000000000007402000000000000000000006a0d000000
             00000000006a0e00000000000000007c03a6020000ab0200000000000000
             007d047401000000000000000000007c04a6010000ab0100000000000000
             0001007c006a0a00000000000000006407190000000000000000007c046a
             0a000000000000000064073c0000007402000000000000000000006a0f00
             00000000000000a01000000000000000000000000000000000000000007c
             04a6010000ab01000000000000000001008c7564005300
-         241           0 RESUME                   0
+         244           0 RESUME                   0
          
-         242           2 LOAD_GLOBAL              1 (NULL + print)
+         245           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('prompt event:')
                       16 LOAD_FAST                0 (event)
                       18 PRECALL                  2
                       22 CALL                     2
                       32 POP_TOP
          
-         245          34 LOAD_CONST               2 ('system')
+         248          34 LOAD_CONST               2 ('system')
          
-         246          36 LOAD_GLOBAL              2 (ts)
+         249          36 LOAD_GLOBAL              2 (ts)
                       48 LOAD_ATTR                2 (gpt)
                       58 LOAD_ATTR                3 (HOW_TO_RESPOND)
          
-         244          68 LOAD_CONST               3 (('role', 'content'))
+         247          68 LOAD_CONST               3 (('role', 'content'))
                       70 BUILD_CONST_KEY_MAP      2
          
-         249          72 LOAD_CONST               2 ('system')
+         252          72 LOAD_CONST               2 ('system')
          
-         250          74 LOAD_GLOBAL              2 (ts)
+         253          74 LOAD_GLOBAL              2 (ts)
                       86 LOAD_ATTR                2 (gpt)
                       96 LOAD_ATTR                4 (HOW_TO_IMPORT)
          
-         248         106 LOAD_CONST               3 (('role', 'content'))
+         251         106 LOAD_CONST               3 (('role', 'content'))
                      108 BUILD_CONST_KEY_MAP      2
          
-         253         110 LOAD_CONST               2 ('system')
+         256         110 LOAD_CONST               2 ('system')
          
-         254         112 LOAD_GLOBAL              2 (ts)
+         257         112 LOAD_GLOBAL              2 (ts)
                      124 LOAD_ATTR                2 (gpt)
                      134 LOAD_ATTR                5 (HOW_TO_TRANSITION)
          
-         252         144 LOAD_CONST               3 (('role', 'content'))
+         255         144 LOAD_CONST               3 (('role', 'content'))
                      146 BUILD_CONST_KEY_MAP      2
          
-         257         148 LOAD_CONST               2 ('system')
+         260         148 LOAD_CONST               2 ('system')
          
-         258         150 LOAD_GLOBAL              2 (ts)
+         261         150 LOAD_GLOBAL              2 (ts)
                      162 LOAD_ATTR                2 (gpt)
                      172 LOAD_ATTR                6 (HOW_TO_GOOGLE)
          
-         256         182 LOAD_CONST               3 (('role', 'content'))
+         259         182 LOAD_CONST               3 (('role', 'content'))
                      184 BUILD_CONST_KEY_MAP      2
          
-         261         186 LOAD_CONST               2 ('system')
+         264         186 LOAD_CONST               2 ('system')
          
-         262         188 LOAD_GLOBAL              2 (ts)
+         265         188 LOAD_GLOBAL              2 (ts)
                      200 LOAD_ATTR                2 (gpt)
                      210 LOAD_ATTR                7 (HOW_TO_GOOGLE_MAPS)
          
-         260         220 LOAD_CONST               3 (('role', 'content'))
+         263         220 LOAD_CONST               3 (('role', 'content'))
                      222 BUILD_CONST_KEY_MAP      2
          
-         265         224 LOAD_CONST               2 ('system')
+         268         224 LOAD_CONST               2 ('system')
          
-         266         226 LOAD_CONST               4 ('the search_uid is ')
+         269         226 LOAD_CONST               4 ('the search_uid is ')
                      228 LOAD_FAST                0 (event)
                      230 LOAD_ATTR                8 (search_uid)
                      240 FORMAT_VALUE             0
                      242 BUILD_STRING             2
          
-         264         244 LOAD_CONST               3 (('role', 'content'))
+         267         244 LOAD_CONST               3 (('role', 'content'))
                      246 BUILD_CONST_KEY_MAP      2
          
-         269         248 LOAD_CONST               2 ('system')
+         272         248 LOAD_CONST               2 ('system')
          
-         270         250 LOAD_CONST               5 ('the actor_key is ')
+         273         250 LOAD_CONST               5 ('the actor_key is ')
                      252 LOAD_FAST                0 (event)
                      254 LOAD_ATTR                9 (actor_key)
                      264 FORMAT_VALUE             0
                      266 BUILD_STRING             2
          
-         268         268 LOAD_CONST               3 (('role', 'content'))
+         271         268 LOAD_CONST               3 (('role', 'content'))
                      270 BUILD_CONST_KEY_MAP      2
          
-         272         272 LOAD_CONST               6 ('user')
+         275         272 LOAD_CONST               6 ('user')
                      274 LOAD_FAST                0 (event)
                      276 LOAD_ATTR               10 (data)
                      286 LOAD_CONST               7 ('prompt')
                      288 BINARY_SUBSCR
                      298 LOAD_CONST               3 (('role', 'content'))
                      300 BUILD_CONST_KEY_MAP      2
          
-         243         302 BUILD_LIST               8
+         246         302 BUILD_LIST               8
                      304 STORE_FAST               1 (messages)
          
-         274         306 LOAD_GLOBAL              2 (ts)
+         277         306 LOAD_GLOBAL              2 (ts)
                      318 LOAD_ATTR                2 (gpt)
                      328 LOAD_METHOD             11 (ask_gpt4)
                      350 LOAD_FAST                1 (messages)
                      352 PRECALL                  1
                      356 CALL                     1
                      366 STORE_FAST               2 (resp)
          
-         276         368 LOAD_GLOBAL              1 (NULL + print)
+         279         368 LOAD_GLOBAL              1 (NULL + print)
                      380 LOAD_FAST                2 (resp)
                      382 PRECALL                  1
                      386 CALL                     1
                      396 POP_TOP
          
-         277         398 LOAD_FAST                2 (resp)
+         280         398 LOAD_FAST                2 (resp)
                      400 LOAD_CONST               8 ('events')
                      402 BINARY_SUBSCR
                      412 GET_ITER
                  >>  414 FOR_ITER               116 (to 648)
                      416 STORE_FAST               3 (new_event)
          
-         278         418 LOAD_GLOBAL              1 (NULL + print)
+         281         418 LOAD_GLOBAL              1 (NULL + print)
                      430 LOAD_CONST               9 ('new event:')
                      432 LOAD_FAST                3 (new_event)
                      434 PRECALL                  2
                      438 CALL                     2
                      448 POP_TOP
          
-         279         450 LOAD_GLOBAL             25 (NULL + from_dict)
+         282         450 LOAD_GLOBAL             25 (NULL + from_dict)
                      462 LOAD_GLOBAL              2 (ts)
                      474 LOAD_ATTR               13 (models)
                      484 LOAD_ATTR               14 (Event)
                      494 LOAD_FAST                3 (new_event)
                      496 PRECALL                  2
                      500 CALL                     2
                      510 STORE_FAST               4 (e)
          
-         280         512 LOAD_GLOBAL              1 (NULL + print)
+         283         512 LOAD_GLOBAL              1 (NULL + print)
                      524 LOAD_FAST                4 (e)
                      526 PRECALL                  1
                      530 CALL                     1
                      540 POP_TOP
          
-         281         542 LOAD_FAST                0 (event)
+         284         542 LOAD_FAST                0 (event)
                      544 LOAD_ATTR               10 (data)
                      554 LOAD_CONST               7 ('prompt')
                      556 BINARY_SUBSCR
                      566 LOAD_FAST                4 (e)
                      568 LOAD_ATTR               10 (data)
                      578 LOAD_CONST               7 ('prompt')
                      580 STORE_SUBSCR
          
-         282         584 LOAD_GLOBAL              2 (ts)
+         285         584 LOAD_GLOBAL              2 (ts)
                      596 LOAD_ATTR               15 (query)
                      606 LOAD_METHOD             16 (insert_event)
                      628 LOAD_FAST                4 (e)
                      630 PRECALL                  1
                      634 CALL                     1
                      644 POP_TOP
                      646 JUMP_BACKWARD          117 (to 414)
          
-         277     >>  648 LOAD_CONST               0 (None)
+         280     >>  648 LOAD_CONST               0 (None)
                      650 RETURN_VALUE
          consts
             None
             'prompt event:'
             'system'
             ('role', 'content')
             'the search_uid is '
@@ -1421,146 +1417,144 @@
             'new event:'
          names      ('print', 'ts', 'gpt', 'HOW_TO_RESPOND', 'HOW_TO_IMPORT', 'HOW_TO_TRANSITION', 'HOW_TO_GOOGLE', 'HOW_TO_GOOGLE_MAPS', 'search_uid', 'actor_key', 'data', 'ask_gpt4', 'from_dict', 'models', 'Event', 'query', 'insert_event')
          varnames   ('event', 'messages', 'resp', 'new_event', 'e')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'handle_prompt'
-         firstlineno 241
+         firstlineno 244
          lnotab
             0x02012003020120fe0405020120fe0405020120fe0405020120fe040502
             0120fe0405020112fe0405020112fe04041ee3041f3e021e01140120013e
             011e012a0140fb
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 4
          flags     : 3
          code
             0x97007c006a0000000000000000007d017c006a0100000000000000007d
             027404000000000000000000006a030000000000000000a0040000000000
             0000000000000000000000000000007c01a6010000ab0100000000000000
             007d037c036a050000000000000000a00600000000000000000000000000
-            000000000000006401a6010000ab0100000000000000007211740f000000
-            000000000000006402a6010000ab01000000000000000001006400530074
-            04000000000000000000006a080000000000000000a00900000000000000
-            000000000000000000000000007c036a000000000000000000a6010000ab
-            0100000000000000007d047c036a0a000000000000000070147c04a00600
-            000000000000000000000000000000000000006403a6010000ab01000000
-            00000000007c035f0a00000000000000007c04a006000000000000000000
-            00000000000000000000006404a6010000ab0100000000000000007c035f
-            0b000000000000000069007c036a050000000000000000a5017c04a5017c
-            035f0500000000000000007404000000000000000000006a030000000000
-            000000a00c00000000000000000000000000000000000000007c03a60100
-            00ab0100000000000000000100741b000000000000000000007c037c02ac
-            05a6020000ab020000000000000000010064005300
-         285           0 RESUME                   0
+            000000000000006401a6010000ab0100000000000000007210740f000000
+            000000000000006402a6010000ab01000000000000000001006e8e740400
+            0000000000000000006a080000000000000000a009000000000000000000
+            00000000000000000000007c036a000000000000000000a6010000ab0100
+            000000000000007d047c036a0a000000000000000070147c04a006000000
+            00000000000000000000000000000000006403a6010000ab010000000000
+            0000007c035f0a00000000000000007c04a0060000000000000000000000
+            0000000000000000006404a6010000ab0100000000000000007c035f0b00
+            0000000000000069007c036a050000000000000000a5017c04a5017c035f
+            0500000000000000007404000000000000000000006a0300000000000000
+            00a00c00000000000000000000000000000000000000007c03a6010000ab
+            0100000000000000000100741b000000000000000000007c037c02ac05a6
+            020000ab020000000000000000010064005300
+         288           0 RESUME                   0
          
-         286           2 LOAD_FAST                0 (event)
+         289           2 LOAD_FAST                0 (event)
                        4 LOAD_ATTR                0 (domain)
                       14 STORE_FAST               1 (domain)
          
-         287          16 LOAD_FAST                0 (event)
+         290          16 LOAD_FAST                0 (event)
                       18 LOAD_ATTR                1 (search_uid)
                       28 STORE_FAST               2 (search_uid)
          
-         289          30 LOAD_GLOBAL              4 (ts)
+         292          30 LOAD_GLOBAL              4 (ts)
                       42 LOAD_ATTR                3 (query)
                       52 LOAD_METHOD              4 (find_company_by_domain)
                       74 LOAD_FAST                1 (domain)
                       76 PRECALL                  1
                       80 CALL                     1
                       90 STORE_FAST               3 (company)
          
-         290          92 LOAD_FAST                3 (company)
+         293          92 LOAD_FAST                3 (company)
                       94 LOAD_ATTR                5 (meta)
                      104 LOAD_METHOD              6 (get)
                      126 LOAD_CONST               1 ('company_uid')
                      128 PRECALL                  1
                      132 CALL                     1
-                     142 POP_JUMP_FORWARD_IF_FALSE    17 (to 178)
+                     142 POP_JUMP_FORWARD_IF_FALSE    16 (to 176)
          
-         291         144 LOAD_GLOBAL             15 (NULL + print)
+         294         144 LOAD_GLOBAL             15 (NULL + print)
                      156 LOAD_CONST               2 ('company already exists. skipping enrichment...')
                      158 PRECALL                  1
                      162 CALL                     1
                      172 POP_TOP
+                     174 JUMP_FORWARD           142 (to 460)
+         
+         297     >>  176 LOAD_GLOBAL              4 (ts)
+                     188 LOAD_ATTR                8 (grata)
+                     198 LOAD_METHOD              9 (enrich)
+                     220 LOAD_FAST                3 (company)
+                     222 LOAD_ATTR                0 (domain)
+                     232 PRECALL                  1
+                     236 CALL                     1
+                     246 STORE_FAST               4 (resp)
          
-         292         174 LOAD_CONST               0 (None)
-                     176 RETURN_VALUE
+         298         248 LOAD_FAST                3 (company)
+                     250 LOAD_ATTR               10 (name)
+                     260 JUMP_IF_TRUE_OR_POP     20 (to 302)
+                     262 LOAD_FAST                4 (resp)
+                     264 LOAD_METHOD              6 (get)
+                     286 LOAD_CONST               3 ('name')
+                     288 PRECALL                  1
+                     292 CALL                     1
+                 >>  302 LOAD_FAST                3 (company)
+                     304 STORE_ATTR              10 (name)
+         
+         299         314 LOAD_FAST                4 (resp)
+                     316 LOAD_METHOD              6 (get)
+                     338 LOAD_CONST               4 ('description')
+                     340 PRECALL                  1
+                     344 CALL                     1
+                     354 LOAD_FAST                3 (company)
+                     356 STORE_ATTR              11 (description)
+         
+         300         366 BUILD_MAP                0
+                     368 LOAD_FAST                3 (company)
+                     370 LOAD_ATTR                5 (meta)
+                     380 DICT_UPDATE              1
+                     382 LOAD_FAST                4 (resp)
+                     384 DICT_UPDATE              1
+                     386 LOAD_FAST                3 (company)
+                     388 STORE_ATTR               5 (meta)
          
-         294     >>  178 LOAD_GLOBAL              4 (ts)
-                     190 LOAD_ATTR                8 (grata)
-                     200 LOAD_METHOD              9 (enrich)
-                     222 LOAD_FAST                3 (company)
-                     224 LOAD_ATTR                0 (domain)
-                     234 PRECALL                  1
-                     238 CALL                     1
-                     248 STORE_FAST               4 (resp)
-         
-         295         250 LOAD_FAST                3 (company)
-                     252 LOAD_ATTR               10 (name)
-                     262 JUMP_IF_TRUE_OR_POP     20 (to 304)
-                     264 LOAD_FAST                4 (resp)
-                     266 LOAD_METHOD              6 (get)
-                     288 LOAD_CONST               3 ('name')
-                     290 PRECALL                  1
-                     294 CALL                     1
-                 >>  304 LOAD_FAST                3 (company)
-                     306 STORE_ATTR              10 (name)
-         
-         296         316 LOAD_FAST                4 (resp)
-                     318 LOAD_METHOD              6 (get)
-                     340 LOAD_CONST               4 ('description')
-                     342 PRECALL                  1
-                     346 CALL                     1
-                     356 LOAD_FAST                3 (company)
-                     358 STORE_ATTR              11 (description)
-         
-         297         368 BUILD_MAP                0
-                     370 LOAD_FAST                3 (company)
-                     372 LOAD_ATTR                5 (meta)
-                     382 DICT_UPDATE              1
-                     384 LOAD_FAST                4 (resp)
-                     386 DICT_UPDATE              1
-                     388 LOAD_FAST                3 (company)
-                     390 STORE_ATTR               5 (meta)
-         
-         298         400 LOAD_GLOBAL              4 (ts)
-                     412 LOAD_ATTR                3 (query)
-                     422 LOAD_METHOD             12 (update_company)
-                     444 LOAD_FAST                3 (company)
-                     446 PRECALL                  1
-                     450 CALL                     1
-                     460 POP_TOP
-         
-         300         462 LOAD_GLOBAL             27 (NULL + enrich_with_gpt)
-                     474 LOAD_FAST                3 (company)
-                     476 LOAD_FAST                2 (search_uid)
-                     478 KW_NAMES                 5
-                     480 PRECALL                  2
-                     484 CALL                     2
-                     494 POP_TOP
-                     496 LOAD_CONST               0 (None)
-                     498 RETURN_VALUE
+         301         398 LOAD_GLOBAL              4 (ts)
+                     410 LOAD_ATTR                3 (query)
+                     420 LOAD_METHOD             12 (update_company)
+                     442 LOAD_FAST                3 (company)
+                     444 PRECALL                  1
+                     448 CALL                     1
+                     458 POP_TOP
+         
+         303     >>  460 LOAD_GLOBAL             27 (NULL + enrich_with_gpt)
+                     472 LOAD_FAST                3 (company)
+                     474 LOAD_FAST                2 (search_uid)
+                     476 KW_NAMES                 5
+                     478 PRECALL                  2
+                     482 CALL                     2
+                     492 POP_TOP
+                     494 LOAD_CONST               0 (None)
+                     496 RETURN_VALUE
          consts
             None
             'company_uid'
             'company already exists. skipping enrichment...'
             'name'
             'description'
             ('company', 'search_uid')
          names      ('domain', 'search_uid', 'ts', 'query', 'find_company_by_domain', 'meta', 'get', 'print', 'grata', 'enrich', 'name', 'description', 'update_company', 'enrich_with_gpt')
          varnames   ('event', 'domain', 'search_uid', 'company', 'resp')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'run_enrichment'
-         firstlineno 285
-         lnotab 0x02010e010e023e0134011e01040248014201340120013e02
+         firstlineno 288
+         lnotab 0x02010e010e023e013401200348014201340120013e02
       'event_id'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 9
          flags     : 3
          code
@@ -1649,593 +1643,593 @@
             0000000000000001007402000000000000000000006a0200000000000000
             00a014000000000000000000000000000000000000000074020000000000
             00000000006a150000000000000000a01600000000000000000000000000
             000000000000007c026a1300000000000000007c037c016a0d0000000000
             000000642a190000000000000000007c016a170000000000000000ac2ba6
             040000ab040000000000000000a6010000ab01000000000000000001008c
             686400530064005300
-         303           0 RESUME                   0
+         306           0 RESUME                   0
          
-         304           2 LOAD_GLOBAL              1 (NULL + print)
+         307           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('processing event...')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-         305          32 LOAD_GLOBAL              2 (ts)
+         308          32 LOAD_GLOBAL              2 (ts)
                       44 LOAD_ATTR                2 (query)
                       54 LOAD_METHOD              3 (find_event_by_id)
                       76 LOAD_FAST                0 (event_id)
                       78 PRECALL                  1
                       82 CALL                     1
                       92 STORE_FAST               1 (event)
          
-         306          94 LOAD_GLOBAL              1 (NULL + print)
+         309          94 LOAD_GLOBAL              1 (NULL + print)
                      106 LOAD_CONST               2 ('event_id')
                      108 LOAD_FAST                0 (event_id)
                      110 PRECALL                  2
                      114 CALL                     2
                      124 POP_TOP
          
-         307         126 LOAD_GLOBAL              1 (NULL + print)
+         310         126 LOAD_GLOBAL              1 (NULL + print)
                      138 LOAD_FAST                1 (event)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 POP_TOP
          
-         308         156 LOAD_GLOBAL              2 (ts)
+         311         156 LOAD_GLOBAL              2 (ts)
                      168 LOAD_ATTR                2 (query)
                      178 LOAD_METHOD              4 (find_search)
                      200 LOAD_FAST                1 (event)
                      202 LOAD_ATTR                5 (search_uid)
                      212 KW_NAMES                 3
                      214 PRECALL                  1
                      218 CALL                     1
                      228 STORE_FAST               2 (search)
          
-         309         230 LOAD_FAST                1 (event)
+         312         230 LOAD_FAST                1 (event)
                      232 LOAD_ATTR                6 (domain)
                      242 STORE_FAST               3 (domain)
          
-         310         244 LOAD_FAST                1 (event)
+         313         244 LOAD_FAST                1 (event)
                      246 LOAD_ATTR                7 (type)
                      256 LOAD_CONST               4 ('land')
                      258 COMPARE_OP               2 (==)
                      264 POP_JUMP_FORWARD_IF_FALSE    18 (to 302)
          
-         311         266 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         314         266 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      278 LOAD_FAST                1 (event)
                      280 KW_NAMES                 5
                      282 PRECALL                  1
                      286 CALL                     1
                      296 POP_TOP
                      298 LOAD_CONST               0 (None)
                      300 RETURN_VALUE
          
-         312     >>  302 LOAD_FAST                1 (event)
+         315     >>  302 LOAD_FAST                1 (event)
                      304 LOAD_ATTR                7 (type)
                      314 LOAD_CONST               6 ('create')
                      316 COMPARE_OP               2 (==)
                      322 POP_JUMP_FORWARD_IF_FALSE    18 (to 360)
          
-         313         324 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         316         324 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      336 LOAD_FAST                1 (event)
                      338 KW_NAMES                 5
                      340 PRECALL                  1
                      344 CALL                     1
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
          
-         314     >>  360 LOAD_FAST                1 (event)
+         317     >>  360 LOAD_FAST                1 (event)
                      362 LOAD_ATTR                7 (type)
                      372 LOAD_CONST               7 ('advance')
                      374 COMPARE_OP               2 (==)
                      380 POP_JUMP_FORWARD_IF_FALSE    18 (to 418)
          
-         315         382 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         318         382 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      394 LOAD_FAST                1 (event)
                      396 KW_NAMES                 5
                      398 PRECALL                  1
                      402 CALL                     1
                      412 POP_TOP
                      414 LOAD_CONST               0 (None)
                      416 RETURN_VALUE
          
-         316     >>  418 LOAD_FAST                1 (event)
+         319     >>  418 LOAD_FAST                1 (event)
                      420 LOAD_ATTR                7 (type)
                      430 LOAD_CONST               8 ('validate')
                      432 COMPARE_OP               2 (==)
                      438 POP_JUMP_FORWARD_IF_FALSE    51 (to 542)
          
-         317         440 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         320         440 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      452 LOAD_FAST                1 (event)
                      454 KW_NAMES                 5
                      456 PRECALL                  1
                      460 CALL                     1
                      470 POP_TOP
          
-         318         472 LOAD_GLOBAL             19 (NULL + run_acquired_check)
+         321         472 LOAD_GLOBAL             19 (NULL + run_acquired_check)
                      484 LOAD_FAST                3 (domain)
                      486 KW_NAMES                 9
                      488 PRECALL                  1
                      492 CALL                     1
                      502 POP_TOP
          
-         319         504 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         322         504 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      516 LOAD_FAST                2 (search)
                      518 LOAD_FAST                3 (domain)
                      520 KW_NAMES                10
                      522 PRECALL                  2
                      526 CALL                     2
                      536 POP_TOP
                      538 LOAD_CONST               0 (None)
                      540 RETURN_VALUE
          
-         320     >>  542 LOAD_FAST                1 (event)
+         323     >>  542 LOAD_FAST                1 (event)
                      544 LOAD_ATTR                7 (type)
                      554 LOAD_CONST              11 ('send')
                      556 COMPARE_OP               2 (==)
                      562 POP_JUMP_FORWARD_IF_FALSE    18 (to 600)
          
-         321         564 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         324         564 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      576 LOAD_FAST                1 (event)
                      578 KW_NAMES                 5
                      580 PRECALL                  1
                      584 CALL                     1
                      594 POP_TOP
                      596 LOAD_CONST               0 (None)
                      598 RETURN_VALUE
          
-         322     >>  600 LOAD_FAST                1 (event)
+         325     >>  600 LOAD_FAST                1 (event)
                      602 LOAD_ATTR                7 (type)
                      612 LOAD_CONST              12 ('client_approve')
                      614 COMPARE_OP               2 (==)
                      620 POP_JUMP_FORWARD_IF_FALSE    35 (to 692)
          
-         323         622 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         326         622 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      634 LOAD_FAST                1 (event)
                      636 KW_NAMES                 5
                      638 PRECALL                  1
                      642 CALL                     1
                      652 POP_TOP
          
-         324         654 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         327         654 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      666 LOAD_FAST                2 (search)
                      668 LOAD_FAST                3 (domain)
                      670 KW_NAMES                10
                      672 PRECALL                  2
                      676 CALL                     2
                      686 POP_TOP
                      688 LOAD_CONST               0 (None)
                      690 RETURN_VALUE
          
-         325     >>  692 LOAD_FAST                1 (event)
+         328     >>  692 LOAD_FAST                1 (event)
                      694 LOAD_ATTR                7 (type)
                      704 LOAD_CONST              13 ('reject')
                      706 COMPARE_OP               2 (==)
                      712 POP_JUMP_FORWARD_IF_FALSE     2 (to 718)
          
-         326         714 LOAD_CONST               0 (None)
+         329         714 LOAD_CONST               0 (None)
                      716 RETURN_VALUE
          
-         327     >>  718 LOAD_FAST                1 (event)
+         330     >>  718 LOAD_FAST                1 (event)
                      720 LOAD_ATTR                7 (type)
                      730 LOAD_CONST              14 ('client_reject')
                      732 COMPARE_OP               2 (==)
                      738 POP_JUMP_FORWARD_IF_FALSE     2 (to 744)
          
-         328         740 LOAD_CONST               0 (None)
+         331         740 LOAD_CONST               0 (None)
                      742 RETURN_VALUE
          
-         329     >>  744 LOAD_FAST                1 (event)
+         332     >>  744 LOAD_FAST                1 (event)
                      746 LOAD_ATTR                7 (type)
                      756 LOAD_CONST              15 ('conflict')
                      758 COMPARE_OP               2 (==)
                      764 POP_JUMP_FORWARD_IF_FALSE    35 (to 836)
          
-         330         766 LOAD_GLOBAL             17 (NULL + run_enrichment)
+         333         766 LOAD_GLOBAL             17 (NULL + run_enrichment)
                      778 LOAD_FAST                1 (event)
                      780 KW_NAMES                 5
                      782 PRECALL                  1
                      786 CALL                     1
                      796 POP_TOP
          
-         331         798 LOAD_GLOBAL             21 (NULL + run_similarity_search)
+         334         798 LOAD_GLOBAL             21 (NULL + run_similarity_search)
                      810 LOAD_FAST                2 (search)
                      812 LOAD_FAST                3 (domain)
                      814 KW_NAMES                10
                      816 PRECALL                  2
                      820 CALL                     2
                      830 POP_TOP
                      832 LOAD_CONST               0 (None)
                      834 RETURN_VALUE
          
-         332     >>  836 LOAD_FAST                1 (event)
+         335     >>  836 LOAD_FAST                1 (event)
                      838 LOAD_ATTR                7 (type)
                      848 LOAD_CONST              16 ('client_conflict')
                      850 COMPARE_OP               2 (==)
                      856 POP_JUMP_FORWARD_IF_FALSE     2 (to 862)
          
-         333         858 LOAD_CONST               0 (None)
+         336         858 LOAD_CONST               0 (None)
                      860 RETURN_VALUE
          
-         336     >>  862 LOAD_FAST                1 (event)
+         339     >>  862 LOAD_FAST                1 (event)
                      864 LOAD_ATTR                7 (type)
                      874 LOAD_CONST              17 ('prompt')
                      876 COMPARE_OP               2 (==)
                      882 POP_JUMP_FORWARD_IF_FALSE    18 (to 920)
          
-         337         884 LOAD_GLOBAL             23 (NULL + handle_prompt)
+         340         884 LOAD_GLOBAL             23 (NULL + handle_prompt)
                      896 LOAD_FAST                1 (event)
                      898 KW_NAMES                 5
                      900 PRECALL                  1
                      904 CALL                     1
                      914 POP_TOP
                      916 LOAD_CONST               0 (None)
                      918 RETURN_VALUE
          
-         338     >>  920 LOAD_FAST                1 (event)
+         341     >>  920 LOAD_FAST                1 (event)
                      922 LOAD_ATTR                7 (type)
                      932 LOAD_CONST              18 ('criteria')
                      934 COMPARE_OP               2 (==)
                      940 POP_JUMP_FORWARD_IF_FALSE    56 (to 1054)
          
-         339         942 LOAD_GLOBAL             25 (NULL + len)
+         342         942 LOAD_GLOBAL             25 (NULL + len)
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
          
-         340        1014 LOAD_GLOBAL             29 (NULL + run_criteria_search)
+         343        1014 LOAD_GLOBAL             29 (NULL + run_criteria_search)
                     1026 LOAD_FAST                2 (search)
                     1028 KW_NAMES                22
                     1030 PRECALL                  1
                     1034 CALL                     1
                     1044 POP_TOP
                     1046 LOAD_CONST               0 (None)
                     1048 RETURN_VALUE
          
-         339     >> 1050 LOAD_CONST               0 (None)
+         342     >> 1050 LOAD_CONST               0 (None)
                     1052 RETURN_VALUE
          
-         341     >> 1054 LOAD_FAST                1 (event)
+         344     >> 1054 LOAD_FAST                1 (event)
                     1056 LOAD_ATTR                7 (type)
                     1066 LOAD_CONST              23 ('maps')
                     1068 COMPARE_OP               2 (==)
                     1074 POP_JUMP_FORWARD_IF_FALSE    19 (to 1114)
          
-         342        1076 LOAD_GLOBAL             31 (NULL + run_maps_search)
+         345        1076 LOAD_GLOBAL             31 (NULL + run_maps_search)
                     1088 LOAD_FAST                2 (search)
                     1090 LOAD_FAST                1 (event)
                     1092 KW_NAMES                24
                     1094 PRECALL                  2
                     1098 CALL                     2
                     1108 POP_TOP
                     1110 LOAD_CONST               0 (None)
                     1112 RETURN_VALUE
          
-         343     >> 1114 LOAD_FAST                1 (event)
+         346     >> 1114 LOAD_FAST                1 (event)
                     1116 LOAD_ATTR                7 (type)
                     1126 LOAD_CONST              25 ('google')
                     1128 COMPARE_OP               2 (==)
                     1134 POP_JUMP_FORWARD_IF_FALSE    19 (to 1174)
          
-         344        1136 LOAD_GLOBAL             33 (NULL + run_google_search)
+         347        1136 LOAD_GLOBAL             33 (NULL + run_google_search)
                     1148 LOAD_FAST                2 (search)
                     1150 LOAD_FAST                1 (event)
                     1152 KW_NAMES                24
                     1154 PRECALL                  2
                     1158 CALL                     2
                     1168 POP_TOP
                     1170 LOAD_CONST               0 (None)
                     1172 RETURN_VALUE
          
-         346     >> 1174 LOAD_FAST                1 (event)
+         349     >> 1174 LOAD_FAST                1 (event)
                     1176 LOAD_ATTR                7 (type)
                     1186 LOAD_CONST              26 ('import')
                     1188 COMPARE_OP               2 (==)
                     1194 POP_JUMP_FORWARD_IF_FALSE    34 (to 1264)
          
-         347        1196 LOAD_GLOBAL              2 (ts)
+         350        1196 LOAD_GLOBAL              2 (ts)
                     1208 LOAD_ATTR                2 (query)
                     1218 LOAD_METHOD             17 (important_targets_from_event)
                     1240 LOAD_FAST                1 (event)
                     1242 KW_NAMES                 5
                     1244 PRECALL                  1
                     1248 CALL                     1
                     1258 POP_TOP
                     1260 LOAD_CONST               0 (None)
                     1262 RETURN_VALUE
          
-         349     >> 1264 LOAD_FAST                1 (event)
+         352     >> 1264 LOAD_FAST                1 (event)
                     1266 LOAD_ATTR                7 (type)
                     1276 LOAD_CONST              27 ('reset')
                     1278 COMPARE_OP               2 (==)
                     1284 POP_JUMP_FORWARD_IF_FALSE    54 (to 1394)
          
-         350        1286 LOAD_GLOBAL              1 (NULL + print)
+         353        1286 LOAD_GLOBAL              1 (NULL + print)
                     1298 LOAD_CONST              28 ('💣 Resetting Inbox...')
                     1300 PRECALL                  1
                     1304 CALL                     1
                     1314 POP_TOP
          
-         351        1316 LOAD_GLOBAL              2 (ts)
+         354        1316 LOAD_GLOBAL              2 (ts)
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
          
-         353     >> 1394 LOAD_FAST                1 (event)
+         356     >> 1394 LOAD_FAST                1 (event)
                     1396 LOAD_ATTR                7 (type)
                     1406 LOAD_CONST              30 ('rating')
                     1408 COMPARE_OP               2 (==)
                     1414 EXTENDED_ARG             1
                     1416 POP_JUMP_FORWARD_IF_FALSE   287 (to 1992)
          
-         355        1418 LOAD_GLOBAL              1 (NULL + print)
+         358        1418 LOAD_GLOBAL              1 (NULL + print)
                     1430 LOAD_FAST                1 (event)
                     1432 PRECALL                  1
                     1436 CALL                     1
                     1446 POP_TOP
          
-         356        1448 LOAD_FAST                1 (event)
+         359        1448 LOAD_FAST                1 (event)
                     1450 LOAD_ATTR               13 (data)
                     1460 LOAD_CONST              30 ('rating')
                     1462 BINARY_SUBSCR
                     1472 STORE_FAST               4 (rating)
          
-         357        1474 LOAD_FAST                1 (event)
+         360        1474 LOAD_FAST                1 (event)
                     1476 LOAD_ATTR               13 (data)
                     1486 LOAD_CONST              31 ('currentView')
                     1488 BINARY_SUBSCR
                     1498 STORE_FAST               5 (from_stage)
          
-         358        1500 LOAD_FAST                4 (rating)
+         361        1500 LOAD_FAST                4 (rating)
                     1502 LOAD_CONST              32 (1)
                     1504 COMPARE_OP               2 (==)
                     1510 POP_JUMP_FORWARD_IF_FALSE    76 (to 1664)
          
-         359        1512 LOAD_GLOBAL              2 (ts)
+         362        1512 LOAD_GLOBAL              2 (ts)
                     1524 LOAD_ATTR                2 (query)
                     1534 LOAD_METHOD             20 (insert_event)
          
-         360        1556 LOAD_GLOBAL              2 (ts)
+         363        1556 LOAD_GLOBAL              2 (ts)
                     1568 LOAD_ATTR               21 (models)
                     1578 LOAD_METHOD             22 (Event)
          
-         361        1600 LOAD_FAST                2 (search)
+         364        1600 LOAD_FAST                2 (search)
                     1602 LOAD_ATTR               19 (uid)
          
-         362        1612 LOAD_CONST              13 ('reject')
+         365        1612 LOAD_CONST              13 ('reject')
          
-         363        1614 LOAD_FAST                3 (domain)
+         366        1614 LOAD_FAST                3 (domain)
          
-         364        1616 LOAD_FAST                1 (event)
+         367        1616 LOAD_FAST                1 (event)
                     1618 LOAD_ATTR               23 (actor_key)
          
-         360        1628 KW_NAMES                33
+         363        1628 KW_NAMES                33
                     1630 PRECALL                  4
                     1634 CALL                     4
          
-         359        1644 PRECALL                  1
+         362        1644 PRECALL                  1
                     1648 CALL                     1
                     1658 POP_TOP
                     1660 LOAD_CONST               0 (None)
                     1662 RETURN_VALUE
          
-         367     >> 1664 LOAD_FAST                4 (rating)
+         370     >> 1664 LOAD_FAST                4 (rating)
                     1666 LOAD_CONST              34 (2)
                     1668 COMPARE_OP               2 (==)
                     1674 POP_JUMP_FORWARD_IF_FALSE    76 (to 1828)
          
-         368        1676 LOAD_GLOBAL              2 (ts)
+         371        1676 LOAD_GLOBAL              2 (ts)
                     1688 LOAD_ATTR                2 (query)
                     1698 LOAD_METHOD             20 (insert_event)
          
-         369        1720 LOAD_GLOBAL              2 (ts)
+         372        1720 LOAD_GLOBAL              2 (ts)
                     1732 LOAD_ATTR               21 (models)
                     1742 LOAD_METHOD             22 (Event)
          
-         370        1764 LOAD_FAST                2 (search)
+         373        1764 LOAD_FAST                2 (search)
                     1766 LOAD_ATTR               19 (uid)
          
-         371        1776 LOAD_CONST              35 ('hold')
+         374        1776 LOAD_CONST              35 ('hold')
          
-         372        1778 LOAD_FAST                3 (domain)
+         375        1778 LOAD_FAST                3 (domain)
          
-         373        1780 LOAD_FAST                1 (event)
+         376        1780 LOAD_FAST                1 (event)
                     1782 LOAD_ATTR               23 (actor_key)
          
-         369        1792 KW_NAMES                33
+         372        1792 KW_NAMES                33
                     1794 PRECALL                  4
                     1798 CALL                     4
          
-         368        1808 PRECALL                  1
+         371        1808 PRECALL                  1
                     1812 CALL                     1
                     1822 POP_TOP
                     1824 LOAD_CONST               0 (None)
                     1826 RETURN_VALUE
          
-         376     >> 1828 LOAD_FAST                5 (from_stage)
+         379     >> 1828 LOAD_FAST                5 (from_stage)
                     1830 LOAD_CONST              36 (('land', 'create', 'advance', 'hold'))
                     1832 CONTAINS_OP              0
                     1834 POP_JUMP_FORWARD_IF_FALSE    76 (to 1988)
          
-         377        1836 LOAD_GLOBAL              2 (ts)
+         380        1836 LOAD_GLOBAL              2 (ts)
                     1848 LOAD_ATTR                2 (query)
                     1858 LOAD_METHOD             20 (insert_event)
          
-         378        1880 LOAD_GLOBAL              2 (ts)
+         381        1880 LOAD_GLOBAL              2 (ts)
                     1892 LOAD_ATTR               21 (models)
                     1902 LOAD_METHOD             22 (Event)
          
-         379        1924 LOAD_FAST                2 (search)
+         382        1924 LOAD_FAST                2 (search)
                     1926 LOAD_ATTR               19 (uid)
          
-         380        1936 LOAD_CONST               8 ('validate')
+         383        1936 LOAD_CONST               8 ('validate')
          
-         381        1938 LOAD_FAST                3 (domain)
+         384        1938 LOAD_FAST                3 (domain)
          
-         382        1940 LOAD_FAST                1 (event)
+         385        1940 LOAD_FAST                1 (event)
                     1942 LOAD_ATTR               23 (actor_key)
          
-         378        1952 KW_NAMES                33
+         381        1952 KW_NAMES                33
                     1954 PRECALL                  4
                     1958 CALL                     4
          
-         377        1968 PRECALL                  1
+         380        1968 PRECALL                  1
                     1972 CALL                     1
                     1982 POP_TOP
                     1984 LOAD_CONST               0 (None)
                     1986 RETURN_VALUE
          
-         376     >> 1988 LOAD_CONST               0 (None)
+         379     >> 1988 LOAD_CONST               0 (None)
                     1990 RETURN_VALUE
          
-         386     >> 1992 LOAD_FAST                1 (event)
+         389     >> 1992 LOAD_FAST                1 (event)
                     1994 LOAD_ATTR                7 (type)
                     2004 LOAD_CONST              37 ('update')
                     2006 COMPARE_OP               2 (==)
                     2012 POP_JUMP_FORWARD_IF_FALSE   185 (to 2384)
          
-         387        2014 LOAD_FAST                3 (domain)
+         390        2014 LOAD_FAST                3 (domain)
                     2016 POP_JUMP_FORWARD_IF_FALSE   129 (to 2276)
          
-         388        2018 LOAD_GLOBAL              2 (ts)
+         391        2018 LOAD_GLOBAL              2 (ts)
                     2030 LOAD_ATTR                2 (query)
                     2040 LOAD_METHOD             24 (find_company_by_domain)
                     2062 LOAD_FAST                3 (domain)
                     2064 PRECALL                  1
                     2068 CALL                     1
                     2078 STORE_FAST               6 (company)
          
-         389        2080 LOAD_FAST                1 (event)
+         392        2080 LOAD_FAST                1 (event)
                     2082 LOAD_ATTR               13 (data)
                     2092 LOAD_METHOD             25 (get)
                     2114 LOAD_CONST              38 ('name')
                     2116 PRECALL                  1
                     2120 CALL                     1
                     2130 POP_JUMP_FORWARD_IF_FALSE    18 (to 2168)
          
-         390        2132 LOAD_FAST                1 (event)
+         393        2132 LOAD_FAST                1 (event)
                     2134 LOAD_ATTR               13 (data)
                     2144 LOAD_CONST              38 ('name')
                     2146 BINARY_SUBSCR
                     2156 LOAD_FAST                6 (company)
                     2158 STORE_ATTR              26 (name)
          
-         396     >> 2168 BUILD_MAP                0
+         399     >> 2168 BUILD_MAP                0
                     2170 LOAD_FAST                6 (company)
                     2172 LOAD_ATTR               27 (meta)
                     2182 DICT_UPDATE              1
                     2184 LOAD_FAST                1 (event)
                     2186 LOAD_ATTR               13 (data)
                     2196 DICT_UPDATE              1
                     2198 LOAD_FAST                6 (company)
                     2200 STORE_ATTR              27 (meta)
          
-         397        2210 LOAD_GLOBAL              2 (ts)
+         400        2210 LOAD_GLOBAL              2 (ts)
                     2222 LOAD_ATTR                2 (query)
                     2232 LOAD_METHOD             28 (update_company)
                     2254 LOAD_FAST                6 (company)
                     2256 PRECALL                  1
                     2260 CALL                     1
                     2270 POP_TOP
                     2272 LOAD_CONST               0 (None)
                     2274 RETURN_VALUE
          
-         399     >> 2276 BUILD_MAP                0
+         402     >> 2276 BUILD_MAP                0
                     2278 LOAD_FAST                2 (search)
                     2280 LOAD_ATTR               27 (meta)
                     2290 DICT_UPDATE              1
                     2292 LOAD_FAST                1 (event)
                     2294 LOAD_ATTR               13 (data)
                     2304 DICT_UPDATE              1
                     2306 LOAD_FAST                2 (search)
                     2308 STORE_ATTR              27 (meta)
          
-         400        2318 LOAD_GLOBAL              2 (ts)
+         403        2318 LOAD_GLOBAL              2 (ts)
                     2330 LOAD_ATTR                2 (query)
                     2340 LOAD_METHOD             29 (update_search)
                     2362 LOAD_FAST                2 (search)
                     2364 PRECALL                  1
                     2368 CALL                     1
                     2378 POP_TOP
                     2380 LOAD_CONST               0 (None)
                     2382 RETURN_VALUE
          
-         402     >> 2384 LOAD_FAST                1 (event)
+         405     >> 2384 LOAD_FAST                1 (event)
                     2386 LOAD_ATTR                7 (type)
                     2396 LOAD_CONST              39 ('move')
                     2398 COMPARE_OP               2 (==)
                     2404 POP_JUMP_FORWARD_IF_FALSE   117 (to 2640)
          
-         404        2406 LOAD_FAST                1 (event)
+         407        2406 LOAD_FAST                1 (event)
                     2408 LOAD_ATTR               13 (data)
                     2418 LOAD_CONST              40 ('domains')
                     2420 BINARY_SUBSCR
                     2430 GET_ITER
                  >> 2432 FOR_ITER               105 (to 2644)
                     2434 STORE_FAST               3 (domain)
          
-         405        2436 LOAD_GLOBAL              1 (NULL + print)
+         408        2436 LOAD_GLOBAL              1 (NULL + print)
                     2448 LOAD_CONST              41 ('moving domain:')
                     2450 LOAD_FAST                3 (domain)
                     2452 PRECALL                  2
                     2456 CALL                     2
                     2466 POP_TOP
          
-         406        2468 LOAD_GLOBAL              2 (ts)
+         409        2468 LOAD_GLOBAL              2 (ts)
                     2480 LOAD_ATTR                2 (query)
                     2490 LOAD_METHOD             20 (insert_event)
          
-         407        2512 LOAD_GLOBAL              2 (ts)
+         410        2512 LOAD_GLOBAL              2 (ts)
                     2524 LOAD_ATTR               21 (models)
                     2534 LOAD_METHOD             22 (Event)
          
-         408        2556 LOAD_FAST                2 (search)
+         411        2556 LOAD_FAST                2 (search)
                     2558 LOAD_ATTR               19 (uid)
          
-         409        2568 LOAD_FAST                3 (domain)
+         412        2568 LOAD_FAST                3 (domain)
          
-         410        2570 LOAD_FAST                1 (event)
+         413        2570 LOAD_FAST                1 (event)
                     2572 LOAD_ATTR               13 (data)
                     2582 LOAD_CONST              42 ('stage')
                     2584 BINARY_SUBSCR
          
-         411        2594 LOAD_FAST                1 (event)
+         414        2594 LOAD_FAST                1 (event)
                     2596 LOAD_ATTR               23 (actor_key)
          
-         407        2606 KW_NAMES                43
+         410        2606 KW_NAMES                43
                     2608 PRECALL                  4
                     2612 CALL                     4
          
-         406        2622 PRECALL                  1
+         409        2622 PRECALL                  1
                     2626 CALL                     1
                     2636 POP_TOP
                     2638 JUMP_BACKWARD          104 (to 2432)
          
-         402     >> 2640 LOAD_CONST               0 (None)
+         405     >> 2640 LOAD_CONST               0 (None)
                     2642 RETURN_VALUE
          
-         404     >> 2644 LOAD_CONST               0 (None)
+         407     >> 2644 LOAD_CONST               0 (None)
                     2646 RETURN_VALUE
          consts
             None
             'processing event...'
             'event_id'
             ('uid',)
             'land'
@@ -2280,15 +2274,15 @@
             ('search_uid', 'domain', 'type', 'actor_key')
          names      ('print', 'ts', 'query', 'find_event_by_id', 'find_search', 'search_uid', 'domain', 'type', 'run_enrichment', 'run_acquired_check', 'run_similarity_search', 'handle_prompt', 'len', 'data', 'run_criteria_search', 'run_maps_search', 'run_google_search', 'important_targets_from_event', 'reset_inbox', 'uid', 'insert_event', 'models', 'Event', 'actor_key', 'find_company_by_domain', 'get', 'name', 'meta', 'update_company', 'update_search')
          varnames   ('event_id', 'event', 'search', 'domain', 'rating', 'from_stage', 'company')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
          name       'process_event'
-         firstlineno 303
+         firstlineno 306
          lnotab
             0x02011e013e0120011e014a010e01160124011601240116012401160120
             012001260116012401160120012601160104011601040116012001260116
             010403160124011601480124ff040216012601160126021601440216011e
             014e0218021e011a011a010c012c012c010c01020102010cfc10ff14080c
             012c012c010c01020102010cfc10ff140808012c012c010c01020102010c
             fc10ff14ff040a160104013e01340124062a0142022a01420216021e0120
@@ -2297,9 +2291,9 @@
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/main.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108010c011402080108010c010c030c26286c280b240d3c2d3c
+      0x00ff020108010c011402080108010c010c030c26286f280b240d3c2d3c
       0f242c2412
```

### Comparing `gandai-1.7.41/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/models.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x573e3966 (Mon May  6 20:32:23 2024 UTC)
-files sz: 4381
+moddate:  0xd29a4f66 (Thu May 23 19:36:50 2024 UTC)
+files sz: 4501
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a0401
@@ -95,146 +95,146 @@
                144 CALL                     2
    
     18         154 PRECALL                  0
                158 CALL                     0
    
     19         168 STORE_NAME              13 (Company)
    
-    58         170 PUSH_NULL
+    62         170 PUSH_NULL
                172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              11 (<code object EventType, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 58>)
+               174 LOAD_CONST              11 (<code object EventType, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 62>)
                176 MAKE_FUNCTION            0
                178 LOAD_CONST              12 ('EventType')
                180 LOAD_NAME               14 (str)
                182 LOAD_NAME                6 (Enum)
                184 PRECALL                  4
                188 CALL                     4
                198 STORE_NAME              15 (EventType)
    
-    70         200 LOAD_NAME                3 (dataclass)
+    74         200 LOAD_NAME                3 (dataclass)
    
-    71         202 PUSH_NULL
+    75         202 PUSH_NULL
                204 LOAD_BUILD_CLASS
-               206 LOAD_CONST              13 (<code object Event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 70>)
+               206 LOAD_CONST              13 (<code object Event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 74>)
                208 MAKE_FUNCTION            0
                210 LOAD_CONST              14 ('Event')
                212 PRECALL                  2
                216 CALL                     2
    
-    70         226 PRECALL                  0
+    74         226 PRECALL                  0
                230 CALL                     0
    
-    71         240 STORE_NAME              16 (Event)
+    75         240 STORE_NAME              16 (Event)
    
-    81         242 LOAD_NAME                3 (dataclass)
+    86         242 LOAD_NAME                3 (dataclass)
    
-    82         244 PUSH_NULL
+    87         244 PUSH_NULL
                246 LOAD_BUILD_CLASS
-               248 LOAD_CONST              15 (<code object Comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 81>)
+               248 LOAD_CONST              15 (<code object Comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 86>)
                250 MAKE_FUNCTION            0
                252 LOAD_CONST              16 ('Comment')
                254 LOAD_NAME               16 (Event)
                256 PRECALL                  3
                260 CALL                     3
    
-    81         270 PRECALL                  0
+    86         270 PRECALL                  0
                274 CALL                     0
    
-    82         284 STORE_NAME              17 (Comment)
+    87         284 STORE_NAME              17 (Comment)
    
-    88         286 LOAD_NAME                3 (dataclass)
+    93         286 LOAD_NAME                3 (dataclass)
    
-    89         288 PUSH_NULL
+    94         288 PUSH_NULL
                290 LOAD_BUILD_CLASS
-               292 LOAD_CONST              17 (<code object Rating, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 88>)
+               292 LOAD_CONST              17 (<code object Rating, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 93>)
                294 MAKE_FUNCTION            0
                296 LOAD_CONST              18 ('Rating')
                298 LOAD_NAME               16 (Event)
                300 PRECALL                  3
                304 CALL                     3
    
-    88         314 PRECALL                  0
+    93         314 PRECALL                  0
                318 CALL                     0
    
-    89         328 STORE_NAME              18 (Rating)
+    94         328 STORE_NAME              18 (Rating)
    
-    94         330 LOAD_NAME                3 (dataclass)
+    99         330 LOAD_NAME                3 (dataclass)
    
-    95         332 PUSH_NULL
+   100         332 PUSH_NULL
                334 LOAD_BUILD_CLASS
-               336 LOAD_CONST              19 (<code object Inclusion, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 94>)
+               336 LOAD_CONST              19 (<code object Inclusion, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 99>)
                338 MAKE_FUNCTION            0
                340 LOAD_CONST              20 ('Inclusion')
                342 PRECALL                  2
                346 CALL                     2
    
-    94         356 PRECALL                  0
+    99         356 PRECALL                  0
                360 CALL                     0
    
-    95         370 STORE_NAME              19 (Inclusion)
+   100         370 STORE_NAME              19 (Inclusion)
    
-   110         372 LOAD_NAME                3 (dataclass)
+   115         372 LOAD_NAME                3 (dataclass)
    
-   111         374 PUSH_NULL
+   116         374 PUSH_NULL
                376 LOAD_BUILD_CLASS
-               378 LOAD_CONST              21 (<code object Exclusion, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 110>)
+               378 LOAD_CONST              21 (<code object Exclusion, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 115>)
                380 MAKE_FUNCTION            0
                382 LOAD_CONST              22 ('Exclusion')
                384 PRECALL                  2
                388 CALL                     2
    
-   110         398 PRECALL                  0
+   115         398 PRECALL                  0
                402 CALL                     0
    
-   111         412 STORE_NAME              20 (Exclusion)
+   116         412 STORE_NAME              20 (Exclusion)
    
-   116         414 LOAD_NAME                3 (dataclass)
+   121         414 LOAD_NAME                3 (dataclass)
    
-   117         416 PUSH_NULL
+   122         416 PUSH_NULL
                418 LOAD_BUILD_CLASS
-               420 LOAD_CONST              23 (<code object Criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 116>)
+               420 LOAD_CONST              23 (<code object Criteria, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 121>)
                422 MAKE_FUNCTION            0
                424 LOAD_CONST              24 ('Criteria')
                426 PRECALL                  2
                430 CALL                     2
    
-   116         440 PRECALL                  0
+   121         440 PRECALL                  0
                444 CALL                     0
    
-   117         454 STORE_NAME              21 (Criteria)
+   122         454 STORE_NAME              21 (Criteria)
    
-   124         456 LOAD_NAME                3 (dataclass)
+   129         456 LOAD_NAME                3 (dataclass)
    
-   125         458 PUSH_NULL
+   130         458 PUSH_NULL
                460 LOAD_BUILD_CLASS
-               462 LOAD_CONST              25 (<code object Maps, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 124>)
+               462 LOAD_CONST              25 (<code object Maps, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 129>)
                464 MAKE_FUNCTION            0
                466 LOAD_CONST              26 ('Maps')
                468 PRECALL                  2
                472 CALL                     2
    
-   124         482 PRECALL                  0
+   129         482 PRECALL                  0
                486 CALL                     0
    
-   125         496 STORE_NAME              22 (Maps)
+   130         496 STORE_NAME              22 (Maps)
    
-   133         498 LOAD_NAME                3 (dataclass)
+   138         498 LOAD_NAME                3 (dataclass)
    
-   134         500 PUSH_NULL
+   139         500 PUSH_NULL
                502 LOAD_BUILD_CLASS
-               504 LOAD_CONST              27 (<code object Search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 133>)
+               504 LOAD_CONST              27 (<code object Search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 138>)
                506 MAKE_FUNCTION            0
                508 LOAD_CONST              28 ('Search')
                510 PRECALL                  2
                514 CALL                     2
    
-   133         524 PRECALL                  0
+   138         524 PRECALL                  0
                528 CALL                     0
    
-   134         538 STORE_NAME              23 (Search)
+   139         538 STORE_NAME              23 (Search)
                540 LOAD_CONST               1 (None)
                542 RETURN_VALUE
    consts
       0
       None
       ('asdict', 'dataclass', 'field')
       ('Enum', 'auto')
@@ -384,69 +384,69 @@
                      192 LOAD_NAME                6 (Optional)
                      194 LOAD_NAME               13 (int)
                      196 BINARY_SUBSCR
                      206 LOAD_NAME                4 (__annotations__)
                      208 LOAD_CONST              10 ('uid')
                      210 STORE_SUBSCR
          
-          28         214 LOAD_NAME               15 (property)
+          32         214 LOAD_NAME               15 (property)
          
-          29         216 LOAD_CONST              11 (<code object ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 28>)
+          33         216 LOAD_CONST              11 (<code object ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 32>)
                      218 MAKE_FUNCTION            0
          
-          28         220 PRECALL                  0
+          32         220 PRECALL                  0
                      224 CALL                     0
          
-          29         234 STORE_NAME              16 (ownership)
+          33         234 STORE_NAME              16 (ownership)
          
-          33         236 LOAD_NAME               15 (property)
+          37         236 LOAD_NAME               15 (property)
          
-          34         238 LOAD_CONST              12 (<code object was_acquired, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 33>)
+          38         238 LOAD_CONST              12 (<code object was_acquired, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 37>)
                      240 MAKE_FUNCTION            0
          
-          33         242 PRECALL                  0
+          37         242 PRECALL                  0
                      246 CALL                     0
          
-          34         256 STORE_NAME              17 (was_acquired)
+          38         256 STORE_NAME              17 (was_acquired)
          
-          38         258 LOAD_NAME               15 (property)
+          42         258 LOAD_NAME               15 (property)
          
-          39         260 LOAD_CONST              13 ('return')
+          43         260 LOAD_CONST              13 ('return')
                      262 LOAD_NAME                3 (str)
                      264 BUILD_TUPLE              2
-                     266 LOAD_CONST              14 (<code object products, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 38>)
+                     266 LOAD_CONST              14 (<code object products, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 42>)
                      268 MAKE_FUNCTION            4 (annotations)
          
-          38         270 PRECALL                  0
+          42         270 PRECALL                  0
                      274 CALL                     0
          
-          39         284 STORE_NAME              18 (products)
+          43         284 STORE_NAME              18 (products)
          
-          43         286 LOAD_NAME               15 (property)
+          47         286 LOAD_NAME               15 (property)
          
-          44         288 LOAD_CONST              13 ('return')
+          48         288 LOAD_CONST              13 ('return')
                      290 LOAD_NAME                3 (str)
                      292 BUILD_TUPLE              2
-                     294 LOAD_CONST              15 (<code object services, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 43>)
+                     294 LOAD_CONST              15 (<code object services, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 47>)
                      296 MAKE_FUNCTION            4 (annotations)
          
-          43         298 PRECALL                  0
+          47         298 PRECALL                  0
                      302 CALL                     0
          
-          44         312 STORE_NAME              19 (services)
+          48         312 STORE_NAME              19 (services)
          
-          48         314 LOAD_NAME               20 (staticmethod)
+          52         314 LOAD_NAME               20 (staticmethod)
          
-          49         316 LOAD_CONST              16 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 48>)
+          53         316 LOAD_CONST              16 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 52>)
                      318 MAKE_FUNCTION            0
          
-          48         320 PRECALL                  0
+          52         320 PRECALL                  0
                      324 CALL                     0
          
-          49         334 STORE_NAME              21 (get_ownership)
+          53         334 STORE_NAME              21 (get_ownership)
                      336 LOAD_CONST               2 (None)
                      338 RETURN_VALUE
          consts
             'Company'
             'domain'
             None
             'name'
@@ -463,53 +463,53 @@
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000007d017c00a0
                   0200000000000000000000000000000000000000007c01a6010000ab0100
                   000000000000005300
-                28           0 RESUME                   0
+                32           0 RESUME                   0
                
-                30           2 LOAD_FAST                0 (self)
+                34           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('ownership')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 STORE_FAST               1 (ownership)
                
-                31          56 LOAD_FAST                0 (self)
+                35          56 LOAD_FAST                0 (self)
                             58 LOAD_METHOD              2 (get_ownership)
                             80 LOAD_FAST                1 (ownership)
                             82 PRECALL                  1
                             86 CALL                     1
                             96 RETURN_VALUE
                consts
                   None
                   'ownership'
                names      ('meta', 'get', 'get_ownership')
                varnames   ('self', 'ownership')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'ownership'
-               firstlineno 28
+               firstlineno 32
                lnotab 0x02023601
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-                33           0 RESUME                   0
+                37           0 RESUME                   0
                
-                36           2 LOAD_FAST                0 (self)
+                40           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('was_acquired')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -518,28 +518,28 @@
                   'was_acquired'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'was_acquired'
-               firstlineno 33
+               firstlineno 37
                lnotab 0x0203
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-                38           0 RESUME                   0
+                42           0 RESUME                   0
                
-                41           2 LOAD_FAST                0 (self)
+                45           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('products')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -548,27 +548,27 @@
                   'products'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'products'
-               firstlineno 38
+               firstlineno 42
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-                43           0 RESUME                   0
+                47           0 RESUME                   0
                
-                46           2 LOAD_FAST                0 (self)
+                50           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('services')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -577,67 +577,67 @@
                   'services'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'services'
-               firstlineno 43
+               firstlineno 47
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c0064016b02000000007202640253007c0064036b020000000072
                   02640453007c005300
-                48           0 RESUME                   0
+                52           0 RESUME                   0
                
-                50           2 LOAD_FAST                0 (ownership)
+                54           2 LOAD_FAST                0 (ownership)
                              4 LOAD_CONST               1 ('Bootstrapped')
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE     2 (to 18)
                
-                51          14 LOAD_CONST               2 ('Private')
+                55          14 LOAD_CONST               2 ('Private')
                             16 RETURN_VALUE
                
-                52     >>   18 LOAD_FAST                0 (ownership)
+                56     >>   18 LOAD_FAST                0 (ownership)
                             20 LOAD_CONST               3 ('Investor Backed')
                             22 COMPARE_OP               2 (==)
                             28 POP_JUMP_FORWARD_IF_FALSE     2 (to 34)
                
-                53          30 LOAD_CONST               4 ('Venture Capital')
+                57          30 LOAD_CONST               4 ('Venture Capital')
                             32 RETURN_VALUE
                
-                55     >>   34 LOAD_FAST                0 (ownership)
+                59     >>   34 LOAD_FAST                0 (ownership)
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
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'get_ownership'
-               firstlineno 48
+               firstlineno 52
                lnotab 0x02020c0104010c010402
          names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'name', 'Optional', 'description', 'source', 'field', 'dict', 'meta', 'id', 'int', 'uid', 'property', 'ownership', 'was_acquired', 'products', 'services', 'staticmethod', 'get_ownership')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Company'
          firstlineno 18
          lnotab
-            0x0c020a011a011a011a01220122012e02020104ff0e010204020104ff0e
+            0x0c020a011a011a011a01220122012e06020104ff0e010204020104ff0e
             01020402010aff0e01020402010aff0e010204020104ff0e01
       'Company'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
@@ -645,69 +645,69 @@
             0x970065005a0164005a0202006503a6000000ab0000000000000000005a
             0402006503a6000000ab0000000000000000005a0502006503a6000000ab
             0000000000000000005a0602006503a6000000ab0000000000000000005a
             0702006503a6000000ab0000000000000000005a0802006503a6000000ab
             0000000000000000005a0902006503a6000000ab0000000000000000005a
             0a02006503a6000000ab0000000000000000005a0b02006503a6000000ab
             0000000000000000005a0c64015300
-          58           0 RESUME                   0
+          62           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('EventType')
                        8 STORE_NAME               2 (__qualname__)
          
-          59          10 PUSH_NULL
+          63          10 PUSH_NULL
                       12 LOAD_NAME                3 (auto)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_NAME               4 (CREATE)
          
-          60          30 PUSH_NULL
+          64          30 PUSH_NULL
                       32 LOAD_NAME                3 (auto)
                       34 PRECALL                  0
                       38 CALL                     0
                       48 STORE_NAME               5 (ADVANCE)
          
-          61          50 PUSH_NULL
+          65          50 PUSH_NULL
                       52 LOAD_NAME                3 (auto)
                       54 PRECALL                  0
                       58 CALL                     0
                       68 STORE_NAME               6 (VALIDATE)
          
-          62          70 PUSH_NULL
+          66          70 PUSH_NULL
                       72 LOAD_NAME                3 (auto)
                       74 PRECALL                  0
                       78 CALL                     0
                       88 STORE_NAME               7 (SEND)
          
-          63          90 PUSH_NULL
+          67          90 PUSH_NULL
                       92 LOAD_NAME                3 (auto)
                       94 PRECALL                  0
                       98 CALL                     0
                      108 STORE_NAME               8 (CLIENT_APPROVE)
          
-          64         110 PUSH_NULL
+          68         110 PUSH_NULL
                      112 LOAD_NAME                3 (auto)
                      114 PRECALL                  0
                      118 CALL                     0
                      128 STORE_NAME               9 (CONFLICT)
          
-          65         130 PUSH_NULL
+          69         130 PUSH_NULL
                      132 LOAD_NAME                3 (auto)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 STORE_NAME              10 (REJECT)
          
-          66         150 PUSH_NULL
+          70         150 PUSH_NULL
                      152 LOAD_NAME                3 (auto)
                      154 PRECALL                  0
                      158 CALL                     0
                      168 STORE_NAME              11 (CLIENT_REJECT)
          
-          67         170 PUSH_NULL
+          71         170 PUSH_NULL
                      172 LOAD_NAME                3 (auto)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 STORE_NAME              12 (CRITERIA)
                      190 LOAD_CONST               1 (None)
                      192 RETURN_VALUE
          consts
@@ -715,117 +715,122 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'auto', 'CREATE', 'ADVANCE', 'VALIDATE', 'SEND', 'CLIENT_APPROVE', 'CONFLICT', 'REJECT', 'CLIENT_REJECT', 'CRITERIA')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'EventType'
-         firstlineno 58
+         firstlineno 62
          lnotab 0x0a0114011401140114011401140114011401
       'EventType'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
-            0x970065005a0164005a0255006503650464013c0000006505650464023c
-            0000006505650464033c00000064045a0665076505190000000000000000
-            00650464053c000000020065086509ac06a6010000ab0100000000000000
-            005a0a6509650464073c000000020065086404ac08a6010000ab01000000
-            00000000005a0b6503650464093c00000064045300
-          70           0 RESUME                   0
+            0x970065005a0164005a0255006503650464013c0000006503650464023c
+            00000064035a056506650719000000000000000000650464043c00000064
+            035a086506650319000000000000000000650464053c0000000200650965
+            0aac06a6010000ab0100000000000000005a0b650a650464073c00000002
+            0065096403ac08a6010000ab0100000000000000005a0c6507650464093c
+            00000064035300
+          74           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Event')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          72          12 LOAD_NAME                3 (int)
+          77          12 LOAD_NAME                3 (str)
                       14 LOAD_NAME                4 (__annotations__)
-                      16 LOAD_CONST               1 ('search_uid')
+                      16 LOAD_CONST               1 ('actor_key')
                       18 STORE_SUBSCR
          
-          73          22 LOAD_NAME                5 (str)
+          78          22 LOAD_NAME                3 (str)
                       24 LOAD_NAME                4 (__annotations__)
-                      26 LOAD_CONST               2 ('actor_key')
+                      26 LOAD_CONST               2 ('type')
                       28 STORE_SUBSCR
          
-          74          32 LOAD_NAME                5 (str)
-                      34 LOAD_NAME                4 (__annotations__)
-                      36 LOAD_CONST               3 ('type')
-                      38 STORE_SUBSCR
+          79          32 LOAD_CONST               3 (None)
+                      34 STORE_NAME               5 (search_uid)
+                      36 LOAD_NAME                6 (Optional)
+                      38 LOAD_NAME                7 (int)
+                      40 BINARY_SUBSCR
+                      50 LOAD_NAME                4 (__annotations__)
+                      52 LOAD_CONST               4 ('search_uid')
+                      54 STORE_SUBSCR
          
-          75          42 LOAD_CONST               4 (None)
-                      44 STORE_NAME               6 (domain)
-                      46 LOAD_NAME                7 (Optional)
-                      48 LOAD_NAME                5 (str)
-                      50 BINARY_SUBSCR
-                      60 LOAD_NAME                4 (__annotations__)
-                      62 LOAD_CONST               5 ('domain')
-                      64 STORE_SUBSCR
-         
-          76          68 PUSH_NULL
-                      70 LOAD_NAME                8 (field)
-                      72 LOAD_NAME                9 (dict)
-                      74 KW_NAMES                 6
-                      76 PRECALL                  1
-                      80 CALL                     1
-                      90 STORE_NAME              10 (data)
-                      92 LOAD_NAME                9 (dict)
-                      94 LOAD_NAME                4 (__annotations__)
-                      96 LOAD_CONST               7 ('data')
-                      98 STORE_SUBSCR
-         
-          77         102 PUSH_NULL
-                     104 LOAD_NAME                8 (field)
-                     106 LOAD_CONST               4 (None)
-                     108 KW_NAMES                 8
-                     110 PRECALL                  1
-                     114 CALL                     1
-                     124 STORE_NAME              11 (id)
-                     126 LOAD_NAME                3 (int)
-                     128 LOAD_NAME                4 (__annotations__)
-                     130 LOAD_CONST               9 ('id')
-                     132 STORE_SUBSCR
-                     136 LOAD_CONST               4 (None)
-                     138 RETURN_VALUE
+          80          58 LOAD_CONST               3 (None)
+                      60 STORE_NAME               8 (domain)
+                      62 LOAD_NAME                6 (Optional)
+                      64 LOAD_NAME                3 (str)
+                      66 BINARY_SUBSCR
+                      76 LOAD_NAME                4 (__annotations__)
+                      78 LOAD_CONST               5 ('domain')
+                      80 STORE_SUBSCR
+         
+          81          84 PUSH_NULL
+                      86 LOAD_NAME                9 (field)
+                      88 LOAD_NAME               10 (dict)
+                      90 KW_NAMES                 6
+                      92 PRECALL                  1
+                      96 CALL                     1
+                     106 STORE_NAME              11 (data)
+                     108 LOAD_NAME               10 (dict)
+                     110 LOAD_NAME                4 (__annotations__)
+                     112 LOAD_CONST               7 ('data')
+                     114 STORE_SUBSCR
+         
+          82         118 PUSH_NULL
+                     120 LOAD_NAME                9 (field)
+                     122 LOAD_CONST               3 (None)
+                     124 KW_NAMES                 8
+                     126 PRECALL                  1
+                     130 CALL                     1
+                     140 STORE_NAME              12 (id)
+                     142 LOAD_NAME                7 (int)
+                     144 LOAD_NAME                4 (__annotations__)
+                     146 LOAD_CONST               9 ('id')
+                     148 STORE_SUBSCR
+                     152 LOAD_CONST               3 (None)
+                     154 RETURN_VALUE
          consts
             'Event'
-            'search_uid'
             'actor_key'
             'type'
             None
+            'search_uid'
             'domain'
             ('default_factory',)
             'data'
             ('default',)
             'id'
-         names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'domain', 'Optional', 'field', 'dict', 'data', 'id')
+         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'search_uid', 'Optional', 'int', 'domain', 'field', 'dict', 'data', 'id')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Event'
-         firstlineno 70
-         lnotab 0x0c020a010a010a011a012201
+         firstlineno 74
+         lnotab 0x0c030a010a011a011a012201
       'Event'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          81           0 RESUME                   0
+          86           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Comment')
                        8 STORE_NAME               2 (__qualname__)
          
-          83          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 83>)
+          88          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 88>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__post_init__)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'Comment'
             code
@@ -833,17 +838,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000640119
                   000000000000000000740400000000000000000000a6020000ab02000000
                   000000000073024a00820164005300
-                83           0 RESUME                   0
+                88           0 RESUME                   0
                
-                85           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                90           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (data)
                             26 LOAD_CONST               1 ('comment')
                             28 BINARY_SUBSCR
                             38 LOAD_GLOBAL              4 (str)
                             50 PRECALL                  2
                             54 CALL                     2
@@ -857,39 +862,39 @@
                   'comment'
                names      ('isinstance', 'data', 'str')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       '__post_init__'
-               firstlineno 83
+               firstlineno 88
                lnotab 0x0202
             None
          names      ('__name__', '__module__', '__qualname__', '__post_init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Comment'
-         firstlineno 81
+         firstlineno 86
          lnotab 0x0a02
       'Comment'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          88           0 RESUME                   0
+          93           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Rating')
                        8 STORE_NAME               2 (__qualname__)
          
-          90          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 90>)
+          95          10 LOAD_CONST               1 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 95>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__post_init__)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'Rating'
             code
@@ -897,17 +902,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000640119
                   000000000000000000740400000000000000000000a6020000ab02000000
                   000000000073024a00820164005300
-                90           0 RESUME                   0
+                95           0 RESUME                   0
                
-                91           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                96           2 LOAD_GLOBAL              1 (NULL + isinstance)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (data)
                             26 LOAD_CONST               1 ('rating')
                             28 BINARY_SUBSCR
                             38 LOAD_GLOBAL              4 (int)
                             50 PRECALL                  2
                             54 CALL                     2
@@ -921,24 +926,24 @@
                   'rating'
                names      ('isinstance', 'data', 'int')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       '__post_init__'
-               firstlineno 90
+               firstlineno 95
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__post_init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Rating'
-         firstlineno 88
+         firstlineno 93
          lnotab 0x0a02
       'Rating'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
@@ -950,282 +955,282 @@
             00ab0100000000000000005a0b6506650719000000000000000000650864
             063c0000000200650364078400ac01a6010000ab0100000000000000005a
             0c6506650719000000000000000000650864083c000000020065036504ac
             01a6010000ab0100000000000000005a0d65066507190000000000000000
             00650864093c000000020065036504ac01a6010000ab0100000000000000
             005a0e65066507190000000000000000006508640a3c000000640b84005a
             0f640c5300
-          94           0 RESUME                   0
+          99           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Inclusion')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          96          12 PUSH_NULL
+         101          12 PUSH_NULL
                       14 LOAD_NAME                3 (field)
                       16 LOAD_NAME                4 (list)
                       18 KW_NAMES                 1
                       20 PRECALL                  1
                       24 CALL                     1
                       34 STORE_NAME               5 (keywords)
                       36 LOAD_NAME                6 (List)
                       38 LOAD_NAME                7 (str)
                       40 BINARY_SUBSCR
                       50 LOAD_NAME                8 (__annotations__)
                       52 LOAD_CONST               2 ('keywords')
                       54 STORE_SUBSCR
          
-          97          58 PUSH_NULL
+         102          58 PUSH_NULL
                       60 LOAD_NAME                3 (field)
-                      62 LOAD_CONST               3 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 97>)
+                      62 LOAD_CONST               3 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 102>)
                       64 MAKE_FUNCTION            0
                       66 KW_NAMES                 1
                       68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_NAME               9 (employees_range)
                       84 LOAD_NAME                6 (List)
                       86 LOAD_NAME               10 (Any)
                       88 BINARY_SUBSCR
                       98 LOAD_NAME                8 (__annotations__)
                      100 LOAD_CONST               4 ('employees_range')
                      102 STORE_SUBSCR
          
-          98         106 PUSH_NULL
+         103         106 PUSH_NULL
                      108 LOAD_NAME                3 (field)
-                     110 LOAD_CONST               5 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 98>)
+                     110 LOAD_CONST               5 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 103>)
                      112 MAKE_FUNCTION            0
                      114 KW_NAMES                 1
                      116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_NAME              11 (ownership)
                      132 LOAD_NAME                6 (List)
                      134 LOAD_NAME                7 (str)
                      136 BINARY_SUBSCR
                      146 LOAD_NAME                8 (__annotations__)
                      148 LOAD_CONST               6 ('ownership')
                      150 STORE_SUBSCR
          
-          99         154 PUSH_NULL
+         104         154 PUSH_NULL
                      156 LOAD_NAME                3 (field)
-                     158 LOAD_CONST               7 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 99>)
+                     158 LOAD_CONST               7 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 104>)
                      160 MAKE_FUNCTION            0
                      162 KW_NAMES                 1
                      164 PRECALL                  1
                      168 CALL                     1
                      178 STORE_NAME              12 (country)
                      180 LOAD_NAME                6 (List)
                      182 LOAD_NAME                7 (str)
                      184 BINARY_SUBSCR
                      194 LOAD_NAME                8 (__annotations__)
                      196 LOAD_CONST               8 ('country')
                      198 STORE_SUBSCR
          
-         100         202 PUSH_NULL
+         105         202 PUSH_NULL
                      204 LOAD_NAME                3 (field)
                      206 LOAD_NAME                4 (list)
                      208 KW_NAMES                 1
                      210 PRECALL                  1
                      214 CALL                     1
                      224 STORE_NAME              13 (state)
                      226 LOAD_NAME                6 (List)
                      228 LOAD_NAME                7 (str)
                      230 BINARY_SUBSCR
                      240 LOAD_NAME                8 (__annotations__)
                      242 LOAD_CONST               9 ('state')
                      244 STORE_SUBSCR
          
-         101         248 PUSH_NULL
+         106         248 PUSH_NULL
                      250 LOAD_NAME                3 (field)
                      252 LOAD_NAME                4 (list)
                      254 KW_NAMES                 1
                      256 PRECALL                  1
                      260 CALL                     1
                      270 STORE_NAME              14 (city)
                      272 LOAD_NAME                6 (List)
                      274 LOAD_NAME                7 (str)
                      276 BINARY_SUBSCR
                      286 LOAD_NAME                8 (__annotations__)
                      288 LOAD_CONST              10 ('city')
                      290 STORE_SUBSCR
          
-         103         294 LOAD_CONST              11 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 103>)
+         108         294 LOAD_CONST              11 (<code object __post_init__, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 108>)
                      296 MAKE_FUNCTION            0
                      298 STORE_NAME              15 (__post_init__)
                      300 LOAD_CONST              12 (None)
                      302 RETURN_VALUE
          consts
             'Inclusion'
             ('default_factory',)
             'keywords'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 2
                flags     : 3
                code 0x97006401640267025300
-                97           0 RESUME                   0
+               102           0 RESUME                   0
                              2 LOAD_CONST               1 (100)
                              4 LOAD_CONST               2 (500)
                              6 BUILD_LIST               2
                              8 RETURN_VALUE
                consts
                   None
                   100
                   500
                names      ()
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       '<lambda>'
-               firstlineno 97
+               firstlineno 102
                lnotab 0x
             'employees_range'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 3
                code 0x9700640167015300
-                98           0 RESUME                   0
+               103           0 RESUME                   0
                              2 LOAD_CONST               1 ('bootstrapped')
                              4 BUILD_LIST               1
                              6 RETURN_VALUE
                consts
                   None
                   'bootstrapped'
                names      ()
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       '<lambda>'
-               firstlineno 98
+               firstlineno 103
                lnotab 0x
             'ownership'
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 3
                code 0x9700640167015300
-                99           0 RESUME                   0
+               104           0 RESUME                   0
                              2 LOAD_CONST               1 ('USA')
                              4 BUILD_LIST               1
                              6 RETURN_VALUE
                consts
                   None
                   'USA'
                names      ()
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       '<lambda>'
-               firstlineno 99
+               firstlineno 104
                lnotab 0x
             'country'
             'state'
             'city'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000640119000000000000000000800a64
                   017c006a00000000000000000064013c0000007c006a0000000000000000
                   00640219000000000000000000800c64037c006a00000000000000000064
                   023c0000006400530064005300
-               103           0 RESUME                   0
+               108           0 RESUME                   0
                
-               104           2 LOAD_FAST                0 (self)
+               109           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (employees_range)
                             14 LOAD_CONST               1 (0)
                             16 BINARY_SUBSCR
                             26 POP_JUMP_FORWARD_IF_NOT_NONE    10 (to 48)
                
-               105          28 LOAD_CONST               1 (0)
+               110          28 LOAD_CONST               1 (0)
                             30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                0 (employees_range)
                             42 LOAD_CONST               1 (0)
                             44 STORE_SUBSCR
                
-               106     >>   48 LOAD_FAST                0 (self)
+               111     >>   48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                0 (employees_range)
                             60 LOAD_CONST               2 (1)
                             62 BINARY_SUBSCR
                             72 POP_JUMP_FORWARD_IF_NOT_NONE    12 (to 98)
                
-               107          74 LOAD_CONST               3 (100000)
+               112          74 LOAD_CONST               3 (100000)
                             76 LOAD_FAST                0 (self)
                             78 LOAD_ATTR                0 (employees_range)
                             88 LOAD_CONST               2 (1)
                             90 STORE_SUBSCR
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                
-               106     >>   98 LOAD_CONST               0 (None)
+               111     >>   98 LOAD_CONST               0 (None)
                            100 RETURN_VALUE
                consts
                   None
                   0
                   1
                   100000
                names      ('employees_range',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       '__post_init__'
-               firstlineno 103
+               firstlineno 108
                lnotab 0x02011a0114011a0118ff
             None
          names      ('__name__', '__module__', '__qualname__', 'field', 'list', 'keywords', 'List', 'str', '__annotations__', 'employees_range', 'Any', 'ownership', 'country', 'state', 'city', '__post_init__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Inclusion'
-         firstlineno 94
+         firstlineno 99
          lnotab 0x0c022e013001300130012e012e02
       'Inclusion'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a025500020065036504ac01a6010000ab01000000
             00000000005a056506650719000000000000000000650864023c00000002
             0065036504ac01a6010000ab0100000000000000005a0965066507190000
             00000000000000650864033c00000064045300
-         110           0 RESUME                   0
+         115           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Exclusion')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         112          12 PUSH_NULL
+         117          12 PUSH_NULL
                       14 LOAD_NAME                3 (field)
                       16 LOAD_NAME                4 (list)
                       18 KW_NAMES                 1
                       20 PRECALL                  1
                       24 CALL                     1
                       34 STORE_NAME               5 (keywords)
                       36 LOAD_NAME                6 (List)
                       38 LOAD_NAME                7 (str)
                       40 BINARY_SUBSCR
                       50 LOAD_NAME                8 (__annotations__)
                       52 LOAD_CONST               2 ('keywords')
                       54 STORE_SUBSCR
          
-         113          58 PUSH_NULL
+         118          58 PUSH_NULL
                       60 LOAD_NAME                3 (field)
                       62 LOAD_NAME                4 (list)
                       64 KW_NAMES                 1
                       66 PRECALL                  1
                       70 CALL                     1
                       80 STORE_NAME               9 (state)
                       82 LOAD_NAME                6 (List)
@@ -1244,66 +1249,66 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'field', 'list', 'keywords', 'List', 'str', '__annotations__', 'state')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Exclusion'
-         firstlineno 110
+         firstlineno 115
          lnotab 0x0c022e01
       'Exclusion'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a025500020065036504ac01a6010000ab01000000
             00000000005a056504650664023c000000020065036507ac01a6010000ab
             0100000000000000005a086507650664033c00000064045a09650a650664
             053c00000064065a0b650c650664073c00000064085300
-         116           0 RESUME                   0
+         121           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Criteria')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         118          12 PUSH_NULL
+         123          12 PUSH_NULL
                       14 LOAD_NAME                3 (field)
                       16 LOAD_NAME                4 (Inclusion)
                       18 KW_NAMES                 1
                       20 PRECALL                  1
                       24 CALL                     1
                       34 STORE_NAME               5 (inclusion)
                       36 LOAD_NAME                4 (Inclusion)
                       38 LOAD_NAME                6 (__annotations__)
                       40 LOAD_CONST               2 ('inclusion')
                       42 STORE_SUBSCR
          
-         119          46 PUSH_NULL
+         124          46 PUSH_NULL
                       48 LOAD_NAME                3 (field)
                       50 LOAD_NAME                7 (Exclusion)
                       52 KW_NAMES                 1
                       54 PRECALL                  1
                       58 CALL                     1
                       68 STORE_NAME               8 (exclusion)
                       70 LOAD_NAME                7 (Exclusion)
                       72 LOAD_NAME                6 (__annotations__)
                       74 LOAD_CONST               3 ('exclusion')
                       76 STORE_SUBSCR
          
-         120          80 LOAD_CONST               4 (25)
+         125          80 LOAD_CONST               4 (25)
                       82 STORE_NAME               9 (result_count)
                       84 LOAD_NAME               10 (int)
                       86 LOAD_NAME                6 (__annotations__)
                       88 LOAD_CONST               5 ('result_count')
                       90 STORE_SUBSCR
          
-         121          94 LOAD_CONST               6 ('any')
+         126          94 LOAD_CONST               6 ('any')
                       96 STORE_NAME              11 (operator)
                       98 LOAD_NAME               12 (str)
                      100 LOAD_NAME                6 (__annotations__)
                      102 LOAD_CONST               7 ('operator')
                      104 STORE_SUBSCR
                      108 LOAD_CONST               8 (None)
                      110 RETURN_VALUE
@@ -1319,70 +1324,70 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'field', 'Inclusion', 'inclusion', '__annotations__', 'Exclusion', 'exclusion', 'result_count', 'int', 'operator', 'str')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Criteria'
-         firstlineno 116
+         firstlineno 121
          lnotab 0x0c02220122010e01
       'Criteria'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a02550064015a036504650564023c000000020065
             066507ac03a6010000ab0100000000000000005a08650965041900000000
             0000000000650564043c00000064055a0a650b650564063c00000064075a
             0c650b650564083c00000064015a0d6504650564093c000000640a5300
-         124           0 RESUME                   0
+         129           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Maps')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         126          12 LOAD_CONST               1 ('')
+         131          12 LOAD_CONST               1 ('')
                       14 STORE_NAME               3 (phrase)
                       16 LOAD_NAME                4 (str)
                       18 LOAD_NAME                5 (__annotations__)
                       20 LOAD_CONST               2 ('phrase')
                       22 STORE_SUBSCR
          
-         127          26 PUSH_NULL
+         132          26 PUSH_NULL
                       28 LOAD_NAME                6 (field)
                       30 LOAD_NAME                7 (list)
                       32 KW_NAMES                 3
                       34 PRECALL                  1
                       38 CALL                     1
                       48 STORE_NAME               8 (areas)
                       50 LOAD_NAME                9 (List)
                       52 LOAD_NAME                4 (str)
                       54 BINARY_SUBSCR
                       64 LOAD_NAME                5 (__annotations__)
                       66 LOAD_CONST               4 ('areas')
                       68 STORE_SUBSCR
          
-         128          72 LOAD_CONST               5 (1)
+         133          72 LOAD_CONST               5 (1)
                       74 STORE_NAME              10 (top_n)
                       76 LOAD_NAME               11 (int)
                       78 LOAD_NAME                5 (__annotations__)
                       80 LOAD_CONST               6 ('top_n')
                       82 STORE_SUBSCR
          
-         129          86 LOAD_CONST               7 (25)
+         134          86 LOAD_CONST               7 (25)
                       88 STORE_NAME              12 (radius)
                       90 LOAD_NAME               11 (int)
                       92 LOAD_NAME                5 (__annotations__)
                       94 LOAD_CONST               8 ('radius')
                       96 STORE_SUBSCR
          
-         130         100 LOAD_CONST               1 ('')
+         135         100 LOAD_CONST               1 ('')
                      102 STORE_NAME              13 (prompt)
                      104 LOAD_NAME                4 (str)
                      106 LOAD_NAME                5 (__annotations__)
                      108 LOAD_CONST               9 ('prompt')
                      110 STORE_SUBSCR
                      114 LOAD_CONST              10 (None)
                      116 RETURN_VALUE
@@ -1400,15 +1405,15 @@
             None
          names      ('__name__', '__module__', '__qualname__', 'phrase', 'str', '__annotations__', 'field', 'list', 'areas', 'List', 'top_n', 'int', 'radius', 'prompt')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Maps'
-         firstlineno 124
+         firstlineno 129
          lnotab 0x0c020e012e010e010e01
       'Maps'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
@@ -1420,145 +1425,145 @@
             000000000000005a0c650b64066505660264088404a6000000ab00000000
             00000000005a0d650b64066505660264098404a6000000ab000000000000
             0000005a0e650b640665056602640a8404a6000000ab0000000000000000
             005a0f650b640665056602640b8404a6000000ab0000000000000000005a
             10650b640665056602640c8404a6000000ab0000000000000000005a1165
             0b640665056602640d8404a6000000ab0000000000000000005a12640e53
             00
-         133           0 RESUME                   0
+         138           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Search')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         135          12 LOAD_NAME                3 (int)
+         140          12 LOAD_NAME                3 (int)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('uid')
                       18 STORE_SUBSCR
          
-         136          22 LOAD_NAME                5 (str)
+         141          22 LOAD_NAME                5 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('label')
                       28 STORE_SUBSCR
          
-         137          32 PUSH_NULL
+         142          32 PUSH_NULL
                       34 LOAD_NAME                6 (field)
                       36 LOAD_NAME                7 (dict)
                       38 KW_NAMES                 3
                       40 PRECALL                  1
                       44 CALL                     1
                       54 STORE_NAME               8 (meta)
                       56 LOAD_NAME                7 (dict)
                       58 LOAD_NAME                4 (__annotations__)
                       60 LOAD_CONST               4 ('meta')
                       62 STORE_SUBSCR
          
-         138          66 PUSH_NULL
+         143          66 PUSH_NULL
                       68 LOAD_NAME                6 (field)
                       70 LOAD_NAME                9 (Criteria)
                       72 KW_NAMES                 3
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_NAME              10 (criteria)
                       90 LOAD_NAME                9 (Criteria)
                       92 LOAD_NAME                4 (__annotations__)
                       94 LOAD_CONST               5 ('criteria')
                       96 STORE_SUBSCR
          
-         142         100 LOAD_NAME               11 (property)
+         147         100 LOAD_NAME               11 (property)
          
-         143         102 LOAD_CONST               6 ('return')
+         148         102 LOAD_CONST               6 ('return')
                      104 LOAD_NAME                5 (str)
                      106 BUILD_TUPLE              2
-                     108 LOAD_CONST               7 (<code object notes, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 142>)
+                     108 LOAD_CONST               7 (<code object notes, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 147>)
                      110 MAKE_FUNCTION            4 (annotations)
          
-         142         112 PRECALL                  0
+         147         112 PRECALL                  0
                      116 CALL                     0
          
-         143         126 STORE_NAME              12 (notes)
+         148         126 STORE_NAME              12 (notes)
          
-         146         128 LOAD_NAME               11 (property)
+         151         128 LOAD_NAME               11 (property)
          
-         147         130 LOAD_CONST               6 ('return')
+         152         130 LOAD_CONST               6 ('return')
                      132 LOAD_NAME                5 (str)
                      134 BUILD_TUPLE              2
-                     136 LOAD_CONST               8 (<code object type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 146>)
+                     136 LOAD_CONST               8 (<code object type, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 151>)
                      138 MAKE_FUNCTION            4 (annotations)
          
-         146         140 PRECALL                  0
+         151         140 PRECALL                  0
                      144 CALL                     0
          
-         147         154 STORE_NAME              13 (type)
+         152         154 STORE_NAME              13 (type)
          
-         150         156 LOAD_NAME               11 (property)
+         155         156 LOAD_NAME               11 (property)
          
-         151         158 LOAD_CONST               6 ('return')
+         156         158 LOAD_CONST               6 ('return')
                      160 LOAD_NAME                5 (str)
                      162 BUILD_TUPLE              2
-                     164 LOAD_CONST               9 (<code object prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 150>)
+                     164 LOAD_CONST               9 (<code object prompt, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 155>)
                      166 MAKE_FUNCTION            4 (annotations)
          
-         150         168 PRECALL                  0
+         155         168 PRECALL                  0
                      172 CALL                     0
          
-         151         182 STORE_NAME              14 (prompt)
+         156         182 STORE_NAME              14 (prompt)
          
-         154         184 LOAD_NAME               11 (property)
+         159         184 LOAD_NAME               11 (property)
          
-         155         186 LOAD_CONST               6 ('return')
+         160         186 LOAD_CONST               6 ('return')
                      188 LOAD_NAME                5 (str)
                      190 BUILD_TUPLE              2
-                     192 LOAD_CONST              10 (<code object products, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 154>)
+                     192 LOAD_CONST              10 (<code object products, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 159>)
                      194 MAKE_FUNCTION            4 (annotations)
          
-         154         196 PRECALL                  0
+         159         196 PRECALL                  0
                      200 CALL                     0
          
-         155         210 STORE_NAME              15 (products)
+         160         210 STORE_NAME              15 (products)
          
-         159         212 LOAD_NAME               11 (property)
+         164         212 LOAD_NAME               11 (property)
          
-         160         214 LOAD_CONST               6 ('return')
+         165         214 LOAD_CONST               6 ('return')
                      216 LOAD_NAME                5 (str)
                      218 BUILD_TUPLE              2
-                     220 LOAD_CONST              11 (<code object services, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 159>)
+                     220 LOAD_CONST              11 (<code object services, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 164>)
                      222 MAKE_FUNCTION            4 (annotations)
          
-         159         224 PRECALL                  0
+         164         224 PRECALL                  0
                      228 CALL                     0
          
-         160         238 STORE_NAME              16 (services)
+         165         238 STORE_NAME              16 (services)
          
-         164         240 LOAD_NAME               11 (property)
+         169         240 LOAD_NAME               11 (property)
          
-         165         242 LOAD_CONST               6 ('return')
+         170         242 LOAD_CONST               6 ('return')
                      244 LOAD_NAME                5 (str)
                      246 BUILD_TUPLE              2
-                     248 LOAD_CONST              12 (<code object customers, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 164>)
+                     248 LOAD_CONST              12 (<code object customers, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 169>)
                      250 MAKE_FUNCTION            4 (annotations)
          
-         164         252 PRECALL                  0
+         169         252 PRECALL                  0
                      256 CALL                     0
          
-         165         266 STORE_NAME              17 (customers)
+         170         266 STORE_NAME              17 (customers)
          
-         169         268 LOAD_NAME               11 (property)
+         174         268 LOAD_NAME               11 (property)
          
-         170         270 LOAD_CONST               6 ('return')
+         175         270 LOAD_CONST               6 ('return')
                      272 LOAD_NAME                5 (str)
                      274 BUILD_TUPLE              2
-                     276 LOAD_CONST              13 (<code object token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 169>)
+                     276 LOAD_CONST              13 (<code object token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py", line 174>)
                      278 MAKE_FUNCTION            4 (annotations)
          
-         169         280 PRECALL                  0
+         174         280 PRECALL                  0
                      284 CALL                     0
          
-         170         294 STORE_NAME              18 (token)
+         175         294 STORE_NAME              18 (token)
                      296 LOAD_CONST              14 (None)
                      298 RETURN_VALUE
          consts
             'Search'
             'uid'
             'label'
             ('default_factory',)
@@ -1569,17 +1574,17 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               142           0 RESUME                   0
+               147           0 RESUME                   0
                
-               144           2 LOAD_FAST                0 (self)
+               149           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('notes')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1588,27 +1593,27 @@
                   'notes'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'notes'
-               firstlineno 142
+               firstlineno 147
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               146           0 RESUME                   0
+               151           0 RESUME                   0
                
-               148           2 LOAD_FAST                0 (self)
+               153           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('search_type')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1617,27 +1622,27 @@
                   'search_type'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'type'
-               firstlineno 146
+               firstlineno 151
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               150           0 RESUME                   0
+               155           0 RESUME                   0
                
-               152           2 LOAD_FAST                0 (self)
+               157           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('prompt')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1646,27 +1651,27 @@
                   'prompt'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'prompt'
-               firstlineno 150
+               firstlineno 155
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               154           0 RESUME                   0
+               159           0 RESUME                   0
                
-               157           2 LOAD_FAST                0 (self)
+               162           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('products')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1675,27 +1680,27 @@
                   'products'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'products'
-               firstlineno 154
+               firstlineno 159
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               159           0 RESUME                   0
+               164           0 RESUME                   0
                
-               162           2 LOAD_FAST                0 (self)
+               167           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('services')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1704,27 +1709,27 @@
                   'services'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'services'
-               firstlineno 159
+               firstlineno 164
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   0000000000000064016400a6020000ab0200000000000000005300
-               164           0 RESUME                   0
+               169           0 RESUME                   0
                
-               167           2 LOAD_FAST                0 (self)
+               172           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (meta)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('customers')
                             38 LOAD_CONST               0 (None)
                             40 PRECALL                  2
                             44 CALL                     2
                             54 RETURN_VALUE
@@ -1733,31 +1738,31 @@
                   'customers'
                names      ('meta', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'customers'
-               firstlineno 164
+               firstlineno 169
                lnotab 0x0203
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007405000000
                   000000000000007c006a030000000000000000a6010000ab010000000000
                   000000a00400000000000000000000000000000000000000006401a60100
                   00ab010000000000000000a6010000ab010000000000000000a005000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   005300
-               169           0 RESUME                   0
+               174           0 RESUME                   0
                
-               172           2 LOAD_GLOBAL              1 (NULL + hashlib)
+               177           2 LOAD_GLOBAL              1 (NULL + hashlib)
                             14 LOAD_ATTR                1 (md5)
                             24 LOAD_GLOBAL              5 (NULL + str)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                3 (uid)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 LOAD_METHOD              4 (encode)
@@ -1775,34 +1780,34 @@
                   'utf-8'
                names      ('hashlib', 'md5', 'str', 'uid', 'encode', 'hexdigest')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
                name       'token'
-               firstlineno 169
+               firstlineno 174
                lnotab 0x0203
             None
          names      ('__name__', '__module__', '__qualname__', 'int', '__annotations__', 'str', 'field', 'dict', 'meta', 'Criteria', 'criteria', 'property', 'notes', 'type', 'prompt', 'products', 'services', 'customers', 'token')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
          name       'Search'
-         firstlineno 133
+         firstlineno 138
          lnotab
             0x0c020a010a012201220402010aff0e01020302010aff0e01020302010a
             ff0e01020302010aff0e01020402010aff0e01020402010aff0e01020402
             010aff0e01
       'Search'
    names      ('hashlib', 'dataclasses', 'asdict', 'dataclass', 'field', 'enum', 'Enum', 'auto', 'typing', 'Any', 'List', 'Optional', 'Actor', 'Company', 'str', 'EventType', 'Event', 'Comment', 'Rating', 'Inclusion', 'Exclusion', 'Criteria', 'Maps', 'Search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/models.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801140110011403020118ff0e01020a160118ff0e0102271e
-      0c020118ff0e01020a02011aff0e01020602011aff0e010205020118ff0e
+      0x00ff02010801140110011403020118ff0e01020a160118ff0e01022b1e
+      0c020118ff0e01020b02011aff0e01020602011aff0e010205020118ff0e
       01020f020118ff0e010205020118ff0e010207020118ff0e010208020118
       ff0e01
```

### Comparing `gandai-1.7.41/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x53523966 (Mon May  6 21:57:39 2024 UTC)
-files sz: 28386
+moddate:  0xeac14f66 (Thu May 23 22:23:38 2024 UTC)
+files sz: 28619
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c026d035a0301
@@ -13,31 +13,31 @@
       066c0d6d0e5a0e01000200650ea6000000ab000000000000000000010064
       0064016c0f5a10640064076c0f6d115a110100640064086c126d135a1301
       00640064096c146d155a156d165a166d175a176d185a186d195a19010002
       006513a6000000ab0000000000000000005a1a640a6517640b6517660464
       0c84045a1b640d6516640b65106a1c00000000000000006a160000000000
       0000006604640e84045a1d640f6515640b65156604641084045a1e641165
       19640b65196604641284045a1f640a65106a1c00000000000000006a1700
-      00000000000000640b64016604641384045a200900090064386415650765
+      00000000000000640b64016604641384045a200900090064376415650765
       061900000000000000000064166521641765226418652364196522640b64
       01660c641a84055a24640b65096a2500000000000000006602641b84045a
-      266439641d6521640b65096a2500000000000000006604641e84055a2764
-      1f84005a28640b65096a2500000000000000006602642084045a29642184
-      005a2a640b65096a2500000000000000006602642284045a2b640b65096a
-      2500000000000000006602642384045a2c641665216602642484045a2d64
-      166521640b65096a2500000000000000006604642584045a2e6416652164
-      0b65096a2500000000000000006604642684045a2f64166521640b65096a
-      2500000000000000006604642784045a3064286521640b65106a1c000000
-      00000000006a1900000000000000006604642984045a31642a6522640b65
-      106a1c00000000000000006a1900000000000000006604642b84045a3264
-      2c6522640b65166604642d84045a33642e6522640b65166604642f84045a
-      3464306521640b65176604643184045a35640d6516640b64016604643284
-      045a3664116519640b64016604643384045a3764306521640b6401660464
-      3484045a3864356521640b64016604643684045a3964166521640b640166
-      04643784045a3a64015300
+      26641c84005a27640b65096a2500000000000000006602641d84045a2864
+      1e84005a29641f84005a2a640b65096a2500000000000000006602642084
+      045a2b640b65096a2500000000000000006602642184045a2c6416652166
+      02642284045a2d64166521640b65096a2500000000000000006604642384
+      045a2e64166521640b65096a2500000000000000006604642484045a2f64
+      166521640b65096a2500000000000000006604642584045a306416652164
+      0b65096a2500000000000000006604642684045a3164276521640b65106a
+      1c00000000000000006a1900000000000000006604642884045a32642965
+      22640b65106a1c00000000000000006a1900000000000000006604642a84
+      045a33642b6522640b65166604642c84045a34642d6522640b6516660464
+      2e84045a35642f6521640b65176604643084045a36640d6516640b640166
+      04643184045a3764116519640b64016604643284045a38642f6521640b64
+      016604643384045a3964346521640b64016604643584045a3a6416652164
+      0b64016604643684045a3b64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (hashlib)
                  8 STORE_NAME               0 (hashlib)
    
@@ -188,15 +188,15 @@
                314 MAKE_FUNCTION            4 (annotations)
                316 STORE_NAME              32 (important_targets_from_event)
    
    176         318 NOP
    
    177         320 NOP
    
-   172         322 LOAD_CONST              56 ((False, None))
+   172         322 LOAD_CONST              55 ((False, None))
                324 LOAD_CONST              21 ('companies')
    
    173         326 LOAD_NAME                7 (List)
                328 LOAD_NAME                6 (Any)
                330 BINARY_SUBSCR
    
    172         340 LOAD_CONST              22 ('search_uid')
@@ -228,189 +228,192 @@
                370 LOAD_NAME                9 (pd)
                372 LOAD_ATTR               37 (DataFrame)
                382 BUILD_TUPLE              2
                384 LOAD_CONST              27 (<code object searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 268>)
                386 MAKE_FUNCTION            4 (annotations)
                388 STORE_NAME              38 (searches_query)
    
-   301         390 LOAD_CONST              57 ((90,))
-               392 LOAD_CONST              29 ('trailing_days')
-               394 LOAD_NAME               33 (int)
-               396 LOAD_CONST              11 ('return')
+   300         390 LOAD_CONST              28 (<code object average_rating_per_search_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 300>)
+               392 MAKE_FUNCTION            0
+               394 STORE_NAME              39 (average_rating_per_search_query)
+   
+   312         396 LOAD_CONST              11 ('return')
                398 LOAD_NAME                9 (pd)
                400 LOAD_ATTR               37 (DataFrame)
-               410 BUILD_TUPLE              4
-               412 LOAD_CONST              30 (<code object recent_validations, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 301>)
-               414 MAKE_FUNCTION            5 (defaults, annotations)
-               416 STORE_NAME              39 (recent_validations)
+               410 BUILD_TUPLE              2
+               412 LOAD_CONST              29 (<code object validation_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 312>)
+               414 MAKE_FUNCTION            4 (annotations)
+               416 STORE_NAME              40 (validation_history)
    
-   346         418 LOAD_CONST              31 (<code object average_rating_per_search_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 346>)
+   355         418 LOAD_CONST              30 (<code object searches_comment_counts, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 355>)
                420 MAKE_FUNCTION            0
-               422 STORE_NAME              40 (average_rating_per_search_query)
+               422 STORE_NAME              41 (searches_comment_counts)
    
-   358         424 LOAD_CONST              11 ('return')
-               426 LOAD_NAME                9 (pd)
-               428 LOAD_ATTR               37 (DataFrame)
-               438 BUILD_TUPLE              2
-               440 LOAD_CONST              32 (<code object validation_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 358>)
-               442 MAKE_FUNCTION            4 (annotations)
-               444 STORE_NAME              41 (validation_history)
-   
-   399         446 LOAD_CONST              33 (<code object enriched_searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 399>)
-               448 MAKE_FUNCTION            0
-               450 STORE_NAME              42 (enriched_searches_query)
+   375         424 LOAD_CONST              31 (<code object enriched_searches_query, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 375>)
+               426 MAKE_FUNCTION            0
+               428 STORE_NAME              42 (enriched_searches_query)
+   
+   402         430 LOAD_CONST              11 ('return')
+               432 LOAD_NAME                9 (pd)
+               434 LOAD_ATTR               37 (DataFrame)
+               444 BUILD_TUPLE              2
+               446 LOAD_CONST              32 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 402>)
+               448 MAKE_FUNCTION            4 (annotations)
+               450 STORE_NAME              43 (actor)
    
-   422         452 LOAD_CONST              11 ('return')
+   416         452 LOAD_CONST              11 ('return')
                454 LOAD_NAME                9 (pd)
                456 LOAD_ATTR               37 (DataFrame)
                466 BUILD_TUPLE              2
-               468 LOAD_CONST              34 (<code object actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 422>)
+               468 LOAD_CONST              33 (<code object buyer, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 416>)
                470 MAKE_FUNCTION            4 (annotations)
-               472 STORE_NAME              43 (actor)
+               472 STORE_NAME              44 (buyer)
    
-   436         474 LOAD_CONST              11 ('return')
-               476 LOAD_NAME                9 (pd)
-               478 LOAD_ATTR               37 (DataFrame)
-               488 BUILD_TUPLE              2
-               490 LOAD_CONST              35 (<code object buyer, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 436>)
-               492 MAKE_FUNCTION            4 (annotations)
-               494 STORE_NAME              44 (buyer)
-   
-   498         496 LOAD_CONST              22 ('search_uid')
-               498 LOAD_NAME               33 (int)
-               500 BUILD_TUPLE              2
-               502 LOAD_CONST              36 (<code object search_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 498>)
-               504 MAKE_FUNCTION            4 (annotations)
-               506 STORE_NAME              45 (search_targets)
-   
-   629         508 LOAD_CONST              22 ('search_uid')
-               510 LOAD_NAME               33 (int)
-               512 LOAD_CONST              11 ('return')
-               514 LOAD_NAME                9 (pd)
-               516 LOAD_ATTR               37 (DataFrame)
-               526 BUILD_TUPLE              4
-               528 LOAD_CONST              37 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 629>)
-               530 MAKE_FUNCTION            4 (annotations)
-               532 STORE_NAME              46 (event)
-   
-   641         534 LOAD_CONST              22 ('search_uid')
-               536 LOAD_NAME               33 (int)
-               538 LOAD_CONST              11 ('return')
-               540 LOAD_NAME                9 (pd)
-               542 LOAD_ATTR               37 (DataFrame)
-               552 BUILD_TUPLE              4
-               554 LOAD_CONST              38 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 641>)
-               556 MAKE_FUNCTION            4 (annotations)
-               558 STORE_NAME              47 (event_history)
-   
-   671         560 LOAD_CONST              22 ('search_uid')
-               562 LOAD_NAME               33 (int)
-               564 LOAD_CONST              11 ('return')
-               566 LOAD_NAME                9 (pd)
-               568 LOAD_ATTR               37 (DataFrame)
-               578 BUILD_TUPLE              4
-               580 LOAD_CONST              39 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 671>)
-               582 MAKE_FUNCTION            4 (annotations)
-               584 STORE_NAME              48 (search_criteria_history)
-   
-   700         586 LOAD_CONST              40 ('uid')
-               588 LOAD_NAME               33 (int)
-               590 LOAD_CONST              11 ('return')
-               592 LOAD_NAME               16 (ts)
-               594 LOAD_ATTR               28 (models)
-               604 LOAD_ATTR               25 (Search)
-               614 BUILD_TUPLE              4
-               616 LOAD_CONST              41 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 700>)
-               618 MAKE_FUNCTION            4 (annotations)
-               620 STORE_NAME              49 (find_search)
-   
-   729         622 LOAD_CONST              42 ('searchToken')
-               624 LOAD_NAME               34 (str)
-               626 LOAD_CONST              11 ('return')
-               628 LOAD_NAME               16 (ts)
-               630 LOAD_ATTR               28 (models)
-               640 LOAD_ATTR               25 (Search)
-               650 BUILD_TUPLE              4
-               652 LOAD_CONST              43 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 729>)
-               654 MAKE_FUNCTION            4 (annotations)
-               656 STORE_NAME              50 (find_search_by_token)
-   
-   738         658 LOAD_CONST              44 ('domain')
-               660 LOAD_NAME               34 (str)
-               662 LOAD_CONST              11 ('return')
-               664 LOAD_NAME               22 (Company)
-               666 BUILD_TUPLE              4
-               668 LOAD_CONST              45 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 738>)
-               670 MAKE_FUNCTION            4 (annotations)
-               672 STORE_NAME              51 (find_company_by_domain)
-   
-   754         674 LOAD_CONST              46 ('email')
-               676 LOAD_NAME               34 (str)
-               678 LOAD_CONST              11 ('return')
-               680 LOAD_NAME               22 (Company)
-               682 BUILD_TUPLE              4
-               684 LOAD_CONST              47 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 754>)
-               686 MAKE_FUNCTION            4 (annotations)
-               688 STORE_NAME              52 (find_actor_by_email)
-   
-   770         690 LOAD_CONST              48 ('event_id')
-               692 LOAD_NAME               33 (int)
-               694 LOAD_CONST              11 ('return')
-               696 LOAD_NAME               23 (Event)
-               698 BUILD_TUPLE              4
-               700 LOAD_CONST              49 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 770>)
-               702 MAKE_FUNCTION            4 (annotations)
-               704 STORE_NAME              53 (find_event_by_id)
-   
-   789         706 LOAD_CONST              13 ('company')
-               708 LOAD_NAME               22 (Company)
-               710 LOAD_CONST              11 ('return')
-               712 LOAD_CONST               1 (None)
-               714 BUILD_TUPLE              4
-               716 LOAD_CONST              50 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 789>)
-               718 MAKE_FUNCTION            4 (annotations)
-               720 STORE_NAME              54 (update_company)
-   
-   818         722 LOAD_CONST              17 ('search')
-               724 LOAD_NAME               25 (Search)
-               726 LOAD_CONST              11 ('return')
-               728 LOAD_CONST               1 (None)
-               730 BUILD_TUPLE              4
-               732 LOAD_CONST              51 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 818>)
-               734 MAKE_FUNCTION            4 (annotations)
-               736 STORE_NAME              55 (update_search)
-   
-   841         738 LOAD_CONST              48 ('event_id')
-               740 LOAD_NAME               33 (int)
-               742 LOAD_CONST              11 ('return')
-               744 LOAD_CONST               1 (None)
-               746 BUILD_TUPLE              4
-               748 LOAD_CONST              52 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 841>)
-               750 MAKE_FUNCTION            4 (annotations)
-               752 STORE_NAME              56 (mute_event)
-   
-   864         754 LOAD_CONST              53 ('comment_id')
-               756 LOAD_NAME               33 (int)
-               758 LOAD_CONST              11 ('return')
-               760 LOAD_CONST               1 (None)
-               762 BUILD_TUPLE              4
-               764 LOAD_CONST              54 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 864>)
-               766 MAKE_FUNCTION            4 (annotations)
-               768 STORE_NAME              57 (delete_comment)
-   
-   875         770 LOAD_CONST              22 ('search_uid')
-               772 LOAD_NAME               33 (int)
-               774 LOAD_CONST              11 ('return')
-               776 LOAD_CONST               1 (None)
-               778 BUILD_TUPLE              4
-               780 LOAD_CONST              55 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 875>)
-               782 MAKE_FUNCTION            4 (annotations)
-               784 STORE_NAME              58 (reset_inbox)
-               786 LOAD_CONST               1 (None)
-               788 RETURN_VALUE
+   478         474 LOAD_CONST              22 ('search_uid')
+               476 LOAD_NAME               33 (int)
+               478 BUILD_TUPLE              2
+               480 LOAD_CONST              34 (<code object search_targets, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 478>)
+               482 MAKE_FUNCTION            4 (annotations)
+               484 STORE_NAME              45 (search_targets)
+   
+   610         486 LOAD_CONST              22 ('search_uid')
+               488 LOAD_NAME               33 (int)
+               490 LOAD_CONST              11 ('return')
+               492 LOAD_NAME                9 (pd)
+               494 LOAD_ATTR               37 (DataFrame)
+               504 BUILD_TUPLE              4
+               506 LOAD_CONST              35 (<code object search_comments, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 610>)
+               508 MAKE_FUNCTION            4 (annotations)
+               510 STORE_NAME              46 (search_comments)
+   
+   632         512 LOAD_CONST              22 ('search_uid')
+               514 LOAD_NAME               33 (int)
+               516 LOAD_CONST              11 ('return')
+               518 LOAD_NAME                9 (pd)
+               520 LOAD_ATTR               37 (DataFrame)
+               530 BUILD_TUPLE              4
+               532 LOAD_CONST              36 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 632>)
+               534 MAKE_FUNCTION            4 (annotations)
+               536 STORE_NAME              47 (event)
+   
+   644         538 LOAD_CONST              22 ('search_uid')
+               540 LOAD_NAME               33 (int)
+               542 LOAD_CONST              11 ('return')
+               544 LOAD_NAME                9 (pd)
+               546 LOAD_ATTR               37 (DataFrame)
+               556 BUILD_TUPLE              4
+               558 LOAD_CONST              37 (<code object event_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 644>)
+               560 MAKE_FUNCTION            4 (annotations)
+               562 STORE_NAME              48 (event_history)
+   
+   674         564 LOAD_CONST              22 ('search_uid')
+               566 LOAD_NAME               33 (int)
+               568 LOAD_CONST              11 ('return')
+               570 LOAD_NAME                9 (pd)
+               572 LOAD_ATTR               37 (DataFrame)
+               582 BUILD_TUPLE              4
+               584 LOAD_CONST              38 (<code object search_criteria_history, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 674>)
+               586 MAKE_FUNCTION            4 (annotations)
+               588 STORE_NAME              49 (search_criteria_history)
+   
+   703         590 LOAD_CONST              39 ('uid')
+               592 LOAD_NAME               33 (int)
+               594 LOAD_CONST              11 ('return')
+               596 LOAD_NAME               16 (ts)
+               598 LOAD_ATTR               28 (models)
+               608 LOAD_ATTR               25 (Search)
+               618 BUILD_TUPLE              4
+               620 LOAD_CONST              40 (<code object find_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 703>)
+               622 MAKE_FUNCTION            4 (annotations)
+               624 STORE_NAME              50 (find_search)
+   
+   731         626 LOAD_CONST              41 ('searchToken')
+               628 LOAD_NAME               34 (str)
+               630 LOAD_CONST              11 ('return')
+               632 LOAD_NAME               16 (ts)
+               634 LOAD_ATTR               28 (models)
+               644 LOAD_ATTR               25 (Search)
+               654 BUILD_TUPLE              4
+               656 LOAD_CONST              42 (<code object find_search_by_token, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 731>)
+               658 MAKE_FUNCTION            4 (annotations)
+               660 STORE_NAME              51 (find_search_by_token)
+   
+   740         662 LOAD_CONST              43 ('domain')
+               664 LOAD_NAME               34 (str)
+               666 LOAD_CONST              11 ('return')
+               668 LOAD_NAME               22 (Company)
+               670 BUILD_TUPLE              4
+               672 LOAD_CONST              44 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 740>)
+               674 MAKE_FUNCTION            4 (annotations)
+               676 STORE_NAME              52 (find_company_by_domain)
+   
+   756         678 LOAD_CONST              45 ('email')
+               680 LOAD_NAME               34 (str)
+               682 LOAD_CONST              11 ('return')
+               684 LOAD_NAME               22 (Company)
+               686 BUILD_TUPLE              4
+               688 LOAD_CONST              46 (<code object find_actor_by_email, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 756>)
+               690 MAKE_FUNCTION            4 (annotations)
+               692 STORE_NAME              53 (find_actor_by_email)
+   
+   772         694 LOAD_CONST              47 ('event_id')
+               696 LOAD_NAME               33 (int)
+               698 LOAD_CONST              11 ('return')
+               700 LOAD_NAME               23 (Event)
+               702 BUILD_TUPLE              4
+               704 LOAD_CONST              48 (<code object find_event_by_id, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 772>)
+               706 MAKE_FUNCTION            4 (annotations)
+               708 STORE_NAME              54 (find_event_by_id)
+   
+   791         710 LOAD_CONST              13 ('company')
+               712 LOAD_NAME               22 (Company)
+               714 LOAD_CONST              11 ('return')
+               716 LOAD_CONST               1 (None)
+               718 BUILD_TUPLE              4
+               720 LOAD_CONST              49 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 791>)
+               722 MAKE_FUNCTION            4 (annotations)
+               724 STORE_NAME              55 (update_company)
+   
+   820         726 LOAD_CONST              17 ('search')
+               728 LOAD_NAME               25 (Search)
+               730 LOAD_CONST              11 ('return')
+               732 LOAD_CONST               1 (None)
+               734 BUILD_TUPLE              4
+               736 LOAD_CONST              50 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 820>)
+               738 MAKE_FUNCTION            4 (annotations)
+               740 STORE_NAME              56 (update_search)
+   
+   843         742 LOAD_CONST              47 ('event_id')
+               744 LOAD_NAME               33 (int)
+               746 LOAD_CONST              11 ('return')
+               748 LOAD_CONST               1 (None)
+               750 BUILD_TUPLE              4
+               752 LOAD_CONST              51 (<code object mute_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 843>)
+               754 MAKE_FUNCTION            4 (annotations)
+               756 STORE_NAME              57 (mute_event)
+   
+   866         758 LOAD_CONST              52 ('comment_id')
+               760 LOAD_NAME               33 (int)
+               762 LOAD_CONST              11 ('return')
+               764 LOAD_CONST               1 (None)
+               766 BUILD_TUPLE              4
+               768 LOAD_CONST              53 (<code object delete_comment, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 866>)
+               770 MAKE_FUNCTION            4 (annotations)
+               772 STORE_NAME              58 (delete_comment)
+   
+   877         774 LOAD_CONST              22 ('search_uid')
+               776 LOAD_NAME               33 (int)
+               778 LOAD_CONST              11 ('return')
+               780 LOAD_CONST               1 (None)
+               782 BUILD_TUPLE              4
+               784 LOAD_CONST              54 (<code object reset_inbox, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 877>)
+               786 MAKE_FUNCTION            4 (annotations)
+               788 STORE_NAME              59 (reset_inbox)
+               790 LOAD_CONST               1 (None)
+               792 RETURN_VALUE
    consts
       0
       None
       ('asdict',)
       ('time',)
       ('Any', 'List')
       ('from_dict',)
@@ -1758,15 +1761,15 @@
             0000000000000000000000000000006404a6010000ab0100000000000000
             006a0900000000000000006405190000000000000000007c0364063c0000
             007c03640719000000000000000000a00b00000000000000000000000000
             0000000000000064088400a6010000ab0100000000000000007c0364093c
             0000007c035300
          268           0 RESUME                   0
          
-         269           2 LOAD_CONST               1 ("\n    SELECT \n        s.uid,\n        s.label,\n        s.updated,\n        s.fields,\n        s.meta->>'search_type' as type,\n        s.meta->>'notes' as notes,\n        s.meta->>'products' as products,\n        s.meta->>'services' as services,\n        s.meta->>'customers' as customers,\n        s.meta->>'end_customer' as end_customer,\n        s.meta->>'last_list' as last_list,\n        s.meta->>'next_due_date' as next_due_date,\n        s.meta->>'geographies' as geographies,\n        s.meta->>'week' as week,\n        s.meta->>'day' as day,\n        COALESCE(s.meta->>'search_status', 'active') as search_status\n    FROM search s\n    ORDER BY updated\n    ")
+         269           2 LOAD_CONST               1 ("\n    SELECT \n        s.uid,\n        s.label,\n        s.updated,\n        s.meta->>'type' as type,\n        s.meta->>'notes' as notes,\n        s.meta->>'products' as products,\n        s.meta->>'services' as services,\n        s.meta->>'customers' as customers,\n        s.meta->>'end_customer' as end_customer,\n        s.meta->>'last_list' as last_list,\n        s.meta->>'next_due_date' as next_due_date,\n        s.meta->>'geographies' as geographies,\n        s.meta->>'week' as week,\n        s.meta->>'day' as day,\n\n        COALESCE(s.meta->>'search_status', 'active') as search_status\n    FROM search s\n    ORDER BY updated\n    ")
                        4 STORE_FAST               0 (statement)
          
          290           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
@@ -1850,15 +1853,15 @@
                      454 RETURN_VALUE
          ExceptionTable:
            56 to 250 -> 276 [1] lasti
            276 to 282 -> 284 [3] lasti
            290 to 290 -> 284 [3] lasti
          consts
             None
-            "\n    SELECT \n        s.uid,\n        s.label,\n        s.updated,\n        s.fields,\n        s.meta->>'search_type' as type,\n        s.meta->>'notes' as notes,\n        s.meta->>'products' as products,\n        s.meta->>'services' as services,\n        s.meta->>'customers' as customers,\n        s.meta->>'end_customer' as end_customer,\n        s.meta->>'last_list' as last_list,\n        s.meta->>'next_due_date' as next_due_date,\n        s.meta->>'geographies' as geographies,\n        s.meta->>'week' as week,\n        s.meta->>'day' as day,\n        COALESCE(s.meta->>'search_status', 'active') as search_status\n    FROM search s\n    ORDER BY updated\n    "
+            "\n    SELECT \n        s.uid,\n        s.label,\n        s.updated,\n        s.meta->>'type' as type,\n        s.meta->>'notes' as notes,\n        s.meta->>'products' as products,\n        s.meta->>'services' as services,\n        s.meta->>'customers' as customers,\n        s.meta->>'end_customer' as end_customer,\n        s.meta->>'last_list' as last_list,\n        s.meta->>'next_due_date' as next_due_date,\n        s.meta->>'geographies' as geographies,\n        s.meta->>'week' as week,\n        s.meta->>'day' as day,\n\n        COALESCE(s.meta->>'search_status', 'active') as search_status\n    FROM search s\n    ORDER BY updated\n    "
             ('columns',)
             'label'
             ' - '
             0
             'client'
             'uid'
             code
@@ -1905,164 +1908,28 @@
          varnames   ('statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'searches_query'
          firstlineno 268
          lnotab 0x0201041534014e0174fe2e035c01240104ff1603
-      90
-      'trailing_days'
-      code
-         argcount  : 1
-         nlocals   : 5
-         stacksize : 6
-         flags     : 3
-         code
-            0x97007401000000000000000000007c00740200000000000000000000a6
-            020000ab02000000000000000073024a00820164017c009b0064029d037d
-            01740400000000000000000000a003000000000000000000000000000000
-            0000000000a6000000ab00000000000000000035007d027c02a004000000
-            0000000000000000000000000000000000740b000000000000000000006a
-            0600000000000000007c01a6010000ab010000000000000000a6010000ab
-            0100000000000000007d03740f000000000000000000006a080000000000
-            0000007c03a0090000000000000000000000000000000000000000a60000
-            00ab0000000000000000007c03a00a000000000000000000000000000000
-            0000000000a6000000ab000000000000000000ac03a6020000ab02000000
-            00000000007d04640064006400a6020000ab02000000000000000001006e
-            0b2300310073047702780359007701010059000100010074170000000000
-            00000000007c046404190000000000000000007c04640419000000000000
-            000000a00c0000000000000000000000000000000000000000a6000000ab
-            0000000000000000007a0b00006405a6020000ab0200000000000000007c
-            0464063c0000007c045300
-         301           0 RESUME                   0
-         
-         302           2 LOAD_GLOBAL              1 (NULL + isinstance)
-                      14 LOAD_FAST                0 (trailing_days)
-                      16 LOAD_GLOBAL              2 (int)
-                      28 PRECALL                  2
-                      32 CALL                     2
-                      42 POP_JUMP_FORWARD_IF_TRUE     2 (to 48)
-                      44 LOAD_ASSERTION_ERROR
-                      46 RAISE_VARARGS            1
-         
-         303     >>   48 LOAD_CONST               1 ("\n    WITH ranked_actors AS (\n        SELECT \n            a.name as analyst,\n            a.key,\n            s.uid,\n            COUNT(e.id) AS count,\n            MAX(e.created) AS max_created,\n            ROW_NUMBER() OVER (\n                PARTITION BY s.uid\n                ORDER BY COUNT(e.id) DESC\n            ) as rn\n        FROM \n            event e\n        INNER JOIN \n            actor a ON a.key = e.actor_key\n        INNER JOIN \n            search s ON s.uid = e.search_uid\n        WHERE\n            a.type = 'research' \n            AND e.type = 'validate'\n            AND to_timestamp(e.created) > now() - interval '")
-         
-         324          50 LOAD_FAST                0 (trailing_days)
-         
-         303          52 FORMAT_VALUE             0
-                      54 LOAD_CONST               2 (" day'\n        GROUP BY \n            a.key, analyst, s.uid\n    )\n    SELECT \n        key as actor_key,\n        analyst, \n        uid, \n        count,\n        max_created\n    FROM \n        ranked_actors\n    WHERE \n        rn = 1;\n    ")
-                      56 BUILD_STRING             3
-                      58 STORE_FAST               1 (statement)
-         
-         339          60 LOAD_GLOBAL              4 (db)
-                      72 LOAD_METHOD              3 (connect)
-                      94 PRECALL                  0
-                      98 CALL                     0
-                     108 BEFORE_WITH
-                     110 STORE_FAST               2 (conn)
-         
-         340         112 LOAD_FAST                2 (conn)
-                     114 LOAD_METHOD              4 (execute)
-                     136 LOAD_GLOBAL             11 (NULL + sqlalchemy)
-                     148 LOAD_ATTR                6 (text)
-                     158 LOAD_FAST                1 (statement)
-                     160 PRECALL                  1
-                     164 CALL                     1
-                     174 PRECALL                  1
-                     178 CALL                     1
-                     188 STORE_FAST               3 (result)
-         
-         341         190 LOAD_GLOBAL             15 (NULL + pd)
-                     202 LOAD_ATTR                8 (DataFrame)
-                     212 LOAD_FAST                3 (result)
-                     214 LOAD_METHOD              9 (fetchall)
-                     236 PRECALL                  0
-                     240 CALL                     0
-                     250 LOAD_FAST                3 (result)
-                     252 LOAD_METHOD             10 (keys)
-                     274 PRECALL                  0
-                     278 CALL                     0
-                     288 KW_NAMES                 3
-                     290 PRECALL                  2
-                     294 CALL                     2
-                     304 STORE_FAST               4 (df)
-         
-         339         306 LOAD_CONST               0 (None)
-                     308 LOAD_CONST               0 (None)
-                     310 LOAD_CONST               0 (None)
-                     312 PRECALL                  2
-                     316 CALL                     2
-                     326 POP_TOP
-                     328 JUMP_FORWARD            11 (to 352)
-                 >>  330 PUSH_EXC_INFO
-                     332 WITH_EXCEPT_START
-                     334 POP_JUMP_FORWARD_IF_TRUE     4 (to 344)
-                     336 RERAISE                  2
-                 >>  338 COPY                     3
-                     340 POP_EXCEPT
-                     342 RERAISE                  1
-                 >>  344 POP_TOP
-                     346 POP_EXCEPT
-                     348 POP_TOP
-                     350 POP_TOP
-         
-         342     >>  352 LOAD_GLOBAL             23 (NULL + round)
-                     364 LOAD_FAST                4 (df)
-                     366 LOAD_CONST               4 ('count')
-                     368 BINARY_SUBSCR
-                     378 LOAD_FAST                4 (df)
-                     380 LOAD_CONST               4 ('count')
-                     382 BINARY_SUBSCR
-                     392 LOAD_METHOD             12 (max)
-                     414 PRECALL                  0
-                     418 CALL                     0
-                     428 BINARY_OP               11 (/)
-                     432 LOAD_CONST               5 (2)
-                     434 PRECALL                  2
-                     438 CALL                     2
-                     448 LOAD_FAST                4 (df)
-                     450 LOAD_CONST               6 ('activity')
-                     452 STORE_SUBSCR
-         
-         343         456 LOAD_FAST                4 (df)
-                     458 RETURN_VALUE
-         ExceptionTable:
-           110 to 304 -> 330 [1] lasti
-           330 to 336 -> 338 [3] lasti
-           344 to 344 -> 338 [3] lasti
-         consts
-            None
-            "\n    WITH ranked_actors AS (\n        SELECT \n            a.name as analyst,\n            a.key,\n            s.uid,\n            COUNT(e.id) AS count,\n            MAX(e.created) AS max_created,\n            ROW_NUMBER() OVER (\n                PARTITION BY s.uid\n                ORDER BY COUNT(e.id) DESC\n            ) as rn\n        FROM \n            event e\n        INNER JOIN \n            actor a ON a.key = e.actor_key\n        INNER JOIN \n            search s ON s.uid = e.search_uid\n        WHERE\n            a.type = 'research' \n            AND e.type = 'validate'\n            AND to_timestamp(e.created) > now() - interval '"
-            " day'\n        GROUP BY \n            a.key, analyst, s.uid\n    )\n    SELECT \n        key as actor_key,\n        analyst, \n        uid, \n        count,\n        max_created\n    FROM \n        ranked_actors\n    WHERE \n        rn = 1;\n    "
-            ('columns',)
-            'count'
-            2
-            'activity'
-         names      ('isinstance', 'int', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'round', 'max')
-         varnames   ('trailing_days', 'statement', 'conn', 'result', 'df')
-         freevars   ()
-         cellvars   ()
-         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
-         name       'recent_validations'
-         firstlineno 301
-         lnotab 0x02012e01021502eb082434014e0174fe2e036801
       code
          argcount  : 0
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970064017d007401000000000000000000006a0100000000000000007c
             00740400000000000000000000a6020000ab0200000000000000005300
-         346           0 RESUME                   0
+         300           0 RESUME                   0
          
-         347           2 LOAD_CONST               1 ('\n       SELECT\n        search_uid,\n        AVG(rating::int) AS rating_avg,\n        COUNT(rating) as rating_count\n    FROM rating \n    GROUP BY search_uid\n    ')
+         301           2 LOAD_CONST               1 ('\n       SELECT\n        search_uid,\n        AVG(rating::int) AS rating_avg,\n        COUNT(rating) as rating_count\n    FROM rating \n    GROUP BY search_uid\n    ')
                        4 STORE_FAST               0 (query)
          
-         355           6 LOAD_GLOBAL              1 (NULL + pd)
+         309           6 LOAD_GLOBAL              1 (NULL + pd)
                       18 LOAD_ATTR                1 (read_sql)
                       28 LOAD_FAST                0 (query)
                       30 LOAD_GLOBAL              4 (db)
                       42 PRECALL                  2
                       46 CALL                     2
                       56 RETURN_VALUE
          consts
@@ -2070,15 +1937,15 @@
             '\n       SELECT\n        search_uid,\n        AVG(rating::int) AS rating_avg,\n        COUNT(rating) as rating_count\n    FROM rating \n    GROUP BY search_uid\n    '
          names      ('pd', 'read_sql', 'db')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'average_rating_per_search_query'
-         firstlineno 346
+         firstlineno 300
          lnotab 0x02010408
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -2090,66 +1957,66 @@
             0600000000000000007c02a0070000000000000000000000000000000000
             000000a6000000ab0000000000000000007c02a008000000000000000000
             0000000000000000000000a6000000ab000000000000000000ac02a60200
             00ab0200000000000000007d037413000000000000000000007c03640319
             00000000000000000064047a0b00006405a6020000ab0200000000000000
             007c0364063c000000640064006400a6020000ab02000000000000000001
             006e0b230031007304770278035900770101005900010001007c035300
-         358           0 RESUME                   0
+         312           0 RESUME                   0
          
-         359           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT\n            e.search_uid,\n            a.name as analyst,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 7 * 86400 THEN 1 ELSE 0 END) AS last_7_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400 THEN 1 ELSE 0 END) AS last_30_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) AS last_90_days,\n            SUM(CASE WHEN e.type = 'validate' THEN 1 ELSE 0 END) AS total_validations,\n            RANK() OVER (PARTITION BY e.search_uid ORDER BY SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) DESC) as rank\n        FROM\n            event e\n        LEFT JOIN\n            actor a ON a.key = e.actor_key\n        WHERE\n            e.type = 'validate'\n        GROUP BY\n            e.search_uid, analyst\n    )\n    SELECT\n        search_uid,\n        analyst,\n        last_7_days,\n        last_30_days,\n        last_90_days,\n        total_validations\n    FROM\n        RankedEvents\n    WHERE\n        rank = 1\n        AND last_90_days > 0\n    ;\n    ")
+         313           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT\n            e.search_uid,\n            a.name as analyst,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 1 * 86400 THEN 1 ELSE 0 END) AS last_1_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 7 * 86400 THEN 1 ELSE 0 END) AS last_7_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400 THEN 1 ELSE 0 END) AS last_30_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) AS last_90_days,\n            SUM(CASE WHEN e.type = 'validate' THEN 1 ELSE 0 END) AS total_validations,\n            RANK() OVER (PARTITION BY e.search_uid ORDER BY SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) DESC) as rank\n        FROM\n            event e\n        LEFT JOIN\n            actor a ON a.key = e.actor_key\n        WHERE\n            e.type = 'validate'\n        GROUP BY\n            e.search_uid, analyst\n    )\n    SELECT\n        search_uid,\n        analyst,\n        last_1_days,\n        last_7_days,\n        last_30_days,\n        last_90_days,\n        total_validations\n    FROM\n        RankedEvents\n    WHERE\n        rank = 1\n        AND last_90_days > 0\n    ;\n    ")
                        4 STORE_FAST               0 (stmt)
          
-         392           6 LOAD_GLOBAL              0 (db)
+         348           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               1 (conn)
          
-         393          58 LOAD_FAST                1 (conn)
+         349          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                0 (stmt)
                      106 PRECALL                  1
                      110 CALL                     1
                      120 PRECALL                  1
                      124 CALL                     1
                      134 STORE_FAST               2 (result)
          
-         394         136 LOAD_GLOBAL             11 (NULL + pd)
+         350         136 LOAD_GLOBAL             11 (NULL + pd)
                      148 LOAD_ATTR                6 (DataFrame)
                      158 LOAD_FAST                2 (result)
                      160 LOAD_METHOD              7 (fetchall)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 LOAD_FAST                2 (result)
                      198 LOAD_METHOD              8 (keys)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 KW_NAMES                 2
                      236 PRECALL                  2
                      240 CALL                     2
                      250 STORE_FAST               3 (df)
          
-         395         252 LOAD_GLOBAL             19 (NULL + round)
+         351         252 LOAD_GLOBAL             19 (NULL + round)
                      264 LOAD_FAST                3 (df)
                      266 LOAD_CONST               3 ('total_validations')
                      268 BINARY_SUBSCR
                      278 LOAD_CONST               4 (300)
                      280 BINARY_OP               11 (/)
                      284 LOAD_CONST               5 (2)
                      286 PRECALL                  2
                      290 CALL                     2
                      300 LOAD_FAST                3 (df)
                      302 LOAD_CONST               6 ('total_validations_pct')
                      304 STORE_SUBSCR
          
-         392         308 LOAD_CONST               0 (None)
+         348         308 LOAD_CONST               0 (None)
                      310 LOAD_CONST               0 (None)
                      312 LOAD_CONST               0 (None)
                      314 PRECALL                  2
                      318 CALL                     2
                      328 POP_TOP
                      330 JUMP_FORWARD            11 (to 354)
                  >>  332 PUSH_EXC_INFO
@@ -2160,36 +2027,128 @@
                      342 POP_EXCEPT
                      344 RERAISE                  1
                  >>  346 POP_TOP
                      348 POP_EXCEPT
                      350 POP_TOP
                      352 POP_TOP
          
-         396     >>  354 LOAD_FAST                3 (df)
+         352     >>  354 LOAD_FAST                3 (df)
                      356 RETURN_VALUE
          ExceptionTable:
            56 to 306 -> 332 [1] lasti
            332 to 338 -> 340 [3] lasti
            346 to 346 -> 340 [3] lasti
          consts
             None
-            "\n    WITH RankedEvents AS (\n        SELECT\n            e.search_uid,\n            a.name as analyst,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 7 * 86400 THEN 1 ELSE 0 END) AS last_7_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400 THEN 1 ELSE 0 END) AS last_30_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) AS last_90_days,\n            SUM(CASE WHEN e.type = 'validate' THEN 1 ELSE 0 END) AS total_validations,\n            RANK() OVER (PARTITION BY e.search_uid ORDER BY SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) DESC) as rank\n        FROM\n            event e\n        LEFT JOIN\n            actor a ON a.key = e.actor_key\n        WHERE\n            e.type = 'validate'\n        GROUP BY\n            e.search_uid, analyst\n    )\n    SELECT\n        search_uid,\n        analyst,\n        last_7_days,\n        last_30_days,\n        last_90_days,\n        total_validations\n    FROM\n        RankedEvents\n    WHERE\n        rank = 1\n        AND last_90_days > 0\n    ;\n    "
+            "\n    WITH RankedEvents AS (\n        SELECT\n            e.search_uid,\n            a.name as analyst,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 1 * 86400 THEN 1 ELSE 0 END) AS last_1_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 7 * 86400 THEN 1 ELSE 0 END) AS last_7_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400 THEN 1 ELSE 0 END) AS last_30_days,\n            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) AS last_90_days,\n            SUM(CASE WHEN e.type = 'validate' THEN 1 ELSE 0 END) AS total_validations,\n            RANK() OVER (PARTITION BY e.search_uid ORDER BY SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) DESC) as rank\n        FROM\n            event e\n        LEFT JOIN\n            actor a ON a.key = e.actor_key\n        WHERE\n            e.type = 'validate'\n        GROUP BY\n            e.search_uid, analyst\n    )\n    SELECT\n        search_uid,\n        analyst,\n        last_1_days,\n        last_7_days,\n        last_30_days,\n        last_90_days,\n        total_validations\n    FROM\n        RankedEvents\n    WHERE\n        rank = 1\n        AND last_90_days > 0\n    ;\n    "
             ('columns',)
             'total_validations'
             300
             2
             'total_validations_pct'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'round')
          varnames   ('stmt', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'validation_history'
-         firstlineno 358
-         lnotab 0x0201042134014e01740138fd2e04
+         firstlineno 312
+         lnotab 0x0201042334014e01740138fd2e04
+      code
+         argcount  : 0
+         nlocals   : 4
+         stacksize : 6
+         flags     : 3
+         code
+            0x970064017d00740000000000000000000000a001000000000000000000
+            0000000000000000000000a6000000ab00000000000000000035007d017c
+            01a002000000000000000000000000000000000000000074070000000000
+            00000000006a0400000000000000007c00a6010000ab0100000000000000
+            00a6010000ab0100000000000000007d02740b000000000000000000006a
+            0600000000000000007c02a0070000000000000000000000000000000000
+            000000a6000000ab0000000000000000007c02a008000000000000000000
+            0000000000000000000000a6000000ab000000000000000000ac02a60200
+            00ab0200000000000000007d03640064006400a6020000ab020000000000
+            00000001006e0b230031007304770278035900770101005900010001007c
+            035300
+         355           0 RESUME                   0
+         
+         356           2 LOAD_CONST               1 ("\n        SELECT \n            e.search_uid as uid,\n            COUNT(*) as comment_count\n        FROM event e\n        WHERE \n            e.type = 'comment'\n            AND e.domain is null\n            -- last 30 days\n            AND e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400\n        GROUP BY e.search_uid\n        ")
+                       4 STORE_FAST               0 (statement)
+         
+         368           6 LOAD_GLOBAL              0 (db)
+                      18 LOAD_METHOD              1 (connect)
+                      40 PRECALL                  0
+                      44 CALL                     0
+                      54 BEFORE_WITH
+                      56 STORE_FAST               1 (conn)
+         
+         369          58 LOAD_FAST                1 (conn)
+                      60 LOAD_METHOD              2 (execute)
+                      82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                0 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+                     120 PRECALL                  1
+                     124 CALL                     1
+                     134 STORE_FAST               2 (result)
+         
+         370         136 LOAD_GLOBAL             11 (NULL + pd)
+                     148 LOAD_ATTR                6 (DataFrame)
+                     158 LOAD_FAST                2 (result)
+                     160 LOAD_METHOD              7 (fetchall)
+                     182 PRECALL                  0
+                     186 CALL                     0
+                     196 LOAD_FAST                2 (result)
+                     198 LOAD_METHOD              8 (keys)
+                     220 PRECALL                  0
+                     224 CALL                     0
+                     234 KW_NAMES                 2
+                     236 PRECALL                  2
+                     240 CALL                     2
+                     250 STORE_FAST               3 (df)
+         
+         368         252 LOAD_CONST               0 (None)
+                     254 LOAD_CONST               0 (None)
+                     256 LOAD_CONST               0 (None)
+                     258 PRECALL                  2
+                     262 CALL                     2
+                     272 POP_TOP
+                     274 JUMP_FORWARD            11 (to 298)
+                 >>  276 PUSH_EXC_INFO
+                     278 WITH_EXCEPT_START
+                     280 POP_JUMP_FORWARD_IF_TRUE     4 (to 290)
+                     282 RERAISE                  2
+                 >>  284 COPY                     3
+                     286 POP_EXCEPT
+                     288 RERAISE                  1
+                 >>  290 POP_TOP
+                     292 POP_EXCEPT
+                     294 POP_TOP
+                     296 POP_TOP
+         
+         372     >>  298 LOAD_FAST                3 (df)
+                     300 RETURN_VALUE
+         ExceptionTable:
+           56 to 250 -> 276 [1] lasti
+           276 to 282 -> 284 [3] lasti
+           290 to 290 -> 284 [3] lasti
+         consts
+            None
+            "\n        SELECT \n            e.search_uid as uid,\n            COUNT(*) as comment_count\n        FROM event e\n        WHERE \n            e.type = 'comment'\n            AND e.domain is null\n            -- last 30 days\n            AND e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400\n        GROUP BY e.search_uid\n        "
+            ('columns',)
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
+         varnames   ('statement', 'conn', 'result', 'df')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+         name       'searches_comment_counts'
+         firstlineno 355
+         lnotab 0x0201040c34014e0174fe2e04
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
@@ -2197,93 +2156,137 @@
             00a00200000000000000000000000000000000000000007c016401640264
             03ac04a6040000ab0400000000000000007d027c02640519000000000000
             000000a00300000000000000000000000000000000000000006406a60100
             00ab0100000000000000007c0264053c0000007c02640719000000000000
             000000a00300000000000000000000000000000000000000006406a60100
             00ab0100000000000000007c0264073c0000007c02640819000000000000
             000000a00300000000000000000000000000000000000000006406a60100
-            00ab0100000000000000007c0264083c0000007c025300
-         399           0 RESUME                   0
+            00ab0100000000000000007c0264083c0000007c02640919000000000000
+            000000a00300000000000000000000000000000000000000006406a60100
+            00ab0100000000000000007c0264093c0000007c02a00200000000000000
+            00000000000000000000000000740900000000000000000000a6000000ab
+            00000000000000000064016403ac0aa6030000ab0300000000000000007d
+            027c02640b19000000000000000000a00300000000000000000000000000
+            000000000000006406a6010000ab0100000000000000007c02640b3c0000
+            007c025300
+         375           0 RESUME                   0
          
-         400           2 LOAD_GLOBAL              1 (NULL + searches_query)
+         376           2 LOAD_GLOBAL              1 (NULL + searches_query)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               0 (searches)
          
-         402          30 LOAD_GLOBAL              3 (NULL + validation_history)
+         378          30 LOAD_GLOBAL              3 (NULL + validation_history)
                       42 PRECALL                  0
                       46 CALL                     0
                       56 STORE_FAST               1 (recent_event_count)
          
-         404          58 LOAD_FAST                0 (searches)
+         380          58 LOAD_FAST                0 (searches)
                       60 LOAD_METHOD              2 (merge)
          
-         405          82 LOAD_FAST                1 (recent_event_count)
+         381          82 LOAD_FAST                1 (recent_event_count)
                       84 LOAD_CONST               1 ('uid')
                       86 LOAD_CONST               2 ('search_uid')
                       88 LOAD_CONST               3 ('left')
          
-         404          90 KW_NAMES                 4
+         380          90 KW_NAMES                 4
                       92 PRECALL                  4
                       96 CALL                     4
                      106 STORE_FAST               2 (df)
          
-         408         108 LOAD_FAST                2 (df)
-                     110 LOAD_CONST               5 ('last_7_days')
+         384         108 LOAD_FAST                2 (df)
+                     110 LOAD_CONST               5 ('last_1_days')
                      112 BINARY_SUBSCR
                      122 LOAD_METHOD              3 (fillna)
                      144 LOAD_CONST               6 (0)
                      146 PRECALL                  1
                      150 CALL                     1
                      160 LOAD_FAST                2 (df)
-                     162 LOAD_CONST               5 ('last_7_days')
+                     162 LOAD_CONST               5 ('last_1_days')
                      164 STORE_SUBSCR
          
-         409         168 LOAD_FAST                2 (df)
-                     170 LOAD_CONST               7 ('last_30_days')
+         385         168 LOAD_FAST                2 (df)
+                     170 LOAD_CONST               7 ('last_7_days')
                      172 BINARY_SUBSCR
                      182 LOAD_METHOD              3 (fillna)
                      204 LOAD_CONST               6 (0)
                      206 PRECALL                  1
                      210 CALL                     1
                      220 LOAD_FAST                2 (df)
-                     222 LOAD_CONST               7 ('last_30_days')
+                     222 LOAD_CONST               7 ('last_7_days')
                      224 STORE_SUBSCR
          
-         410         228 LOAD_FAST                2 (df)
-                     230 LOAD_CONST               8 ('last_90_days')
+         386         228 LOAD_FAST                2 (df)
+                     230 LOAD_CONST               8 ('last_30_days')
                      232 BINARY_SUBSCR
                      242 LOAD_METHOD              3 (fillna)
                      264 LOAD_CONST               6 (0)
                      266 PRECALL                  1
                      270 CALL                     1
                      280 LOAD_FAST                2 (df)
-                     282 LOAD_CONST               8 ('last_90_days')
+                     282 LOAD_CONST               8 ('last_30_days')
                      284 STORE_SUBSCR
          
-         419         288 LOAD_FAST                2 (df)
-                     290 RETURN_VALUE
+         387         288 LOAD_FAST                2 (df)
+                     290 LOAD_CONST               9 ('last_90_days')
+                     292 BINARY_SUBSCR
+                     302 LOAD_METHOD              3 (fillna)
+                     324 LOAD_CONST               6 (0)
+                     326 PRECALL                  1
+                     330 CALL                     1
+                     340 LOAD_FAST                2 (df)
+                     342 LOAD_CONST               9 ('last_90_days')
+                     344 STORE_SUBSCR
+         
+         389         348 LOAD_FAST                2 (df)
+                     350 LOAD_METHOD              2 (merge)
+                     372 LOAD_GLOBAL              9 (NULL + searches_comment_counts)
+                     384 PRECALL                  0
+                     388 CALL                     0
+                     398 LOAD_CONST               1 ('uid')
+                     400 LOAD_CONST               3 ('left')
+                     402 KW_NAMES                10
+                     404 PRECALL                  3
+                     408 CALL                     3
+                     418 STORE_FAST               2 (df)
+         
+         390         420 LOAD_FAST                2 (df)
+                     422 LOAD_CONST              11 ('comment_count')
+                     424 BINARY_SUBSCR
+                     434 LOAD_METHOD              3 (fillna)
+                     456 LOAD_CONST               6 (0)
+                     458 PRECALL                  1
+                     462 CALL                     1
+                     472 LOAD_FAST                2 (df)
+                     474 LOAD_CONST              11 ('comment_count')
+                     476 STORE_SUBSCR
+         
+         399         480 LOAD_FAST                2 (df)
+                     482 RETURN_VALUE
          consts
             None
             'uid'
             'search_uid'
             'left'
             ('left_on', 'right_on', 'how')
-            'last_7_days'
+            'last_1_days'
             0
+            'last_7_days'
             'last_30_days'
             'last_90_days'
-         names      ('searches_query', 'validation_history', 'merge', 'fillna')
+            ('on', 'how')
+            'comment_count'
+         names      ('searches_query', 'validation_history', 'merge', 'fillna', 'searches_comment_counts')
          varnames   ('searches', 'recent_event_count', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'enriched_searches_query'
-         firstlineno 399
-         lnotab 0x02011c021c02180108ff12043c013c013c09
+         firstlineno 375
+         lnotab 0x02011c021c02180108ff12043c013c013c013c0248013c09
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
@@ -2294,66 +2297,66 @@
             00000000007c01a0070000000000000000000000000000000000000000a6
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d027c02a0090000000000000000000000000000000000
             00000067006403a201ac02a6010000ab0100000000000000007d027c0263
             02640064006400a6020000ab020000000000000000010053002300310073
             047702780359007701010059000100010064005300
-         422           0 RESUME                   0
+         402           0 RESUME                   0
          
-         423           2 LOAD_GLOBAL              0 (db)
+         403           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         424          54 LOAD_FAST                0 (conn)
+         404          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         425          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         405          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         426         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
+         406         100 LOAD_CONST               1 ('\n                SELECT * FROM actor\n                ')
          
-         425         102 PRECALL                  1
+         405         102 PRECALL                  1
                      106 CALL                     1
          
-         424         116 PRECALL                  1
+         404         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         431         132 LOAD_GLOBAL             11 (NULL + pd)
+         411         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         432         248 LOAD_FAST                2 (df)
+         412         248 LOAD_FAST                2 (df)
                      250 LOAD_METHOD              9 (drop)
                      272 BUILD_LIST               0
                      274 LOAD_CONST               3 (('id', 'created', 'updated'))
                      276 LIST_EXTEND              1
                      278 KW_NAMES                 2
                      280 PRECALL                  1
                      284 CALL                     1
                      294 STORE_FAST               2 (df)
          
-         433         296 LOAD_FAST                2 (df)
+         413         296 LOAD_FAST                2 (df)
          
-         423         298 SWAP                     2
+         403         298 SWAP                     2
                      300 LOAD_CONST               0 (None)
                      302 LOAD_CONST               0 (None)
                      304 LOAD_CONST               0 (None)
                      306 PRECALL                  2
                      310 CALL                     2
                      320 POP_TOP
                      322 RETURN_VALUE
@@ -2381,15 +2384,15 @@
             ('id', 'created', 'updated')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'drop')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'actor'
-         firstlineno 422
+         firstlineno 402
          lnotab 0x020134011801160102ff0eff10077401300102f6
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -2402,54 +2405,54 @@
             000000ab0000000000000000007c01a00800000000000000000000000000
             00000000000000a6000000ab000000000000000000ac02a6020000ab0200
             000000000000007d02640064006400a6020000ab02000000000000000001
             006e0b23003100730477027803590077010100590001000100640384007d
             037c02640419000000000000000000a00900000000000000000000000000
             000000000000007c03a6010000ab0100000000000000007c0264053c0000
             007c025300
-         436           0 RESUME                   0
+         416           0 RESUME                   0
          
-         437           2 LOAD_GLOBAL              0 (db)
+         417           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         438          54 LOAD_FAST                0 (conn)
+         418          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         439          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         419          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         440         100 LOAD_CONST               1 ("\n                SELECT \n                    e.id,\n                    e.domain,\n                    e.created as updated,\n                    a.name as updated_by, \n                    to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n                    c.name, \n                    c.description,\n                    c.source,\n                    c.meta->>'ownership' as ownership, \n                    c.meta->>'headquarters' as headquarters,\n                    c.meta->>'city' as city,\n                    c.meta->>'state' as state,\n                    c.meta->>'designation' as designation,\n                    c.meta->>'products' as products,\n                    c.meta->>'services' as services,\n                    c.meta->>'end_customer' as end_customer,\n                    c.meta->>'geographies' as geographies,\n                    c.meta->>'was_acquired' as was_acquired,\n                    c.meta->>'justification' as justification,\n                    c.meta->>'year_founded' as year_founded,\n                    c.meta->>'linkedin' as linkedin,\n                    c.meta->>'linkedin_range' as linkedin_range,\n                    c.meta->>'primary_contact' as primary_contact,\n                    c.meta->>'industry' as industry,\n                    c.meta->>'revenue_estimates' as revenue_estimates,\n                    c.meta->>'location_count' as location_count,\n                    c.meta->>'business_models' as business_models,\n                    c.meta->>'facility_size' as facility_size,\n                    c.meta,\n                    COALESCE(co.comments, '[]'::jsonb) as comments\n                FROM event e\n                LEFT JOIN actor a ON e.actor_key = a.key\n                LEFT JOIN company c ON e.domain = c.domain\n                LEFT JOIN comment co ON e.domain = co.domain\n                WHERE e.type = 'buyer'\n                ")
+         420         100 LOAD_CONST               1 ("\n                SELECT \n                    e.id,\n                    e.domain,\n                    e.created as updated,\n                    a.name as updated_by, \n                    to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n                    c.name, \n                    c.description,\n                    c.source,\n                    c.meta->>'ownership' as ownership, \n                    c.meta->>'headquarters' as headquarters,\n                    c.meta->>'city' as city,\n                    c.meta->>'state' as state,\n                    c.meta->>'designation' as designation,\n                    c.meta->>'products' as products,\n                    c.meta->>'services' as services,\n                    c.meta->>'end_customer' as end_customer,\n                    c.meta->>'geographies' as geographies,\n                    c.meta->>'was_acquired' as was_acquired,\n                    c.meta->>'justification' as justification,\n                    c.meta->>'year_founded' as year_founded,\n                    c.meta->>'linkedin' as linkedin,\n                    c.meta->>'linkedin_range' as linkedin_range,\n                    c.meta->>'primary_contact' as primary_contact,\n                    c.meta->>'industry' as industry,\n                    c.meta->>'revenue_estimates' as revenue_estimates,\n                    c.meta->>'location_count' as location_count,\n                    c.meta->>'business_models' as business_models,\n                    c.meta->>'facility_size' as facility_size,\n                    c.meta,\n                    COALESCE(co.comments, '[]'::jsonb) as comments\n                FROM event e\n                LEFT JOIN actor a ON e.actor_key = a.key\n                LEFT JOIN company c ON e.domain = c.domain\n                LEFT JOIN comment co ON e.domain = co.domain\n                WHERE e.type = 'buyer'\n                ")
          
-         439         102 PRECALL                  1
+         419         102 PRECALL                  1
                      106 CALL                     1
          
-         438         116 PRECALL                  1
+         418         116 PRECALL                  1
                      120 CALL                     1
                      130 STORE_FAST               1 (result)
          
-         480         132 LOAD_GLOBAL             11 (NULL + pd)
+         460         132 LOAD_GLOBAL             11 (NULL + pd)
                      144 LOAD_ATTR                6 (DataFrame)
                      154 LOAD_FAST                1 (result)
                      156 LOAD_METHOD              7 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                1 (result)
                      194 LOAD_METHOD              8 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 2
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               2 (df)
          
-         437         248 LOAD_CONST               0 (None)
+         417         248 LOAD_CONST               0 (None)
                      250 LOAD_CONST               0 (None)
                      252 LOAD_CONST               0 (None)
                      254 PRECALL                  2
                      258 CALL                     2
                      268 POP_TOP
                      270 JUMP_FORWARD            11 (to 294)
                  >>  272 PUSH_EXC_INFO
@@ -2460,30 +2463,30 @@
                      282 POP_EXCEPT
                      284 RERAISE                  1
                  >>  286 POP_TOP
                      288 POP_EXCEPT
                      290 POP_TOP
                      292 POP_TOP
          
-         482     >>  294 LOAD_CONST               3 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 482>)
+         462     >>  294 LOAD_CONST               3 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 462>)
                      296 MAKE_FUNCTION            0
                      298 STORE_FAST               3 (get_employees)
          
-         494         300 LOAD_FAST                2 (df)
+         474         300 LOAD_FAST                2 (df)
                      302 LOAD_CONST               4 ('meta')
                      304 BINARY_SUBSCR
                      314 LOAD_METHOD              9 (apply)
                      336 LOAD_FAST                3 (get_employees)
                      338 PRECALL                  1
                      342 CALL                     1
                      352 LOAD_FAST                2 (df)
                      354 LOAD_CONST               5 ('employees')
                      356 STORE_SUBSCR
          
-         495         360 LOAD_FAST                2 (df)
+         475         360 LOAD_FAST                2 (df)
                      362 RETURN_VALUE
          ExceptionTable:
            52 to 246 -> 272 [1] lasti
            272 to 278 -> 280 [3] lasti
            286 to 286 -> 280 [3] lasti
          consts
             None
@@ -2498,60 +2501,60 @@
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab010000000000000000721e09007403000000000000000000007c
                   00640119000000000000000000a6010000ab010000000000000000530023
                   0001005900640053007803590077017c00a0000000000000000000000000
                   0000000000000000006402a6010000ab010000000000000000721b7c0064
                   0219000000000000000000a0000000000000000000000000000000000000
                   0000006403a6010000ab010000000000000000530064005300
-               482           0 RESUME                   0
+               462           0 RESUME                   0
                
-               483           2 LOAD_FAST                0 (meta)
+               463           2 LOAD_FAST                0 (meta)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('employees')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    30 (to 104)
                
-               485          44 NOP
+               465          44 NOP
                
-               486          46 LOAD_GLOBAL              3 (NULL + int)
+               466          46 LOAD_GLOBAL              3 (NULL + int)
                             58 LOAD_FAST                0 (meta)
                             60 LOAD_CONST               1 ('employees')
                             62 BINARY_SUBSCR
                             72 PRECALL                  1
                             76 CALL                     1
                             86 RETURN_VALUE
                        >>   88 PUSH_EXC_INFO
                
-               487          90 POP_TOP
+               467          90 POP_TOP
                
-               488          92 POP_EXCEPT
+               468          92 POP_EXCEPT
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                        >>   98 COPY                     3
                            100 POP_EXCEPT
                            102 RERAISE                  1
                
-               489     >>  104 LOAD_FAST                0 (meta)
+               469     >>  104 LOAD_FAST                0 (meta)
                            106 LOAD_METHOD              0 (get)
                            128 LOAD_CONST               2 ('grata_employee_estimates')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 POP_JUMP_FORWARD_IF_FALSE    27 (to 200)
                
-               490         146 LOAD_FAST                0 (meta)
+               470         146 LOAD_FAST                0 (meta)
                            148 LOAD_CONST               2 ('grata_employee_estimates')
                            150 BINARY_SUBSCR
                            160 LOAD_METHOD              0 (get)
                            182 LOAD_CONST               3 ('count')
                            184 PRECALL                  1
                            188 CALL                     1
                            198 RETURN_VALUE
                
-               492     >>  200 LOAD_CONST               0 (None)
+               472     >>  200 LOAD_CONST               0 (None)
                            202 RETURN_VALUE
                ExceptionTable:
                  46 to 84 -> 88 [0]
                  88 to 90 -> 98 [1] lasti
                consts
                   None
                   'employees'
@@ -2559,25 +2562,25 @@
                   'count'
                names      ('get', 'int')
                varnames   ('meta',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_employees'
-               firstlineno 482
+               firstlineno 462
                lnotab 0x02012a0202012c0102010c012a013602
             'meta'
             'employees'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'apply')
          varnames   ('conn', 'result', 'df', 'get_employees')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'buyer'
-         firstlineno 436
+         firstlineno 416
          lnotab 0x020134011801160102ff0eff102a74d52e2d060c3c01
       code
          argcount  : 1
          nlocals   : 10
          stacksize : 6
          flags     : 3
          code
@@ -2599,59 +2602,59 @@
             010000ab0100000000000000007c04640c3c0000007c04640d1900000000
             0000000000a00a00000000000000000000000000000000000000007c07a6
             010000ab0100000000000000007c04640d3c0000007c04a00a0000000000
             0000000000000000000000000000007c08640eac0fa6020000ab02000000
             00000000007c0464103c0000007c04a00a00000000000000000000000000
             000000000000007c09640eac0fa6020000ab0200000000000000007c0464
             113c0000007c045300
-         498           0 RESUME                   0
+         478           0 RESUME                   0
          
-         501           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        c.description,\n        c.source,\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        \n        \n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n    ;\n    ")
+         481           2 LOAD_CONST               1 ("\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        c.description as grata_description,\n        c.meta->>'description' as description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         562           6 LOAD_GLOBAL              0 (db)
+         543           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         563          58 LOAD_FAST                2 (conn)
+         544          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         564          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         545          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                1 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         565         120 LOAD_CONST               2 ('search_uid')
+         546         120 LOAD_CONST               2 ('search_uid')
                      122 LOAD_FAST                0 (search_uid)
                      124 BUILD_MAP                1
          
-         563         126 PRECALL                  2
+         544         126 PRECALL                  2
                      130 CALL                     2
                      140 STORE_FAST               3 (result)
          
-         567         142 LOAD_GLOBAL             11 (NULL + pd)
+         548         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         562         258 LOAD_CONST               0 (None)
+         543         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -2662,139 +2665,139 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         569     >>  304 LOAD_CONST               4 ('return')
+         550     >>  304 LOAD_CONST               4 ('return')
                      306 LOAD_GLOBAL             18 (str)
                      318 BUILD_TUPLE              2
-                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 569>)
+                     320 LOAD_CONST               5 (<code object list_to_csv, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 550>)
                      322 MAKE_FUNCTION            4 (annotations)
                      324 STORE_FAST               5 (list_to_csv)
          
-         581         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 581>)
+         562         326 LOAD_CONST               6 (<code object get_employees, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 562>)
                      328 MAKE_FUNCTION            0
                      330 STORE_FAST               6 (get_employees)
          
-         593         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 593>)
+         574         332 LOAD_CONST               7 (<code object get_ownership, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 574>)
                      334 MAKE_FUNCTION            0
                      336 STORE_FAST               7 (get_ownership)
          
-         601         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 601>)
+         582         338 LOAD_CONST               8 (<code object get_state, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 582>)
                      340 MAKE_FUNCTION            0
                      342 STORE_FAST               8 (get_state)
          
-         611         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 611>)
+         592         344 LOAD_CONST               9 (<code object get_city, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 592>)
                      346 MAKE_FUNCTION            0
                      348 STORE_FAST               9 (get_city)
          
-         620         350 LOAD_FAST                4 (df)
+         601         350 LOAD_FAST                4 (df)
                      352 LOAD_CONST              10 ('end_customer')
                      354 BINARY_SUBSCR
                      364 LOAD_METHOD             10 (apply)
                      386 LOAD_FAST                5 (list_to_csv)
                      388 PRECALL                  1
                      392 CALL                     1
                      402 LOAD_FAST                4 (df)
                      404 LOAD_CONST              10 ('end_customer')
                      406 STORE_SUBSCR
          
-         621         410 LOAD_FAST                4 (df)
+         602         410 LOAD_FAST                4 (df)
                      412 LOAD_CONST              11 ('meta')
                      414 BINARY_SUBSCR
                      424 LOAD_METHOD             10 (apply)
                      446 LOAD_FAST                6 (get_employees)
                      448 PRECALL                  1
                      452 CALL                     1
                      462 LOAD_FAST                4 (df)
                      464 LOAD_CONST              12 ('employees')
                      466 STORE_SUBSCR
          
-         622         470 LOAD_FAST                4 (df)
+         603         470 LOAD_FAST                4 (df)
                      472 LOAD_CONST              13 ('ownership')
                      474 BINARY_SUBSCR
                      484 LOAD_METHOD             10 (apply)
                      506 LOAD_FAST                7 (get_ownership)
                      508 PRECALL                  1
                      512 CALL                     1
                      522 LOAD_FAST                4 (df)
                      524 LOAD_CONST              13 ('ownership')
                      526 STORE_SUBSCR
          
-         623         530 LOAD_FAST                4 (df)
+         604         530 LOAD_FAST                4 (df)
                      532 LOAD_METHOD             10 (apply)
                      554 LOAD_FAST                8 (get_state)
                      556 LOAD_CONST              14 (1)
                      558 KW_NAMES                15
                      560 PRECALL                  2
                      564 CALL                     2
                      574 LOAD_FAST                4 (df)
                      576 LOAD_CONST              16 ('state')
                      578 STORE_SUBSCR
          
-         624         582 LOAD_FAST                4 (df)
+         605         582 LOAD_FAST                4 (df)
                      584 LOAD_METHOD             10 (apply)
                      606 LOAD_FAST                9 (get_city)
                      608 LOAD_CONST              14 (1)
                      610 KW_NAMES                15
                      612 PRECALL                  2
                      616 CALL                     2
                      626 LOAD_FAST                4 (df)
                      628 LOAD_CONST              17 ('city')
                      630 STORE_SUBSCR
          
-         626         634 LOAD_FAST                4 (df)
+         607         634 LOAD_FAST                4 (df)
                      636 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
-            "\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        c.description,\n        c.source,\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        \n        \n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n    ;\n    "
+            "\n    WITH RankedEvents AS (\n        SELECT *,\n            ROW_NUMBER() OVER(PARTITION BY search_uid, domain ORDER BY created DESC) AS rn\n        FROM event\n        WHERE \n            domain is not null\n            AND search_uid = :search_uid\n            AND type NOT IN ('comment','rating','criteria','update','review','mute')\n    )\n    SELECT \n        e.search_uid, \n        e.domain, \n        e.type as stage, \n        e.created as updated, \n        to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,\n        a.name as updated_by, \n        c.name, \n        c.description as grata_description,\n        c.meta->>'description' as description,\n        c.source,\n        -- uh is this necessary?\n        c.meta->>'ownership' as ownership, \n        c.meta->>'headquarters' as headquarters,\n        c.meta->>'city' as city,\n        c.meta->>'state' as state,\n        c.meta->>'designation' as designation,\n        c.meta->>'products' as products,\n        c.meta->>'services' as services,\n        c.meta->>'end_customer' as end_customer,\n        c.meta->>'geographies' as geographies,\n        c.meta->>'was_acquired' as was_acquired,\n        c.meta->>'justification' as justification,\n        c.meta->>'year_founded' as year_founded,\n        c.meta->>'linkedin' as linkedin,\n        c.meta->>'linkedin_range' as linkedin_range,\n        c.meta->>'primary_contact' as primary_contact,\n        c.meta->>'industry' as industry,\n        c.meta->>'revenue_estimates' as revenue_estimates,\n        c.meta->>'location_count' as location_count,\n        c.meta->>'business_models' as business_models,\n        c.meta->>'facility_size' as facility_size,\n        c.meta->>'contact_name' as contact_name,\n        c.meta->>'contact_title' as contact_title,\n        c.meta->>'contact_email' as contact_email,\n        c.meta->>'contact_phone' as contact_phone,\n        c.meta->>'contact_address' as contact_address,\n        c.meta->>'gpt' as gpt,\n        c.meta,\n        r.rating::int, \n        COALESCE(co.comments, '[]'::jsonb) as comments\n    FROM RankedEvents e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    LEFT JOIN company c ON e.domain = c.domain\n    LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain\n    LEFT JOIN rating r ON e.search_uid = r.search_uid AND e.domain = r.domain\n    \n    WHERE \n        e.rn = 1\n    ;\n    "
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
-               569           0 RESUME                   0
+               550           0 RESUME                   0
                
-               571           2 NOP
+               552           2 NOP
                
-               572           4 LOAD_GLOBAL              1 (NULL + json)
+               553           4 LOAD_GLOBAL              1 (NULL + json)
                             16 LOAD_ATTR                1 (loads)
                             26 LOAD_FAST                0 (list_str)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               1 (list_data)
                
-               575          44 LOAD_CONST               1 (', ')
+               556          44 LOAD_CONST               1 (', ')
                             46 LOAD_METHOD              2 (join)
                             68 LOAD_FAST                1 (list_data)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 STORE_FAST               2 (csv_str)
                
-               577          86 LOAD_FAST                2 (csv_str)
+               558          86 LOAD_FAST                2 (csv_str)
                             88 RETURN_VALUE
                        >>   90 PUSH_EXC_INFO
                
-               578          92 POP_TOP
+               559          92 POP_TOP
                
-               579          94 POP_EXCEPT
+               560          94 POP_EXCEPT
                             96 LOAD_CONST               2 ('')
                             98 RETURN_VALUE
                        >>  100 COPY                     3
                            102 POP_EXCEPT
                            104 RERAISE                  1
                ExceptionTable:
                  4 to 86 -> 90 [0]
@@ -2805,75 +2808,75 @@
                   ''
                names      ('json', 'loads', 'join')
                varnames   ('list_str', 'list_data', 'csv_str')
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'list_to_csv'
-               firstlineno 569
+               firstlineno 550
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
-               581           0 RESUME                   0
+               562           0 RESUME                   0
                
-               582           2 LOAD_FAST                0 (meta)
+               563           2 LOAD_FAST                0 (meta)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('employees')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE    30 (to 104)
                
-               584          44 NOP
+               565          44 NOP
                
-               585          46 LOAD_GLOBAL              3 (NULL + int)
+               566          46 LOAD_GLOBAL              3 (NULL + int)
                             58 LOAD_FAST                0 (meta)
                             60 LOAD_CONST               1 ('employees')
                             62 BINARY_SUBSCR
                             72 PRECALL                  1
                             76 CALL                     1
                             86 RETURN_VALUE
                        >>   88 PUSH_EXC_INFO
                
-               586          90 POP_TOP
+               567          90 POP_TOP
                
-               587          92 POP_EXCEPT
+               568          92 POP_EXCEPT
                             94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                        >>   98 COPY                     3
                            100 POP_EXCEPT
                            102 RERAISE                  1
                
-               588     >>  104 LOAD_FAST                0 (meta)
+               569     >>  104 LOAD_FAST                0 (meta)
                            106 LOAD_METHOD              0 (get)
                            128 LOAD_CONST               2 ('grata_employee_estimates')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 POP_JUMP_FORWARD_IF_FALSE    27 (to 200)
                
-               589         146 LOAD_FAST                0 (meta)
+               570         146 LOAD_FAST                0 (meta)
                            148 LOAD_CONST               2 ('grata_employee_estimates')
                            150 BINARY_SUBSCR
                            160 LOAD_METHOD              0 (get)
                            182 LOAD_CONST               3 ('count')
                            184 PRECALL                  1
                            188 CALL                     1
                            198 RETURN_VALUE
                
-               591     >>  200 LOAD_CONST               0 (None)
+               572     >>  200 LOAD_CONST               0 (None)
                            202 RETURN_VALUE
                ExceptionTable:
                  46 to 84 -> 88 [0]
                  88 to 90 -> 98 [1] lasti
                consts
                   None
                   'employees'
@@ -2881,57 +2884,57 @@
                   'count'
                names      ('get', 'int')
                varnames   ('meta',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'get_employees'
-               firstlineno 581
+               firstlineno 562
                lnotab 0x02012a0202012c0102010c012a013602
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 19
                code
                   0x97007c0064016b02000000007202640253007c0064036b020000000072
                   02640453007c005300
-               593           0 RESUME                   0
+               574           0 RESUME                   0
                
-               594           2 LOAD_FAST                0 (ownership)
+               575           2 LOAD_FAST                0 (ownership)
                              4 LOAD_CONST               1 ('Bootstrapped')
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE     2 (to 18)
                
-               595          14 LOAD_CONST               2 ('Private')
+               576          14 LOAD_CONST               2 ('Private')
                             16 RETURN_VALUE
                
-               596     >>   18 LOAD_FAST                0 (ownership)
+               577     >>   18 LOAD_FAST                0 (ownership)
                             20 LOAD_CONST               3 ('Investor Backed')
                             22 COMPARE_OP               2 (==)
                             28 POP_JUMP_FORWARD_IF_FALSE     2 (to 34)
                
-               597          30 LOAD_CONST               4 ('Venture Capital')
+               578          30 LOAD_CONST               4 ('Venture Capital')
                             32 RETURN_VALUE
                
-               599     >>   34 LOAD_FAST                0 (ownership)
+               580     >>   34 LOAD_FAST                0 (ownership)
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
-               firstlineno 593
+               firstlineno 574
                lnotab 0x02010c0104010c010402
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 19
                code
@@ -2941,78 +2944,78 @@
                   00ab010000000000000000725a7c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017406000000
                   000000000000006a0400000000000000006a050000000000000000a00000
                   000000000000000000000000000000000000007c016405a6020000ab0200
                   000000000000007d027c02530064005300
-               601           0 RESUME                   0
+               582           0 RESUME                   0
                
-               602           2 LOAD_FAST                0 (row)
+               583           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('state')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               603          44 LOAD_FAST                0 (row)
+               584          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('state')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               604     >>   60 LOAD_FAST                0 (row)
+               585     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    90 (to 282)
                
-               605         102 LOAD_FAST                0 (row)
+               586         102 LOAD_FAST                0 (row)
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
                
-               606         204 LOAD_GLOBAL              6 (ts)
+               587         204 LOAD_GLOBAL              6 (ts)
                            216 LOAD_ATTR                4 (constants)
                            226 LOAD_ATTR                5 (STATE_NAMES)
                            236 LOAD_METHOD              0 (get)
                            258 LOAD_FAST                1 (state_name)
                            260 LOAD_CONST               5 ('')
                            262 PRECALL                  2
                            266 CALL                     2
                            276 STORE_FAST               2 (state_code)
                
-               607         278 LOAD_FAST                2 (state_code)
+               588         278 LOAD_FAST                2 (state_code)
                            280 RETURN_VALUE
                
-               609     >>  282 LOAD_CONST               0 (None)
+               590     >>  282 LOAD_CONST               0 (None)
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
-               firstlineno 601
+               firstlineno 582
                lnotab 0x02012a0110012a0166014a010402
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 19
                code
@@ -3020,67 +3023,67 @@
                   010000ab01000000000000000072087c0064011900000000000000000053
                   007c00a00000000000000000000000000000000000000000006402a60100
                   00ab01000000000000000072357c00640219000000000000000000a00100
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000640419000000000000000000a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d017c01530064
                   005300
-               611           0 RESUME                   0
+               592           0 RESUME                   0
                
-               612           2 LOAD_FAST                0 (row)
+               593           2 LOAD_FAST                0 (row)
                              4 LOAD_METHOD              0 (get)
                             26 LOAD_CONST               1 ('city')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_FALSE     8 (to 60)
                
-               613          44 LOAD_FAST                0 (row)
+               594          44 LOAD_FAST                0 (row)
                             46 LOAD_CONST               1 ('city')
                             48 BINARY_SUBSCR
                             58 RETURN_VALUE
                
-               614     >>   60 LOAD_FAST                0 (row)
+               595     >>   60 LOAD_FAST                0 (row)
                             62 LOAD_METHOD              0 (get)
                             84 LOAD_CONST               2 ('headquarters')
                             86 PRECALL                  1
                             90 CALL                     1
                            100 POP_JUMP_FORWARD_IF_FALSE    53 (to 208)
                
-               615         102 LOAD_FAST                0 (row)
+               596         102 LOAD_FAST                0 (row)
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
                
-               616         204 LOAD_FAST                1 (city_name)
+               597         204 LOAD_FAST                1 (city_name)
                            206 RETURN_VALUE
                
-               618     >>  208 LOAD_CONST               0 (None)
+               599     >>  208 LOAD_CONST               0 (None)
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
-               firstlineno 611
+               firstlineno 592
                lnotab 0x02012a0110012a0166010402
             'end_customer'
             'meta'
             'employees'
             'ownership'
             1
             ('axis',)
@@ -3088,77 +3091,176 @@
             'city'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'str', 'apply')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df', 'list_to_csv', 'get_employees', 'get_ownership', 'get_state', 'get_city')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_targets'
-         firstlineno 498
+         firstlineno 478
          lnotab
-            0x0203043d34011801260106fe100474fb2e07160c060c0608060a06093c
+            0x0203043e34011801260106fe100474fb2e07160c060c0608060a06093c
             013c013c0134013402
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
+            0x970064017d01740000000000000000000000a001000000000000000000
+            0000000000000000000000a6000000ab00000000000000000035007d027c
+            02a002000000000000000000000000000000000000000074070000000000
+            00000000006a0400000000000000007c01a6010000ab0100000000000000
+            0064027c006901a6020000ab0200000000000000007d03740b0000000000
+            00000000006a0600000000000000007c03a0070000000000000000000000
+            000000000000000000a6000000ab0000000000000000007c03a008000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
+            02000000000000000001006e0b2300310073047702780359007701010059
+            00010001007c045300
+         610           0 RESUME                   0
+         
+         611           2 LOAD_CONST               1 ("\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    ")
+                       4 STORE_FAST               1 (statement)
+         
+         623           6 LOAD_GLOBAL              0 (db)
+                      18 LOAD_METHOD              1 (connect)
+                      40 PRECALL                  0
+                      44 CALL                     0
+                      54 BEFORE_WITH
+                      56 STORE_FAST               2 (conn)
+         
+         624          58 LOAD_FAST                2 (conn)
+                      60 LOAD_METHOD              2 (execute)
+         
+         625          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+                      94 LOAD_ATTR                4 (text)
+                     104 LOAD_FAST                1 (statement)
+                     106 PRECALL                  1
+                     110 CALL                     1
+         
+         626         120 LOAD_CONST               2 ('search_uid')
+                     122 LOAD_FAST                0 (search_uid)
+                     124 BUILD_MAP                1
+         
+         624         126 PRECALL                  2
+                     130 CALL                     2
+                     140 STORE_FAST               3 (result)
+         
+         628         142 LOAD_GLOBAL             11 (NULL + pd)
+                     154 LOAD_ATTR                6 (DataFrame)
+                     164 LOAD_FAST                3 (result)
+                     166 LOAD_METHOD              7 (fetchall)
+                     188 PRECALL                  0
+                     192 CALL                     0
+                     202 LOAD_FAST                3 (result)
+                     204 LOAD_METHOD              8 (keys)
+                     226 PRECALL                  0
+                     230 CALL                     0
+                     240 KW_NAMES                 3
+                     242 PRECALL                  2
+                     246 CALL                     2
+                     256 STORE_FAST               4 (df)
+         
+         623         258 LOAD_CONST               0 (None)
+                     260 LOAD_CONST               0 (None)
+                     262 LOAD_CONST               0 (None)
+                     264 PRECALL                  2
+                     268 CALL                     2
+                     278 POP_TOP
+                     280 JUMP_FORWARD            11 (to 304)
+                 >>  282 PUSH_EXC_INFO
+                     284 WITH_EXCEPT_START
+                     286 POP_JUMP_FORWARD_IF_TRUE     4 (to 296)
+                     288 RERAISE                  2
+                 >>  290 COPY                     3
+                     292 POP_EXCEPT
+                     294 RERAISE                  1
+                 >>  296 POP_TOP
+                     298 POP_EXCEPT
+                     300 POP_TOP
+                     302 POP_TOP
+         
+         629     >>  304 LOAD_FAST                4 (df)
+                     306 RETURN_VALUE
+         ExceptionTable:
+           56 to 256 -> 282 [1] lasti
+           282 to 288 -> 290 [3] lasti
+           296 to 296 -> 290 [3] lasti
+         consts
+            None
+            "\n    SELECT \n        e.*,\n        a.name as author\n    FROM event e\n    LEFT JOIN actor a ON e.actor_key = a.key\n    WHERE\n        e.type = 'comment'\n        AND e.domain is null\n        AND search_uid = :search_uid\n    "
+            'search_uid'
+            ('columns',)
+         names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
+         varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
+         name       'search_comments'
+         firstlineno 610
+         lnotab 0x0201040c34011801260106fe100474fb2e06
+      code
+         argcount  : 1
+         nlocals   : 5
+         stacksize : 6
+         flags     : 3
+         code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000035007d0164017d027c
             01a002000000000000000000000000000000000000000074070000000000
             00000000006a0400000000000000007c02a6010000ab0100000000000000
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         629           0 RESUME                   0
+         632           0 RESUME                   0
          
-         630           2 LOAD_GLOBAL              0 (db)
+         633           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         631          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         634          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         636          58 LOAD_FAST                1 (conn)
+         639          58 LOAD_FAST                1 (conn)
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
          
-         637         142 LOAD_GLOBAL             11 (NULL + pd)
+         640         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         630         258 LOAD_CONST               0 (None)
+         633         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3169,15 +3271,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         638     >>  304 LOAD_FAST                4 (df)
+         641     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            52 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3186,15 +3288,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 629
+         firstlineno 632
          lnotab 0x020134010405540174f92e08
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3206,65 +3308,65 @@
             007c01a6010000ab01000000000000000064027c006901a6020000ab0200
             000000000000007d03740f000000000000000000006a0800000000000000
             007c03a0090000000000000000000000000000000000000000a6000000ab
             0000000000000000007c03a00a0000000000000000000000000000000000
             000000a6000000ab000000000000000000ac03a6020000ab020000000000
             0000007d04640064006400a6020000ab02000000000000000001006e0b23
             0031007304770278035900770101005900010001007c045300
-         641           0 RESUME                   0
+         644           0 RESUME                   0
          
-         642           2 LOAD_GLOBAL              1 (NULL + isinstance)
+         645           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (search_uid)
                       16 LOAD_GLOBAL              2 (int)
                       28 PRECALL                  2
                       32 CALL                     2
                       42 POP_JUMP_FORWARD_IF_TRUE     2 (to 48)
                       44 LOAD_ASSERTION_ERROR
                       46 RAISE_VARARGS            1
          
-         643     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
+         646     >>   48 LOAD_CONST               1 ("\n    SELECT \n        e.id,\n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.domain,\n        e.data,\n        a.type as actor_type,\n        a.key as actor_key,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type != 'mute'\n    ORDER BY created DESC\n    ;\n\n    ")
                       50 STORE_FAST               1 (statement)
          
-         665          52 LOAD_GLOBAL              4 (db)
+         668          52 LOAD_GLOBAL              4 (db)
                       64 LOAD_METHOD              3 (connect)
                       86 PRECALL                  0
                       90 CALL                     0
                      100 BEFORE_WITH
                      102 STORE_FAST               2 (conn)
          
-         666         104 LOAD_FAST                2 (conn)
+         669         104 LOAD_FAST                2 (conn)
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
          
-         667         188 LOAD_GLOBAL             15 (NULL + pd)
+         670         188 LOAD_GLOBAL             15 (NULL + pd)
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
          
-         665         304 LOAD_CONST               0 (None)
+         668         304 LOAD_CONST               0 (None)
                      306 LOAD_CONST               0 (None)
                      308 LOAD_CONST               0 (None)
                      310 PRECALL                  2
                      314 CALL                     2
                      324 POP_TOP
                      326 JUMP_FORWARD            11 (to 350)
                  >>  328 PUSH_EXC_INFO
@@ -3275,15 +3377,15 @@
                      338 POP_EXCEPT
                      340 RERAISE                  1
                  >>  342 POP_TOP
                      344 POP_EXCEPT
                      346 POP_TOP
                      348 POP_TOP
          
-         668     >>  350 LOAD_FAST                4 (df)
+         671     >>  350 LOAD_FAST                4 (df)
                      352 RETURN_VALUE
          ExceptionTable:
            102 to 302 -> 328 [1] lasti
            328 to 334 -> 336 [3] lasti
            342 to 342 -> 336 [3] lasti
          consts
             None
@@ -3292,15 +3394,15 @@
             ('columns',)
          names      ('isinstance', 'int', 'db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event_history'
-         firstlineno 641
+         firstlineno 644
          lnotab 0x02012e0104163401540174fe2e03
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -3311,56 +3413,56 @@
             0064027c006901a6020000ab0200000000000000007d03740b0000000000
             00000000006a0600000000000000007c03a0070000000000000000000000
             000000000000000000a6000000ab0000000000000000007c03a008000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             00ac03a6020000ab0200000000000000007d04640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c045300
-         671           0 RESUME                   0
+         674           0 RESUME                   0
          
-         673           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
+         676           2 LOAD_CONST               1 ("\n    SELECT \n        e.type as event_type,\n        s.label as search_label,\n        e.search_uid,\n        e.data,\n        -- a.type as actor_type,\n        a.name,\n        to_timestamp(e.created) as created \n    FROM event e\n    JOIN actor a on e.actor_key = a.key\n    JOIN search s on e.search_uid = s.uid\n    WHERE \n        e.search_uid = :search_uid\n        AND e.type in ('import', 'criteria','google','google_maps')\n    ORDER BY created DESC\n    ;\n    ")
                        4 STORE_FAST               1 (statement)
          
-         691           6 LOAD_GLOBAL              0 (db)
+         694           6 LOAD_GLOBAL              0 (db)
                       18 LOAD_METHOD              1 (connect)
                       40 PRECALL                  0
                       44 CALL                     0
                       54 BEFORE_WITH
                       56 STORE_FAST               2 (conn)
          
-         692          58 LOAD_FAST                2 (conn)
+         695          58 LOAD_FAST                2 (conn)
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
          
-         693         142 LOAD_GLOBAL             11 (NULL + pd)
+         696         142 LOAD_GLOBAL             11 (NULL + pd)
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
          
-         691         258 LOAD_CONST               0 (None)
+         694         258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 PRECALL                  2
                      268 CALL                     2
                      278 POP_TOP
                      280 JUMP_FORWARD            11 (to 304)
                  >>  282 PUSH_EXC_INFO
@@ -3371,15 +3473,15 @@
                      292 POP_EXCEPT
                      294 RERAISE                  1
                  >>  296 POP_TOP
                      298 POP_EXCEPT
                      300 POP_TOP
                      302 POP_TOP
          
-         694     >>  304 LOAD_FAST                4 (df)
+         697     >>  304 LOAD_FAST                4 (df)
                      306 RETURN_VALUE
          ExceptionTable:
            56 to 256 -> 282 [1] lasti
            282 to 288 -> 290 [3] lasti
            296 to 296 -> 290 [3] lasti
          consts
             None
@@ -3388,15 +3490,15 @@
             ('columns',)
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'statement', 'conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search_criteria_history'
-         firstlineno 671
+         firstlineno 674
          lnotab 0x020204123401540174fe2e03
       'uid'
       code
          argcount  : 1
          nlocals   : 7
          stacksize : 7
          flags     : 3
@@ -3414,96 +3516,96 @@
             000000000000007d05741300000000000000000000741400000000000000
             0000006a0b00000000000000006a0c00000000000000007c05a6020000ab
             0200000000000000007d067c066a0d0000000000000000a00e0000000000
             0000000000000000000000000000006403a6010000ab0100000000000000
             006404190000000000000000007c066a0f000000000000000064053c0000
             00640064006400a6020000ab02000000000000000001006e0b2300310073
             04770278035900770101005900010001007c065300
-         700           0 RESUME                   0
+         703           0 RESUME                   0
          
-         701           2 LOAD_GLOBAL              0 (db)
+         704           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         702          54 LOAD_CONST               1 ("\n            SELECT \n                uid, \n                label, \n                meta, \n                fields, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            ")
+         705          54 LOAD_CONST               1 ("\n            SELECT \n                uid, \n                label, \n                meta, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            ")
                       56 STORE_FAST               2 (statement)
          
-         716          58 LOAD_FAST                1 (conn)
+         718          58 LOAD_FAST                1 (conn)
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
          
-         718         142 LOAD_FAST                3 (result)
+         720         142 LOAD_FAST                3 (result)
                      144 LOAD_METHOD              5 (fetchone)
                      166 PRECALL                  0
                      170 CALL                     0
                      180 STORE_FAST               4 (row)
          
-         719         182 LOAD_FAST                4 (row)
+         721         182 LOAD_FAST                4 (row)
                      184 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 214)
          
-         720         186 NOP
+         722         186 NOP
          
-         701         188 LOAD_CONST               0 (None)
+         704         188 LOAD_CONST               0 (None)
                      190 LOAD_CONST               0 (None)
                      192 LOAD_CONST               0 (None)
                      194 PRECALL                  2
                      198 CALL                     2
                      208 POP_TOP
                      210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         722     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         724     >>  214 LOAD_GLOBAL             13 (NULL + dict)
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
          
-         723         308 LOAD_GLOBAL             19 (NULL + from_dict)
+         725         308 LOAD_GLOBAL             19 (NULL + from_dict)
                      320 LOAD_GLOBAL             20 (ts)
                      332 LOAD_ATTR               11 (models)
                      342 LOAD_ATTR               12 (Search)
                      352 LOAD_FAST                5 (obj)
                      354 PRECALL                  2
                      358 CALL                     2
                      368 STORE_FAST               6 (search)
          
-         724         370 LOAD_FAST                6 (search)
+         726         370 LOAD_FAST                6 (search)
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
          
-         701         450 LOAD_CONST               0 (None)
+         704         450 LOAD_CONST               0 (None)
                      452 LOAD_CONST               0 (None)
                      454 LOAD_CONST               0 (None)
                      456 PRECALL                  2
                      460 CALL                     2
                      470 POP_TOP
                      472 JUMP_FORWARD            11 (to 496)
                  >>  474 PUSH_EXC_INFO
@@ -3514,72 +3616,72 @@
                      484 POP_EXCEPT
                      486 RERAISE                  1
                  >>  488 POP_TOP
                      490 POP_EXCEPT
                      492 POP_TOP
                      494 POP_TOP
          
-         726     >>  496 LOAD_FAST                6 (search)
+         728     >>  496 LOAD_FAST                6 (search)
                      498 RETURN_VALUE
          ExceptionTable:
            52 to 186 -> 474 [1] lasti
            214 to 448 -> 474 [1] lasti
            474 to 480 -> 482 [3] lasti
            488 to 488 -> 482 [3] lasti
          consts
             None
-            "\n            SELECT \n                uid, \n                label, \n                meta, \n                fields, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            "
+            "\n            SELECT \n                uid, \n                label, \n                meta, \n                meta->>'next_due_date' as next_due_date,\n                meta->>'notes' as notes,\n                COALESCE(criteria.data, '{}'::jsonb) as criteria\n            FROM search\n            LEFT JOIN criteria ON search.uid = criteria.search_uid\n            \n            WHERE uid = :uid\n            "
             'uid'
             ' - '
             0
             'client'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'fetchone', 'dict', 'zip', 'keys', 'from_dict', 'ts', 'models', 'Search', 'label', 'split', 'meta')
          varnames   ('uid', 'conn', 'statement', 'result', 'row', 'obj', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search'
-         firstlineno 700
-         lnotab 0x02013401040e54022801040102ed1a155e013e0150e92e19
+         firstlineno 703
+         lnotab 0x02013401040d54022801040102ee1a145e013e0150ea2e18
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
-         729           0 RESUME                   0
+         731           0 RESUME                   0
          
-         730           2 LOAD_GLOBAL              1 (NULL + searches_query)
+         732           2 LOAD_GLOBAL              1 (NULL + searches_query)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (searches)
          
-         731          30 LOAD_FAST                1 (searches)
+         733          30 LOAD_FAST                1 (searches)
                       32 LOAD_FAST                1 (searches)
                       34 LOAD_CONST               1 ('searchToken')
                       36 BINARY_SUBSCR
                       46 LOAD_FAST                0 (searchToken)
                       48 COMPARE_OP               2 (==)
                       54 BINARY_SUBSCR
                       64 STORE_FAST               2 (search)
          
-         732          66 LOAD_FAST                2 (search)
+         734          66 LOAD_FAST                2 (search)
                       68 LOAD_ATTR                1 (empty)
                       78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
          
-         733          80 LOAD_CONST               0 (None)
+         735          80 LOAD_CONST               0 (None)
                       82 RETURN_VALUE
          
-         735     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
+         737     >>   84 LOAD_GLOBAL              5 (NULL + find_search)
                       96 LOAD_FAST                2 (search)
                       98 LOAD_ATTR                3 (iloc)
                      108 LOAD_CONST               2 (0)
                      110 BINARY_SUBSCR
                      120 LOAD_CONST               3 ('uid')
                      122 BINARY_SUBSCR
                      132 PRECALL                  1
@@ -3592,15 +3694,15 @@
             'uid'
          names      ('searches_query', 'empty', 'find_search', 'iloc')
          varnames   ('searchToken', 'searches', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_token'
-         firstlineno 729
+         firstlineno 731
          lnotab 0x02011c0124010e010402
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3614,41 +3716,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         738           0 RESUME                   0
+         740           0 RESUME                   0
          
-         739           2 LOAD_GLOBAL              0 (db)
+         741           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         740          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         742          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         745          58 LOAD_FAST                1 (conn)
+         747          58 LOAD_FAST                1 (conn)
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
          
-         739         142 LOAD_CONST               0 (None)
+         741         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3659,24 +3761,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         747     >>  188 LOAD_FAST                3 (result)
+         749     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         748         210 LOAD_CONST               0 (None)
+         750         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         750     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         752     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3684,15 +3786,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         751         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         753         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Company)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3705,15 +3807,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 738
+         firstlineno 740
          lnotab 0x02013401040554fa2e08160104028201
       'email'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3728,41 +3830,41 @@
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000006a0c00000000000000006a0d00000000000000007c
             04a6020000ab0200000000000000005300
-         754           0 RESUME                   0
+         756           0 RESUME                   0
          
-         755           2 LOAD_GLOBAL              0 (db)
+         757           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         756          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
+         758          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM actor\n                WHERE email = :email\n            ')
                       56 STORE_FAST               2 (statement)
          
-         761          58 LOAD_FAST                1 (conn)
+         763          58 LOAD_FAST                1 (conn)
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
          
-         755         142 LOAD_CONST               0 (None)
+         757         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3773,24 +3875,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         763     >>  188 LOAD_FAST                3 (result)
+         765     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         764         210 LOAD_CONST               0 (None)
+         766         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         766     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         768     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3798,15 +3900,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         767         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         769         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (ts)
                      368 LOAD_ATTR               12 (models)
                      378 LOAD_ATTR               13 (Actor)
                      388 LOAD_FAST                4 (obj)
                      390 PRECALL                  2
                      394 CALL                     2
                      404 RETURN_VALUE
@@ -3821,15 +3923,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'ts', 'models', 'Actor')
          varnames   ('email', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_actor_by_email'
-         firstlineno 754
+         firstlineno 756
          lnotab 0x02013401040554fa2e08160104028201
       'event_id'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -3843,41 +3945,41 @@
             0101005900010001007c036a05000000000000000064036b020000000072
             0264005300740d00000000000000000000740f000000000000000000007c
             03a0080000000000000000000000000000000000000000a6000000ab0000
             000000000000007c03a00900000000000000000000000000000000000000
             00a6000000ab000000000000000000a6020000ab020000000000000000a6
             010000ab0100000000000000007d04741500000000000000000000741600
             0000000000000000007c04a6020000ab0200000000000000005300
-         770           0 RESUME                   0
+         772           0 RESUME                   0
          
-         771           2 LOAD_GLOBAL              0 (db)
+         773           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         772          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
+         774          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE id = :event_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         777          58 LOAD_FAST                1 (conn)
+         779          58 LOAD_FAST                1 (conn)
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
          
-         771         142 LOAD_CONST               0 (None)
+         773         142 LOAD_CONST               0 (None)
                      144 LOAD_CONST               0 (None)
                      146 LOAD_CONST               0 (None)
                      148 PRECALL                  2
                      152 CALL                     2
                      162 POP_TOP
                      164 JUMP_FORWARD            11 (to 188)
                  >>  166 PUSH_EXC_INFO
@@ -3888,24 +3990,24 @@
                      176 POP_EXCEPT
                      178 RERAISE                  1
                  >>  180 POP_TOP
                      182 POP_EXCEPT
                      184 POP_TOP
                      186 POP_TOP
          
-         779     >>  188 LOAD_FAST                3 (result)
+         781     >>  188 LOAD_FAST                3 (result)
                      190 LOAD_ATTR                5 (rowcount)
                      200 LOAD_CONST               3 (0)
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE     2 (to 214)
          
-         780         210 LOAD_CONST               0 (None)
+         782         210 LOAD_CONST               0 (None)
                      212 RETURN_VALUE
          
-         782     >>  214 LOAD_GLOBAL             13 (NULL + dict)
+         784     >>  214 LOAD_GLOBAL             13 (NULL + dict)
                      226 LOAD_GLOBAL             15 (NULL + zip)
                      238 LOAD_FAST                3 (result)
                      240 LOAD_METHOD              8 (keys)
                      262 PRECALL                  0
                      266 CALL                     0
                      276 LOAD_FAST                3 (result)
                      278 LOAD_METHOD              9 (fetchone)
@@ -3913,15 +4015,15 @@
                      304 CALL                     0
                      314 PRECALL                  2
                      318 CALL                     2
                      328 PRECALL                  1
                      332 CALL                     1
                      342 STORE_FAST               4 (obj)
          
-         783         344 LOAD_GLOBAL             21 (NULL + from_dict)
+         785         344 LOAD_GLOBAL             21 (NULL + from_dict)
                      356 LOAD_GLOBAL             22 (Event)
                      368 LOAD_FAST                4 (obj)
                      370 PRECALL                  2
                      374 CALL                     2
                      384 RETURN_VALUE
          ExceptionTable:
            52 to 140 -> 166 [1] lasti
@@ -3934,15 +4036,15 @@
             0
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Event')
          varnames   ('event_id', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_event_by_id'
-         firstlineno 770
+         firstlineno 772
          lnotab 0x02013401040554fa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 12
          flags     : 3
          code
@@ -3954,71 +4056,71 @@
             000000000000007c006a0800000000000000007c006a0900000000000000
             007415000000000000000000006a0b00000000000000007c006a0c000000
             0000000000a6010000ab01000000000000000064029c06a6020000ab0200
             0000000000000001007c01a00d0000000000000000000000000000000000
             000000a6000000ab0000000000000000000100640064006400a6020000ab
             020000000000000000010064005300230031007304770278035900770101
             0059000100010064005300
-         789           0 RESUME                   0
+         791           0 RESUME                   0
          
-         790           2 LOAD_GLOBAL              0 (db)
+         792           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         791          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
+         793          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                uid = :uid,\n                name = :name,\n                description = :description,\n                source = :source,\n                meta = :meta,\n                updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         803          58 LOAD_FAST                1 (conn)
+         805          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         804          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         806          82 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       94 LOAD_ATTR                4 (text)
                      104 LOAD_FAST                2 (statement)
                      106 PRECALL                  1
                      110 CALL                     1
          
-         806         120 LOAD_FAST                0 (company)
+         808         120 LOAD_FAST                0 (company)
                      122 LOAD_ATTR                5 (uid)
          
-         807         132 LOAD_FAST                0 (company)
+         809         132 LOAD_FAST                0 (company)
                      134 LOAD_ATTR                6 (name)
          
-         808         144 LOAD_FAST                0 (company)
+         810         144 LOAD_FAST                0 (company)
                      146 LOAD_ATTR                7 (description)
          
-         809         156 LOAD_FAST                0 (company)
+         811         156 LOAD_FAST                0 (company)
                      158 LOAD_ATTR                8 (domain)
          
-         810         168 LOAD_FAST                0 (company)
+         812         168 LOAD_FAST                0 (company)
                      170 LOAD_ATTR                9 (source)
          
-         811         180 LOAD_GLOBAL             21 (NULL + json)
+         813         180 LOAD_GLOBAL             21 (NULL + json)
                      192 LOAD_ATTR               11 (dumps)
                      202 LOAD_FAST                0 (company)
                      204 LOAD_ATTR               12 (meta)
                      214 PRECALL                  1
                      218 CALL                     1
          
-         805         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
+         807         228 LOAD_CONST               2 (('uid', 'name', 'description', 'domain', 'source', 'meta'))
                      230 BUILD_CONST_KEY_MAP      6
          
-         803         232 PRECALL                  2
+         805         232 PRECALL                  2
                      236 CALL                     2
                      246 POP_TOP
          
-         815         248 LOAD_FAST                1 (conn)
+         817         248 LOAD_FAST                1 (conn)
                      250 LOAD_METHOD             13 (commit)
                      272 PRECALL                  0
                      276 CALL                     0
                      286 POP_TOP
          
-         790         288 LOAD_CONST               0 (None)
+         792         288 LOAD_CONST               0 (None)
                      290 LOAD_CONST               0 (None)
                      292 LOAD_CONST               0 (None)
                      294 PRECALL                  2
                      298 CALL                     2
                      308 POP_TOP
                      310 LOAD_CONST               0 (None)
                      312 RETURN_VALUE
@@ -4045,15 +4147,15 @@
             ('uid', 'name', 'description', 'domain', 'source', 'meta')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'uid', 'name', 'description', 'domain', 'source', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 789
+         firstlineno 791
          lnotab 0x02013401040c180126020c010c010c010c010c0130fa04fe100c28e7
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
@@ -4063,58 +4165,58 @@
             006a0400000000000000006401a6010000ab010000000000000000740b00
             0000000000000000006a0600000000000000007c006a0700000000000000
             00a6010000ab0100000000000000007c006a08000000000000000064029c
             02a6020000ab02000000000000000001007c01a009000000000000000000
             0000000000000000000000a6000000ab0000000000000000000100640064
             006400a6020000ab02000000000000000001006400530023003100730477
             02780359007701010059000100010064005300
-         818           0 RESUME                   0
+         820           0 RESUME                   0
          
-         819           2 LOAD_GLOBAL              0 (db)
+         821           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         820          54 LOAD_FAST                1 (conn)
+         822          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         821          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         823          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         822         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
+         824         100 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    meta = :meta,\n                    updated = FLOOR(EXTRACT(EPOCH FROM NOW()))\n                WHERE uid = :uid\n                ')
          
-         821         102 PRECALL                  1
+         823         102 PRECALL                  1
                      106 CALL                     1
          
-         831         116 LOAD_GLOBAL             11 (NULL + json)
+         833         116 LOAD_GLOBAL             11 (NULL + json)
                      128 LOAD_ATTR                6 (dumps)
                      138 LOAD_FAST                0 (search)
                      140 LOAD_ATTR                7 (meta)
                      150 PRECALL                  1
                      154 CALL                     1
          
-         832         164 LOAD_FAST                0 (search)
+         834         164 LOAD_FAST                0 (search)
                      166 LOAD_ATTR                8 (uid)
          
-         830         176 LOAD_CONST               2 (('meta', 'uid'))
+         832         176 LOAD_CONST               2 (('meta', 'uid'))
                      178 BUILD_CONST_KEY_MAP      2
          
-         820         180 PRECALL                  2
+         822         180 PRECALL                  2
                      184 CALL                     2
                      194 POP_TOP
          
-         835         196 LOAD_FAST                1 (conn)
+         837         196 LOAD_FAST                1 (conn)
                      198 LOAD_METHOD              9 (commit)
                      220 PRECALL                  0
                      224 CALL                     0
                      234 POP_TOP
          
-         819         236 LOAD_CONST               0 (None)
+         821         236 LOAD_CONST               0 (None)
                      238 LOAD_CONST               0 (None)
                      240 LOAD_CONST               0 (None)
                      242 PRECALL                  2
                      246 CALL                     2
                      256 POP_TOP
                      258 LOAD_CONST               0 (None)
                      260 RETURN_VALUE
@@ -4141,15 +4243,15 @@
             ('meta', 'uid')
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'json', 'dumps', 'meta', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 818
+         firstlineno 820
          lnotab 0x020134011801160102ff0e0a30010cfe04f6100f28f0
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4160,61 +4262,61 @@
             006901a6020000ab02000000000000000001007c01a00200000000000000
             000000000000000000000000007407000000000000000000006a04000000
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00500000000000000000000000000000000000000
             00a6000000ab0000000000000000000100640064006400a6020000ab0200
             000000000000000100640053002300310073047702780359007701010059
             000100010064005300
-         841           0 RESUME                   0
+         843           0 RESUME                   0
          
-         843           2 LOAD_GLOBAL              0 (db)
+         845           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         844          54 LOAD_FAST                1 (conn)
+         846          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         845          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         847          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         846         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
+         848         100 LOAD_CONST               1 ("\n                UPDATE event\n                SET\n                    type = 'mute'\n                WHERE id = :event_id\n                ")
          
-         845         102 PRECALL                  1
+         847         102 PRECALL                  1
                      106 CALL                     1
          
-         854         116 LOAD_CONST               2 ('event_id')
+         856         116 LOAD_CONST               2 ('event_id')
                      118 LOAD_FAST                0 (event_id)
          
-         853         120 BUILD_MAP                1
+         855         120 BUILD_MAP                1
          
-         844         122 PRECALL                  2
+         846         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         857         138 LOAD_FAST                1 (conn)
+         859         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         858         216 LOAD_FAST                1 (conn)
+         860         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              5 (commit)
                      240 PRECALL                  0
                      244 CALL                     0
                      254 POP_TOP
          
-         843         256 LOAD_CONST               0 (None)
+         845         256 LOAD_CONST               0 (None)
                      258 LOAD_CONST               0 (None)
                      260 LOAD_CONST               0 (None)
                      262 PRECALL                  2
                      266 CALL                     2
                      276 POP_TOP
                      278 LOAD_CONST               0 (None)
                      280 RETURN_VALUE
@@ -4242,15 +4344,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('event_id', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'mute_event'
-         firstlineno 841
+         firstlineno 843
          lnotab 0x020234011801160102ff0e0904ff02f7100d4e0128f1
       'comment_id'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
@@ -4262,58 +4364,58 @@
             0064027c006901a6020000ab02000000000000000001007c01a002000000
             00000000000000000000000000000000007407000000000000000000006a
             0400000000000000006403a6010000ab010000000000000000a6010000ab
             01000000000000000001007c01a005000000000000000000000000000000
             0000000000a6000000ab0000000000000000000100640064006400a60200
             00ab02000000000000000001006400530023003100730477027803590077
             01010059000100010064005300
-         864           0 RESUME                   0
+         866           0 RESUME                   0
          
-         865           2 LOAD_GLOBAL              0 (db)
+         867           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         866          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
+         868          54 LOAD_CONST               1 ('\n                DELETE FROM event\n                WHERE id = :comment_id\n            ')
                       56 STORE_FAST               2 (statement)
          
-         870          58 LOAD_FAST                1 (conn)
+         872          58 LOAD_FAST                1 (conn)
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
          
-         871         142 LOAD_FAST                1 (conn)
+         873         142 LOAD_FAST                1 (conn)
                      144 LOAD_METHOD              2 (execute)
                      166 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      178 LOAD_ATTR                4 (text)
                      188 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      190 PRECALL                  1
                      194 CALL                     1
                      204 PRECALL                  1
                      208 CALL                     1
                      218 POP_TOP
          
-         872         220 LOAD_FAST                1 (conn)
+         874         220 LOAD_FAST                1 (conn)
                      222 LOAD_METHOD              5 (commit)
                      244 PRECALL                  0
                      248 CALL                     0
                      258 POP_TOP
          
-         865         260 LOAD_CONST               0 (None)
+         867         260 LOAD_CONST               0 (None)
                      262 LOAD_CONST               0 (None)
                      264 LOAD_CONST               0 (None)
                      266 PRECALL                  2
                      270 CALL                     2
                      280 POP_TOP
                      282 LOAD_CONST               0 (None)
                      284 RETURN_VALUE
@@ -4341,15 +4443,15 @@
             'REFRESH MATERIALIZED VIEW comment'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('comment_id', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'delete_comment'
-         firstlineno 864
+         firstlineno 866
          lnotab 0x02013401040454014e0128f9
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -4362,71 +4464,71 @@
             00000000006403a6010000ab010000000000000000a6010000ab01000000
             000000000001007c01a00200000000000000000000000000000000000000
             007407000000000000000000006a0400000000000000006404a6010000ab
             010000000000000000a6010000ab01000000000000000001007c01a00500
             00000000000000000000000000000000000000a6000000ab000000000000
             0000000100640064006400a6020000ab0200000000000000000100640053
             002300310073047702780359007701010059000100010064005300
-         875           0 RESUME                   0
+         877           0 RESUME                   0
          
-         879           2 LOAD_GLOBAL              0 (db)
+         881           2 LOAD_GLOBAL              0 (db)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         880          54 LOAD_FAST                1 (conn)
+         882          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         881          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+         883          78 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                       90 LOAD_ATTR                4 (text)
          
-         882         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
+         884         100 LOAD_CONST               1 ("\n                DELETE FROM event\n                WHERE search_uid = :search_uid\n                and type = 'create'\n                ")
          
-         881         102 PRECALL                  1
+         883         102 PRECALL                  1
                      106 CALL                     1
          
-         888         116 LOAD_CONST               2 ('search_uid')
+         890         116 LOAD_CONST               2 ('search_uid')
                      118 LOAD_FAST                0 (search_uid)
                      120 BUILD_MAP                1
          
-         880         122 PRECALL                  2
+         882         122 PRECALL                  2
                      126 CALL                     2
                      136 POP_TOP
          
-         890         138 LOAD_FAST                1 (conn)
+         892         138 LOAD_FAST                1 (conn)
                      140 LOAD_METHOD              2 (execute)
                      162 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      174 LOAD_ATTR                4 (text)
                      184 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW comment')
                      186 PRECALL                  1
                      190 CALL                     1
                      200 PRECALL                  1
                      204 CALL                     1
                      214 POP_TOP
          
-         891         216 LOAD_FAST                1 (conn)
+         893         216 LOAD_FAST                1 (conn)
                      218 LOAD_METHOD              2 (execute)
                      240 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      252 LOAD_ATTR                4 (text)
                      262 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW rating')
                      264 PRECALL                  1
                      268 CALL                     1
                      278 PRECALL                  1
                      282 CALL                     1
                      292 POP_TOP
          
-         894         294 LOAD_FAST                1 (conn)
+         896         294 LOAD_FAST                1 (conn)
                      296 LOAD_METHOD              5 (commit)
                      318 PRECALL                  0
                      322 CALL                     0
                      332 POP_TOP
          
-         879         334 LOAD_CONST               0 (None)
+         881         334 LOAD_CONST               0 (None)
                      336 LOAD_CONST               0 (None)
                      338 LOAD_CONST               0 (None)
                      340 PRECALL                  2
                      344 CALL                     2
                      354 POP_TOP
                      356 LOAD_CONST               0 (None)
                      358 RETURN_VALUE
@@ -4455,23 +4557,22 @@
             'REFRESH MATERIALIZED VIEW rating'
          names      ('db', 'connect', 'execute', 'sqlalchemy', 'text', 'commit')
          varnames   ('search_uid', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'reset_inbox'
-         firstlineno 875
+         firstlineno 877
          lnotab 0x020434011801160102ff0e0706f8100a4e014e0328f1
       (False, None)
-      (90,)
-   names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'important_targets_from_event', 'int', 'str', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'recent_validations', 'average_rating_per_search_query', 'validation_history', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'event', 'event_history', 'search_criteria_history', 'find_search', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
+   names      ('hashlib', 'json', 'dataclasses', 'asdict', 'time', 'typing', 'Any', 'List', 'pandas', 'pd', 'sqlalchemy', 'dacite', 'from_dict', 'dotenv', 'load_dotenv', 'gandai', 'ts', 'helpers', 'gandai.db', 'connect_with_connector', 'gandai.models', 'Actor', 'Company', 'Event', 'EventType', 'Search', 'db', 'insert_event', 'models', 'insert_company', 'insert_actor', 'insert_search', 'important_targets_from_event', 'int', 'str', 'bool', 'insert_companies_as_targets', 'DataFrame', 'searches_query', 'average_rating_per_search_query', 'validation_history', 'searches_comment_counts', 'enriched_searches_query', 'actor', 'buyer', 'search_targets', 'search_comments', 'event', 'event_history', 'search_criteria_history', 'find_search', 'find_search_by_token', 'find_company_by_domain', 'find_actor_by_email', 'find_event_by_id', 'update_company', 'update_search', 'mute_event', 'delete_comment', 'reset_inbox')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010c010c011002080108010c010c02140208010c010c
       011c021406101e240e100f1010244c020102fb04010eff020202fe020302
-      fd020402fc020502fb020602fa086016211c2d060c16290617160e163e0c
-      7f00041a0c1a1e1a1d241d2409101010101013101d10171017100b
+      fd020402fc020502fb020602fa08601620060c162b0614061b160e163e0c
+      7f00051a161a0c1a1e1a1d241c2409101010101013101d10171017100b
```

### Comparing `gandai-1.7.41/gandai/__pycache__/secrets.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/__pycache__/tasks.cpython-311.pyc` & `gandai-1.7.42/gandai/__pycache__/tasks.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x70523966 (Mon May  6 21:58:08 2024 UTC)
+moddate:  0xee5c3966 (Mon May  6 22:42:54 2024 UTC)
 files sz: 1079
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `gandai-1.7.41/gandai/analytics.py` & `gandai-1.7.42/gandai/analytics.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/constants.py` & `gandai-1.7.42/gandai/constants.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/db.py` & `gandai-1.7.42/gandai/db.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/google.py` & `gandai-1.7.42/gandai/google.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/grata.py` & `gandai-1.7.42/gandai/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/main.py` & `gandai-1.7.42/gandai/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,16 @@
     c.meta->>'contact_email' as contact_email,
     c.meta->>'contact_phone' as contact_phone,
     c.meta->>'contact_address' as contact_address,
 
     For fields that are lists, you will use a csv string 
     For these lists, such as products or services, try to stick to top 5 or less areas of focus.
 
+    You will fill out the description field with a description of the company.
+    
     If you are unsure, just leave that key out of the response data
 
     """
 
     HEADERS = {
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/14.0 Safari/605.1.15",
         "Accept": "text/html",
@@ -145,15 +147,16 @@
             "content": HOW_TO_ENRICH,
         },
     ]
 
     resp = ts.gpt.ask_gpt4(messages)
     update_event = from_dict(ts.models.Event, resp)
     update_event.search_uid = search_uid
-    ts.query.insert_event(update_event)
+    print(update_event)
+    # ts.query.insert_event(update_event)
 
     return resp
 
 
 def run_similarity_search(search: ts.models.Search, domain: str) -> None:
     grata_companies = ts.grata.find_similar(domain=domain, search=search)
     ts.query.insert_companies_as_targets(
@@ -285,21 +288,21 @@
 def run_enrichment(event: ts.models.Event) -> None:
     domain = event.domain
     search_uid = event.search_uid
 
     company = ts.query.find_company_by_domain(domain)
     if company.meta.get("company_uid"):
         print("company already exists. skipping enrichment...")
-        return None
+    else:
 
-    resp = ts.grata.enrich(company.domain)
-    company.name = company.name or resp.get("name")
-    company.description = resp.get("description")
-    company.meta = {**company.meta, **resp}
-    ts.query.update_company(company)
+        resp = ts.grata.enrich(company.domain)
+        company.name = company.name or resp.get("name")
+        company.description = resp.get("description")
+        company.meta = {**company.meta, **resp}
+        ts.query.update_company(company)
 
     enrich_with_gpt(company=company, search_uid=search_uid)
 
 
 def process_event(event_id: int) -> None:
     print("processing event...")
     event: ts.models.Event = ts.query.find_event_by_id(event_id)
```

### Comparing `gandai-1.7.41/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.7.42/gandai/migrations/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/migrations/db_seed.py` & `gandai-1.7.42/gandai/migrations/db_seed.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/migrations/dealcloud.py` & `gandai-1.7.42/gandai/migrations/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/migrations/sql/230818-alter.sql` & `gandai-1.7.42/gandai/migrations/sql/230818-alter.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/migrations/sql/schema.sql` & `gandai-1.7.42/gandai/migrations/sql/schema.sql`

 * *Files 5% similar despite different names*

```diff
@@ -34,25 +34,25 @@
 
 -- wait this probably alreaady exists
 -- CREATE INDEX idx_actor_key ON actor(key);
 
 
 CREATE TABLE IF NOT EXISTS event (
     id SERIAL PRIMARY KEY,
-    search_uid INTEGER NOT NULL REFERENCES search(uid),
+    search_uid INTEGER REFERENCES search(uid),
     domain VARCHAR(255) REFERENCES company(domain),
     actor_key VARCHAR(255) NOT NULL REFERENCES actor(key),
     type VARCHAR(255) NOT NULL,
     data JSONB DEFAULT '{}'::jsonb,
     created BIGINT NOT NULL DEFAULT FLOOR(EXTRACT(EPOCH FROM NOW()))
 );
 
 CREATE INDEX idx_event_actor_key ON event(actor_key);
 CREATE INDEX idx_event_search_uid ON event(search_uid);
-ALTER TABLE event ADD CONSTRAINT unique_event_type_domain_search_uid_created UNIQUE (type, domain, search_uid, created);
+-- ALTER TABLE event ADD CONSTRAINT unique_event_type_domain_search_uid_created UNIQUE (type, domain, search_uid, created); # 240523-alter.sql
 
 
 -- Pretty sure I am no longer using this? 
 CREATE TABLE IF NOT EXISTS checkpoint (
     id SERIAL PRIMARY KEY,
     event_id INTEGER NOT NULL REFERENCES event(id) ON DELETE CASCADE,
     created BIGINT NOT NULL DEFAULT FLOOR(EXTRACT(EPOCH FROM NOW()))
```

### Comparing `gandai-1.7.41/gandai/models.py` & `gandai-1.7.42/gandai/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     name: Optional[str] = None
     description: Optional[str] = None
     source: Optional[str] = None
     meta: dict = field(default_factory=dict)
     id: int = field(default=None)  # primary key
     uid: Optional[int] = field(default=None)  # foreign key
 
+    # @property
+    # def description(self):
+    #     return self.meta.get("description", None)
+
     @property
     def ownership(self):
         ownership = self.meta.get("ownership", None)
         return self.get_ownership(ownership)
 
     @property
     def was_acquired(self):
@@ -65,17 +69,18 @@
     REJECT = auto()
     CLIENT_REJECT = auto()
     CRITERIA = auto()
 
 
 @dataclass
 class Event:
-    search_uid: int  # fk # add index
+      # fk # add index
     actor_key: str  # fk
     type: str  # enum
+    search_uid: Optional[int] = None
     domain: Optional[str] = None  # fk
     data: dict = field(default_factory=dict)
     id: int = field(default=None)  # pk
     # created: int = field(init=False)
 
 
 @dataclass
```

### Comparing `gandai-1.7.41/gandai/query.py` & `gandai-1.7.42/gandai/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                 new_event_id = result.scalar_one()
                 if new_event_id is not None:
                     new_event_ids.append(new_event_id)
 
                 if stage_dict.get(domain) is not None:
                     comment = ts.models.Event(
                         search_uid=event.search_uid,
-                        actor_key=event.actor_key,
+                        actor_key=event.actor_key,  # todo this should be the system
                         domain=domain,
                         type="comment",
                         data={
                             "comment": f"imported {domain}. Was in stage: {get_stage(domain)}",
                         },
                     )
                     ts.query.insert_event(comment)
@@ -267,86 +267,40 @@
 
 def searches_query() -> pd.DataFrame:
     statement = f"""
     SELECT 
         s.uid,
         s.label,
         s.updated,
-        s.fields,
-        s.meta->>'search_type' as type,
+        s.meta->>'type' as type,
         s.meta->>'notes' as notes,
         s.meta->>'products' as products,
         s.meta->>'services' as services,
         s.meta->>'customers' as customers,
         s.meta->>'end_customer' as end_customer,
         s.meta->>'last_list' as last_list,
         s.meta->>'next_due_date' as next_due_date,
         s.meta->>'geographies' as geographies,
         s.meta->>'week' as week,
         s.meta->>'day' as day,
+
         COALESCE(s.meta->>'search_status', 'active') as search_status
     FROM search s
     ORDER BY updated
     """
     with db.connect() as conn:
         result = conn.execute(sqlalchemy.text(statement))
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
     df["client"] = df["label"].str.split(" - ").str[0]
     df["searchToken"] = df["uid"].apply(
         lambda x: hashlib.md5(str(x).encode("utf-8")).hexdigest()
     )
     return df
 
 
-## chopping block ##
-def recent_validations(trailing_days: int = 90) -> pd.DataFrame:
-    assert isinstance(trailing_days, int)
-    statement = f"""
-    WITH ranked_actors AS (
-        SELECT 
-            a.name as analyst,
-            a.key,
-            s.uid,
-            COUNT(e.id) AS count,
-            MAX(e.created) AS max_created,
-            ROW_NUMBER() OVER (
-                PARTITION BY s.uid
-                ORDER BY COUNT(e.id) DESC
-            ) as rn
-        FROM 
-            event e
-        INNER JOIN 
-            actor a ON a.key = e.actor_key
-        INNER JOIN 
-            search s ON s.uid = e.search_uid
-        WHERE
-            a.type = 'research' 
-            AND e.type = 'validate'
-            AND to_timestamp(e.created) > now() - interval '{trailing_days} day'
-        GROUP BY 
-            a.key, analyst, s.uid
-    )
-    SELECT 
-        key as actor_key,
-        analyst, 
-        uid, 
-        count,
-        max_created
-    FROM 
-        ranked_actors
-    WHERE 
-        rn = 1;
-    """
-    with db.connect() as conn:
-        result = conn.execute(sqlalchemy.text(statement))
-        df = pd.DataFrame(result.fetchall(), columns=result.keys())
-    df["activity"] = round(df["count"] / df["count"].max(), 2)
-    return df
-
-
 def average_rating_per_search_query():
     query = """
        SELECT
         search_uid,
         AVG(rating::int) AS rating_avg,
         COUNT(rating) as rating_count
     FROM rating 
@@ -357,14 +311,15 @@
 
 def validation_history() -> pd.DataFrame:
     stmt = """
     WITH RankedEvents AS (
         SELECT
             e.search_uid,
             a.name as analyst,
+            SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 1 * 86400 THEN 1 ELSE 0 END) AS last_1_days,
             SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 7 * 86400 THEN 1 ELSE 0 END) AS last_7_days,
             SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400 THEN 1 ELSE 0 END) AS last_30_days,
             SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) AS last_90_days,
             SUM(CASE WHEN e.type = 'validate' THEN 1 ELSE 0 END) AS total_validations,
             RANK() OVER (PARTITION BY e.search_uid ORDER BY SUM(CASE WHEN e.created >= EXTRACT(EPOCH FROM NOW()) - 90 * 86400 THEN 1 ELSE 0 END) DESC) as rank
         FROM
             event e
@@ -374,14 +329,15 @@
             e.type = 'validate'
         GROUP BY
             e.search_uid, analyst
     )
     SELECT
         search_uid,
         analyst,
+        last_1_days,
         last_7_days,
         last_30_days,
         last_90_days,
         total_validations
     FROM
         RankedEvents
     WHERE
@@ -392,27 +348,51 @@
     with db.connect() as conn:
         result = conn.execute(sqlalchemy.text(stmt))
         df = pd.DataFrame(result.fetchall(), columns=result.keys())
         df["total_validations_pct"] = round(df["total_validations"] / 300, 2)
     return df
 
 
+def searches_comment_counts():
+    statement = f"""
+        SELECT 
+            e.search_uid as uid,
+            COUNT(*) as comment_count
+        FROM event e
+        WHERE 
+            e.type = 'comment'
+            AND e.domain is null
+            -- last 30 days
+            AND e.created >= EXTRACT(EPOCH FROM NOW()) - 30 * 86400
+        GROUP BY e.search_uid
+        """
+    with db.connect() as conn:
+        result = conn.execute(sqlalchemy.text(statement))
+        df = pd.DataFrame(result.fetchall(), columns=result.keys())
+
+    return df
+
+
 def enriched_searches_query():
     searches = searches_query()
     # recent_event_count = recent_validations()
     recent_event_count = validation_history()
 
     df = searches.merge(
         recent_event_count, left_on="uid", right_on="search_uid", how="left"
     )
 
+    df["last_1_days"] = df["last_1_days"].fillna(0)
     df["last_7_days"] = df["last_7_days"].fillna(0)
     df["last_30_days"] = df["last_30_days"].fillna(0)
     df["last_90_days"] = df["last_90_days"].fillna(0)
 
+    df = df.merge(searches_comment_counts(), on="uid", how="left")
+    df["comment_count"] = df["comment_count"].fillna(0)
+
     # df = df.merge(
     #     average_rating_per_search_query(),
     #     left_on="uid",
     #     right_on="search_uid",
     #     how="left",
     # )
     # df["activity"] = df["activity"].fillna(0)
@@ -512,16 +492,18 @@
         e.search_uid, 
         e.domain, 
         e.type as stage, 
         e.created as updated, 
         to_char(to_timestamp(e.created), 'YYYY-MM-DD') as change_date,
         a.name as updated_by, 
         c.name, 
-        c.description,
+        c.description as grata_description,
+        c.meta->>'description' as description,
         c.source,
+        -- uh is this necessary?
         c.meta->>'ownership' as ownership, 
         c.meta->>'headquarters' as headquarters,
         c.meta->>'city' as city,
         c.meta->>'state' as state,
         c.meta->>'designation' as designation,
         c.meta->>'products' as products,
         c.meta->>'services' as services,
@@ -539,16 +521,15 @@
         c.meta->>'business_models' as business_models,
         c.meta->>'facility_size' as facility_size,
         c.meta->>'contact_name' as contact_name,
         c.meta->>'contact_title' as contact_title,
         c.meta->>'contact_email' as contact_email,
         c.meta->>'contact_phone' as contact_phone,
         c.meta->>'contact_address' as contact_address,
-        
-        
+        c.meta->>'gpt' as gpt,
         c.meta,
         r.rating::int, 
         COALESCE(co.comments, '[]'::jsonb) as comments
     FROM RankedEvents e
     LEFT JOIN actor a ON e.actor_key = a.key
     LEFT JOIN company c ON e.domain = c.domain
     LEFT JOIN comment co ON e.search_uid = co.search_uid AND e.domain = co.domain
@@ -622,14 +603,36 @@
     df["ownership"] = df["ownership"].apply(get_ownership)
     df["state"] = df.apply(get_state, axis=1)
     df["city"] = df.apply(get_city, axis=1)
     # df['year_founded'] = df['year_founded'].dropna().apply(lambda x: int(x))
     return df
 
 
+def search_comments(search_uid: int) -> pd.DataFrame:
+    statement = """
+    SELECT 
+        e.*,
+        a.name as author
+    FROM event e
+    LEFT JOIN actor a ON e.actor_key = a.key
+    WHERE
+        e.type = 'comment'
+        AND e.domain is null
+        AND search_uid = :search_uid
+    """
+
+    with db.connect() as conn:
+        result = conn.execute(
+            sqlalchemy.text(statement),
+            {"search_uid": search_uid},
+        )
+        df = pd.DataFrame(result.fetchall(), columns=result.keys())
+    return df
+
+
 def event(search_uid: int) -> pd.DataFrame:
     with db.connect() as conn:
         statement = """
                 SELECT *
                 FROM event
                 WHERE search_uid = :search_uid
             """
@@ -700,15 +703,14 @@
 def find_search(uid: int) -> ts.models.Search:
     with db.connect() as conn:
         statement = """
             SELECT 
                 uid, 
                 label, 
                 meta, 
-                fields, 
                 meta->>'next_due_date' as next_due_date,
                 meta->>'notes' as notes,
                 COALESCE(criteria.data, '{}'::jsonb) as criteria
             FROM search
             LEFT JOIN criteria ON search.uid = criteria.search_uid
             
             WHERE uid = :uid
```

### Comparing `gandai-1.7.41/gandai/secrets.py` & `gandai-1.7.42/gandai/secrets.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai/tasks.py` & `gandai-1.7.42/gandai/tasks.py`

 * *Files identical despite different names*

### Comparing `gandai-1.7.41/gandai.egg-info/SOURCES.txt` & `gandai-1.7.42/gandai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,8 +40,9 @@
 gandai/migrations/db_create.py
 gandai/migrations/db_seed.py
 gandai/migrations/dealcloud.py
 gandai/migrations/__pycache__/__init__.cpython-311.pyc
 gandai/migrations/__pycache__/dealcloud.cpython-311.pyc
 gandai/migrations/sql/2305023-alter.sql
 gandai/migrations/sql/230818-alter.sql
+gandai/migrations/sql/240523-alter.sql
 gandai/migrations/sql/schema.sql
```

