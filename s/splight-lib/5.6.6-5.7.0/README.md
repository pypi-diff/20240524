# Comparing `tmp/splight_lib-5.6.6.tar.gz` & `tmp/splight_lib-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight_lib-5.6.6.tar", max compression
+gzip compressed data, was "splight_lib-5.7.0.tar", max compression
```

## Comparing `splight_lib-5.6.6.tar` & `splight_lib-5.7.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0        0 2024-05-17 12:39:58.628778 splight_lib-5.6.6/LICENSE.txt
--rw-r--r--   0        0        0     1108 2024-05-17 12:39:58.628778 splight_lib-5.6.6/README.md
--rw-r--r--   0        0        0     1532 2024-05-17 12:39:58.628778 splight_lib-5.6.6/pyproject.toml
--rw-r--r--   0        0        0      114 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/__init__.py
--rw-r--r--   0        0        0        0 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/abstract/__init__.py
--rw-r--r--   0        0        0     3358 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/abstract/client.py
--rw-r--r--   0        0        0      160 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/auth/__init__.py
--rw-r--r--   0        0        0      404 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/auth/exceptions.py
--rw-r--r--   0        0        0     2944 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/auth/mac_auth.py
--rw-r--r--   0        0        0      224 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/auth/token.py
--rw-r--r--   0        0        0        0 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/__init__.py
--rw-r--r--   0        0        0      358 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/database/__init__.py
--rw-r--r--   0        0        0      785 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/database/abstract.py
--rw-r--r--   0        0        0      582 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/database/builder.py
--rw-r--r--   0        0        0     1277 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/database/classmap.py
--rw-r--r--   0        0        0     6192 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/database/local_client.py
--rw-r--r--   0        0        0    12163 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/database/remote_client.py
--rw-r--r--   0        0        0      474 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/datalake/__init__.py
--rw-r--r--   0        0        0     1878 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/datalake/abstract.py
--rw-r--r--   0        0        0     1649 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/datalake/buffer.py
--rw-r--r--   0        0        0      944 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/datalake/builder.py
--rw-r--r--   0        0        0      210 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/datalake/exceptions.py
--rw-r--r--   0        0        0     3728 2024-05-17 12:39:58.628778 splight_lib-5.6.6/splight_lib/client/datalake/local_client.py
--rw-r--r--   0        0        0    13636 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0        0        0     1505 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/client/datalake/schemas.py
--rw-r--r--   0        0        0      948 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/client/exceptions.py
--rw-r--r--   0        0        0      981 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/client/file_handler.py
--rw-r--r--   0        0        0      595 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/client/filter.py
--rw-r--r--   0        0        0       96 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/client/hub/__init__.py
--rw-r--r--   0        0        0      803 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/client/hub/abstract.py
--rw-r--r--   0        0        0     4660 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/client/hub/client.py
--rw-r--r--   0        0        0     5218 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/client/tests/test_database.py
--rw-r--r--   0        0        0     1623 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/client/tests/test_datalake.py
--rw-r--r--   0        0        0      105 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/component/__init__.py
--rw-r--r--   0        0        0     6963 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/component/abstract.py
--rw-r--r--   0        0        0      480 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/component/exceptions.py
--rw-r--r--   0        0        0     7844 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/component/spec.py
--rw-r--r--   0        0        0       49 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/component/tests/test_abstract.py
--rw-r--r--   0        0        0     4115 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/component/tests/test_spec.py
--rw-r--r--   0        0        0      210 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/constants.py
--rw-r--r--   0        0        0     2002 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/encryption.py
--rw-r--r--   0        0        0      303 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/execution/__init__.py
--rw-r--r--   0        0        0     3988 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/execution/engine.py
--rw-r--r--   0        0        0      282 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/execution/exceptions.py
--rw-r--r--   0        0        0     2990 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/execution/scheduling.py
--rw-r--r--   0        0        0     1932 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/execution/task.py
--rw-r--r--   0        0        0     1034 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/execution/tests/test_execution.py
--rw-r--r--   0        0        0     1048 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/execution/tests/test_scheduling.py
--rw-r--r--   0        0        0     1302 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/execution/trigger.py
--rw-r--r--   0        0        0      192 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/logging/__init__.py
--rw-r--r--   0        0        0     1516 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/logging/_internal.py
--rw-r--r--   0        0        0     1426 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/logging/component.py
--rw-r--r--   0        0        0      130 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/logging/constants.py
--rw-r--r--   0        0        0     4881 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/logging/logging.py
--rw-r--r--   0        0        0     4316 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/logging/tests/test_logging.py
--rw-r--r--   0        0        0     1271 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/__init__.py
--rw-r--r--   0        0        0     7791 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/alert.py
--rw-r--r--   0        0        0     1600 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/asset.py
--rw-r--r--   0        0        0      452 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/attribute.py
--rw-r--r--   0        0        0     6311 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/base.py
--rw-r--r--   0        0        0    18782 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/component.py
--rw-r--r--   0        0        0     2857 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/dashboard.py
--rw-r--r--   0        0        0     1024 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/data_address.py
--rw-r--r--   0        0        0      634 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/exceptions.py
--rw-r--r--   0        0        0     1869 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/file.py
--rw-r--r--   0        0        0     6710 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/function.py
--rw-r--r--   0        0        0      790 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/generic.py
--rw-r--r--   0        0        0     7153 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/hub.py
--rw-r--r--   0        0        0     1334 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/hub_solution.py
--rw-r--r--   0        0        0      606 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/metadata.py
--rw-r--r--   0        0        0     2162 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/native.py
--rw-r--r--   0        0        0     2398 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/pipeline.py
--rw-r--r--   0        0        0      487 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/secret.py
--rw-r--r--   0        0        0    11054 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/tests/models.json
--rw-r--r--   0        0        0     2376 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/tests/test_component_object_instance.py
--rw-r--r--   0        0        0     3599 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/tests/test_database_model.py
--rw-r--r--   0        0        0     1389 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/tests/test_metadata.py
--rw-r--r--   0        0        0      823 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/models/tests/test_models.py
--rw-r--r--   0        0        0      212 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/restclient/__init__.py
--rw-r--r--   0        0        0    16872 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/restclient/client.py
--rw-r--r--   0        0        0      964 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/restclient/exceptions.py
--rw-r--r--   0        0        0     1108 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/restclient/tests/test_restclient.py
--rw-r--r--   0        0        0     2386 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/restclient/types.py
--rw-r--r--   0        0        0     3586 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/settings.py
--rw-r--r--   0        0        0      427 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/stringcase.py
--rw-r--r--   0        0        0     2834 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/testing/__init__.py
--rw-r--r--   0        0        0      251 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/tests/FakeProc.py
--rw-r--r--   0        0        0     5885 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/tests/asset_geometries.json
--rw-r--r--   0        0        0     5400 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/tests/test_api_contracts.py
--rw-r--r--   0        0        0       41 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/tests/test_encryption.py
--rw-r--r--   0        0        0        0 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/utils/__init__.py
--rw-r--r--   0        0        0     2297 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/utils/custom_model.py
--rw-r--r--   0        0        0      626 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/utils/hub.py
--rw-r--r--   0        0        0       78 2024-05-17 12:39:58.632778 splight_lib-5.6.6/splight_lib/version.py
--rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 splight_lib-5.6.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-24 18:13:34.773238 splight_lib-5.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     1108 2024-05-24 18:13:34.773238 splight_lib-5.7.0/README.md
+-rw-r--r--   0        0        0     1532 2024-05-24 18:13:34.777238 splight_lib-5.7.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/abstract/__init__.py
+-rw-r--r--   0        0        0     3358 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/abstract/client.py
+-rw-r--r--   0        0        0      160 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/auth/__init__.py
+-rw-r--r--   0        0        0      404 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/auth/exceptions.py
+-rw-r--r--   0        0        0     2944 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/auth/mac_auth.py
+-rw-r--r--   0        0        0      224 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/auth/token.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/__init__.py
+-rw-r--r--   0        0        0      358 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/database/__init__.py
+-rw-r--r--   0        0        0      785 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/database/abstract.py
+-rw-r--r--   0        0        0      582 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/database/builder.py
+-rw-r--r--   0        0        0     1383 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/database/classmap.py
+-rw-r--r--   0        0        0     6192 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/database/local_client.py
+-rw-r--r--   0        0        0    12793 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/database/remote_client.py
+-rw-r--r--   0        0        0      474 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0        0        0     1878 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0        0        0     1649 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/datalake/buffer.py
+-rw-r--r--   0        0        0      944 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/datalake/builder.py
+-rw-r--r--   0        0        0      210 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/datalake/exceptions.py
+-rw-r--r--   0        0        0     3728 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0        0        0    13636 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0        0        0     1505 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/datalake/schemas.py
+-rw-r--r--   0        0        0     1162 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/exceptions.py
+-rw-r--r--   0        0        0      981 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/file_handler.py
+-rw-r--r--   0        0        0      595 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/filter.py
+-rw-r--r--   0        0        0       96 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/hub/__init__.py
+-rw-r--r--   0        0        0      803 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/hub/abstract.py
+-rw-r--r--   0        0        0     4660 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/hub/client.py
+-rw-r--r--   0        0        0     5361 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/tests/test_database.py
+-rw-r--r--   0        0        0     1727 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/client/tests/test_datalake.py
+-rw-r--r--   0        0        0      105 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/component/__init__.py
+-rw-r--r--   0        0        0     6963 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/component/abstract.py
+-rw-r--r--   0        0        0      480 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/component/exceptions.py
+-rw-r--r--   0        0        0     7844 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/component/spec.py
+-rw-r--r--   0        0        0       49 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/component/tests/test_abstract.py
+-rw-r--r--   0        0        0     4115 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/component/tests/test_spec.py
+-rw-r--r--   0        0        0      210 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/constants.py
+-rw-r--r--   0        0        0     2002 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/encryption.py
+-rw-r--r--   0        0        0      303 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/execution/__init__.py
+-rw-r--r--   0        0        0     3988 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/execution/engine.py
+-rw-r--r--   0        0        0      282 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/execution/exceptions.py
+-rw-r--r--   0        0        0     2990 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/execution/scheduling.py
+-rw-r--r--   0        0        0     1932 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/execution/task.py
+-rw-r--r--   0        0        0     1034 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/execution/tests/test_execution.py
+-rw-r--r--   0        0        0     1048 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/execution/tests/test_scheduling.py
+-rw-r--r--   0        0        0     1302 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/execution/trigger.py
+-rw-r--r--   0        0        0      192 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/logging/__init__.py
+-rw-r--r--   0        0        0     1516 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/logging/_internal.py
+-rw-r--r--   0        0        0     1426 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/logging/component.py
+-rw-r--r--   0        0        0      130 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/logging/constants.py
+-rw-r--r--   0        0        0     4881 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/logging/logging.py
+-rw-r--r--   0        0        0     4316 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/logging/tests/test_logging.py
+-rw-r--r--   0        0        0     1297 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/__init__.py
+-rw-r--r--   0        0        0     7791 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/alert.py
+-rw-r--r--   0        0        0     2267 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/asset.py
+-rw-r--r--   0        0        0      452 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/attribute.py
+-rw-r--r--   0        0        0     6344 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/base.py
+-rw-r--r--   0        0        0    18782 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/component.py
+-rw-r--r--   0        0        0     2857 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/dashboard.py
+-rw-r--r--   0        0        0     1024 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/data_address.py
+-rw-r--r--   0        0        0      680 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/exceptions.py
+-rw-r--r--   0        0        0     1869 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/file.py
+-rw-r--r--   0        0        0     6710 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/function.py
+-rw-r--r--   0        0        0      790 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/generic.py
+-rw-r--r--   0        0        0     7153 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/hub.py
+-rw-r--r--   0        0        0     1334 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/hub_solution.py
+-rw-r--r--   0        0        0      606 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/metadata.py
+-rw-r--r--   0        0        0     2162 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/native.py
+-rw-r--r--   0        0        0     2398 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/pipeline.py
+-rw-r--r--   0        0        0      487 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/secret.py
+-rw-r--r--   0        0        0    11054 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/tests/models.json
+-rw-r--r--   0        0        0     2376 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/tests/test_component_object_instance.py
+-rw-r--r--   0        0        0     4354 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/tests/test_database_model.py
+-rw-r--r--   0        0        0     1389 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/tests/test_metadata.py
+-rw-r--r--   0        0        0      823 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/models/tests/test_models.py
+-rw-r--r--   0        0        0      212 2024-05-24 18:13:34.777238 splight_lib-5.7.0/splight_lib/restclient/__init__.py
+-rw-r--r--   0        0        0    16872 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/restclient/client.py
+-rw-r--r--   0        0        0      964 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/restclient/exceptions.py
+-rw-r--r--   0        0        0     1108 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/restclient/tests/test_restclient.py
+-rw-r--r--   0        0        0     2386 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/restclient/types.py
+-rw-r--r--   0        0        0     3586 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/settings.py
+-rw-r--r--   0        0        0      427 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/stringcase.py
+-rw-r--r--   0        0        0     2834 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/testing/__init__.py
+-rw-r--r--   0        0        0      251 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/tests/FakeProc.py
+-rw-r--r--   0        0        0     5885 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/tests/asset_geometries.json
+-rw-r--r--   0        0        0     5400 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/tests/test_api_contracts.py
+-rw-r--r--   0        0        0       41 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/tests/test_encryption.py
+-rw-r--r--   0        0        0        0 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/utils/__init__.py
+-rw-r--r--   0        0        0     2297 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/utils/custom_model.py
+-rw-r--r--   0        0        0      626 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/utils/hub.py
+-rw-r--r--   0        0        0       78 2024-05-24 18:13:34.781238 splight_lib-5.7.0/splight_lib/version.py
+-rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 splight_lib-5.7.0/PKG-INFO
```

### Comparing `splight_lib-5.6.6/README.md` & `splight_lib-5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/pyproject.toml` & `splight_lib-5.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splight-lib"
-version = "5.6.6"
+version = "5.7.0"
 description = "Splight Library"
 authors = ["Splight Dev <dev@splight-ae.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 concurrent-log-handler = "0.9.21"
```

### Comparing `splight_lib-5.6.6/splight_lib/abstract/client.py` & `splight_lib-5.7.0/splight_lib/abstract/client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/auth/mac_auth.py` & `splight_lib-5.7.0/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/database/abstract.py` & `splight_lib-5.7.0/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/database/builder.py` & `splight_lib-5.7.0/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/database/classmap.py` & `splight_lib-5.7.0/splight_lib/client/database/classmap.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from splight_lib.constants import ENGINE_PREFIX, HUB_PREFIX
 
 MODEL_NAME_MAP = {
     "advancedfilter": f"{ENGINE_PREFIX}/alert/advancedfilters/",
     "alert": f"{ENGINE_PREFIX}/alert/alerts/",
-    "asset": f"{ENGINE_PREFIX}/assets/",
+    "asset": f"{ENGINE_PREFIX}/asset/assets/",
+    "assetkind": f"{ENGINE_PREFIX}/asset/kinds/",
+    # TODO: update to new endpoint for attributes
     "attribute": f"{ENGINE_PREFIX}/attributes/",
     "metadata": f"{ENGINE_PREFIX}/metadata/",
     "chart": f"{ENGINE_PREFIX}/dashboard/charts/",
     "chartitem": f"{ENGINE_PREFIX}/dashboard/chartitems/",
     "component": f"{ENGINE_PREFIX}/component/components/",
     "componentobject": f"{ENGINE_PREFIX}/component/objects/",
     "dashboard": f"{ENGINE_PREFIX}/dashboard/dashboards/",
```

### Comparing `splight_lib-5.6.6/splight_lib/client/database/local_client.py` & `splight_lib-5.7.0/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/database/remote_client.py` & `splight_lib-5.7.0/splight_lib/client/database/remote_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     MODEL_NAME_MAP,
 )
 from splight_lib.client.exceptions import (
     SPLIGHT_REQUEST_EXCEPTIONS,
     InstanceNotFound,
     InvalidModel,
     InvalidModelName,
+    RequestError,
 )
 from splight_lib.constants import ENGINE_PREFIX
 from splight_lib.logging._internal import LogTags, get_splight_logger
 from splight_lib.restclient import SplightRestClient
 
 logger = get_splight_logger()
 
@@ -112,15 +113,16 @@
         ------
         InvalidModelName thrown when the model name is not correct.
         """
         logger.debug("Deleting instance %s.", id, tags=LogTags.DATABASE)
         api_path = self._get_api_path(resource_name)
         url = self._base_url / api_path / f"{id}/"
         response = self._restclient.delete(url)
-        response.raise_for_status()
+        if response.is_error:
+            raise RequestError(response.status_code, response.text)
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
     def _get(
         self,
         resource_name: str,
         first: bool = False,
         **kwargs,
@@ -151,15 +153,16 @@
         model_name = resource_name.lower()
         api_path = CUSTOM_PATHS_MAP.get(model_name)
         if not api_path:
             raise InvalidModelName(model_name)
         api_path = api_path.format_map({"prefix": ENGINE_PREFIX, **instance})
         url = self._base_url / api_path
         response = self._restclient.post(url, json=instance)
-        response.raise_for_status()
+        if response.is_error:
+            raise RequestError(response.status_code, response.text)
         return response.json()
 
     def _retrieve_multiple(
         self, resource_name: str, first: bool = False, **kwargs
     ) -> List[Dict]:
         logger.debug(f"Retrieving objects {resource_name}")
         api_path = self._get_api_path(resource_name)
@@ -176,16 +179,16 @@
     def _retrieve_single(self, resource_name: str, id: str) -> Dict:
         logger.debug(f"Retrieving object {resource_name} with id {id}")
         api_path = self._get_api_path(resource_name)
         url = self._base_url / api_path / f"{id}/"
         response = self._restclient.get(url)
         if response.status_code == codes.NOT_FOUND:
             raise InstanceNotFound(resource_name, id)
-        else:
-            response.raise_for_status()
+        elif response.is_error:
+            raise RequestError(response.status_code, response.text)
         return response.json()
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=1)
     def download(
         self,
         resource_name: str,
         instance: Dict,
@@ -210,15 +213,16 @@
         """
         if resource_name.lower() != "file":
             raise InvalidModel("Only files can be downloaded.")
         api_path = self._get_api_path(resource_name)
         resource_id = instance.get("id")
         url = self._base_url / api_path / f"{resource_id}/download_url/"
         response = self._restclient.get(url)
-        response.raise_for_status()
+        if response.is_error:
+            raise RequestError(response.status_code, response.text)
         download_url = response.json().get("url")
 
         file = NamedTemporaryFile(mode="wb+", suffix=instance["name"])
         # TODO: Check why python wget is raised and error with code 403
         response = requests.get(download_url, stream=True)
         with open(file.name, "wb") as f:
             length = int(response.headers.get("content-length"))
@@ -249,15 +253,16 @@
                 else None
             )
             kwargs["page"] = next_page
 
     def _list(self, url: furl, **kwargs) -> PaginatedResponse:
         params = self._parse_params(**kwargs)
         response = self._restclient.get(url, params=params)
