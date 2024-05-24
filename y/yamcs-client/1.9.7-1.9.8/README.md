# Comparing `tmp/yamcs_client-1.9.7.tar.gz` & `tmp/yamcs_client-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamcs_client-1.9.7.tar", last modified: Fri May 10 14:29:46 2024, max compression
+gzip compressed data, was "yamcs_client-1.9.8.tar", last modified: Fri May 24 08:03:53 2024, max compression
```

## Comparing `yamcs_client-1.9.7.tar` & `yamcs_client-1.9.8.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.689078 yamcs_client-1.9.7/
--rw-r--r--   0 fdi        (503) staff       (20)     7652 2018-08-10 14:47:21.000000 yamcs_client-1.9.7/LICENSE
--rw-r--r--   0 fdi        (503) staff       (20)       34 2020-03-04 12:26:47.000000 yamcs_client-1.9.7/MANIFEST.in
--rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-05-10 14:29:46.688716 yamcs_client-1.9.7/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)      578 2020-06-18 07:14:03.000000 yamcs_client-1.9.7/README.md
--rw-r--r--   0 fdi        (503) staff       (20)       38 2024-05-10 14:29:46.689148 yamcs_client-1.9.7/setup.cfg
--rw-r--r--   0 fdi        (503) staff       (20)     1730 2023-11-03 10:38:04.000000 yamcs_client-1.9.7/setup.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.615717 yamcs_client-1.9.7/src/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.617446 yamcs_client-1.9.7/src/yamcs/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.619476 yamcs_client-1.9.7/src/yamcs/api/
--rw-r--r--   0 fdi        (503) staff       (20)    13519 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/api/annotations_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)     3573 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/api/exception_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)     5033 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/api/httpbody_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    13148 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/api/websocket_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.620478 yamcs_client-1.9.7/src/yamcs/archive/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/archive/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    46715 2024-04-17 19:59:36.000000 yamcs_client-1.9.7/src/yamcs/archive/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     8466 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/archive/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.621283 yamcs_client-1.9.7/src/yamcs/client/
--rw-r--r--   0 fdi        (503) staff       (20)     1495 2024-03-04 11:15:08.000000 yamcs_client-1.9.7/src/yamcs/client/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     5326 2024-03-18 13:20:14.000000 yamcs_client-1.9.7/src/yamcs/client/activities.py
--rw-r--r--   0 fdi        (503) staff       (20)    24601 2024-05-10 10:26:26.000000 yamcs_client-1.9.7/src/yamcs/client/core.py
--rw-r--r--   0 fdi        (503) staff       (20)       22 2024-05-10 14:25:31.000000 yamcs_client-1.9.7/src/yamcs/clientversion.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.623912 yamcs_client-1.9.7/src/yamcs/core/
--rw-r--r--   0 fdi        (503) staff       (20)       28 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/core/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     7290 2024-05-10 10:20:44.000000 yamcs_client-1.9.7/src/yamcs/core/auth.py
--rw-r--r--   0 fdi        (503) staff       (20)     5597 2024-05-10 10:20:28.000000 yamcs_client-1.9.7/src/yamcs/core/context.py
--rw-r--r--   0 fdi        (503) staff       (20)      393 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/core/exceptions.py
--rw-r--r--   0 fdi        (503) staff       (20)     4234 2023-04-16 19:38:09.000000 yamcs_client-1.9.7/src/yamcs/core/futures.py
--rw-r--r--   0 fdi        (503) staff       (20)    13731 2024-05-10 08:42:48.000000 yamcs_client-1.9.7/src/yamcs/core/helpers.py
--rw-r--r--   0 fdi        (503) staff       (20)     1611 2023-04-16 20:00:45.000000 yamcs_client-1.9.7/src/yamcs/core/pagination.py
--rw-r--r--   0 fdi        (503) staff       (20)     7817 2024-03-16 08:21:22.000000 yamcs_client-1.9.7/src/yamcs/core/subscriptions.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.624601 yamcs_client-1.9.7/src/yamcs/filetransfer/
--rw-r--r--   0 fdi        (503) staff       (20)       65 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/filetransfer/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    11570 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/filetransfer/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    15610 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/filetransfer/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.625870 yamcs_client-1.9.7/src/yamcs/link/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/link/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     8258 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/link/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     1996 2024-02-24 17:03:41.000000 yamcs_client-1.9.7/src/yamcs/link/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.627040 yamcs_client-1.9.7/src/yamcs/mdb/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/mdb/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    15401 2024-03-01 15:24:22.000000 yamcs_client-1.9.7/src/yamcs/mdb/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    13254 2024-02-24 16:11:30.000000 yamcs_client-1.9.7/src/yamcs/mdb/model.py
--rw-r--r--   0 fdi        (503) staff       (20)    12970 2024-02-24 16:07:18.000000 yamcs_client-1.9.7/src/yamcs/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.627628 yamcs_client-1.9.7/src/yamcs/protobuf/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.628506 yamcs_client-1.9.7/src/yamcs/protobuf/actions/
--rw-r--r--   0 fdi        (503) staff       (20)     4545 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/actions/actions_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.630619 yamcs_client-1.9.7/src/yamcs/protobuf/activities/
--rw-r--r--   0 fdi        (503) staff       (20)    17234 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/activities/activities_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    38288 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/activities/activities_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.632805 yamcs_client-1.9.7/src/yamcs/protobuf/alarms/
--rw-r--r--   0 fdi        (503) staff       (20)    29047 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/alarms/alarms_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    40124 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/alarms/alarms_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.637153 yamcs_client-1.9.7/src/yamcs/protobuf/archive/
--rw-r--r--   0 fdi        (503) staff       (20)    33962 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/archive/archive_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    53220 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/archive/index_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    43577 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    19316 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/archive/rocksdb_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.637886 yamcs_client-1.9.7/src/yamcs/protobuf/audit/
--rw-r--r--   0 fdi        (503) staff       (20)    11973 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/audit/audit_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.638447 yamcs_client-1.9.7/src/yamcs/protobuf/auth/
--rw-r--r--   0 fdi        (503) staff       (20)     8446 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/auth/auth_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.639041 yamcs_client-1.9.7/src/yamcs/protobuf/buckets/
--rw-r--r--   0 fdi        (503) staff       (20)    34808 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/buckets/buckets_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.641223 yamcs_client-1.9.7/src/yamcs/protobuf/commanding/
--rw-r--r--   0 fdi        (503) staff       (20)    12415 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/commanding/clearance_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    41600 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/commanding/commanding_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    47775 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/commanding/commands_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    33253 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/commanding/queues_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.641586 yamcs_client-1.9.7/src/yamcs/protobuf/config/
--rw-r--r--   0 fdi        (503) staff       (20)    17412 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/config/config_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.641942 yamcs_client-1.9.7/src/yamcs/protobuf/cop1/
--rw-r--r--   0 fdi        (503) staff       (20)    34928 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/cop1/cop1_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.642467 yamcs_client-1.9.7/src/yamcs/protobuf/database/
--rw-r--r--   0 fdi        (503) staff       (20)     8255 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/database/database_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.643358 yamcs_client-1.9.7/src/yamcs/protobuf/events/
--rw-r--r--   0 fdi        (503) staff       (20)     9301 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/events/events_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    30677 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/events/events_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.643833 yamcs_client-1.9.7/src/yamcs/protobuf/filetransfer/
--rw-r--r--   0 fdi        (503) staff       (20)    80380 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.644915 yamcs_client-1.9.7/src/yamcs/protobuf/iam/
--rw-r--r--   0 fdi        (503) staff       (20)    73419 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/iam/iam_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    10014 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/iam/sessions_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.646455 yamcs_client-1.9.7/src/yamcs/protobuf/instances/
--rw-r--r--   0 fdi        (503) staff       (20)    19968 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/instances/instances_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    32345 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/instances/instances_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.646837 yamcs_client-1.9.7/src/yamcs/protobuf/links/
--rw-r--r--   0 fdi        (503) staff       (20)    31906 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/links/links_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.647475 yamcs_client-1.9.7/src/yamcs/protobuf/mdb/
--rw-r--r--   0 fdi        (503) staff       (20)   280528 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/mdb/mdb_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.649554 yamcs_client-1.9.7/src/yamcs/protobuf/packets/
--rw-r--r--   0 fdi        (503) staff       (20)     6029 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/packets/packets_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    46220 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/packets/packets_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.650507 yamcs_client-1.9.7/src/yamcs/protobuf/plists/
--rw-r--r--   0 fdi        (503) staff       (20)     4238 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/plists/plists_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    18747 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/plists/plists_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.652751 yamcs_client-1.9.7/src/yamcs/protobuf/processing/
--rw-r--r--   0 fdi        (503) staff       (20)    37572 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/processing/mdb_override_service_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    86589 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/processing/processing_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.654241 yamcs_client-1.9.7/src/yamcs/protobuf/pvalue/
--rw-r--r--   0 fdi        (503) staff       (20)    28924 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/protobuf/pvalue/pvalue_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    10465 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.654797 yamcs_client-1.9.7/src/yamcs/protobuf/replication/
--rw-r--r--   0 fdi        (503) staff       (20)    13030 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/replication/replication_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.655682 yamcs_client-1.9.7/src/yamcs/protobuf/server/
--rw-r--r--   0 fdi        (503) staff       (20)    70072 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/server/server_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.658738 yamcs_client-1.9.7/src/yamcs/protobuf/services/
--rw-r--r--   0 fdi        (503) staff       (20)     6369 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/services/services_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    11946 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/services/services_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.659146 yamcs_client-1.9.7/src/yamcs/protobuf/table/
--rw-r--r--   0 fdi        (503) staff       (20)    68243 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/table/table_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.660399 yamcs_client-1.9.7/src/yamcs/protobuf/tco/
--rw-r--r--   0 fdi        (503) staff       (20)    32749 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/tco/tco_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.660868 yamcs_client-1.9.7/src/yamcs/protobuf/time/
--rw-r--r--   0 fdi        (503) staff       (20)    12958 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/time/time_service_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.661490 yamcs_client-1.9.7/src/yamcs/protobuf/timeline/
--rw-r--r--   0 fdi        (503) staff       (20)   125195 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/timeline/timeline_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.662444 yamcs_client-1.9.7/src/yamcs/protobuf/yamcsManagement/
--rw-r--r--   0 fdi        (503) staff       (20)    32409 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py
--rw-r--r--   0 fdi        (503) staff       (20)    42446 2024-04-17 20:21:54.000000 yamcs_client-1.9.7/src/yamcs/protobuf/yamcs_pb2.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.663953 yamcs_client-1.9.7/src/yamcs/storage/
--rw-r--r--   0 fdi        (503) staff       (20)       55 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/storage/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     5683 2024-03-05 11:43:25.000000 yamcs_client-1.9.7/src/yamcs/storage/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     6439 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/storage/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.664665 yamcs_client-1.9.7/src/yamcs/tco/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/tco/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     4867 2024-02-24 17:10:21.000000 yamcs_client-1.9.7/src/yamcs/tco/client.py
--rw-r--r--   0 fdi        (503) staff       (20)     3089 2024-02-24 17:11:07.000000 yamcs_client-1.9.7/src/yamcs/tco/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.665380 yamcs_client-1.9.7/src/yamcs/timeline/
--rw-r--r--   0 fdi        (503) staff       (20)       57 2022-05-30 08:31:08.000000 yamcs_client-1.9.7/src/yamcs/timeline/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     7923 2024-03-05 11:01:12.000000 yamcs_client-1.9.7/src/yamcs/timeline/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    16141 2024-03-05 10:37:49.000000 yamcs_client-1.9.7/src/yamcs/timeline/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.666715 yamcs_client-1.9.7/src/yamcs/tmtc/
--rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.7/src/yamcs/tmtc/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)    51419 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/tmtc/client.py
--rw-r--r--   0 fdi        (503) staff       (20)    35330 2024-04-18 19:05:56.000000 yamcs_client-1.9.7/src/yamcs/tmtc/model.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-10 14:29:46.688250 yamcs_client-1.9.7/src/yamcs_client.egg-info/
--rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-05-10 14:29:46.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)     3504 2024-05-10 14:29:46.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/SOURCES.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2024-05-10 14:29:46.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/dependency_links.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2022-04-07 19:46:24.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/not-zip-safe
--rw-r--r--   0 fdi        (503) staff       (20)       55 2024-05-10 14:29:46.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/requires.txt
--rw-r--r--   0 fdi        (503) staff       (20)        6 2024-05-10 14:29:46.000000 yamcs_client-1.9.7/src/yamcs_client.egg-info/top_level.txt
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.228873 yamcs_client-1.9.8/
+-rw-r--r--   0 fdi        (503) staff       (20)     7652 2018-08-10 14:47:21.000000 yamcs_client-1.9.8/LICENSE
+-rw-r--r--   0 fdi        (503) staff       (20)       34 2020-03-04 12:26:47.000000 yamcs_client-1.9.8/MANIFEST.in
+-rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-05-24 08:03:53.228548 yamcs_client-1.9.8/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)      578 2020-06-18 07:14:03.000000 yamcs_client-1.9.8/README.md
+-rw-r--r--   0 fdi        (503) staff       (20)       38 2024-05-24 08:03:53.228932 yamcs_client-1.9.8/setup.cfg
+-rw-r--r--   0 fdi        (503) staff       (20)     1730 2023-11-03 10:38:04.000000 yamcs_client-1.9.8/setup.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.150536 yamcs_client-1.9.8/src/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.152501 yamcs_client-1.9.8/src/yamcs/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.153989 yamcs_client-1.9.8/src/yamcs/api/
+-rw-r--r--   0 fdi        (503) staff       (20)    13519 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/api/annotations_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)     3573 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/api/exception_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5033 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/api/httpbody_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13148 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/api/websocket_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.154763 yamcs_client-1.9.8/src/yamcs/archive/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.8/src/yamcs/archive/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    46715 2024-05-24 07:55:12.000000 yamcs_client-1.9.8/src/yamcs/archive/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8466 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/archive/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.155840 yamcs_client-1.9.8/src/yamcs/client/
+-rw-r--r--   0 fdi        (503) staff       (20)     1495 2024-03-04 11:15:08.000000 yamcs_client-1.9.8/src/yamcs/client/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5326 2024-03-18 13:20:14.000000 yamcs_client-1.9.8/src/yamcs/client/activities.py
+-rw-r--r--   0 fdi        (503) staff       (20)    25809 2024-05-24 07:03:32.000000 yamcs_client-1.9.8/src/yamcs/client/core.py
+-rw-r--r--   0 fdi        (503) staff       (20)       22 2024-05-24 07:49:31.000000 yamcs_client-1.9.8/src/yamcs/clientversion.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.159843 yamcs_client-1.9.8/src/yamcs/core/
+-rw-r--r--   0 fdi        (503) staff       (20)       28 2022-04-07 19:17:50.000000 yamcs_client-1.9.8/src/yamcs/core/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7290 2024-05-10 10:20:44.000000 yamcs_client-1.9.8/src/yamcs/core/auth.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5597 2024-05-13 19:01:09.000000 yamcs_client-1.9.8/src/yamcs/core/context.py
+-rw-r--r--   0 fdi        (503) staff       (20)      393 2022-04-07 19:17:50.000000 yamcs_client-1.9.8/src/yamcs/core/exceptions.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4234 2023-04-16 19:38:09.000000 yamcs_client-1.9.8/src/yamcs/core/futures.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13731 2024-05-10 08:42:48.000000 yamcs_client-1.9.8/src/yamcs/core/helpers.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1611 2023-04-16 20:00:45.000000 yamcs_client-1.9.8/src/yamcs/core/pagination.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7817 2024-03-16 08:21:22.000000 yamcs_client-1.9.8/src/yamcs/core/subscriptions.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.162450 yamcs_client-1.9.8/src/yamcs/filetransfer/
+-rw-r--r--   0 fdi        (503) staff       (20)       65 2022-04-07 19:17:50.000000 yamcs_client-1.9.8/src/yamcs/filetransfer/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    11570 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/filetransfer/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    15610 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/filetransfer/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.163726 yamcs_client-1.9.8/src/yamcs/link/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.8/src/yamcs/link/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8258 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/link/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1996 2024-02-24 17:03:41.000000 yamcs_client-1.9.8/src/yamcs/link/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.165152 yamcs_client-1.9.8/src/yamcs/mdb/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.8/src/yamcs/mdb/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    15401 2024-03-01 15:24:22.000000 yamcs_client-1.9.8/src/yamcs/mdb/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13254 2024-02-24 16:11:30.000000 yamcs_client-1.9.8/src/yamcs/mdb/model.py
+-rw-r--r--   0 fdi        (503) staff       (20)    13266 2024-05-24 06:22:20.000000 yamcs_client-1.9.8/src/yamcs/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.165556 yamcs_client-1.9.8/src/yamcs/protobuf/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.166357 yamcs_client-1.9.8/src/yamcs/protobuf/actions/
+-rw-r--r--   0 fdi        (503) staff       (20)     4545 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/protobuf/actions/actions_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.167253 yamcs_client-1.9.8/src/yamcs/protobuf/activities/
+-rw-r--r--   0 fdi        (503) staff       (20)    17234 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/activities/activities_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    38288 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/activities/activities_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.168535 yamcs_client-1.9.8/src/yamcs/protobuf/alarms/
+-rw-r--r--   0 fdi        (503) staff       (20)    29047 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/alarms/alarms_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    40124 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/alarms/alarms_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.170765 yamcs_client-1.9.8/src/yamcs/protobuf/archive/
+-rw-r--r--   0 fdi        (503) staff       (20)    33962 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/protobuf/archive/archive_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    53220 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/archive/index_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    43577 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    19316 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/archive/rocksdb_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.171312 yamcs_client-1.9.8/src/yamcs/protobuf/audit/
+-rw-r--r--   0 fdi        (503) staff       (20)    11973 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/audit/audit_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.171740 yamcs_client-1.9.8/src/yamcs/protobuf/auth/
+-rw-r--r--   0 fdi        (503) staff       (20)     8446 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/auth/auth_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.172147 yamcs_client-1.9.8/src/yamcs/protobuf/buckets/
+-rw-r--r--   0 fdi        (503) staff       (20)    34808 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/buckets/buckets_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.174048 yamcs_client-1.9.8/src/yamcs/protobuf/commanding/
+-rw-r--r--   0 fdi        (503) staff       (20)    12415 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/commanding/clearance_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    41600 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/commanding/commanding_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    47775 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/commanding/commands_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    33253 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/commanding/queues_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.174435 yamcs_client-1.9.8/src/yamcs/protobuf/config/
+-rw-r--r--   0 fdi        (503) staff       (20)    17412 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/config/config_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.174798 yamcs_client-1.9.8/src/yamcs/protobuf/cop1/
+-rw-r--r--   0 fdi        (503) staff       (20)    34928 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/cop1/cop1_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.175358 yamcs_client-1.9.8/src/yamcs/protobuf/database/
+-rw-r--r--   0 fdi        (503) staff       (20)     8255 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/database/database_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.176179 yamcs_client-1.9.8/src/yamcs/protobuf/events/
+-rw-r--r--   0 fdi        (503) staff       (20)     9301 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/events/events_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    30677 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/events/events_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.176916 yamcs_client-1.9.8/src/yamcs/protobuf/filetransfer/
+-rw-r--r--   0 fdi        (503) staff       (20)    80380 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.178386 yamcs_client-1.9.8/src/yamcs/protobuf/iam/
+-rw-r--r--   0 fdi        (503) staff       (20)    73419 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/iam/iam_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    10014 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/iam/sessions_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.179647 yamcs_client-1.9.8/src/yamcs/protobuf/instances/
+-rw-r--r--   0 fdi        (503) staff       (20)    19968 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/instances/instances_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    32345 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/instances/instances_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.180000 yamcs_client-1.9.8/src/yamcs/protobuf/links/
+-rw-r--r--   0 fdi        (503) staff       (20)    31906 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/protobuf/links/links_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.180392 yamcs_client-1.9.8/src/yamcs/protobuf/mdb/
+-rw-r--r--   0 fdi        (503) staff       (20)   280528 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/mdb/mdb_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.182020 yamcs_client-1.9.8/src/yamcs/protobuf/packets/
+-rw-r--r--   0 fdi        (503) staff       (20)     6029 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/packets/packets_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    46220 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/packets/packets_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.182886 yamcs_client-1.9.8/src/yamcs/protobuf/plists/
+-rw-r--r--   0 fdi        (503) staff       (20)     4238 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/plists/plists_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    18747 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/plists/plists_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.184057 yamcs_client-1.9.8/src/yamcs/protobuf/processing/
+-rw-r--r--   0 fdi        (503) staff       (20)    37572 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/processing/mdb_override_service_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    86589 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/processing/processing_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.186201 yamcs_client-1.9.8/src/yamcs/protobuf/pvalue/
+-rw-r--r--   0 fdi        (503) staff       (20)    28924 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/protobuf/pvalue/pvalue_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    10465 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.186694 yamcs_client-1.9.8/src/yamcs/protobuf/replication/
+-rw-r--r--   0 fdi        (503) staff       (20)    13030 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/replication/replication_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.187424 yamcs_client-1.9.8/src/yamcs/protobuf/server/
+-rw-r--r--   0 fdi        (503) staff       (20)    70072 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/server/server_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.188816 yamcs_client-1.9.8/src/yamcs/protobuf/services/
+-rw-r--r--   0 fdi        (503) staff       (20)     6369 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/services/services_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    11946 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/services/services_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.189271 yamcs_client-1.9.8/src/yamcs/protobuf/table/
+-rw-r--r--   0 fdi        (503) staff       (20)    68243 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/table/table_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.190159 yamcs_client-1.9.8/src/yamcs/protobuf/tco/
+-rw-r--r--   0 fdi        (503) staff       (20)    32749 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/tco/tco_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.190513 yamcs_client-1.9.8/src/yamcs/protobuf/time/
+-rw-r--r--   0 fdi        (503) staff       (20)    12958 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/time/time_service_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.190980 yamcs_client-1.9.8/src/yamcs/protobuf/timeline/
+-rw-r--r--   0 fdi        (503) staff       (20)   125195 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/timeline/timeline_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.191941 yamcs_client-1.9.8/src/yamcs/protobuf/yamcsManagement/
+-rw-r--r--   0 fdi        (503) staff       (20)    32409 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py
+-rw-r--r--   0 fdi        (503) staff       (20)    42446 2024-04-17 20:21:54.000000 yamcs_client-1.9.8/src/yamcs/protobuf/yamcs_pb2.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.197607 yamcs_client-1.9.8/src/yamcs/storage/
+-rw-r--r--   0 fdi        (503) staff       (20)       55 2022-04-07 19:17:50.000000 yamcs_client-1.9.8/src/yamcs/storage/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     5683 2024-03-05 11:43:25.000000 yamcs_client-1.9.8/src/yamcs/storage/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6439 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/storage/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.199235 yamcs_client-1.9.8/src/yamcs/tco/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.8/src/yamcs/tco/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4867 2024-02-24 17:10:21.000000 yamcs_client-1.9.8/src/yamcs/tco/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)     3089 2024-02-24 17:11:07.000000 yamcs_client-1.9.8/src/yamcs/tco/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.201508 yamcs_client-1.9.8/src/yamcs/timeline/
+-rw-r--r--   0 fdi        (503) staff       (20)       57 2022-05-30 08:31:08.000000 yamcs_client-1.9.8/src/yamcs/timeline/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7923 2024-05-10 15:24:50.000000 yamcs_client-1.9.8/src/yamcs/timeline/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    16141 2024-03-05 10:37:49.000000 yamcs_client-1.9.8/src/yamcs/timeline/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.202775 yamcs_client-1.9.8/src/yamcs/tmtc/
+-rw-r--r--   0 fdi        (503) staff       (20)        0 2022-04-07 19:17:50.000000 yamcs_client-1.9.8/src/yamcs/tmtc/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)    51419 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/tmtc/client.py
+-rw-r--r--   0 fdi        (503) staff       (20)    35330 2024-04-18 19:05:56.000000 yamcs_client-1.9.8/src/yamcs/tmtc/model.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-24 08:03:53.228030 yamcs_client-1.9.8/src/yamcs_client.egg-info/
+-rw-r--r--   0 fdi        (503) staff       (20)     1677 2024-05-24 08:03:53.000000 yamcs_client-1.9.8/src/yamcs_client.egg-info/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)     3504 2024-05-24 08:03:53.000000 yamcs_client-1.9.8/src/yamcs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2024-05-24 08:03:53.000000 yamcs_client-1.9.8/src/yamcs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2022-04-07 19:46:24.000000 yamcs_client-1.9.8/src/yamcs_client.egg-info/not-zip-safe
+-rw-r--r--   0 fdi        (503) staff       (20)       55 2024-05-24 08:03:53.000000 yamcs_client-1.9.8/src/yamcs_client.egg-info/requires.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        6 2024-05-24 08:03:53.000000 yamcs_client-1.9.8/src/yamcs_client.egg-info/top_level.txt
```

### Comparing `yamcs_client-1.9.7/LICENSE` & `yamcs_client-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/PKG-INFO` & `yamcs_client-1.9.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-client
-Version: 1.9.7
+Version: 1.9.8
 Summary: Yamcs API client library
 Home-page: https://github.com/yamcs/python-yamcs-client
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `yamcs_client-1.9.7/README.md` & `yamcs_client-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/setup.py` & `yamcs_client-1.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/api/annotations_pb2.py` & `yamcs_client-1.9.8/src/yamcs/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/api/exception_pb2.py` & `yamcs_client-1.9.8/src/yamcs/api/exception_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/api/httpbody_pb2.py` & `yamcs_client-1.9.8/src/yamcs/api/httpbody_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/api/websocket_pb2.py` & `yamcs_client-1.9.8/src/yamcs/api/websocket_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/archive/client.py` & `yamcs_client-1.9.8/src/yamcs/archive/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/archive/model.py` & `yamcs_client-1.9.8/src/yamcs/archive/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/client/__init__.py` & `yamcs_client-1.9.8/src/yamcs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/client/activities.py` & `yamcs_client-1.9.8/src/yamcs/client/activities.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/client/core.py` & `yamcs_client-1.9.8/src/yamcs/client/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import functools
 import os
+import urllib.parse
 from typing import Any, Callable, Iterable, Iterator, List, Mapping, Optional, Union
 from urllib.parse import urlparse
 
 from google.protobuf import timestamp_pb2
 from yamcs.archive.client import ArchiveClient
 from yamcs.core.auth import APIKeyCredentials, Credentials
 from yamcs.core.context import Context
@@ -24,18 +25,20 @@
     Event,
     Instance,
     InstanceTemplate,
     Link,
     LinkEvent,
     LoadParameterValuesResult,
     Processor,
+    RdbTablespace,
     ServerInfo,
     Service,
     UserInfo,
 )
+from yamcs.protobuf.archive import rocksdb_service_pb2
 from yamcs.protobuf.auth import auth_pb2
 from yamcs.protobuf.events import events_pb2, events_service_pb2
 from yamcs.protobuf.iam import iam_pb2
 from yamcs.protobuf.instances import instances_pb2, instances_service_pb2
 from yamcs.protobuf.links import links_pb2
 from yamcs.protobuf.processing import processing_pb2
 from yamcs.protobuf.pvalue import pvalue_service_pb2
@@ -516,14 +519,46 @@
         # Return an iterator anyway for similarity with other API methods
         response = self.ctx.get_proto(path="/links/" + instance)
         message = links_pb2.ListLinksResponse()
         message.ParseFromString(response.content)
         links = getattr(message, "links")
         return iter([Link(link) for link in links])
 
+    def list_rdb_tablespaces(self) -> Iterable[RdbTablespace]:
+        """
+        Lists RocksDB tablespaces.
+        """
+        response = self.ctx.get_proto(path="/archive/rocksdb/tablespaces")
+        message = rocksdb_service_pb2.ListRocksDbTablespacesResponse()
+        message.ParseFromString(response.content)
+        tablespaces = getattr(message, "tablespaces")
+        return iter([RdbTablespace(tablespace) for tablespace in tablespaces])
+
+    def compact_rdb_column_family(
+        self,
+        tablespace: str,
+        cf: str,
+        dbpath: Optional[str] = None,
+    ):
+        """
+        Compact a RocksDB column family.
+
+        :param tablespace:
+            RocksDB tablespace name
+        :cf:
+            Column family name
+        :param dbpath:
+            Optional path under the tablespace root.
+        """
+        req = rocksdb_service_pb2.CompactDatabaseRequest()
+        req.cfname = cf
+        encoded_name = urllib.parse.quote_plus(dbpath or "")
+        url = f"/archive/rocksdb/{tablespace}/{encoded_name}:compact"
+        self.ctx.post_proto(url, data=req.SerializeToString())
+
     def send_event(
         self,
         instance: str,
         message: str,
         event_type: Optional[str] = None,
         time: Optional[datetime.datetime] = None,
         severity: Optional[str] = "info",
@@ -536,15 +571,14 @@
 
         :param instance:
             A Yamcs instance name.
         :param message:
             Event message.
         :param event_type:
             Type of event.
-
         :param severity:
             The severity level of the event. One of ``info``,
             ``watch``, ``warning``, ``distress``, ``critical``
             or ``severe``. Defaults to ``info``.
         :param time:
             Time of the event. If unspecified, defaults to mission time.
         :param source:
```

