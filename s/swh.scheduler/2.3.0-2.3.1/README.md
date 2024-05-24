# Comparing `tmp/swh_scheduler-2.3.0.tar.gz` & `tmp/swh_scheduler-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh_scheduler-2.3.0.tar", last modified: Wed May 22 15:45:49 2024, max compression
+gzip compressed data, was "swh_scheduler-2.3.1.tar", last modified: Fri May 24 07:54:29 2024, max compression
```

## Comparing `swh_scheduler-2.3.0.tar` & `swh_scheduler-2.3.1.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.459625 swh_scheduler-2.3.0/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1419 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       14 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2630 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/LICENSE.Celery
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2703 2024-05-22 15:45:49.459625 swh_scheduler-2.3.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      292 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/README.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.415625 swh_scheduler-2.3.0/data/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      646 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/data/README.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1769 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/data/elastic-template.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/data/update-index-settings.json
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.415625 swh_scheduler-2.3.0/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.419625 swh_scheduler-2.3.0/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.419625 swh_scheduler-2.3.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      887 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7664 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3060 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/simulator.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      939 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1935 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/requirements-journal.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       21 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/requirements-simulator.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       48 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      187 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-05-22 15:45:49.459625 swh_scheduler-2.3.0/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.419625 swh_scheduler-2.3.0/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       36 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/sql/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1384 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/sql/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.403625 swh_scheduler-2.3.0/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.423625 swh_scheduler-2.3.0/swh/scheduler/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2195 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.427625 swh_scheduler-2.3.0/swh/scheduler/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      649 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      910 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/api/serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4203 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/api/server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    41268 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/backend.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.427625 swh_scheduler-2.3.0/swh/scheduler/celery_backend/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/celery_backend/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14088 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/celery_backend/config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3283 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/celery_backend/pika_listener.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13221 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/celery_backend/recurrent_visits.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6779 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/celery_backend/runner.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.431625 swh_scheduler-2.3.0/swh/scheduler/cli/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3157 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5640 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/add_forge_now.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7546 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/admin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4826 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/celery_monitor.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1051 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2203 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/journal.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18286 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5089 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/origin_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2552 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/simulator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12944 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/task.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7914 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/task_type.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15189 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       62 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2933 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      473 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18935 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12008 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/journal_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14710 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/model.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3647 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.431625 swh_scheduler-2.3.0/swh/scheduler/simulator/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5652 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/simulator/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6293 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/simulator/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2349 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/simulator/origin_scheduler.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7801 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/simulator/origins.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2754 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/simulator/task_scheduler.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.435625 swh_scheduler-2.3.0/swh/scheduler/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       44 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10846 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14607 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/40-func.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/60-indexes.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.443625 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2111 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/02.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/03.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/04.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5119 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/05.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      625 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/06.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1727 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/07.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1924 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/08.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7034 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/09.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1581 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/10.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2070 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/11.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1769 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/12.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      967 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/13.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1729 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/14.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1126 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/15.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2467 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/16.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      152 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/17.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      328 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/18.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      958 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/19.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/20.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2467 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/23.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      471 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/24.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2944 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/25.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1478 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/26.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1113 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/27.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2112 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/28.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1241 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/29.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      224 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/30-bis.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2991 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/30.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      680 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/31.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2182 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/32.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3628 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/33.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1738 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/34.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      617 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/35.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2944 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/task.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.451625 swh_scheduler-2.3.0/swh/scheduler/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3756 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/common.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.451625 swh_scheduler-2.3.0/swh/scheduler/tests/data/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/data/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      555 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/data/logging-config.yaml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/lister/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/lister/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/lister/foo/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      317 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/lister/foo/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      386 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/lister/foo/tasks.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/loader/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/loader/bar/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      317 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/loader/bar/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      381 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/loader/bar/tasks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/tasks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2568 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_api_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11224 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_celery_tasks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24334 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5688 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_add_forge_now.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4174 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_celery_monitor.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2042 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3770 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_journal.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8485 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1677 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_origin_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4315 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_task_type.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1624 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2055 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3838 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2836 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    30355 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_journal_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2731 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_model.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8371 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_recurrent_visits.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    62043 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_scheduler.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3532 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1967 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_simulator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      776 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_temporary.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5947 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3915 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh.scheduler.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2703 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      106 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      554 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1199 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.636901 swh_scheduler-2.3.1/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1419 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       14 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2630 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/LICENSE.Celery
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2703 2024-05-24 07:54:29.636901 swh_scheduler-2.3.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      292 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/README.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.596901 swh_scheduler-2.3.1/data/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      646 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/data/README.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1769 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/data/elastic-template.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/data/update-index-settings.json
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.596901 swh_scheduler-2.3.1/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.596901 swh_scheduler-2.3.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.596901 swh_scheduler-2.3.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      887 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7664 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3060 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/docs/simulator.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      939 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1935 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/requirements-journal.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       21 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/requirements-simulator.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       48 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      187 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-05-24 07:54:29.640901 swh_scheduler-2.3.1/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.596901 swh_scheduler-2.3.1/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       36 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/sql/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1384 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/sql/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.584901 swh_scheduler-2.3.1/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.604901 swh_scheduler-2.3.1/swh/scheduler/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2195 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.604901 swh_scheduler-2.3.1/swh/scheduler/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      649 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      910 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/api/serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4203 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/api/server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    41855 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/backend.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.604901 swh_scheduler-2.3.1/swh/scheduler/celery_backend/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/celery_backend/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14088 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/celery_backend/config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3283 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/celery_backend/pika_listener.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13221 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/celery_backend/recurrent_visits.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6779 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/celery_backend/runner.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.608901 swh_scheduler-2.3.1/swh/scheduler/cli/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3157 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5640 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/add_forge_now.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7546 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/admin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4826 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/celery_monitor.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1051 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2203 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/journal.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18286 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5089 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/origin_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2552 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/simulator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12944 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/task.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7914 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/task_type.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15189 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       62 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/cli_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2933 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      473 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18955 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12008 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/journal_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14710 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/model.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3647 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.612901 swh_scheduler-2.3.1/swh/scheduler/simulator/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5652 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/simulator/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6293 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/simulator/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2349 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/simulator/origin_scheduler.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7801 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/simulator/origins.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2754 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/simulator/task_scheduler.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.612901 swh_scheduler-2.3.1/swh/scheduler/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       44 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10846 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14607 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/40-func.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/60-indexes.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.624901 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2111 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/02.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/03.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/04.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5119 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/05.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      625 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/06.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1727 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/07.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1924 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/08.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7034 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/09.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1581 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/10.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2070 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/11.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1769 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/12.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      967 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/13.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1729 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/14.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1126 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/15.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2467 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/16.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      152 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/17.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      328 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/18.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      958 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/19.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/20.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2467 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/23.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      471 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/24.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2944 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/25.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1478 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/26.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1113 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/27.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2112 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/28.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1241 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/29.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      224 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/30-bis.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2991 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/30.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      680 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/31.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2182 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/32.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3628 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/33.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1738 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/34.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      617 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/35.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2944 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/task.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.632901 swh_scheduler-2.3.1/swh/scheduler/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3756 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/common.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.632901 swh_scheduler-2.3.1/swh/scheduler/tests/data/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/data/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      555 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/data/logging-config.yaml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.632901 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.632901 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/lister/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/lister/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.632901 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/lister/foo/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      317 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/lister/foo/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      386 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/lister/foo/tasks.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.632901 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/loader/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.632901 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/loader/bar/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      317 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/loader/bar/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      381 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/fixtures/loader/bar/tasks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/tasks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2568 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_api_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11224 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_celery_tasks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24334 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5688 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_add_forge_now.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4174 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_celery_monitor.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2042 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3770 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_journal.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8485 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1677 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_origin_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4315 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_task_type.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1624 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2055 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3838 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2836 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    30355 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_journal_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2731 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_model.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8371 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_recurrent_visits.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    62540 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_scheduler.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3532 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1967 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_simulator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      776 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_temporary.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5947 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3915 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/swh/scheduler/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-24 07:54:29.632901 swh_scheduler-2.3.1/swh.scheduler.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2703 2024-05-24 07:54:29.000000 swh_scheduler-2.3.1/swh.scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2024-05-24 07:54:29.000000 swh_scheduler-2.3.1/swh.scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-24 07:54:29.000000 swh_scheduler-2.3.1/swh.scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      106 2024-05-24 07:54:29.000000 swh_scheduler-2.3.1/swh.scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      554 2024-05-24 07:54:29.000000 swh_scheduler-2.3.1/swh.scheduler.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-24 07:54:29.000000 swh_scheduler-2.3.1/swh.scheduler.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1199 2024-05-24 07:54:23.000000 swh_scheduler-2.3.1/tox.ini
```

### Comparing `swh_scheduler-2.3.0/.pre-commit-config.yaml` & `swh_scheduler-2.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/CODE_OF_CONDUCT.md` & `swh_scheduler-2.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/LICENSE` & `swh_scheduler-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/LICENSE.Celery` & `swh_scheduler-2.3.1/LICENSE.Celery`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/PKG-INFO` & `swh_scheduler-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scheduler
-Version: 2.3.0
+Version: 2.3.1
 Summary: Software Heritage scheduler
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-scheduler/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler.git
```