-        response.raise_for_status()
+        if response.is_error:
+            raise RequestError(response.status_code, response.text)
         return response.json()
 
     def _create(
         self,
         resource_name: str,
         instance: Dict,
         files: Optional[Dict[str, str]] = None,
@@ -277,15 +282,16 @@
             # TODO: Fix in API so here we only use data argument
             if files_payload:
                 req_args = {"data": instance, "files": files_payload}
             else:
                 req_args = {"json": instance}
 
             response = self._restclient.post(url, **req_args)
-            response.raise_for_status()
+            if response.is_error:
+                raise RequestError(response.status_code, response.text)
             instance = response.json()
         logger.debug(
             "Instance %s created", instance["id"], tags=LogTags.DATABASE
         )
         return instance
 
     def _update(
@@ -314,42 +320,46 @@
             if files_payload:
                 req_args = {"data": instance, "files": files_payload}
             else:
                 req_args = {"json": instance}
 
             response = self._restclient.put(url, **req_args)
 
-        response.raise_for_status()
+        if response.is_error:
+            raise RequestError(response.status_code, response.text)
         return response.json()
 
     def _create_file(self, instance: Dict, url: furl):
         response = self._restclient.post(url, data=instance)
-        response.raise_for_status()
+        if response.is_error:
+            raise RequestError(response.status_code, response.text)
         file_path = instance["file"]
         # Check is this is handled somewher
         created_instance = response.json()
         self._upload_file(created_instance, file_path=file_path)
         return created_instance
 
     def _upload_file(self, instance: Dict, file_path: str):
         api_path = self._get_api_path("file")
         resource_id = instance.get("id")
         url = self._base_url / api_path / f"{resource_id}/upload_url/"
         response = self._restclient.get(url)
-        response.raise_for_status()
+        if response.is_error:
+            raise RequestError(response.status_code, response.text)
         upload_url = response.json().get("url")
         file = open(file_path, "rb")
         file_name = instance["name"]
         with open(file_path, "rb") as fid:
             file = {"file": (file_name, fid)}
             response = requests.put(
                 upload_url,
                 files=file,
             )
-            response.raise_for_status()
+            if response.is_error:
+                raise RequestError(response.status_code, response.text)
         logger.debug(
             "File uploaded succesfully %s.", resource_id, tags=LogTags.DATABASE
         )
 
     @staticmethod
     def _get_api_path(resource_name: str) -> str:
         model_name = resource_name.lower()
```

### Comparing `splight_lib-5.6.6/splight_lib/client/datalake/abstract.py` & `splight_lib-5.7.0/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/datalake/buffer.py` & `splight_lib-5.7.0/splight_lib/client/datalake/buffer.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/datalake/builder.py` & `splight_lib-5.7.0/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/datalake/local_client.py` & `splight_lib-5.7.0/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/datalake/remote_client.py` & `splight_lib-5.7.0/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/datalake/schemas.py` & `splight_lib-5.7.0/splight_lib/client/datalake/schemas.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/exceptions.py` & `splight_lib-5.7.0/splight_lib/client/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,22 @@
     TimeoutError,
     ConnectError,
     ReadTimeout,
     SplightConnectError,
 )
 
 
+class RequestError(Exception):
+    def __init__(self, status_code: int, text: str):
+        self._msg = f"Got an error status code: {status_code} - {text}"
+
+    def __str__(self) -> str:
+        return self._msg
+
+
 class InvalidModelName(Exception):
     def __init__(self, model_name: str):
         self._msg = f"Model {model_name} is not a valid database model"
 
     def __str__(self) -> str:
         return self._msg
```

### Comparing `splight_lib-5.6.6/splight_lib/client/file_handler.py` & `splight_lib-5.7.0/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/filter.py` & `splight_lib-5.7.0/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/hub/abstract.py` & `splight_lib-5.7.0/splight_lib/client/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/hub/client.py` & `splight_lib-5.7.0/splight_lib/client/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/client/tests/test_database.py` & `splight_lib-5.7.0/splight_lib/client/tests/test_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 class MockResponse:
     status_code = 200
 
     def __init__(self, json_data):
         self.json_data = json_data
 
+    @property
+    def is_error(self) -> bool:
+        return False if self.status_code < 400 else True
+
     def raise_for_status(self):
         return None
 
     def json(self):
         return self.json_data
 
 
@@ -111,14 +115,15 @@
         access_id=access_id,
         secret_key=secret_key,
     )
 
     mock_delete = mocker.patch.object(
         SplightRestClient,
         "delete",
+        return_value=MockResponse({}),
     )
     client.delete("alert", "instance_id")
     mock_delete.assert_called_once()
 
 
 def test_delete_invalid_model_name():
     secret_key = os.getenv("SECRET_KEY")
