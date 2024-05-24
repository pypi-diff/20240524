# Comparing `tmp/pulumi_dbtcloud-0.2.0a1716230957.tar.gz` & `tmp/pulumi_dbtcloud-0.2.0a1716506595.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_dbtcloud-0.2.0a1716230957.tar", last modified: Mon May 20 18:51:56 2024, max compression
+gzip compressed data, was "pulumi_dbtcloud-0.2.0a1716506595.tar", last modified: Thu May 23 23:41:21 2024, max compression
```

## Comparing `pulumi_dbtcloud-0.2.0a1716230957.tar` & `pulumi_dbtcloud-0.2.0a1716506595.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:51:56.350298 pulumi_dbtcloud-0.2.0a1716230957/
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-20 18:51:56.350298 pulumi_dbtcloud-0.2.0a1716230957/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:51:56.346298 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/
--rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    58952 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/big_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/big_query_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:51:56.350298 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    44015 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    29643 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    14311 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment_variable_job_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    17531 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/extended_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/fabric_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26070 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/fabric_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_azure_dev_ops_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_azure_dev_ops_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_big_query_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_big_query_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_databricks_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_extended_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_privatelink_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    15719 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    68381 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/license_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    29421 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22244 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/postgres_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_artefacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    38478 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/service_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    28611 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/snowflake_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    21154 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:51:56.350298 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-20 18:51:56.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-20 18:51:56.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:51:56.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 18:51:56.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 18:51:56.000000 pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-20 18:51:50.000000 pulumi_dbtcloud-0.2.0a1716230957/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:51:56.350298 pulumi_dbtcloud-0.2.0a1716230957/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     6464 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58952 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/big_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13597 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/big_query_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44015 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29643 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14311 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15591 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment_variable_job_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14286 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/extended_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/fabric_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26070 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/fabric_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_azure_dev_ops_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_azure_dev_ops_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_big_query_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_big_query_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_databricks_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_extended_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_privatelink_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15719 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68381 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/license_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29421 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22244 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/postgres_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8750 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_artefacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    38478 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/service_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28611 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/snowflake_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21154 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-23 23:41:21.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-23 23:41:21.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:41:21.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 23:41:21.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 23:41:21.000000 pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-23 23:41:15.000000 pulumi_dbtcloud-0.2.0a1716506595/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 23:41:21.983166 pulumi_dbtcloud-0.2.0a1716506595/setup.cfg
```

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/PKG-INFO` & `pulumi_dbtcloud-0.2.0a1716506595/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dbtcloud
-Version: 0.2.0a1716230957
+Version: 0.2.0a1716506595
 Summary: A Pulumi package for creating and managing dbt Cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-dbtcloud
 Keywords: pulumi,dbtcloud,dbt,cloud,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/README.md` & `pulumi_dbtcloud-0.2.0a1716506595/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/__init__.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/_inputs.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/_utilities.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/big_query_connection.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/big_query_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/big_query_credential.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/big_query_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/__init__.pyi` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/config/vars.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/connection.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/databricks_credential.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/databricks_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment_variable.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/environment_variable_job_override.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/environment_variable_job_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/extended_attributes.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/extended_attributes.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,35 +15,25 @@
 class ExtendedAttributesArgs:
     def __init__(__self__, *,
                  extended_attributes: pulumi.Input[str],
                  project_id: pulumi.Input[int],
                  state: Optional[pulumi.Input[int]] = None):
         """
         The set of arguments for constructing a ExtendedAttributes resource.
-        :param pulumi.Input[str] extended_attributes: A JSON string listing the extended attributes mapping. The keys are the connections attributes available in the
-               `profiles.yml` for a given adapter. Any fields entered will override connection details or credentials set on the
-               environment or project. To avoid incorrect Terraform diffs, it is recommended to create this string using `jsonencode`
-               in your Terraform code. (see example)
         :param pulumi.Input[int] project_id: Project ID to create the extended attributes in
         :param pulumi.Input[int] state: Extended Attributes state (1 is active, 2 is inactive)
         """
         pulumi.set(__self__, "extended_attributes", extended_attributes)
         pulumi.set(__self__, "project_id", project_id)
         if state is not None:
             pulumi.set(__self__, "state", state)
 
     @property
     @pulumi.getter(name="extendedAttributes")
     def extended_attributes(self) -> pulumi.Input[str]:
-        """
-        A JSON string listing the extended attributes mapping. The keys are the connections attributes available in the
-        `profiles.yml` for a given adapter. Any fields entered will override connection details or credentials set on the
-        environment or project. To avoid incorrect Terraform diffs, it is recommended to create this string using `jsonencode`
-        in your Terraform code. (see example)
-        """
         return pulumi.get(self, "extended_attributes")
 
     @extended_attributes.setter
     def extended_attributes(self, value: pulumi.Input[str]):
         pulumi.set(self, "extended_attributes", value)
 
     @property
