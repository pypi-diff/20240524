# Comparing `tmp/neuro-extras-24.2.0.tar.gz` & `tmp/neuro-extras-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-extras-24.2.0.tar", last modified: Tue Feb 13 13:59:09 2024, max compression
+gzip compressed data, was "neuro-extras-24.5.0.tar", last modified: Fri May 24 15:34:33 2024, max compression
```

## Comparing `neuro-extras-24.2.0.tar` & `neuro-extras-24.5.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 13:59:09.870845 neuro-extras-24.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-13 13:59:09.870845 neuro-extras-24.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 13:59:09.862845 neuro-extras-24.2.0/neuro_extras/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 13:59:09.866845 neuro-extras-24.2.0/neuro_extras/assets/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1214 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/assets/merge_docker_auths.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 13:59:09.866845 neuro-extras-24.2.0/neuro_extras/assets/seldon.package/
--rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/assets/seldon.package/seldon.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/assets/seldon.package/seldon_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 13:59:09.866845 neuro-extras-24.2.0/neuro_extras/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/data/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/data/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    12534 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/data/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/data/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/data/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/data/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/data/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/data/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/data/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/data/web.py
--rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/image_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/seldon.py
--rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/neuro_extras/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 13:59:09.866845 neuro-extras-24.2.0/neuro_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-13 13:59:09.000000 neuro-extras-24.2.0/neuro_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-02-13 13:59:09.000000 neuro-extras-24.2.0/neuro_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 13:59:09.000000 neuro-extras-24.2.0/neuro_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-13 13:59:09.000000 neuro-extras-24.2.0/neuro_extras.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 13:58:53.000000 neuro-extras-24.2.0/neuro_extras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-13 13:59:09.000000 neuro-extras-24.2.0/neuro_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-13 13:59:09.000000 neuro-extras-24.2.0/neuro_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-02-13 13:59:09.870845 neuro-extras-24.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 13:59:09.866845 neuro-extras-24.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 13:59:09.870845 neuro-extras-24.2.0/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 13:59:09.870845 neuro-extras-24.2.0/tests/e2e/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/data/cloud_to_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/data/cloud_to_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/data/local_to_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/data/local_to_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/data/platform_to_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/data/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/data/test_data_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/data/test_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/test_init_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/test_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/e2e/test_seldon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 13:59:09.870845 neuro-extras-24.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 13:59:09.870845 neuro-extras-24.2.0/tests/unit/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/unit/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/unit/image/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/unit/image/test_remote_image_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/unit/test_auth_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-13 13:58:42.000000 neuro-extras-24.2.0/tests/unit/test_select_job_preset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:33.516321 neuro-extras-24.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-24 15:34:33.516321 neuro-extras-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:33.512321 neuro-extras-24.5.0/neuro_extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:33.512321 neuro-extras-24.5.0/neuro_extras/assets/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1214 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/assets/merge_docker_auths.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:33.512321 neuro-extras-24.5.0/neuro_extras/assets/seldon.package/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/assets/seldon.package/seldon.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/assets/seldon.package/seldon_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:33.512321 neuro-extras-24.5.0/neuro_extras/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/data/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/data/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12535 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/data/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/data/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/data/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/data/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/data/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/data/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/data/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/image_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/seldon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/neuro_extras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:33.512321 neuro-extras-24.5.0/neuro_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-24 15:34:33.000000 neuro-extras-24.5.0/neuro_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-24 15:34:33.000000 neuro-extras-24.5.0/neuro_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:34:33.000000 neuro-extras-24.5.0/neuro_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-24 15:34:33.000000 neuro-extras-24.5.0/neuro_extras.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:34:16.000000 neuro-extras-24.5.0/neuro_extras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 15:34:33.000000 neuro-extras-24.5.0/neuro_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 15:34:33.000000 neuro-extras-24.5.0/neuro_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-24 15:34:33.516321 neuro-extras-24.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:33.512321 neuro-extras-24.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:33.516321 neuro-extras-24.5.0/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:33.516321 neuro-extras-24.5.0/tests/e2e/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/data/cloud_to_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/data/cloud_to_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/data/local_to_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/data/local_to_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/data/platform_to_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/data/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/data/test_data_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/data/test_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/test_init_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/test_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/e2e/test_seldon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:33.516321 neuro-extras-24.5.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:33.516321 neuro-extras-24.5.0/tests/unit/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/unit/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/unit/image/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/unit/image/test_remote_image_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/unit/test_auth_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-24 15:34:08.000000 neuro-extras-24.5.0/tests/unit/test_select_job_preset.py
```

### Comparing `neuro-extras-24.2.0/LICENSE` & `neuro-extras-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/README.md` & `neuro-extras-24.5.0/README.md`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/__init__.py` & `neuro-extras-24.5.0/neuro_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/assets/merge_docker_auths.sh` & `neuro-extras-24.5.0/neuro_extras/assets/merge_docker_auths.sh`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/assets/seldon.package/seldon.Dockerfile` & `neuro-extras-24.5.0/neuro_extras/assets/seldon.package/seldon.Dockerfile`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/assets/seldon.package/seldon_model.py` & `neuro-extras-24.5.0/neuro_extras/assets/seldon.package/seldon_model.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/cli.py` & `neuro-extras-24.5.0/neuro_extras/cli.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/common.py` & `neuro-extras-24.5.0/neuro_extras/common.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/config.py` & `neuro-extras-24.5.0/neuro_extras/config.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/data/__init__.py` & `neuro-extras-24.5.0/neuro_extras/data/__init__.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/data/archive.py` & `neuro-extras-24.5.0/neuro_extras/data/archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for archive management operations (compression and extraction)"""
+
 import abc
 import logging
 
 from ..utils import CLIRunner
 from .common import ArchiveType, Resource, ensure_folder_exists
```

