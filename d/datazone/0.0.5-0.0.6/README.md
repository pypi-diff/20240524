# Comparing `tmp/datazone-0.0.5.tar.gz` & `tmp/datazone-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazone-0.0.5.tar", max compression
+gzip compressed data, was "datazone-0.0.6.tar", max compression
```

## Comparing `datazone-0.0.5.tar` & `datazone-0.0.6.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0     2670 2024-03-21 15:31:24.807687 datazone-0.0.5/README.md
--rw-r--r--   0        0        0      198 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/auth/__init__.py
--rw-r--r--   0        0        0      165 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/auth/login.py
--rw-r--r--   0        0        0       98 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/auth/main.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/dataset/__init__.py
--rw-r--r--   0        0        0      703 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/dataset/list.py
--rw-r--r--   0        0        0      365 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/dataset/main.py
--rw-r--r--   0        0        0     1054 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/dataset/show.py
--rw-r--r--   0        0        0     1189 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/dataset/transactions.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/dataset/view/__init__.py
--rw-r--r--   0        0        0      478 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/dataset/view/create.py
--rw-r--r--   0        0        0      262 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/dataset/view/delete.py
--rw-r--r--   0        0        0      856 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/dataset/view/list.py
--rw-r--r--   0        0        0      272 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/dataset/view/main.py
--rw-r--r--   0        0        0     1250 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/datazone_typer.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/execution/__init__.py
--rw-r--r--   0        0        0     1459 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/execution/list.py
--rw-r--r--   0        0        0     2966 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/execution/log.py
--rw-r--r--   0        0        0      245 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/execution/main.py
--rw-r--r--   0        0        0     1225 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/execution/run.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/extract/__init__.py
--rw-r--r--   0        0        0     1964 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/extract/create.py
--rw-r--r--   0        0        0      270 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/extract/delete.py
--rw-r--r--   0        0        0      565 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/extract/execute.py
--rw-r--r--   0        0        0      926 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/extract/list.py
--rw-r--r--   0        0        0      329 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/extract/main.py
--rw-r--r--   0        0        0     1696 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/main.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/pipeline/__init__.py
--rw-r--r--   0        0        0      505 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/pipeline/create.py
--rw-r--r--   0        0        0      105 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/pipeline/main.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/profile/__init__.py
--rw-r--r--   0        0        0     1032 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/profile/create.py
--rw-r--r--   0        0        0      222 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/profile/delete.py
--rw-r--r--   0        0        0      599 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/profile/list.py
--rw-r--r--   0        0        0      339 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/profile/main.py
--rw-r--r--   0        0        0      245 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/profile/set_default.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/repository/__init__.py
--rw-r--r--   0        0        0     1283 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/repository/clone.py
--rw-r--r--   0        0        0     1126 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/repository/create.py
--rw-r--r--   0        0        0     4342 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/repository/deploy.py
--rw-r--r--   0        0        0      654 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/repository/list.py
--rw-r--r--   0        0        0      476 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/repository/main.py
--rw-r--r--   0        0        0      362 2024-03-21 15:31:24.807687 datazone-0.0.5/datazone/cli/repository/pull.py
--rw-r--r--   0        0        0     1885 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/repository/summary.py
--rw-r--r--   0        0        0     1091 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/repository/template_loader.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/repository/templates/__init__.py
--rw-r--r--   0        0        0      127 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/repository/templates/config.yml.jinja
--rw-r--r--   0        0        0      585 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/repository/templates/hello_world.py.jinja
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/schedule/__init__.py
--rw-r--r--   0        0        0     1225 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/schedule/create.py
--rw-r--r--   0        0        0      273 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/schedule/delete.py
--rw-r--r--   0        0        0      986 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/schedule/list.py
--rw-r--r--   0        0        0      260 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/schedule/main.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/source/__init__.py
--rw-r--r--   0        0        0     4130 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/source/create.py
--rw-r--r--   0        0        0      270 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/source/delete.py
--rw-r--r--   0        0        0      794 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/source/list.py
--rw-r--r--   0        0        0      254 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/cli/source/main.py
--rw-r--r--   0        0        0      149 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/constants.py
--rw-r--r--   0        0        0      211 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/context.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/common/__init__.py
--rw-r--r--   0        0        0     2391 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/common/config.py
--rw-r--r--   0        0        0     5739 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/common/settings.py
--rw-r--r--   0        0        0      287 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/common/types.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/connections/__init__.py
--rw-r--r--   0        0        0     2130 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/connections/auth.py
--rw-r--r--   0        0        0     1522 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/connections/session.py
--rw-r--r--   0        0        0      266 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/dataset.py
--rw-r--r--   0        0        0      225 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/extract.py
--rw-r--r--   0        0        0      481 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/mappings.py
--rw-r--r--   0        0        0     1288 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/core/transform.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/decorators/__init__.py
--rw-r--r--   0        0        0     1047 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/decorators/transform.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/errors/__init__.py
--rw-r--r--   0        0        0      258 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/errors/auth.py
--rw-r--r--   0        0        0      310 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/errors/base.py
--rw-r--r--   0        0        0      803 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/errors/common.py
--rw-r--r--   0        0        0      300 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/errors/local_errors.py
--rw-r--r--   0        0        0      157 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/extract_definitions/__init__.py
--rw-r--r--   0        0        0      325 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/extract_definitions/aws_s3_csv.py
--rw-r--r--   0        0        0       38 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/extract_definitions/base.py
--rw-r--r--   0        0        0      227 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/extract_definitions/mysql.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/models/__init__.py
--rw-r--r--   0        0        0      891 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/models/common.py
--rw-r--r--   0        0        0      866 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/models/config.py
--rw-r--r--   0        0        0      563 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/models/settings.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/service_callers/__init__.py
--rw-r--r--   0        0        0      977 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/service_callers/base.py
--rw-r--r--   0        0        0     1366 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/service_callers/crud.py
--rw-r--r--   0        0        0     1093 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/service_callers/dataset.py
--rw-r--r--   0        0        0      130 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/service_callers/git.py
--rw-r--r--   0        0        0     2420 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/service_callers/job.py
--rw-r--r--   0        0        0     1590 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/service_callers/repository.py
--rw-r--r--   0        0        0        0 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/utils/__init__.py
--rw-r--r--   0        0        0     1091 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/utils/git.py
--rw-r--r--   0        0        0      907 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/utils/helpers.py
--rw-r--r--   0        0        0      704 2024-03-21 15:31:24.811687 datazone-0.0.5/datazone/utils/types.py
--rw-r--r--   0        0        0     1090 2024-03-21 15:31:24.811687 datazone-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3653 1970-01-01 00:00:00.000000 datazone-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2670 2024-05-24 01:26:59.650879 datazone-0.0.6/README.md
+-rw-r--r--   0        0        0      198 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/auth/__init__.py
+-rw-r--r--   0        0        0      165 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/auth/login.py
+-rw-r--r--   0        0        0       98 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/auth/main.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/dataset/__init__.py
+-rw-r--r--   0        0        0      703 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/dataset/list.py
+-rw-r--r--   0        0        0      365 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/dataset/main.py
+-rw-r--r--   0        0        0     1054 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/dataset/show.py
+-rw-r--r--   0        0        0     1189 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/dataset/transactions.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/dataset/view/__init__.py
+-rw-r--r--   0        0        0      478 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/dataset/view/create.py
+-rw-r--r--   0        0        0      262 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/dataset/view/delete.py
+-rw-r--r--   0        0        0      856 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/dataset/view/list.py
+-rw-r--r--   0        0        0      272 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/dataset/view/main.py
+-rw-r--r--   0        0        0     1250 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/datazone_typer.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/execution/__init__.py
+-rw-r--r--   0        0        0     1459 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/execution/list.py
+-rw-r--r--   0        0        0     2966 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/execution/log.py
+-rw-r--r--   0        0        0      245 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/execution/main.py
+-rw-r--r--   0        0        0     1225 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/execution/run.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/extract/__init__.py
+-rw-r--r--   0        0        0     1964 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/extract/create.py
+-rw-r--r--   0        0        0      270 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/extract/delete.py
+-rw-r--r--   0        0        0      565 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/extract/execute.py
+-rw-r--r--   0        0        0      926 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/extract/list.py
+-rw-r--r--   0        0        0      329 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/extract/main.py
+-rw-r--r--   0        0        0     1696 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/main.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/pipeline/__init__.py
+-rw-r--r--   0        0        0      505 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/pipeline/create.py
+-rw-r--r--   0        0        0      105 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/pipeline/main.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/profile/__init__.py
+-rw-r--r--   0        0        0     1032 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/profile/create.py
+-rw-r--r--   0        0        0      222 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/profile/delete.py
+-rw-r--r--   0        0        0      599 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/profile/list.py
+-rw-r--r--   0        0        0      339 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/profile/main.py
+-rw-r--r--   0        0        0      245 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/profile/set_default.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/__init__.py
+-rw-r--r--   0        0        0     1283 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/clone.py
+-rw-r--r--   0        0        0     1126 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/create.py
+-rw-r--r--   0        0        0     4342 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/deploy.py
+-rw-r--r--   0        0        0      654 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/list.py
+-rw-r--r--   0        0        0      476 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/main.py
+-rw-r--r--   0        0        0      362 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/pull.py
+-rw-r--r--   0        0        0     1885 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/summary.py
+-rw-r--r--   0        0        0     1091 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/template_loader.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/templates/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/templates/config.yml.jinja
+-rw-r--r--   0        0        0      585 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/repository/templates/hello_world.py.jinja
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/schedule/__init__.py
+-rw-r--r--   0        0        0     1225 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/schedule/create.py
+-rw-r--r--   0        0        0      273 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/schedule/delete.py
+-rw-r--r--   0        0        0      986 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/schedule/list.py
+-rw-r--r--   0        0        0      260 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/schedule/main.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/source/__init__.py
+-rw-r--r--   0        0        0     4130 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/source/create.py
+-rw-r--r--   0        0        0      270 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/source/delete.py
+-rw-r--r--   0        0        0      794 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/source/list.py
+-rw-r--r--   0        0        0      254 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/cli/source/main.py
+-rw-r--r--   0        0        0      149 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/constants.py
+-rw-r--r--   0        0        0      211 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/context.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/core/common/__init__.py
+-rw-r--r--   0        0        0     2391 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/core/common/config.py
+-rw-r--r--   0        0        0     5739 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/core/common/settings.py
+-rw-r--r--   0        0        0      287 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/core/common/types.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/core/connections/__init__.py
+-rw-r--r--   0        0        0     2130 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/core/connections/auth.py
+-rw-r--r--   0        0        0     1522 2024-05-24 01:26:59.650879 datazone-0.0.6/datazone/core/connections/session.py
+-rw-r--r--   0        0        0      266 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/core/dataset.py
+-rw-r--r--   0        0        0      225 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/core/extract.py
+-rw-r--r--   0        0        0      679 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/core/mappings.py
+-rw-r--r--   0        0        0     1288 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/core/transform.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/decorators/__init__.py
+-rw-r--r--   0        0        0     1047 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/decorators/transform.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/errors/__init__.py
+-rw-r--r--   0        0        0      258 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/errors/auth.py
+-rw-r--r--   0        0        0      310 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/errors/base.py
+-rw-r--r--   0        0        0      803 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/errors/common.py
+-rw-r--r--   0        0        0      300 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/errors/local_errors.py
+-rw-r--r--   0        0        0      157 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/extract_definitions/__init__.py
+-rw-r--r--   0        0        0      325 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/extract_definitions/aws_s3_csv.py
+-rw-r--r--   0        0        0       38 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/extract_definitions/base.py
+-rw-r--r--   0        0        0      227 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/extract_definitions/mysql.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/models/__init__.py
+-rw-r--r--   0        0        0      972 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/models/common.py
+-rw-r--r--   0        0        0      866 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/models/config.py
+-rw-r--r--   0        0        0      563 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/models/settings.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/service_callers/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/service_callers/base.py
+-rw-r--r--   0        0        0     1366 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/service_callers/crud.py
+-rw-r--r--   0        0        0     1093 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/service_callers/dataset.py
+-rw-r--r--   0        0        0      130 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/service_callers/git.py
+-rw-r--r--   0        0        0     2558 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/service_callers/job.py
+-rw-r--r--   0        0        0     1590 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/service_callers/repository.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/utils/__init__.py
+-rw-r--r--   0        0        0     1091 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/utils/git.py
+-rw-r--r--   0        0        0      907 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/utils/helpers.py
+-rw-r--r--   0        0        0      704 2024-05-24 01:26:59.654879 datazone-0.0.6/datazone/utils/types.py
+-rw-r--r--   0        0        0     1090 2024-05-24 01:26:59.654879 datazone-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3653 1970-01-01 00:00:00.000000 datazone-0.0.6/PKG-INFO
```

### Comparing `datazone-0.0.5/README.md` & `datazone-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/dataset/list.py` & `datazone-0.0.6/datazone/cli/dataset/list.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/dataset/show.py` & `datazone-0.0.6/datazone/cli/dataset/show.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/dataset/transactions.py` & `datazone-0.0.6/datazone/cli/dataset/transactions.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/dataset/view/list.py` & `datazone-0.0.6/datazone/cli/dataset/view/list.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/datazone_typer.py` & `datazone-0.0.6/datazone/cli/datazone_typer.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/execution/list.py` & `datazone-0.0.6/datazone/cli/execution/list.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/execution/log.py` & `datazone-0.0.6/datazone/cli/execution/log.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/execution/run.py` & `datazone-0.0.6/datazone/cli/execution/run.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/extract/create.py` & `datazone-0.0.6/datazone/cli/extract/create.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/extract/execute.py` & `datazone-0.0.6/datazone/cli/extract/execute.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/extract/list.py` & `datazone-0.0.6/datazone/cli/extract/list.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/main.py` & `datazone-0.0.6/datazone/cli/main.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/profile/create.py` & `datazone-0.0.6/datazone/cli/profile/create.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/profile/list.py` & `datazone-0.0.6/datazone/cli/profile/list.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/repository/clone.py` & `datazone-0.0.6/datazone/cli/repository/clone.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/repository/create.py` & `datazone-0.0.6/datazone/cli/repository/create.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/repository/deploy.py` & `datazone-0.0.6/datazone/cli/repository/deploy.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/repository/list.py` & `datazone-0.0.6/datazone/cli/repository/list.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/repository/summary.py` & `datazone-0.0.6/datazone/cli/repository/summary.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/repository/template_loader.py` & `datazone-0.0.6/datazone/cli/repository/template_loader.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/repository/templates/hello_world.py.jinja` & `datazone-0.0.6/datazone/cli/repository/templates/hello_world.py.jinja`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/schedule/create.py` & `datazone-0.0.6/datazone/cli/schedule/create.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/schedule/list.py` & `datazone-0.0.6/datazone/cli/schedule/list.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/source/create.py` & `datazone-0.0.6/datazone/cli/source/create.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/cli/source/list.py` & `datazone-0.0.6/datazone/cli/source/list.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/core/common/config.py` & `datazone-0.0.6/datazone/core/common/config.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/core/common/settings.py` & `datazone-0.0.6/datazone/core/common/settings.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/core/connections/auth.py` & `datazone-0.0.6/datazone/core/connections/auth.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/core/connections/session.py` & `datazone-0.0.6/datazone/core/connections/session.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/core/transform.py` & `datazone-0.0.6/datazone/core/transform.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/decorators/transform.py` & `datazone-0.0.6/datazone/decorators/transform.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/errors/common.py` & `datazone-0.0.6/datazone/errors/common.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/models/common.py` & `datazone-0.0.6/datazone/models/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,7 +32,12 @@
     ExecutionStatus.UPSTREAM_FAILURE,
 ]
 
 
 class JobType(str, Enum):
     EXTRACT = "extract"
     PIPELINE = "pipeline"
+
+
+class OutputMode(str, Enum):
+    OVERWRITE = "overwrite"
+    APPEND = "append"
```