### Comparing `yamcs_client-1.9.7/src/yamcs/core/auth.py` & `yamcs_client-1.9.8/src/yamcs/core/auth.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/core/context.py` & `yamcs_client-1.9.8/src/yamcs/core/context.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/core/futures.py` & `yamcs_client-1.9.8/src/yamcs/core/futures.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/core/helpers.py` & `yamcs_client-1.9.8/src/yamcs/core/helpers.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/core/pagination.py` & `yamcs_client-1.9.8/src/yamcs/core/pagination.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/core/subscriptions.py` & `yamcs_client-1.9.8/src/yamcs/core/subscriptions.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/filetransfer/client.py` & `yamcs_client-1.9.8/src/yamcs/filetransfer/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/filetransfer/model.py` & `yamcs_client-1.9.8/src/yamcs/filetransfer/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/link/client.py` & `yamcs_client-1.9.8/src/yamcs/link/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/link/model.py` & `yamcs_client-1.9.8/src/yamcs/link/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/mdb/client.py` & `yamcs_client-1.9.8/src/yamcs/mdb/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/mdb/model.py` & `yamcs_client-1.9.8/src/yamcs/mdb/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/model.py` & `yamcs_client-1.9.8/src/yamcs/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,14 +293,29 @@
 
     @property
     def checked(self) -> bool:
         """Whether the action is currently checked"""
         return self._proto.checked
 
 
