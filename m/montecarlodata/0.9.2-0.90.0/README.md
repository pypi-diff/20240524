# Comparing `tmp/montecarlodata-0.9.2.tar.gz` & `tmp/montecarlodata-0.90.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/montecarlodata-0.9.2.tar", last modified: Tue Sep  7 18:37:01 2021, max compression
+gzip compressed data, was "dist/montecarlodata-0.90.0.tar", last modified: Fri May 24 17:04:21 2024, max compression
```

## Comparing `montecarlodata-0.9.2.tar` & `montecarlodata-0.90.0.tar`

### file list

```diff
@@ -1,77 +1,275 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.450244 montecarlodata-0.9.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7041 2021-09-07 18:37:01.450244 montecarlodata-0.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6345 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.446244 montecarlodata-0.9.2/montecarlodata/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3331 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.446244 montecarlodata-0.9.2/montecarlodata/collector/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/collector/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6268 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/collector/commands.py
--rw-r--r--   0 root         (0) root         (0)      523 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/collector/fields.py
--rw-r--r--   0 root         (0) root         (0)     9844 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/collector/management.py
--rw-r--r--   0 root         (0) root         (0)     1541 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/collector/network_tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.446244 montecarlodata-0.9.2/montecarlodata/common/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      337 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/common/commands.py
--rw-r--r--   0 root         (0) root         (0)      271 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/common/common.py
--rw-r--r--   0 root         (0) root         (0)     1963 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/common/data.py
--rw-r--r--   0 root         (0) root         (0)     6460 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/common/resources.py
--rw-r--r--   0 root         (0) root         (0)     2729 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/common/user.py
--rw-r--r--   0 root         (0) root         (0)     2162 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.446244 montecarlodata-0.9.2/montecarlodata/discovery/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/discovery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1909 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/discovery/commands.py
--rw-r--r--   0 root         (0) root         (0)     1768 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/errors.py
--rw-r--r--   0 root         (0) root         (0)      100 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/fs_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.446244 montecarlodata-0.9.2/montecarlodata/iac/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/iac/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1760 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/iac/client.py
--rw-r--r--   0 root         (0) root         (0)     2101 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/iac/commands.py
--rw-r--r--   0 root         (0) root         (0)     9102 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/iac/mc_config_service.py
--rw-r--r--   0 root         (0) root         (0)     1769 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/iac/schemas.py
--rw-r--r--   0 root         (0) root         (0)     1175 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/iac/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.446244 montecarlodata-0.9.2/montecarlodata/integrations/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22781 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.446244 montecarlodata-0.9.2/montecarlodata/integrations/info/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/info/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2850 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/info/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.450244 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9378 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.450244 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/bi/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/bi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3700 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/bi/reports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.450244 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1486 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/events.py
--rw-r--r--   0 root         (0) root         (0)     1346 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/glue_athena.py
--rw-r--r--   0 root         (0) root         (0)     2514 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/hive.py
--rw-r--r--   0 root         (0) root         (0)     1653 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/presto.py
--rw-r--r--   0 root         (0) root         (0)     1464 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/spark.py
--rw-r--r--   0 root         (0) root         (0)     3941 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.450244 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/operations/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3277 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/operations/connection_ops.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.450244 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/warehouse/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/warehouse/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2355 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/integrations/onboarding/warehouse/warehouses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.450244 montecarlodata-0.9.2/montecarlodata/queries/
--rw-r--r--   0 root         (0) root         (0)        0 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/queries/__init__.py
--rw-r--r--   0 root         (0) root         (0)      972 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/queries/collector.py
--rw-r--r--   0 root         (0) root         (0)      810 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/queries/iac.py
--rw-r--r--   0 root         (0) root         (0)     7963 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/queries/onboarding.py
--rw-r--r--   0 root         (0) root         (0)      912 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/queries/user.py
--rw-r--r--   0 root         (0) root         (0)     1546 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/settings.py
--rw-r--r--   0 root         (0) root         (0)     4415 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/tools.py
--rw-r--r--   0 root         (0) root         (0)     9268 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/montecarlodata/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-09-07 18:37:01.446244 montecarlodata-0.9.2/montecarlodata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7041 2021-09-07 18:37:01.000000 montecarlodata-0.9.2/montecarlodata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2318 2021-09-07 18:37:01.000000 montecarlodata-0.9.2/montecarlodata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-09-07 18:37:01.000000 montecarlodata-0.9.2/montecarlodata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       81 2021-09-07 18:37:01.000000 montecarlodata-0.9.2/montecarlodata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      494 2021-09-07 18:37:01.000000 montecarlodata-0.9.2/montecarlodata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-09-07 18:37:01.000000 montecarlodata-0.9.2/montecarlodata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2021-09-07 18:37:01.450244 montecarlodata-0.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1430 2021-09-07 18:36:48.000000 montecarlodata-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.577638 montecarlodata-0.90.0/.circleci/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/.circleci/README.md
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/.circleci/config.yml
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/.coveragerc
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/.dockerignore
+-rw-r--r--   0 root         (0) root         (0)       41 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/.git-blame-ignore-revs
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      140 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      212 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6893 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5672 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.581638 montecarlodata-0.90.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.581638 montecarlodata-0.90.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)      302 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/docs/_static/403.html
+-rw-r--r--   0 root         (0) root         (0)      292 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/docs/_static/404.html
+-rw-r--r--   0 root         (0) root         (0)     5132 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/docs/_static/logo.png
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/docs/_static/robots.txt
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      800 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.581638 montecarlodata-0.90.0/montecarlodata/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.581638 montecarlodata-0.90.0/montecarlodata/agents/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/agents/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17387 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/agents/agent.py
+-rw-r--r--   0 root         (0) root         (0)    11271 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/agents/commands.py
+-rw-r--r--   0 root         (0) root         (0)      624 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/agents/fields.py
+-rw-r--r--   0 root         (0) root         (0)     3519 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.585638 montecarlodata-0.90.0/montecarlodata/collector/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/collector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8956 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/collector/commands.py
+-rw-r--r--   0 root         (0) root         (0)      524 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/collector/fields.py
+-rw-r--r--   0 root         (0) root         (0)    15795 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/collector/management.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/collector/network_tests.py
+-rw-r--r--   0 root         (0) root         (0)    15033 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/collector/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.585638 montecarlodata-0.90.0/montecarlodata/common/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/common/commands.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/common/common.py
+-rw-r--r--   0 root         (0) root         (0)     5380 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/common/data.py
+-rw-r--r--   0 root         (0) root         (0)      686 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/common/echo_utils.py
+-rw-r--r--   0 root         (0) root         (0)    44216 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/common/resources.py
+-rw-r--r--   0 root         (0) root         (0)     5915 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/common/user.py
+-rw-r--r--   0 root         (0) root         (0)     4220 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.585638 montecarlodata-0.90.0/montecarlodata/dataimport/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/dataimport/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/dataimport/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.585638 montecarlodata-0.90.0/montecarlodata/dataimport/dbt/
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/dataimport/dbt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/dataimport/dbt/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.585638 montecarlodata-0.90.0/montecarlodata/discovery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/discovery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6235 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/discovery/commands.py
+-rw-r--r--   0 root         (0) root         (0)    15343 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/discovery/networking.py
+-rw-r--r--   0 root         (0) root         (0)     9395 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/discovery/policy_gen.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/errors.py
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/fs_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.585638 montecarlodata-0.90.0/montecarlodata/iac/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/iac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/iac/client.py
+-rw-r--r--   0 root         (0) root         (0)     8679 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/iac/commands.py
+-rw-r--r--   0 root         (0) root         (0)    34512 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/iac/mc_config_service.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/iac/schemas.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/iac/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.585638 montecarlodata-0.90.0/montecarlodata/insights/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/insights/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4394 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/insights/commands.py
+-rw-r--r--   0 root         (0) root         (0)     5026 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/insights/data_insights.py
+-rw-r--r--   0 root         (0) root         (0)      739 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/insights/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.589638 montecarlodata-0.90.0/montecarlodata/integrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73114 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.589638 montecarlodata-0.90.0/montecarlodata/integrations/configure/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/configure/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.589638 montecarlodata-0.90.0/montecarlodata/integrations/configure/bi/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/configure/bi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/configure/bi/bi.py
+-rw-r--r--   0 root         (0) root         (0)      319 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/configure/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.589638 montecarlodata-0.90.0/montecarlodata/integrations/info/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/info/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/info/status.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.589638 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13680 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.589638 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/bi/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/bi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3353 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/bi/reports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.589638 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6619 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/databricks.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/events.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/glue_athena.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/hive.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/presto.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/spark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.589638 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/etl/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/etl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/etl/airflow.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/etl/dbt_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/etl/fivetran.py
+-rw-r--r--   0 root         (0) root         (0)     9167 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.589638 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/operations/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/operations/connection_ops.py
+-rw-r--r--   0 root         (0) root         (0)     2434 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/self_hosted_credentials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.589638 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/streaming/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/streaming/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11639 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/streaming/streamings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.593638 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/transactional/
+-rw-r--r--   0 root         (0) root         (0)      122 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/transactional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1315 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/transactional/transactional_db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.593638 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/vector/
+-rw-r--r--   0 root         (0) root         (0)     1928 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/vector/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.593638 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/warehouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/warehouse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/integrations/onboarding/warehouse/warehouses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.593638 montecarlodata-0.90.0/montecarlodata/keys/
+-rw-r--r--   0 root         (0) root         (0)     1720 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/keys/airflow.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/keys/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.593638 montecarlodata-0.90.0/montecarlodata/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/management/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3437 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/management/commands.py
+-rw-r--r--   0 root         (0) root         (0)     6841 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/management/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.593638 montecarlodata-0.90.0/montecarlodata/monitors/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/monitors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/monitors/monitor_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.593638 montecarlodata-0.90.0/montecarlodata/queries/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/queries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      498 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/queries/bi.py
+-rw-r--r--   0 root         (0) root         (0)      976 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/queries/catalog.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/queries/collector.py
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/queries/common.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/queries/iac.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/queries/insights.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/queries/keys.py
+-rw-r--r--   0 root         (0) root         (0)    24449 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/queries/onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/queries/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.593638 montecarlodata-0.90.0/montecarlodata/secrets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/secrets/commands.py
+-rw-r--r--   0 root         (0) root         (0)     5526 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/secrets/service.py
+-rw-r--r--   0 root         (0) root         (0)     2732 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.593638 montecarlodata-0.90.0/montecarlodata/templates/
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/templates/athena_policy.json
+-rw-r--r--   0 root         (0) root         (0)     1810 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/templates/aws_role.json
+-rw-r--r--   0 root         (0) root         (0)     1741 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/templates/glue_policy.json
+-rw-r--r--   0 root         (0) root         (0)      557 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/templates/msk_policy.json
+-rw-r--r--   0 root         (0) root         (0)     6686 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/tools.py
+-rw-r--r--   0 root         (0) root         (0)    15423 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/montecarlodata/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/montecarlodata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6893 2024-05-24 17:04:21.000000 montecarlodata-0.90.0/montecarlodata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8634 2024-05-24 17:04:21.000000 montecarlodata-0.90.0/montecarlodata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 17:04:21.000000 montecarlodata-0.90.0/montecarlodata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-05-24 17:04:21.000000 montecarlodata-0.90.0/montecarlodata.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      211 2024-05-24 17:04:21.000000 montecarlodata-0.90.0/montecarlodata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-24 17:04:21.000000 montecarlodata-0.90.0/montecarlodata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/requirements-ci.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)      211 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-24 17:04:21.609638 montecarlodata-0.90.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1576 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      662 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/common/test_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/dataimport/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/dataimport/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5284 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/dataimport/test_dbt_import_service.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53682 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_mc_config_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.577638 montecarlodata-0.90.0/tests/iac/test_resources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/convert_to_mac/
+-rw-r--r--   0 root         (0) root         (0)       74 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/convert_to_mac/monitors_uuids
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs/dbt_models/
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs/dbt_models/schema.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs/dbt_models/subdir/
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs/dbt_models/subdir/schema.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs/dir1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs/dir1/dir2/
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs/dir1/dir2/monitors.yml
+-rw-r--r--   0 root         (0) root         (0)       98 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs/dir1/monitors.yml
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs/montecarlo.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/dbt_models/
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/dbt_models/schema.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/dbt_models/subdir/
+-rw-r--r--   0 root         (0) root         (0)      840 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/dbt_models/subdir/schema.yml
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/dbt_project.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/dir1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/dir1/dir2/
+-rw-r--r--   0 root         (0) root         (0)      164 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/dir1/dir2/monitors.yml
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/dir1/monitors.yml
+-rw-r--r--   0 root         (0) root         (0)      648 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/manifest.json
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/embedded_dbt_configs_with_refs/montecarlo.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.601638 montecarlodata-0.90.0/tests/iac/test_resources/import_dbt_tests/
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/import_dbt_tests/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3758 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/import_dbt_tests/expected.yml
+-rw-r--r--   0 root         (0) root         (0)     4395 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/import_dbt_tests/manifest.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/invalid_configs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/invalid_configs/dir1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/invalid_configs/dir1/dir2/
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/invalid_configs/dir1/dir2/monitors.yml
+-rw-r--r--   0 root         (0) root         (0)      118 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/invalid_configs/dir1/monitors.yml
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/invalid_configs/montecarlo.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override/dbt_models/
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override/dbt_models/schema.yml
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override/monitors.yaml
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override/monitors_other.yml
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override/montecarlo.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_montecarlo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_montecarlo/dbt_models/
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_montecarlo/dbt_models/schema.yml
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_montecarlo/monitors.yml
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_montecarlo/monitors_other.yml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_montecarlo/montecarlo.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_yaml/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_yaml/dbt_models/
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_yaml/dbt_models/schema.yml
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_yaml/monitors.yaml
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_yaml/monitors_other.yml
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/namespace_override_yaml/montecarlo.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/standalone_configs/
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/standalone_configs/dbt_project.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/standalone_configs/dir1/
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/standalone_configs/dir1/another_file.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 17:04:21.605638 montecarlodata-0.90.0/tests/iac/test_resources/standalone_configs/dir1/dir2/
+-rw-r--r--   0 root         (0) root         (0)      220 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/standalone_configs/dir1/dir2/monitors.yml
+-rw-r--r--   0 root         (0) root         (0)      311 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/standalone_configs/dir1/dir2/monitors_additional.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/standalone_configs/dir1/emptyfile.yml
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/standalone_configs/dir1/monitors.yml
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/iac/test_resources/standalone_configs/montecarlo.yml
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/sample_mapping.json
+-rw-r--r--   0 root         (0) root         (0)     4169 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_airflow_keys.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_airflow_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     5828 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_aws_util.py
+-rw-r--r--   0 root         (0) root         (0)    26602 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_base_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)    21034 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_collector_management.py
+-rw-r--r--   0 root         (0) root         (0)     2021 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_collector_network_tests.py
+-rw-r--r--   0 root         (0) root         (0)    47120 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_common_resources.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_common_user.py
+-rw-r--r--   0 root         (0) root         (0)     2944 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     4467 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_connection_ops.py
+-rw-r--r--   0 root         (0) root         (0)     8815 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_data_insights.py
+-rw-r--r--   0 root         (0) root         (0)    10890 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_databricks_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     4552 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_dbt_cloud_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     5122 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_events_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     2539 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_fivetran_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_glue_athena_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_gql_util.py
+-rw-r--r--   0 root         (0) root         (0)     3410 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_hive_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)    10280 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_integration_keys.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_integration_status.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_monitor_service.py
+-rw-r--r--   0 root         (0) root         (0)    19757 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_network_discovery.py
+-rw-r--r--   0 root         (0) root         (0)    15129 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_policy_gen_discovery.py
+-rw-r--r--   0 root         (0) root         (0)     2351 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_presto_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     3925 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_report_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     9597 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_secrets.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_self_hosted_credentials_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     3049 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_spark_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     7038 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_streaming_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_transactional_db_onboarding.py
+-rw-r--r--   0 root         (0) root         (0)     5610 2024-05-24 17:03:56.000000 montecarlodata-0.90.0/tests/test_warehouse_onboarding.py
```

### Comparing `montecarlodata-0.9.2/LICENSE` & `montecarlodata-0.90.0/LICENSE`

 * *Files identical despite different names*

### Comparing `montecarlodata-0.9.2/PKG-INFO` & `montecarlodata-0.90.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,159 +1,185 @@
 Metadata-Version: 2.1
 Name: montecarlodata
