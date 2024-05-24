# Comparing `tmp/tikit-1.7.1.240409.tar.gz` & `tmp/tikit-1.7.1.240523.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikit-1.7.1.240409.tar", last modified: Wed Apr 10 11:49:09 2024, max compression
+gzip compressed data, was "tikit-1.7.1.240523.tar", last modified: Fri May 24 09:00:06 2024, max compression
```

## Comparing `tikit-1.7.1.240409.tar` & `tikit-1.7.1.240523.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      700 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/README.md
--rw-r--r--   0 root         (0) root         (0)      413 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      858 2024-04-09 13:14:07.000000 tikit-1.7.1.240409/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/
--rw-r--r--   0 root         (0) root         (0)      185 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7896 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/cli.py
--rw-r--r--   0 root         (0) root         (0)   218778 2024-04-10 11:48:19.000000 tikit-1.7.1.240409/tikit/client.py
--rw-r--r--   0 root         (0) root         (0)     3976 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/default_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/display_optimize/
--rw-r--r--   0 root         (0) root         (0)      133 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/display_optimize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3820 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/display_optimize/dataset.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/display_optimize/resource_group.py
--rw-r--r--   0 root         (0) root         (0)     4933 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/display_optimize/training_model.py
--rw-r--r--   0 root         (0) root         (0)    12329 2024-04-09 13:08:11.000000 tikit-1.7.1.240409/tikit/display_optimize/training_task.py
--rw-r--r--   0 root         (0) root         (0)     1779 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/hdfs.py
--rw-r--r--   0 root         (0) root         (0)    35625 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/hive.py
--rw-r--r--   0 root         (0) root         (0)    20234 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/templates/
--rw-r--r--   0 root         (0) root         (0)     7622 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/templates/service_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/common/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16473 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/abstract_client.py
--rw-r--r--   0 root         (0) root         (0)     2337 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/abstract_model.py
--rw-r--r--   0 root         (0) root         (0)     2002 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/common_client.py
--rw-r--r--   0 root         (0) root         (0)    12338 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/credential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/common/exception/
--rw-r--r--   0 root         (0) root         (0)      741 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/common/http/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5071 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/http/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/common/profile/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1657 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 root         (0) root         (0)     1857 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 root         (0) root         (0)     1574 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/common/sign.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit/tencentcloud/emr/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6015 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)     3465 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    33848 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/tikit/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12419 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   769939 2024-04-10 11:48:19.000000 tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 root         (0) root         (0)   263659 2024-04-09 13:08:11.000000 tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/tione_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/tikit/tencentcloud/wedata/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.770266 tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)      819 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    19834 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)     4802 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-02 08:12:30.000000 tikit-1.7.1.240409/tikit/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 11:49:09.766266 tikit-1.7.1.240409/tikit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      700 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1883 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      413 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-10 11:49:09.000000 tikit-1.7.1.240409/tikit.egg-info/top_level.txt
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.627457 tikit-1.7.1.240523/
+-rw-r--r--   0 liuliu     (501) staff       (20)       71 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/MANIFEST.in
+-rw-r--r--   0 liuliu     (501) staff       (20)     1503 2024-05-24 09:00:06.627228 tikit-1.7.1.240523/PKG-INFO
+-rw-r--r--   0 liuliu     (501) staff       (20)      499 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/README.md
+-rw-r--r--   0 liuliu     (501) staff       (20)      413 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/requirements.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)       38 2024-05-24 09:00:06.627517 tikit-1.7.1.240523/setup.cfg
+-rw-r--r--   0 liuliu     (501) staff       (20)      858 2024-05-24 08:57:52.000000 tikit-1.7.1.240523/setup.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.616619 tikit-1.7.1.240523/tikit/
+-rw-r--r--   0 liuliu     (501) staff       (20)      185 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     7896 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/cli.py
+-rw-r--r--   0 liuliu     (501) staff       (20)   225230 2024-05-24 08:57:52.000000 tikit-1.7.1.240523/tikit/client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     3976 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/default_client.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.618756 tikit-1.7.1.240523/tikit/display_optimize/
+-rw-r--r--   0 liuliu     (501) staff       (20)      133 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/display_optimize/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     3820 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/display_optimize/dataset.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     2242 2024-01-22 08:43:53.000000 tikit-1.7.1.240523/tikit/display_optimize/resource_group.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     4933 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/display_optimize/training_model.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    12329 2024-05-22 11:50:24.000000 tikit-1.7.1.240523/tikit/display_optimize/training_task.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1779 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/hdfs.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    35625 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/hive.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    26442 2024-05-24 08:57:52.000000 tikit-1.7.1.240523/tikit/models.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.619052 tikit-1.7.1.240523/tikit/templates/
+-rw-r--r--   0 liuliu     (501) staff       (20)     7622 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/templates/service_config.yaml
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.619263 tikit-1.7.1.240523/tikit/tencentcloud/
+-rw-r--r--   0 liuliu     (501) staff       (20)      630 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.620355 tikit-1.7.1.240523/tikit/tencentcloud/common/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    16473 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     2337 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     2002 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/common_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    12338 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/credential.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.620726 tikit-1.7.1.240523/tikit/tencentcloud/common/exception/
+-rw-r--r--   0 liuliu     (501) staff       (20)      741 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)      760 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.621038 tikit-1.7.1.240523/tikit/tencentcloud/common/http/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     5071 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/http/request.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.621563 tikit-1.7.1.240523/tikit/tencentcloud/common/profile/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1657 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1857 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     1574 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/common/sign.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.621744 tikit-1.7.1.240523/tikit/tencentcloud/emr/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.622462 tikit-1.7.1.240523/tikit/tencentcloud/emr/v20190103/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     6015 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     3465 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    33848 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/emr/v20190103/models.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.622719 tikit-1.7.1.240523/tikit/tencentcloud/tione/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.624939 tikit-1.7.1.240523/tikit/tencentcloud/tione/v20211111/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    14837 2024-05-24 08:57:52.000000 tikit-1.7.1.240523/tikit/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 liuliu     (501) staff       (20)   778994 2024-05-24 08:57:52.000000 tikit-1.7.1.240523/tikit/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 liuliu     (501) staff       (20)   263659 2024-05-22 11:50:24.000000 tikit-1.7.1.240523/tikit/tencentcloud/tione/v20211111/tione_client.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.625631 tikit-1.7.1.240523/tikit/tencentcloud/wedata/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.626548 tikit-1.7.1.240523/tikit/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 liuliu     (501) staff       (20)        0 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 liuliu     (501) staff       (20)      819 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 liuliu     (501) staff       (20)    19834 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 liuliu     (501) staff       (20)     4802 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 liuliu     (501) staff       (20)      893 2023-10-25 02:56:46.000000 tikit-1.7.1.240523/tikit/util.py
+drwxr-xr-x   0 liuliu     (501) staff       (20)        0 2024-05-24 09:00:06.626845 tikit-1.7.1.240523/tikit.egg-info/
+-rw-r--r--   0 liuliu     (501) staff       (20)     1503 2024-05-24 09:00:06.000000 tikit-1.7.1.240523/tikit.egg-info/PKG-INFO
+-rw-r--r--   0 liuliu     (501) staff       (20)     1883 2024-05-24 09:00:06.000000 tikit-1.7.1.240523/tikit.egg-info/SOURCES.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)        1 2024-05-24 09:00:06.000000 tikit-1.7.1.240523/tikit.egg-info/dependency_links.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)       40 2024-05-24 09:00:06.000000 tikit-1.7.1.240523/tikit.egg-info/entry_points.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)      413 2024-05-24 09:00:06.000000 tikit-1.7.1.240523/tikit.egg-info/requires.txt
+-rw-r--r--   0 liuliu     (501) staff       (20)        6 2024-05-24 09:00:06.000000 tikit-1.7.1.240523/tikit.egg-info/top_level.txt
```

### Comparing `tikit-1.7.1.240409/setup.py` & `tikit-1.7.1.240523/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def long_description():
     with io.open('README.md', 'r', encoding='utf8') as fileobj:
         return fileobj.read()
 
 
 setup(
     name='tikit',
-    version='1.7.1.240409',
+    version='1.7.1.240523',
     url='https://cloud.tencent.com/',
     license='MIT',
     author='TI PLATFORM TEAM',
     author_email='TI_Platform@tencent.com',
     description='Kit for TI PLATFORM',
     long_description=long_description(),
     packages=find_packages(),
```

### Comparing `tikit-1.7.1.240409/tikit/cli.py` & `tikit-1.7.1.240523/tikit/cli.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/client.py` & `tikit-1.7.1.240523/tikit/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,17 @@
                     "ANNOTATION_TYPE_OCR"]
 ANNOTATION_FORMATS = ["ANNOTATION_FORMAT_TI",
                       "ANNOTATION_FORMAT_PASCAL",
                       "ANNOTATION_FORMAT_COCO",
                       "ANNOTATION_FORMAT_FILE"]
 ALL_SUPPORT_TRAINING_MODES = ["PS_WORKER", "DDP", "MPI", "HOROVOD"]
 REGION_DICT = {"ap-guangzhou": 1,
-               "ap-shanghai":4,
-               "ap-beijing":8,
-               "ap-nanjing":33}
+               "ap-shanghai": 4,
+               "ap-beijing": 8,
+               "ap-nanjing": 33}
 
 
 class Client(object):
     # 临时秘钥使用，提前获取临时秘钥，避免访问的时候失败
     _secret_ahead_time = 60 * 5
 
     def __init__(self, secret_id=None, secret_key=None, region=None, token=None, proxies=None, tione_endpoint=None):
@@ -637,15 +637,15 @@
                 price_req.SpecsParam.append({"SpecName": spec.SpecName, "SpecCount": 1})
             price_result = self._tione_client.DescribeBillingSpecsPrice(price_req)
             for i in range(len(price_result.SpecsPrice)):
                 specs.Specs[i].SpecId = str(price_result.SpecsPrice[i].RealTotalCost / 100.0)
             return specs
         except TencentCloudSDKException as err:
             raise
-    
+
     def describe_postpaid_reasoning_price(self):
         """查询每种配置的每小时的价格，价格单位：元
 
         :rtype:     tikit.tencentcloud.tione.v20211111.models.DescribeBillingSpecsResponse
         """
         try:
             req = models.DescribeBillingSpecsRequest()
@@ -694,15 +694,14 @@
         rsp.Specs = [gen_spec(d) for d in specs]
         return rsp
 
     def describe_hy_available_gpu(self):
         """获取当前可用GPU"""
         return self._tione_client.DescribeTJResourceDetail()
 
-
     def describe_taiji_hy_tasks(self, filters=None, tag_filters=None, offset=0, limit=50, order="DESC",
                                 order_field="UpdateTime"):
         """获取训练任务列表
 
         :param filters:     过滤器，eg：[{ "Name": "TaskStatus", "Values": ["Running"] }]
         :type filters:      list of Filter
         :param tag_filters: 标签过滤器，eg：[{ "TagKey": "TagKeyA", "TagValue": ["TagValueA"] }]
@@ -951,22 +950,22 @@
             req.SubnetId = sub_net_id
 
             return self._tione_client.CreateTrainingTask(req)
         except TencentCloudSDKException as err:
             raise
 
     def create_taiji_hy_training_task(self,
-                             name,
-                             worker_resource,
-                             template_name=None,
-                             base_model_id=None,
-                             input_data_config=None,
-                             tags=None,
-                             tuning_parameters_dict={},
-                             remark=None):
+                                      name,
+                                      worker_resource,
+                                      template_name=None,
+                                      base_model_id=None,
+                                      input_data_config=None,
+                                      tags=None,
+                                      tuning_parameters_dict={},
+                                      remark=None):
         """创建训练任务
 
         :param name:        任务名称
         :type name:         str
         :param worker_resource:     worker节点的配置
         :type worker_resource:      :class:`tikit.models.ResourceConfigInfo`
         :param template_name:     太极模版名称
@@ -1011,15 +1010,17 @@
             if input_data_config is not None:
                 req.DataConfigs, req.DataSource = self._parse_training_task_input_data(input_data_config)
 
             rsp = self._tione_client.CreateTrainingTask(req)
             if rsp.Id is not None:
                 training_task_id = rsp.Id
                 region_id = REGION_DICT[self._region]