+class RdbTablespace:
+    def __init__(self, proto):
+        self._proto = proto
+
+    @property
+    def name(self) -> str:
+        """Tablespace name"""
+        return self._proto.name
+
+    @property
+    def data_dir(self) -> str:
+        """Data directory"""
+        return self._proto.dataDir
+
+
 class Instance:
     def __init__(self, proto):
         self._proto = proto
 
     @property
     def name(self) -> str:
         """Name of this instance."""
```

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/actions/actions_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/actions/actions_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/activities/activities_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/activities/activities_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/activities/activities_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/activities/activities_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/alarms/alarms_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/alarms/alarms_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/alarms/alarms_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/alarms/alarms_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/archive/archive_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/archive/archive_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/archive/index_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/archive/index_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/archive/parameter_archive_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/archive/rocksdb_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/archive/rocksdb_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/audit/audit_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/audit/audit_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/auth/auth_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/buckets/buckets_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/buckets/buckets_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/commanding/clearance_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/commanding/clearance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/commanding/commanding_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/commanding/commanding_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/commanding/commands_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/commanding/commands_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/commanding/queues_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/commanding/queues_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/config/config_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/config/config_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/cop1/cop1_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/cop1/cop1_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/database/database_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/database/database_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/events/events_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/events/events_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/events/events_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/filetransfer/filetransfer_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/iam/iam_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/iam/iam_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/iam/sessions_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/iam/sessions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/instances/instances_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/instances/instances_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/instances/instances_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/instances/instances_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/links/links_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/links/links_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/mdb/mdb_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/mdb/mdb_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/packets/packets_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/packets/packets_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/packets/packets_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/packets/packets_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/plists/plists_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/plists/plists_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/plists/plists_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/plists/plists_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/processing/mdb_override_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/processing/mdb_override_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/processing/processing_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/processing/processing_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/pvalue/pvalue_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/pvalue/pvalue_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/pvalue/pvalue_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/replication/replication_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/replication/replication_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/server/server_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/server/server_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/services/services_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/services/services_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/services/services_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/services/services_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/table/table_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/table/table_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/tco/tco_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/tco/tco_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/time/time_service_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/time/time_service_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/timeline/timeline_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/timeline/timeline_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/yamcsManagement/yamcsManagement_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/protobuf/yamcs_pb2.py` & `yamcs_client-1.9.8/src/yamcs/protobuf/yamcs_pb2.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/storage/client.py` & `yamcs_client-1.9.8/src/yamcs/storage/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/storage/model.py` & `yamcs_client-1.9.8/src/yamcs/storage/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/tco/client.py` & `yamcs_client-1.9.8/src/yamcs/tco/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/tco/model.py` & `yamcs_client-1.9.8/src/yamcs/tco/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/timeline/client.py` & `yamcs_client-1.9.8/src/yamcs/timeline/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/timeline/model.py` & `yamcs_client-1.9.8/src/yamcs/timeline/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/tmtc/client.py` & `yamcs_client-1.9.8/src/yamcs/tmtc/client.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs/tmtc/model.py` & `yamcs_client-1.9.8/src/yamcs/tmtc/model.py`

 * *Files identical despite different names*

### Comparing `yamcs_client-1.9.7/src/yamcs_client.egg-info/PKG-INFO` & `yamcs_client-1.9.8/src/yamcs_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-client
-Version: 1.9.7
+Version: 1.9.8
 Summary: Yamcs API client library
 Home-page: https://github.com/yamcs/python-yamcs-client
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `yamcs_client-1.9.7/src/yamcs_client.egg-info/SOURCES.txt` & `yamcs_client-1.9.8/src/yamcs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