### Comparing `neuro-extras-24.2.0/neuro_extras/data/azure.py` & `neuro-extras-24.5.0/neuro_extras/data/azure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for copying files from/to Azure"""
+
 import logging
 import os
 from urllib import parse
 
 from yarl import URL
 
 from ..utils import CLIRunner
```

### Comparing `neuro-extras-24.2.0/neuro_extras/data/common.py` & `neuro-extras-24.5.0/neuro_extras/data/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for common functionality and key abstractions related to data copy"""
+
 import abc
 import logging
 import os
 import re
 from dataclasses import dataclass
 from enum import Flag, auto
 from functools import cached_property
```

### Comparing `neuro-extras-24.2.0/neuro_extras/data/fs.py` & `neuro-extras-24.5.0/neuro_extras/data/fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for copying files on local filesystem"""
+
 import os
 from pathlib import Path
 
 from ..utils import CLIRunner
 from .common import Copier, DataUrlType, Resource
```

### Comparing `neuro-extras-24.2.0/neuro_extras/data/gcs.py` & `neuro-extras-24.5.0/neuro_extras/data/gcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for copying files from/to Google Cloud Storage"""
+
 from ..utils import CLIRunner
 from .common import Copier, DataUrlType, Resource
 
 
 class GCSCopier(Copier, CLIRunner):
     """Copier, that is capable of copying to/from Google Cloud Storage"""
```

### Comparing `neuro-extras-24.2.0/neuro_extras/data/local.py` & `neuro-extras-24.5.0/neuro_extras/data/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module for handling copy operations, that can be run locally
 
 Contains:
 - LocalToLocalCopier
 - LocalToCloudCopier
 - CloudToLocalCopier
 """
+
 import logging
 import os
 import tempfile
 from pathlib import Path
 from typing import Type
 
 from neuro_extras.data.fs import LocalFSCopier
```

### Comparing `neuro-extras-24.2.0/neuro_extras/data/operations.py` & `neuro-extras-24.5.0/neuro_extras/data/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module for data operations
 
 Provides:
 - CopyOperation
 """
+
 import logging
 from pathlib import Path
 from typing import List, Optional, Tuple
 
 from neuro_sdk import Client
 
 from ..utils import provide_temp_dir
```

### Comparing `neuro-extras-24.2.0/neuro_extras/data/remote.py` & `neuro-extras-24.5.0/neuro_extras/data/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for copying files by running neu.ro jobs"""
+
 import logging
 from dataclasses import dataclass, replace
 from typing import List, Mapping, Optional, Tuple
 
 from neuro_cli.utils import resolve_disk
 from neuro_sdk import Client, DiskVolume, RemoteImage, SecretFile, Volume
 from yarl import URL