### Comparing `swh_scheduler-2.3.0/conftest.py` & `swh_scheduler-2.3.1/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/data/README.md` & `swh_scheduler-2.3.1/data/README.md`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/data/elastic-template.json` & `swh_scheduler-2.3.1/data/elastic-template.json`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/docs/cli.rst` & `swh_scheduler-2.3.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/docs/index.rst` & `swh_scheduler-2.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/docs/simulator.rst` & `swh_scheduler-2.3.1/docs/simulator.rst`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/mypy.ini` & `swh_scheduler-2.3.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/pyproject.toml` & `swh_scheduler-2.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/sql/Makefile` & `swh_scheduler-2.3.1/sql/Makefile`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/__init__.py` & `swh_scheduler-2.3.1/swh/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/api/client.py` & `swh_scheduler-2.3.1/swh/scheduler/api/client.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/api/serializers.py` & `swh_scheduler-2.3.1/swh/scheduler/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/api/server.py` & `swh_scheduler-2.3.1/swh/scheduler/api/server.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/backend.py` & `swh_scheduler-2.3.1/swh/scheduler/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -910,15 +910,16 @@
             timestamp = utcnow()
 
         cur.execute(
             "select * from swh_scheduler_schedule_task_run(%s, %s, %s, %s)",
             (task_id, backend_id, metadata, timestamp),
         )
 