-Version: 0.9.2
+Version: 0.90.0
 Summary: Monte Carlo's CLI
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3>=1.19.4
+Requires-Dist: click>=8.1.3
+Requires-Dist: click-config-file==0.6.0
+Requires-Dist: requests<=3.0.0,>=2.0.0
+Requires-Dist: retry==0.9.2
+Requires-Dist: tabulate>=0.8.7
+Requires-Dist: dataclasses-json>=0.5.4
+Requires-Dist: PyYAML>=5.4.1
+Requires-Dist: python-box>=6.0.0
+Requires-Dist: pycarlo>=0.8.12
+Requires-Dist: Jinja2>=3.1.2
+Requires-Dist: questionary==1.10.0
 
 # Monte Carlo CLI
+
 Monte Carlo's Alpha CLI!
 
 ## Installation
-Requires Python 3.7 or greater. Normally you can install and update using pip. For instance: 
-```
+
+Requires Python 3.8 or greater. Normally you can install and update using `pip`. For instance:
+
+```shell
+pip install virtualenv
 virtualenv venv
 . venv/bin/activate
 
 pip install -U montecarlodata
 ```
+
 Developers of the CLI can use:
-```
-make install 
+
+```shell
+pip install virtualenv
+make install
 . venv/bin/activate
+pre-commit install
 ```
 
 Either way confirm the installation by running:
-```
+
+```shell
 montecarlo --version
 ```
 
-If the Python requirement does not work for you please reach out to `customer-success@montecarlodata.com`. Docker is an option.
+If the Python requirement does not work for you please reach out to `support@montecarlodata.com`. Docker is an option.
 
 ## Quick start
+
 First time users can configure the tool by following the onscreen prompts:
-```
+
+```shell
 montecarlo configure
 ```