-                print("monitor_url : https://console.cloud.tencent.com/tione/v2/job/detail/%s?regionId=%d&detailTab=monitor&monitorTab=training" % (training_task_id, region_id))
+                print(
+                    "monitor_url : https://console.cloud.tencent.com/tione/v2/job/detail/%s?regionId=%d&detailTab=monitor&monitorTab=training" % (
+                    training_task_id, region_id))
             return rsp
         except TencentCloudSDKException as err:
             raise
 
     def _convert_data_config_old(self, input_data_item) -> List[models.DataConfig]:
         # 兼容旧版本的处理
         result = []
@@ -1079,15 +1080,14 @@
             assert input_data_item.CFSTurboId
             data_config.CFSTurboSource.Id = input_data_item.CFSTurboId
             data_config.CFSTurboSource.Path = input_data_item.CFSTurboPath
         else:
             print("warning! not supported DataSourceType", input_data_item.DataSource)
             return None
         return data_config
-        
 
     def _parse_training_task_input_data(self, input_data_config):
         if not isinstance(input_data_config, list) and input_data_config.DataConfigDict:
             # 兼容旧版本的处理
             data_configs = self._convert_data_config_old(input_data_config)
             return data_configs, input_data_config.DataSource
         if not isinstance(input_data_config, list):
@@ -1550,15 +1550,15 @@
         for version in versions.TrainingModelVersions:
             new_length = len(version.TrainingModelVersion)
             if new_length > len(ret) or (new_length == len(ret) and version.TrainingModelVersion > ret):
                 ret = version.TrainingModelVersion
         return "v%d" % (int(ret[1:]) + 1)
 
     def _set_reaoning_env(self, req, reasoning_env):
-        req.ReasoningEnvironmentSource = reasoning_env.Source 
+        req.ReasoningEnvironmentSource = reasoning_env.Source
         if reasoning_env.Source == "CUSTOM":
             req.ReasoningImageInfo = models.ImageInfo()
             req.ReasoningImageInfo.ImageType = reasoning_env.ImageType
             req.ReasoningImageInfo.ImageUrl = reasoning_env.ImageUrl
             req.ReasoningImageInfo.RegistryRegion = reasoning_env.RegistryRegion
             req.ReasoningImageInfo.RegistryId = reasoning_env.RegistryId
             return
@@ -1569,32 +1569,31 @@
                     req.ReasoningEnvironment = image.InferTemplateImage
                     req.ReasoningEnvironmentId = reasoning_env.ImageKey
                     return
         raise TencentCloudSDKException(
             message='image key "{}" is invalid, please use "describe_system_images" to get image key list'.format(
                 reasoning_env.ImageKey))
 
-    def _check_model_clean_params(self, req, 
-                                    model_auto_clean=None, 
-                                    model_clean_period=None, 
-                                    max_reserved_models=None):
+    def _check_model_clean_params(self, req,
+                                  model_auto_clean=None,
+                                  model_clean_period=None,
+                                  max_reserved_models=None):
         if model_auto_clean is not None:
             req.AutoClean = model_auto_clean
         if model_clean_period is not None:
             if model_clean_period == 0:
                 req.ModelCleanPeriod = 65535
             else:
                 req.ModelCleanPeriod = model_clean_period
         if max_reserved_models is not None:
             if max_reserved_models == 0:
                 req.MaxReservedModels = 65535
             else:
                 req.MaxReservedModels = max_reserved_models
 
-
     def _create_model_by_task(self,
                               req,
                               training_job_id,
                               reasoning_env,
                               model_output_path,
                               model_format,
                               training_model_index=None,
@@ -1619,15 +1618,14 @@
                     req.TrainingModelCosPath.Paths[0] = req.TrainingModelCosPath.Paths[0] + training_job_id + "/"
             else:
                 task = self.describe_training_task(training_job_id)
                 req.TrainingJobName = task.TrainingTaskDetail.Name
                 req.TrainingModelCosPath = task.TrainingTaskDetail.Output
                 req.TrainingModelCosPath.Paths[0] = req.TrainingModelCosPath.Paths[0] + training_job_id + "/"
                 req.AlgorithmFramework = task.TrainingTaskDetail.FrameworkName
-            
 
             # 训练指标优先使用参数里面的
             req.TrainingModelIndex = training_model_index
             if not training_model_index:
                 req.TrainingModelIndex = self._get_model_index(training_job_id)
 
             self._set_reaoning_env(req, reasoning_env)
@@ -1635,30 +1633,29 @@
             req.ModelMoveMode = "CUT" if delete_task_cos_model else "COPY"
             req.Tags = tags
             req.IsQAT = is_qat
             return self._tione_client.CreateTrainingModel(req)
 
         except TencentCloudSDKException as err:
             raise
-    
+
     def _create_taiji_hy_model_by_task(self,
-                              req,
-                              training_job_id,
-                              training_model_index=None,
-                              tags=None):
+                                       req,
+                                       training_job_id,
+                                       training_model_index=None,
+                                       tags=None):
         try:
             req.TrainingJobId = training_job_id
             req.TrainingModelSource = "JOB"
             req.ModelVersionType = "TAIJI_HY"
             req.ReasoningEnvironmentSource = "SYSTEM"
 
             task = self.describe_training_task(training_job_id)
             req.TrainingJobName = task.TrainingTaskDetail.Name
             req.AlgorithmFramework = task.TrainingTaskDetail.FrameworkName
-            
 
             # 训练指标优先使用参数里面的
             req.TrainingModelIndex = training_model_index
             if not training_model_index:
                 req.TrainingModelIndex = self._get_model_index(training_job_id)
 
             req.Tags = tags
@@ -1678,15 +1675,15 @@
                               delete_task_cos_model=False,
                               tags=None,
                               is_qat=False):
         try:
             req.TrainingJobId = training_job_id
             req.TrainingModelSource = "JOB"
             self._set_cos_path_info(req, model_output_path)
-            req.ModelFormat = model_format 
+            req.ModelFormat = model_format
             # get job info from task
             if model_format == "SAVED_MODEL":
                 task = self.describe_training_task(training_job_id)
                 req.TrainingJobName = task.TrainingTaskDetail.Name
                 req.AlgorithmFramework = task.TrainingTaskDetail.FrameworkName
                 if training_model_cos_path is not None:
                     self._set_task_cos_path_info(req, training_model_cos_path)
@@ -1697,15 +1694,15 @@
                 req.TrainingModelCosPath.Paths[0] = req.TrainingModelCosPath.Paths[0] + training_job_id + "/"
                 req.AlgorithmFramework = task.TrainingTaskDetail.FrameworkName
 
             # 训练指标优先使用参数里面的
             req.TrainingModelIndex = training_model_index
             if not training_model_index:
                 req.TrainingModelIndex = self._get_model_index(training_job_id)
-            
+
             self._set_reaoning_env(req, reasoning_env)
 
             req.ModelMoveMode = "CUT" if delete_task_cos_model else "COPY"
             req.Tags = tags
             req.IsQAT = is_qat
             return self._tione_client.CreateTrainingModel(req)
         except TencentCloudSDKException as err:
@@ -1718,15 +1715,15 @@
         cos_path_info = models.CosPathInfo()
         cos_path_info.Bucket = model_output_path.Bucket
         cos_path_info.Region = model_output_path.Region
         cos_path_info.Paths = [model_output_path.Path]
         cos_path_info.Uin = model_output_path.Uin
         cos_path_info.SubUin = model_output_path.SubUin
         req.ModelOutputPath = cos_path_info
-    
+
     def _set_task_cos_path_info(self, req, training_model_cos_path):
         if isinstance(training_model_cos_path, str):
             req.TrainingModelCosPath = self.parse_cos_info(training_model_cos_path)
             return
         cos_path_info = models.CosPathInfo()
         cos_path_info.Bucket = training_model_cos_path.Bucket
         cos_path_info.Region = training_model_cos_path.Region
@@ -1825,16 +1822,16 @@
         """
         req = models.CreateTrainingModelRequest()
         req.ImportMethod = "MODEL"
         req.TrainingModelName = training_model_name
         req.ModelAffiliation = "AI_MARKET"
 
         return self._create_taiji_hy_model_by_task(req,
-                                          training_job_id,
-                                          tags=tags)
+                                                   training_job_id,
+                                                   tags=tags)
 
     def create_model_by_cos(self,
                             training_model_name,
                             algorithm_framework,
                             model_cos_path,
                             reasoning_env,
                             model_format,
@@ -1892,22 +1889,22 @@
             self._set_task_cos_path_info(req, model_cos_path)
             req.TrainingModelIndex = model_index
             req.TrainingModelSource = "COS"
 
             # 设置镜像
             self._set_reaoning_env(req, reasoning_env)
 
-            #self._set_cos_path_info(req, model_output_path)
+            # self._set_cos_path_info(req, model_output_path)
             req.ModelFormat = model_format
 
             req.ModelMoveMode = "CUT" if delete_task_cos_model else "COPY"
             req.Tags = tags
             req.IsQAT = is_qat
 
-            self._check_model_clean_params(req, model_auto_clean, model_clean_period, max_reserved_models) 
+            self._check_model_clean_params(req, model_auto_clean, model_clean_period, max_reserved_models)
             return self._tione_client.CreateTrainingModel(req)
         except TencentCloudSDKException as err:
             raise
 
     def create_model_version_by_task(self,
                                      training_model_id,
                                      training_job_id,
@@ -2035,44 +2032,44 @@
             req.TrainingModelId = training_model_id
             req.TrainingModelVersion = self._get_model_new_version(training_model_id)
             req.AlgorithmFramework = algorithm_framework
             self._set_task_cos_path_info(req, model_cos_path)
             req.TrainingModelIndex = model_index
             req.TrainingModelSource = "COS"
 
-            #self._set_cos_path_info(req, model_output_path)
+            # self._set_cos_path_info(req, model_output_path)
             req.ModelFormat = model_format
 
             req.ModelMoveMode = "CUT" if delete_task_cos_model else "COPY"
 
             self._set_reaoning_env(req, reasoning_env)
 
             req.Tags = tags
             req.IsQAT = is_qat
             self._check_model_clean_params(req, model_auto_clean, model_clean_period, max_reserved_models)
-            
+
             return self._tione_client.CreateTrainingModel(req)
         except TencentCloudSDKException as err:
             raise
 
-    def append_model_into_existed_version_by_task(self, 
-                                          training_model_id,
-                                          training_model_version,
-                                          training_job_id,
-                                          training_model_cos_path,
-                                          reasoning_env,
-                                          model_output_path,
-                                          model_format,
-                                          training_model_index=None,
-                                          model_auto_clean=None,
-                                          model_clean_period=None, 
-                                          max_reserved_models=None,
-                                          delete_task_cos_model=False,
-                                          tags=None,
-                                          is_qat=False):
+    def append_model_into_existed_version_by_task(self,
+                                                  training_model_id,
+                                                  training_model_version,
+                                                  training_job_id,
+                                                  training_model_cos_path,
+                                                  reasoning_env,
+                                                  model_output_path,
+                                                  model_format,
+                                                  training_model_index=None,
+                                                  model_auto_clean=None,
+                                                  model_clean_period=None,
+                                                  max_reserved_models=None,
+                                                  delete_task_cos_model=False,
+                                                  tags=None,
+                                                  is_qat=False):
         """使用现有的任务的结果来追加模型至现有的模型版本
 
         :param training_model_id: 模型ID
         :type training_model_id: str
         :param training_model_version: 模型版本
         :type training_model_version: str
         :param training_job_id: 训练任务id
@@ -2121,32 +2118,32 @@
                                               reasoning_env,
                                               model_format,
                                               model_output_path,
                                               training_model_index,
                                               delete_task_cos_model,
                                               tags,
                                               is_qat)
