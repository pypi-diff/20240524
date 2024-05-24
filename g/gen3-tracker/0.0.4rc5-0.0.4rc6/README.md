# Comparing `tmp/gen3_tracker-0.0.4rc5.tar.gz` & `tmp/gen3_tracker-0.0.4rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_tracker-0.0.4rc5.tar", last modified: Sun May 12 13:42:30 2024, max compression
+gzip compressed data, was "gen3_tracker-0.0.4rc6.tar", last modified: Thu May 23 15:30:04 2024, max compression
```

## Comparing `gen3_tracker-0.0.4rc5.tar` & `gen3_tracker-0.0.4rc6.tar`

### file list

```diff
@@ -1,70 +1,74 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.783902 gen3_tracker-0.0.4rc5/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.4rc5/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     2371 2024-05-12 13:42:30.783411 gen3_tracker-0.0.4rc5/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1524 2024-05-06 16:38:51.000000 gen3_tracker-0.0.4rc5/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.716234 gen3_tracker-0.0.4rc5/gen3_tracker/
--rw-r--r--   0 walsbr   (320923486) 1971611142     5974 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2963 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.733293 gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.734855 gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     3310 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5151 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/access/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.735194 gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/access/policies/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/access/policies/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     6820 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/access/requestor.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1123 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/access/submitter.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    13801 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.735391 gen3_tracker-0.0.4rc5/gen3_tracker/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142    18461 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.735996 gen3_tracker-0.0.4rc5/gen3_tracker/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142    10325 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/config/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.737056 gen3_tracker-0.0.4rc5/gen3_tracker/gen3/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-04-27 13:15:12.000000 gen3_tracker-0.0.4rc5/gen3_tracker/gen3/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.738172 gen3_tracker-0.0.4rc5/gen3_tracker/gen3/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1323 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/gen3/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      883 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc5/gen3_tracker/gen3/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc5/gen3_tracker/gen3/buckets/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3354 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/gen3/indexd.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4164 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/gen3/jobs.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.740275 gen3_tracker-0.0.4rc5/gen3_tracker/git/
--rw-r--r--   0 walsbr   (320923486) 1971611142    20215 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/git/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    11639 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/git/adder.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    32036 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/git/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2508 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/git/cloner.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1466 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/git/initializer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2609 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/git/snapshotter.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.765514 gen3_tracker-0.0.4rc5/gen3_tracker/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     5924 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4979 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    13471 2024-05-03 19:08:14.000000 gen3_tracker-0.0.4rc5/gen3_tracker/meta/dataframer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    11143 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/meta/skeleton.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4428 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/meta/validator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1211 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/meta/visualizer.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.775701 gen3_tracker-0.0.4rc5/gen3_tracker/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2781 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     4799 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2411 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1566 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/gen3_tracker/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.731120 gen3_tracker-0.0.4rc5/gen3_tracker.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2371 2024-05-12 13:42:30.000000 gen3_tracker-0.0.4rc5/gen3_tracker.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1642 2024-05-12 13:42:30.000000 gen3_tracker-0.0.4rc5/gen3_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-05-12 13:42:30.000000 gen3_tracker-0.0.4rc5/gen3_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       45 2024-05-12 13:42:30.000000 gen3_tracker-0.0.4rc5/gen3_tracker.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      209 2024-05-12 13:42:30.000000 gen3_tracker-0.0.4rc5/gen3_tracker.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       13 2024-05-12 13:42:30.000000 gen3_tracker-0.0.4rc5/gen3_tracker.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-05-12 13:42:30.783956 gen3_tracker-0.0.4rc5/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142      819 2024-05-12 13:42:18.000000 gen3_tracker-0.0.4rc5/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.776181 gen3_tracker-0.0.4rc5/tests/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-04-16 13:21:28.000000 gen3_tracker-0.0.4rc5/tests/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.778317 gen3_tracker-0.0.4rc5/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2307 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      470 2024-05-05 15:05:17.000000 gen3_tracker-0.0.4rc5/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3392 2024-05-08 18:45:03.000000 gen3_tracker-0.0.4rc5/tests/integration/test_bucket_import.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3394 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/tests/integration/test_bundle.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3826 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/tests/integration/test_end_to_end_workflow.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-12 13:42:30.781424 gen3_tracker-0.0.4rc5/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-05-02 22:49:35.000000 gen3_tracker-0.0.4rc5/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    20363 2024-05-01 22:45:46.000000 gen3_tracker-0.0.4rc5/tests/unit/test_flatten_fhir_example.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/tests/unit/test_hash_types.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      601 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc5/tests/unit/test_read_dvc.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.789691 gen3_tracker-0.0.4rc6/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_tracker-0.0.4rc6/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2371 2024-05-23 15:30:04.784351 gen3_tracker-0.0.4rc6/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1524 2024-05-06 16:38:51.000000 gen3_tracker-0.0.4rc6/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.735893 gen3_tracker-0.0.4rc6/gen3_tracker/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5974 2024-05-22 00:42:43.000000 gen3_tracker-0.0.4rc6/gen3_tracker/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2963 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.739181 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-10-19 18:09:26.000000 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.741205 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3310 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5151 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.746666 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/policies/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-07-07 00:00:20.000000 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/policies/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      189 2024-02-29 16:26:49.000000 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/policies/add-project-default.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142       76 2024-02-26 20:40:22.000000 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/policies/add-user-read.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142      204 2024-05-09 02:02:53.000000 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/policies/add-user-write.yaml
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6820 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/requestor.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1123 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/submitter.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13796 2024-05-15 03:49:57.000000 gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.747260 gen3_tracker-0.0.4rc6/gen3_tracker/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    18461 2024-05-21 23:43:06.000000 gen3_tracker-0.0.4rc6/gen3_tracker/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.748203 gen3_tracker-0.0.4rc6/gen3_tracker/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    10325 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      137 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc6/gen3_tracker/config.yaml
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.750146 gen3_tracker-0.0.4rc6/gen3_tracker/gen3/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-04-27 13:15:12.000000 gen3_tracker-0.0.4rc6/gen3_tracker/gen3/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.765105 gen3_tracker-0.0.4rc6/gen3_tracker/gen3/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1323 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/gen3/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      883 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc6/gen3_tracker/gen3/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      559 2024-02-26 20:51:35.000000 gen3_tracker-0.0.4rc6/gen3_tracker/gen3/buckets/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3354 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/gen3/indexd.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6201 2024-05-15 20:04:35.000000 gen3_tracker-0.0.4rc6/gen3_tracker/gen3/jobs.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.768994 gen3_tracker-0.0.4rc6/gen3_tracker/git/
+-rw-r--r--   0 walsbr   (320923486) 1971611142    23443 2024-05-16 06:52:43.000000 gen3_tracker-0.0.4rc6/gen3_tracker/git/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    11639 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/git/adder.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    37906 2024-05-16 19:45:28.000000 gen3_tracker-0.0.4rc6/gen3_tracker/git/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3026 2024-05-16 13:45:52.000000 gen3_tracker-0.0.4rc6/gen3_tracker/git/cloner.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1466 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/git/initializer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2609 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/git/snapshotter.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.772381 gen3_tracker-0.0.4rc6/gen3_tracker/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5924 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5107 2024-05-23 14:56:48.000000 gen3_tracker-0.0.4rc6/gen3_tracker/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    22163 2024-05-23 14:58:52.000000 gen3_tracker-0.0.4rc6/gen3_tracker/meta/dataframer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13547 2024-05-23 14:55:54.000000 gen3_tracker-0.0.4rc6/gen3_tracker/meta/skeleton.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4428 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/meta/validator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1211 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/meta/visualizer.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.778870 gen3_tracker-0.0.4rc6/gen3_tracker/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2781 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4799 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2411 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1566 2024-05-11 19:00:33.000000 gen3_tracker-0.0.4rc6/gen3_tracker/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.738626 gen3_tracker-0.0.4rc6/gen3_tracker.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2371 2024-05-23 15:30:04.000000 gen3_tracker-0.0.4rc6/gen3_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1857 2024-05-23 15:30:04.000000 gen3_tracker-0.0.4rc6/gen3_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2024-05-23 15:30:04.000000 gen3_tracker-0.0.4rc6/gen3_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       45 2024-05-23 15:30:04.000000 gen3_tracker-0.0.4rc6/gen3_tracker.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      209 2024-05-23 15:30:04.000000 gen3_tracker-0.0.4rc6/gen3_tracker.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       13 2024-05-23 15:30:04.000000 gen3_tracker-0.0.4rc6/gen3_tracker.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2024-05-23 15:30:04.789767 gen3_tracker-0.0.4rc6/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142      912 2024-05-23 15:29:36.000000 gen3_tracker-0.0.4rc6/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.779506 gen3_tracker-0.0.4rc6/tests/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-04-16 13:21:28.000000 gen3_tracker-0.0.4rc6/tests/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.781486 gen3_tracker-0.0.4rc6/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2307 2024-05-15 03:31:16.000000 gen3_tracker-0.0.4rc6/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      470 2024-05-05 15:05:17.000000 gen3_tracker-0.0.4rc6/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3388 2024-05-16 02:28:15.000000 gen3_tracker-0.0.4rc6/tests/integration/test_bucket_import.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3394 2024-05-15 03:31:16.000000 gen3_tracker-0.0.4rc6/tests/integration/test_bundle.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3913 2024-05-16 03:02:50.000000 gen3_tracker-0.0.4rc6/tests/integration/test_end_to_end_workflow.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2024-05-23 15:30:04.783433 gen3_tracker-0.0.4rc6/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2024-05-02 22:49:35.000000 gen3_tracker-0.0.4rc6/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    20363 2024-05-01 22:45:46.000000 gen3_tracker-0.0.4rc6/tests/unit/test_flatten_fhir_example.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2024-05-15 03:31:16.000000 gen3_tracker-0.0.4rc6/tests/unit/test_hash_types.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      601 2024-05-15 03:31:16.000000 gen3_tracker-0.0.4rc6/tests/unit/test_read_dvc.py
```

### Comparing `gen3_tracker-0.0.4rc5/LICENSE` & `gen3_tracker-0.0.4rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/PKG-INFO` & `gen3_tracker-0.0.4rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_tracker
-Version: 0.0.4rc5
+Version: 0.0.4rc6
 Summary: A CLI for adding version control to Gen3 data submission projects.
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: walsbr
 Author-email: walsbr@ohsu.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `gen3_tracker-0.0.4rc5/README.md` & `gen3_tracker-0.0.4rc6/README.md`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/__init__.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/cli.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/access/__init__.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/access/cli.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/access/requestor.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/access/submitter.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/access/submitter.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/collaborator/cli.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/collaborator/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             output.exit_code = 1
             if config.debug:
                 raise e
 
 
 @collaborator.command(name="pending")
 @click.pass_obj