-MCD tokens can be generated from the [dashboard](https://getmontecarlo.com/settings/api).
- 
-Any AWS profiles or regions should be for the account the Data Collector (DC) is deployed to. If you are not using the
-CLI for onboarding, you may leave the AWS configuration blank.
 
-Use the `--help` flag for details on any advanced options (e.g. creating multiple montecarlo profiles) or any prompts.
+MCD tokens can be generated from the [dashboard](https://getmontecarlo.com/get-token).
+
+Use the `--help` flag for details on any advanced options (e.g. creating multiple montecarlo profiles) or
+see docs [here][cli-docs].
 
 That's it! You can always validate your connection with:
-```
+
+```shell
 montecarlo validate
 ```
 
 ## User settings
-Any configuration set by `montecarlo configure` can be found in '~/.mcd/' by default.
+
+Any configuration set by `montecarlo configure` can be found in `~/.mcd/` by default.
 
 The MCD ID and Token can be overwritten, or even set, by the environment:
-- MCD_DEFAULT_API_ID
-- MCD_DEFAULT_API_TOKEN
 
-These two are required either as part of `configure` or as environment variables. 
-For AWS, system defaults are used if not set as part of `configure`.
+- `MCD_DEFAULT_API_ID`
+- `MCD_DEFAULT_API_TOKEN`
+
+These two are required either as part of `configure` or as environment variables.
 
 The following values can also be set by the environment:
-- MCD_API_ENDPOINT - Overwrite the default API endpoint
-- MCD_VERBOSE_ERRORS - Enable verbose logging on errors (default=false)
+
+- `MCD_API_ENDPOINT` - Overwrite the default API endpoint
+- `MCD_VERBOSE_ERRORS` - Enable verbose logging on errors (default=false)
 
 ## Help
-Help for commands, options and arguments can be found using the `--help` flag.
-Additional documentation is available [here](https://docs.getmontecarlo.com/docs).
 
-All commands, except `configure` and `validate`, support an `--option-file` flag, which allows you to use a file in place of passing options.
-For instance, a `--name` flag can be set by creating a file containing:
+Documentation for commands, options, and arguments can be found [here][cli-docs].
+
+You can also use `montecarlo help` to echo all help text or use the `--help` flag on any command.
+
+## Examples
+
+### Using Docker from a local installation
+
+```shell
+docker build -t montecarlo .
+docker run -e MCD_DEFAULT_API_ID='<ID>' -e MCD_DEFAULT_API_TOKEN='<TOKEN>' montecarlo --version
 ```
-name="Artemis"
+
+Replace `--version` with any sub-commands or options. If interacting with files those directories will probably need to be mounted too.
+
+### Configure a named profile with custom config-path
+
+```shell
+$ montecarlo configure --profile-name zeus --config-path .
+Key ID: 1234
+Secret:
+
+$ cat ./profiles.ini
+[zeus]
+mcd_id = 1234
+mcd_token = 5678
 ```
-Any dashes must be replaced by underscores. For instance, `--foo-bar` would be `foo_bar="qux"`.
 
-Resolution is CLI Options > Option File.
+### List active integrations
 
-## Examples
-- Using Docker from a local installation
-    ```
-    docker build -t montecarlo .
-    docker run -v ${HOME}/.aws/credentials:/root/.aws/credentials:ro \
-               -e MCD_DEFAULT_API_ID='<ID>' \
-               -e MCD_DEFAULT_API_TOKEN='<TOKEN>' \
-               -e AWS_DEFAULT_PROFILE='<PROFILE>' \
-               -e AWS_DEFAULT_REGION='us-east-1' \
-               montecarlo --version
-    ```
-    Replace `--version` with any sub-commands or options. If interacting with files those directories will probably need to be mounted too.
-
-
-- Configure a named profile with custom config-path
-    ```
-    $ montecarlo configure --profile-name zeus --config-path .
-    Key ID: 1234
-    Secret:
-    AWS profile name []: shiva
-    AWS region [us-east-1]:
-  
-    $  cat ./profiles.ini 
-    [zeus]
-    mcd_id = 1234
-    mcd_token = 5678
-    aws_profile = shiva
-    aws_region = us-east-1
-    ```
-  
-- List active integrations
-    ```
-    $ montecarlo integrations list
-    ╒══════════════════╤══════════════════════════════════════╤══════════════════════════════════╕
-    │ Integration      │ ID                                   │ Created on (UTC)                 │
-    ╞══════════════════╪══════════════════════════════════════╪══════════════════════════════════╡
-    │ Odin             │ 58005657-2914-4701-9a11-260ac425b14e │ 2021-01-02T01:30:52.806602+00:00 │
-    ├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
-    │ Thor             │ 926816bd-ab17-4f95-a953-fa14482c59de │ 2021-01-02T01:31:19.892205+00:00 │
-    ├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
-    │ Loki             │ 1cf1dc0d-d8ec-4c85-8e64-57ab2ad8e023 │ 2021-01-02T01:32:37.709747+00:00 │
-    ╘══════════════════╧══════════════════════════════════════╧══════════════════════════════════╛
-    ```
-
-- Apply monitors configuration
-
-    ```
-    $ montecarlo monitors apply --namespace my-monitors
-
-    Gathering monitor configuration files.
-    - models/customer_success/schema.yml - Embedded monitor configuration found.
-    - models/customer_success/schema.yml - Monitor configuration found.
-    - models/lineage/schema.yml - Embedded monitor configuration found.
-    
-    Modifications:
-    - ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod.customer_360
-    - ResourceModificationType.UPDATE - Monitor: type=categories, table=analytics:prod.customer_360
-    - ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod_lineage.lineage_nodes
-    - ResourceModificationType.UPDATE - Freshness SLI: table=analytics:prod.customer_360, freshness_threshold=30
-    ```
+```shell
+$ montecarlo integrations list
+╒══════════════════╤══════════════════════════════════════╤══════════════════════════════════╕
+│ Integration      │ ID                                   │ Created on (UTC)                 │
+╞══════════════════╪══════════════════════════════════════╪══════════════════════════════════╡
+│ Odin             │ 58005657-2914-4701-9a11-260ac425b14e │ 2021-01-02T01:30:52.806602+00:00 │
+├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
+│ Thor             │ 926816bd-ab17-4f95-a953-fa14482c59de │ 2021-01-02T01:31:19.892205+00:00 │
+├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
+│ Loki             │ 1cf1dc0d-d8ec-4c85-8e64-57ab2ad8e023 │ 2021-01-02T01:32:37.709747+00:00 │
+╘══════════════════╧══════════════════════════════════════╧══════════════════════════════════╛
+```
+
+### Apply monitors configuration
+
+```shell
+$ montecarlo monitors apply --namespace my-monitors
+
+Gathering monitor configuration files.
+- models/customer_success/schema.yml - Embedded monitor configuration found.
+- models/customer_success/schema.yml - Monitor configuration found.
+- models/lineage/schema.yml - Embedded monitor configuration found.
+
+Modifications:
+- ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod.customer_360
+- ResourceModificationType.UPDATE - Monitor: type=categories, table=analytics:prod.customer_360
+- ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod_lineage.lineage_nodes
+- ResourceModificationType.UPDATE - Freshness SLI: table=analytics:prod.customer_360, freshness_threshold=30
+```
+
+### Import DBT manifest
+
+```shell
+$ montecarlo import dbt-manifest --dbt-manifest-file target/manifest.json
+
+Importing DBT objects into Monte Carlo catalog. please wait...
+
+Imported a total of 51 DBT objects into Monte Carlo catalog.
+```
 
 ## Tests and Releases
-Locally `make test` will run all tests. CircleCI manages all testing for deployment.
 
-When ready to release make a PR for `master`. After merging CircleCI will test and deploy to [PyPI](https://pypi.org/project/montecarlodata/).
+Locally `make test` will run all tests. CircleCI manages all testing for deployment.
 
-Don't forget to increment the version number in `setup.py` first! An existing version will not be deployed.
+To publish a new release, simply add a new version tag, e.g. `v1.0.0`, and push that tag to GitHub. CircleCI will take care of publishing a new package to [PyPI](https://pypi.org/project/montecarlodata/) and generating documentation.
 
 ## License
+
 Apache 2.0 - See the [LICENSE](http://www.apache.org/licenses/LICENSE-2.0) for more information.
 
+[cli-docs]: https://clidocs.getmontecarlo.com/
```

### Comparing `montecarlodata-0.9.2/README.md` & `montecarlodata-0.90.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,138 +1,151 @@
 # Monte Carlo CLI
+
 Monte Carlo's Alpha CLI!
 
 ## Installation
-Requires Python 3.7 or greater. Normally you can install and update using pip. For instance: 
-```
+
+Requires Python 3.8 or greater. Normally you can install and update using `pip`. For instance:
+
+```shell
+pip install virtualenv
 virtualenv venv
 . venv/bin/activate
 
 pip install -U montecarlodata
 ```
+
 Developers of the CLI can use:
-```
-make install 
+
+```shell
+pip install virtualenv
+make install
 . venv/bin/activate
+pre-commit install
 ```
 
 Either way confirm the installation by running:
-```
+
+```shell
 montecarlo --version
 ```
 
-If the Python requirement does not work for you please reach out to `customer-success@montecarlodata.com`. Docker is an option.
+If the Python requirement does not work for you please reach out to `support@montecarlodata.com`. Docker is an option.
 
 ## Quick start
+
 First time users can configure the tool by following the onscreen prompts:
-```
+
+```shell
 montecarlo configure
 ```
-MCD tokens can be generated from the [dashboard](https://getmontecarlo.com/settings/api).
- 
-Any AWS profiles or regions should be for the account the Data Collector (DC) is deployed to. If you are not using the
-CLI for onboarding, you may leave the AWS configuration blank.
 
-Use the `--help` flag for details on any advanced options (e.g. creating multiple montecarlo profiles) or any prompts.
+MCD tokens can be generated from the [dashboard](https://getmontecarlo.com/get-token).
+
+Use the `--help` flag for details on any advanced options (e.g. creating multiple montecarlo profiles) or
+see docs [here][cli-docs].
 
 That's it! You can always validate your connection with:
-```
+
+```shell
 montecarlo validate
 ```
 
 ## User settings
-Any configuration set by `montecarlo configure` can be found in '~/.mcd/' by default.
+
+Any configuration set by `montecarlo configure` can be found in `~/.mcd/` by default.
 
 The MCD ID and Token can be overwritten, or even set, by the environment:
-- MCD_DEFAULT_API_ID
-- MCD_DEFAULT_API_TOKEN
 
-These two are required either as part of `configure` or as environment variables. 
-For AWS, system defaults are used if not set as part of `configure`.
+- `MCD_DEFAULT_API_ID`
+- `MCD_DEFAULT_API_TOKEN`
+
+These two are required either as part of `configure` or as environment variables.
 
 The following values can also be set by the environment:
-- MCD_API_ENDPOINT - Overwrite the default API endpoint
-- MCD_VERBOSE_ERRORS - Enable verbose logging on errors (default=false)
+
+- `MCD_API_ENDPOINT` - Overwrite the default API endpoint
+- `MCD_VERBOSE_ERRORS` - Enable verbose logging on errors (default=false)
 
 ## Help
-Help for commands, options and arguments can be found using the `--help` flag.
-Additional documentation is available [here](https://docs.getmontecarlo.com/docs).
 
-All commands, except `configure` and `validate`, support an `--option-file` flag, which allows you to use a file in place of passing options.
-For instance, a `--name` flag can be set by creating a file containing:
+Documentation for commands, options, and arguments can be found [here][cli-docs].
+
+You can also use `montecarlo help` to echo all help text or use the `--help` flag on any command.
+
+## Examples
+
+### Using Docker from a local installation
+
+```shell
+docker build -t montecarlo .
+docker run -e MCD_DEFAULT_API_ID='<ID>' -e MCD_DEFAULT_API_TOKEN='<TOKEN>' montecarlo --version
 ```
-name="Artemis"
+
+Replace `--version` with any sub-commands or options. If interacting with files those directories will probably need to be mounted too.
+
+### Configure a named profile with custom config-path
+
+```shell
+$ montecarlo configure --profile-name zeus --config-path .
+Key ID: 1234
+Secret:
+
+$ cat ./profiles.ini
+[zeus]
+mcd_id = 1234
+mcd_token = 5678
 ```
-Any dashes must be replaced by underscores. For instance, `--foo-bar` would be `foo_bar="qux"`.
 
-Resolution is CLI Options > Option File.
+### List active integrations
 
-## Examples
-- Using Docker from a local installation
-    ```
-    docker build -t montecarlo .
-    docker run -v ${HOME}/.aws/credentials:/root/.aws/credentials:ro \
-               -e MCD_DEFAULT_API_ID='<ID>' \
-               -e MCD_DEFAULT_API_TOKEN='<TOKEN>' \
-               -e AWS_DEFAULT_PROFILE='<PROFILE>' \
-               -e AWS_DEFAULT_REGION='us-east-1' \
-               montecarlo --version
-    ```
-    Replace `--version` with any sub-commands or options. If interacting with files those directories will probably need to be mounted too.
-
-
-- Configure a named profile with custom config-path
-    ```
-    $ montecarlo configure --profile-name zeus --config-path .
-    Key ID: 1234
-    Secret:
-    AWS profile name []: shiva
-    AWS region [us-east-1]:
-  
-    $  cat ./profiles.ini 
-    [zeus]
-    mcd_id = 1234
-    mcd_token = 5678
-    aws_profile = shiva
-    aws_region = us-east-1
-    ```
-  
-- List active integrations
-    ```
-    $ montecarlo integrations list
-    ╒══════════════════╤══════════════════════════════════════╤══════════════════════════════════╕
-    │ Integration      │ ID                                   │ Created on (UTC)                 │
-    ╞══════════════════╪══════════════════════════════════════╪══════════════════════════════════╡
-    │ Odin             │ 58005657-2914-4701-9a11-260ac425b14e │ 2021-01-02T01:30:52.806602+00:00 │
-    ├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
-    │ Thor             │ 926816bd-ab17-4f95-a953-fa14482c59de │ 2021-01-02T01:31:19.892205+00:00 │
-    ├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
-    │ Loki             │ 1cf1dc0d-d8ec-4c85-8e64-57ab2ad8e023 │ 2021-01-02T01:32:37.709747+00:00 │
-    ╘══════════════════╧══════════════════════════════════════╧══════════════════════════════════╛
-    ```
-
-- Apply monitors configuration
-
-    ```
-    $ montecarlo monitors apply --namespace my-monitors
-
-    Gathering monitor configuration files.
-    - models/customer_success/schema.yml - Embedded monitor configuration found.
-    - models/customer_success/schema.yml - Monitor configuration found.
-    - models/lineage/schema.yml - Embedded monitor configuration found.
-    
-    Modifications:
-    - ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod.customer_360
-    - ResourceModificationType.UPDATE - Monitor: type=categories, table=analytics:prod.customer_360
-    - ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod_lineage.lineage_nodes
-    - ResourceModificationType.UPDATE - Freshness SLI: table=analytics:prod.customer_360, freshness_threshold=30
-    ```
+```shell
+$ montecarlo integrations list
+╒══════════════════╤══════════════════════════════════════╤══════════════════════════════════╕
+│ Integration      │ ID                                   │ Created on (UTC)                 │
+╞══════════════════╪══════════════════════════════════════╪══════════════════════════════════╡
+│ Odin             │ 58005657-2914-4701-9a11-260ac425b14e │ 2021-01-02T01:30:52.806602+00:00 │
+├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
+│ Thor             │ 926816bd-ab17-4f95-a953-fa14482c59de │ 2021-01-02T01:31:19.892205+00:00 │
+├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
+│ Loki             │ 1cf1dc0d-d8ec-4c85-8e64-57ab2ad8e023 │ 2021-01-02T01:32:37.709747+00:00 │
+╘══════════════════╧══════════════════════════════════════╧══════════════════════════════════╛
+```
+
+### Apply monitors configuration
+
+```shell
+$ montecarlo monitors apply --namespace my-monitors
+
+Gathering monitor configuration files.
+- models/customer_success/schema.yml - Embedded monitor configuration found.
+- models/customer_success/schema.yml - Monitor configuration found.
+- models/lineage/schema.yml - Embedded monitor configuration found.
+
+Modifications:
+- ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod.customer_360
+- ResourceModificationType.UPDATE - Monitor: type=categories, table=analytics:prod.customer_360
+- ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod_lineage.lineage_nodes
+- ResourceModificationType.UPDATE - Freshness SLI: table=analytics:prod.customer_360, freshness_threshold=30
+```
+
+### Import DBT manifest
+
+```shell
+$ montecarlo import dbt-manifest --dbt-manifest-file target/manifest.json
+
+Importing DBT objects into Monte Carlo catalog. please wait...
+
+Imported a total of 51 DBT objects into Monte Carlo catalog.
+```
 
 ## Tests and Releases
-Locally `make test` will run all tests. CircleCI manages all testing for deployment.
 
-When ready to release make a PR for `master`. After merging CircleCI will test and deploy to [PyPI](https://pypi.org/project/montecarlodata/).
+Locally `make test` will run all tests. CircleCI manages all testing for deployment.
 
-Don't forget to increment the version number in `setup.py` first! An existing version will not be deployed.
+To publish a new release, simply add a new version tag, e.g. `v1.0.0`, and push that tag to GitHub. CircleCI will take care of publishing a new package to [PyPI](https://pypi.org/project/montecarlodata/) and generating documentation.
 
 ## License
-Apache 2.0 - See the [LICENSE](http://www.apache.org/licenses/LICENSE-2.0) for more information.
+
+Apache 2.0 - See the [LICENSE](http://www.apache.org/licenses/LICENSE-2.0) for more information.
+
+[cli-docs]: https://clidocs.getmontecarlo.com/
```

### Comparing `montecarlodata-0.9.2/montecarlodata/collector/commands.py` & `montecarlodata-0.90.0/montecarlodata/discovery/commands.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,139 +1,193 @@
+from typing import Dict, Optional, List
+
 import click
 import click_config_file
 
-import montecarlodata.settings as settings
-from montecarlodata.collector.network_tests import CollectorNetworkTestService
-from montecarlodata.collector.fields import DEFAULT_COLLECTION_REGION
-from montecarlodata.collector.management import CollectorManagementService
-from montecarlodata.tools import validate_json_callback, add_common_options
-from montecarlodata.common.commands import DISAMBIGUATE_DC_OPTIONS
+from montecarlodata import settings
+from montecarlodata.common.commands import DISAMBIGUATE_DC_OPTIONS, DC_RESOURCE_OPTIONS
+from montecarlodata.common.resources import CloudResourceService
+from montecarlodata.discovery.networking import NetworkDiscoveryService
+from montecarlodata.discovery.policy_gen import PolicyDiscoveryService
+from montecarlodata.tools import add_common_options
 
 # Shared command verbiage
-PROFILE_VERBIAGE = 'If not specified, the one in the Monte Carlo CLI profile is used'
-ADD_DC_VERBIAGE = 'Prompts to opens browser to CF console. If declined (or skipped) can use deploy, get-template ' \
-                  'or open-link with the generated ID.'
-
-# Options shared across commands
-REGION_OPTIONS = [
-    *DISAMBIGUATE_DC_OPTIONS,
-    click.option('--aws-region', required=False, default=DEFAULT_COLLECTION_REGION, show_default=True,
-                 help='AWS region where the collector is deployed or intended to be deployed.')
-]
-DEPLOYMENT_OPTIONS = [
-    click.option('--aws-profile', required=False, help=f'AWS profile. {PROFILE_VERBIAGE}.'),
-    click.option('--params', required=False, default=None, callback=validate_json_callback,
-                 help="""
-                  Parameters key,value pairs as JSON. If a key is not specified the existing (or default) value is used.
-                  \b
-                  \n
-                  E.g. --params '{"CreateEventInfra":"True"}'
-                  """),  # \b disables wrapping
-    *REGION_OPTIONS
-]
-
-NETWORK_TEST_OPTIONS = [
-    *DISAMBIGUATE_DC_OPTIONS,
-    click.option('--host', required=True, help='Host to check.'),
-    click.option('--port', required=True, type=click.INT, help='Port to check.'),
-    click.option('--timeout', required=False, default=5, type=click.INT, show_default=True, help='Timeout in seconds.')
+DISCOVERY_REVIEW_VERBIAGE = (
+    "After review, output of this command can be redirected into "
+    "`montecarlo integrations create-role` or `montecarlo discovery cf-role-gen` "
+    "if you prefer IaC"
+)
+
+GLUE_COMMON_OPTIONS = [
+    click.option(
+        "--database-name",
+        "database_names",
+        required=True,
+        multiple=True,
+        help="Glue/Athena database name to generate a policy from. Enter '\\*' to give Monte Carlo access "
+        "to all databases. This option can be passed multiple times for more than one database.",
+    ),
+    click.option(
+        "--data-bucket-name",
+        "bucket_names",
+        required=False,
+        multiple=True,
+        help="Name of a S3 bucket storing the data for your Glue/Athena tables. If this option is not "
+        "specified the bucket names are derived (looked up) from the tables in your databases. This "
+        "option can be passed multiple times for more than one bucket. Enter '\\*' to give Monte "
+        "Carlo access to all buckets.",
+    ),
 ]
 
 
-@click.group(help='Manage a data collector.')
-def collectors():
+@click.group(help="Display information about resources.")
+def discovery():
     """
-    Group for any collector related subcommands
+    Group for any discovery related subcommands
     """
     pass
 
 
-@collectors.command(help='List all collector records.', name='list')
-@click.pass_obj
-@click.option('--active-only', required=False, default=False, show_default=True, is_flag=True,
-              help='Only list active collectors.')
-@click_config_file.configuration_option(settings.OPTION_FILE_FLAG)
-def list_collectors(ctx, active_only):
-    CollectorManagementService(config=ctx['config'], aws_wrapper=None).echo_collectors(active_only=active_only)
-
-
-@collectors.command(help=f'Add a collector record to the account. {ADD_DC_VERBIAGE}', name='add')
-@click.pass_obj
-@click.option('--no-prompt', required=False, default=False, show_default=True, is_flag=True,
-              help='Skip prompt for launching browser (Auto no).')
-@click_config_file.configuration_option(settings.OPTION_FILE_FLAG)
-def add_collector(ctx, no_prompt):
-    CollectorManagementService(config=ctx['config']).add_collector(no_prompt=no_prompt)
-
-
-@collectors.command(help='Get link to the latest template. For initial deployment or manually upgrading.')
-@click.pass_obj
-@add_common_options(REGION_OPTIONS)
-@click_config_file.configuration_option(settings.OPTION_FILE_FLAG)
-def get_template(ctx, aws_region, **kwargs):
-    """
-    Get the latest template for this account
-    """
-    CollectorManagementService(config=ctx['config'], aws_region_override=aws_region).echo_template(**kwargs)
-
-
-@collectors.command(help='Opens browser to CF console with a quick create link. For initial deployment.')
-@click.pass_obj
-@click.option('--dry', required=False, default=False, show_default=True, is_flag=True, help='Echos quick create link.')
-@add_common_options(REGION_OPTIONS)
-@click_config_file.configuration_option(settings.OPTION_FILE_FLAG)
-def open_link(ctx, aws_region, **kwargs):
-    """
-    Open browser with a quick create link for deploying a data collector
-    """
-    CollectorManagementService(config=ctx['config'], aws_region_override=aws_region).launch_quick_create_link(**kwargs)
-
-
-@collectors.command(help='Deploy a data collector stack.')
-@click.pass_obj
-@add_common_options(DEPLOYMENT_OPTIONS)
-@click.option('--stack-name', required=True, help='The name that is associated with the CloudFormation stack. '
-                                                  'Must be unique in the region.')
-@click.option('--enable-termination-protection/--no-enable-termination-protection', 'termination_protection',
-              default=False, show_default=True, help='Enable termination protection for this stack.')
-@click_config_file.configuration_option(settings.OPTION_FILE_FLAG)
-def deploy(ctx, aws_profile, aws_region, params, **kwargs):
-    """
-    Deploy a collector for this account
-    """
-    CollectorManagementService(config=ctx['config'], aws_profile_override=aws_profile,
-                               aws_region_override=aws_region).deploy_template(new_params=params, **kwargs)
-
-
-@collectors.command(help='Upgrade to the latest version.')
-@click.pass_obj
-@add_common_options(DEPLOYMENT_OPTIONS)
-@click_config_file.configuration_option(settings.OPTION_FILE_FLAG)
-def upgrade(ctx, aws_profile, aws_region, params, **kwargs):
-    """
-    Upgrade the collector for this account
-    """
-    CollectorManagementService(config=ctx['config'], aws_profile_override=aws_profile,
-                               aws_region_override=aws_region).upgrade_template(new_params=params, **kwargs)
-
-
-@collectors.command(help='Checks if telnet connection is usable from the collector.')
-@click.pass_obj
-@add_common_options(NETWORK_TEST_OPTIONS)
-@click_config_file.configuration_option(settings.OPTION_FILE_FLAG)
-def test_telnet(ctx, **kwargs):
-    """
-    Network debugging utility to test telnet via the collector
-    """
-    CollectorNetworkTestService(config=ctx['config']).echo_telnet_test(**kwargs)
-
-
-@collectors.command(help='Tests if a destination exists and accepts requests. '
-                        'Opens a TCP Socket to a specific port from the collector.')
-@click.pass_obj
-@add_common_options(NETWORK_TEST_OPTIONS)
-@click_config_file.configuration_option(settings.OPTION_FILE_FLAG)
-def test_tcp_open(ctx, **kwargs):
-    """
-    Network debugging utility to test TCP open via the collector
-    """
-    CollectorNetworkTestService(config=ctx['config']).echo_tcp_open_test(**kwargs)
+@discovery.command(help="List details about EMR clusters in a region.")
+@click.option("--aws-profile", help="AWS profile.", required=True)
+@click.option("--aws-region", help="AWS region.", required=True)
+@click.option(
+    "--only-log-locations",
+    help="Display only unique log locations",
+    is_flag=True,
+    default=False,
+)
+@click.option(
+    "--created-after",
+    help="Display clusters created after date (e.g. 2017-07-04T00:01:30)",
+    required=False,
+)
+@click.option(
+    "--state",
+    help="Cluster states",
+    required=False,
+    type=click.Choice(["active", "terminated", "failed"]),
+    multiple=True,
+)
+@click.option(
+    "--no-grid",
+    help="Do not display as grid and print as results are available, useful when the cluster list is large",
+    is_flag=True,
+    default=False,
+)
+@click_config_file.configuration_option(settings.OPTION_FILE_FLAG)
+@click.pass_obj
+def list_emr_clusters(
+    ctx: Dict,
+    aws_profile: Optional[str] = None,
+    aws_region: Optional[str] = None,
+    only_log_locations: Optional[bool] = False,
+    created_after: Optional[str] = None,
+    state: Optional[List] = None,
+    no_grid: Optional[bool] = False,
+) -> None:
+    CloudResourceService(
+        config=ctx["config"],
+        aws_profile_override=aws_profile,
+        aws_region_override=aws_region,
+    ).list_emr_clusters(
+        only_log_locations=only_log_locations,
+        created_after=created_after,
+        states=state,
+        no_grid=no_grid,
+    )
+
+
+@discovery.command(
+    help="Alpha network recommender. Attempts to analyze and makes recommendations on how to connect a "
+    "resource with the Data Collector."
+)
+@click.pass_obj
+@click.option(
+    "--resource-identifier",
+    required=True,
+    help="Identifier for the AWS resource you want to connect the Collector with (e.g. Redshift cluster ID).",
+)
+@click.option(
+    "--resource-type",
+    required=True,
+    help="Type of AWS resource.",
+    type=click.Choice(NetworkDiscoveryService.MCD_NETWORK_REC_RESOURCE_TYPE_MAP.keys()),
+)
+@click.option(
+    "--collector-aws-profile",
+    required=True,
+    help="AWS profile for the Collector.",
+)
+@add_common_options(DC_RESOURCE_OPTIONS)
+@add_common_options(DISAMBIGUATE_DC_OPTIONS)
+@click_config_file.configuration_option(settings.OPTION_FILE_FLAG)
+def network_recommender(ctx, **kwargs):
+    NetworkDiscoveryService(
+        config=ctx["config"], aws_wrapper=None
+    ).recommend_network_dispatcher(**kwargs)
+
+
+@discovery.command(
+    help="Generate a CloudFormation template to create a resource access IAM role. "
+    "After review, this template can be deployed using CloudFormation. "
+    "The Role ARN and External ID for onboarding can be found in the stack outputs."
+)
+@click.pass_obj
+@click.option(
+    "--policy-file",
+    "policy_files",
+    required=True,
+    multiple=True,
+    type=click.File(),
+    help="File containing an IAM policy to generate an IAM role from. This option can be passed "
+    "multiple times for more than one policy.",
+)
+@add_common_options(DISAMBIGUATE_DC_OPTIONS)
+def cf_role_gen(ctx, **kwargs):
+    PolicyDiscoveryService(config=ctx["config"], aws_wrapper=None).generate_cf_role(
+        **kwargs
+    )
+
+
+@discovery.command(
+    help=f"Generate an IAM policy for Glue. {DISCOVERY_REVIEW_VERBIAGE}."
+)
+@click.pass_obj
+@add_common_options(GLUE_COMMON_OPTIONS)
+@add_common_options(DC_RESOURCE_OPTIONS)
+@add_common_options(DISAMBIGUATE_DC_OPTIONS)
+def glue_policy_gen(ctx, **kwargs):
+    PolicyDiscoveryService(config=ctx["config"], aws_wrapper=None).generate_glue_policy(
+        **kwargs
+    )
+
+
+@discovery.command(help=f"Generate an IAM policy for MSK. {DISCOVERY_REVIEW_VERBIAGE}.")
+@click.pass_obj
+@add_common_options(DC_RESOURCE_OPTIONS)
+@add_common_options(DISAMBIGUATE_DC_OPTIONS)
+def msk_policy_gen(ctx, **kwargs):
+    PolicyDiscoveryService(config=ctx["config"], aws_wrapper=None).generate_msk_policy(
+        **kwargs
+    )
+
+
+@discovery.command(
+    help=f"Generate an IAM policy for Athena. {DISCOVERY_REVIEW_VERBIAGE}."
+)
+@click.pass_obj
+@add_common_options(GLUE_COMMON_OPTIONS)
+@click.option(
+    "--workgroup-name",
+    required=True,
+    default="primary",
+    show_default=True,
+    help="Athena workgroup for Monte Carlo to use when performing queries. "
+    'The "primary" workgroup for the region is used if one is not specified.',
+)
+@add_common_options(DC_RESOURCE_OPTIONS)
+@add_common_options(DISAMBIGUATE_DC_OPTIONS)
+def athena_policy_gen(ctx, **kwargs):
+    PolicyDiscoveryService(
+        config=ctx["config"], aws_wrapper=None
+    ).generate_athena_policy(**kwargs)
```

### Comparing `montecarlodata-0.9.2/montecarlodata/iac/schemas.py` & `montecarlodata-0.90.0/montecarlodata/iac/schemas.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,53 +3,82 @@
 from typing import List, Optional
 
 from dataclasses_json import LetterCase
 from dataclasses_json import dataclass_json
 from marshmallow import fields
 
 from montecarlodata.iac.utils import field_spec
-from montecarlodata.settings import DEFAULT_MONTECARLO_MONITOR_CONFIG_VERSION, DEFAULT_INCLUDE_PATTERNS, DEFAULT_EXCLUDE_PATTERNS
+from montecarlodata.settings import (
+    DEFAULT_MONTECARLO_MONITOR_CONFIG_VERSION,
+    DEFAULT_INCLUDE_PATTERNS,
+    DEFAULT_EXCLUDE_PATTERNS,
+)
 
 
 @dataclass_json
 @dataclass
 class ProjectConfig:
-    version: Optional[int] = field_spec(fields.Int(required=False), default_factory=lambda: DEFAULT_MONTECARLO_MONITOR_CONFIG_VERSION)
+    version: Optional[int] = field_spec(
+        fields.Int(required=False),
+        default_factory=lambda: DEFAULT_MONTECARLO_MONITOR_CONFIG_VERSION,
+    )
     default_resource: Optional[str] = field_spec(fields.Str(required=False))
     include_file_patterns: Optional[List[str]] = field_spec(
         fields.List(fields.Str(required=True)),
-        default_factory=lambda: DEFAULT_INCLUDE_PATTERNS)
+        default_factory=lambda: DEFAULT_INCLUDE_PATTERNS,
+    )
     exclude_file_patterns: Optional[List[str]] = field_spec(
-        fields.List(fields.Str(required=True)),
-        default_factory=list)
+        fields.List(fields.Str(required=True)), default_factory=list
+    )
+    namespace: Optional[str] = None
 
     def __post_init__(self):
-        self.exclude_file_patterns = list(set(self.exclude_file_patterns + DEFAULT_EXCLUDE_PATTERNS))
+        self.exclude_file_patterns = list(
+            set(self.exclude_file_patterns + DEFAULT_EXCLUDE_PATTERNS)
+        )
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
 class ResourceModification:
     type: str
     description: str
-    resource_as_json: str
+    is_significant_change: bool = False
+    diff_string: Optional[str] = None
+    resource_type: Optional[str] = None
+    resource_index: Optional[int] = None
+
+
+@dataclass_json(letter_case=LetterCase.CAMEL)
+@dataclass
+class ConfigTemplateUpdateAsyncResponse:
+    update_uuid: Optional[str] = None
+    errors_as_json: Optional[str] = None
+    warnings_as_json: Optional[str] = None
 
     def __post_init__(self):
-        self.resource = json.loads(self.resource_as_json)
+        self.errors = json.loads(self.errors_as_json) if self.errors_as_json else {}
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
-class ConfigTemplateUpdateResponse:
-    resource_modifications: List[ResourceModification]
+class ConfigTemplateUpdateState:
+    state: str
+    resource_modifications: Optional[List[ResourceModification]] = None
     errors_as_json: Optional[str] = None
+    warnings_as_json: Optional[str] = None
     changes_applied: bool = False
 
     def __post_init__(self):
-        self.errors = json.loads(self.errors_as_json)
+        self.resource_modifications = self.resource_modifications or []
+        self.errors = json.loads(self.errors_as_json) if self.errors_as_json else {}
+
+    @property
+    def warnings(self):
+        return json.loads(self.warnings_as_json) if self.warnings_as_json else {}
 
 
 @dataclass_json(letter_case=LetterCase.CAMEL)
 @dataclass
 class ConfigTemplateDeleteResponse:
     num_deleted: int
-    changes_applied: bool = False
+    changes_applied: bool = False
```

### Comparing `montecarlodata-0.9.2/montecarlodata/iac/utils.py` & `montecarlodata-0.90.0/montecarlodata/iac/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import contextlib
 from dataclasses import field
-from typing import Dict
+from typing import Dict, Any
 
 from box import Box
 from dataclasses_json import config
 
 
 def field_spec(mm_field, default_factory=None, encoder=None, decoder=None):
     """
     dataclasses-json allows configuring a Marshmallow field which will be used for schema validation.
     See https://github.com/lidatong/dataclasses-json#overriding--extending
     Syntax involves a lot of boilerplate, so trying to minimize by using this function.
     """
-    f = field(metadata=config(
-        mm_field=mm_field,
-        encoder=encoder,
-        decoder=decoder
-    ))
+    f = field(metadata=config(mm_field=mm_field, encoder=encoder, decoder=decoder))
 
     # The following makes all of our dataclass fields optional.
     # We are enforcing required fields using marshmallow validators, so let's simplify and make
     # all the dataclass fields optional.
     if default_factory:
         f.default_factory = default_factory
     else:
         f.default = None
 
     return f
 
+
 def is_dbt_schema(yaml_as_dict: Box) -> bool:
     with contextlib.suppress(KeyError):
         return isinstance(yaml_as_dict.models, list)
     return False
 
-def has_montecarlo_property(yaml_as_dict: Dict) -> bool:
-    return 'montecarlo' in yaml_as_dict
+
+def has_montecarlo_property(yaml_as_dict: Dict[str, Any]) -> bool:
+    return "montecarlo" in yaml_as_dict
+
+
+def has_namespace_property(yaml_as_dict: Dict[str, Any]) -> bool:
+    return "namespace" in yaml_as_dict
```

### Comparing `montecarlodata-0.9.2/montecarlodata/integrations/info/status.py` & `montecarlodata-0.90.0/montecarlodata/integrations/info/status.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,40 +7,73 @@
 from montecarlodata.common.user import UserService
 from montecarlodata.config import Config
 from montecarlodata.errors import manage_errors
 from montecarlodata.integrations.onboarding.fields import GQL_TO_FRIENDLY_CONNECTION_MAP
 
 
 class OnboardingStatusService:
-    _INTEGRATION_FRIENDLY_HEADERS = ['Integration', 'ID', 'Created on (UTC)']
+    _INTEGRATION_FRIENDLY_HEADERS = [
+        "Integration",
+        "Name",
+        "ID",
+        "Connection",
+        "Created on (UTC)",
+    ]
 
     def __init__(self, config: Config, user_service: Optional[UserService] = None):
         self._abort_on_error = True
         self._user_service = user_service or UserService(config=config)
 
     @manage_errors
-    def display_integrations(self, headers: Optional[str] = 'firstrow', table_format: Optional[str] = 'fancy_grid'):
+    def display_integrations(
+        self,
+        headers: Optional[str] = "firstrow",
+        table_format: Optional[str] = "fancy_grid",
+    ):
         """
         Display active integrations in an easy to read table. E.g.
-        ╒══════════════════╤══════════════════════════════════════╤══════════════════════════════════╕
-        │ Integration      │ ID                                   │ Created on (UTC)                 │
-        ╞══════════════════╪══════════════════════════════════════╪══════════════════════════════════╡
-        │ Hive (metastore) │ 1023721b-e639-44ed-9838-e1f669d3fc85 │ 2020-05-09T01:49:52.806602+00:00 │
-        ╘══════════════════╧══════════════════════════════════════╧══════════════════════════════════╛
+        ╒═══════════════════╤═══════════╤══════════════════════════════════════╤═════════════════════════════╤══════════════════════════════════╕
+        │ Integration       │ Name      │ ID                                   │ Connection                  │ Created on (UTC)                 │
+        ╞═══════════════════╪═══════════╪══════════════════════════════════════╪═════════════════════════════╪══════════════════════════════════╡
+        │ Snowflake         │ rick_test │ 9403e385-1a56-4c3b-b185-4f2bb8e324d3 │ account: hda34492.us-east-1 │ 2022-03-25T19:55:11.858022+00:00 │
+        ╘═══════════════════╧═══════════╧══════════════════════════════════════╧═════════════════════════════╧══════════════════════════════════╛
         """
         table = [self._INTEGRATION_FRIENDLY_HEADERS]
-        for integration in (self._user_service.warehouses or [{}]) + (self._user_service.bi_containers or [{}]):
-            table += self._build_table_record(connections=integration.get('connections'))
+        for integration in (
+            (self._user_service.warehouses or [{}])
+            + (self._user_service.bi_containers or [{}])
+            + (self._user_service.etl_containers or [{}])
+        ):
+            table += self._build_table_record(
+                name=integration.get("name"), connections=integration.get("connections")
+            )
         click.echo(tabulate(table, headers=headers, tablefmt=table_format))
 
-    @staticmethod
-    def _build_table_record(connections: List[Dict]) -> List[List[str]]:
+    def _build_table_record(
+        self, name: str, connections: List[Dict]
+    ) -> List[List[str]]:
         table = []
         for connection in connections or []:
             table.append(
                 [
-                    GQL_TO_FRIENDLY_CONNECTION_MAP.get(normalize_gql(connection['type']), connection['type']),
-                    connection['uuid'],
-                    connection['createdOn']
+                    GQL_TO_FRIENDLY_CONNECTION_MAP.get(
+                        normalize_gql(connection["type"]), connection["type"]
+                    ),
+                    name,
+                    connection["uuid"],
+                    self._build_connection_info(connection),
+                    connection["createdOn"],
                 ]
             )  # order by the friendly headers, defaulting to gql response if not found
         return table
+
+    @staticmethod
+    def _build_connection_info(connection: Dict) -> Optional[str]:
+        identifiers = connection.get("connectionIdentifiers")
+        if not identifiers:
+            return None
+        connection_info = []
+        for identifier in identifiers:
+            key = identifier.get("key")
+            value = identifier.get("value")
+            connection_info.append(f"{key}: {value}")
+        return "\n".join(connection_info)
```

### Comparing `montecarlodata-0.9.2/montecarlodata/integrations/onboarding/base.py` & `montecarlodata-0.90.0/montecarlodata/integrations/onboarding/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,190 +1,352 @@
 import json
 import os
-from typing import Optional, Dict, List
+from typing import Optional, Dict
 
 import click
 from tabulate import tabulate
 
-from montecarlodata.common.data import ConnectionOptions, ValidationResult, OnboardingConfiguration
-from montecarlodata.common.common import normalize_gql
+from montecarlodata.common.data import (
+    ConnectionOptions,
+    ValidationResult,
+    OnboardingConfiguration,
+)
 from montecarlodata.common.user import UserService
 from montecarlodata.config import Config
 from montecarlodata.errors import complain_and_abort, prompt_connection
-from montecarlodata.integrations.onboarding.fields import S3_CERT_MECHANISM, GQL_TO_FRIENDLY_CONNECTION_MAP, \
-    DATA_LAKE_WAREHOUSE_TYPE, EXPECTED_ADD_CONNECTION_RESPONSE_FIELD, CONFIRM_CONNECTION_VERBIAGE, VALIDATIONS_FAILED_VERBIAGE, \
-    SKIP_ADD_CONNECTION_VERBIAGE, CONNECTION_TEST_SUCCESS_VERBIAGE, CONNECTION_TEST_FAILED_VERBIAGE, \
-    ADD_CONNECTION_FAILED_VERBIAGE, ADD_CONNECTION_SUCCESS_VERBIAGE
+from montecarlodata.integrations.onboarding.fields import (
+    S3_CERT_MECHANISM,
+    GQL_TO_FRIENDLY_CONNECTION_MAP,
+    DATA_LAKE_WAREHOUSE_TYPE,
+    EXPECTED_ADD_CONNECTION_RESPONSE_FIELD,
+    CONFIRM_CONNECTION_VERBIAGE,
+    VALIDATIONS_FAILED_VERBIAGE,
+    SKIP_ADD_CONNECTION_VERBIAGE,
+    CONNECTION_TEST_SUCCESS_VERBIAGE,
+    CONNECTION_TEST_FAILED_VERBIAGE,
+    ADD_CONNECTION_FAILED_VERBIAGE,
+    ADD_CONNECTION_SUCCESS_VERBIAGE,
+    MAIN_CONNECTION_TYPES,
+)
 from montecarlodata.queries.onboarding import ADD_CONNECTION_MUTATION
 from montecarlodata.utils import GqlWrapper, AwsClientWrapper
 
 
 class BaseOnboardingService:
-    _VALIDATION_STATUS_HEADERS = ['Validation', 'Result', 'Details']
-    _VALIDATION_PASSED = 'Passed'
-    _VALIDATION_FAILED = 'Failed'
-
-    def __init__(self, config: Config, user_service: Optional[UserService] = None,
-                 request_wrapper: Optional[GqlWrapper] = None,
-                 aws_wrapper: Optional[AwsClientWrapper] = None):
-
+    _VALIDATION_STATUS_HEADERS = ["Validation", "Result", "Details"]
+    _VALIDATION_PASSED = "Passed"
+    _VALIDATION_FAILED = "Failed"
+    _ETL_CONNECTION_TYPES = ["fivetran", "airflow"]
+
+    def __init__(
+        self,
+        config: Config,
+        user_service: Optional[UserService] = None,
+        request_wrapper: Optional[GqlWrapper] = None,
+        aws_wrapper: Optional[AwsClientWrapper] = None,
+    ):
         self._abort_on_error = True  # Aborts methods with deco on unhandled error
         self._dc_outputs = None
 
         self._user_service = user_service or UserService(config=config)
-        self._request_wrapper = request_wrapper or GqlWrapper(mcd_id=config.mcd_id, mcd_token=config.mcd_token)
-        self._aws_wrapper = aws_wrapper or AwsClientWrapper(profile_name=config.aws_profile,
-                                                            region_name=config.aws_region)
+        self._request_wrapper = request_wrapper or GqlWrapper(config)
+        self._aws_wrapper = aws_wrapper
 
     def onboard(self, **kwargs):
         """
         Convenience wrapper to validate and add a connection.
         """
-        onboarding_config = OnboardingConfiguration(**kwargs)  # not passed as arg to avoid having to change all clients
-        onboarding_config.connection_options = self._build_connection_options(**onboarding_config.connection_options)
-
-        onboarding_config.warehouse_name = onboarding_config.connection_options.monolith_base_payload.pop('warehouseName', None)
-        onboarding_config.warehouse_type = onboarding_config.connection_options.monolith_base_payload.pop('warehouseType', DATA_LAKE_WAREHOUSE_TYPE)
+        onboarding_config = self._get_onboard_config(**kwargs)
 
         result = self._validate_connection(
             query=onboarding_config.validation_query,
             response_field=onboarding_config.validation_response,
-            **onboarding_config.connection_options.monolith_base_payload
+            **onboarding_config.connection_options.monolith_base_payload,
         )
 
         if not onboarding_config.connection_options.validate_only:
-            prompt = VALIDATIONS_FAILED_VERBIAGE if result.has_warnings else CONFIRM_CONNECTION_VERBIAGE
-            prompt_connection(message=prompt, skip_prompt=onboarding_config.connection_options.auto_yes)
-            self._add_connection(temp_path=result.credentials_key, onboarding_config=onboarding_config)
+            prompt = (
+                VALIDATIONS_FAILED_VERBIAGE
+                if result.has_warnings
+                else CONFIRM_CONNECTION_VERBIAGE
+            )
+            prompt_connection(
+                message=prompt,
+                skip_prompt=onboarding_config.connection_options.auto_yes,
+            )
+            self._add_connection(
+                temp_path=result.credentials_key, onboarding_config=onboarding_config
+            )
         else:
             click.echo(SKIP_ADD_CONNECTION_VERBIAGE)
 
+    def add_connection(self, key: str, **kwargs):
+        onboarding_config = self._get_onboard_config(**kwargs)
+        self._add_connection(temp_path=key, onboarding_config=onboarding_config)
+
     def handle_cert(self, cert_prefix: str, options: Dict) -> None:
         """
         Handles cert payload from either an s3 path or file. Uploading the latter
         Options is updated if successful.
         """
-        if options.get('cert_file') is not None:
-            bucket_name = self._get_dc_property(prop='PrivateS3BucketArn').split(':')[5]  # get name from arn
-            object_name = os.path.join(cert_prefix, os.path.basename(options['cert_file']))
-            self._aws_wrapper.upload_file(bucket_name=bucket_name, object_name=object_name,
-                                          file_path=options['cert_file'])
+        active_agent = self._user_service.get_collector_agent(options.get("dc_id"))
+        if options.get("cert_file") is not None:
+            if active_agent:
+                complain_and_abort("cert_file option is not supported for agents.")
+
+            self._aws_wrapper = self._aws_wrapper or AwsClientWrapper(
+                profile_name=options.get("aws_profile"),
+                region_name=options.get("aws_region"),
+            )
+            # get bucket name from arn
+            bucket_name = self._get_dc_property(prop="PrivateS3BucketArn").split(":")[5]
+            object_name = os.path.join(
+                cert_prefix, os.path.basename(options["cert_file"])
+            )
+            self._aws_wrapper.upload_file(
+                bucket_name=bucket_name,
+                object_name=object_name,
+                file_path=options["cert_file"],
+            )
 
-            click.echo(f"Uploaded '{options['cert_file']}' to s3://{bucket_name}/{object_name}")
-            options['cert_s3'] = object_name
+            click.echo(
+                f"Uploaded '{options['cert_file']}' to s3://{bucket_name}/{object_name}"
+            )
+            options["cert_s3"] = object_name
 
-        if options.get('cert_s3') is not None:
+        ssl_options = {}
+        if options.get("cert_s3") is not None:
             # reformat to generic options and specify a mechanism
-            options['ssl_options'] = {'mechanism': S3_CERT_MECHANISM, 'cert': options.pop('cert_s3')}
-        options.pop('cert_file', None)
-
-    def _validate_connection(self, query: str, response_field: str, **kwargs) -> ValidationResult:
+            ssl_options = {
+                "mechanism": S3_CERT_MECHANISM,
+                "cert": options.pop("cert_s3"),
+            }
+        options.pop("cert_file", None)
+
+        if options.get("skip_cert_verification") is not None:
+            ssl_options["skip_verification"] = options.pop("skip_cert_verification")
+
+        if ssl_options:
+            options["ssl_options"] = ssl_options
+
+    def _validate_connection(
+        self, query: str, response_field: str, **kwargs
+    ) -> ValidationResult:
         """
         Validate connection before adding using the expected gql response_field (e.g. testPrestoCredentials)
         """
         response = self._request_wrapper.make_request_v2(
-            query=query,
-            operation=response_field,
-            variables=kwargs
+            query=query, operation=response_field, variables=kwargs
         )
 
         summary = self._build_validation_summary(response.data)
-        temp_path = response.data.get('key')
-        warnings = response.data.get('warnings')
+        temp_path = response.data.get("key")
+        warnings = response.data.get("warnings")
 
         if temp_path is not None:
-            click.echo(f'{CONNECTION_TEST_SUCCESS_VERBIAGE}{summary}')
+            click.echo(f"{CONNECTION_TEST_SUCCESS_VERBIAGE}{summary}")
             return ValidationResult(
                 has_warnings=warnings is not None and len(warnings) > 0,
-                credentials_key=temp_path
+                credentials_key=temp_path,
             )
 
-        complain_and_abort(f'{CONNECTION_TEST_FAILED_VERBIAGE}{summary}')
+        complain_and_abort(f"{CONNECTION_TEST_FAILED_VERBIAGE}{summary}")
 
-    def _build_validation_summary(self, response: Dict, table_format: Optional[str] = 'fancy_grid') -> str:
+    def _build_validation_summary(
+        self, response: Dict, table_format: Optional[str] = "fancy_grid"
+    ) -> str:
         data = []
-        if response.get('validations'):
-            for passed in response.get('validations'):
-                data.append([
-                    passed.get('message'),
-                    self._VALIDATION_PASSED,
-                    None
-                ])
-
-        if response.get('warnings'):
-            for failed in response.get('warnings', []):
-                data.append([
-                    failed.get('message'),
-                    self._VALIDATION_FAILED,
-                    failed.get('data', {}).get('error')
-                ])
+        if response.get("validations"):
+            for passed in response.get("validations"):
+                data.append([passed.get("message"), self._VALIDATION_PASSED, None])
+
+        if response.get("warnings"):
+            for failed in response.get("warnings", []):
+                data.append(
+                    [
+                        failed.get("message"),
+                        self._VALIDATION_FAILED,
+                        failed.get("data", {}).get("error"),
+                    ]
+                )
 
         if data:
-            return '\n' + tabulate(data, headers=self._VALIDATION_STATUS_HEADERS, tablefmt=table_format)
+            return "\n" + tabulate(
+                data, headers=self._VALIDATION_STATUS_HEADERS, tablefmt=table_format
+            )
 
         # do not provide a summary if no detailed response is available
-        return ''
+        return ""
 
-    def _add_connection(self, temp_path: str, onboarding_config: OnboardingConfiguration) -> bool:
+    def _add_connection(
+        self, temp_path: str, onboarding_config: OnboardingConfiguration
+    ) -> bool:
         """
         Add connection and setup any associated jobs
         """
-        warehouse_type = onboarding_config.warehouse_type or DATA_LAKE_WAREHOUSE_TYPE  # default to data-lake
-        connection_request = {'key': temp_path, 'connectionType': onboarding_config.connection_type}
-        connection_request.update(self._disambiguate_warehouses(warehouse_type))
+        connection_request = {
+            "key": temp_path,
+            "connectionType": onboarding_config.connection_type,
+        }
+
+        connection_request.update(self._disambiguate_warehouses(onboarding_config))
 
         # Set optional properties
         if onboarding_config.warehouse_name:
-            connection_request['name'] = onboarding_config.warehouse_name
+            connection_request["name"] = onboarding_config.warehouse_name
         if onboarding_config.job_types:
-            connection_request['jobTypes'] = onboarding_config.job_types
+            connection_request["jobTypes"] = onboarding_config.job_types
         if onboarding_config.job_limits:
-            connection_request['jobLimits'] = json.dumps(onboarding_config.job_limits)
-        if onboarding_config.connection_options and onboarding_config.connection_options.dc_id:
-            connection_request['dcId'] = onboarding_config.connection_options.dc_id
+            connection_request["jobLimits"] = json.dumps(onboarding_config.job_limits)
+        if (
+            onboarding_config.connection_options
+            and onboarding_config.connection_options.dc_id
+        ):
+            connection_request["dcId"] = onboarding_config.connection_options.dc_id
 
         response = self._request_wrapper.make_request_v2(
             query=onboarding_config.connection_query or ADD_CONNECTION_MUTATION,
-            operation=onboarding_config.connection_response or EXPECTED_ADD_CONNECTION_RESPONSE_FIELD,
+            operation=onboarding_config.connection_response
+            or EXPECTED_ADD_CONNECTION_RESPONSE_FIELD,
             variables=connection_request,
         )
-        connection_id = response.data.get('connection', {}).get('uuid')
+
+        connection_id = response.data.get("connection", {}).get("uuid")
         if connection_id is not None:
-            click.echo(f"{ADD_CONNECTION_SUCCESS_VERBIAGE}"
-                       f"{GQL_TO_FRIENDLY_CONNECTION_MAP.get(onboarding_config.connection_type, onboarding_config.connection_type.capitalize())}.")
+            click.echo(
+                f"{ADD_CONNECTION_SUCCESS_VERBIAGE}"
+                f"{GQL_TO_FRIENDLY_CONNECTION_MAP.get(onboarding_config.connection_type, onboarding_config.connection_type.capitalize())}."
+            )
             return True
         complain_and_abort(ADD_CONNECTION_FAILED_VERBIAGE)
 
-    def _disambiguate_warehouses(self, warehouse_type: str) -> Dict:
+    def _disambiguate_warehouses(
+        self, onboarding_config: OnboardingConfiguration
+    ) -> Dict:
         """
         Determine type of connection request to build using the following criteria -
-            1) Does an existing warehouse exist and is it a data-lake? If so, attach connection.
-            2) Otherwise, it is either the first connection or traditional warehouse (e.g. redshift, snowflake, etc.)
-
-        Multiple lakes are not supported.
+            1) If it is an ETL connection there should not be any warehouse set so we can skip this step
+            2) If it is a main connection type or a traditional warehouse (i.e. not a lake), create a new warehouse.
+            3) If a name has been passed, create the connection in that warehouse.
+            4) If no name has been passed but there is only one warehouse, use it.
+            5) Otherwise fail.
         """
-        if len(self._user_service.warehouses) > 0 and warehouse_type == DATA_LAKE_WAREHOUSE_TYPE:
-            for warehouse in self._user_service.warehouses:
-                if normalize_gql(warehouse['connectionType']) == DATA_LAKE_WAREHOUSE_TYPE:
-                    return {'dwId': warehouse['uuid']}
-        return {'createWarehouseType': warehouse_type}
+        is_etl_connection = (
+            onboarding_config.connection_type in self._ETL_CONNECTION_TYPES
+        )
+
+        if is_etl_connection:
+            return {}
+
+        warehouse_type = (
+            onboarding_config.warehouse_type or DATA_LAKE_WAREHOUSE_TYPE
+        )  # default to data-lake
+        connection_type = onboarding_config.connection_type
+        create_warehouse = onboarding_config.create_warehouse
+
+        # Main connections require the creation of a new warehouse.
+        if (
+            connection_type in MAIN_CONNECTION_TYPES
+            or warehouse_type != DATA_LAKE_WAREHOUSE_TYPE
+        ) and create_warehouse:
+            return {"createWarehouseType": warehouse_type}
+
+        name = onboarding_config.warehouse_name
+
+        dw_id = self._get_warehouse_id_from_name(name)
+        return {"dwId": dw_id}
+
+    def _get_warehouse_id_from_name(self, name: Optional[str]) -> str:
+        warehouses = self._user_service.warehouses
+
+        # If it is not a new warehouse, find the warehouse with the given name to create the new connection belonging
+        # to it. If the name is not found, it is an error.
+        if name:
+            warehouses = [
+                warehouse for warehouse in warehouses if warehouse.get("name") == name
+            ]
+            if warehouses:
+                return warehouses[0]["uuid"]
+            complain_and_abort("Could not find warehouse with given name")
+        # Name is optional if there is only one warehouse.
+        elif len(warehouses) == 1:
+            return warehouses[0]["uuid"]
+        # If more than one warehouse exists, name is required.
+        else:
+            complain_and_abort("Name is required to disambiguate lake warehouses")
+
+    def _get_bi_container_id_from_connection_id(
+        self, bi_connection_id: Optional[str]
+    ) -> str:
+        """
+        Exchange a Connection UUID for the parent BI Container's UUID
+        """
+        bi_containers = self._user_service.bi_containers
+        for bi_container in bi_containers:
+            connections = bi_container.get("connections")
+            for connection in connections:
+                if connection["uuid"] == bi_connection_id:
+                    return bi_container["uuid"]
+        complain_and_abort("Could not find BI container with given connection ID")
 
     def _get_dc_property(self, prop: str) -> Optional[str]:
         """
         Retrieve property from DC stack outputs
         """
         self._dc_outputs = self._dc_outputs or self._aws_wrapper.get_stack_outputs(
-            self._user_service.active_collector['stackArn'])  # cache lookup
+            self._user_service.active_collector["stackArn"]
+        )  # cache lookup
         for output in self._dc_outputs:
-            if output['OutputKey'] == prop:
-                return output['OutputValue']
+            if output["OutputKey"] == prop:
+                return output["OutputValue"]
 
     @staticmethod
     def _build_connection_options(**kwargs) -> ConnectionOptions:
         """
         Create connection options from arguments
         """
         connection_options = ConnectionOptions(**kwargs)
 
         if connection_options.monolith_connection_payload:
-            connection_options.monolith_base_payload['connectionOptions'] = connection_options.monolith_connection_payload
+            connection_options.monolith_base_payload["connectionOptions"] = (
+                connection_options.monolith_connection_payload
+            )
         return connection_options
+
+    def _get_onboard_config(self, **kwargs) -> OnboardingConfiguration:
+        agent_id = kwargs.get("agent_id")
+        if agent_id:
+            agent = self._user_service.get_agent(agent_id)
+            kwargs["dc_id"] = agent["dc_id"]
+        onboarding_config = OnboardingConfiguration(
+            **kwargs
+        )  # not passed as arg to avoid having to change all clients
+
+        is_etl_connection = (
+            onboarding_config.connection_type in self._ETL_CONNECTION_TYPES
+        )
+
+        onboarding_config.connection_options = self._build_connection_options(
+            **onboarding_config.connection_options
+        )
+
+        if is_etl_connection:
+            onboarding_config.warehouse_name = (
+                onboarding_config.connection_options.monolith_base_payload.pop(
+                    "etl_name", onboarding_config.warehouse_name
+                )
+            )
+        else:
+            onboarding_config.warehouse_name = (
+                onboarding_config.connection_options.monolith_base_payload.pop(
+                    "warehouseName", onboarding_config.connection_type
+                )
+            )
+        # Prefer explicitly set types.
+        if not onboarding_config.warehouse_type and not is_etl_connection:
+            onboarding_config.warehouse_type = (
+                onboarding_config.connection_options.monolith_base_payload.pop(
+                    "warehouseType", DATA_LAKE_WAREHOUSE_TYPE
+                )
+            )
+
+        return onboarding_config
```

### Comparing `montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/events.py` & `montecarlodata-0.90.0/montecarlodata/integrations/onboarding/vector/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,58 @@
-from typing import Optional
+from copy import deepcopy
 
 import click
 
+from pycarlo.core import Client
+
+from montecarlodata.collector.validation import CollectorValidationService
 from montecarlodata.config import Config
-from montecarlodata.errors import complain_and_abort, manage_errors
+from montecarlodata.errors import manage_errors
 from montecarlodata.integrations.onboarding.base import BaseOnboardingService
-from montecarlodata.integrations.onboarding.fields import EXPECTED_TOGGLE_EVENTS_GQL_RESPONSE_FIELD
-from montecarlodata.queries.onboarding import TOGGLE_EVENT_MUTATION
-
+from montecarlodata.integrations.onboarding.fields import (
+    EXPECTED_ADD_CONNECTION_RESPONSE_FIELD,
+    PINECONE_CONNECTION_TYPE,
+    PINECONE_WAREHOUSE_TYPE,
+)
+from montecarlodata.queries.onboarding import (
+    ADD_CONNECTION_MUTATION,
+)
 
-class EventsOnboardingService(BaseOnboardingService):
 
-    def __init__(self, config: Config, **kwargs):
+class VectorDbOnboardingService(BaseOnboardingService):
+    def __init__(self, config: Config, mc_client: Client, **kwargs):
         super().__init__(config, **kwargs)
+        self._validation_service = CollectorValidationService(
+            config=config,
+            mc_client=mc_client,
+            user_service=self._user_service,
+            request_wrapper=self._request_wrapper,
+        )
 
     @manage_errors
-    def toggle_event_configuration(self, **kwargs) -> Optional[bool]:
-        """
-        Toggle event configuration (effectively onboarding it if enable is set to true)
-        """
-        num_of_warehouses = len(self._user_service.warehouses)
-
-        if num_of_warehouses == 1:
-            kwargs['dwId'] = self._user_service.warehouses[0]['uuid']
-            variables = self._request_wrapper.convert_snakes_to_camels(kwargs)
-            status = self._request_wrapper.make_request(query=TOGGLE_EVENT_MUTATION, variables=variables).get(
-                EXPECTED_TOGGLE_EVENTS_GQL_RESPONSE_FIELD, {}).get('success')
-            if status:
-                click.echo(f"Success! {'Enabled' if kwargs['enable'] else 'Disabled'} events.")
-                return True
-            complain_and_abort('Failed to toggle events!')
-        complain_and_abort(f'Events only supports one warehouse. Found {num_of_warehouses}')
+    def onboard_pinecone(self, **kwargs) -> None:
+        credentials_key = self._validation_service.test_new_credentials(
+            connection_type=PINECONE_CONNECTION_TYPE,
+            **kwargs,
+        )
+
+        environment = kwargs.get("environment")
+        project_id = kwargs.get("project_id")
+        name = kwargs.get("name") or f"{environment}:{project_id}"
+
+        variables = {
+            "connection_type": PINECONE_CONNECTION_TYPE,
+            "create_warehouse_type": PINECONE_WAREHOUSE_TYPE,
+            "dc_id": kwargs.get("dc_id"),
+            "key": credentials_key,
+            "name": name,
+        }
+
+        response = self._request_wrapper.make_request_v2(
+            query=ADD_CONNECTION_MUTATION,
+            operation=EXPECTED_ADD_CONNECTION_RESPONSE_FIELD,
+            variables=variables,
+        )
+
+        click.echo(
+            f"Successfully created connection (id={response.data.connection.uuid})"
+        )
```

### Comparing `montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/glue_athena.py` & `montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/glue_athena.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 from montecarlodata.config import Config
 from montecarlodata.errors import manage_errors
 from montecarlodata.integrations.onboarding.base import BaseOnboardingService
-from montecarlodata.integrations.onboarding.fields import EXPECTED_GLUE_GQL_RESPONSE_FIELD, \
-    EXPECTED_ATHENA_GQL_RESPONSE_FIELD, GLUE_CONNECTION_TYPE, ATHENA_CONNECTION_TYPE
-from montecarlodata.queries.onboarding import TEST_GLUE_CRED_MUTATION, TEST_ATHENA_CRED_MUTATION
+from montecarlodata.integrations.onboarding.fields import (
+    EXPECTED_GLUE_GQL_RESPONSE_FIELD,
+    EXPECTED_ATHENA_GQL_RESPONSE_FIELD,
+    GLUE_CONNECTION_TYPE,
+    ATHENA_CONNECTION_TYPE,
+)
+from montecarlodata.queries.onboarding import (
+    TEST_GLUE_CRED_MUTATION,
+    TEST_ATHENA_CRED_MUTATION,
+)
 
 
 class GlueAthenaOnboardingService(BaseOnboardingService):
-
     def __init__(self, config: Config, **kwargs):
         super().__init__(config, **kwargs)
 
     @manage_errors
     def onboard_glue(self, **kwargs) -> None:
         """
         Onboard a glue connection by validating and adding a connection
         """
-        self.onboard(validation_query=TEST_GLUE_CRED_MUTATION,
-                     validation_response=EXPECTED_GLUE_GQL_RESPONSE_FIELD,
-                     connection_type=GLUE_CONNECTION_TYPE, **kwargs)
+        self.onboard(
+            validation_query=TEST_GLUE_CRED_MUTATION,
+            validation_response=EXPECTED_GLUE_GQL_RESPONSE_FIELD,
+            connection_type=GLUE_CONNECTION_TYPE,
+            **kwargs
+        )
 
     @manage_errors
     def onboard_athena(self, **kwargs) -> None:
         """
         Onboard an athena connection by validating and adding a connection
         """
-        self.onboard(validation_query=TEST_ATHENA_CRED_MUTATION,
-                     validation_response=EXPECTED_ATHENA_GQL_RESPONSE_FIELD,
-                     connection_type=ATHENA_CONNECTION_TYPE, **kwargs)
+        self.onboard(
+            validation_query=TEST_ATHENA_CRED_MUTATION,
+            validation_response=EXPECTED_ATHENA_GQL_RESPONSE_FIELD,
+            connection_type=ATHENA_CONNECTION_TYPE,
+            **kwargs
+        )
```

### Comparing `montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/hive.py` & `montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/hive.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,80 @@
 from montecarlodata.config import Config
 from montecarlodata.errors import manage_errors
 from montecarlodata.integrations.onboarding.base import BaseOnboardingService
-from montecarlodata.integrations.onboarding.fields import EXPECTED_GENERIC_DB_GQL_RESPONSE_FIELD, \
-    EXPECTED_HIVE_S3_GQL_RESPONSE_FIELD, EXPECTED_HIVE_SQL_GQL_RESPONSE_FIELD, HIVE_MYSQL_CONNECTION_TYPE, \
-    HIVE_S3_CONNECTION_TYPE, HIVE_SQL_CONNECTION_TYPE, QL_JOB_TYPE, AWS_RDS_CA_CERT, PRESTO_CATALOG_KEY, \
-    HIVE_GET_PARTS_KEY, HIVE_MAX_PARTS_KEY, HIVE_MAX_PARTS_DEFAULT_VALUE
-from montecarlodata.queries.onboarding import TEST_DATABASE_CRED_MUTATION, TEST_S3_CRED_MUTATION, \
-    TEST_HIVE_SQL_CRED_MUTATION
+from montecarlodata.integrations.onboarding.fields import (
+    EXPECTED_GENERIC_DB_GQL_RESPONSE_FIELD,
+    EXPECTED_HIVE_S3_GQL_RESPONSE_FIELD,
+    EXPECTED_HIVE_SQL_GQL_RESPONSE_FIELD,
+    HIVE_MYSQL_CONNECTION_TYPE,
+    HIVE_S3_CONNECTION_TYPE,
+    HIVE_SQL_CONNECTION_TYPE,
+    QL_JOB_TYPE,
+    AWS_RDS_CA_CERT,
+    PRESTO_CATALOG_KEY,
+    HIVE_GET_PARTS_KEY,
+    HIVE_MAX_PARTS_KEY,
+    HIVE_MAX_PARTS_DEFAULT_VALUE,
+)
+from montecarlodata.queries.onboarding import (
+    TEST_DATABASE_CRED_MUTATION,
+    TEST_S3_CRED_MUTATION,
+    TEST_HIVE_SQL_CRED_MUTATION,
+)
 
 
 class HiveOnboardingService(BaseOnboardingService):
-
     def __init__(self, config: Config, **kwargs):
         super().__init__(config, **kwargs)
 
     @manage_errors
     def onboard_hive_mysql(self, **kwargs) -> None:
         """
         Onboard a hive-mysql connection by validating and adding a connection
         """
-        if kwargs['use_ssl']:
-            kwargs['ssl_options'] = {'ca': AWS_RDS_CA_CERT}
-            kwargs.pop('use_ssl')
-
-        catalog = kwargs.pop('catalog', None)
-        job_limits = {HIVE_GET_PARTS_KEY: True, HIVE_MAX_PARTS_KEY: HIVE_MAX_PARTS_DEFAULT_VALUE}
+        if kwargs["use_ssl"]:
+            kwargs["ssl_options"] = {"ca": AWS_RDS_CA_CERT}
+            kwargs.pop("use_ssl")
+
+        catalog = kwargs.pop("catalog", None)
+        job_limits = {
+            HIVE_GET_PARTS_KEY: True,
+            HIVE_MAX_PARTS_KEY: HIVE_MAX_PARTS_DEFAULT_VALUE,
+        }
 
         if catalog:
             job_limits[PRESTO_CATALOG_KEY] = catalog
 
-        kwargs['connectionType'] = HIVE_MYSQL_CONNECTION_TYPE
-        self.onboard(validation_query=TEST_DATABASE_CRED_MUTATION,
-                     validation_response=EXPECTED_GENERIC_DB_GQL_RESPONSE_FIELD,
-                     connection_type=HIVE_MYSQL_CONNECTION_TYPE, job_limits=job_limits, **kwargs)
+        kwargs["connectionType"] = HIVE_MYSQL_CONNECTION_TYPE
+        self.onboard(
+            validation_query=TEST_DATABASE_CRED_MUTATION,
+            validation_response=EXPECTED_GENERIC_DB_GQL_RESPONSE_FIELD,
+            connection_type=HIVE_MYSQL_CONNECTION_TYPE,
+            job_limits=job_limits,
+            **kwargs
+        )
 
     @manage_errors
     def onboard_hive_s3(self, **kwargs) -> None:
         """
         Onboard a presto-s3 connection by validating and adding a connection
         """
-        kwargs['connectionType'] = HIVE_S3_CONNECTION_TYPE
-        self.onboard(validation_query=TEST_S3_CRED_MUTATION,
-                     validation_response=EXPECTED_HIVE_S3_GQL_RESPONSE_FIELD,
-                     connection_type=HIVE_S3_CONNECTION_TYPE, job_types=QL_JOB_TYPE, **kwargs)
+        kwargs["connectionType"] = HIVE_S3_CONNECTION_TYPE
+        self.onboard(
+            validation_query=TEST_S3_CRED_MUTATION,
+            validation_response=EXPECTED_HIVE_S3_GQL_RESPONSE_FIELD,
+            connection_type=HIVE_S3_CONNECTION_TYPE,
+            job_types=QL_JOB_TYPE,
+            **kwargs
+        )
 
     @manage_errors
     def onboard_hive_sql(self, **kwargs) -> None:
         """
         Onboard a hive-sql connection by validating and adding a connection
         """
-        self.onboard(validation_query=TEST_HIVE_SQL_CRED_MUTATION,
-                     validation_response=EXPECTED_HIVE_SQL_GQL_RESPONSE_FIELD,
-                     connection_type=HIVE_SQL_CONNECTION_TYPE, **kwargs)
+        self.onboard(
+            validation_query=TEST_HIVE_SQL_CRED_MUTATION,
+            validation_response=EXPECTED_HIVE_SQL_GQL_RESPONSE_FIELD,
+            connection_type=HIVE_SQL_CONNECTION_TYPE,
+            **kwargs
+        )
```

### Comparing `montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/presto.py` & `montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/presto.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 from montecarlodata.config import Config
 from montecarlodata.errors import manage_errors
 from montecarlodata.integrations.onboarding.base import BaseOnboardingService
-from montecarlodata.integrations.onboarding.fields import EXPECTED_PRESTO_SQL_GQL_RESPONSE_FIELD, \
-    EXPECTED_PRESTO_S3_GQL_RESPONSE_FIELD, PRESTO_SQL_CONNECTION_TYPE, PRESTO_S3_CONNECTION_TYPE, QL_JOB_TYPE, \
-    PRESTO_CERT_PREFIX
-from montecarlodata.queries.onboarding import TEST_PRESTO_CRED_MUTATION, TEST_S3_CRED_MUTATION
+from montecarlodata.integrations.onboarding.fields import (
+    EXPECTED_PRESTO_SQL_GQL_RESPONSE_FIELD,
+    EXPECTED_PRESTO_S3_GQL_RESPONSE_FIELD,
+    PRESTO_SQL_CONNECTION_TYPE,
+    PRESTO_S3_CONNECTION_TYPE,
+    QL_JOB_TYPE,
+    PRESTO_CERT_PREFIX,
+)
+from montecarlodata.queries.onboarding import (
+    TEST_PRESTO_CRED_MUTATION,
+    TEST_S3_CRED_MUTATION,
+)
 
 
 class PrestoOnboardingService(BaseOnboardingService):
-
     def __init__(self, config: Config, **kwargs):
         super().__init__(config, **kwargs)
 
     @manage_errors
     def onboard_presto_sql(self, **kwargs) -> None:
         """
         Onboard a presto-sql connection by validating and adding a connection.
         Also, optionally uploads a certificate to the DC bucket.
         """
         self.handle_cert(cert_prefix=PRESTO_CERT_PREFIX, options=kwargs)
-        self.onboard(validation_query=TEST_PRESTO_CRED_MUTATION,
-                     validation_response=EXPECTED_PRESTO_SQL_GQL_RESPONSE_FIELD,
-                     connection_type=PRESTO_SQL_CONNECTION_TYPE, **kwargs)
+        self.onboard(
+            validation_query=TEST_PRESTO_CRED_MUTATION,
+            validation_response=EXPECTED_PRESTO_SQL_GQL_RESPONSE_FIELD,
+            connection_type=PRESTO_SQL_CONNECTION_TYPE,
+            **kwargs
+        )
 
     @manage_errors
     def onboard_presto_s3(self, **kwargs) -> None:
         """
         Onboard a presto-s3 connection by validating and adding a connection
         """
-        kwargs['connectionType'] = PRESTO_S3_CONNECTION_TYPE
-        self.onboard(validation_query=TEST_S3_CRED_MUTATION,
-                     validation_response=EXPECTED_PRESTO_S3_GQL_RESPONSE_FIELD,
-                     connection_type=PRESTO_S3_CONNECTION_TYPE, job_types=QL_JOB_TYPE, **kwargs)
+        kwargs["connectionType"] = PRESTO_S3_CONNECTION_TYPE
+        self.onboard(
+            validation_query=TEST_S3_CRED_MUTATION,
+            validation_response=EXPECTED_PRESTO_S3_GQL_RESPONSE_FIELD,
+            connection_type=PRESTO_S3_CONNECTION_TYPE,
+            job_types=QL_JOB_TYPE,
+            **kwargs
+        )
```

### Comparing `montecarlodata-0.9.2/montecarlodata/integrations/onboarding/data_lake/spark.py` & `montecarlodata-0.90.0/montecarlodata/integrations/onboarding/data_lake/spark.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 from montecarlodata.config import Config
 from montecarlodata.errors import manage_errors
 from montecarlodata.integrations.onboarding.base import BaseOnboardingService
-from montecarlodata.integrations.onboarding.fields import SPARK_CONNECTION_TYPE, EXPECTED_SPARK_GQL_RESPONSE_FIELD
-from montecarlodata.queries.onboarding import TEST_SPARK_BINARY_MODE_CRED_MUTATION, \
-    TEST_SPARK_HTTP_MODE_CRED_MUTATION, TEST_SPARK_DATABRICKS_CRED_MUTATION
-
-SPARK_BINARY_MODE_CONFIG_TYPE = 'binary'
-SPARK_HTTP_MODE_CONFIG_TYPE = 'http'
-SPARK_DATABRICKS_CONFIG_TYPE = 'databricks'
+from montecarlodata.integrations.onboarding.fields import (
+    SPARK_CONNECTION_TYPE,
+    EXPECTED_SPARK_GQL_RESPONSE_FIELD,
+)
+from montecarlodata.queries.onboarding import (
+    TEST_SPARK_BINARY_MODE_CRED_MUTATION,
+    TEST_SPARK_HTTP_MODE_CRED_MUTATION,
+    TEST_SPARK_DATABRICKS_CRED_MUTATION,
+)
+
+SPARK_BINARY_MODE_CONFIG_TYPE = "binary"
+SPARK_HTTP_MODE_CONFIG_TYPE = "http"
+SPARK_DATABRICKS_CONFIG_TYPE = "databricks"
 
 
 class SparkOnboardingService(BaseOnboardingService):
 
     _MUTATIONS = {
         SPARK_BINARY_MODE_CONFIG_TYPE: TEST_SPARK_BINARY_MODE_CRED_MUTATION,
         SPARK_HTTP_MODE_CONFIG_TYPE: TEST_SPARK_HTTP_MODE_CRED_MUTATION,
@@ -23,11 +29,14 @@
 
     @manage_errors
     def onboard_spark(self, config_type: str, **kwargs) -> None:
         """
         Onboard a spark connection by validating and adding a connection
         """
         validation_query = self._MUTATIONS[config_type]
-        kwargs['connectionType'] = SPARK_CONNECTION_TYPE
-        self.onboard(validation_query=validation_query,
-                     validation_response=EXPECTED_SPARK_GQL_RESPONSE_FIELD,
-                     connection_type=SPARK_CONNECTION_TYPE, **kwargs)
+        kwargs["connectionType"] = SPARK_CONNECTION_TYPE
+        self.onboard(
+            validation_query=validation_query,
+            validation_response=EXPECTED_SPARK_GQL_RESPONSE_FIELD,
+            connection_type=SPARK_CONNECTION_TYPE,
+            **kwargs
+        )
```

### Comparing `montecarlodata-0.9.2/montecarlodata/integrations/onboarding/warehouse/warehouses.py` & `montecarlodata-0.90.0/montecarlodata/integrations/onboarding/warehouse/warehouses.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,74 @@
 from montecarlodata.common.common import read_as_base64
 from montecarlodata.config import Config
 from montecarlodata.errors import manage_errors
 from montecarlodata.integrations.onboarding.base import BaseOnboardingService
-from montecarlodata.integrations.onboarding.fields import EXPECTED_GENERIC_DB_GQL_RESPONSE_FIELD, \
-    REDSHIFT_CONNECTION_TYPE, REDSHIFT_WAREHOUSE_TYPE, SNOWFLAKE_CONNECTION_TYPE, SNOWFLAKE_WAREHOUSE_TYPE, \
-    EXPECTED_SNOWFLAKE_GQL_RESPONSE_FIELD, BQ_WAREHOUSE_TYPE, EXPECTED_BQ_GQL_RESPONSE_FIELD, BQ_CONNECTION_TYPE
-from montecarlodata.queries.onboarding import TEST_DATABASE_CRED_MUTATION, TEST_SNOWFLAKE_CRED_MUTATION, \
-    TEST_BQ_CRED_MUTATION
+from montecarlodata.integrations.onboarding.fields import (
+    EXPECTED_GENERIC_DB_GQL_RESPONSE_FIELD,
+    REDSHIFT_CONNECTION_TYPE,
+    REDSHIFT_WAREHOUSE_TYPE,
+    SNOWFLAKE_CONNECTION_TYPE,
+    SNOWFLAKE_WAREHOUSE_TYPE,
+    EXPECTED_SNOWFLAKE_GQL_RESPONSE_FIELD,
+    BQ_WAREHOUSE_TYPE,
+    EXPECTED_BQ_GQL_RESPONSE_FIELD,
+    BQ_CONNECTION_TYPE,
+)
+from montecarlodata.queries.onboarding import (
+    TEST_DATABASE_CRED_MUTATION,
+    TEST_SNOWFLAKE_CRED_MUTATION,
+    TEST_BQ_CRED_MUTATION,
+)
 
 
 class WarehouseOnboardingService(BaseOnboardingService):
-
     def __init__(self, config: Config, **kwargs):
         super().__init__(config, **kwargs)
 
     @manage_errors
     def onboard_redshift(self, **kwargs) -> None:
         """
         Onboard a redshift connection by validating and adding a connection.
         """
-        kwargs['connectionType'] = REDSHIFT_CONNECTION_TYPE
-        kwargs['warehouseType'] = REDSHIFT_WAREHOUSE_TYPE
-        self.onboard(validation_query=TEST_DATABASE_CRED_MUTATION,
-                     validation_response=EXPECTED_GENERIC_DB_GQL_RESPONSE_FIELD,
-                     connection_type=REDSHIFT_CONNECTION_TYPE, **kwargs)
+        kwargs["connectionType"] = REDSHIFT_CONNECTION_TYPE
+        kwargs["warehouseType"] = REDSHIFT_WAREHOUSE_TYPE
+        self.onboard(
+            validation_query=TEST_DATABASE_CRED_MUTATION,
+            validation_response=EXPECTED_GENERIC_DB_GQL_RESPONSE_FIELD,
+            connection_type=REDSHIFT_CONNECTION_TYPE,
+            **kwargs
+        )
 
     @manage_errors
     def onboard_snowflake(self, **kwargs) -> None:
         """
         Onboard a snowflake connection by validating and adding a connection.
         """
-        kwargs['warehouseType'] = SNOWFLAKE_WAREHOUSE_TYPE
-        self.onboard(validation_query=TEST_SNOWFLAKE_CRED_MUTATION,
-                     validation_response=EXPECTED_SNOWFLAKE_GQL_RESPONSE_FIELD,
-                     connection_type=SNOWFLAKE_CONNECTION_TYPE, **kwargs)
+        kwargs["warehouseType"] = SNOWFLAKE_WAREHOUSE_TYPE
+        if kwargs.get("private_key"):
+            kwargs["private_key"] = read_as_base64(kwargs.pop("private_key")).decode(
+                "utf-8"
+            )
+        self.onboard(
+            validation_query=TEST_SNOWFLAKE_CRED_MUTATION,
+            validation_response=EXPECTED_SNOWFLAKE_GQL_RESPONSE_FIELD,
+            connection_type=SNOWFLAKE_CONNECTION_TYPE,
+            **kwargs
+        )
 
     @manage_errors
     def onboard_bq(self, **kwargs) -> None:
         """
         Onboard a BigQuery connection by validating and adding a connection.
 
         Reads and encodes service file as base64.
         """
-        kwargs['warehouseType'] = BQ_WAREHOUSE_TYPE
-        kwargs['serviceJson'] = read_as_base64(kwargs.pop('ServiceFile')).decode('utf-8')
-        self.onboard(validation_query=TEST_BQ_CRED_MUTATION,
-                     validation_response=EXPECTED_BQ_GQL_RESPONSE_FIELD,
-                     connection_type=BQ_CONNECTION_TYPE, **kwargs)
+        kwargs["warehouseType"] = BQ_WAREHOUSE_TYPE
+        kwargs["serviceJson"] = read_as_base64(kwargs.pop("ServiceFile")).decode(
+            "utf-8"
+        )
+        self.onboard(
+            validation_query=TEST_BQ_CRED_MUTATION,
+            validation_response=EXPECTED_BQ_GQL_RESPONSE_FIELD,
+            connection_type=BQ_CONNECTION_TYPE,
+            **kwargs
+        )
```

### Comparing `montecarlodata-0.9.2/montecarlodata/queries/collector.py` & `montecarlodata-0.90.0/montecarlodata/queries/collector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Queries related to managing the collector
 
 GENERATE_COLLECTOR_TEMPLATE = """
-mutation generateCollectorTemplate($region:String, $dcId:UUID) {
-  generateCollectorTemplate(region:$region, dcId:$dcId) {
+mutation generateCollectorTemplate($region:String, $dcId:UUID, $updateInfra:Boolean) {
+  generateCollectorTemplate(region:$region, dcId:$dcId, updateInfra: $updateInfra) {
     dc {
+      uuid
       templateLaunchUrl
       stackArn
       customerAwsAccountId
       active
       apiGatewayId
+      templateVariant
     }
   }
 }
 """
 
 ADD_COLLECTOR_RECORD = """
 mutation createCollectorRecord {
```

### Comparing `montecarlodata-0.9.2/montecarlodata/tools.py` & `montecarlodata-0.90.0/montecarlodata/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Command line tools
 """
+
 import copy
 import json
-from typing import Set
+from datetime import datetime
+from typing import Set, Optional
 
 import click
-from click import Option
+from click import Option, Context
 
 import montecarlodata.settings as settings
 from montecarlodata.common.common import normalize_gql
 
 
 class AdvancedOptions(Option):
     """
@@ -19,61 +21,108 @@
 
     Usage example -
         click.option('--foo' cls=MutuallyExclusiveOptions, mutually_exclusive_options=['bar']),
         click.option('--bar', cls=MutuallyExclusiveOptions, mutually_exclusive_options=['foo'])
     """
 
     def __init__(self, *args, **kwargs):
-        help_text = kwargs.get('help', '')
-        self._friendly_mutual_args = self._friendly_required_args = self._friendly_at_least_one_set = None
-
-        self.mutually_exclusive_options = set(kwargs.pop('mutually_exclusive_options', []))
-        self.required_with_options = set(kwargs.pop('required_with_options', []))
-        self.at_least_one_set = set(kwargs.pop('at_least_one_set', []))
-        self.prompt_if_requested = kwargs.pop('prompt_if_requested', False)
+        help_text = kwargs.get("help", "")
+        self._friendly_mutual_args = self._friendly_required_args = (
+            self._friendly_at_least_one_set
+        ) = None
+
+        self.mutually_exclusive_options = set(
+            kwargs.pop("mutually_exclusive_options", [])
+        )
+        self.required_with_options = set(kwargs.pop("required_with_options", []))
+        self.at_least_one_set = set(kwargs.pop("at_least_one_set", []))
+        self.prompt_if_requested = kwargs.pop("prompt_if_requested", False)
+
+        self.values_with_required_options = set(
+            kwargs.pop("values_with_required_options", [])
+        )
+        self.required_options_for_values = set(
+            kwargs.pop("required_options_for_values", [])
+        )
 
         # Update help for options and create friendly args (i.e. human readable).
         if self.mutually_exclusive_options:
-            self._friendly_mutual_args = self._create_friendly_args(options=self.mutually_exclusive_options)
+            self._friendly_mutual_args = self._create_friendly_args(
+                options=self.mutually_exclusive_options
+            )
             help_text = f"{help_text} This option cannot be used with {self._friendly_mutual_args}."
         if self.required_with_options:
-            self._friendly_required_args = self._create_friendly_args(options=self.required_with_options)
+            self._friendly_required_args = self._create_friendly_args(
+                options=self.required_with_options
+            )
             help_text = f"{help_text} This option requires setting {self._friendly_required_args}."
-        self._friendly_at_least_one_set = self._create_friendly_args(self.at_least_one_set)
-        kwargs['help'] = help_text
+        if self.required_options_for_values:
+            self._friendly_required_options_for_values = self._create_friendly_args(
+                self.required_options_for_values
+            )
+            help_text = (
+                f"{help_text} This option requires setting {self._friendly_required_options_for_values} "
+                f"when it is set to one of these values: {self.values_with_required_options}."
+            )
+        self._friendly_at_least_one_set = self._create_friendly_args(
+            self.at_least_one_set
+        )
+        kwargs["help"] = help_text
         super(AdvancedOptions, self).__init__(*args, **kwargs)
 
     def handle_parse_result(self, ctx, opts, args):
         """
         Handle any conflicts, missing values or any required hidden prompts.
         """
         cli_friendly_name = normalize_gql(self.name)
 
-        if self.mutually_exclusive_options.intersection(opts) and self.name in opts:
-            raise click.BadParameter(f"Cannot use '{cli_friendly_name}' with {self._friendly_mutual_args}.")
-        if self.name in opts and not self.required_with_options.issubset(opts):
-            raise click.BadParameter(f"Cannot use '{cli_friendly_name}' without {self._friendly_required_args}.")
-        if self.prompt_if_requested and self.name in opts and opts[self.name] == settings.SHOW_PROMPT_VALUE:
-            opts[self.name] = click.prompt(cli_friendly_name, hide_input=True)
-        else:
-            self.prompt = None
+        if self.name in opts:
+            if self.mutually_exclusive_options.intersection(opts):
+                raise click.BadParameter(
+                    f"Cannot use '{cli_friendly_name}' with {self._friendly_mutual_args}."
+                )
+            if not self.required_with_options.issubset(opts):
+                raise click.BadParameter(
+                    f"Cannot use '{cli_friendly_name}' without {self._friendly_required_args}."
+                )
+            if opts[
+                self.name
+            ] in self.values_with_required_options and not self.required_options_for_values.issubset(
+                opts
+            ):
+                raise click.BadParameter(
+                    f"Cannot use '{cli_friendly_name}' with value '{opts[self.name]}' without "
+                    f"{self._friendly_required_options_for_values}."
+                )
+            if (
+                self.prompt_if_requested
+                and opts[self.name] == settings.SHOW_PROMPT_VALUE
+            ):
+                opts[self.name] = click.prompt(cli_friendly_name, hide_input=True)
+            else:
+                self.prompt = None
+
         if self.at_least_one_set and not any(x in opts for x in self.at_least_one_set):
-            raise click.BadParameter(f'Missing required options from {self._friendly_at_least_one_set}.')
+            raise click.BadParameter(
+                f"Missing required options from {self._friendly_at_least_one_set}."
+            )
 
         return super(AdvancedOptions, self).handle_parse_result(ctx, opts, args)
 
     @staticmethod
     def _create_friendly_args(options: Set[str]) -> str:
         """
         Build a more human readable sentence from options.
         """
         friendly_options = list(copy.deepcopy(options))
         last_element = friendly_options.pop() if len(friendly_options) > 1 else None
 
-        friendly_options = ', '.join([f"'{normalize_gql(option)}'" for option in friendly_options])
+        friendly_options = ", ".join(
+            [f"'{normalize_gql(option)}'" for option in friendly_options]
+        )
         if last_element:
             friendly_options = f"{friendly_options}, and '{last_element}'"
         return friendly_options
 
 
 def add_common_options(options):
     """
@@ -91,19 +140,47 @@
 def validate_json_callback(ctx_, param_, value):
     """
     Convenience callback to help validate (and load) JSON in option strings
     """
     try:
         return json.loads(value)
     except json.decoder.JSONDecodeError as err:
-        raise click.BadParameter(f'Malformed JSON - {err}')
+        raise click.BadParameter(f"Malformed JSON - {err}")
     except TypeError:
         return value
 
 
 def convert_uuid_callback(ctx_, param_, value):
     """
     Convenience callback to convert UUIDs into strings
     """
     if value:
         return str(value)  # str(None) returns 'None'
     return value
+
+
+def convert_empty_str_callback(ctx_, param_, value):
+    """
+    Convenience callback to convert an empty (or empty like) string into None
+    """
+    if bool(value and not value.isspace()):
+        return value
+
+
+def dump_help(cmd, parent: Optional[Context] = None):
+    """
+    Recursively echos help text for a cmd
+    """
+    ctx = click.core.Context(cmd, info_name=cmd.name, parent=parent)
+    click.echo(cmd.get_help(ctx), err=True)
+    for sub in getattr(cmd, "commands", {}).values():
+        dump_help(sub, ctx)
+
+
+def format_date(dt: str) -> str:
+    """Format string from ISO format to YYYY-MM-DD"""
+    return datetime.fromisoformat(dt).strftime("%Y-%m-%d")
+
+
+def format_datetime(dt: str) -> str:
+    """Format string from ISO format to YYYY-MM-DD HH:MM:SS"""
+    return datetime.fromisoformat(dt).strftime("%Y-%m-%d %H:%M:%S")
```

### Comparing `montecarlodata-0.9.2/montecarlodata.egg-info/PKG-INFO` & `montecarlodata-0.90.0/montecarlodata.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,159 +1,185 @@
 Metadata-Version: 2.1
 Name: montecarlodata
-Version: 0.9.2
+Version: 0.90.0
 Summary: Monte Carlo's CLI
 Home-page: https://www.montecarlodata.com/
 Author: Monte Carlo Data, Inc
 Author-email: info@montecarlodata.com
 License: Apache Software License (Apache 2.0)
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3>=1.19.4
+Requires-Dist: click>=8.1.3
+Requires-Dist: click-config-file==0.6.0
+Requires-Dist: requests<=3.0.0,>=2.0.0
+Requires-Dist: retry==0.9.2
+Requires-Dist: tabulate>=0.8.7
+Requires-Dist: dataclasses-json>=0.5.4
+Requires-Dist: PyYAML>=5.4.1
+Requires-Dist: python-box>=6.0.0
+Requires-Dist: pycarlo>=0.8.12
+Requires-Dist: Jinja2>=3.1.2
+Requires-Dist: questionary==1.10.0
 
 # Monte Carlo CLI
+
 Monte Carlo's Alpha CLI!
 
 ## Installation
-Requires Python 3.7 or greater. Normally you can install and update using pip. For instance: 
-```
+
+Requires Python 3.8 or greater. Normally you can install and update using `pip`. For instance:
+
+```shell
+pip install virtualenv
 virtualenv venv
 . venv/bin/activate
 
 pip install -U montecarlodata
 ```
+
 Developers of the CLI can use:
-```
-make install 
+
+```shell
+pip install virtualenv
+make install
 . venv/bin/activate
+pre-commit install
 ```
 
 Either way confirm the installation by running:
-```
+
+```shell
 montecarlo --version
 ```
 
-If the Python requirement does not work for you please reach out to `customer-success@montecarlodata.com`. Docker is an option.
+If the Python requirement does not work for you please reach out to `support@montecarlodata.com`. Docker is an option.
 
 ## Quick start
+
 First time users can configure the tool by following the onscreen prompts:
-```
+
+```shell
 montecarlo configure
 ```
-MCD tokens can be generated from the [dashboard](https://getmontecarlo.com/settings/api).
- 
-Any AWS profiles or regions should be for the account the Data Collector (DC) is deployed to. If you are not using the
-CLI for onboarding, you may leave the AWS configuration blank.
 
-Use the `--help` flag for details on any advanced options (e.g. creating multiple montecarlo profiles) or any prompts.
+MCD tokens can be generated from the [dashboard](https://getmontecarlo.com/get-token).
+
+Use the `--help` flag for details on any advanced options (e.g. creating multiple montecarlo profiles) or
+see docs [here][cli-docs].
 
 That's it! You can always validate your connection with:
-```
+
+```shell
 montecarlo validate
 ```
 
 ## User settings
-Any configuration set by `montecarlo configure` can be found in '~/.mcd/' by default.
+
+Any configuration set by `montecarlo configure` can be found in `~/.mcd/` by default.
 
 The MCD ID and Token can be overwritten, or even set, by the environment:
-- MCD_DEFAULT_API_ID
-- MCD_DEFAULT_API_TOKEN
 
-These two are required either as part of `configure` or as environment variables. 
-For AWS, system defaults are used if not set as part of `configure`.
+- `MCD_DEFAULT_API_ID`
+- `MCD_DEFAULT_API_TOKEN`
+
+These two are required either as part of `configure` or as environment variables.
 
 The following values can also be set by the environment:
-- MCD_API_ENDPOINT - Overwrite the default API endpoint
-- MCD_VERBOSE_ERRORS - Enable verbose logging on errors (default=false)
+
+- `MCD_API_ENDPOINT` - Overwrite the default API endpoint
+- `MCD_VERBOSE_ERRORS` - Enable verbose logging on errors (default=false)
 
 ## Help
-Help for commands, options and arguments can be found using the `--help` flag.
-Additional documentation is available [here](https://docs.getmontecarlo.com/docs).
 
-All commands, except `configure` and `validate`, support an `--option-file` flag, which allows you to use a file in place of passing options.
-For instance, a `--name` flag can be set by creating a file containing:
+Documentation for commands, options, and arguments can be found [here][cli-docs].
+
+You can also use `montecarlo help` to echo all help text or use the `--help` flag on any command.
+
+## Examples
+
+### Using Docker from a local installation
+
+```shell
+docker build -t montecarlo .
+docker run -e MCD_DEFAULT_API_ID='<ID>' -e MCD_DEFAULT_API_TOKEN='<TOKEN>' montecarlo --version
 ```
-name="Artemis"
+
+Replace `--version` with any sub-commands or options. If interacting with files those directories will probably need to be mounted too.
+
+### Configure a named profile with custom config-path
+
+```shell
+$ montecarlo configure --profile-name zeus --config-path .
+Key ID: 1234
+Secret:
+
+$ cat ./profiles.ini
+[zeus]
+mcd_id = 1234
+mcd_token = 5678
 ```
-Any dashes must be replaced by underscores. For instance, `--foo-bar` would be `foo_bar="qux"`.
 
-Resolution is CLI Options > Option File.
+### List active integrations
 
-## Examples
-- Using Docker from a local installation
-    ```
-    docker build -t montecarlo .
-    docker run -v ${HOME}/.aws/credentials:/root/.aws/credentials:ro \
-               -e MCD_DEFAULT_API_ID='<ID>' \
-               -e MCD_DEFAULT_API_TOKEN='<TOKEN>' \
-               -e AWS_DEFAULT_PROFILE='<PROFILE>' \
-               -e AWS_DEFAULT_REGION='us-east-1' \
-               montecarlo --version
-    ```
-    Replace `--version` with any sub-commands or options. If interacting with files those directories will probably need to be mounted too.
-
-
-- Configure a named profile with custom config-path
-    ```
-    $ montecarlo configure --profile-name zeus --config-path .
-    Key ID: 1234
-    Secret:
-    AWS profile name []: shiva
-    AWS region [us-east-1]:
-  
-    $  cat ./profiles.ini 
-    [zeus]
-    mcd_id = 1234
-    mcd_token = 5678
-    aws_profile = shiva
-    aws_region = us-east-1
-    ```
-  
-- List active integrations
-    ```
-    $ montecarlo integrations list
-    ╒══════════════════╤══════════════════════════════════════╤══════════════════════════════════╕
-    │ Integration      │ ID                                   │ Created on (UTC)                 │
-    ╞══════════════════╪══════════════════════════════════════╪══════════════════════════════════╡
-    │ Odin             │ 58005657-2914-4701-9a11-260ac425b14e │ 2021-01-02T01:30:52.806602+00:00 │
-    ├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
-    │ Thor             │ 926816bd-ab17-4f95-a953-fa14482c59de │ 2021-01-02T01:31:19.892205+00:00 │
-    ├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
-    │ Loki             │ 1cf1dc0d-d8ec-4c85-8e64-57ab2ad8e023 │ 2021-01-02T01:32:37.709747+00:00 │
-    ╘══════════════════╧══════════════════════════════════════╧══════════════════════════════════╛
-    ```
-
-- Apply monitors configuration
-
-    ```
-    $ montecarlo monitors apply --namespace my-monitors
-
-    Gathering monitor configuration files.
-    - models/customer_success/schema.yml - Embedded monitor configuration found.
-    - models/customer_success/schema.yml - Monitor configuration found.
-    - models/lineage/schema.yml - Embedded monitor configuration found.
-    
-    Modifications:
-    - ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod.customer_360
-    - ResourceModificationType.UPDATE - Monitor: type=categories, table=analytics:prod.customer_360
-    - ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod_lineage.lineage_nodes
-    - ResourceModificationType.UPDATE - Freshness SLI: table=analytics:prod.customer_360, freshness_threshold=30
-    ```
+```shell
+$ montecarlo integrations list
+╒══════════════════╤══════════════════════════════════════╤══════════════════════════════════╕
+│ Integration      │ ID                                   │ Created on (UTC)                 │
+╞══════════════════╪══════════════════════════════════════╪══════════════════════════════════╡
+│ Odin             │ 58005657-2914-4701-9a11-260ac425b14e │ 2021-01-02T01:30:52.806602+00:00 │
+├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
+│ Thor             │ 926816bd-ab17-4f95-a953-fa14482c59de │ 2021-01-02T01:31:19.892205+00:00 │
+├──────────────────┼──────────────────────────────────────┼──────────────────────────────────┤
+│ Loki             │ 1cf1dc0d-d8ec-4c85-8e64-57ab2ad8e023 │ 2021-01-02T01:32:37.709747+00:00 │
+╘══════════════════╧══════════════════════════════════════╧══════════════════════════════════╛
+```
+
+### Apply monitors configuration
+
+```shell
+$ montecarlo monitors apply --namespace my-monitors
+
+Gathering monitor configuration files.
+- models/customer_success/schema.yml - Embedded monitor configuration found.
+- models/customer_success/schema.yml - Monitor configuration found.
+- models/lineage/schema.yml - Embedded monitor configuration found.
+
+Modifications:
+- ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod.customer_360
+- ResourceModificationType.UPDATE - Monitor: type=categories, table=analytics:prod.customer_360
+- ResourceModificationType.UPDATE - Monitor: type=stats, table=analytics:prod_lineage.lineage_nodes
+- ResourceModificationType.UPDATE - Freshness SLI: table=analytics:prod.customer_360, freshness_threshold=30
+```
+
+### Import DBT manifest
+
+```shell
+$ montecarlo import dbt-manifest --dbt-manifest-file target/manifest.json
+
+Importing DBT objects into Monte Carlo catalog. please wait...
+
+Imported a total of 51 DBT objects into Monte Carlo catalog.
+```
 
 ## Tests and Releases
-Locally `make test` will run all tests. CircleCI manages all testing for deployment.
 
-When ready to release make a PR for `master`. After merging CircleCI will test and deploy to [PyPI](https://pypi.org/project/montecarlodata/).
+Locally `make test` will run all tests. CircleCI manages all testing for deployment.
 
-Don't forget to increment the version number in `setup.py` first! An existing version will not be deployed.
+To publish a new release, simply add a new version tag, e.g. `v1.0.0`, and push that tag to GitHub. CircleCI will take care of publishing a new package to [PyPI](https://pypi.org/project/montecarlodata/) and generating documentation.
 
 ## License
+
 Apache 2.0 - See the [LICENSE](http://www.apache.org/licenses/LICENSE-2.0) for more information.
 
+[cli-docs]: https://clidocs.getmontecarlo.com/
```

### Comparing `montecarlodata-0.9.2/setup.py` & `montecarlodata-0.90.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-import distutils.text_file
 from pathlib import Path
 from typing import List, Optional
 
 from setuptools import setup, find_packages
 
-__VERSION__ = '0.9.2'
 
-
-def parse_requirements(file_name: Optional[str] = 'requirements.txt') -> List[str]:
-    return distutils.text_file.TextFile(filename=str(Path(__file__).with_name(file_name))).readlines()
+def parse_requirements(file_name: Optional[str] = "requirements.txt") -> List[str]:
+    with Path.open(Path(__file__).parent / file_name, "r") as f:
+        return f.readlines()
 
 
 def get_long_description():
-    with open('README.md', 'r') as fh:
+    with open("README.md", "r") as fh:
         return fh.read()
 
 
 setup(
-    name='montecarlodata',
-    version=__VERSION__,
-    license='Apache Software License (Apache 2.0)',
-    description='Monte Carlo\'s CLI',
+    name="montecarlodata",
+    use_scm_version=True,
+    license="Apache Software License (Apache 2.0)",
+    description="Monte Carlo's CLI",
     long_description=get_long_description(),
-    long_description_content_type='text/markdown',
-    author='Monte Carlo Data, Inc',
-    author_email='info@montecarlodata.com',
-    url='https://www.montecarlodata.com/',
-    packages=find_packages(exclude=['tests*']),
+    long_description_content_type="text/markdown",
+    author="Monte Carlo Data, Inc",
+    author_email="info@montecarlodata.com",
+    url="https://www.montecarlodata.com/",
+    packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     install_requires=parse_requirements(),
-    entry_points='''
+    entry_points="""
         [console_scripts]
         montecarlo=montecarlodata.cli:entry_point
-    ''',
+    """,
     classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Natural Language :: English',
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8'
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Natural Language :: English",
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
-    python_requires='>=3.7'
+    python_requires=">=3.8",
+    setup_requires=["setuptools", "setuptools_scm"],
 )
```