-            
+
         except TencentCloudSDKException as err:
             raise
 
     def append_model_into_existed_version_by_cos(self,
-                                                  training_model_id,
-                                                  training_model_version,
-                                                  model_cos_path,
-                                                  model_format,
-                                                  reasoning_env,
-                                                  model_output_path,
-                                                  model_index=None,
-                                                  model_auto_clean=None,
-                                                  model_clean_period=None,
-                                                  max_reserved_models=None,
-                                                  delete_task_cos_model=False,
-                                                  tags=None,
-                                                  is_qat=False):
+                                                 training_model_id,
+                                                 training_model_version,
+                                                 model_cos_path,
+                                                 model_format,
+                                                 reasoning_env,
+                                                 model_output_path,
+                                                 model_index=None,
+                                                 model_auto_clean=None,
+                                                 model_clean_period=None,
+                                                 max_reserved_models=None,
+                                                 delete_task_cos_model=False,
+                                                 tags=None,
+                                                 is_qat=False):
         """使用现有的cos路径来更新现有模型版本的模型
         :param training_model_id: 模型ID
         :type training_model_id: str
         :param training_model_version: 模型版本
         :type training_model_version: str
         :param model_cos_path: 模型来源路径
         :type model_cos_path: :class:`tikit.models.CosPathInfo`
@@ -2325,15 +2322,15 @@
         try:
             req = models.DescribeTrainingModelVersionRequest()
             req.TrainingModelVersionId = training_model_version_id
             return self._tione_client.DescribeTrainingModelVersion(req)
         except TencentCloudSDKException as err:
             raise
 
-    def delete_training_model(self, training_model_id,enable_delete_cos=True,model_version_type=None):
+    def delete_training_model(self, training_model_id, enable_delete_cos=True, model_version_type=None):
         """删除模型
 
         :param training_model_id: 模型id
         :type training_model_id: str
         :param enable_delete_cos: 是否同步清理cos
         :type enable_delete_cos: bool
         :param model_version_type: 删除模型类型，枚举值：NORMAL 普通，ACCELERATE 加速，不传则删除所有
@@ -2446,25 +2443,28 @@
             req.BatchTaskName = batch_task_name
             req.JobType = job_type
             if job_type == 2:
                 if cron_info is None:
                     raise Exception("cron_info is required")
                 req.CronInfo = cron_info
 
-            parse_input_configs, _ = self._parse_training_task_input_data(self._parse_batch_cos_target_path(input_config))
+            parse_input_configs, _ = self._parse_training_task_input_data(
+                self._parse_batch_cos_target_path(input_config))
             if len(parse_input_configs) > 1:
                 raise Exception("input_config max length is 1")
             req.DataConfigs = parse_input_configs
 
-            parse_output_configs, _ = self._parse_training_task_input_data(self._parse_batch_cos_target_path(output_config))
+            parse_output_configs, _ = self._parse_training_task_input_data(
+                self._parse_batch_cos_target_path(output_config))
             if len(parse_output_configs) > 1:
                 raise Exception("output_config max length is 1")
             req.Outputs = parse_output_configs
 
-            if parse_input_configs[0].DataSourceType == "WEDATA_HDFS" or parse_output_configs[0].DataSourceType == "WEDATA_HDFS":
+            if parse_input_configs[0].DataSourceType == "WEDATA_HDFS" or parse_output_configs[
+                0].DataSourceType == "WEDATA_HDFS":
                 if vpc_id is None or subnet_id is None:
                     raise Exception("WEDATA_HDFS require vpc_id and subnet_id")
 
             imageInfo = models.ImageInfo()
             if model_info is not None:
                 if code_package is not None:
                     req.CodePackage = self.parse_cos_info(code_package)
@@ -2550,15 +2550,14 @@
                     if "gpu" in imageInfo.ImageUrl:
                         billing_spec_req.ResourceType = "GPU"
                     if "cpu" in imageInfo.ImageUrl:
                         billing_spec_req.ResourceType = "CPU"
                 billing_spec = self._tione_client.DescribeBillingSpecs(billing_spec_req)
                 for v in billing_spec.Specs:
                     if resource_config_info.InstanceType == v.SpecName:
-
                         worker_info.InstanceType = resource_config_info.InstanceType
                         worker_info.InstanceTypeAlias = v.SpecAlias
                         break
                 if worker_info.InstanceType is None:
                     raise Exception("please enter the correct InstanceType: %s" % resource_config_info.InstanceType)
             req.ResourceConfigInfo = worker_info
 
@@ -2766,45 +2765,45 @@
         :param command:                启动命令
         :type command:                 str
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.CreateModelServiceResponse`
         """
 
         return self._create_model_service_do("", worker_resource, framework, service_group_id,
-                                            service_description, resource_group_id, model_config_info, model_cos_path,
-                                            volume_mount, service_limit, scheduled_action, model_hot_update_enable,
-                                            env, scale_mode, replicas, horizontal_pod_autoscaler, log_enable,
-                                            log_logset_id, log_topic_id, authorization_enable, tags, cron_scale_jobs,
-                                            scale_strategy, hybrid_billing_prepaid_replicas,command,True)
+                                             service_description, resource_group_id, model_config_info, model_cos_path,
+                                             volume_mount, service_limit, scheduled_action, model_hot_update_enable,
+                                             env, scale_mode, replicas, horizontal_pod_autoscaler, log_enable,
+                                             log_logset_id, log_topic_id, authorization_enable, tags, cron_scale_jobs,
+                                             scale_strategy, hybrid_billing_prepaid_replicas, command, True)
 
     def create_model_service(self,
-                            service_group_name,
-                            worker_resource,
-                            framework=None,
-                            service_description=None,
-                            resource_group_id=None,
-                            model_config_info=None,
-                            model_cos_path=None,
-                            volume_mount=None,
-                            service_limit=None,
-                            scheduled_action=None,
-                            model_hot_update_enable=False,
-                            env=None,
-                            scale_mode="MANUAL",
-                            replicas=1,
-                            horizontal_pod_autoscaler=None,
-                            log_enable=False,
-                            log_logset_id=None,
-                            log_topic_id=None,
-                            authorization_enable=False,
-                            tags=None,
-                            cron_scale_jobs=None,
-                            scale_strategy=None,
-                            hybrid_billing_prepaid_replicas=None,
-                            command=None):
+                             service_group_name,
+                             worker_resource,
+                             framework=None,
+                             service_description=None,
+                             resource_group_id=None,
+                             model_config_info=None,
+                             model_cos_path=None,
+                             volume_mount=None,
+                             service_limit=None,
+                             scheduled_action=None,
+                             model_hot_update_enable=False,
+                             env=None,
+                             scale_mode="MANUAL",
+                             replicas=1,
+                             horizontal_pod_autoscaler=None,
+                             log_enable=False,
+                             log_logset_id=None,
+                             log_topic_id=None,
+                             authorization_enable=False,
+                             tags=None,
+                             cron_scale_jobs=None,
+                             scale_strategy=None,
+                             hybrid_billing_prepaid_replicas=None,
+                             command=None):
 
         """创建模型服务
 
         :param service_group_name:     服务名称
         :type service_group_name:      str
         :param worker_resource:        worker节点的配置
         :type worker_resource:         :class:`tikit.models.ModelServiceResourceConfigInfo`
@@ -2853,27 +2852,27 @@
         :param command:                启动命令
         :type command:                 str
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.CreateModelServiceResponse`
         """
 
         return self._create_model_service_do(service_group_name, worker_resource, framework, "",
-                                            service_description, resource_group_id, model_config_info, model_cos_path,
-                                            volume_mount, service_limit, scheduled_action, model_hot_update_enable,
-                                            env, scale_mode, replicas, horizontal_pod_autoscaler, log_enable,
-                                            log_logset_id, log_topic_id, authorization_enable, tags, cron_scale_jobs,
-                                            scale_strategy, hybrid_billing_prepaid_replicas, command,False)
+                                             service_description, resource_group_id, model_config_info, model_cos_path,
+                                             volume_mount, service_limit, scheduled_action, model_hot_update_enable,
+                                             env, scale_mode, replicas, horizontal_pod_autoscaler, log_enable,
+                                             log_logset_id, log_topic_id, authorization_enable, tags, cron_scale_jobs,
+                                             scale_strategy, hybrid_billing_prepaid_replicas, command, False)
 
     def create_taiji_model_service(self,
-                                     service_name,
-                                     service_description,
-                                     model_version_id,
-                                     instance_type,
-                                     replicas=1,
-                                     enable_auth=True):
+                                   service_name,
+                                   service_description,
+                                   model_version_id,
+                                   instance_type,
+                                   replicas=1,
+                                   enable_auth=True):
         """创建太极混元模型服务
 
 
         :param service_name:            服务名
         :param service_description:     服务描述
         :param model_version_id:        模型ID
         :param instance_type:           资源实例名称
@@ -2992,15 +2991,15 @@
                     content += f'service_group_id: {service_group_id}\n'
                 if not si_found:
                     content += f'service_id: {service_id}\n'
             with open(filename, 'w') as outfile:
                 outfile.write(content)
             return f'成功创建服务{service_id}，服务ID已经写入文件{filename}。如果需要创建新版本，需要新建一个配置文件，切勿重用文件{filename}，否则会丢失本次新建的服务配置。'
 
-    def _create_model_service_file_to_arguments(self, filename: str)-> dict:
+    def _create_model_service_file_to_arguments(self, filename: str) -> dict:
         result = {}
         if not os.path.exists(filename):
             raise FileNotFoundError(filename)
         import yaml
         with open(filename, 'r') as infile:
             data = yaml.load(infile, Loader=yaml.SafeLoader)
 
@@ -3072,15 +3071,15 @@
         if data.get('model_hot_update_enable'):
             result['model_hot_update_enable'] = True
 
         if data.get('env'):
             result['env'] = []
             for e in data.get('env'):
                 ev = models.EnvVar()
-                ev.Name = e['name'] 
+                ev.Name = e['name']
                 ev.Value = e['value']
                 result['env'].append(ev)
 
         if data.get('replicas') is None:
             raise ValueError('replicas should not be empty')
         result['replicas'] = data['replicas']
         scale_mode = data.get('scale_mode', 'MANUAL')
@@ -3120,15 +3119,15 @@
                 cron_jobs.append(job)
             result['cron_scale_jobs'] = cron_jobs
         elif scale_mode == 'MANUAL' and not scale_strategy:
             pass
         else:
             message = f'invalid value: (scale_mode x scale_strategy) tuple should only be one of [(MANUAL, NONE), (AUTO, HPA), (AUTO, CRON)], but your input is ({scale_mode}, {scale_strategy})'
             raise ValueError(message)
-        
+
         if data.get('log_enable'):
             result['log_enable'] = True
             result['log_logset_id'] = data.get('log_config').get('logset_id')
             result['log_topic_id'] = data.get('log_config').get('topic_id')
         if data.get('authorization_enable'):
             result['authorization_enable'] = True
         if data.get('tags'):
@@ -3166,40 +3165,40 @@
                 schedule_action.ScheduleStopTime = stop_time.astimezone().isoformat()
             else:
                 schedule_action.ScheduleStopTime = stop_time
             result['scheduled_action'] = schedule_action
         return result
 
     def _create_model_service_do(self,
-                                service_group_name,
-                                worker_resource,
-                                framework=None,
-                                service_group_id=None,
-                                service_description=None,
-                                resource_group_id=None,
-                                model_config_info=None,
-                                model_cos_path=None,
-                                volume_mount=None,
-                                service_limit=None,
-                                scheduled_action=None,
-                                model_hot_update_enable=False,
-                                env=None,
-                                scale_mode="MANUAL",
-                                replicas=1,
-                                horizontal_pod_autoscaler=None,
-                                log_enable=False,
-                                log_logset_id=None,
-                                log_topic_id=None,
-                                authorization_enable=False,
-                                tags=None,
-                                cron_scale_jobs=None,
-                                scale_strategy=None,
-                                hybrid_billing_prepaid_replicas=None,
-                                command=None,
-                                new_version=False):
+                                 service_group_name,
+                                 worker_resource,
+                                 framework=None,
+                                 service_group_id=None,
+                                 service_description=None,
+                                 resource_group_id=None,
+                                 model_config_info=None,
+                                 model_cos_path=None,
+                                 volume_mount=None,
+                                 service_limit=None,
+                                 scheduled_action=None,
+                                 model_hot_update_enable=False,
+                                 env=None,
+                                 scale_mode="MANUAL",
+                                 replicas=1,
+                                 horizontal_pod_autoscaler=None,
+                                 log_enable=False,
+                                 log_logset_id=None,
+                                 log_topic_id=None,
+                                 authorization_enable=False,
+                                 tags=None,
+                                 cron_scale_jobs=None,
+                                 scale_strategy=None,
+                                 hybrid_billing_prepaid_replicas=None,
+                                 command=None,
+                                 new_version=False):
         """创建模型服务
 
         :param service_group_name:     服务名称
         :type service_group_name:      str
         :param worker_resource:        worker节点的配置
         :type worker_resource:         :class:`tikit.models.ModelServiceResourceConfigInfo`
         :param framework:              运行的框架环境
@@ -3262,16 +3261,16 @@
             req.Command = command
 
             if not framework:
                 if not model_config_info or not model_config_info.ModelVersionId:
                     raise ValueError("framework should not be empty when no models chosen")
                 modelInfo = self.describe_training_model_version(model_config_info.ModelVersionId)
                 framework = TiModels.FrameworkInfo.new_custom_image(
-                                                                    "PRESET",
-                                                                    modelInfo.TrainingModelVersion.ReasoningEnvironment)
+                    "PRESET",
+                    modelInfo.TrainingModelVersion.ReasoningEnvironment)
             if framework.Name == "CUSTOM":
                 req.ImageInfo = models.ImageInfo()
                 req.ImageInfo.ImageType = framework.ImageType
                 req.ImageInfo.ImageUrl = framework.ImageUrl
                 req.ImageInfo.RegistryRegion = framework.RegistryRegion
                 req.ImageInfo.RegistryId = framework.RegistryId
 
@@ -3292,15 +3291,15 @@
                     req.ModelInfo.CosPathInfo = self.parse_cos_info(model_cos_path)
                 else:
                     req.ModelInfo.CosPathInfo = model_config_info.CosPathInfo
                 req.ModelInfo.AlgorithmFramework = model_config_info.AlgorithmFramework
                 req.ModelInfo.ModelType = model_config_info.ModelType
 
             req.Env = env
-            
+
             req.VolumeMount = volume_mount
             req.ServiceLimit = service_limit
             req.ScheduledAction = scheduled_action
             req.ModelHotUpdateEnable = model_hot_update_enable
 
             worker_info = models.ResourceInfo()
             if charge_type == "PREPAID" or charge_type == "HYBRID_PAID":
@@ -3340,18 +3339,18 @@
 
         :param filename:     模型文件描述文件   
         :type filename:      str
         """
         args = self._modify_model_service_file_to_arguments(filename)
         result = self.modify_model_service(**args)
         if (result.Service and result.Service.ServiceGroupId and
-               result.Service.ServiceId):
+                result.Service.ServiceId):
             return f'success to update ModelService {result.Service.ServiceId}'