-def project_approve_request(config: Config):
+def project_ls_pending(config: Config):
     """Show all pending requests."""
     import gen3_tracker.collaborator.access.requestor
 
     with CLIOutput(config=config) as output:
         try:
             with Halo(text='Searching', spinner='line', placement='right', color='white'):
                 auth = ensure_auth(config=config)
```

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/common/__init__.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/config/__init__.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/gen3/buckets/__init__.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/gen3/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/gen3/buckets/cli.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/gen3/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/gen3/buckets/lister.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/gen3/buckets/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/gen3/indexd.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/gen3/indexd.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/git/__init__.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/git/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import json
 import logging
 import multiprocessing
 import os
 import pathlib
+import re
 import subprocess
 import time
 import typing
 import uuid
 import zipfile
 from abc import abstractmethod
 from datetime import datetime
 from typing import NamedTuple
 
 import pydantic
 import pytz
 import yaml
+from fhir.resources.attachment import Attachment
 from gen3.auth import Gen3Auth
 from pydantic import BaseModel, ConfigDict, field_validator
 
 from gen3_tracker import ACED_NAMESPACE
 from gen3_tracker.common import ACCEPTABLE_HASHES, parse_iso_tz_date
 
 # constants ---------------------------------------------------------------------
@@ -29,14 +31,16 @@
 RESET_MESSAGE = 'Resetting changes in the repository...'
 UNDO_INIT_MESSAGE = 'Removing change control from repository...'
 MISSING_GIT_MESSAGE = '.git is not initialized in the current directory.'
 MISSING_G3T_MESSAGE = '.g3t is not initialized in the current directory.'
 STATUS_MESSAGE = 'Showing changed stages...'
 DIFF_MESSAGE = 'Showing details of changed files...'
 
+LOGGED_ALREADY = set()
+
 
 # process helpers ---------------------------------------------------------------
 class CommandResult(NamedTuple):
     """
     A NamedTuple that represents the result of a command execution.
 
     Attributes:
@@ -66,15 +70,15 @@
     size: int
     is_symlink: typing.Optional[bool] = False
     realpath: typing.Optional[str] = None
     """For symlinked files, the real path to the file."""
     source_url: typing.Optional[str] = None
     """bucket imports, the url to the file."""
 
-    _object_id: typing.Optional[str] = None
+    object_id: typing.Optional[str] = None
 
     @pydantic.model_validator(mode="after")
     def check_hash_value(self):
         """Check that the hash value is valid."""
         hash_type = self.hash
         assert hash_type in ACCEPTABLE_HASHES, f'Invalid hash type {hash_type}'
         v = getattr(self, hash_type)
@@ -85,20 +89,24 @@
     @property
     def hash_value(self):
         """Get the hash value."""
         return getattr(self, self.hash)
 
     def set_object_id(self, project_id: str) -> str:
         """ create a unique did for this object within a project"""
-        self._object_id = str(uuid.uuid5(ACED_NAMESPACE, project_id + f"::{self.path}"))
-        return self._object_id
+        assert self.path, 'path is required'
 
-    @property
-    def object_id(self):
-        return self._object_id
+        def _normalize_file_url(path: str) -> str:
+            """Strip leading ./ and file:/// from file urls."""
+            path = re.sub(r'^file:\/\/\/', '', path)
+            path = re.sub(r'^\.\/', '', path)
+            return path
+
+        self.object_id = str(uuid.uuid5(ACED_NAMESPACE, project_id + f"::{_normalize_file_url(self.path)}"))
+        return self.object_id
 
 
 class DVCMeta(BaseModel):
     model_config = ConfigDict(
         extra='allow',
     )
 
@@ -109,31 +117,92 @@
     no_bucket: typing.Optional[bool] = False
 
 
 class DVC(BaseModel):
     model_config = ConfigDict(
         extra='allow',
     )
-    meta: typing.Optional[DVCMeta] = {}
+    meta: typing.Optional[DVCMeta] = None
     outs: list[DVCItem]
     project_id: typing.Optional[str] = None
 
     @field_validator('outs')
     def check_outs(cls, v):
         if len(v) < 1:
             raise ValueError('outs must contain at least one item')
         return v
 
+    @pydantic.model_validator(mode="after")
+    def check_object_id(self):
+        """Set the object_id if empty."""
+        if not self.object_id and self.project_id:
+            self.outs[0].set_object_id(self.project_id)
+        return self
+
     @property
     def out(self) -> DVCItem:
+        """Convenience method to get the first out."""
         return self.outs[0]
 
     @property
     def object_id(self) -> str:
-        return self.outs[0].set_object_id(self.project_id)
+        """Convenience method to get the first object_id."""
+        if not self.outs[0].object_id and self.project_id:
+            self.outs[0].set_object_id(self.project_id)
+        return self.outs[0].object_id
+
+    @classmethod
+    def from_document_reference(cls, config, document_reference, references) -> 'DVC':
+        """Factory: create DVC from DocumentReference.
+
+        Args:
+            config (object): our config object
+            document_reference (DocumentReference): loaded DocumentReferences
+            references (dict): cross ref of Reference to Identifiers
+
+        """
+        attachment: Attachment = document_reference.content[0].attachment
+        assert attachment.extension, document_reference
+        source_path = [_.valueUrl for _ in attachment.extension if _.url.endswith('source_path')][0]
+        md5 = [_.valueString for _ in attachment.extension if _.url.endswith('md5')][0]
+        assert source_path, document_reference
+        assert md5, document_reference
+        dvc_object = DVC(
+            project_id=config.gen3.project_id,
+            outs=[
+                DVCItem(
+                    modified=attachment.creation.isoformat(),
+                    path=attachment.url.replace('file:///', ''),
+                    size=attachment.size,
+                    realpath=source_path.replace('file:///', ''),
+                    mime=attachment.contentType,
+                    md5=md5,
+                    hash='md5',
+                    object_id=document_reference.id
+                )
+            ],
+        )
+        if document_reference.subject:
+
+            if document_reference.subject.reference in references:
+                key = document_reference.subject.reference.split('/')[0]
+
+                if key not in ['ResearchStudy']:
+                    value = references[document_reference.subject.reference]
+                    meta = DVCMeta.model_validate({key: value})
+                    assert isinstance(meta, DVCMeta), f"Did not get expected meta {meta}"
+                    dvc_object.meta = meta
+            else:
+                msg = f"Did not find {document_reference.subject.reference} in references"
+                if msg not in LOGGED_ALREADY:
+                    logging.getLogger(__package__).warning(msg)
+                    LOGGED_ALREADY.add(msg)
+        assert attachment.url.replace('file:///', '') == dvc_object.out.path, f"attachment and dvc path doesn't match"
+        assert document_reference.id == dvc_object.object_id, f"Did not get expected ID {config.gen3.project_id} {attachment.url}/{document_reference.id} {dvc_object.out.path}/{dvc_object.object_id}"
+        return dvc_object
 
 
 def run_command(command: str, dry_run: bool = False, raise_on_err: bool = True, env: dict = None, no_capture: bool = False) -> CommandResult:
     """Run a shell command and return its output. Raise an exception if the command fails."""
     _logger = logging.getLogger(__package__)
     if dry_run:
         _logger.info(f'dry_run: {command}')
```

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/git/adder.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/git/adder.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/git/cli.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/git/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,38 +4,43 @@
 import multiprocessing
 import os
 import pathlib
 import re
 import shutil
 import subprocess
 import sys