```

### Comparing `neuro-extras-24.2.0/neuro_extras/data/s3.py` & `neuro-extras-24.5.0/neuro_extras/data/s3.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/data/web.py` & `neuro-extras-24.5.0/neuro_extras/data/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for copying files from HTTP(S) sources"""
+
 from ..utils import CLIRunner
 from .common import Copier, DataUrlType, Resource
 
 
 class WebCopier(Copier, CLIRunner):
     """Copier for downloading data from HTTP(S) sources"""
```

### Comparing `neuro-extras-24.2.0/neuro_extras/image.py` & `neuro-extras-24.5.0/neuro_extras/image.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/image_builder.py` & `neuro-extras-24.5.0/neuro_extras/image_builder.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/k8s.py` & `neuro-extras-24.5.0/neuro_extras/k8s.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/main.py` & `neuro-extras-24.5.0/neuro_extras/main.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/seldon.py` & `neuro-extras-24.5.0/neuro_extras/seldon.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/neuro_extras/utils.py` & `neuro-extras-24.5.0/neuro_extras/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -217,15 +217,14 @@
     for cluster_preset_name, cluster_preset_info in client.presets.items():
         # Don't even try to use GPU machines for image builds
         # Also ignore scheduled presets (they don't work with schedule-timeout)
         # see https://github.com/neuro-inc/neuro-extras/issues/488
         if (
             cluster_preset_info.cpu >= min_cpu
             and cluster_preset_info.memory_mb >= min_mem
-            and cluster_preset_info.gpu is None
             and not cluster_preset_info.scheduler_enabled
         ):
             good_presets.append((cluster_preset_name, cluster_preset_info))
             good_presets_names.append(cluster_preset_name)
     # Sort presets by cost - memory - cpu
     good_presets.sort(key=lambda p: (p[1].credits_per_hour, p[1].memory_mb, p[1].cpu))
 
@@ -253,23 +252,14 @@
             if len(good_presets) > 0:
                 # We have a better preset
                 logger.warning(
                     f"The selected resource preset {preset} does not "
                     f"satisfy recommended minimum hardware requirements. "
                     f"Consider using '{good_presets[0][0]}'"
                 )
-            elif client.presets[preset].gpu is None:
-                # The message is only displayed if user selected a bad non-GPU preset
-                logger.warning(
-                    f"Selected resource preset {preset} does not satisfy "
-                    f"minimal hardware requirements. "
-                    "The job might take long time to accomplish. "
-                    "Consider contacting your cluster manager or admin "
-                    "to adjust the cluster configuration"
-                )
             return preset
 
 
 def get_default_preset(neuro_client: Client) -> str:
     """Get default preset name via Neu.ro client"""
     return next(iter(neuro_client.presets.keys()))
```

### Comparing `neuro-extras-24.2.0/neuro_extras.egg-info/SOURCES.txt` & `neuro-extras-24.5.0/neuro_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/pyproject.toml` & `neuro-extras-24.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/setup.cfg` & `neuro-extras-24.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [flake8]
 max-line-length = 88
 exclude = 
 	.git
 	venv
 	__pycache__
-ignore = F541,W503,E203
+ignore = F541,W503,E203,E704
 
 [isort]
 line_length = 88
 include_trailing_comma = True
 multi_line_output = 3
 force_grid_wrap = 0
 combine_as_imports = True
```

### Comparing `neuro-extras-24.2.0/setup.py` & `neuro-extras-24.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 setup(
     name="neuro-extras",
     version=version,
     python_requires=">=3.8.0",
     url="https://github.com/neuro-inc/neuro-extras",
     packages=find_packages(),
     install_requires=[
-        "neuro-cli>=21.11.4",
+        "neuro-cli>=24.5.0",
         "click>=8.0",
         "toml>=0.10.0",
         "pyyaml>=3.0",
     ],
     entry_points={
         "console_scripts": ["neuro-extras=neuro_extras:main"],
         "neuro_api": ["neuro-extras=neuro_extras:setup_plugin"],
```

### Comparing `neuro-extras-24.2.0/tests/e2e/conftest.py` & `neuro-extras-24.5.0/tests/e2e/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,15 @@
 SRC_CLUSTER_ENV_VAR = "NEURO_CLUSTER"
 DST_CLUSTER_ENV_VAR = "NEURO_CLUSTER_SECONDARY"
 
 
 class CLIRunner(Protocol):
     def __call__(
         self, args: List[str], enable_retry: bool = False
-    ) -> "CompletedProcess[str]":
-        ...
+    ) -> "CompletedProcess[str]": ...
 
 
 def get_tested_archive_types() -> List[str]:
     """Get tested archive types
 
     If PYTEST_DATA_COPY_ARCHIVE_TYPES is set,
     returns its value, split on `,`.