-    
-    def _modify_model_service_file_to_arguments(self, filename: str)-> dict:
+
+    def _modify_model_service_file_to_arguments(self, filename: str) -> dict:
         result = {}
         if not os.path.exists(filename):
             raise FileNotFoundError(filename)
         import yaml
         with open(filename, 'r') as infile:
             data = yaml.load(infile, Loader=yaml.SafeLoader)
 
@@ -3378,20 +3377,20 @@
                 image_info.get('image_type'),
                 image_info.get('image_url'),
                 registry_region=None if not image_info.get('registry_region') else image_info['registry_region'],
                 registry_id=None if not image_info.get('registry_id') else image_info['registry_id'],
             )
         if data.get('model_hot_update_enable'):
             result['model_hot_update_enable'] = True
-        
+
         if data.get('env'):
             result['env'] = []
             for e in data.get('env'):
                 ev = models.EnvVar()
-                ev.Name = e['name'] 
+                ev.Name = e['name']
                 ev.Value = e['value']
                 result['env'].append(ev)
 
         if data.get('replicas') is None:
             raise ValueError('replicas should not be empty')
         result['replicas'] = data['replicas']
         hybrid_billing_prepaid_replicas = data.get('hybrid_billing_prepaid_replicas')
@@ -3434,15 +3433,15 @@
                 cron_jobs.append(job)
             result['cron_scale_jobs'] = cron_jobs
         elif scale_mode == 'MANUAL' and not scale_strategy:
             pass
         else:
             message = f'invalid value: (scale_mode x scale_strategy) tuple should only be one of [(MANUAL, NONE), (AUTO, HPA), (AUTO, CRON)], but your input is ({scale_mode}, {scale_strategy})'
             raise ValueError(message)
-        
+
         if data.get('log_enable'):
             result['log_enable'] = True
             result['log_logset_id'] = data.get('log_config').get('logset_id')
             result['log_topic_id'] = data.get('log_config').get('topic_id')
         if data.get('authorization_enable'):
             result['authorization_enable'] = True
         _svc_limit = data.get('service_limit')
@@ -3471,15 +3470,14 @@
             if isinstance(stop_time, datetime.datetime):
                 schedule_action.ScheduleStopTime = stop_time.astimezone().isoformat()
             else:
                 schedule_action.ScheduleStopTime = stop_time
             result['scheduled_action'] = schedule_action
         return result
 
-
     def modify_model_service(self,
                              service_id,
                              model_config_info=None,
                              model_cos_path=None,
                              framework=None,
                              volume_mount=None,
                              service_limit=None,
@@ -3495,15 +3493,15 @@
                              log_topic_id=None,
                              service_action=None,
                              service_description=None,
                              scale_strategy=None,
                              cron_scale_jobs=None,
                              hybrid_billing_prepaid_replicas=None,
                              command=None,
-                             )->models.ModifyModelServiceResponse:
+                             ) -> models.ModifyModelServiceResponse:
         """更新模型服务版本
 
         :param service_id:                 服务版本id
         :type service_id:                  str
         :param model_config_info:          模型信息
         :type model_config_info:           :class:`tikit.models.ModelConfigInfo`
         :param model_cos_path:             模型cos信息
@@ -3544,15 +3542,15 @@
         :type cron_scale_jobs:             list of :class:`tikit.tencentcloud.tione.v20211111.models.CronScaleJob`
         :param hybrid_billing_prepaid_replicas:  混合计费模式下预付费实例数
         :type hybrid_billing_prepaid_replicas:   int
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.ModifyModelServiceResponse`
         """
 
-        try:            
+        try:
             req = models.ModifyModelServiceRequest()
             req.ServiceId = service_id
             req.Command = command
 
             if model_config_info is not None:
                 req.ModelInfo = models.ModelInfo()
                 req.ModelInfo.ModelId = model_config_info.ModelId
@@ -3572,15 +3570,15 @@
                 req.ImageInfo = models.ImageInfo()
                 req.ImageInfo.ImageType = framework.ImageType
                 req.ImageInfo.ImageUrl = framework.ImageUrl
                 req.ImageInfo.RegistryRegion = framework.RegistryRegion
                 req.ImageInfo.RegistryId = framework.RegistryId
 
             req.Env = env
-            
+
             req.VolumeMount = volume_mount
             req.ServiceLimit = service_limit
             req.ScheduledAction = scheduled_action
             req.ModelHotUpdateEnable = model_hot_update_enable
 
             worker_info = models.ResourceInfo()
             if worker_resource:
@@ -3610,15 +3608,15 @@
             if req.Command is not None:
                 req.CommandBase64 = base64.b64encode(req.Command.encode()).decode("utf-8")
 
             print(req._serialize())
             return self._tione_client.ModifyModelService(req)
         except TencentCloudSDKException as err:
             raise
