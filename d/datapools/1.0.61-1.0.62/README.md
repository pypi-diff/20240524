# Comparing `tmp/datapools-1.0.61.tar.gz` & `tmp/datapools-1.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.61.tar", last modified: Fri May 24 08:57:54 2024, max compression
+gzip compressed data, was "datapools-1.0.62.tar", last modified: Fri May 24 10:34:33 2024, max compression
```

## Comparing `datapools-1.0.61.tar` & `datapools-1.0.62.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.785375 datapools-1.0.61/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-24 08:57:38.000000 datapools-1.0.61/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    20504 2024-05-24 08:57:38.000000 datapools-1.0.61/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-24 08:57:38.000000 datapools-1.0.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-24 08:57:38.000000 datapools-1.0.61/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-24 08:57:54.785375 datapools-1.0.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-24 08:57:38.000000 datapools-1.0.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.769375 datapools-1.0.61/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.773375 datapools-1.0.61/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.773375 datapools-1.0.61/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.773375 datapools-1.0.61/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.773375 datapools-1.0.61/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.777375 datapools-1.0.61/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.777375 datapools-1.0.61/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.777375 datapools-1.0.61/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.777375 datapools-1.0.61/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.777375 datapools-1.0.61/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.777375 datapools-1.0.61/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.777375 datapools-1.0.61/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.777375 datapools-1.0.61/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.781376 datapools-1.0.61/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.781376 datapools-1.0.61/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.781376 datapools-1.0.61/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.781376 datapools-1.0.61/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.781376 datapools-1.0.61/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.781376 datapools-1.0.61/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.781376 datapools-1.0.61/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-05-24 08:57:38.000000 datapools-1.0.61/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.781376 datapools-1.0.61/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-24 08:57:54.000000 datapools-1.0.61/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-24 08:57:54.000000 datapools-1.0.61/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:57:54.000000 datapools-1.0.61/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 08:57:54.000000 datapools-1.0.61/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-24 08:57:54.000000 datapools-1.0.61/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 08:57:54.000000 datapools-1.0.61/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 08:57:54.785375 datapools-1.0.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-24 08:57:38.000000 datapools-1.0.61/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:54.781376 datapools-1.0.61/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 08:57:38.000000 datapools-1.0.61/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-24 08:57:38.000000 datapools-1.0.61/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-24 08:57:38.000000 datapools-1.0.61/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-24 08:57:38.000000 datapools-1.0.61/tests/test_session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.748338 datapools-1.0.62/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-24 10:34:25.000000 datapools-1.0.62/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    20762 2024-05-24 10:34:25.000000 datapools-1.0.62/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-24 10:34:25.000000 datapools-1.0.62/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-24 10:34:25.000000 datapools-1.0.62/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-24 10:34:33.748338 datapools-1.0.62/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-24 10:34:25.000000 datapools-1.0.62/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.732338 datapools-1.0.62/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.736338 datapools-1.0.62/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.736338 datapools-1.0.62/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.736338 datapools-1.0.62/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.736338 datapools-1.0.62/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.740338 datapools-1.0.62/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.740338 datapools-1.0.62/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.740338 datapools-1.0.62/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.740338 datapools-1.0.62/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.740338 datapools-1.0.62/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.740338 datapools-1.0.62/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.740338 datapools-1.0.62/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.740338 datapools-1.0.62/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.740338 datapools-1.0.62/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.740338 datapools-1.0.62/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.744338 datapools-1.0.62/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.744338 datapools-1.0.62/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.744338 datapools-1.0.62/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.744338 datapools-1.0.62/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.744338 datapools-1.0.62/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-05-24 10:34:25.000000 datapools-1.0.62/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.744338 datapools-1.0.62/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-24 10:34:33.000000 datapools-1.0.62/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-24 10:34:33.000000 datapools-1.0.62/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 10:34:33.000000 datapools-1.0.62/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 10:34:33.000000 datapools-1.0.62/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-24 10:34:33.000000 datapools-1.0.62/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 10:34:33.000000 datapools-1.0.62/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 10:34:33.748338 datapools-1.0.62/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-24 10:34:25.000000 datapools-1.0.62/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:33.744338 datapools-1.0.62/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:34:25.000000 datapools-1.0.62/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-24 10:34:25.000000 datapools-1.0.62/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-24 10:34:25.000000 datapools-1.0.62/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-24 10:34:25.000000 datapools-1.0.62/tests/test_session_manager.py
```

### Comparing `datapools-1.0.61/HISTORY.md` & `datapools-1.0.62/HISTORY.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- . [sergpsu]
+- . [sergpsu]
+- Merge pull request #80 from torrentsai/1.0.61_2. [S]
+
+  1.0.61
+- Release: version 1.0.61 🚀 [sergpsu]
+- Release: version 1.0.61 🚀 [sergpsu]
+
+
+1.0.61 (2024-05-24)
+-------------------
+- Release: version 1.0.61 🚀 [sergpsu]
 - Merge pull request #78 from torrentsai/dmtlvn/chunking. [Dmytro Levin]
 
   Content chunking support
 - Multi embedding evaluation support. [Dmytro]
 - Merge pull request #79 from torrentsai/sergpsu-async-redis. [S]
 
   Scheduler stop criteria