```

### Comparing `neuro-extras-24.2.0/tests/e2e/data/cloud_to_local.py` & `neuro-extras-24.5.0/tests/e2e/data/cloud_to_local.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/e2e/data/cloud_to_platform.py` & `neuro-extras-24.5.0/tests/e2e/data/cloud_to_platform.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/e2e/data/local_to_cloud.py` & `neuro-extras-24.5.0/tests/e2e/data/local_to_cloud.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/e2e/data/local_to_local.py` & `neuro-extras-24.5.0/tests/e2e/data/local_to_local.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/e2e/data/platform_to_cloud.py` & `neuro-extras-24.5.0/tests/e2e/data/platform_to_cloud.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/e2e/data/resources.py` & `neuro-extras-24.5.0/tests/e2e/data/resources.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/e2e/data/test_data_cp.py` & `neuro-extras-24.5.0/tests/e2e/data/test_data_cp.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/e2e/data/test_data_transfer.py` & `neuro-extras-24.5.0/tests/e2e/data/test_data_transfer.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/e2e/test_image.py` & `neuro-extras-24.5.0/tests/e2e/test_image.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/e2e/test_k8s.py` & `neuro-extras-24.5.0/tests/e2e/test_k8s.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/e2e/test_seldon.py` & `neuro-extras-24.5.0/tests/e2e/test_seldon.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/unit/image/conftest.py` & `neuro-extras-24.5.0/tests/unit/image/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
         "cpu-small": neuro_sdk.Preset(
             credits_per_hour=Decimal(1), cpu=1, memory=1 * 1024 * 1024
         ),
         "custom-preset": neuro_sdk.Preset(
             credits_per_hour=Decimal(1),
             cpu=5,
             memory=3 * 1024 * 1024,
-            gpu=1,
-            gpu_model="mygpu",
+            nvidia_gpu=1,
         ),
     }
 
 
 def _get_mock_clusters() -> t.Dict[str, neuro_sdk.Cluster]:
     return {
         "mycluster": neuro_sdk.Cluster(
@@ -35,14 +34,15 @@
             registry_url=URL("https://registry.mycluster.noexists"),
             storage_url=URL("https://mycluster.noexists/api/v1/storage"),
             users_url=URL("https://noexists/api/v1/users"),
             monitoring_url=URL("https://mycluster.noexists/api/v1/jobs"),
             secrets_url=URL("https://mycluster.noexists/api/v1/secrets"),
             disks_url=URL("https://mycluster.noexists/api/v1/disks"),
             buckets_url=URL("https://mycluster.noexists/api/v1/buckets"),
+            resource_pools={},
             presets=_get_mock_presets(),
             orgs=[],
         ),
     }
 
 
 def _get_mock_projects() -> t.Dict[neuro_sdk.Project.Key, neuro_sdk.Project]:
```

### Comparing `neuro-extras-24.2.0/tests/unit/image/test_remote_image_builder.py` & `neuro-extras-24.5.0/tests/unit/image/test_remote_image_builder.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/unit/test_auth_merge.py` & `neuro-extras-24.5.0/tests/unit/test_auth_merge.py`

 * *Files identical despite different names*

### Comparing `neuro-extras-24.2.0/tests/unit/test_select_job_preset.py` & `neuro-extras-24.5.0/tests/unit/test_select_job_preset.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,14 @@
     )
     assert selected_preset == preset
 
 
 def test_when_nothing_fits_first_preset_is_used(mock_client: MockNeuroClient) -> None:
     presets = {
         "bad": Preset(cpu=1, memory=9999, credits_per_hour=Decimal("5")),
-        "gpu": Preset(cpu=4, memory=9999, credits_per_hour=Decimal("15"), gpu=1),
+        "gpu": Preset(cpu=4, memory=9999, credits_per_hour=Decimal("15"), nvidia_gpu=1),
     }
     selected_preset = select_job_preset(
         preset=None, client=mock_client, min_mem=4096, min_cpu=2
     )
     mock_client.presets.update(presets)
     assert selected_preset is None
```