+import time
 import zipfile
 from datetime import datetime
 
 import click
+import pytz
 import yaml
+from fhir.resources.documentreference import DocumentReference
 from gen3.auth import Gen3AuthError
 from gen3.file import Gen3File
 from gen3.index import Gen3Index
 from halo import Halo
 from tqdm import tqdm
 
 import gen3_tracker
 from gen3_tracker import Config
-from gen3_tracker.common import CLIOutput, INFO_COLOR, ERROR_COLOR, is_url, filter_dicts
+from gen3_tracker.common import CLIOutput, INFO_COLOR, ERROR_COLOR, is_url, filter_dicts, SUCCESS_COLOR, \
+    read_ndjson_file
 from gen3_tracker.config import init as config_init
 from gen3_tracker.config import init as config_init, ensure_auth
 from gen3_tracker.git import git_files, to_indexd, to_remote, dvc_data, \
     data_file_changes, modified_date, git_status, DVC, MISSING_G3T_MESSAGE
 from gen3_tracker.git import run_command, \
     MISSING_GIT_MESSAGE, git_repository_exists
-from gen3_tracker.git.adder import url_path
+from gen3_tracker.git.adder import url_path, write_dvc_file
 from gen3_tracker.git.cloner import ls
 from gen3_tracker.git.initializer import initialize_project_server_side
 from gen3_tracker.git.snapshotter import push_snapshot
+from gen3_tracker.meta.skeleton import meta_index
 
 # logging.basicConfig(level=logging.INFO)
 _logger = logging.getLogger(__package__)
 
 
 # @click.command(cls=NaturalOrderGroup)
 # @click.option('--debug', is_flag=True, envvar='G3T_DEBUG', help='Enable debug mode. G3T_DEBUG environment variable can also be used.')
@@ -90,32 +95,15 @@
         _check_parameters(config, project_id)
 
         logs = []
         # create directories
         for _ in config_init(config, project_id):
             logs.append(_)
 
-        # ensure a git repo
-        if not pathlib.Path('.git').exists():
-            command = 'git init'
-            run_command(command, dry_run=config.dry_run, no_capture=True)
-        else:
-            click.secho('Git repository already exists.', fg=INFO_COLOR, file=sys.stderr)
-
-        pathlib.Path('MANIFEST').mkdir(exist_ok=True)
-        pathlib.Path('META').mkdir(exist_ok=True)
-        pathlib.Path('LOGS').mkdir(exist_ok=True)
-        with open('.gitignore', 'w') as f:
-            f.write('LOGS/\n')
-        with open('META/README.md', 'w') as f:
-            f.write('This directory contains metadata files for the data files in the MANIFEST directory.\n')
-        with open('MANIFEST/README.md', 'w') as f:
-            f.write('This directory contains dvc files that reference the data files.\n')
-        run_command('git add MANIFEST META .gitignore .g3t', dry_run=config.dry_run, no_capture=True)
-        run_command('git commit -m "initialized" MANIFEST META .gitignore .g3t', dry_run=config.dry_run, no_capture=True)
+        ensure_git_repo(config)
 
         if not no_server:
             logs.extend(initialize_project_server_side(config, project_id))
 
             if approve:
                 run_command('g3t projects create', dry_run=config.dry_run, no_capture=True)
                 run_command('g3t collaborator approve --all', dry_run=config.dry_run, no_capture=True)
@@ -128,14 +116,35 @@
 
     except Exception as e:
         click.secho(str(e), fg=ERROR_COLOR, file=sys.stderr)
         if config.debug:
             raise
 
 
+def ensure_git_repo(config):
+    # ensure a git repo
+    if not pathlib.Path('.git').exists():
+        command = 'git init'
+        run_command(command, dry_run=config.dry_run, no_capture=True)
+    else:
+        click.secho('Git repository already exists.', fg=INFO_COLOR, file=sys.stderr)
+    pathlib.Path('MANIFEST').mkdir(exist_ok=True)
+    pathlib.Path('META').mkdir(exist_ok=True)
+    pathlib.Path('LOGS').mkdir(exist_ok=True)
+    with open('.gitignore', 'w') as f:
+        f.write('LOGS/\n')
+        f.write('.g3t/state/\n')  # legacy
+    with open('META/README.md', 'w') as f:
+        f.write('This directory contains metadata files for the data files in the MANIFEST directory.\n')
+    with open('MANIFEST/README.md', 'w') as f:
+        f.write('This directory contains dvc files that reference the data files.\n')
+    run_command('git add MANIFEST META .gitignore .g3t', dry_run=config.dry_run, no_capture=True)
+    run_command('git commit -m "initialized" MANIFEST META .gitignore .g3t', dry_run=config.dry_run, no_capture=True)
+
+
 # Note: The commented code below is an example of how to use context settings to allow extra arguments.
 # context_settings=dict(
 #     ignore_unknown_options=True,
 #     allow_extra_args=True,
 # )
 
 
@@ -143,16 +152,42 @@
 @click.argument('target')
 @click.pass_context
 def add(ctx, target):
     """
     Update references to data files to the repository.
 
     \b
-    TARGETS are "data files" not checked into the repository.
-    We commit their proxies - MANIFEST/*.dvc files.
+    TARGET is a "data file", either files or urls.
+    We commit their proxies - MANIFEST/<TARGET>.dvc files.
+    \b
+    If the TARGET is a file in the local file system:
+        - We will automatically calculate the hash, size, modified and mime type of the file
+        - You can specify those values with the --<hash>, --size, --modified and --mime options
+        - As a convenience, you can use wildcards to add multiple files at once.
+          If wildcards are used, the hash, size, modified and mime type parameters are ignored.
+    \b
+    If the TARGET is a url:
+        - You must specify the hash, size, modified and mime type
+        - Wildcards are not supported
+    \b
+    --<hash> <value>: Valid options are: ['md5', 'sha1', 'sha256', 'sha512', 'crc', 'etag']
+                      Value must conform to the hash type.
+    \b
+    --modified: A variety of date formats are supported, see https://tinyurl.com/ysad3rj7
+    \b
+    --mime: If not specified, it will be inferred from the file extension.
+    \b
+    Identifiers:
+    In order to link a file with associated Patient, Specimen, Observation or Task, you can use one of the following identifiers:
+    --patient <value>: The patient identifier
+    --specimen <value>: The specimen identifier, requires patient
+    --observation <value>: The observation identifier, requires patient, optionally specimen
+    --task <value>: The task identifier, requires either patient or specimen
+    The <value> is a user defined string that will be used to link the data file with the associated resource.  Do not use PHI in the value.
+    See `g3t meta` for more
     """
     from gen3_tracker.git.adder import add_file, add_url
 
     config: Config = ctx.obj
     try:
         # needs to be in project root
         assert git_repository_exists(config.debug), MISSING_GIT_MESSAGE
@@ -168,53 +203,90 @@
             all_changed_files, updates = add_file(ctx, target)
 
         #
         # if it is an update, we do not need to add the file to git
         #
         adds = [str(_) for _ in all_changed_files if _ not in updates]
         if adds:
+            adds.append('.gitignore')
             run_command(f'git add {" ".join([str(_) for _ in adds])}', dry_run=config.dry_run, no_capture=True)
 
     except Exception as e:
         click.secho(str(e), fg=ERROR_COLOR, file=sys.stderr)
         if config.debug:
             raise
 
 