-        return TaskRun(**cur.fetchone())
+        row = cur.fetchone()
+        return TaskRun(**row)
 
     @db_transaction()
     def mass_schedule_task_runs(
         self, task_runs: List[TaskRun], db=None, cur=None
     ) -> None:
         """Schedule a bunch of task runs.
 
@@ -942,76 +943,95 @@
     def start_task_run(
         self,
         backend_id: str,
         metadata: Optional[Dict[str, Any]] = None,
         timestamp: Optional[datetime.datetime] = None,
         db=None,
         cur=None,
-    ) -> TaskRun:
+    ) -> Optional[TaskRun]:
         """Mark a given task as started, updating the corresponding task_run
            entry in the database.
 
         Args:
             backend_id: the identifier of the job in the backend
             metadata: metadata to add to the task_run entry
             timestamp: the instant the event occurred
 
         Returns:
-            a TaskRun object with updated fields
+            a TaskRun object with updated fields, or None if there was no
+            TaskRun recorded with a matching backend_id.
 
         """
 
         if metadata is None:
             metadata = {}
 
         if timestamp is None:
             timestamp = utcnow()
 
         cur.execute(
             "select * from swh_scheduler_start_task_run(%s, %s, %s)",
             (backend_id, metadata, timestamp),
         )
 
-        return TaskRun(**cur.fetchone())
+        for row in cur:
+            if row["status"] is not None:
+                return TaskRun(**row)
+
+        logger.debug(
+            "Failed to mark task run %s as started",
+            backend_id,
+        )
+        return None
 
     @db_transaction()
     def end_task_run(
         self,
         backend_id: str,
         status: TaskRunStatus,
         metadata: Optional[Dict[str, Any]] = None,
         timestamp: Optional[datetime.datetime] = None,
         db=None,
         cur=None,
-    ) -> TaskRun:
+    ) -> Optional[TaskRun]:
         """Mark a given task as ended, updating the corresponding task_run entry in the
         database.
 
         Args:
             backend_id: the identifier of the job in the backend
             status: how the task ended
             metadata: metadata to add to the task_run entry
             timestamp: the instant the event occurred
 
         Returns:
-            a TaskRun object with updated fields
+            a TaskRun object with updated fields, or None if there was no
+            TaskRun recorded with a matching backend_id.
 
         """
 
         if metadata is None:
             metadata = {}
 
         if timestamp is None:
             timestamp = utcnow()
 
         cur.execute(
             "select * from swh_scheduler_end_task_run(%s, %s, %s, %s)",
             (backend_id, status, metadata, timestamp),
         )
-        return TaskRun(**cur.fetchone())
+
+        for row in cur:
+            if row["status"] is not None:
+                return TaskRun(**row)
+
+        logger.debug(
+            "Failed to mark task run %s as ended",
+            backend_id,
+        )
+        return None
 
     @db_transaction()
     def filter_task_to_archive(
         self,
         after_ts: str,
         before_ts: str,
         limit: int = 10,
```

### Comparing `swh_scheduler-2.3.0/swh/scheduler/celery_backend/config.py` & `swh_scheduler-2.3.1/swh/scheduler/celery_backend/config.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/celery_backend/pika_listener.py` & `swh_scheduler-2.3.1/swh/scheduler/celery_backend/pika_listener.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/celery_backend/recurrent_visits.py` & `swh_scheduler-2.3.1/swh/scheduler/celery_backend/recurrent_visits.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/celery_backend/runner.py` & `swh_scheduler-2.3.1/swh/scheduler/celery_backend/runner.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/__init__.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/add_forge_now.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/add_forge_now.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/admin.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/admin.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/celery_monitor.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/celery_monitor.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/config.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/config.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/journal.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/journal.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/origin.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/origin.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/origin_utils.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/origin_utils.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/simulator.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/simulator.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/task.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/task.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/task_type.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/task_type.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/cli/utils.py` & `swh_scheduler-2.3.1/swh/scheduler/cli/utils.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/conftest.py` & `swh_scheduler-2.3.1/swh/scheduler/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/interface.py` & `swh_scheduler-2.3.1/swh/scheduler/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
 
     @remote_api_endpoint("task_run/start")
     def start_task_run(
         self,
         backend_id: str,
         metadata: Optional[Dict[str, Any]] = None,
         timestamp: Optional[datetime.datetime] = None,
-    ) -> TaskRun:
+    ) -> Optional[TaskRun]:
         """Mark a given task as started, updating the corresponding task_run
            entry in the database.
 
         Args:
             backend_id: the identifier of the job in the backend
             metadata: metadata to add to the task_run entry
             timestamp: the instant the event occurred