```

### Comparing `splight_lib-5.6.6/splight_lib/client/tests/test_datalake.py` & `splight_lib-5.7.0/splight_lib/client/tests/test_datalake.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 class MockResponse:
     status_code = 200
 
     def __init__(self, json_data):
         self.json_data = json_data
 
+    @property
+    def is_error(self) -> bool:
+        return False if self.status_code < 400 else True
+
     def raise_for_status(self):
         return None
 
     def json(self):
         return self.json_data
```

### Comparing `splight_lib-5.6.6/splight_lib/component/abstract.py` & `splight_lib-5.7.0/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/component/spec.py` & `splight_lib-5.7.0/splight_lib/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/component/tests/test_spec.py` & `splight_lib-5.7.0/splight_lib/component/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/encryption.py` & `splight_lib-5.7.0/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/execution/engine.py` & `splight_lib-5.7.0/splight_lib/execution/engine.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/execution/scheduling.py` & `splight_lib-5.7.0/splight_lib/execution/scheduling.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/execution/task.py` & `splight_lib-5.7.0/splight_lib/execution/task.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/execution/tests/test_execution.py` & `splight_lib-5.7.0/splight_lib/execution/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/execution/tests/test_scheduling.py` & `splight_lib-5.7.0/splight_lib/execution/tests/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/execution/trigger.py` & `splight_lib-5.7.0/splight_lib/execution/trigger.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/logging/_internal.py` & `splight_lib-5.7.0/splight_lib/logging/_internal.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/logging/component.py` & `splight_lib-5.7.0/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/logging/logging.py` & `splight_lib-5.7.0/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/logging/tests/test_logging.py` & `splight_lib-5.7.0/splight_lib/logging/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/__init__.py` & `splight_lib-5.7.0/splight_lib/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from splight_lib.models.alert import Alert, AlertItem
-from splight_lib.models.asset import Asset
+from splight_lib.models.asset import Asset, AssetKind
 from splight_lib.models.attribute import Attribute
 from splight_lib.models.component import (
     Component,
     ComponentObject,
     ComponentObjectInstance,
     RoutineEvaluation,
     RoutineObject,
@@ -26,14 +26,15 @@
 from splight_lib.models.secret import Secret
 
 __all__ = [
     AdvancedFilter,
     Alert,
     AlertItem,
     Asset,
+    AssetKind,
     Attribute,
     Boolean,
     Chart,
     ChartItem,
     Component,
     ComponentObject,
     ComponentObjectInstance,
```

### Comparing `splight_lib-5.6.6/splight_lib/models/alert.py` & `splight_lib-5.7.0/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/asset.py` & `splight_lib-5.7.0/splight_lib/models/asset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,61 @@
 import warnings
 from typing import Any, List, Optional, Tuple
 
 from geojson_pydantic import GeometryCollection
-from pydantic import Field
+from pydantic import BaseModel, Field
 
 from splight_lib.constants import DESCRIPTION_MAX_LENGTH
 from splight_lib.models.attribute import Attribute
 from splight_lib.models.base import SplightDatabaseBaseModel
+from splight_lib.models.exceptions import MethodNotAllowed
 from splight_lib.models.metadata import Metadata
 
 warnings.filterwarnings("ignore", category=UserWarning)
 
 
+class AssetRepr(BaseModel):
+    id: str
+    name: str
+
+
+class AssetRelationship(BaseModel):
+    id: str
+    name: str
+    description: Optional[str] = None
+    related_asset_kind: Optional[str] = None
+    asset: AssetRepr
+    related_asset: AssetRepr
+
+
+class AssetKind(SplightDatabaseBaseModel):
+    id: Optional[str] = None
+    name: str
+
+    def save(self):
+        raise MethodNotAllowed("AssetKind objects are read-only")
+
+    def delete(self):
+        raise MethodNotAllowed("AssetKind objects are read-only")
+
+
 class Asset(SplightDatabaseBaseModel):
     id: Optional[str] = None
     name: str
     description: Optional[str] = Field(
         default=None, max_length=DESCRIPTION_MAX_LENGTH
     )
     tags: List[str] = []
     attributes: List[Attribute] = []
     metadata: List[Metadata] = []
     geometry: Optional[GeometryCollection] = None
     centroid_coordinates: Optional[Tuple[float, float]] = None
-    related_assets: Optional[List["Asset"]] = []
+    kind: Optional[AssetKind] = None
+    related_to: List[AssetRelationship] = []
+    related_from: List[AssetRelationship] = []
 
     def set_attribute(self, attribute: Attribute, value: Any, value_type: str):
         new_value = self._db_client.operate(
             resource_name="set-asset-attribute",
             instance={
                 "asset": self.id,
                 "attribute": attribute.id,
```

### Comparing `splight_lib-5.6.6/splight_lib/models/base.py` & `splight_lib-5.7.0/splight_lib/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     def save(self):
         files_dict = self._get_model_files_dict()
         saved = self._db_client.save(
             self.__class__.__name__,
             self.model_dump(exclude_none=True, mode="json"),
             files=files_dict,
         )
-        if not self.id:
-            self.id = saved["id"]
+        for field in self.model_fields:
+            setattr(self, field, saved.get(field))
 
     def delete(self):
         self._db_client.delete(
             resource_name=self.__class__.__name__, id=self.id
         )
 
     @classmethod
```

### Comparing `splight_lib-5.6.6/splight_lib/models/component.py` & `splight_lib-5.7.0/splight_lib/models/component.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/dashboard.py` & `splight_lib-5.7.0/splight_lib/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/data_address.py` & `splight_lib-5.7.0/splight_lib/models/data_address.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/exceptions.py` & `splight_lib-5.7.0/splight_lib/models/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+class MethodNotAllowed(Exception):
+    pass
+
+
 class InvalidObjectInstance(Exception):
     pass
 
 
 class SecretNotFound(Exception):
     def __init__(self, name: str):
         msg = f"Secret {name} not found in database"
```

### Comparing `splight_lib-5.6.6/splight_lib/models/file.py` & `splight_lib-5.7.0/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/function.py` & `splight_lib-5.7.0/splight_lib/models/function.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/generic.py` & `splight_lib-5.7.0/splight_lib/models/generic.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/hub.py` & `splight_lib-5.7.0/splight_lib/models/hub.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/hub_solution.py` & `splight_lib-5.7.0/splight_lib/models/hub_solution.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/metadata.py` & `splight_lib-5.7.0/splight_lib/models/metadata.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/native.py` & `splight_lib-5.7.0/splight_lib/models/native.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/pipeline.py` & `splight_lib-5.7.0/splight_lib/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/tests/models.json` & `splight_lib-5.7.0/splight_lib/models/tests/models.json`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/tests/test_component_object_instance.py` & `splight_lib-5.7.0/splight_lib/models/tests/test_component_object_instance.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/tests/test_database_model.py` & `splight_lib-5.7.0/splight_lib/models/tests/test_database_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from typing import Optional  # noqa: E402
 from unittest.mock import patch  # noqa: E402
 from uuid import uuid4  # noqa: E402
 
 import pytest  # noqa: E402
 
-from splight_lib.client.database.local_client import (  # noqa: E402
-    LocalDatabaseClient,
+from splight_lib.client.database.remote_client import (  # noqa: E402
+    RemoteDatabaseClient,
 )
 from splight_lib.models.base import SplightDatabaseBaseModel  # noqa: E402
 from splight_lib.settings import settings  # noqa: E402
 
 settings.configure(LOCAL_ENVIRONMENT=True)
 
 
@@ -49,26 +49,26 @@
         "name": "ObiWan",
         "age": 45,
         "saber_color": "blue",
     },
 ]
 
 
-@patch.object(LocalDatabaseClient, "_get", return_value=RESOURCE_LIST)
+@patch.object(RemoteDatabaseClient, "_get", return_value=RESOURCE_LIST)
 def test_list(mock):
     instances = Resource.list()
     mock.assert_called_with(Resource.__name__)
     assert all([isinstance(item, Resource) for item in instances])
     assert all(
         [item.id == RESOURCE_LIST[idx]["id"]]
         for idx, item in enumerate(instances)
     )
 
 
-@patch.object(LocalDatabaseClient, "_get", return_value=RESOURCE_LIST)
+@patch.object(RemoteDatabaseClient, "_get", return_value=RESOURCE_LIST)
 def test_list_first(mock):
     instances = Resource.list(first=True)
     mock.assert_called_with(Resource.__name__, first=True)
     assert all([isinstance(item, Resource) for item in instances])
     assert all(
         [item.id == RESOURCE_LIST[idx]["id"]]
         for idx, item in enumerate(instances)
@@ -77,57 +77,83 @@
 
 @pytest.mark.parametrize(
     "instance_dict",
     RESOURCE_LIST,
 )
 def test_retrieve(instance_dict):
     with patch.object(
-        LocalDatabaseClient, "_get", return_value=instance_dict
+        RemoteDatabaseClient, "_get", return_value=instance_dict
     ) as mock:
-        instance = Resource.retrieve(instance_dict["id"])
-        mock.assert_called_with(Resource.__name__, id=instance.id, first=True)
-        assert instance.model_dump() == instance_dict
+        with patch.object(
+            RemoteDatabaseClient,
+            "_get_api_path",
+            return_value="/api/resource/",
+        ):
+            instance = Resource.retrieve(instance_dict["id"])
+            mock.assert_called_with(
+                Resource.__name__, id=instance.id, first=True
+            )
+            assert instance.model_dump() == instance_dict
 
 
 @pytest.mark.parametrize(
     "instance_dict",
     RESOURCE_LIST,
 )
 def test_save_with_id(instance_dict):
     with patch.object(
-        LocalDatabaseClient, "save", return_value=instance_dict
+        RemoteDatabaseClient, "save", return_value=instance_dict
     ) as mock:
-        resource = Resource.model_validate(instance_dict)
-        resource.save()
-        mock.assert_called_with(Resource.__name__, instance_dict, files=None)
-        assert resource.model_dump() == instance_dict
+        with patch.object(
+            RemoteDatabaseClient,
+            "_get_api_path",
+            return_value="/api/resource/",
+        ):
+            resource = Resource.model_validate(instance_dict)
+            resource.save()
+            mock.assert_called_with(
+                Resource.__name__, instance_dict, files=None
+            )
+            assert resource.model_dump() == instance_dict
 
 
 @pytest.mark.parametrize(
     "instance_dict",
     RESOURCE_LIST,
 )
 def test_save_without_id(instance_dict):
     with patch.object(
-        LocalDatabaseClient, "save", return_value=instance_dict
+        RemoteDatabaseClient, "save", return_value=instance_dict
     ) as mock:
-        resource = Resource.model_validate(instance_dict)
-        resource.id = None
-        resource_dict = resource.model_dump(exclude_none=True)
-        resource.save()
-        mock.assert_called_with(Resource.__name__, resource_dict, files=None)
-        assert resource.model_dump() == instance_dict
+        with patch.object(
+            RemoteDatabaseClient,
+            "_get_api_path",
+            return_value="/api/resource/",
+        ):
+            resource = Resource.model_validate(instance_dict)
+            resource.id = None
+            resource_dict = resource.model_dump(exclude_none=True)
+            resource.save()
+            mock.assert_called_with(
+                Resource.__name__, resource_dict, files=None
+            )
+            assert resource.model_dump() == instance_dict
 
 
 @pytest.mark.parametrize(
     "instance_dict",
     RESOURCE_LIST,
 )
 def test_delete(instance_dict):
     with patch.object(
-        LocalDatabaseClient, "delete", return_value=None
+        RemoteDatabaseClient, "delete", return_value=instance_dict
     ) as mock:
-        resource = Resource.model_validate(instance_dict)
-        resource.delete()
-        mock.assert_called_with(
-            resource_name=Resource.__name__, id=resource.id
-        )
+        with patch.object(
+            RemoteDatabaseClient,
+            "_get_api_path",
+            return_value="/api/resource/",
+        ):
+            resource = Resource.model_validate(instance_dict)
+            resource.delete()
+            mock.assert_called_with(
+                resource_name=Resource.__name__, id=resource.id
+            )
```

### Comparing `splight_lib-5.6.6/splight_lib/models/tests/test_metadata.py` & `splight_lib-5.7.0/splight_lib/models/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/models/tests/test_models.py` & `splight_lib-5.7.0/splight_lib/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/restclient/client.py` & `splight_lib-5.7.0/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/restclient/exceptions.py` & `splight_lib-5.7.0/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/restclient/tests/test_restclient.py` & `splight_lib-5.7.0/splight_lib/restclient/tests/test_restclient.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/restclient/types.py` & `splight_lib-5.7.0/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/settings.py` & `splight_lib-5.7.0/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/testing/__init__.py` & `splight_lib-5.7.0/splight_lib/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/tests/asset_geometries.json` & `splight_lib-5.7.0/splight_lib/tests/asset_geometries.json`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/tests/test_api_contracts.py` & `splight_lib-5.7.0/splight_lib/tests/test_api_contracts.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/utils/custom_model.py` & `splight_lib-5.7.0/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/splight_lib/utils/hub.py` & `splight_lib-5.7.0/splight_lib/utils/hub.py`

 * *Files identical despite different names*

### Comparing `splight_lib-5.6.6/PKG-INFO` & `splight_lib-5.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 5.6.6
+Version: 5.7.0
 Summary: Splight Library
 Author: Splight Dev
 Author-email: dev@splight-ae.com
 Requires-Python: >=3.8.1,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