### Comparing `datazone-0.0.5/datazone/models/config.py` & `datazone-0.0.6/datazone/models/config.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/models/settings.py` & `datazone-0.0.6/datazone/models/settings.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/service_callers/base.py` & `datazone-0.0.6/datazone/service_callers/base.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/service_callers/crud.py` & `datazone-0.0.6/datazone/service_callers/crud.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/service_callers/dataset.py` & `datazone-0.0.6/datazone/service_callers/dataset.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/service_callers/job.py` & `datazone-0.0.6/datazone/service_callers/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, Dict
 
+from datazone.errors.common import DatazoneServiceError
 from datazone.service_callers.base import BaseServiceCaller
 
 
 class JobServiceCaller(BaseServiceCaller):
     service_name = "job"
 
     @classmethod
@@ -68,8 +69,10 @@
         response = session.get(f"{cls.get_service_url()}/extract/deploy/{extract_id}")
         return response.json()
 
     @classmethod
     def project_check(cls, project_changes: Dict):
         session = cls.get_session()
         response = session.post(f"{cls.get_service_url()}/inspect/project-check", json=project_changes)
+        if not response.ok:
+            raise DatazoneServiceError(response.text)
         return response.json()
```

### Comparing `datazone-0.0.5/datazone/service_callers/repository.py` & `datazone-0.0.6/datazone/service_callers/repository.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/utils/git.py` & `datazone-0.0.6/datazone/utils/git.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/utils/helpers.py` & `datazone-0.0.6/datazone/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/datazone/utils/types.py` & `datazone-0.0.6/datazone/utils/types.py`

 * *Files identical despite different names*

### Comparing `datazone-0.0.5/pyproject.toml` & `datazone-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datazone"
-version = "0.0.5"
+version = "0.0.6"
 description = "Datazone Client Package"
 authors = ["resulyurttakalan <resul@datazone.co>"]
 readme = "README.md"
 packages = [{ include = "datazone" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `datazone-0.0.5/PKG-INFO` & `datazone-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datazone
-Version: 0.0.5
+Version: 0.0.6
 Summary: Datazone Client Package
 Author: resulyurttakalan
 Author-email: resul@datazone.co
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