-        
+
     def patch_model_service(self,
                             service_id,
                             model_config_info=None,
                             model_cos_path=None,
                             framework=None,
                             volume_mount=None,
                             service_limit=None,
@@ -3677,26 +3675,24 @@
         :param scale_strategy:             自动伸缩策略
         :type scale_strategy:              str
         :param cron_scale_jobs:            自动伸缩策略配置 HPA
         :type cron_scale_jobs:             list of :class:`tikit.tencentcloud.tione.v20211111.models.CronScaleJob`
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.ModifyModelServiceResponse`
         """
-        
-        
 
         try:
             query_req = models.DescribeModelServiceRequest()
             query_req.ServiceId = service_id
             query_rsp = self._tione_client.DescribeModelService(query_req)
             if isinstance(query_rsp, TencentCloudSDKException):
                 # error
                 raise
             oldService = query_rsp.Service
-            
+
             req = models.ModifyModelServiceRequest()
             req.ServiceId = service_id
 
             if model_config_info is not None:
                 req.ModelInfo = models.ModelInfo()
                 req.ModelInfo.ModelId = model_config_info.ModelId
                 req.ModelInfo.ModelName = model_config_info.ModelName
@@ -3718,105 +3714,104 @@
                 req.ImageInfo.ImageType = framework.ImageType
                 req.ImageInfo.ImageUrl = framework.ImageUrl
                 req.ImageInfo.RegistryRegion = framework.RegistryRegion
                 req.ImageInfo.RegistryId = framework.RegistryId
             else:
                 req.ImageInfo = oldService.ServiceInfo.ImageInfo
 
-            
             if env is not None:
                 req.Env = env
             else:
                 req.Env = oldService.ServiceInfo.Env
-            
+
             if volume_mount is not None:
                 req.VolumeMount = volume_mount
             else:
                 req.VolumeMount = oldService.ServiceInfo.VolumeMount
-                
+
             if service_limit is not None:
                 req.ServiceLimit = service_limit
             else:
                 req.ServiceLimit = oldService.ServiceLimit
-                
+
             if scheduled_action is not None:
                 req.ScheduledAction = scheduled_action
             else:
                 req.ScheduledAction = oldService.ScheduledAction
-                
+
             if model_hot_update_enable is not None:
                 req.ModelHotUpdateEnable = model_hot_update_enable
             else:
                 req.ModelHotUpdateEnable = oldService.ServiceInfo.ModelHotUpdateEnable
-            
+
             if oldService.ChargeType == "PREPAID":
                 worker_info = models.ResourceInfo()
                 if worker_resource is not None:
                     worker_info.Cpu = worker_resource.Cpu
                     worker_info.Memory = worker_resource.Memory
                     worker_info.Gpu = worker_resource.Gpu
                     worker_info.GpuType = worker_resource.GpuType
                 else:
                     worker_info = oldService.ServiceInfo.Resources
                 req.Resources = worker_info
             else:
                 if worker_resource is not None:
                     req.InstanceType = worker_resource.InstanceType
                 else:
-                    req.InstanceType = oldService.ServiceInfo.InstanceType       
+                    req.InstanceType = oldService.ServiceInfo.InstanceType
 
             if req.ScaleMode is not None:
                 req.ScaleMode = scale_mode
             else:
                 req.ScaleMode = oldService.ServiceInfo.ScaleMode
-            
+
             if req.Replicas is not None:
                 req.Replicas = replicas
             else:
                 req.Replicas = oldService.ServiceInfo.Replicas
-                
+
             if horizontal_pod_autoscaler is not None:
                 req.HorizontalPodAutoscaler = horizontal_pod_autoscaler
             else:
                 req.HorizontalPodAutoscaler = oldService.ServiceInfo.HorizontalPodAutoscaler
-            
+
             if log_enable is not None:
                 req.LogEnable = log_enable
                 if log_enable:
                     req.LogConfig = models.LogConfig()
                 req.LogConfig.LogsetId = log_logset_id
                 req.LogConfig.TopicId = log_topic_id
             else:
                 req.LogEnable = oldService.ServiceInfo.LogEnable
                 if log_enable:
                     req.LogConfig = models.LogConfig()
                 req.LogConfig.LogsetId = oldService.ServiceInfo.LogConfig.LogsetId
                 req.LogConfig.TopicId = oldService.ServiceInfo.LogConfig.TopicId
-                
+
             req.ServiceAction = service_action
             if service_description is not None:
                 req.ServiceDescription = service_description
             else:
                 req.ServiceDescription = oldService.ServiceDescription
-            
+
             if scale_strategy is not None:
                 req.ScaleStrategy = scale_strategy
             else:
                 req.ScaleStrategy = oldService.ServiceInfo.ScaleStrategy
-                
+
             if cron_scale_jobs is not None:
                 req.CronScaleJobs = cron_scale_jobs
             else:
                 req.CronScaleJobs = oldService.ServiceInfo.CronScaleJobs
 
             print(req._serialize())
             return self._tione_client.ModifyModelService(req)
         except TencentCloudSDKException as err:
             raise
-    
+
     def scale_model_service(self,
                             service_id,
                             scale_mode="MANUAL",
                             replicas=1,
                             horizontal_pod_autoscaler=None,
                             scale_strategy=None,
                             cron_scale_jobs=None):
@@ -3847,46 +3842,44 @@
             req.ServiceAction = "SCALE"
             req.ScaleStrategy = scale_strategy
             req.CronScaleJobs = cron_scale_jobs
             print(req._serialize())
             return self._tione_client.ModifyModelService(req)
         except TencentCloudSDKException as err:
             raise
-    
-    
-    
+
     def describe_api_configs(self, service_group_id: str) -> models.DescribeAPIConfigsResponse:
         """查看服务对应的API
 
         :param service_group_id: 服务id
         :type service_group_id: str
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.DescribeAPIConfigsResponse`
         """
         req = models.DescribeAPIConfigsRequest()
         f = models.Filter()
         f.Name = 'ServiceGroupId'
         f.Values = [service_group_id]
         req.Filters = [f]
-        try: 
+        try:
             return self._tione_client.DescribeAPIConfigs(req)
         except TencentCloudSDKException as err:
             raise
 
     def describe_service_call_info(self, service_group_id: str) -> models.DescribeModelServiceCallInfoResponse:
         """查看服务对应的调用信息
 
         :param service_group_id: 服务id
         :type service_group_id: str
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.DescribeModelServiceCallInfoResponse`
         """
         req = models.DescribeModelServiceCallInfoRequest()
         req.ServiceGroupId = service_group_id
-        try: 
+        try:
             return self._tione_client.DescribeModelServiceCallInfo(req)
         except TencentCloudSDKException as err:
             raise
 
     def describe_taiji_model_service_call_info(self, service_id: str):
         """查看太极混元模型调用信息
 
@@ -3898,16 +3891,15 @@
         req = models.DescribeModelServiceCallInfoRequest()
         req.ServiceGroupId = service_id.rstrip("-1")
         req.ServiceCategory = "TAIJI_HY"
         try:
             return self._tione_client.DescribeModelServiceCallInfo(req)
         except TencentCloudSDKException as err:
             raise
-    
-    
+
     def get_model_service_summary(self):
         """查询所有服务的概要
 
         :return:
         :rtype: list
         """
         resp = self.describe_model_service_groups()
@@ -3927,15 +3919,15 @@
                     'ServiceId': svc_id,
                     'Description': svc_desc,
                     'ChargeType': charge_type,
                 })
         return svcs
 
     def describe_taiji_model_service_groups(self, filters=None, order_field=None, order=None, offset=None, limit=None,
-                                 tag_filters=None):
+                                            tag_filters=None):
         """查看太极混元所有在线推理服务
 
         :param filters: 过滤器
         :type filters: list of Filter
         :param order_field: 排序字段
         :type order_field: str
         :param order: 排序方式，ASC/DESC
@@ -3959,15 +3951,15 @@
             req.TagFilters = tag_filters
             req.ServiceCategory = "TAIJI_HY"
             return self._tione_client.DescribeModelServiceGroups(req)
         except TencentCloudSDKException as err:
             raise
 
     def describe_model_service_groups(self, filters=None, order_field=None, order=None, offset=None, limit=None,
-                                 tag_filters=None):
+                                      tag_filters=None):
         """查看所有在线推理服务
 
         :param filters: 过滤器
         :type filters: list of Filter
         :param order_field: 排序字段
         :type order_field: str
         :param order: 排序方式，ASC/DESC
@@ -4005,15 +3997,15 @@
             req = models.DescribeModelServiceGroupRequest()
             req.ServiceGroupId = service_group_id
             return self._tione_client.DescribeModelServiceGroup(req)
         except TencentCloudSDKException as err:
             raise
 
     def describe_model_services(self, filters=None, order_field=None, order=None, offset=None, limit=None,
-                                 tag_filters=None):
+                                tag_filters=None):
         """查询多个服务版本
 
         :param filters: 过滤器
         :type filters: list of Filter
         :param order_field: 排序字段
         :type order_field: str
         :param order: 排序方式，ASC/DESC
@@ -4050,15 +4042,15 @@
         try:
             req = models.DescribeModelServiceRequest()
             req.ServiceId = service_id
             return self._tione_client.DescribeModelService(req)
         except TencentCloudSDKException as err:
             raise
 
-    def stop_model_service(self, service_id:str):
+    def stop_model_service(self, service_id: str):
         """关闭服务版本
 
         :param service_id: 服务版本id
         :type service_id: str
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.ModifyModelServiceResponse`
         """
@@ -4129,15 +4121,15 @@
                 entry.ServiceId = service_id
                 entry.Weight = weight
                 req.Weights.append(entry)
             return self._tione_client.ModifyServiceGroupWeights(req)
         except TencentCloudSDKException as err:
             raise
 
-    def get_service_group_id_by_name(self, name: str)->str:
+    def get_service_group_id_by_name(self, name: str) -> str:
         """根据服务名字查询服务ID
 
         :param name: 服务名字
         :type order: str
         :return:
         :rtype: str
         """
@@ -4148,36 +4140,36 @@
         f.Values = [name]
         resp = self.describe_model_service_groups(filters=[f])
         if len(resp.ServiceGroups) > 1:
             raise ValueError(f'name should be unique, but {len(resp.ServiceGroups)} service groups found')
         if len(resp.ServiceGroups) == 1:
             return resp.ServiceGroups[0].ServiceGroupId
         return name
-    
-    def describe_infer_templates(self)->models.DescribeInferTemplatesResponse:
+
+    def describe_infer_templates(self) -> models.DescribeInferTemplatesResponse:
         """查询推理框架信息
 
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.DescribeInferTemplatesResponse`
         """
         try:
             req = models.DescribeInferTemplatesRequest()
             return self._tione_client.DescribeInferTemplates(req)
         except TencentCloudSDKException as err:
             raise
-    
-    def describe_reasoning_env(self)->models.DescribeInferTemplatesResponse:
+
+    def describe_reasoning_env(self) -> models.DescribeInferTemplatesResponse:
         """查询推理环境信息
 
         :return:
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.DescribeInferTemplatesResponse`
         """
         return self.describe_infer_templates()
-    
-    def get_service_id_by_name(self, name: str, version: str)->str:
+
+    def get_service_id_by_name(self, name: str, version: str) -> str:
         """根据服务版本名字查询服务版本ID
 
         :param name: 服务版本名字
         :type order: str
         :return:
         :rtype: str
         """
@@ -4219,17 +4211,16 @@
         return {
             "secret_id": self._secret_id,
             "secret_key": self._secret_key,
             "region": self._region,
             "tione_client": self._tione_client
         }
 
-    
     def describe_model_accelerate_tasks(self, filters=None, order_field=None, order=None, offset=None, limit=None,
-                                 tag_filters=None):
+                                        tag_filters=None):
         """查看加速任务列表
 
         :param filters:         过滤器
         :type filters:          list of Filter
         :param order_field:     排序字段
         :type order_field:      str
         :param order:           排序方式，ASC/DESC
@@ -4251,31 +4242,30 @@
             req.Offset = offset
             req.Limit = limit
             req.TagFilters = tag_filters
             return self._tione_client.DescribeModelAccelerateTasks(req)
         except TencentCloudSDKException as err:
             raise
 
-    
     def create_model_accelerate_task(self,
-                             model_acc_task_name,
-                             model_source,
-                             model_format,
-                             model_name,
-                             model_version,
-                             model_input_path,
-                             model_output_path,
-                             tensor_infos,
-                             acc_engine_version = None,
-                             optimization_level = None,
-                             gpu_type = None,
-                             hyper_parameter = None,
-                             tags = None,
-                             model_signature = None,
-                             framework_version = None):
+                                     model_acc_task_name,
+                                     model_source,
+                                     model_format,
+                                     model_name,
+                                     model_version,
+                                     model_input_path,
+                                     model_output_path,
+                                     tensor_infos,
+                                     acc_engine_version=None,
+                                     optimization_level=None,
+                                     gpu_type=None,
+                                     hyper_parameter=None,
+                                     tags=None,
+                                     model_signature=None,
+                                     framework_version=None):
         """创建模型加速任务
 
         :param model_acc_task_name:        任务名称
         :type model_acc_task_name:         str
         :param model_source:               模型来源(JOB/COS)
         :type model_source:                str
         :param model_format:               模型格式(TORCH_SCRIPT/DETECTRON2/SAVED_MODEL/FROZEN_GRAPH/MMDETECTION/ONNX/HUGGING_FACE)
@@ -4309,119 +4299,113 @@
             req.ModelAccTaskName = model_acc_task_name
             req.ModelSource = model_source
             self._set_cos_input_path_info(req, model_input_path)
             self._set_cos_path_info(req, model_output_path)
             req.ModelName = model_name
             req.ModelVersion = model_version
             req.ModelFormat = model_format
-            
+
             if gpu_type is not None:
                 req.GPUType = gpu_type
             if optimization_level is not None:
                 req.OptimizationLevel = optimization_level
-            
+
             if acc_engine_version is not None:
                 req.AccEngineVersion = acc_engine_version
             else:
                 req.AccEngineVersion = self._describe_model_acc_engine_version(req.ModelFormat)
             req.TensorInfos = tensor_infos
             req.HyperParameter = hyper_parameter
             req.Tags = tags
             req.ModelSignature = model_signature
             req.FrameworkVersion = framework_version
 
             return self._tione_client.CreateModelAccelerateTask(req)
         except TencentCloudSDKException as err:
             raise
-    
 
     def _set_cos_input_path_info(self, req, model_input_path):
         if isinstance(model_input_path, str):
             req.ModelInputPath = self.parse_cos_info(model_input_path)
             return
         cos_path_info = models.CosPathInfo()
         cos_path_info.Bucket = model_input_path.Bucket
         cos_path_info.Region = model_input_path.Region
         cos_path_info.Paths = [model_input_path.Path]
         cos_path_info.Uin = model_input_path.Uin
         cos_path_info.SubUin = model_input_path.SubUin
         req.ModelInputPath = cos_path_info
-    
-    
+
     def _describe_model_acc_engine_version(self, model_format):
         versions = self.describe_model_acc_engine_versions()
         ret = "v1.0"
         for engine_version in versions.ModelAccEngineVersions:
             if model_format == engine_version.ModelFormat:
                 for version in engine_version.EngineVersions:
                     if len(version.Version) > len(ret) or (len(version.Version) == len(ret) and version.Version > ret):
                         ret = version.Version
         return ret
 
-    
     def describe_model_accelerate_task(self, model_acc_task_id):
         """查询模型加速任务详情
 
         :param model_acc_task_id:        模型加速任务id
         :type model_acc_task_id:         str
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.DescribeModelAccelerateTaskResponse` 
         """
         try:
             req = models.DescribeModelAccelerateTaskRequest()
             req.ModelAccTaskId = model_acc_task_id
             return self._tione_client.DescribeModelAccelerateTask(req)
         except TencentCloudSDKException as err:
             raise
 
-
     def stop_model_accelerate_task(self, model_acc_task_id):
         """停止模型加速任务
 
         :param model_acc_task_id:        模型加速任务id
         :type model_acc_task_id:         str
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.StopModelAccelerateTaskResponse` 
         """
         try:
             req = models.StopModelAccelerateTaskRequest()
             req.ModelAccTaskId = model_acc_task_id
             return self._tione_client.StopModelAccelerateTask(req)
         except TencentCloudSDKException as err:
             raise
 
-
     def delete_model_accelerate_task(self, model_acc_task_id):
         """删除模型加速任务
 
         :param model_acc_task_id:        模型加速任务id
         :type model_acc_task_id:         str
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.DeleteModelAccelerateTaskResponse` 
         """
         try:
             req = models.DeleteModelAccelerateTaskRequest()
             req.ModelAccTaskId = model_acc_task_id
             return self._tione_client.DeleteModelAccelerateTask(req)
         except TencentCloudSDKException as err:
             raise
 
-    
     def restart_model_accelerate_task(self,
-                             model_acc_task_id,
-                             model_source,
-                             model_format,
-                             model_name,
-                             model_version,
-                             model_input_path,
-                             model_output_path,
-                             tensor_infos,
-                             acc_engine_version = None,
-                             optimization_level = None,
-                             gpu_type = None,
-                             hyper_parameter = None,
-                             tags = None,
-                             model_signature = None):
+                                      model_acc_task_id,
+                                      model_source,
+                                      model_format,
+                                      model_name,
+                                      model_version,
+                                      model_input_path,
+                                      model_output_path,
+                                      tensor_infos,
+                                      acc_engine_version=None,
+                                      optimization_level=None,
+                                      gpu_type=None,
+                                      hyper_parameter=None,
+                                      tags=None,
+                                      model_signature=None):
         """重启模型加速任务
         :param model_acc_task_id:        任务id
         :type model_acc_task_id:         str
         :param model_source:             模型来源(JOB/COS)
         :type model_source:              str
         :param model_format:             模型格式(TORCH_SCRIPT/DETECTRON2/SAVED_MODEL/FROZEN_GRAPH/MMDETECTION/ONNX/HUGGING_FACE)
         :type model_format:              str
@@ -4472,17 +4456,16 @@
             req.HyperParameter = hyper_parameter
             req.Tags = tags
             req.ModelSignature = model_signature
 
             return self._tione_client.RestartModelAccelerateTask(req)
         except TencentCloudSDKException as err:
             raise
-     
 
-    def create_optimized_model(self, model_acc_task_id, tags = None):
+    def create_optimized_model(self, model_acc_task_id, tags=None):
         """保存优化模型
 
         :param model_acc_task_id:        模型加速任务id
         :type model_acc_task_id:         str
         :param tags:                     标签
         :type tags:                      list of :class:`tikit.tencentcloud.tione.v20211111.models.Tag`
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.CreateOptimizedModelResponse`
@@ -4490,35 +4473,33 @@
         try:
             req = models.CreateOptimizedModelRequest()
             req.ModelAccTaskId = model_acc_task_id
             req.Tags = tags
             return self._tione_client.CreateOptimizedModel(req)
         except TencentCloudSDKException as err:
             raise
