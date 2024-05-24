# Comparing `tmp/pilot-platform-common-0.7.4.tar.gz` & `tmp/pilot-platform-common-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot-platform-common-0.7.4.tar", last modified: Thu Apr 25 20:32:32 2024, max compression
+gzip compressed data, was "pilot-platform-common-1.0.0.tar", last modified: Fri May 24 16:18:06 2024, max compression
```

## Comparing `pilot-platform-common-0.7.4.tar` & `pilot-platform-common-1.0.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.199103 pilot-platform-common-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-25 20:32:32.199103 pilot-platform-common-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/geid/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/geid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/geid/geid_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/jwt_handler/
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/jwt_handler/JWTHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/jwt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/jwt_handler/jwt_handler_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/jwt_handler/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/models/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/models/config_center_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/models/service_id_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.191103 pilot-platform-common-0.7.4/common/object_storage_adaptor/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/object_storage_adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/object_storage_adaptor/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/object_storage_adaptor/boto3_admin_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17073 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/object_storage_adaptor/boto3_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/object_storage_adaptor/minio_policy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/common/permissions/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/permissions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/permissions/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/permissions/permissions_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/permissions/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/common/project/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/project/project_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/project/project_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/common/services/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/services/auth_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/common/vault/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/vault/vault_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/common/vault/vault_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-25 20:32:32.000000 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-25 20:32:32.000000 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:32:32.000000 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-25 20:32:32.000000 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 20:32:32.000000 pilot-platform-common-0.7.4/pilot_platform_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 20:32:32.199103 pilot-platform-common-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.195103 pilot-platform-common-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.199103 pilot-platform-common-0.7.4/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/fixtures/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/fixtures/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:32:32.199103 pilot-platform-common-0.7.4/tests/permissions/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/permissions/test_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    19843 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/permissions/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/permissions/test_permissions_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_geid_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_jwt_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_project_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-25 20:31:35.000000 pilot-platform-common-0.7.4/tests/test_vault_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.714060 pilot-platform-common-1.0.0/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.714060 pilot-platform-common-1.0.0/common/geid/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/geid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/geid/geid_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.714060 pilot-platform-common-1.0.0/common/jwt_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/jwt_handler/JWTHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/jwt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/jwt_handler/jwt_handler_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/jwt_handler/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/models/config_center_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/models/service_id_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/object_storage_adaptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/object_storage_adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/object_storage_adaptor/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/object_storage_adaptor/boto3_admin_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17073 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/object_storage_adaptor/boto3_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/object_storage_adaptor/minio_policy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/permissions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/permissions/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/permissions/permissions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/permissions/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/project/project_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/project/project_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/services/auth_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/common/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/vault/vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/common/vault/vault_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.718060 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-24 16:18:06.000000 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-24 16:18:06.000000 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:18:06.000000 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-24 16:18:06.000000 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 16:18:06.000000 pilot-platform-common-1.0.0/pilot_platform_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/fixtures/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/fixtures/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:18:06.722060 pilot-platform-common-1.0.0/tests/permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/permissions/test_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19843 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/permissions/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/permissions/test_permissions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_geid_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_jwt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_project_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-24 16:17:04.000000 pilot-platform-common-1.0.0/tests/test_vault_client.py
```

### Comparing `pilot-platform-common-0.7.4/PKG-INFO` & `pilot-platform-common-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.7.4
+Version: 1.0.0
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Systems
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.7.4/README.md` & `pilot-platform-common-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/__init__.py` & `pilot-platform-common-1.0.0/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/geid/geid_client.py` & `pilot-platform-common-1.0.0/common/geid/geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/jwt_handler/JWTHandler.py` & `pilot-platform-common-1.0.0/common/jwt_handler/JWTHandler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/jwt_handler/models.py` & `pilot-platform-common-1.0.0/common/jwt_handler/models.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/logging/formatter.py` & `pilot-platform-common-1.0.0/common/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/logging/logging.py` & `pilot-platform-common-1.0.0/common/logging/logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/models/config_center_policy.py` & `pilot-platform-common-1.0.0/common/models/config_center_policy.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/object_storage_adaptor/base_client.py` & `pilot-platform-common-1.0.0/common/object_storage_adaptor/base_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/object_storage_adaptor/boto3_admin_client.py` & `pilot-platform-common-1.0.0/common/object_storage_adaptor/boto3_admin_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/object_storage_adaptor/boto3_client.py` & `pilot-platform-common-1.0.0/common/object_storage_adaptor/boto3_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/object_storage_adaptor/minio_policy_client.py` & `pilot-platform-common-1.0.0/common/object_storage_adaptor/minio_policy_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/permissions/exceptions.py` & `pilot-platform-common-1.0.0/common/permissions/exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/permissions/permissions.py` & `pilot-platform-common-1.0.0/common/permissions/permissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,8 +169,8 @@
     permission_request = permission_manager.build_request(permissions, role)
 
     auth_client = AuthClient(auth_url)
     assertions = await auth_client.get_assertions(project_code, permission_request)
 
     mapped_assertions = permission_manager.map_assertions(permission_request, assertions)
 
-    return mapped_assertions.dict()['assertion']
+    return mapped_assertions.model_dump()['assertion']
```

### Comparing `pilot-platform-common-0.7.4/common/permissions/permissions_manager.py` & `pilot-platform-common-1.0.0/common/permissions/permissions_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def _assertion_mapper(
         self, permission_request: PermissionsSchema, assertions: dict[str, Union[bool, list]]
     ) -> PermissionsMappedAssertionSchema:
         """Map assertions against single requested permission."""
 
         permission = True
         if not assertions['has_permission']:
-            if permission_request.dict() in assertions['denied']:
+            if permission_request.model_dump() in assertions['denied']:
                 permission = False
         mapped = {
             f'{permission_request.zone}_{permission_request.resource}_' f'{permission_request.operation}': permission
         }
 
         return PermissionsMappedAssertionSchema(assertion=mapped)
 
@@ -76,15 +76,15 @@
         """Map rbac assertions from auth service against requested permissions."""
 
         mapped_assertions = {}
         try:
             for mapped in (
                 self._assertion_mapper(permission, assertions) for permission in permissions_requested.permissions
             ):
-                mapped_assertions.update(mapped.dict()['assertion'])
+                mapped_assertions.update(mapped.model_dump()['assertion'])
 
             return PermissionsMappedAssertionSchema(assertion=mapped_assertions)
 
         except ValidationError:
             logger.exception('Failed to parse and validate mapped asserted permissions.')
             raise PermissionValidationError('Permission mapped assertion validation failed')
```

### Comparing `pilot-platform-common-0.7.4/common/permissions/schemas.py` & `pilot-platform-common-1.0.0/common/permissions/schemas.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/project/project_client.py` & `pilot-platform-common-1.0.0/common/project/project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/project/project_exceptions.py` & `pilot-platform-common-1.0.0/common/project/project_exceptions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/common/services/auth_client.py` & `pilot-platform-common-1.0.0/common/services/auth_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     async def get_assertions(
         self, project_code: str, permissions: PermissionsRequestSchema
     ) -> dict[str, Union[bool, list]]:
         """Retrieve bulk rbac permission assertions."""
 
         try:
-            payload = permissions.dict()['permissions']
+            payload = permissions.model_dump()['permissions']
             async with AsyncClient(timeout=15) as client:
                 response = await client.post(
                     self.service_url + 'authorize', json=payload, params={'project_code': project_code}
                 )
                 response.raise_for_status()
 
             return response.json()
```

### Comparing `pilot-platform-common-0.7.4/common/vault/vault_client.py` & `pilot-platform-common-1.0.0/common/vault/vault_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/pilot_platform_common.egg-info/PKG-INFO` & `pilot-platform-common-1.0.0/pilot_platform_common.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-common
-Version: 0.7.4
+Version: 1.0.0
 Summary: Generates entity ID and connects with Vault (secret engine) to retrieve credentials
 Author: Indoc Systems
 Author-email: etaylor@indocresearch.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `pilot-platform-common-0.7.4/pilot_platform_common.egg-info/SOURCES.txt` & `pilot-platform-common-1.0.0/pilot_platform_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/pyproject.toml` & `pilot-platform-common-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "common"
-version = "0.7.4"
+version = "1.0.0"
 description = ""
 authors = ["Indoc Systems"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = ">=0.19.1"
 python-json-logger = ">= 0.1.11, <= 2.02"
 aioboto3 = "^9.6.0"
 xmltodict = "^0.13.0"
 minio = "^7.1.8"
 httpx = ">=0.23.0,<0.27.0"
 pyjwt = "2.6.0"
 redis = "^4.5"
-starlette = ">=0.25.0,<0.36.0"
+starlette = ">=0.37.2,<0.38.0"
 cryptography = "39.0.0"
-pydantic = "^1.10.8"
+pydantic = "^2.7.1"
+requests = ">=2.26.0,<2.32.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.1"
 pytest-asyncio = "0.20.3"
 pytest-cov = "4.0.0"
 pytest-httpx = "0.26.0"
 pytest-mock = "3.10.0"
```

### Comparing `pilot-platform-common-0.7.4/setup.py` & `pilot-platform-common-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setuptools.setup(
     name='pilot-platform-common',
-    version='0.7.4',
+    version='1.0.0',
     author='Indoc Systems',
     author_email='etaylor@indocresearch.org',
     description='Generates entity ID and connects with Vault (secret engine) to retrieve credentials',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     classifiers=[
@@ -28,15 +28,17 @@
         'httpx>=0.23.0,<0.27.0',
         'redis>=4.5.0,<5.0.0',
         'aioboto3==9.6.0',
         'xmltodict==0.13.0',
         'minio==7.1.8',
         'python-json-logger==2.0.2',
         'pyjwt==2.6.0',
-        'starlette>=0.25.0,<0.36.0',
+        'starlette>=0.37.2,<0.38.0',
+        'requests>=2.26.0,<2.32.0',
         'cryptography==39.0.0',
+        'pydantic>=2.7.1,<3.0.0',
     ],
     include_package_data=True,
     package_data={
         '': ['*.crt'],
     },
 )
```

### Comparing `pilot-platform-common-0.7.4/tests/conftest.py` & `pilot-platform-common-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/tests/fixtures/metadata.py` & `pilot-platform-common-1.0.0/tests/fixtures/metadata.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/tests/permissions/test_auth_client.py` & `pilot-platform-common-1.0.0/tests/permissions/test_auth_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/tests/permissions/test_permissions.py` & `pilot-platform-common-1.0.0/tests/permissions/test_permissions.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/tests/permissions/test_permissions_manager.py` & `pilot-platform-common-1.0.0/tests/permissions/test_permissions_manager.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/tests/test_formatter.py` & `pilot-platform-common-1.0.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/tests/test_geid_client.py` & `pilot-platform-common-1.0.0/tests/test_geid_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/tests/test_jwt_handler.py` & `pilot-platform-common-1.0.0/tests/test_jwt_handler.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/tests/test_logging.py` & `pilot-platform-common-1.0.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/tests/test_project_client.py` & `pilot-platform-common-1.0.0/tests/test_project_client.py`

 * *Files identical despite different names*

### Comparing `pilot-platform-common-0.7.4/tests/test_vault_client.py` & `pilot-platform-common-1.0.0/tests/test_vault_client.py`

 * *Files identical despite different names*