```

### Comparing `datapools-1.0.61/LICENSE` & `datapools-1.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/PKG-INFO` & `datapools-1.0.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.61
+Version: 1.0.62
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.61/README.md` & `datapools-1.0.62/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/api.py` & `datapools-1.0.62/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/cli.py` & `datapools-1.0.62/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/common/backend_api.py` & `datapools-1.0.62/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/common/queues/__init__.py` & `datapools-1.0.62/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/common/queues/rabbitmq.py` & `datapools-1.0.62/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/common/queues/types.py` & `datapools-1.0.62/datapools/common/queues/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from enum import Enum
+from typing import Optional, Any
 
 # from ..logger import logger
 
 
 class QueueRole(Enum):
     Publisher = 1
     Receiver = 2
@@ -13,14 +14,18 @@
     Task = 1
     Report = 2
     StorageInvalidation = 3
     Stop = 4
 
 
 class QueueMessage:
+    session_id: str
+    type: QueueMessageType
+    data: Optional[Any] = None
+
     def __init__(self, session_id: str, message_type: QueueMessageType, data=None):
         self.session_id = session_id
         self.type = message_type
         self.data = data
 
     def encode(self):
         # logger.info( f'encoding {self.type=} {self.data=}')
```

### Comparing `datapools-1.0.61/datapools/common/session_manager.py` & `datapools-1.0.62/datapools/common/session_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,14 +193,15 @@
             return Session(session_id, self.r)
         return None
 
     async def remove(self, session_id):
         await self.r.delete(SessionManager.get_meta_key(session_id))
         await self.r.delete(SessionManager.get_urls_key(session_id))
         await self.r.delete(SessionManager.get_content_key(session_id))
+        await self.r.delete(SessionManager.get_tags_usage_key(session_id))
 
     def gen_session_id(self) -> str:
         # TODO: add existance check
         return md5(str(time.time()).encode()).hexdigest()
 
     @staticmethod
     def get_meta_key(session_id):
```

### Comparing `datapools-1.0.61/datapools/common/stoppable.py` & `datapools-1.0.62/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/common/storage/base_storage.py` & `datapools-1.0.62/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/common/storage/file_storage.py` & `datapools-1.0.62/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.62/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.62/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/common/types.py` & `datapools-1.0.62/datapools/common/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/producer/base_producer.py` & `datapools-1.0.62/datapools/producer/base_producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 
     async def router_loop(self):
         try:
             while not await self.is_stopped():
                 message = await self.eval_queue.pop(timeout=1)
                 if message:
                     qm = QueueMessage.decode(message.body)
+                    logger.info(f"{qm.session_id=}")
                     try:
                         session = await self.session_manager.get(qm.session_id)
                         if session is None or await session.is_stopped():
                             logger.info(f"session is deleted or stopped {qm.session_id=} {message.message_id}")
                             await self.eval_queue.mark_done(message)
                             continue
```

### Comparing `datapools-1.0.61/datapools/scheduler/scheduler.py` & `datapools-1.0.62/datapools/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.62/datapools/worker/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.62/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/default/default.py` & `datapools-1.0.62/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.62/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.62/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.62/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.62/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.62/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.62/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.62/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.62/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.62/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools/worker/worker.py` & `datapools-1.0.62/datapools/worker/worker.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/datapools.egg-info/PKG-INFO` & `datapools-1.0.62/datapools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.61
+Version: 1.0.62
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.61/datapools.egg-info/SOURCES.txt` & `datapools-1.0.62/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/setup.py` & `datapools-1.0.62/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/tests/test_base.py` & `datapools-1.0.62/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.61/tests/test_session_manager.py` & `datapools-1.0.62/tests/test_session_manager.py`

 * *Files identical despite different names*