-      
 
     def describe_model_acc_engine_versions(self):
         """查询模型加速引擎版本列表
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.DescribeModelAccEngineVersionsResponse`
         """
         try:
             req = models.DescribeModelAccEngineVersionsRequest()
             return self._tione_client.DescribeModelAccEngineVersions(req)
         except TencentCloudSDKException as err:
             raise
 
-    
     def create_batch_model_acc_tasks(self,
-                                    model_acc_task_name,
-                                    batch_model_acc_tasks,
-                                    model_output_path,
-                                    optimization_level = None,
-                                    gpu_type = None,
-                                    hyper_parameter = None,
-                                    tags = None):
+                                     model_acc_task_name,
+                                     batch_model_acc_tasks,
+                                     model_output_path,
+                                     optimization_level=None,
+                                     gpu_type=None,
+                                     hyper_parameter=None,
+                                     tags=None):
         """批量创建模型加速任务
 
         :param model_acc_task_name:        任务名称
         :type model_acc_task_name:         str
         :param batch_model_acc_tasks:      批量模型加速任务
         :type batch_model_acc_tasks:       list of tikit.tencentcloud.tione.v20211111.models.BatchModelAccTask
         :param model_output_path:          模型加速保存路径
@@ -4541,20 +4522,19 @@
                 req.GPUType = gpu_type
             if optimization_level is not None:
                 req.OptimizationLevel = optimization_level
             req.HyperParameter = hyper_parameter
             req.Tags = tags
             if batch_model_acc_tasks is not None:
                 self._set_batch_model_acc_task(req, batch_model_acc_tasks)
-            
+
             return self._tione_client.CreateBatchModelAccTasks(req)
         except TencentCloudSDKException as err:
             raise
 
-    
     def _set_batch_model_acc_task(self, req, batch_model_acc_tasks):
         batch_tasks = []
         for batch_model_acc_task in batch_model_acc_tasks:
             batch_task = models.BatchModelAccTask()
             batch_task.ModelName = batch_model_acc_task.ModelName
             batch_task.ModelVersion = batch_model_acc_task.ModelVersion
             batch_task.ModelFormat = batch_model_acc_task.ModelFormat
@@ -4563,17 +4543,17 @@
             batch_task.TensorInfos = batch_model_acc_task.TensorInfos
             batch_task.ModelSignature = batch_model_acc_task.ModelSignature
 
             if batch_model_acc_task.AccEngineVersion is not None:
                 batch_task.AccEngineVersion = batch_model_acc_task.AccEngineVersion
             else:
                 batch_task.AccEngineVersion = self._describe_model_acc_engine_version(batch_task.ModelFormat)
-            
+
             batch_tasks.append(batch_task)
-        
+
         req.BatchModelAccTasks = batch_tasks
 
     def describe_model_acc_optimized_report(self, model_acc_task_id):
         """查询模型加速任务效果报告
 
         :param model_acc_task_id: 模型加速任务id
         :type model_acc_task_id: str