+@cli.command(context_settings=dict(ignore_unknown_options=True, allow_extra_args=True))
+@click.argument('targets',  nargs=-1)
+@click.option('--message', '-m', help='The commit message.')
+@click.option('--all', '-a', is_flag=True, default=False, help='Automatically stage files that have been modified and deleted.')
+@click.pass_context
+def commit(ctx, targets, message, all):
+    """Commit the changes
+    \b
+    TARGETS: list of files (default: all)
+    """
+    config: Config = ctx.obj
+    command = [
+        "git",
+        "commit",
+        "-m",
+        f'"{message}"',
+    ] + list(targets)
+
+    if all:
+        command.append("-a")
+
+    run_command(" ".join(command), dry_run=config.dry_run, no_capture=True)
+
+
 @cli.command()
 @click.pass_obj
 def status(config):
     """Show changed files."""
+    soft_error = False
     try:
         with Halo(text='Scanning', spinner='line', placement='right', color='white'):
             manifest_path = pathlib.Path('MANIFEST')
             changes = data_file_changes(manifest_path)
             # Get a list of all files in the MANIFEST directory and its subdirectories
             files = glob.glob('MANIFEST/**/*.dvc', recursive=True)
             # Filter out directories, keep only files
             files = [f for f in files if os.path.isfile(f)]
+        if not files:
+            click.secho(f"No files have been added.", fg=INFO_COLOR, file=sys.stderr)
+        else:
             # Find the most recently changed file
             latest_file = max(files, key=os.path.getmtime)
-            # Get the modification time
-            document_reference_mtime = os.path.getmtime('META/DocumentReference.ndjson')
 
-        if document_reference_mtime < os.path.getmtime(latest_file):
-            click.secho(f"DocumentReference.ndjson is out of date. The most recently changed file is {latest_file}.", fg=INFO_COLOR, file=sys.stderr)
+            document_reference_mtime = 0
 
-        if changes:
-            click.secho(f"# There are {len(changes)} data files that you need to update via `g3t add`:", fg=INFO_COLOR, file=sys.stderr)
-            cwd = pathlib.Path.cwd()
-            for _ in changes:
-                data_path = str(_.data_path).replace(str(cwd) + '/', "")
-                click.secho(f'  g3t add {data_path} # changed: {modified_date(_.data_path)},  last added: {modified_date(_.dvc_path)}', fg=INFO_COLOR, file=sys.stderr)
-        else:
-            click.secho("No data file changes.", fg=INFO_COLOR, file=sys.stderr)
+            if pathlib.Path('META/DocumentReference.ndjson').exists():
+                # Get the modification time
+                document_reference_mtime = os.path.getmtime('META/DocumentReference.ndjson')
+
+            if document_reference_mtime < os.path.getmtime(latest_file):
+                click.secho(f"DocumentReference.ndjson is out of date. The most recently changed file is {latest_file}.  Please run `g3t meta init`", fg=INFO_COLOR, file=sys.stderr)
+                soft_error = True
+
+            if changes:
+                click.secho(f"# There are {len(changes)} data files that you need to update via `g3t add`:", fg=INFO_COLOR, file=sys.stderr)
+                cwd = pathlib.Path.cwd()
+                for _ in changes:
+                    data_path = str(_.data_path).replace(str(cwd) + '/', "")
+                    click.secho(f'  g3t add {data_path} # changed: {modified_date(_.data_path)},  last added: {modified_date(_.dvc_path)}', fg=INFO_COLOR, file=sys.stderr)
+                    soft_error = True
+            else:
+                click.secho("No data file changes.", fg=INFO_COLOR, file=sys.stderr)
 
         _ = run_command('git status')
         print(_.stdout)
+        if soft_error:
+            exit(1)
     except Exception as e:
         click.secho(str(e), fg=ERROR_COLOR, file=sys.stderr)
         if config.debug:
             raise
 
 
 @cli.command()