@@ -310,15 +310,15 @@
     @remote_api_endpoint("task_run/end")
     def end_task_run(
         self,
         backend_id: str,
         status: TaskRunStatus,
         metadata: Optional[Dict[str, Any]] = None,
         timestamp: Optional[datetime.datetime] = None,
-    ) -> TaskRun:
+    ) -> Optional[TaskRun]:
         """Mark a given task as ended, updating the corresponding task_run entry in the
         database.
 
         Args:
             backend_id: the identifier of the job in the backend
             status: how the task ended
             metadata: metadata to add to the task_run entry
```

### Comparing `swh_scheduler-2.3.0/swh/scheduler/journal_client.py` & `swh_scheduler-2.3.1/swh/scheduler/journal_client.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/model.py` & `swh_scheduler-2.3.1/swh/scheduler/model.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/pytest_plugin.py` & `swh_scheduler-2.3.1/swh/scheduler/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/simulator/__init__.py` & `swh_scheduler-2.3.1/swh/scheduler/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/simulator/common.py` & `swh_scheduler-2.3.1/swh/scheduler/simulator/common.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/simulator/origin_scheduler.py` & `swh_scheduler-2.3.1/swh/scheduler/simulator/origin_scheduler.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/simulator/origins.py` & `swh_scheduler-2.3.1/swh/scheduler/simulator/origins.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/simulator/task_scheduler.py` & `swh_scheduler-2.3.1/swh/scheduler/simulator/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/30-schema.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/40-func.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/40-func.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/60-indexes.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/02.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/02.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/03.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/03.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/04.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/04.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/05.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/05.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/06.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/06.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/07.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/07.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/08.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/08.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/09.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/09.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/10.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/10.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/11.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/11.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/12.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/12.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/13.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/13.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/14.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/14.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/15.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/15.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/16.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/16.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/19.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/19.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/23.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/23.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/25.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/25.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/26.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/26.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/27.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/27.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/28.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/28.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/29.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/29.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/30.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/30.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/31.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/31.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/32.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/32.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/33.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/33.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/34.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/34.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/35.sql` & `swh_scheduler-2.3.1/swh/scheduler/sql/upgrades/35.sql`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/task.py` & `swh_scheduler-2.3.1/swh/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/common.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/common.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/data/logging-config.yaml` & `swh_scheduler-2.3.1/swh/scheduler/tests/data/logging-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/tasks.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_api_client.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_celery_tasks.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_celery_tasks.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_add_forge_now.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_add_forge_now.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_celery_monitor.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_celery_monitor.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_config.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_journal.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_journal.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_origin.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_origin.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_origin_utils.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_origin_utils.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_task_type.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_task_type.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_utils.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_common.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_config.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_init.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_journal_client.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_journal_client.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_model.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_recurrent_visits.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_recurrent_visits.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_scheduler.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -662,14 +662,31 @@
             scheduled=btask.scheduled,
             started=ts,
             ended=ts2,
             metadata={"something": "stupid", "other": "stuff"},
             status="eventful",
         )
 
+    def test_start_end_task_run_not_scheduled(self, swh_scheduler):
+        assert (
+            swh_scheduler.start_task_run(
+                backend_id=str(uuid.uuid4()), metadata={}, timestamp=utcnow()
+            )
+            is None
+        )
+        assert (
+            swh_scheduler.end_task_run(
+                backend_id=str(uuid.uuid4()),
+                metadata={},
+                timestamp=utcnow(),
+                status="eventful",
+            )
+            is None
+        )
+
     def test_get_or_create_lister(self, swh_scheduler):
         db_listers = []
         for lister_args in LISTERS:
             db_listers.append(swh_scheduler.get_or_create_lister(**lister_args))
 
         for lister, lister_args in zip(db_listers, LISTERS):
             assert lister.name == lister_args["name"]
```

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_server.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_simulator.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_temporary.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_temporary.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/tests/test_utils.py` & `swh_scheduler-2.3.1/swh/scheduler/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh/scheduler/utils.py` & `swh_scheduler-2.3.1/swh/scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh.scheduler.egg-info/PKG-INFO` & `swh_scheduler-2.3.1/swh.scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scheduler
-Version: 2.3.0
+Version: 2.3.1
 Summary: Software Heritage scheduler
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-scheduler/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler.git
```

### Comparing `swh_scheduler-2.3.0/swh.scheduler.egg-info/SOURCES.txt` & `swh_scheduler-2.3.1/swh.scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/swh.scheduler.egg-info/requires.txt` & `swh_scheduler-2.3.1/swh.scheduler.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `swh_scheduler-2.3.0/tox.ini` & `swh_scheduler-2.3.1/tox.ini`

 * *Files identical despite different names*