@@ -4581,33 +4561,170 @@
         """
         try:
             req = models.DescribeModelAccOptimizedReportRequest()
             req.ModelAccTaskId = model_acc_task_id
             return self._tione_client.DescribeModelAccOptimizedReport(req)
         except TencentCloudSDKException as err:
             raise
-    def describe_taiji_template(self, template_id) :
+
+    def describe_taiji_template(self, template_id):
         """查询Taiji训练模板
 
         :param template_id: 训练模板id
         :type template_id: str
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.DescribeTAIJITemplateResponse`
         """
         try:
             req = models.DescribeTAIJITemplateRequest()
             req.TemplateId = template_id
             return self._tione_client.DescribeTAIJITemplate(req)
         except TencentCloudSDKException as err:
             raise
-    
-    def describe_taiji_template_list(self) :
+
+    def describe_taiji_template_list(self):
         """查询Taiji训练模板列表 
         :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.DescribeTAIJITemplateListResponse`
         """
         try:
             req = models.DescribeTAIJITemplateListRequest()
             return self._tione_client.DescribeTAIJITemplateList(req)
         except TencentCloudSDKException as err:
             raise
-             
 
+    def create_notebook(self,
+                        name,
+                        image_info=None,
+                        resource_info=None,
+                        input_data_config=None,
+                        ssh_config=None,
+                        tags=None,
+                        resource_group_id="",
+                        vpc_id=None,
+                        subnet_id=None):
+        """创建Notebook实例
+        :param name:        实例名称
+        :type name:         str
+        :param image_info:   实例镜像信息
+        :type image_info:    :class:`tikit.models.ImageInfo`
+        :param resource_info:     实例资源配置配置
+        :type resource_info:      :class:`tikit.models.ResourceConfigInfo`
+        :param input_data_config:   输入的存储信息
+        :type input_data_config:    list or :class:`tikit.models.NotebookDataConfig`
+        :param ssh_config:  ssh配置信息
+        :type ssh_config:   :class:`tikit.models.SSHConfig`
+        :param tags:                标签
+        :type tags:                 list of :class:`tikit.tencentcloud.tione.v20211111.models.Tag`
+        :param resource_group_id:   预付费的资源组id
+        :type resource_group_id:    str
+        :param vpc_id:   挂载cfs或者turbofs时，需要打通的vpc_id
+        :type vpc_id:    str
+        :param subnet_id:   挂载cfs或者turbofs时，vpc下的subnet
+        :type subnet_id:    str
+        :return:
+        :rtype: :class:`tikit.tencentcloud.tione.v20211111.models.CreateTrainingTaskResponse`
+        """
+        try:
+            req = models.CreateNotebookRequest()
+            req.Name = name
+            req.AutoStopping = False
+            req.AutomaticStopTime = 1
+            req.ChargeType = "PREPAID"
+            req.DirectInternetAccess = True
+            req.LogEnable = False
+            req.ResourceGroupId = resource_group_id
+            req.Tags = tags
+            req.RootAccess = True
+            if vpc_id is not None:
+                req.VpcId = vpc_id
+            if subnet_id is not None:
+                req.SubnetId = subnet_id
+
+            # 构造ImageInfo参数
+            req.ImageInfo = models.ImageInfo()
+            req.ImageInfo.ImageName = image_info.ImageName
+            req.ImageInfo.ImageType = image_info.ImageType
+            req.ImageInfo.ImageUrl = image_info.ImageUrl
+            req.ImageInfo.RegistryRegion = image_info.RegistryRegion
+            req.ImageInfo.RegistryId = image_info.RegistryId
+
+            if image_info.ImageType == "SYSTEM":
+                req.ImageType = "SYSTEM"
+            else:
+                req.ImageType = "CUSTOM"
+
+            # 设置资源
+            if resource_group_id is None:
+                raise TencentCloudSDKException(
+                    message='please set resource group id')
+            req.ResourceGroupId = resource_group_id
+            resource_conf = models.ResourceConf()
+            resource_conf.Cpu = resource_info.Cpu
+            resource_conf.Gpu = resource_info.Gpu
+            resource_conf.Memory = resource_info.Memory
+            resource_conf.GpuType = resource_info.GpuType
+            req.ResourceConf = resource_conf
+
+            # 设置挂载
+            if input_data_config is None:
+                raise TencentCloudSDKException(
+                    message='please configure at least one data config')
+            else:
+                req.DataConfigs, req.VolumeSourceType = self._parse_notebook_input_data(input_data_config)
+
+            # 设置SSH配置
+            if ssh_config is not None and ssh_config.Enable:
+                req.SSHConfig = models.SSHConfig()
+                req.SSHConfig.Enable = True
+                req.SSHConfig.PublicKey = ssh_config.PublicKey
+
+            return self._tione_client.CreateNotebook(req)
+        except TencentCloudSDKException as err:
+            raise
+
+    def _parse_notebook_input_data(self, input_data_config):
+        data_configs = []
+        data_type = ""
+        for input_data_item in input_data_config:
+            data_config = self._convert_notebook_data_config(input_data_item)
+            if not data_config:
+                continue
+            data_configs.append(data_config)
+            data_type = input_data_item.DataSource
+        return data_configs, data_type
 
+    def _convert_notebook_data_config(self, input_data_item) -> models.DataConfig:
+        data_config = models.DataConfig()
+        data_config.DataSourceType = input_data_item.DataSource
+        data_config.MappingPath = input_data_item.TargetPath
+        if input_data_item.DataSource == "CFS":
+            data_config.CFSSource = models.CFSConfig()
+            assert input_data_item.CfsId
+            data_config.CFSSource.Id = input_data_item.CfsId
+            data_config.CFSSource.Path = input_data_item.CfsPath
+        elif input_data_item.DataSource == "CFS_TURBO":
+            data_config.CFSSource = models.CFSConfig()
+            assert input_data_item.CFSTurboId
+            data_config.CFSSource.Id = input_data_item.CFSTurboId
+            data_config.CFSSource.Path = input_data_item.CFSTurboPath
+        elif input_data_item.DataSource == "CLOUD_PREMIUM" or input_data_item.DataSource == "CLOUD_SSD":
+            data_config.CBSSource = models.CBSConfig()
+            assert input_data_item.VolumeSizeInGB
+            data_config.CBSSource.VolumeSizeInGB = input_data_item.VolumeSize
+        elif input_data_item.DataSource == "LOCAL_DISK":
+            data_config.LocalDiskSource = models.LocalDisk()
+            assert input_data_item.InstanceId
+            data_config.LocalDiskSource.InstanceId = input_data_item.InstanceId
+        elif input_data_item.DataSource == "GooseFS":
+            data_config.GooseFSSource = models.GooseFSSource()
+            assert input_data_item.GooseFSId
+            assert input_data_item.GooseFSNameSpace
+            data_config.GooseFSSource.Id = input_data_item.GooseFSId
+            data_config.GooseFSSource.NameSpace = input_data_item.GooseFSNameSpace
+        elif input_data_item.DataSource == "GooseFSx":
+            data_config.GooseFSSource = models.GooseFSSource()
+            assert input_data_item.GooseFSId
+            data_config.GooseFSSource.Id = input_data_item.GooseFSId
+            data_config.GooseFSSource.Path = input_data_item.GooseFSxPath
+        else:
+            print("warning! not supported DataSourceType", input_data_item.DataSource)
+            return None
+        return data_config
```

### Comparing `tikit-1.7.1.240409/tikit/default_client.py` & `tikit-1.7.1.240523/tikit/default_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/display_optimize/dataset.py` & `tikit-1.7.1.240523/tikit/display_optimize/dataset.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/display_optimize/resource_group.py` & `tikit-1.7.1.240523/tikit/display_optimize/resource_group.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/display_optimize/training_model.py` & `tikit-1.7.1.240523/tikit/display_optimize/training_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/display_optimize/training_task.py` & `tikit-1.7.1.240523/tikit/display_optimize/training_task.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/hdfs.py` & `tikit-1.7.1.240523/tikit/hdfs.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/hive.py` & `tikit-1.7.1.240523/tikit/hive.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/models.py` & `tikit-1.7.1.240523/tikit/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -583,7 +583,210 @@
         """
 
         :param model_version_id: 模型ID
         :type model_version_id: str
         """
         return ModelConfigInfo('', '', model_version_id, '', '',
                                model_type=model_type)
+
+class ImageInfo:
+    def __init__(self, image_name=None, image_type=None, image_url=None, registry_region=None, registry_id=None):
+        self.ImageName = image_name
+        self.ImageType = image_type
+        self.ImageUrl = image_url
+        self.RegistryRegion = registry_region
+        self.RegistryId = registry_id
+
+    @staticmethod
+    def new_build_in_image(image_name):
+        """内置镜像配置
+
+        :param image_name:  镜像名称
+        :type image_name:    str
+        :return:
+        :rtype:
+        """
+        return ImageInfo(image_name=image_name, image_type="SYSTEM")
+
+    @staticmethod
+    def new_custom_image(image_type, image_url, registry_region=None, registry_id=None):
+        """自定义镜像配置
+
+        :param image_type:      腾讯云容器镜像服务的镜像类型，如"CCR","TCR"
+        :type image_type:       str
+        :param image_url:       腾讯云容器镜像服务的镜像地址
+        :type image_url:        str
+        :param registry_region: 腾讯云容器镜像服务的镜像仓库的域
+        :type registry_region:  str
+        :param registry_id:     腾讯云容器镜像服务的镜像仓库ID
+        :type registry_id:      str
+        :return:
+        :rtype:
+        """
+        return ImageInfo(image_type=image_type, image_url=image_url, registry_region=registry_region, registry_id=registry_id)
+
+
+class SSHConfig:
+    def __init__(self):
+        self.Enable = False
+        self.PublicKey = None
+
+    @staticmethod
+    def new_ssh_config(public_key):
+        """新建一个高性能云硬盘类型的存储配置
+
+        :param public_key: ssh公钥信息
+        :type public_key: str
+        :return:
+        :rtype:
+        """
+        ret = SSHConfig()
+        ret.PublicKey = public_key
+        if public_key is not None and len(public_key) > 0:
+            ret.Enable = True
+        return ret
+
+class NotebookDataConfig:
+    def __init__(self):
+        self.DataSource = None
+        self.TargetPath = None
+        self.VolumeSize = None
+        self.CfsId = None
+        self.CfsPath = None
+        self.GooseFSId = None
+        self.GooseFSNameSpace = None
+        self.GooseFSxId = None
+        self.GooseFSxPath = None
+        self.CFSTurboId = None
+        self.CFSTurboPath = None
+        self.InstanceId = None
+
+    @staticmethod
+    def new_mount_cloud_premium(volume_size, target_path):
+        """新建一个高性能云硬盘类型的存储配置
+
+        :param volume_size:
+        :type volume_size: int
+        :param  target_path: 目标挂载路径
+        :type target_path: str
+        :return:
+        :rtype:
+        """
+        ret = NotebookDataConfig()
+        ret.TargetPath = target_path
+        ret.DataSource = "CLOUD_PREMIUM"
+        ret.VolumeSize = volume_size
+        return ret
+
+    @staticmethod
+    def new_mount_cloud_ssd(volume_size, target_path):
+        """新建一个SSD云硬盘类型的存储配置
+
+        :param volume_size:
+        :type volume_size: int
+        :param  target_path: 目标挂载路径
+        :type target_path: str
+        :return:
+        :rtype:
+        """
+        ret = NotebookDataConfig()
+        ret.TargetPath = target_path
+        ret.DataSource = "CLOUD_SSD"
+        ret.VolumeSize = volume_size
+        return ret
+
+    @staticmethod
+    def new_mount_cfs(cfs_id, source_path, target_path):
+        """新建一个cfs类型的存储配置
+
+        :param cfs_id:      CFS的ID
+        :type cfs_id: str
+        :param  source_path: CFS的路径
+        :type source_path: str
+        :param  target_path: 目标挂载路径
+        :type target_path: str
+        :return:
+        :rtype:
+        """
+        ret = NotebookDataConfig()
+        ret.TargetPath = target_path
+        ret.DataSource = "CFS"
+        ret.CfsId = cfs_id
+        ret.CfsPath = source_path
+        return ret
+
+    @staticmethod
+    def new_mount_goosefs(goosefs_id, namespace, target_path):
+        """新建一个goosefs类型的存储配置
+
+        :param goosefs_id: goosefs实例id
+        :type goosefs_id: str
+        :param  namespace: 命名空间
+        :type namespace: str
+        :param  target_path: 目标挂载路径
+        :type target_path: str
+        :return:
+        :rtype:
+        """
+        ret = NotebookDataConfig()
+        ret.TargetPath = target_path
+        ret.DataSource = "GooseFS"
+        ret.GooseFSNameSpace = namespace
+        ret.GooseFSId = goosefs_id
+        return ret
+
+    @staticmethod
+    def new_mount_goosefsx(goosefsx_id, goosefsx_path, target_path):
+        """新建一个goosefsx类型的存储配置
+
+        :param goosefsx_id: goosefsx实例id
+        :type goosefsx_id: str
+        :param goosefsx_path: goosefsx路径
+        :type goosefsx_path: str
+        :param  target_path: 目标挂载路径
+        :type target_path: str
+        :return:
+        :rtype:
+        """
+        ret = NotebookDataConfig()
+        ret.TargetPath = target_path
+        ret.DataSource = "GooseFSx"
+        ret.GooseFSId = goosefsx_id
+        ret.GooseFSxPath = goosefsx_path
+        return ret
+
+    @staticmethod
+    def new_mount_cfs_turbofs(cfs_turbofs_id, source_path, target_path):
+        """新建一个turbocfs类型的存储配置
+
+        :param cfs_turbofs_id: cfs_turbofs实例id
+        :type cfs_turbofs_id: str
+        :param  source_path: CFS的路径
+        :type source_path: str
+        :param  target_path: 目标挂载路径
+        :type target_path: str
+        :return:
+        :rtype:
+        """
+        ret = NotebookDataConfig()
+        ret.TargetPath = target_path
+        ret.DataSource = "CFS_TURBO"
+        ret.CFSTurboId = cfs_turbofs_id
+        ret.CFSTurboPath= source_path
+        return ret
+
+    @staticmethod
+    def new_mount_local_disk(instance_id, target_path):
+        """新建一个本地磁盘类型的存储配置
+
+        :param instance_id: 节点id
+        :type instance_id: str
+        :param  target_path: 目标挂载路径
+        :type target_path: str
+        :return:
+        :rtype:
+        """
+        ret = NotebookDataConfig()
+        ret.TargetPath = target_path
+        ret.DataSource = "LOCAL_DISK"
+        ret.InstanceId = instance_id
+        return ret
```

### Comparing `tikit-1.7.1.240409/tikit/templates/service_config.yaml` & `tikit-1.7.1.240523/tikit/templates/service_config.yaml`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/__init__.py` & `tikit-1.7.1.240523/tikit/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/common/abstract_client.py` & `tikit-1.7.1.240523/tikit/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/common/abstract_model.py` & `tikit-1.7.1.240523/tikit/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/common/common_client.py` & `tikit-1.7.1.240523/tikit/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/common/credential.py` & `tikit-1.7.1.240523/tikit/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/common/exception/__init__.py` & `tikit-1.7.1.240523/tikit/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tikit-1.7.1.240523/tikit/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/common/http/request.py` & `tikit-1.7.1.240523/tikit/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/common/profile/client_profile.py` & `tikit-1.7.1.240523/tikit/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/common/profile/http_profile.py` & `tikit-1.7.1.240523/tikit/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/common/sign.py` & `tikit-1.7.1.240523/tikit/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/emr_client.py` & `tikit-1.7.1.240523/tikit/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/errorcodes.py` & `tikit-1.7.1.240523/tikit/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/emr/v20190103/models.py` & `tikit-1.7.1.240523/tikit/tencentcloud/emr/v20190103/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/errorcodes.py` & `tikit-1.7.1.240523/tikit/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -351,7 +351,61 @@
 UNAUTHORIZEDOPERATION_NOPERMISSION = 'UnauthorizedOperation.NoPermission'
 
 # 未知参数错误。
 UNKNOWNPARAMETER = 'UnknownParameter'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
+
+# 查询预付费资源组详情失败。
+INTERNALERROR_QUERYRESOURCEGROUPFAILED = 'InternalError.QueryResourceGroupFailed'
+
+# 查询子网信息失败。
+INTERNALERROR_QUERYSUBNETINFOFAILED = 'InternalError.QuerySubnetInfoFailed'
+
+# 查询用户临时密钥失败
+INTERNALERROR_QUERYUSERTMPCREDENTIALFAILED = 'InternalError.QueryUserTMPCredentialFailed'
+
+# 数据配置数量超过最大限制
+INVALIDPARAMETERVALUE_DATACONFIGNUMLIMITEXCEEDED = 'InvalidParameterValue.DataConfigNumLimitExceeded'
+
+# 获取CFS的挂载IP失败
+INVALIDPARAMETERVALUE_GETCFSMOUNTIPFAILED = 'InvalidParameterValue.GetCFSMountIPFailed'
+
+# 获取GooseFS实例失败
+INVALIDPARAMETERVALUE_GETGOOSEFSFAILED = 'InvalidParameterValue.GetGooseFSFailed'
+
+# GooseFS的配置不能为空
+INVALIDPARAMETERVALUE_GOOSEFSCONFIGCANNOTEMPTY = 'InvalidParameterValue.GooseFSConfigCannotEmpty'
+
+# 所选的GooseFS实例不存在
+INVALIDPARAMETERVALUE_GOOSEFSNOTEXIST = 'InvalidParameterValue.GooseFSNotExist'
+
+# 裸金属资源组不支持创建免费存储的Notebook
+INVALIDPARAMETERVALUE_NOTALLOWEDTOCREATEFREEVOLUMENOTEBOOKWITHBAREMETALRESOURCEGROUP = 'InvalidParameterValue.NotAllowedToCreateFreeVolumeNotebookWithBareMetalResourceGroup'
+
+# 纳管资源组不支持cbs存储，请使用CFS
+INVALIDPARAMETERVALUE_NOTALLOWEDTOCREATEFREEVOLUMENOTEBOOKWITHSWRESOURCEGROUP = 'InvalidParameterValue.NotAllowedToCreateFreeVolumeNotebookWithSWResourceGroup'
+
+# 裸金属资源组不支持创建Notebook
+INVALIDPARAMETERVALUE_NOTALLOWEDTOCREATENOTEBOOKWITHBAREMETALRESOURCEGROUP = 'InvalidParameterValue.NotAllowedToCreateNotebookWithBareMetalResourceGroup'
+
+# 资源配置不合法
+INVALIDPARAMETERVALUE_RESOURCECONFIGILLEGAL = 'InvalidParameterValue.ResourceConfigIllegal'
+
+# 不支持使用GooseFS实例
+INVALIDPARAMETERVALUE_UNSUPPORTEDGOOSEFSCONFIG = 'InvalidParameterValue.UnsupportedGooseFSConfig'
+
+# 不支持同一实例挂载多个CBS存储
+INVALIDPARAMETERVALUE_UNSUPPORTEDMULTICBSSTORAGE = 'InvalidParameterValue.UnsupportedMultiCBSStorage'
+
+# 按量计费资源售罄。
+OPERATIONDENIED_BILLINGSTATUSRESOURCEINSUFFICIENT = 'OperationDenied.BillingStatusResourceInsufficient'
+
+# IP不合法。
+OPERATIONDENIED_IPILLEGAL = 'OperationDenied.IpIllegal'
+
+# 操作不允许
+OPERATIONDENIED_NOTALLOW = 'OperationDenied.NotAllow'
+
+# 预付费资源组余量不足。
+OPERATIONDENIED_RESOURCEGROUPINSUFFICIENT = 'OperationDenied.ResourceGroupInsufficient'
```

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/models.py` & `tikit-1.7.1.240523/tikit/tencentcloud/tione/v20211111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -817,14 +817,67 @@
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
 
 
+class CBSConfig(AbstractModel):
+    """CBS存储配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param VolumeSizeInGB: 存储大小
+注意：此字段可能返回 null，表示取不到有效值。
+        :type VolumeSizeInGB: int
+        """
+        self.VolumeSizeInGB = None
+
+    def _deserialize(self, params):
+        self.VolumeSizeInGB = params.get("VolumeSizeInGB")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+
+
+class LocalDisk(AbstractModel):
+    """本地磁盘信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 节点ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceId: str
+        :param LocalPath: 本地路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LocalPath: str
+        """
+        self.InstanceId = None
+        self.LocalPath = None
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.LocalPath = params.get("LocalPath")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+
+
 class CFSConfig(AbstractModel):
     """CFS存储的配置
 
     """
 
     def __init__(self):
         r"""