@@ -76,18 +66,14 @@
     def __init__(__self__, *,
                  extended_attributes: Optional[pulumi.Input[str]] = None,
                  extended_attributes_id: Optional[pulumi.Input[int]] = None,
                  project_id: Optional[pulumi.Input[int]] = None,
                  state: Optional[pulumi.Input[int]] = None):
         """
         Input properties used for looking up and filtering ExtendedAttributes resources.
-        :param pulumi.Input[str] extended_attributes: A JSON string listing the extended attributes mapping. The keys are the connections attributes available in the
-               `profiles.yml` for a given adapter. Any fields entered will override connection details or credentials set on the
-               environment or project. To avoid incorrect Terraform diffs, it is recommended to create this string using `jsonencode`
-               in your Terraform code. (see example)
         :param pulumi.Input[int] extended_attributes_id: Extended Attributes ID
         :param pulumi.Input[int] project_id: Project ID to create the extended attributes in
         :param pulumi.Input[int] state: Extended Attributes state (1 is active, 2 is inactive)
         """
         if extended_attributes is not None:
             pulumi.set(__self__, "extended_attributes", extended_attributes)
         if extended_attributes_id is not None:
@@ -96,20 +82,14 @@
             pulumi.set(__self__, "project_id", project_id)
         if state is not None:
             pulumi.set(__self__, "state", state)
 
     @property
     @pulumi.getter(name="extendedAttributes")
     def extended_attributes(self) -> Optional[pulumi.Input[str]]:
-        """
-        A JSON string listing the extended attributes mapping. The keys are the connections attributes available in the
-        `profiles.yml` for a given adapter. Any fields entered will override connection details or credentials set on the
-        environment or project. To avoid incorrect Terraform diffs, it is recommended to create this string using `jsonencode`
-        in your Terraform code. (see example)
-        """
         return pulumi.get(self, "extended_attributes")
 
     @extended_attributes.setter
     def extended_attributes(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "extended_attributes", value)
 
     @property
@@ -201,18 +181,14 @@
 
         ```sh
         $ pulumi import dbtcloud:index/extendedAttributes:ExtendedAttributes test_extended_attributes 12345:6789
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] extended_attributes: A JSON string listing the extended attributes mapping. The keys are the connections attributes available in the
-               `profiles.yml` for a given adapter. Any fields entered will override connection details or credentials set on the
-               environment or project. To avoid incorrect Terraform diffs, it is recommended to create this string using `jsonencode`
-               in your Terraform code. (see example)
         :param pulumi.Input[int] project_id: Project ID to create the extended attributes in
         :param pulumi.Input[int] state: Extended Attributes state (1 is active, 2 is inactive)
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -315,18 +291,14 @@
         """
         Get an existing ExtendedAttributes resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] extended_attributes: A JSON string listing the extended attributes mapping. The keys are the connections attributes available in the
-               `profiles.yml` for a given adapter. Any fields entered will override connection details or credentials set on the
-               environment or project. To avoid incorrect Terraform diffs, it is recommended to create this string using `jsonencode`
-               in your Terraform code. (see example)
         :param pulumi.Input[int] extended_attributes_id: Extended Attributes ID
         :param pulumi.Input[int] project_id: Project ID to create the extended attributes in
         :param pulumi.Input[int] state: Extended Attributes state (1 is active, 2 is inactive)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ExtendedAttributesState.__new__(_ExtendedAttributesState)
@@ -336,20 +308,14 @@
         __props__.__dict__["project_id"] = project_id
         __props__.__dict__["state"] = state
         return ExtendedAttributes(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="extendedAttributes")
     def extended_attributes(self) -> pulumi.Output[str]:
-        """
-        A JSON string listing the extended attributes mapping. The keys are the connections attributes available in the
-        `profiles.yml` for a given adapter. Any fields entered will override connection details or credentials set on the
-        environment or project. To avoid incorrect Terraform diffs, it is recommended to create this string using `jsonencode`
-        in your Terraform code. (see example)
-        """
         return pulumi.get(self, "extended_attributes")
 
     @property
     @pulumi.getter(name="extendedAttributesId")
     def extended_attributes_id(self) -> pulumi.Output[int]:
         """
         Extended Attributes ID
```

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/fabric_connection.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/fabric_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/fabric_credential.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/fabric_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_azure_dev_ops_project.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_azure_dev_ops_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_azure_dev_ops_repository.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_azure_dev_ops_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_big_query_connection.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_big_query_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_big_query_credential.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_big_query_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_connection.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_databricks_credential.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_databricks_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_environment.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_environment_variable.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_environment_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_extended_attributes.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_extended_attributes.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_group.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_group_users.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_group_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_job.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_notification.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_postgres_credential.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_postgres_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_privatelink_endpoint.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_privatelink_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_project.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_repository.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_service_token.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_service_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_snowflake_credential.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_snowflake_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_user.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_user_groups.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/get_webhook.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/get_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/group.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/job.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/license_map.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/license_map.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/notification.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/outputs.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/postgres_credential.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/postgres_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_artefacts.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_artefacts.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_connection.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/project_repository.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/project_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/provider.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/repository.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/service_token.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/service_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/snowflake_credential.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/snowflake_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/user_groups.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/user_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud/webhook.py` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/PKG-INFO` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dbtcloud
-Version: 0.2.0a1716230957
+Version: 0.2.0a1716506595
 Summary: A Pulumi package for creating and managing dbt Cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-dbtcloud
 Keywords: pulumi,dbtcloud,dbt,cloud,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dbtcloud-0.2.0a1716230957/pulumi_dbtcloud.egg-info/SOURCES.txt` & `pulumi_dbtcloud-0.2.0a1716506595/pulumi_dbtcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