@@ -251,19 +323,29 @@
         s3-map - (admin) s3 index only external s3
     """
     from gen3_tracker.gen3.jobs import publish_commits
     from gen3_tracker.gen3.buckets import get_program_bucket
 
     config = ctx.obj
 
-    if re_run:
-        # step = 'publish'
-        raise NotImplementedError("Re-run not implemented")
-
     try:
+
+        if re_run:
+            # step = 'publish'
+            raise NotImplementedError("Re-run not implemented")
+
+        try:
+            run_command("g3t status")
+        except Exception as e:
+            click.secho("Please correct issues before pushing.", fg=ERROR_COLOR, file=sys.stderr)
+            click.secho(str(e), fg=ERROR_COLOR, file=sys.stderr)
+            if config.debug:
+                raise
+            exit(1)
+
         with Halo(text='Scanning', spinner='line', placement='right', color='white'):
 
             # check git status
             branch, uncommitted = git_status()
             assert not uncommitted, f"Uncommitted changes found.  Please commit or stash them first."
 
             # check dvc vs external files
@@ -333,18 +415,22 @@
             )
 
         with Halo(text='Uploading snapshot', spinner='line', placement='right', color='white'):
             push_snapshot(config, auth=auth)
 
         if step in ['publish', 'all']:
             if transfer_method == 'gen3':
-                with Halo(text='Publishing', spinner='line', placement='right', color='white'):
-                    _ = publish_commits(config, wait=wait, auth=auth, bucket_name=bucket_name)
-                click.secho(f'Published project', fg=INFO_COLOR, file=sys.stderr)
-                click.secho(_, fg=INFO_COLOR, file=sys.stdout)
+                with Halo(text='Publishing', spinner='line', placement='right', color='white') as spinner:
+                    _ = publish_commits(config, wait=wait, auth=auth, bucket_name=bucket_name, spinner=spinner)
+                click.secho(f'Published project. See logs/publish.log', fg=SUCCESS_COLOR, file=sys.stderr)
+                with open("logs/publish.log", 'a') as f:
+                    log_msg = {'timestamp': datetime.now(pytz.UTC).isoformat()}
+                    log_msg.update(_)
+                    f.write(json.dumps(log_msg, separators=(',', ':')))
+                    f.write('\n')
             else:
                 click.secho(f'Auto-publishing not supported for {transfer_method}. Please use --step publish after uploading', fg=ERROR_COLOR, file=sys.stderr)
 
     except Exception as e:
         click.secho(str(e), fg=ERROR_COLOR, file=sys.stderr)
         if config.debug:
             raise
@@ -429,22 +515,60 @@
 @cli.command()
 @click.argument('project_id', default=None, required=False, envvar=f"{gen3_tracker.ENV_VARIABLE_PREFIX}PROJECT_ID", metavar='PROJECT_ID')
 @click.pass_obj
 def clone(config, project_id):
     """Clone a repository into a new directory"""
     try:
         config.gen3.project_id = project_id
+        assert not pathlib.Path(project_id).exists(), f"{project_id} already exists.  Please remove it first."
+        os.mkdir(project_id)
+        os.chdir(project_id)
         with Halo(text='Cloning', spinner='line', placement='right', color='white'):
             auth = gen3_tracker.config.ensure_auth(config=config)
             snapshot, zip_filepath = download_snapshot(auth, config)
             assert not pathlib.Path('.git').exists(), "A git repository already exists.  Please remove it, or move to another directory first."
             # unzip
             with zipfile.ZipFile(zip_filepath, 'r') as zip_ref:
                 zip_ref.extractall('.')
 
+            # if we just unzipped a .git these directories will exist
+            expected_dirs = ['.git', 'META', 'MANIFEST']
+            if not all([pathlib.Path(_).exists() for _ in expected_dirs]):
+                # if not, we have downloaded a legacy SNAPSHOT.zip, so lets migrate the data to the expected drirectories
+                click.secho(f"{expected_dirs} not found after downloading {snapshot['file_name']} processing legacy snapshot", fg=INFO_COLOR, file=sys.stderr)
+                # legacy - was this a *SNAPSHOT.zip?
+                meta_files = (pathlib.Path('studies') / config.gen3.project)
+                # legacy - was this a *meta.zip?
+                if not meta_files.exists():
+                    meta_files = pathlib.Path('.')
+                # create local directories and git
+                [_ for _ in config_init(config, project_id)]
+                ensure_git_repo(config=config)
+                # move ndjson from studies to META
+                for _ in meta_files.glob('*.ndjson'):
+                    shutil.move(_, 'META/')
+                # add to git
+                run_command('git add META/*.*')
+                # migrate DocumentReferences to MANIFEST
+                references = meta_index()
+                manifest_files = []
+                for _ in read_ndjson_file('META/DocumentReference.ndjson'):
+                    document_reference = DocumentReference.parse_obj(_)
+                    dvc_object = DVC.from_document_reference(config, document_reference, references)
+                    manifest_files.append(write_dvc_file(yaml_data=dvc_object.model_dump(), target=dvc_object.out.path))
+
+                # Get the current time in seconds since the epoch
+                current_time = time.time()
+                # Update the access and modification times of the file
+                os.utime('META/DocumentReference.ndjson', (current_time, current_time))
+
+                run_command('git add MANIFEST/')
+                run_command('git commit -m "migrated from legacy" MANIFEST/ META/ .gitignore')
+                shutil.move(zip_filepath, config.work_dir / zip_filepath.name)
+
         click.secho(f"Cloned {snapshot['file_name']}", fg=INFO_COLOR, file=sys.stderr)
         run_command("git status", no_capture=True)
 
     except Exception as e:
         click.secho(str(e), fg=ERROR_COLOR, file=sys.stderr)
         if config.debug:
             raise
@@ -513,15 +637,15 @@
             # list all data files
             dvc_objects = {_.object_id: _ for _ in dvc_objects}
 
             def _dvc_meta(dvc_object, full=False) -> dict:
                 if not dvc_object:
                     return {}
                 _ = {}
-                if not full:
+                if not full and dvc_object.meta:
                     for k, v in dvc_object.meta.model_dump(exclude_none=True).items():
                         if v:
                             _[k] = v
                 else:
                     _ = dvc_object.model_dump(exclude_none=True)
                 _['object_id'] = dvc_object.object_id
                 return _
```

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/git/initializer.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/git/initializer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/git/snapshotter.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/git/snapshotter.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/meta/__init__.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/meta/cli.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/meta/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -98,29 +98,29 @@
 @click.argument("directory_path",
                 type=click.Path(exists=True, file_okay=False),
                 default="./META", required=False)
 @click.argument("output_path",
                 type=click.Path(file_okay=True),
                 default="meta.csv", required=False)
 @click.option('--dtale', 'launch_dtale', default=False, show_default=True, is_flag=True, help='Open the graph in a browser using the dtale package for interactive data exploration.')
+@click.option('--data_type', required=True, type=click.Choice(['Patient', 'Specimen', 'Observation', 'DocumentReference']), default=None, show_default=True,  help='Create a data frame for a specific data type.')
 @click.pass_obj
-def render_df(config: Config, directory_path: str, output_path: str, launch_dtale: bool):
+def render_df(config: Config, directory_path: str, output_path: str, launch_dtale: bool, data_type: str):
     """Render a metadata dataframe.
 
     \b
     directory_path: The directory path to the metadata.
     output_path: The output path for the dataframe. default [meta.csv]
     """
     try:
         from gen3_tracker.meta.dataframer import create_dataframe
-        with Halo(text='Creating DataFrame', spinner='line', placement='right', color='white'):
-            df = create_dataframe(directory_path, config.work_dir)
+        df = create_dataframe(directory_path, config.work_dir, data_type)
 
         if launch_dtale:
-            from dtale import dtale
+            import dtale
             dtale.show(df, subprocess=False, open_browser=True, port=40000)
         else:
             # export to csv
             df.to_csv(output_path, index=False)
             click.secho(f"Saved {output_path}", fg=INFO_COLOR, file=sys.stderr)
     except Exception as e:
         click.secho(str(e), fg=ERROR_COLOR, file=sys.stderr)
```

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/meta/dataframer.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/meta/dataframer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import json
 import pathlib
 import sqlite3
-from typing import Generator
+from functools import lru_cache
+from typing import Generator, Optional, List, Tuple
 
 import inflection
 import ndjson
 import numpy as np
 import pandas as pd
+from tqdm import tqdm
 
 
 class LocalFHIRDatabase:
     def __init__(self, db_name):  # , db_name=pathlib.Path('.g3t') / 'local.db'):
         self.db_name = db_name
         self.connection = None
         self.cursor = None
@@ -119,32 +121,73 @@
             self.bulk_insert_data(reader)
 
     def load_ndjson_from_dir(self, path: str = 'META', pattern: str = '*.ndjson'):
         """Load all the NDJSON files in the directory into the database."""
         for file_path in pathlib.Path(path).glob(pattern):
             self.load_from_ndjson_file(file_path)
 
+    @lru_cache(maxsize=None)
     def patient_everything(self, patient_id) -> Generator[dict, None, None]:
         """Return all the resources for a patient."""
         cursor = self.connection.cursor()
-        cursor.execute("SELECT * FROM resources WHERE json_extract(resource, '$.subject.reference') = ?",
+        cursor.execute("SELECT * FROM resources WHERE key = ?",
                        (f"Patient/{patient_id}",))
 
         for _ in cursor.fetchall():
             key, resource_type, resource = _
             yield json.loads(resource)
 
+    @lru_cache(maxsize=None)
     def patient(self, patient_id) -> dict:
         """Return the patient resource."""
         cursor = self.connection.cursor()
-        cursor.execute("SELECT * FROM resources WHERE json_extract(resource, '$.id') = ?", (patient_id,))
+        cursor.execute("SELECT * FROM resources WHERE key = ?", (f"Patient/{patient_id}",))
         key, resource_type, resource = cursor.fetchone()
         return json.loads(resource)
 
-    def flattened_procedure(self) -> Generator[dict, None, None]:
+    @lru_cache(maxsize=None)
+    def flattened_procedure(self, procedure_key) -> dict:
+        """Return the procedure with everything resolved."""
+        cursor = self.connection.cursor()
+        cursor.execute("SELECT * FROM resources WHERE key = ?", (procedure_key,))
+        key, resource_type, resource = cursor.fetchone()
+        procedure = json.loads(resource)
+
+        # simplify the identifier
+        procedure['identifier'] = procedure['identifier'][0]['value']
+        # simplify the code
+        procedure['code'] = procedure['code']['coding'][0]['display']
+        # simplify the reason
+        procedure['reason'] = procedure['reason'][0]['reference']['reference']
+        # simplify the occurrenceAge
+        procedure['occurrenceAge'] = procedure['occurrenceAge']['value']
+        # simplify the subject
+        subject = procedure['subject']['reference']
+        procedure['subject'] = subject
+        return procedure
+
+    @lru_cache(maxsize=None)
+    def flattened_condition(self, condition_key) -> dict:
+        """Return the procedure with everything resolved."""
+        cursor = self.connection.cursor()
+        cursor.execute("SELECT * FROM resources WHERE key = ?", (condition_key,))
+        key, resource_type, resource = cursor.fetchone()
+        condition = json.loads(resource)
+
+        # simplify the identifier
+        condition['identifier'] = condition['identifier'][0]['value']
+        # simplify the code
+        condition['code'] = condition['code']['coding'][0]['display']
+        for coding_normalized, coding_source in normalize_coding(condition):
+            condition[coding_source] = coding_normalized
+        # simplify the onsetAge
+        condition['onsetAge'] = condition['onsetAge']['value']
+        return condition
+
+    def flattened_procedures(self) -> Generator[dict, None, None]:
         """Return all the procedures with everything resolved"""
         loaded_db = self
         connection = sqlite3.connect(loaded_db.db_name)
         cursor = connection.cursor()
         cursor.execute("SELECT * FROM resources where resource_type = ?", ("Procedure",))
 
         for _ in cursor.fetchall():
@@ -210,34 +253,102 @@
                         procedure[resource_type] = []
                     procedure[resource_type].append(resource)
 
             yield procedure
 
         connection.close()
 
-    def flattened_document_reference(self) -> Generator[dict, None, None]:
+    def flattened_observations(self) -> Generator[dict, None, None]:
+        loaded_db = self
+        connection = sqlite3.connect(loaded_db.db_name)
+        cursor = connection.cursor()
+        cursor.execute("SELECT * FROM resources where resource_type = ?", ("Observation",))
+        for _ in tqdm(cursor.fetchall()):
+            key, resource_type, observation_str = _
+            observation = json.loads(observation_str)
+
+            # simplify the subject
+            subject = observation['subject']['reference']
+            observation['subject'] = subject
+
+            # simplify the identifier
+            observation['identifier'] = observation.get('identifier', [{'value': None}])[0]['value']
+
+            # simplify the value
+            value_normalized, value_source = normalize_value(observation)
+            observation['value_normalized'] = value_normalized
+            value_numeric = observation['value_normalized'].split(' ')[0]
+
+            if is_number(value_numeric):
+                observation['value_numeric'] = float(value_numeric)
+            else:
+                observation['value_numeric'] = None
+
+            del observation[value_source]
+
+            # simplify extensions
+            for _ in observation.get('extension', []):
+                value_normalized, value_source = normalize_value(_)
+                observation[_['url'].split('/')[-1]] = value_normalized
+
+            if subject.startswith('Patient/'):
+                _, patient_id = subject.split('/')
+                resource = loaded_db.patient(patient_id)
+                observation['patient'] = resource['identifier'][0]['value']
+                # TODO - add more patient details
+
+            if observation.get('focus'):
+                focus = observation['focus']
+                for f in focus:
+                    if f['reference'].startswith('Procedure/'):
+                        p = self.flattened_procedure(f['reference'])
+                        for k, v in p.items():
+                            if k in ['id', 'subject', 'resourceType']:
+                                continue
+                            observation[f"procedure_{k}"] = v
+                        if "procedure_reason" in observation:
+                            c = self.flattened_condition(observation["procedure_reason"])
+                            for k, v in c.items():
+                                if k in ['id', 'subject', 'resourceType']:
+                                    continue
+                                observation[f"condition_{k}"] = v
+                            del observation["procedure_reason"]
+
+                        del observation['focus']
+                        break
+
+
+            for coding_normalized, coding_source in normalize_coding(observation):
+                observation[coding_source] = coding_normalized
+
+            yield observation
+
+        connection.close()
+
+    def flattened_document_references(self) -> Generator[dict, None, None]:
         loaded_db = self
         connection = sqlite3.connect(loaded_db.db_name)
         cursor = connection.cursor()
         cursor.execute("SELECT * FROM resources where resource_type = ?", ("DocumentReference",))
 
         for _ in cursor.fetchall():
             key, resource_type, procedure = _
             document_reference = json.loads(procedure)
 
             # simplify the subject
             subject = document_reference['subject']['reference']
             document_reference['subject'] = subject
 
             # simplify the identifier
-            document_reference['identifier'] = document_reference['identifier'][0]['value']
+            document_reference['identifier'] = document_reference.get('identifier', [{'value': None}])[0]['value']
 
             # simplify the extensions
             for _ in document_reference['content'][0]['attachment']['extension']:
-                document_reference[_['url'].split('/')[-1]] = _.get('valueString') or _.get('valueUrl')
+                value_normalized, value_source = normalize_value(_)
+                document_reference[_['url'].split('/')[-1]] = value_normalized
 
             for k, v in document_reference['content'][0]['attachment'].items():
                 if k in ['extension']:
                     continue
                 document_reference[k] = v
 
             if subject.startswith('Patient/'):
@@ -258,24 +369,15 @@
                         # must be focus
                         if f"Procedure/{procedure['id']}" not in [_['reference'] for _ in resource['focus']]:
                             continue
 
                         # TODO - pick first coding, h2 allow user to specify preferred coding
                         code = resource['code']['coding'][0]['code']
 
-                        if 'valueQuantity' in resource:
-                            value = resource['valueQuantity']['value']
-                        elif 'valueCodeableConcept' in resource:
-                            value = resource['valueCodeableConcept']['text']
-                        elif 'valueInteger' in resource:
-                            value = resource['valueInteger']
-                        elif 'valueString' in resource:
-                            value = resource['valueString']
-                        else:
-                            value = None
+                        value = normalize_value(resource)
 
                         assert value is not None, f"no value for {resource['id']}"
                         document_reference[code] = value
 
                         continue
 
                     # skip these
@@ -290,31 +392,130 @@
 
             del document_reference['content']
             yield document_reference
 
         connection.close()
 
 
-def create_dataframe(directory_path: str, work_path: str) -> pd.DataFrame:
+def create_dataframe(directory_path: str, work_path: str, data_type:str) -> pd.DataFrame:
     """Create a dataframe from the FHIR data in the directory."""
     assert pathlib.Path(work_path).exists(), f"Directory {work_path} does not exist."
     work_path = pathlib.Path(work_path)
     db_path = (work_path / "local_fhir.db")
     db_path.unlink(missing_ok=True)
 
     db = LocalFHIRDatabase(db_name=db_path)
     db.load_ndjson_from_dir(path=directory_path)
 
-    df = pd.DataFrame(db.flattened_document_reference())
+    if data_type == "DocumentReference":
+        df = pd.DataFrame(db.flattened_document_reference())
+    elif data_type == "Observation":
+        df = pd.DataFrame(db.flattened_observations())
+    else:
+        raise ValueError(f"{data_type} not supported yet. Supported data types are DocumentReference and Observation")
+    assert not df.empty, "Dataframe is empty, are there any DocumentReference resources?"
+
     front_column_names = ["resourceType", "identifier"]
     if "patient" in df.columns:
         front_column_names = front_column_names + ["patient"]
+
     remaining_columns = [col for col in df.columns if col not in front_column_names]
     rear_column_names = ["status", "id"]
     if "subject" in df.columns:
         rear_column_names = rear_column_names + ["subject"]
+    for c in df.columns:
+        if c.endswith("_identifier"):
+            rear_column_names.append(c)
     remaining_columns = [col for col in remaining_columns if col not in rear_column_names]
 
     reordered_columns = front_column_names + remaining_columns + rear_column_names
     df = df[reordered_columns]
     df = df.replace({np.nan: ''})
     return df
+
+
+def normalize_value(resource_dict: dict) -> tuple[Optional[str], Optional[str]]:
+    """return a tuple containing the normalized value and the name of the field it was derived from"""
+    value_normalized = None
+    value_source = None
+
+    if 'valueQuantity' in resource_dict:
+        value = resource_dict['valueQuantity']
+        value_normalized = f"{value['value']} {value.get('unit', '')}"
+        value_source = 'valueQuantity'
+    elif 'valueCodeableConcept' in resource_dict:
+        value = resource_dict['valueCodeableConcept']
+        value_normalized = ' '.join([coding['display'] for coding in value.get('coding', [])])
+        value_source = 'valueCodeableConcept'
+    elif 'valueString' in resource_dict:
+        value_normalized = resource_dict['valueString']
+        value_source = 'valueString'
+    elif 'valueBoolean' in resource_dict:
+        value_normalized = str(resource_dict['valueBoolean'])
+        value_source = 'valueBoolean'
+    elif 'valueInteger' in resource_dict:
+        value_normalized = str(resource_dict['valueInteger'])
+        value_source = 'valueInteger'
+    elif 'valueRange' in resource_dict:
+        value = resource_dict['valueRange']
+        low = value['low']
+        high = value['high']
+        value_normalized = f"{low['value']} - {high['value']} {low.get('unit', '')}"
+        value_source = 'valueRange'
+    elif 'valueRatio' in resource_dict:
+        value = resource_dict['valueRatio']
+        numerator = value['numerator']
+        denominator = value['denominator']
+        value_normalized = f"{numerator['value']} {numerator.get('unit', '')}/{denominator['value']} {denominator.get('unit', '')}"
+        value_source = 'valueRatio'
+    elif 'valueSampledData' in resource_dict:
+        value = resource_dict['valueSampledData']
+        value_normalized = value['data']
+        value_source = 'valueSampledData'
+    elif 'valueTime' in resource_dict:
+        value_normalized = resource_dict['valueTime']
+        value_source = 'valueTime'
+    elif 'valueDateTime' in resource_dict:
+        value_normalized = resource_dict['valueDateTime']
+        value_source = 'valueDateTime'
+    elif 'valuePeriod' in resource_dict:
+        value = resource_dict['valuePeriod']
+        value_normalized = f"{value['start']} to {value['end']}"
+        value_source = 'valuePeriod'
+
+    return value_normalized, value_source
+
+
+def normalize_coding(resource_dict: dict) -> List[Tuple[str, str]]:
+    def extract_coding(coding_list):
+        return ' '.join([coding.get('display', '') for coding in coding_list if 'display' in coding])
+
+    def find_codings_in_dict(d: dict, parent_key: str = '') -> List[Tuple[str, str]]:
+        codings = []
+        for key, value in d.items():
+            if isinstance(value, list):
+                for item in value:
+                    if isinstance(item, dict):
+                        # Check if the dict contains a 'coding' list
+                        if 'coding' in item and isinstance(item['coding'], list):
+                            coding_string = extract_coding(item['coding'])
+                            codings.append((coding_string, key))
+                        # Recursively search in the dict
+                        codings.extend(find_codings_in_dict(item, key))
+            elif isinstance(value, dict):
+                # Check if the dict contains a 'coding' list
+                if 'coding' in value and isinstance(value['coding'], list):
+                    coding_string = extract_coding(value['coding'])
+                    codings.append((coding_string, key))
+                # Recursively search in the dict
+                codings.extend(find_codings_in_dict(value, key))
+        return codings
+
+    return find_codings_in_dict(resource_dict)
+
+def is_number(s):
+    """ Returns True if string is a number. """
+    try:
+        complex(s)
+        return True
+    except ValueError:
+        return False
```

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/meta/skeleton.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/meta/skeleton.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pathlib
+import uuid
 from datetime import datetime, UTC
 
 import orjson
 from fhir.resources.attachment import Attachment
 from fhir.resources.bundle import Bundle, BundleEntry, BundleEntryRequest
 from fhir.resources.documentreference import DocumentReference
 from fhir.resources.fhirtypes import DocumentReferenceContentType
@@ -12,14 +13,15 @@
 from fhir.resources.patient import Patient
 from fhir.resources.researchstudy import ResearchStudy
 from fhir.resources.researchsubject import ResearchSubject
 from fhir.resources.resource import Resource
 from fhir.resources.specimen import Specimen
 from fhir.resources.task import Task, TaskOutput, TaskInput
 
+from gen3_tracker import ACED_NAMESPACE
 from gen3_tracker.common import create_id, EmitterContextManager
 from gen3_tracker.git import DVC, run_command, dvc_data
 
 
 def _get_system(identifier: str, project_id: str):
     """Return system component of simplified identifier"""
     if '#' in identifier:
@@ -40,14 +42,17 @@
             for line in f:
                 record = orjson.loads(line)
                 _id = record.get('id')
                 resource_type = record.get('resourceType')
                 if resource_type == 'Bundle':
                     continue
                 official_identifier = next((identifier.get('value') for identifier in record.get('identifier', []) if identifier.get('use') == 'official'), None)
+                if not official_identifier and record.get('identifier'):
+                    official_identifier = record['identifier'][0]['value']
+
                 if _id and official_identifier:
                     id_dict[f"{resource_type}/{_id}"] = official_identifier
 
     return id_dict
 
 
 def update_document_reference(document_reference: DocumentReference, dvc_data: DVC):
@@ -85,90 +90,133 @@
     attachment.creation = dvc_data.out.modified
 
     content = DocumentReferenceContentType(attachment=attachment)
 
     document_reference.content = [content]
 
 
-def create_skeleton(dvc: dict, project_id: str) -> list[Resource]:
+def create_id_from_strings(resource_type: str, project_id: str, identifier_string: str) -> str:
+    """Create an id from strings."""
+    if not identifier_string:
+        return None
+    # cbds-smmart_labkey_demo/Specimen/https://aced-idp.org/cbds-smmart_labkey_demo|0000321955
+    # cbds-smmart_labkey_demo/Specimen/https://aced-idp.org/cbds-smmart_labkey_demo|0000321955
+    print(f"{project_id}/{resource_type}/{_get_system(identifier_string, project_id)}|{identifier_string}")
+    return str(uuid.uuid5(ACED_NAMESPACE, f"{project_id}/{resource_type}/{_get_system(identifier_string, project_id)}|{identifier_string}"))
+
+
+def create_skeleton(dvc: dict, project_id: str, meta_index: set[str] = []) -> list[Resource]:
     """
     Create a skeleton graph for document and ancestors from a set of identifiers.
     """
     dvc = DVC.model_validate(dvc)
 
     specimen_identifier = dvc.meta.specimen
     patient_identifier = dvc.meta.patient
     task_identifier = dvc.meta.task
     observation_identifier = dvc.meta.observation
     project_id = dvc.project_id or project_id
+
     assert dvc.out, f"out required {dvc}"
     document_reference_id = dvc.out.set_object_id(project_id=project_id)
 
     assert project_id, "project_id required"
     assert project_id.count('-') == 1, "project_id must be of the form program-project"
     program, project = project_id.split('-')
 
-    # create entities
-    research_study = research_subject = observation = specimen = patient = task = None
+    research_study = research_subject = observation = specimen = patient = task = document_reference = None
 
-    research_study = ResearchStudy(status='active')
-    research_study.description = f"Skeleton ResearchStudy for {project_id}"
-    research_study.identifier = [
-        Identifier(value=project_id, system=_get_system(project_id, project_id=project_id),
-                   use='official')]
-    research_study.id = create_id(research_study, project_id)
-    research_study_id = research_study.id
+    # check if we have already created the resources
+
+    research_study_id = create_id_from_strings(resource_type='ResearchStudy', project_id=project_id, identifier_string=project_id)
+    specimen_id = create_id_from_strings(resource_type='Specimen', project_id=project_id, identifier_string=specimen_identifier)
+    patient_id = create_id_from_strings(resource_type='Patient', project_id=project_id, identifier_string=patient_identifier)
+    task_id = create_id_from_strings(resource_type='Task', project_id=project_id, identifier_string=task_identifier)
+    observation_id = create_id_from_strings(resource_type='Observation', project_id=project_id, identifier_string=observation_identifier)
+
+    _ = f'ResearchStudy/{research_study_id}'
+    if _ in meta_index:
+        research_study = meta_index[_]
+    _ = f'Specimen/{specimen_id}'
+    if _ in meta_index:
+        specimen = meta_index[_]
+    _ = f'Patient/{patient_id}'
+    if _ in meta_index:
+        patient = meta_index[_]
+    _ = f'Task/{task_id}'
+    if _ in meta_index:
+        task = meta_index[_]
+    _ = f'Observation/{observation_id}'
+    if _ in meta_index:
+        observation = meta_index[_]
+
+    # create entities
 
     document_reference = DocumentReference(status='current', content=[{'attachment': {'url': "file://"}}])
     document_reference.id = document_reference_id
     document_reference.identifier = [
         Identifier(value=document_reference_id, system=_get_system(document_reference_id, project_id=project_id),
                    use='official')]
     update_document_reference(document_reference, dvc)
 
-    if patient_identifier:
+    if not research_study:
+        research_study = ResearchStudy(status='active')
+        research_study.description = f"Skeleton ResearchStudy for {project_id}"
+        research_study.identifier = [
+            Identifier(value=project_id, system=_get_system(project_id, project_id=project_id),
+                       use='official')]
+        research_study.id = create_id(research_study, project_id)
+
+    if not patient and patient_identifier:
         patient = Patient()
         patient.identifier = [Identifier(value=patient_identifier, system=_get_system(patient_identifier, project_id=project_id), use='official')]
         patient.id = create_id(patient, project_id)
 
         research_subject = ResearchSubject(
             status='active',
             study={'reference': f"ResearchStudy/{research_study_id}"},
             subject={'reference': f"Patient/{patient.id}"}
         )
         research_subject.identifier = [Identifier(value=patient_identifier, system=_get_system(patient_identifier, project_id=project_id), use='official')]
         research_subject.id = create_id(research_subject, project_id)
 
-    if observation_identifier:
-        assert patient, "patient required for observation"
+    if not observation and observation_identifier:
         observation = Observation(status='final', code={'text': 'unknown'})
         observation.identifier = [Identifier(value=observation_identifier, system=_get_system(observation_identifier, project_id=project_id), use='official')]
-        observation.subject = {'reference': f"Patient/{patient.id}"}
         observation.id = create_id(observation, project_id)
 
-    if specimen_identifier:
+        assert patient, "patient required for observation"
+        observation.subject = {'reference': f"Patient/{patient.id}"}
+        patient_id = patient.id
+
+    if not specimen and specimen_identifier:
+        print(f'{specimen_identifier} Specimen/{specimen_id} not in {[(k, _) for k, _ in meta_index.items() if k.startswith("Specimen")]}')
+        exit(1)
         specimen = Specimen()
         specimen.identifier = [Identifier(value=specimen_identifier, system=_get_system(specimen_identifier, project_id=project_id), use='official')]
         specimen.id = create_id(specimen, project_id)
+        specimen_id = specimen.id
+
         assert patient, "patient required for specimen"
         specimen.subject = {'reference': f"Patient/{patient.id}"}
 
-    if task_identifier:
+    if not task and task_identifier:
         task = Task(intent='unknown', status='completed')
         task.identifier = [Identifier(value=task_identifier, system=_get_system(task_identifier, project_id=project_id),
                                       use='official')]
         task.id = create_id(task, project_id)
+        task_id = task.id
 
     # create relationships
 
     # assign subject, specimen of observation
     if observation and specimen and not observation.specimen:
-        observation.specimen = {'reference': f"Specimen/{specimen.id}"}
+        observation.specimen = {'reference': f"Specimen/{specimen_id}"}
     if observation and patient and not observation.subject:
-        observation.subject = {'reference': f"Patient/{patient.id}"}
+        observation.subject = {'reference': f"Patient/{patient_id}"}
 
     if task:
         task.input = []
         if specimen:
             task.input.append(
                 TaskInput(
                     valueReference={"reference": f"Specimen/{specimen.id}"},
@@ -186,23 +234,23 @@
             TaskOutput(
                 valueReference={'reference': f"DocumentReference/{document_reference.id}"},
                 type={'text': 'DocumentReference'})
         ]
 
     # assign document reference subject
     if observation:
-        document_reference.subject = {'reference': f"Observation/{observation.id}"}
+        document_reference.subject = {'reference': f"Observation/{observation_id}"}
     if specimen and not document_reference.subject:
-        document_reference.subject = {'reference': f"Specimen/{specimen.id}"}
+        document_reference.subject = {'reference': f"Specimen/{specimen_id}"}
     if patient and not document_reference.subject:
-        document_reference.subject = {'reference': f"Patient/{patient.id}"}
+        document_reference.subject = {'reference': f"Patient/{patient_id}"}
     if not document_reference.subject:
-        document_reference.subject = {'reference': f"ResearchStudy/{research_study.id}"}
+        document_reference.subject = {'reference': f"ResearchStudy/{research_study_id}"}
 
-    return [_ for _ in [research_study, research_subject, patient, observation, specimen, task, document_reference] if _]
+    return [_ for _ in [research_study, research_subject, patient, observation, specimen, task, document_reference] if _ and not isinstance(_, str)]
 
 
 def update_meta_files(dry_run=False, project_id=None) -> list[str]:
     """Maintain the META directory."""
     assert project_id, "project_id required"
     manifest_path = pathlib.Path('MANIFEST')
     dvc_files = [_ for _ in manifest_path.rglob('*.dvc')]
@@ -213,15 +261,15 @@
     before_meta_files = [_ for _ in pathlib.Path('META').glob('*.ndjson')]
     before_meta_index = set(list(meta_index().keys()))
 
     emitted_already = []
 
     with EmitterContextManager('META') as emitter:
         for _ in dvc_data(dvc_files):
-            resources = create_skeleton(_, project_id)
+            resources = create_skeleton(_, project_id, meta_index())
             for resource in resources:
                 key = f"{resource.resource_type}/{resource.id}"
                 if key not in emitted_already:
                     emitter.emit(resource.resource_type).write(
                         resource.json(option=orjson.OPT_APPEND_NEWLINE)
                     )
                     emitted_already.append(f"{resource.resource_type}/{resource.id}")
```

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/meta/validator.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/meta/visualizer.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/meta/visualizer.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/projects/__init__.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/projects/cli.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/projects/lister.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker/projects/remover.py` & `gen3_tracker-0.0.4rc6/gen3_tracker/projects/remover.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker.egg-info/PKG-INFO` & `gen3_tracker-0.0.4rc6/gen3_tracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3-tracker
-Version: 0.0.4rc5
+Version: 0.0.4rc6
 Summary: A CLI for adding version control to Gen3 data submission projects.
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: walsbr
 Author-email: walsbr@ohsu.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
```

### Comparing `gen3_tracker-0.0.4rc5/gen3_tracker.egg-info/SOURCES.txt` & `gen3_tracker-0.0.4rc6/gen3_tracker.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 LICENSE
 README.md
 setup.py
 gen3_tracker/__init__.py
 gen3_tracker/cli.py
+gen3_tracker/config.yaml
 gen3_tracker.egg-info/PKG-INFO
 gen3_tracker.egg-info/SOURCES.txt
 gen3_tracker.egg-info/dependency_links.txt
 gen3_tracker.egg-info/entry_points.txt
 gen3_tracker.egg-info/requires.txt
 gen3_tracker.egg-info/top_level.txt
 gen3_tracker/collaborator/__init__.py
 gen3_tracker/collaborator/cli.py
 gen3_tracker/collaborator/access/__init__.py
 gen3_tracker/collaborator/access/cli.py
 gen3_tracker/collaborator/access/requestor.py
 gen3_tracker/collaborator/access/submitter.py
 gen3_tracker/collaborator/access/policies/__init__.py
+gen3_tracker/collaborator/access/policies/add-project-default.yaml
+gen3_tracker/collaborator/access/policies/add-user-read.yaml
+gen3_tracker/collaborator/access/policies/add-user-write.yaml
 gen3_tracker/common/__init__.py
 gen3_tracker/config/__init__.py
 gen3_tracker/gen3/__init__.py
 gen3_tracker/gen3/indexd.py
 gen3_tracker/gen3/jobs.py
 gen3_tracker/gen3/buckets/__init__.py
 gen3_tracker/gen3/buckets/cli.py
```

### Comparing `gen3_tracker-0.0.4rc5/setup.py` & `gen3_tracker-0.0.4rc6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,27 @@
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 
 setup(
     name='gen3_tracker',
-    version='0.0.4rc5',
+    version='0.0.4rc6',
     description='A CLI for adding version control to Gen3 data submission projects.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='walsbr',
     author_email='walsbr@ohsu.edu',
     url='https://github.com/ACED-IDP/gen3_util',
     packages=find_packages(exclude=['tests', 'tests.*']),
     install_requires=requirements,
+    include_package_data=True,
+    package_data={  # Optional
+        '': ['*.yaml'],
+    },
     extras_require={
         'dtale': ['dtale'],
     },
     entry_points={
         'console_scripts': [
             'g3t=gen3_tracker.cli:cli',
         ],
```

### Comparing `gen3_tracker-0.0.4rc5/tests/integration/__init__.py` & `gen3_tracker-0.0.4rc6/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/tests/integration/test_bucket_import.py` & `gen3_tracker-0.0.4rc6/tests/integration/test_bucket_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     for _ in ['bucket', 'committed', 'uncommitted']:
         assert _ in listing
 
     # files should appear in uncommitted
     assert len(listing['uncommitted']) == len(SHOULD_SUCCEED)
 
     # commit the changes
-    run(runner, ["--debug", "commit", "-am", "\"initial commit\""])
+    run(runner, ["--debug", "commit", "-am", "initial commit"])
 
     # test the ls command, should now be in committed
     result = run(runner, ["--debug", "--format", "json",  "ls"])
     listing = json.loads(result.stdout)
     assert len(listing['committed']) == len(SHOULD_SUCCEED)
 
     # test the ls filter
```

### Comparing `gen3_tracker-0.0.4rc5/tests/integration/test_bundle.py` & `gen3_tracker-0.0.4rc6/tests/integration/test_bundle.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/tests/integration/test_end_to_end_workflow.py` & `gen3_tracker-0.0.4rc6/tests/integration/test_end_to_end_workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import pathlib
 
 import yaml
 from click.testing import CliRunner
 
 from gen3_tracker.config import ensure_auth, default
-from gen3_tracker.git import DVC
+from gen3_tracker.git import DVC, run_command
 from tests.integration import run, validate_document_in_psql_graph, validate_document_in_elastic
 
 
 def test_simple_workflow(runner: CliRunner, project_id, tmpdir) -> None:
     """Test the init command."""
     # change to the temporary directory
     assert tmpdir.chdir()
@@ -43,15 +43,15 @@
     dvc.project_id = project_id
     object_id = dvc.object_id
 
     # create the meta file
     run(runner, ["--debug", "meta", "init"], expected_files=["META/DocumentReference.ndjson"])
 
     # commit the changes, delegating to git
-    run(runner, ["--debug", "commit", "-am", "\"initial commit\""])
+    run(runner, ["--debug", "commit", "-am", "initial commit"])
 
     # validate the meta files
     run(runner, ["--debug", "meta", "validate"])
 
     # create a visualisation
     run(runner, ["--debug", "meta", "graph"], expected_files=["meta.html"])
 
@@ -76,15 +76,16 @@
     os.chdir("clone")
 
     # clone the project
     run(runner, ["--debug", "clone", project_id])
     # pull the data
     run(runner, ["--debug", "pull"])
     # check the files exist in the cloned directory
-    assert pathlib.Path("my-project-data/hello.txt").exists()
+    run_command("ls -l")
+    assert pathlib.Path("my-project-data/hello.txt").exists(), "hello.txt does not exist in the cloned directory."
 
     # remove the project from the server.
     # TODO note, this does not remove the files from the bucket (UChicago bug)
     # See https://ohsucomputationalbio.slack.com/archives/C043HPV0VMY/p1714065633867229
     run(runner, ["--debug", "projects", "empty", "--project_id", project_id, "--confirm", "empty"])
     run(runner, ["--debug", "projects", "rm", "--project_id", project_id])
```

### Comparing `gen3_tracker-0.0.4rc5/tests/unit/test_flatten_fhir_example.py` & `gen3_tracker-0.0.4rc6/tests/unit/test_flatten_fhir_example.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/tests/unit/test_hash_types.py` & `gen3_tracker-0.0.4rc6/tests/unit/test_hash_types.py`

 * *Files identical despite different names*

### Comparing `gen3_tracker-0.0.4rc5/tests/unit/test_read_dvc.py` & `gen3_tracker-0.0.4rc6/tests/unit/test_read_dvc.py`

 * *Files identical despite different names*