@@ -2848,21 +2901,23 @@
         :type DirectInternetAccess: bool
         :param ResourceGroupId: 资源组ID(for预付费)
         :type ResourceGroupId: str
         :param VpcId: Vpc-Id
         :type VpcId: str
         :param SubnetId: 子网Id
         :type SubnetId: str
-        :param VolumeSourceType: 存储的类型。取值包含： 
-    FREE:    预付费的免费存储
-    CLOUD_PREMIUM： 高性能云硬盘
-    CLOUD_SSD： SSD云硬盘
-    CFS:     CFS存储，包含NFS和turbo
+        :param VolumeSourceType: 存储的类型。取值包含：
+        FREE：预付费的免费存储
+        CLOUD_PREMIUM：高性能云硬盘
+        CLOUD_SSD：SSD云硬盘
+        CFS：CFS存储
+        CFS_TURBO：CFS Turbo存储
+        GooseFSx：GooseFSx存储
         :type VolumeSourceType: str
-        :param VolumeSizeInGB: 存储卷大小，单位GB
+        :param VolumeSizeInGB: 云硬盘存储卷大小，单位GB
         :type VolumeSizeInGB: int
         :param VolumeSourceCFS: CFS存储的配置
         :type VolumeSourceCFS: :class:`tencentcloud.tione.v20211111.models.CFSConfig`
         :param LogConfig: 日志配置
         :type LogConfig: :class:`tencentcloud.tione.v20211111.models.LogConfig`
         :param LifecycleScriptId: 生命周期脚本的ID
         :type LifecycleScriptId: str
@@ -2870,16 +2925,30 @@
         :type DefaultCodeRepoId: str
         :param AdditionalCodeRepoIds: 其他GIT存储库的ID，最多3个
         :type AdditionalCodeRepoIds: list of str
         :param AutomaticStopTime: 自动停止时间，单位小时
         :type AutomaticStopTime: int
         :param Tags: 标签配置
         :type Tags: list of Tag
-        :param DataConfigs: 数据配置
+        :param DataConfigs: 数据配置，只支持WEDATA_HDFS存储类型
         :type DataConfigs: list of DataConfig
+        :param UserType: 用户类型
+        :type UserType: str
+        :param UserDataInfo: 用户数据信息
+        :type UserDataInfo: :class:`tencentcloud.tione.v20211111.models.UserDataInfo`
+        :param ImageInfo: 镜像信息
+        :type ImageInfo: :class:`tencentcloud.tione.v20211111.models.ImageInfo`
+        :param ImageType: 镜像类型，包括SYSTEM、TCR、CCR
+        :type ImageType: str
+        :param SSHConfig: SSH配置信息
+        :type SSHConfig: :class:`tencentcloud.tione.v20211111.models.SSHConfig`
+        :param VolumeSourceGooseFS: GooseFS存储配置
+        :type VolumeSourceGooseFS: :class:`tencentcloud.tione.v20211111.models.GooseFS`
+        :param DataPipelineTaskId: 数据构建任务ID
+        :type DataPipelineTaskId: str
         """
         self.Name = None
         self.ChargeType = None
         self.ResourceConf = None
         self.LogEnable = None
         self.RootAccess = None
         self.AutoStopping = None
@@ -2893,14 +2962,21 @@
         self.LogConfig = None
         self.LifecycleScriptId = None
         self.DefaultCodeRepoId = None
         self.AdditionalCodeRepoIds = None
         self.AutomaticStopTime = None
         self.Tags = None
         self.DataConfigs = None
+        self.UserType = None
+        self.UserDataInfo = None
+        self.ImageInfo = None
+        self.ImageType = None
+        self.SSHConfig = None
+        self.VolumeSourceGooseFS = None
+        self.DataPipelineTaskId = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.ChargeType = params.get("ChargeType")
         if params.get("ResourceConf") is not None:
             self.ResourceConf = ResourceConf()
@@ -2932,18 +3008,34 @@
                 self.Tags.append(obj)
         if params.get("DataConfigs") is not None:
             self.DataConfigs = []
             for item in params.get("DataConfigs"):
                 obj = DataConfig()
                 obj._deserialize(item)
                 self.DataConfigs.append(obj)
+        self.UserType = params.get("UserType")
+        if params.get("UserDataInfo") is not None:
+            self.UserDataInfo = UserDataInfo()
+            self.UserDataInfo._deserialize(params.get("UserDataInfo"))
+        if params.get("ImageInfo") is not None:
+            self.ImageInfo = ImageInfo()
+            self.ImageInfo._deserialize(params.get("ImageInfo"))
+        self.ImageType = params.get("ImageType")
+        if params.get("SSHConfig") is not None:
+            self.SSHConfig = SSHConfig()
+            self.SSHConfig._deserialize(params.get("SSHConfig"))
+        if params.get("VolumeSourceGooseFS") is not None:
+            self.VolumeSourceGooseFS = GooseFS()
+            self.VolumeSourceGooseFS._deserialize(params.get("VolumeSourceGooseFS"))
+        self.DataPipelineTaskId = params.get("DataPipelineTaskId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class CreateNotebookResponse(AbstractModel):
     """CreateNotebook返回参数结构体
@@ -3752,25 +3844,33 @@
         :type AIMarketAlgoPreModelSource: :class:`tencentcloud.tione.v20211111.models.AIMarketAlgoPreModelSource`
         :param GooseFSSource: 来自GooseFS的数据
 注意：此字段可能返回 null，表示取不到有效值。
         :type GooseFSSource: :class:`tencentcloud.tione.v20211111.models.GooseFSSource`
         :param CFSTurboSource: 来自CFSTurbo的数据
 注意：此字段可能返回 null，表示取不到有效值。
         :type CFSTurboSource: :class:`tencentcloud.tione.v20211111.models.CFSTurboSource`
+        :param LocalDiskSource: 来自本地磁盘的信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LocalDiskSource: :class:`tencentcloud.tione.v20211111.models.LocalDisk`
+        :param CBSSource: CBS配置信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CBSSource: :class:`tencentcloud.tione.v20211111.models.CBSConfig`
         """
         self.MappingPath = None
         self.DataSourceType = None
         self.DataSetSource = None
         self.COSSource = None
         self.CFSSource = None
         self.HDFSSource = None
         self.WeDataHDFSSource = None
         self.AIMarketAlgoPreModelSource = None
         self.GooseFSSource = None
         self.CFSTurboSource = None
+        self.LocalDiskSource = None
+        self.CBSSource = None
 
 
     def _deserialize(self, params):
         self.MappingPath = params.get("MappingPath")
         self.DataSourceType = params.get("DataSourceType")
         if params.get("DataSetSource") is not None:
             self.DataSetSource = DataSetConfig()
@@ -3792,21 +3892,153 @@
             self.AIMarketAlgoPreModelSource._deserialize(params.get("AIMarketAlgoPreModelSource"))
         if params.get("GooseFSSource") is not None:
             self.GooseFSSource = GooseFSSource()
             self.GooseFSSource._deserialize(params.get("GooseFSSource"))
         if params.get("CFSTurboSource") is not None:
             self.CFSTurboSource = CFSTurboSource()
             self.CFSTurboSource._deserialize(params.get("CFSTurboSource"))
+        if params.get("LocalDiskSource") is not None:
+            self.LocalDiskSource = LocalDisk()
+            self.LocalDiskSource._deserialize(params.get("LocalDiskSource"))
+        if params.get("CBSSource") is not None:
+            self.CBSSource = CBSConfig()
+            self.CBSSource._deserialize(params.get("CBSSource"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
+
+
+class GooseFS(AbstractModel):
+    """配置GooseFS参数
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Id: goosefs实例id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param Type: GooseFS类型，包括GooseFS和GooseFSx
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: str
+        :param Path: GooseFSx实例需要挂载的路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Path: str
+        """
+        self.Id = None
+        self.Type = None
+        self.Path = None
+
+    def _deserialize(self, params):
+        self.Id = params.get("Id")
+        self.Type = params.get("Type")
+        self.Path = params.get("Path")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+
+
+class SSHConfig(AbstractModel):
+    """notebook ssh端口配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Enable: 是否开启ssh
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Enable: bool
+        :param PublicKey: 公钥信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PublicKey: str
+        :param Port: 端口号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Port: int
+        :param LoginCommand: 登录命令
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LoginCommand: str
+        """
+        self.Enable = None
+        self.PublicKey = None
+        self.Port = None
+        self.LoginCommand = None
+
+    def _deserialize(self, params):
+        self.Enable = params.get("Enable")
+        self.PublicKey = params.get("PublicKey")
+        self.Port = params.get("Port")
+        self.LoginCommand = params.get("LoginCommand")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+
+
+class UserDataInfo(AbstractModel):
+    """用户数据
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _AiMarketInfo: ai市场cos自动下载配置
+        :type AiMarketInfo: :class:`tencentcloud.tione.v20211111.models.AiMarketInfo`
+        """
+        self.AiMarketInfo = None
+
+    def _deserialize(self, params):
+        if params.get("AiMarketInfo") is not None:
+            self.AiMarketInfo = AiMarketInfo()
+            self.AiMarketInfo._deserialize(params.get("AiMarketInfo"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+
+
+class AiMarketInfo(AbstractModel):
+    """ai市场cos信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AlgorithmCosConfig: 算法cos信息
+        :type AlgorithmCosConfig: :class:`tencentcloud.tione.v20211111.models.CosPathInfo`
+        """
+        self.AlgorithmCosConfig = None
+
+    @property
+    def AlgorithmCosConfig(self):
+        return self.AlgorithmCosConfig
+
+    def _deserialize(self, params):
+        if params.get("AlgorithmCosConfig") is not None:
+            self.AlgorithmCosConfig = CosPathInfo()
+            self.AlgorithmCosConfig._deserialize(params.get("AlgorithmCosConfig"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
 
 
 class DataPoint(AbstractModel):
     """数据点
 
     """
 
@@ -13011,32 +13243,36 @@
 class ImageInfo(AbstractModel):
     """镜像描述信息
 
     """
 
     def __init__(self):
         r"""
+        :param ImageName: 镜像名称
+        :type ImageName: str
         :param ImageType: 镜像类型：TCR为腾讯云TCR镜像; CCR为腾讯云TCR个人版镜像，PreSet为平台预置镜像
         :type ImageType: str
         :param ImageUrl: 镜像地址
         :type ImageUrl: str
         :param RegistryRegion: TCR镜像对应的地域
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegistryRegion: str
         :param RegistryId: TCR镜像对应的实例id
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegistryId: str
         """
+        self.ImageName = None
         self.ImageType = None
         self.ImageUrl = None
         self.RegistryRegion = None
         self.RegistryId = None
 
 
     def _deserialize(self, params):
+        self.ImageName =  params.get("ImageName")
         self.ImageType = params.get("ImageType")
         self.ImageUrl = params.get("ImageUrl")
         self.RegistryRegion = params.get("RegistryRegion")
         self.RegistryId = params.get("RegistryId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
@@ -21446,27 +21682,36 @@
 
     """
 
     def __init__(self):
         r"""
         :param Id: GooseFS实例的ID
         :type Id: string
+        :param Path: GooseFSx实例需要挂载的路径
+        :type Path: str
+        :param NameSpace: GooseFS命名空间
+        :type NameSpace: string
         """
         self.Id = None
+        self.NameSpace = None
+        self.Path = None
 
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
+        self.NameSpace = params.get("NameSpace")
+        self.Path = params.get("Path")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
 
+
 class CFSTurboSource(AbstractModel):
     """CFSTurbo的配置
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/tione/v20211111/tione_client.py` & `tikit-1.7.1.240523/tikit/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/errorcodes.py` & `tikit-1.7.1.240523/tikit/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/models.py` & `tikit-1.7.1.240523/tikit/tencentcloud/wedata/v20210820/models.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/tencentcloud/wedata/v20210820/wedata_client.py` & `tikit-1.7.1.240523/tikit/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit/util.py` & `tikit-1.7.1.240523/tikit/util.py`

 * *Files identical despite different names*

### Comparing `tikit-1.7.1.240409/tikit.egg-info/SOURCES.txt` & `tikit-1.7.1.240523/tikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

