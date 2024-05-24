# Comparing `tmp/sageworks-0.6.5.tar.gz` & `tmp/sageworks-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.6.5.tar", last modified: Sun May 19 21:37:59 2024, max compression
+gzip compressed data, was "sageworks-0.6.6.tar", last modified: Fri May 24 14:49:47 2024, max compression
```

## Comparing `sageworks-0.6.5.tar` & `sageworks-0.6.6.tar`

### file list

```diff
@@ -1,563 +1,565 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.010372 sageworks-0.6.5/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.952835 sageworks-0.6.5/.github/
--rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.6.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.6.5/.github/dependabot.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.953259 sageworks-0.6.5/.github/workflows/
--rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.6.5/.github/workflows/deploy-docs.yml
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.6.5/.github/workflows/python-lint.yml
--rw-r--r--   0 briford    (501) staff       (20)     2037 2024-05-15 21:28:12.000000 sageworks-0.6.5/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      791 2024-04-16 15:58:18.000000 sageworks-0.6.5/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.6.5/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.6.5/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.6.5/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     4961 2024-05-19 21:37:59.010304 sageworks-0.6.5/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     3510 2024-05-09 14:32:45.000000 sageworks-0.6.5/README.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.6.5/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.942536 sageworks-0.6.5/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.954401 sageworks-0.6.5/applications/aws_dashboard/
--rw-r--r--   0 briford    (501) staff       (20)     1071 2024-05-19 20:22:47.000000 sageworks-0.6.5/applications/aws_dashboard/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.6.5/applications/aws_dashboard/Dockerfile_plugins
--rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.6.5/applications/aws_dashboard/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-09 14:37:33.000000 sageworks-0.6.5/applications/aws_dashboard/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.955050 sageworks-0.6.5/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-06 16:51:44.000000 sageworks-0.6.5/applications/aws_dashboard/assets/bootstrap_darkly.min.css
--rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-06 16:51:44.000000 sageworks-0.6.5/applications/aws_dashboard/assets/default.css
--rw-r--r--   0 briford    (501) staff       (20)    10375 2024-04-16 15:58:18.000000 sageworks-0.6.5/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.6.5/applications/aws_dashboard/assets/trash.png
--rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-26 21:03:22.000000 sageworks-0.6.5/applications/aws_dashboard/dashboard
--rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.6.5/applications/aws_dashboard/nginx.conf
--rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.6.5/applications/aws_dashboard/open_source_config.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.942467 sageworks-0.6.5/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.955427 sageworks-0.6.5/applications/aws_dashboard/pages/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)    11700 2024-04-16 15:58:18.000000 sageworks-0.6.5/applications/aws_dashboard/pages/data_sources/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.6.5/applications/aws_dashboard/pages/data_sources/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.6.5/applications/aws_dashboard/pages/data_sources/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.955777 sageworks-0.6.5/applications/aws_dashboard/pages/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)     4212 2024-04-16 15:58:18.000000 sageworks-0.6.5/applications/aws_dashboard/pages/endpoints/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2677 2024-04-16 15:58:18.000000 sageworks-0.6.5/applications/aws_dashboard/pages/endpoints/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2458 2024-04-23 23:23:47.000000 sageworks-0.6.5/applications/aws_dashboard/pages/endpoints/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.956159 sageworks-0.6.5/applications/aws_dashboard/pages/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)    11614 2024-04-16 15:58:18.000000 sageworks-0.6.5/applications/aws_dashboard/pages/feature_sets/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.6.5/applications/aws_dashboard/pages/feature_sets/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.5/applications/aws_dashboard/pages/feature_sets/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.956270 sageworks-0.6.5/applications/aws_dashboard/pages/license/
--rw-r--r--   0 briford    (501) staff       (20)     1531 2024-05-19 19:25:10.000000 sageworks-0.6.5/applications/aws_dashboard/pages/license/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.956629 sageworks-0.6.5/applications/aws_dashboard/pages/main/
--rw-r--r--   0 briford    (501) staff       (20)     4899 2024-04-06 16:51:44.000000 sageworks-0.6.5/applications/aws_dashboard/pages/main/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     3307 2024-05-19 19:21:21.000000 sageworks-0.6.5/applications/aws_dashboard/pages/main/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.6.5/applications/aws_dashboard/pages/main/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.956975 sageworks-0.6.5/applications/aws_dashboard/pages/models/
--rw-r--r--   0 briford    (501) staff       (20)     3954 2024-04-23 23:23:47.000000 sageworks-0.6.5/applications/aws_dashboard/pages/models/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2234 2024-04-27 20:59:25.000000 sageworks-0.6.5/applications/aws_dashboard/pages/models/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2152 2024-04-23 23:23:47.000000 sageworks-0.6.5/applications/aws_dashboard/pages/models/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.957309 sageworks-0.6.5/applications/aws_dashboard/pages/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     1791 2024-04-26 21:07:33.000000 sageworks-0.6.5/applications/aws_dashboard/pages/pipelines/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2664 2024-04-26 20:07:24.000000 sageworks-0.6.5/applications/aws_dashboard/pages/pipelines/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1927 2024-04-26 21:04:41.000000 sageworks-0.6.5/applications/aws_dashboard/pages/pipelines/page.py
--rw-r--r--   0 briford    (501) staff       (20)      407 2024-05-19 21:33:27.000000 sageworks-0.6.5/applications/aws_dashboard/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.6.5/applications/aws_dashboard/supervisord.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.942587 sageworks-0.6.5/applications/experiments/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.957996 sageworks-0.6.5/applications/experiments/compound_explorer/
--rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.6.5/applications/experiments/compound_explorer/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.6.5/applications/experiments/compound_explorer/README.md
--rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-06 16:51:44.000000 sageworks-0.6.5/applications/experiments/compound_explorer/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.958246 sageworks-0.6.5/applications/experiments/compound_explorer/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.6.5/applications/experiments/compound_explorer/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.6.5/applications/experiments/compound_explorer/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     7678 2024-04-16 15:58:18.000000 sageworks-0.6.5/applications/experiments/compound_explorer/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.6.5/applications/experiments/compound_explorer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.6.5/applications/experiments/compound_explorer/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.958588 sageworks-0.6.5/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/aws_identity_check.py
--rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/build_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.958698 sageworks-0.6.5/aws_setup/event_bridge/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/event_bridge/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.959154 sageworks-0.6.5/aws_setup/event_bridge/dynamic_docker/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/event_bridge/dynamic_docker/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/event_bridge/dynamic_docker/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/event_bridge/dynamic_docker/cdk.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.959269 sageworks-0.6.5/aws_setup/event_bridge/dynamic_docker/lambda/
--rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.6.5/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
--rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.6.5/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.960045 sageworks-0.6.5/aws_setup/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_core/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_core/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/sageworks_core/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_core/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_core/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.6.5/aws_setup/sageworks_core/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.960261 sageworks-0.6.5/aws_setup/sageworks_core/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/aws_setup/sageworks_core/sageworks_core/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_core/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.960394 sageworks-0.6.5/aws_setup/sageworks_core/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_core/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.960579 sageworks-0.6.5/aws_setup/sageworks_core/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_core/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.961388 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.961605 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-24 21:53:47.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.961732 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.961928 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.962502 sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.962706 sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     6849 2024-05-19 20:45:52.000000 sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.963529 sageworks-0.6.5/data/
--rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.6.5/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.6.5/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.6.5/data/test_data.json
--rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.6.5/data/wine_dataset.csv
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.963711 sageworks-0.6.5/docs/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.964031 sageworks-0.6.5/docs/admin/
--rw-r--r--   0 briford    (501) staff       (20)     2176 2024-04-16 15:58:18.000000 sageworks-0.6.5/docs/admin/docker_push.md
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/admin/pypi_release.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.965216 sageworks-0.6.5/docs/api_classes/
--rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.6.5/docs/api_classes/data_source.md
--rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.6.5/docs/api_classes/endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.6.5/docs/api_classes/feature_set.md
--rw-r--r--   0 briford    (501) staff       (20)     5350 2024-04-06 16:51:44.000000 sageworks-0.6.5/docs/api_classes/meta.md
--rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/api_classes/model.md
--rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/api_classes/monitor.md
--rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/api_classes/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     4894 2024-04-19 15:50:50.000000 sageworks-0.6.5/docs/api_classes/pipelines.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.966204 sageworks-0.6.5/docs/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.6.5/docs/aws_setup/aws_access_management.md
--rw-r--r--   0 briford    (501) staff       (20)     5610 2024-05-06 14:50:56.000000 sageworks-0.6.5/docs/aws_setup/aws_tips_and_tricks.md
--rw-r--r--   0 briford    (501) staff       (20)     4210 2024-05-09 14:32:45.000000 sageworks-0.6.5/docs/aws_setup/core_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.6.5/docs/aws_setup/dashboard_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     7313 2024-05-15 23:47:50.000000 sageworks-0.6.5/docs/aws_setup/domain_cert_setup.md
--rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.6.5/docs/aws_setup/full_pipeline.md
--rw-r--r--   0 briford    (501) staff       (20)     3438 2024-05-09 14:20:27.000000 sageworks-0.6.5/docs/aws_setup/sso_setup.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.966343 sageworks-0.6.5/docs/concepts/
--rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.6.5/docs/concepts/model_monitoring.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.966488 sageworks-0.6.5/docs/core_classes/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.967620 sageworks-0.6.5/docs/core_classes/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.6.5/docs/core_classes/artifacts/artifact.md
--rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/artifacts/athena_source.md
--rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.6.5/docs/core_classes/artifacts/data_source_abstract.md
--rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/artifacts/endpoint_core.md
--rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/artifacts/feature_set_core.md
--rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/artifacts/model_core.md
--rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/artifacts/monitor_core.md
--rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/artifacts/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/overview.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.968678 sageworks-0.6.5/docs/core_classes/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/transforms/data_loaders_heavy.md
--rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/transforms/data_loaders_light.md
--rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.6.5/docs/core_classes/transforms/data_to_features.md
--rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/transforms/features_to_model.md
--rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/transforms/model_to_endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/core_classes/transforms/overview.md
--rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.6.5/docs/core_classes/transforms/pandas_transforms.md
--rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.6.5/docs/core_classes/transforms/transform.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.969085 sageworks-0.6.5/docs/enterprise/
--rw-r--r--   0 briford    (501) staff       (20)     4075 2024-04-28 19:13:56.000000 sageworks-0.6.5/docs/enterprise/index.md
--rw-r--r--   0 briford    (501) staff       (20)      786 2024-04-28 17:52:09.000000 sageworks-0.6.5/docs/enterprise/project_branding.md
--rw-r--r--   0 briford    (501) staff       (20)      892 2024-04-28 18:00:11.000000 sageworks-0.6.5/docs/enterprise/themes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.969202 sageworks-0.6.5/docs/getting_started/
--rw-r--r--   0 briford    (501) staff       (20)     1975 2024-05-09 14:38:45.000000 sageworks-0.6.5/docs/getting_started/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.969339 sageworks-0.6.5/docs/glue/
--rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.6.5/docs/glue/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.971622 sageworks-0.6.5/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.6.5/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.6.5/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.6.5/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.6.5/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.6.5/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.6.5/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.6.5/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.5/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.6.5/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.5/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.6.5/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)     3443 2024-05-09 14:20:27.000000 sageworks-0.6.5/docs/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.972312 sageworks-0.6.5/docs/misc/
--rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.6.5/docs/misc/faq.md
--rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/misc/general_info.md
--rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/misc/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.6.5/docs/misc/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.972559 sageworks-0.6.5/docs/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     3361 2024-04-16 15:58:18.000000 sageworks-0.6.5/docs/plugins/index.md
--rw-r--r--   0 briford    (501) staff       (20)      750 2024-04-06 16:51:44.000000 sageworks-0.6.5/docs/plugins/plugin_api_changes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.972679 sageworks-0.6.5/docs/repl/
--rw-r--r--   0 briford    (501) staff       (20)     2080 2024-05-09 14:40:59.000000 sageworks-0.6.5/docs/repl/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.972923 sageworks-0.6.5/docs/research/
--rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.6.5/docs/research/eda.md
--rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.6.5/docs/research/htg.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.973045 sageworks-0.6.5/examples/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.973159 sageworks-0.6.5/examples/ag-grid/
--rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-06 16:51:44.000000 sageworks-0.6.5/examples/ag-grid/hello_world.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.973734 sageworks-0.6.5/examples/datasource/
--rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.6.5/examples/datasource/datasource_from_df.py
--rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.6.5/examples/datasource/datasource_from_s3.py
--rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.6.5/examples/datasource/datasource_query.py
--rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.6.5/examples/datasource/datasource_stats.py
--rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.6.5/examples/datasource/datasource_to_featureset.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.974071 sageworks-0.6.5/examples/endpoint/
--rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.6.5/examples/endpoint/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/endpoint/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.6.5/examples/endpoint/endpoint_metrics.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.974422 sageworks-0.6.5/examples/featureset/
--rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.6.5/examples/featureset/featureset_eda.py
--rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/featureset/featureset_query.py
--rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.6.5/examples/featureset/featureset_to_model.py
--rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/full_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.974759 sageworks-0.6.5/examples/glue/
--rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.6.5/examples/glue/glue_hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.6.5/examples/glue/glue_hello_world_with_log.py
--rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.6.5/examples/glue/glue_load_s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.975102 sageworks-0.6.5/examples/meta/
--rw-r--r--   0 briford    (501) staff       (20)      363 2024-04-06 16:51:44.000000 sageworks-0.6.5/examples/meta/meta_list_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      328 2024-04-06 16:51:44.000000 sageworks-0.6.5/examples/meta/meta_list_models.py
--rw-r--r--   0 briford    (501) staff       (20)      659 2024-04-06 16:51:44.000000 sageworks-0.6.5/examples/meta/meta_model_metrics.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.975442 sageworks-0.6.5/examples/model/
--rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/model/model_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.6.5/examples/model/model_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      705 2024-05-08 21:58:54.000000 sageworks-0.6.5/examples/model/onboard_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.975678 sageworks-0.6.5/examples/monitor/
--rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.6.5/examples/monitor/monitor_setup.py
--rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.6.5/examples/monitor/monitor_usage.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.976380 sageworks-0.6.5/examples/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     1000 2024-04-19 14:53:32.000000 sageworks-0.6.5/examples/pipelines/abalone_pipeline_v1.json
--rw-r--r--   0 briford    (501) staff       (20)     1073 2024-04-19 19:42:10.000000 sageworks-0.6.5/examples/pipelines/abalone_pipeline_v2.json
--rw-r--r--   0 briford    (501) staff       (20)     4435 2024-04-20 17:35:29.000000 sageworks-0.6.5/examples/pipelines/aqsol_pipeline_v1.json
--rw-r--r--   0 briford    (501) staff       (20)      142 2024-04-19 14:55:38.000000 sageworks-0.6.5/examples/pipelines/pipeline_details.py
--rw-r--r--   0 briford    (501) staff       (20)      324 2024-04-19 14:55:38.000000 sageworks-0.6.5/examples/pipelines/pipeline_execute.py
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-04-19 14:51:51.000000 sageworks-0.6.5/examples/pipelines/pipeline_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.946264 sageworks-0.6.5/examples/plugins/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.976846 sageworks-0.6.5/examples/plugins/pages/
--rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-09 15:13:19.000000 sageworks-0.6.5/examples/plugins/pages/my_plugin_page.py
--rw-r--r--   0 briford    (501) staff       (20)     1635 2024-04-16 15:58:18.000000 sageworks-0.6.5/examples/plugins/pages/plugin_page_1.py
--rw-r--r--   0 briford    (501) staff       (20)     2464 2024-04-16 15:58:18.000000 sageworks-0.6.5/examples/plugins/pages/plugin_page_2.py
--rw-r--r--   0 briford    (501) staff       (20)     4528 2024-04-16 15:58:18.000000 sageworks-0.6.5/examples/plugins/pages/plugin_page_3.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.977092 sageworks-0.6.5/examples/plugins/views/
--rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-06 16:51:44.000000 sageworks-0.6.5/examples/plugins/views/model_plugin_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-06 16:51:44.000000 sageworks-0.6.5/examples/plugins/views/my_view_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.977674 sageworks-0.6.5/examples/plugins/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1733 2024-04-16 15:58:18.000000 sageworks-0.6.5/examples/plugins/web_components/custom_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-16 15:58:18.000000 sageworks-0.6.5/examples/plugins/web_components/endpoint_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     3660 2024-04-16 15:58:18.000000 sageworks-0.6.5/examples/plugins/web_components/endpoint_turbo.py
--rw-r--r--   0 briford    (501) staff       (20)     2596 2024-04-16 15:58:18.000000 sageworks-0.6.5/examples/plugins/web_components/model_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     2238 2024-04-16 15:58:18.000000 sageworks-0.6.5/examples/plugins/web_components/model_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.978251 sageworks-0.6.5/examples/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.6.5/examples/storage/data_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.6.5/examples/storage/data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/storage/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/storage/hello_world_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     4380 2024-04-16 15:58:18.000000 sageworks-0.6.5/examples/storage/plugin_page_example.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.978846 sageworks-0.6.5/examples/storage/sagemaker_pipelines/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/storage/sagemaker_pipelines/all_steps.py
--rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/storage/sagemaker_pipelines/hello.py
--rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/storage/sagemaker_pipelines/ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.946545 sageworks-0.6.5/examples/storage/sagemaker_pipelines/storage/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.979515 sageworks-0.6.5/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.6.5/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
--rw-r--r--   0 briford    (501) staff       (20)     3117 2024-05-15 16:07:08.000000 sageworks-0.6.5/mkdocs.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.980039 sageworks-0.6.5/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.6.5/notebooks/ML_Pipeline_with_SageWorks.ipynb
--rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.6.5/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
--rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.6.5/notebooks/Outliers_in_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.981609 sageworks-0.6.5/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.6.5/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.6.5/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.6.5/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.6.5/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.5/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.5/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      444 2024-05-19 21:32:59.000000 sageworks-0.6.5/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.982900 sageworks-0.6.5/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     1710 2024-04-16 15:58:18.000000 sageworks-0.6.5/scripts/ag_table_row_selection.py
--rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.6.5/scripts/athena_ddl_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.6.5/scripts/copy_data_catalog_db.py
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-04-16 15:58:18.000000 sageworks-0.6.5/scripts/create_glue_workflow_with_trigger.py
--rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.6.5/scripts/delete_redis_keys.py
--rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.6.5/scripts/glue_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.6.5/scripts/model_endpoint_sanity_check.py
--rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.6.5/scripts/onboard_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.6.5/scripts/onboard_models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.983143 sageworks-0.6.5/scripts/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.6.5/scripts/storage/dns_data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1723 2024-04-06 16:51:44.000000 sageworks-0.6.5/scripts/storage/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.6.5/scripts/test_feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)      533 2024-05-19 21:37:59.010703 sageworks-0.6.5/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.6.5/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.947030 sageworks-0.6.5/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.983260 sageworks-0.6.5/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.984060 sageworks-0.6.5/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.5/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.984938 sageworks-0.6.5/src/sageworks/algorithms/dataframe/
--rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.6.5/src/sageworks/algorithms/dataframe/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/dataframe/aggregation.py
--rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/dataframe/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
--rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/dataframe/feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/dataframe/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/dataframe/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.947371 sageworks-0.6.5/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.985062 sageworks-0.6.5/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.6.5/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.985177 sageworks-0.6.5/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.6.5/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.985295 sageworks-0.6.5/src/sageworks/algorithms/spark/
--rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.6.5/src/sageworks/algorithms/spark/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.986145 sageworks-0.6.5/src/sageworks/algorithms/sql/
--rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.6.5/src/sageworks/algorithms/sql/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/sql/column_stats.py
--rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/sql/correlations.py
--rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/sql/descriptive_stats.py
--rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/sql/outliers.py
--rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/sql/sample_rows.py
--rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/algorithms/sql/value_counts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.987418 sageworks-0.6.5/src/sageworks/api/
--rw-r--r--   0 briford    (501) staff       (20)      708 2024-04-18 20:46:23.000000 sageworks-0.6.5/src/sageworks/api/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/api/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/api/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/api/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)    16482 2024-04-21 15:28:58.000000 sageworks-0.6.5/src/sageworks/api/meta.py
--rw-r--r--   0 briford    (501) staff       (20)     2595 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/api/model.py
--rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/api/monitor.py
--rw-r--r--   0 briford    (501) staff       (20)     6953 2024-04-26 21:22:37.000000 sageworks-0.6.5/src/sageworks/api/pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     6659 2024-04-26 21:22:37.000000 sageworks-0.6.5/src/sageworks/api/pipeline_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.987729 sageworks-0.6.5/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)    11198 2024-05-09 14:32:45.000000 sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.989017 sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.989153 sageworks-0.6.5/src/sageworks/core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.990431 sageworks-0.6.5/src/sageworks/core/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    17938 2024-04-15 22:06:08.000000 sageworks-0.6.5/src/sageworks/core/artifacts/artifact.py
--rw-r--r--   0 briford    (501) staff       (20)    22432 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/core/artifacts/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/artifacts/data_source_abstract.py
--rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/artifacts/data_source_factory.py
--rw-r--r--   0 briford    (501) staff       (20)    36630 2024-04-21 18:44:59.000000 sageworks-0.6.5/src/sageworks/core/artifacts/endpoint_core.py
--rw-r--r--   0 briford    (501) staff       (20)    29698 2024-04-22 20:46:36.000000 sageworks-0.6.5/src/sageworks/core/artifacts/feature_set_core.py
--rw-r--r--   0 briford    (501) staff       (20)    37022 2024-05-19 19:25:11.000000 sageworks-0.6.5/src/sageworks/core/artifacts/model_core.py
--rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/artifacts/monitor_core.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.990569 sageworks-0.6.5/src/sageworks/core/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     6919 2024-04-26 21:22:37.000000 sageworks-0.6.5/src/sageworks/core/pipelines/pipeline_executor.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.990941 sageworks-0.6.5/src/sageworks/core/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.991082 sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.991333 sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.991875 sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.992017 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.992120 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.992220 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.992350 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.992705 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.992828 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.992930 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.993140 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/chunk/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.993286 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.993407 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.993534 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/storage/
--rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.993917 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     5674 2024-04-23 15:16:38.000000 sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.994054 sageworks-0.6.5/src/sageworks/core/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.949411 sageworks-0.6.5/src/sageworks/core/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.994157 sageworks-0.6.5/src/sageworks/core/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.994280 sageworks-0.6.5/src/sageworks/core/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.994504 sageworks-0.6.5/src/sageworks/core/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.994800 sageworks-0.6.5/src/sageworks/core/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.6.5/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.995076 sageworks-0.6.5/src/sageworks/core/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/core/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.995987 sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     8604 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)    18139 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
--rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/core/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.996149 sageworks-0.6.5/src/sageworks/experiments/
--rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/experiments/view_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.996443 sageworks-0.6.5/src/sageworks/repl/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/repl/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15486 2024-04-21 15:35:25.000000 sageworks-0.6.5/src/sageworks/repl/sageworks_shell.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:58.996749 sageworks-0.6.5/src/sageworks/resources/
--rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.6.5/src/sageworks/resources/open_source_api.key
--rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/resources/signature_verify_pub.pem
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.001512 sageworks-0.6.5/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.5/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15587 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/utils/aws_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5447 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/chem_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    16543 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/utils/config_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/dashboard_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     4194 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/utils/datetime_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/docker_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.6.5/src/sageworks/utils/ecs_info.py
--rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/endpoint_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/endpoint_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/extract_model_artifact.py
--rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/glue_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6396 2024-05-19 19:25:10.000000 sageworks-0.6.5/src/sageworks/utils/license_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     1439 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/utils/markdown_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    15517 2024-04-22 20:45:19.000000 sageworks-0.6.5/src/sageworks/utils/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    12684 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/utils/plugin_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     9533 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/repl_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/s3_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/sageworks_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/sageworks_sqs.py
--rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.6.5/src/sageworks/utils/symbols.py
--rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/test_data_generator.py
--rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.6.5/src/sageworks/utils/trace_calls.py
--rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/utils/type_abbrev.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.002351 sageworks-0.6.5/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)     3517 2024-04-16 22:29:17.000000 sageworks-0.6.5/src/sageworks/views/artifacts_text_view.py
--rw-r--r--   0 briford    (501) staff       (20)     7780 2024-04-28 17:17:45.000000 sageworks-0.6.5/src/sageworks/views/artifacts_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3158 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/views/data_source_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2150 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/views/endpoint_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3206 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/views/feature_set_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/views/model_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.004039 sageworks-0.6.5/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     5916 2024-04-25 23:06:38.000000 sageworks-0.6.5/src/sageworks/web_components/component_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3525 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     5854 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/correlation_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/web_components/data_details_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     4558 2024-04-06 16:51:44.000000 sageworks-0.6.5/src/sageworks/web_components/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)     3068 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/endpoint_metric_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.005098 sageworks-0.6.5/src/sageworks/web_components/experiments/
--rw-r--r--   0 briford    (501) staff       (20)      837 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/experiments/color_maps.py
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/web_components/experiments/compound_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2974 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/experiments/dashboard_metric_plots.py
--rw-r--r--   0 briford    (501) staff       (20)     2240 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/experiments/data_table.py
--rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/web_components/experiments/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)      838 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/experiments/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/web_components/experiments/outlier_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2373 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/experiments/plugin_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.6.5/src/sageworks/web_components/experiments/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     8690 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2278 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/model_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     7191 2024-05-19 17:03:46.000000 sageworks-0.6.5/src/sageworks/web_components/plugin_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3530 2024-04-25 23:09:25.000000 sageworks-0.6.5/src/sageworks/web_components/plugin_unit_test.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.005596 sageworks-0.6.5/src/sageworks/web_components/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     2786 2024-04-26 21:04:42.000000 sageworks-0.6.5/src/sageworks/web_components/plugins/ag_table.py
--rw-r--r--   0 briford    (501) staff       (20)     4058 2024-05-19 19:25:10.000000 sageworks-0.6.5/src/sageworks/web_components/plugins/license_details.py
--rw-r--r--   0 briford    (501) staff       (20)     9653 2024-04-15 13:43:00.000000 sageworks-0.6.5/src/sageworks/web_components/plugins/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2429 2024-04-26 21:22:37.000000 sageworks-0.6.5/src/sageworks/web_components/plugins/pipeline_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2945 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/regression_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     6838 2024-05-06 17:24:24.000000 sageworks-0.6.5/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     5185 2024-04-16 15:58:18.000000 sageworks-0.6.5/src/sageworks/web_components/violin_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.009887 sageworks-0.6.5/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     4961 2024-05-19 21:37:58.000000 sageworks-0.6.5/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)    19102 2024-05-19 21:37:58.000000 sageworks-0.6.5/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2024-05-19 21:37:58.000000 sageworks-0.6.5/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)       74 2024-05-19 21:37:58.000000 sageworks-0.6.5/src/sageworks.egg-info/entry_points.txt
--rw-r--r--   0 briford    (501) staff       (20)      421 2024-05-19 21:37:58.000000 sageworks-0.6.5/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2024-05-19 21:37:58.000000 sageworks-0.6.5/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.006375 sageworks-0.6.5/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.006872 sageworks-0.6.5/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.6.5/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.007107 sageworks-0.6.5/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.6.5/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.6.5/tests/aws_account/aws_service_broker_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.007810 sageworks-0.6.5/tests/connectors/
--rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/connectors/s3_bucket.py
--rw-r--r--   0 briford    (501) staff       (20)     5618 2024-04-26 21:04:42.000000 sageworks-0.6.5/tests/create_aqsol_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/create_basic_test_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/create_realtime_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     2378 2024-04-22 20:46:36.000000 sageworks-0.6.5/tests/create_training_adjusted_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/create_wine_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     4448 2024-04-16 15:58:18.000000 sageworks-0.6.5/tests/delete_test_artifacts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.007926 sageworks-0.6.5/tests/plugin_tests/
--rw-r--r--   0 briford    (501) staff       (20)     1885 2024-04-16 15:58:18.000000 sageworks-0.6.5/tests/plugin_tests/crashing_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.008158 sageworks-0.6.5/tests/specific/
--rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/specific/capital_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/specific/deletion_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.008859 sageworks-0.6.5/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     5142 2024-04-20 00:25:37.000000 sageworks-0.6.5/tests/transforms/model_metrics_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.6.5/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.6.5/tests/transforms/pandas_to_data_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.009227 sageworks-0.6.5/tests/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      681 2024-04-16 15:58:18.000000 sageworks-0.6.5/tests/web_components/confusion_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)      677 2024-04-16 15:58:18.000000 sageworks-0.6.5/tests/web_components/correlation_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)     5269 2024-04-16 15:58:18.000000 sageworks-0.6.5/tests/web_components/plugin_interface_test.py
--rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.6.5/tox.ini
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.009595 sageworks-0.6.5/ui_testing/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-19 21:37:59.009712 sageworks-0.6.5/ui_testing/assets/
--rw-r--r--   0 briford    (501) staff       (20)      597 2024-05-13 15:14:49.000000 sageworks-0.6.5/ui_testing/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)     5770 2024-05-19 19:25:10.000000 sageworks-0.6.5/ui_testing/table_comparison.py
--rw-r--r--   0 briford    (501) staff       (20)     2025 2024-05-19 19:25:10.000000 sageworks-0.6.5/ui_testing/theme_switching.py
--rw-r--r--   0 briford    (501) staff       (20)     1819 2024-05-19 19:25:10.000000 sageworks-0.6.5/ui_testing/theme_switching_2.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.850116 sageworks-0.6.6/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.756734 sageworks-0.6.6/.github/
+-rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.6.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.6.6/.github/dependabot.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.757215 sageworks-0.6.6/.github/workflows/
+-rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.6.6/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.6.6/.github/workflows/python-lint.yml
+-rw-r--r--   0 briford    (501) staff       (20)     2037 2024-05-15 21:28:12.000000 sageworks-0.6.6/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      791 2024-04-16 15:58:18.000000 sageworks-0.6.6/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.6.6/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.6.6/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.6.6/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     4961 2024-05-24 14:49:47.850048 sageworks-0.6.6/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     3510 2024-05-09 14:32:45.000000 sageworks-0.6.6/README.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.6.6/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.745838 sageworks-0.6.6/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.759456 sageworks-0.6.6/applications/aws_dashboard/
+-rw-r--r--   0 briford    (501) staff       (20)     1071 2024-05-19 21:38:50.000000 sageworks-0.6.6/applications/aws_dashboard/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/Dockerfile_plugins
+-rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.6.6/applications/aws_dashboard/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-09 14:37:33.000000 sageworks-0.6.6/applications/aws_dashboard/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.761005 sageworks-0.6.6/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-06 16:51:44.000000 sageworks-0.6.6/applications/aws_dashboard/assets/bootstrap_darkly.min.css
+-rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-06 16:51:44.000000 sageworks-0.6.6/applications/aws_dashboard/assets/default.css
+-rw-r--r--   0 briford    (501) staff       (20)    10375 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/aws_dashboard/assets/trash.png
+-rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-26 21:03:22.000000 sageworks-0.6.6/applications/aws_dashboard/dashboard
+-rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/aws_dashboard/nginx.conf
+-rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/open_source_config.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.745762 sageworks-0.6.6/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.761625 sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)    11700 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.762328 sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)     4212 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2677 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2458 2024-04-23 23:23:47.000000 sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.763023 sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)    11614 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.763294 sageworks-0.6.6/applications/aws_dashboard/pages/license/
+-rw-r--r--   0 briford    (501) staff       (20)     1531 2024-05-19 19:25:10.000000 sageworks-0.6.6/applications/aws_dashboard/pages/license/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.764003 sageworks-0.6.6/applications/aws_dashboard/pages/main/
+-rw-r--r--   0 briford    (501) staff       (20)     4899 2024-04-06 16:51:44.000000 sageworks-0.6.6/applications/aws_dashboard/pages/main/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     3307 2024-05-19 19:21:21.000000 sageworks-0.6.6/applications/aws_dashboard/pages/main/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/aws_dashboard/pages/main/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.764647 sageworks-0.6.6/applications/aws_dashboard/pages/models/
+-rw-r--r--   0 briford    (501) staff       (20)     3954 2024-04-23 23:23:47.000000 sageworks-0.6.6/applications/aws_dashboard/pages/models/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2234 2024-04-27 20:59:25.000000 sageworks-0.6.6/applications/aws_dashboard/pages/models/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2152 2024-04-23 23:23:47.000000 sageworks-0.6.6/applications/aws_dashboard/pages/models/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.765349 sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     1791 2024-04-26 21:07:33.000000 sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2664 2024-04-26 20:07:24.000000 sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1927 2024-04-26 21:04:41.000000 sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/page.py
+-rw-r--r--   0 briford    (501) staff       (20)      407 2024-05-19 21:33:27.000000 sageworks-0.6.6/applications/aws_dashboard/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/aws_dashboard/supervisord.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.745891 sageworks-0.6.6/applications/experiments/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.766707 sageworks-0.6.6/applications/experiments/compound_explorer/
+-rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/experiments/compound_explorer/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/experiments/compound_explorer/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-06 16:51:44.000000 sageworks-0.6.6/applications/experiments/compound_explorer/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.767195 sageworks-0.6.6/applications/experiments/compound_explorer/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/experiments/compound_explorer/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/experiments/compound_explorer/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     7678 2024-04-16 15:58:18.000000 sageworks-0.6.6/applications/experiments/compound_explorer/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.6.6/applications/experiments/compound_explorer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.6.6/applications/experiments/compound_explorer/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.767681 sageworks-0.6.6/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/aws_identity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.767826 sageworks-0.6.6/aws_setup/event_bridge/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/event_bridge/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.768483 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/cdk.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.768713 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/lambda/
+-rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
+-rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.769881 sageworks-0.6.6/aws_setup/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_core/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.6.6/aws_setup/sageworks_core/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.770161 sageworks-0.6.6/aws_setup/sageworks_core/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/aws_setup/sageworks_core/sageworks_core/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.770504 sageworks-0.6.6/aws_setup/sageworks_core/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.770702 sageworks-0.6.6/aws_setup/sageworks_core/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.771961 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.772209 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-24 21:53:47.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.772559 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.772773 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.773605 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.773848 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     6849 2024-05-19 21:59:13.000000 sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.775137 sageworks-0.6.6/data/
+-rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.6.6/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.6.6/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.6.6/data/test_data.json
+-rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.6.6/data/wine_dataset.csv
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.775398 sageworks-0.6.6/docs/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.775639 sageworks-0.6.6/docs/admin/
+-rw-r--r--   0 briford    (501) staff       (20)     2176 2024-04-16 15:58:18.000000 sageworks-0.6.6/docs/admin/docker_push.md
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/admin/pypi_release.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.776778 sageworks-0.6.6/docs/api_classes/
+-rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/api_classes/data_source.md
+-rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/api_classes/endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/api_classes/feature_set.md
+-rw-r--r--   0 briford    (501) staff       (20)     5350 2024-04-06 16:51:44.000000 sageworks-0.6.6/docs/api_classes/meta.md
+-rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/api_classes/model.md
+-rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/api_classes/monitor.md
+-rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/api_classes/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     4894 2024-04-19 15:50:50.000000 sageworks-0.6.6/docs/api_classes/pipelines.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.777785 sageworks-0.6.6/docs/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/aws_setup/aws_access_management.md
+-rw-r--r--   0 briford    (501) staff       (20)     5610 2024-05-06 14:50:56.000000 sageworks-0.6.6/docs/aws_setup/aws_tips_and_tricks.md
+-rw-r--r--   0 briford    (501) staff       (20)     4210 2024-05-09 14:32:45.000000 sageworks-0.6.6/docs/aws_setup/core_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/aws_setup/dashboard_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     7313 2024-05-15 23:47:50.000000 sageworks-0.6.6/docs/aws_setup/domain_cert_setup.md
+-rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/aws_setup/full_pipeline.md
+-rw-r--r--   0 briford    (501) staff       (20)     3438 2024-05-09 14:20:27.000000 sageworks-0.6.6/docs/aws_setup/sso_setup.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.778289 sageworks-0.6.6/docs/blogs_research/
+-rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/blogs_research/eda.md
+-rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/blogs_research/htg.md
+-rw-r--r--   0 briford    (501) staff       (20)      802 2024-05-21 22:30:34.000000 sageworks-0.6.6/docs/blogs_research/index.md
+-rw-r--r--   0 briford    (501) staff       (20)     1245 2024-05-21 22:34:16.000000 sageworks-0.6.6/docs/blogs_research/residual_analysis.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.778412 sageworks-0.6.6/docs/concepts/
+-rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/concepts/model_monitoring.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.778545 sageworks-0.6.6/docs/core_classes/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.779545 sageworks-0.6.6/docs/core_classes/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/core_classes/artifacts/artifact.md
+-rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/athena_source.md
+-rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/core_classes/artifacts/data_source_abstract.md
+-rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/endpoint_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/feature_set_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/model_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/monitor_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/artifacts/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/overview.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.780612 sageworks-0.6.6/docs/core_classes/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/transforms/data_loaders_heavy.md
+-rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/transforms/data_loaders_light.md
+-rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/core_classes/transforms/data_to_features.md
+-rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/transforms/features_to_model.md
+-rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/transforms/model_to_endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/core_classes/transforms/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/core_classes/transforms/pandas_transforms.md
+-rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.6.6/docs/core_classes/transforms/transform.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.781002 sageworks-0.6.6/docs/enterprise/
+-rw-r--r--   0 briford    (501) staff       (20)     4075 2024-05-20 20:55:48.000000 sageworks-0.6.6/docs/enterprise/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      786 2024-04-28 17:52:09.000000 sageworks-0.6.6/docs/enterprise/project_branding.md
+-rw-r--r--   0 briford    (501) staff       (20)      892 2024-04-28 18:00:11.000000 sageworks-0.6.6/docs/enterprise/themes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.781138 sageworks-0.6.6/docs/getting_started/
+-rw-r--r--   0 briford    (501) staff       (20)     1975 2024-05-09 14:38:45.000000 sageworks-0.6.6/docs/getting_started/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.781267 sageworks-0.6.6/docs/glue/
+-rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/glue/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.783544 sageworks-0.6.6/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.6.6/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)     3443 2024-05-09 14:20:27.000000 sageworks-0.6.6/docs/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.784371 sageworks-0.6.6/docs/misc/
+-rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.6.6/docs/misc/faq.md
+-rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/misc/general_info.md
+-rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/misc/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.6.6/docs/misc/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.784679 sageworks-0.6.6/docs/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     3361 2024-04-16 15:58:18.000000 sageworks-0.6.6/docs/plugins/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      750 2024-04-06 16:51:44.000000 sageworks-0.6.6/docs/plugins/plugin_api_changes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.784820 sageworks-0.6.6/docs/repl/
+-rw-r--r--   0 briford    (501) staff       (20)     2080 2024-05-09 14:40:59.000000 sageworks-0.6.6/docs/repl/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.784956 sageworks-0.6.6/examples/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.785118 sageworks-0.6.6/examples/ag-grid/
+-rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/ag-grid/hello_world.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.786603 sageworks-0.6.6/examples/datasource/
+-rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/datasource/datasource_from_df.py
+-rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/datasource/datasource_from_s3.py
+-rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.6.6/examples/datasource/datasource_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.6.6/examples/datasource/datasource_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/datasource/datasource_to_featureset.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.787256 sageworks-0.6.6/examples/endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/endpoint/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/endpoint/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/endpoint/endpoint_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.787783 sageworks-0.6.6/examples/featureset/
+-rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/featureset/featureset_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/featureset/featureset_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.6.6/examples/featureset/featureset_to_model.py
+-rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/full_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.788612 sageworks-0.6.6/examples/glue/
+-rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.6.6/examples/glue/glue_hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.6.6/examples/glue/glue_hello_world_with_log.py
+-rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.6.6/examples/glue/glue_load_s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.789137 sageworks-0.6.6/examples/meta/
+-rw-r--r--   0 briford    (501) staff       (20)      363 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/meta/meta_list_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      328 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/meta/meta_list_models.py
+-rw-r--r--   0 briford    (501) staff       (20)      659 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/meta/meta_model_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.789623 sageworks-0.6.6/examples/model/
+-rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/model/model_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.6.6/examples/model/model_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      705 2024-05-08 21:58:54.000000 sageworks-0.6.6/examples/model/onboard_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.790100 sageworks-0.6.6/examples/monitor/
+-rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/monitor/monitor_setup.py
+-rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.6.6/examples/monitor/monitor_usage.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.791627 sageworks-0.6.6/examples/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     1000 2024-04-19 14:53:32.000000 sageworks-0.6.6/examples/pipelines/abalone_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)     1073 2024-04-19 19:42:10.000000 sageworks-0.6.6/examples/pipelines/abalone_pipeline_v2.json
+-rw-r--r--   0 briford    (501) staff       (20)     4435 2024-04-20 17:35:29.000000 sageworks-0.6.6/examples/pipelines/aqsol_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)      142 2024-04-19 14:55:38.000000 sageworks-0.6.6/examples/pipelines/pipeline_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      324 2024-04-19 14:55:38.000000 sageworks-0.6.6/examples/pipelines/pipeline_execute.py
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-04-19 14:51:51.000000 sageworks-0.6.6/examples/pipelines/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.749192 sageworks-0.6.6/examples/plugins/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.792517 sageworks-0.6.6/examples/plugins/pages/
+-rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-09 15:13:19.000000 sageworks-0.6.6/examples/plugins/pages/my_plugin_page.py
+-rw-r--r--   0 briford    (501) staff       (20)     1635 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/pages/plugin_page_1.py
+-rw-r--r--   0 briford    (501) staff       (20)     2464 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/pages/plugin_page_2.py
+-rw-r--r--   0 briford    (501) staff       (20)     4528 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/pages/plugin_page_3.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.792998 sageworks-0.6.6/examples/plugins/views/
+-rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/plugins/views/model_plugin_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-06 16:51:44.000000 sageworks-0.6.6/examples/plugins/views/my_view_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.793724 sageworks-0.6.6/examples/plugins/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1733 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/web_components/custom_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/web_components/endpoint_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     3660 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/web_components/endpoint_turbo.py
+-rw-r--r--   0 briford    (501) staff       (20)     2596 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/web_components/model_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     2238 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/plugins/web_components/model_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.794755 sageworks-0.6.6/examples/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.6.6/examples/storage/data_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.6.6/examples/storage/data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/hello_world_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     4380 2024-04-16 15:58:18.000000 sageworks-0.6.6/examples/storage/plugin_page_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.795265 sageworks-0.6.6/examples/storage/sagemaker_pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/all_steps.py
+-rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/hello.py
+-rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.749452 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.796022 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     3285 2024-05-24 14:48:45.000000 sageworks-0.6.6/mkdocs.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.797039 sageworks-0.6.6/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.6.6/notebooks/ML_Pipeline_with_SageWorks.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.6.6/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.6.6/notebooks/Outliers_in_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.805949 sageworks-0.6.6/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.6/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      444 2024-05-19 21:32:59.000000 sageworks-0.6.6/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.810059 sageworks-0.6.6/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1710 2024-04-16 15:58:18.000000 sageworks-0.6.6/scripts/ag_table_row_selection.py
+-rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/athena_ddl_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.6.6/scripts/copy_data_catalog_db.py
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-04-16 15:58:18.000000 sageworks-0.6.6/scripts/create_glue_workflow_with_trigger.py
+-rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.6.6/scripts/delete_redis_keys.py
+-rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/glue_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/model_endpoint_sanity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/onboard_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/onboard_models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.810461 sageworks-0.6.6/scripts/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.6.6/scripts/storage/dns_data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1723 2024-04-06 16:51:44.000000 sageworks-0.6.6/scripts/storage/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.6.6/scripts/test_feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)      533 2024-05-24 14:49:47.850506 sageworks-0.6.6/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.6.6/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.749906 sageworks-0.6.6/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.810696 sageworks-0.6.6/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.811578 sageworks-0.6.6/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.813264 sageworks-0.6.6/src/sageworks/algorithms/dataframe/
+-rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/aggregation.py
+-rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
+-rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/dataframe/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.750223 sageworks-0.6.6/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.813540 sageworks-0.6.6/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.813745 sageworks-0.6.6/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.813951 sageworks-0.6.6/src/sageworks/algorithms/spark/
+-rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/spark/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.815560 sageworks-0.6.6/src/sageworks/algorithms/sql/
+-rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/column_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/correlations.py
+-rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/descriptive_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/outliers.py
+-rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/sample_rows.py
+-rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/algorithms/sql/value_counts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.816844 sageworks-0.6.6/src/sageworks/api/
+-rw-r--r--   0 briford    (501) staff       (20)      708 2024-04-18 20:46:23.000000 sageworks-0.6.6/src/sageworks/api/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/api/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/api/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/api/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)    16482 2024-04-21 15:28:58.000000 sageworks-0.6.6/src/sageworks/api/meta.py
+-rw-r--r--   0 briford    (501) staff       (20)     2595 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/api/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/api/monitor.py
+-rw-r--r--   0 briford    (501) staff       (20)     6953 2024-04-26 21:22:37.000000 sageworks-0.6.6/src/sageworks/api/pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     6659 2024-04-26 21:22:37.000000 sageworks-0.6.6/src/sageworks/api/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.817440 sageworks-0.6.6/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)    11198 2024-05-09 14:32:45.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.819044 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.819202 sageworks-0.6.6/src/sageworks/core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.820515 sageworks-0.6.6/src/sageworks/core/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    17938 2024-04-15 22:06:08.000000 sageworks-0.6.6/src/sageworks/core/artifacts/artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)    22432 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/core/artifacts/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/artifacts/data_source_abstract.py
+-rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/artifacts/data_source_factory.py
+-rw-r--r--   0 briford    (501) staff       (20)    36630 2024-04-21 18:44:59.000000 sageworks-0.6.6/src/sageworks/core/artifacts/endpoint_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    29698 2024-04-22 20:46:36.000000 sageworks-0.6.6/src/sageworks/core/artifacts/feature_set_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    37022 2024-05-19 19:25:11.000000 sageworks-0.6.6/src/sageworks/core/artifacts/model_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/artifacts/monitor_core.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.820665 sageworks-0.6.6/src/sageworks/core/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     6919 2024-04-26 21:22:37.000000 sageworks-0.6.6/src/sageworks/core/pipelines/pipeline_executor.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.821340 sageworks-0.6.6/src/sageworks/core/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.821506 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.821735 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.822300 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.822449 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.822557 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.822654 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.822909 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.823282 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.823407 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.823516 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.823722 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/chunk/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.823877 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.824028 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.824176 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.824816 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     5674 2024-04-23 15:16:38.000000 sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.824970 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.752371 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.825072 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.825222 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.825462 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.825833 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.826367 sageworks-0.6.6/src/sageworks/core/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/core/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.827223 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     8604 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    18139 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
+-rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/core/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.827547 sageworks-0.6.6/src/sageworks/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/experiments/view_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.828306 sageworks-0.6.6/src/sageworks/repl/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/repl/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15486 2024-04-21 15:35:25.000000 sageworks-0.6.6/src/sageworks/repl/sageworks_shell.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.828733 sageworks-0.6.6/src/sageworks/resources/
+-rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.6.6/src/sageworks/resources/open_source_api.key
+-rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/resources/signature_verify_pub.pem
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.833179 sageworks-0.6.6/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.6/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15587 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/utils/aws_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5447 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/chem_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    16543 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/utils/config_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/dashboard_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     4194 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/utils/datetime_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/docker_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.6.6/src/sageworks/utils/ecs_info.py
+-rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/endpoint_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/endpoint_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/extract_model_artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/glue_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6404 2024-05-20 15:33:17.000000 sageworks-0.6.6/src/sageworks/utils/license_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     1439 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/utils/markdown_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    15517 2024-04-22 20:45:19.000000 sageworks-0.6.6/src/sageworks/utils/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    12684 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/utils/plugin_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     9533 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/repl_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/s3_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/sageworks_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/sageworks_sqs.py
+-rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.6.6/src/sageworks/utils/symbols.py
+-rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/test_data_generator.py
+-rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.6.6/src/sageworks/utils/trace_calls.py
+-rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/utils/type_abbrev.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.834691 sageworks-0.6.6/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)     3517 2024-04-16 22:29:17.000000 sageworks-0.6.6/src/sageworks/views/artifacts_text_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     7780 2024-04-28 17:17:45.000000 sageworks-0.6.6/src/sageworks/views/artifacts_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3158 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/views/data_source_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2150 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/views/endpoint_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3206 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/views/feature_set_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/views/model_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.838397 sageworks-0.6.6/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     5916 2024-04-25 23:06:38.000000 sageworks-0.6.6/src/sageworks/web_components/component_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3525 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     5854 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/correlation_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/web_components/data_details_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     4558 2024-04-06 16:51:44.000000 sageworks-0.6.6/src/sageworks/web_components/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     3068 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/endpoint_metric_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.840723 sageworks-0.6.6/src/sageworks/web_components/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)      837 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/color_maps.py
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/compound_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2974 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/dashboard_metric_plots.py
+-rw-r--r--   0 briford    (501) staff       (20)     2240 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/data_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      838 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/outlier_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2373 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/plugin_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.6.6/src/sageworks/web_components/experiments/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     8690 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2278 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/model_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     7191 2024-05-19 17:03:46.000000 sageworks-0.6.6/src/sageworks/web_components/plugin_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3530 2024-04-25 23:09:25.000000 sageworks-0.6.6/src/sageworks/web_components/plugin_unit_test.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.841875 sageworks-0.6.6/src/sageworks/web_components/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     2786 2024-04-26 21:04:42.000000 sageworks-0.6.6/src/sageworks/web_components/plugins/ag_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     5498 2024-05-22 14:54:18.000000 sageworks-0.6.6/src/sageworks/web_components/plugins/license_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     9653 2024-04-15 13:43:00.000000 sageworks-0.6.6/src/sageworks/web_components/plugins/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2429 2024-04-26 21:22:37.000000 sageworks-0.6.6/src/sageworks/web_components/plugins/pipeline_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2945 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/regression_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     6838 2024-05-06 17:24:24.000000 sageworks-0.6.6/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     5185 2024-04-16 15:58:18.000000 sageworks-0.6.6/src/sageworks/web_components/violin_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.849595 sageworks-0.6.6/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     4961 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)    19184 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)       74 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/entry_points.txt
+-rw-r--r--   0 briford    (501) staff       (20)      421 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2024-05-24 14:49:47.000000 sageworks-0.6.6/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.843256 sageworks-0.6.6/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.844093 sageworks-0.6.6/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.6.6/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.844492 sageworks-0.6.6/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.6.6/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.6.6/tests/aws_account/aws_service_broker_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.845681 sageworks-0.6.6/tests/connectors/
+-rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/connectors/s3_bucket.py
+-rw-r--r--   0 briford    (501) staff       (20)     5618 2024-04-26 21:04:42.000000 sageworks-0.6.6/tests/create_aqsol_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/create_basic_test_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/create_realtime_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     2378 2024-04-22 20:46:36.000000 sageworks-0.6.6/tests/create_training_adjusted_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/create_wine_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     4448 2024-04-16 15:58:18.000000 sageworks-0.6.6/tests/delete_test_artifacts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.845849 sageworks-0.6.6/tests/plugin_tests/
+-rw-r--r--   0 briford    (501) staff       (20)     1885 2024-04-16 15:58:18.000000 sageworks-0.6.6/tests/plugin_tests/crashing_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.846157 sageworks-0.6.6/tests/specific/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/specific/capital_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/specific/deletion_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.847542 sageworks-0.6.6/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     5142 2024-04-20 00:25:37.000000 sageworks-0.6.6/tests/transforms/model_metrics_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.6.6/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.6.6/tests/transforms/pandas_to_data_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.848096 sageworks-0.6.6/tests/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      681 2024-04-16 15:58:18.000000 sageworks-0.6.6/tests/web_components/confusion_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      677 2024-04-16 15:58:18.000000 sageworks-0.6.6/tests/web_components/correlation_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     5269 2024-04-16 15:58:18.000000 sageworks-0.6.6/tests/web_components/plugin_interface_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.6.6/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.848945 sageworks-0.6.6/ui_testing/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-24 14:49:47.849183 sageworks-0.6.6/ui_testing/assets/
+-rw-r--r--   0 briford    (501) staff       (20)      597 2024-05-13 15:14:49.000000 sageworks-0.6.6/ui_testing/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)     5770 2024-05-19 19:25:10.000000 sageworks-0.6.6/ui_testing/table_comparison.py
+-rw-r--r--   0 briford    (501) staff       (20)     2025 2024-05-19 19:25:10.000000 sageworks-0.6.6/ui_testing/theme_switching.py
+-rw-r--r--   0 briford    (501) staff       (20)     1819 2024-05-19 19:25:10.000000 sageworks-0.6.6/ui_testing/theme_switching_2.py
```

### Comparing `sageworks-0.6.5/.github/PULL_REQUEST_TEMPLATE.md` & `sageworks-0.6.6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/.github/workflows/deploy-docs.yml` & `sageworks-0.6.6/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/.github/workflows/python-lint.yml` & `sageworks-0.6.6/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/.gitignore` & `sageworks-0.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/CONTRIBUTING.md` & `sageworks-0.6.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/LICENSE` & `sageworks-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/Makefile` & `sageworks-0.6.6/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/PKG-INFO` & `sageworks-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.6.5
+Version: 0.6.6
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sageworks-0.6.5/README.md` & `sageworks-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/Dockerfile` & `sageworks-0.6.6/applications/aws_dashboard/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 RUN pip install --no-cache-dir -r requirements.txt
 
 # Copy the Nginx and Supervisor configuration files
 COPY nginx.conf /etc/nginx/sites-available/default
 COPY supervisord.conf /etc/supervisor/conf.d/supervisord.conf
 
 # Install Sageworks (changes often)
-RUN pip install --no-cache-dir sageworks==0.6.3
+RUN pip install --no-cache-dir sageworks==0.6.5
 
 # Copy the current directory contents into the container at /app
 COPY . /app
 
 # Grab the config file from build args, copy, and set ENV var
 ARG SAGEWORKS_CONFIG
 COPY $SAGEWORKS_CONFIG /app/sageworks_config.json
```

### Comparing `sageworks-0.6.5/applications/aws_dashboard/README.md` & `sageworks-0.6.6/applications/aws_dashboard/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/app.py` & `sageworks-0.6.6/applications/aws_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/assets/bootstrap_darkly.min.css` & `sageworks-0.6.6/applications/aws_dashboard/assets/bootstrap_darkly.min.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/assets/default.css` & `sageworks-0.6.6/applications/aws_dashboard/assets/default.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/assets/favicon.ico` & `sageworks-0.6.6/applications/aws_dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/assets/trash.png` & `sageworks-0.6.6/applications/aws_dashboard/assets/trash.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/dashboard` & `sageworks-0.6.6/applications/aws_dashboard/dashboard`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/open_source_config.json` & `sageworks-0.6.6/applications/aws_dashboard/open_source_config.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/data_sources/callbacks.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/data_sources/layout.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/data_sources/page.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/data_sources/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/endpoints/callbacks.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/endpoints/layout.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/endpoints/page.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/endpoints/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/feature_sets/callbacks.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/feature_sets/layout.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/feature_sets/page.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/feature_sets/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/license/page.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/license/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/main/callbacks.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/main/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/main/layout.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/main/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/main/page.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/main/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/models/callbacks.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/models/layout.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/models/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/models/page.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/models/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/pipelines/callbacks.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/pipelines/layout.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/aws_dashboard/pages/pipelines/page.py` & `sageworks-0.6.6/applications/aws_dashboard/pages/pipelines/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/experiments/compound_explorer/app.py` & `sageworks-0.6.6/applications/experiments/compound_explorer/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/experiments/compound_explorer/assets/custom.css` & `sageworks-0.6.6/applications/experiments/compound_explorer/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/experiments/compound_explorer/callbacks.py` & `sageworks-0.6.6/applications/experiments/compound_explorer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/applications/experiments/compound_explorer/layout.py` & `sageworks-0.6.6/applications/experiments/compound_explorer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/aws_account_check.py` & `sageworks-0.6.6/aws_setup/aws_account_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/aws_identity_check.py` & `sageworks-0.6.6/aws_setup/aws_identity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/build_ml_pipeline.py` & `sageworks-0.6.6/aws_setup/build_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/event_bridge/dynamic_docker/app.py` & `sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/event_bridge/dynamic_docker/cdk.json` & `sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py` & `sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py` & `sageworks-0.6.6/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_core/README.md` & `sageworks-0.6.6/aws_setup/sageworks_core/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_core/app.py` & `sageworks-0.6.6/aws_setup/sageworks_core/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_core/cdk.json` & `sageworks-0.6.6/aws_setup/sageworks_core/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py` & `sageworks-0.6.6/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.6.6/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_dashboard_full/README.md` & `sageworks-0.6.6/aws_setup/sageworks_dashboard_full/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_dashboard_full/app.py` & `sageworks-0.6.6/aws_setup/sageworks_dashboard_full/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_dashboard_full/cdk.json` & `sageworks-0.6.6/aws_setup/sageworks_dashboard_full/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py` & `sageworks-0.6.6/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py` & `sageworks-0.6.6/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/README.md` & `sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/app.py` & `sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/cdk.json` & `sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py` & `sageworks-0.6.6/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     aws_logs as logs,
 )
 from aws_cdk.aws_certificatemanager import Certificate
 from aws_cdk.aws_ecs_patterns import ApplicationLoadBalancedFargateService
 from constructs import Construct
 
 # When you want a different version change this line
-dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_6_3_amd64"
+dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_6_5_amd64"
 
 
 class SageworksDashboardStackProps(StackProps):
     def __init__(
         self,
         sageworks_bucket: str,
         sageworks_api_key: str,
```

### Comparing `sageworks-0.6.5/data/abalone.csv` & `sageworks-0.6.6/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/data/test_data.csv` & `sageworks-0.6.6/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/data/test_data.json` & `sageworks-0.6.6/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/data/wine_dataset.csv` & `sageworks-0.6.6/data/wine_dataset.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/admin/docker_push.md` & `sageworks-0.6.6/docs/admin/docker_push.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/admin/pypi_release.md` & `sageworks-0.6.6/docs/admin/pypi_release.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/api_classes/data_source.md` & `sageworks-0.6.6/docs/api_classes/data_source.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/api_classes/endpoint.md` & `sageworks-0.6.6/docs/api_classes/endpoint.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/api_classes/feature_set.md` & `sageworks-0.6.6/docs/api_classes/feature_set.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/api_classes/meta.md` & `sageworks-0.6.6/docs/api_classes/meta.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/api_classes/model.md` & `sageworks-0.6.6/docs/api_classes/model.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/api_classes/monitor.md` & `sageworks-0.6.6/docs/api_classes/monitor.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/api_classes/overview.md` & `sageworks-0.6.6/docs/api_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/api_classes/pipelines.md` & `sageworks-0.6.6/docs/api_classes/pipelines.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/aws_setup/aws_access_management.md` & `sageworks-0.6.6/docs/aws_setup/aws_access_management.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/aws_setup/aws_tips_and_tricks.md` & `sageworks-0.6.6/docs/aws_setup/aws_tips_and_tricks.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/aws_setup/core_stack.md` & `sageworks-0.6.6/docs/aws_setup/core_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/aws_setup/dashboard_stack.md` & `sageworks-0.6.6/docs/aws_setup/dashboard_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/aws_setup/domain_cert_setup.md` & `sageworks-0.6.6/docs/aws_setup/domain_cert_setup.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/aws_setup/full_pipeline.md` & `sageworks-0.6.6/docs/aws_setup/full_pipeline.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/aws_setup/sso_setup.md` & `sageworks-0.6.6/docs/aws_setup/sso_setup.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/concepts/model_monitoring.md` & `sageworks-0.6.6/docs/concepts/model_monitoring.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/core_classes/artifacts/overview.md` & `sageworks-0.6.6/docs/core_classes/artifacts/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/core_classes/overview.md` & `sageworks-0.6.6/docs/core_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/core_classes/transforms/overview.md` & `sageworks-0.6.6/docs/core_classes/transforms/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/core_classes/transforms/pandas_transforms.md` & `sageworks-0.6.6/docs/core_classes/transforms/pandas_transforms.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/core_classes/transforms/transform.md` & `sageworks-0.6.6/docs/core_classes/transforms/transform.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/enterprise/index.md` & `sageworks-0.6.6/docs/enterprise/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 | **<a href="https://supercowpowers.github.io/sageworks/api_classes/overview/" target="_blank">Python API</a>** | 🟢  | 🟢  | 🟢  | 🟢 |
 | **<a href="https://supercowpowers.github.io/sageworks/repl/" target="_blank">SageWorks REPL</a>** | 🟢  | 🟢  | 🟢 | 🟢 |
 | **<a href="https://supercowpowers.github.io/sageworks/" target="_blank">Dashboard</a>** | 🟢  | 🟢  | 🟢 | 🟢 |
 | **<a href="https://supercowpowers.github.io/sageworks/aws_setup/core_stack/" target="_blank">AWS Onboarding</a>**      | ➖ | 🟢  | 🟢  | 🟢 |
 | **<a href="https://supercowpowers.github.io/sageworks/plugins/" target="_blank">Dashboard Plugins</a>** | ➖  | 🟢  | 🟢  | 🟢 |
 | **<a href="https://supercowpowers.github.io/sageworks/plugins/" target="_blank">Custom Pages</a>**        | ➖  | ➖  | 🟢  | 🟢 |
 | **<a href="https://supercowpowers.github.io/sageworks/enterprise/themes/" target="_blank">Themes</a>**              | ➖  | ➖  | 🟢  | 🟢 |
-| **<a href="https://supercowpowers.github.io/sageworks/api_classes/pipelines/" target="_blank">ML Pipelines</a>**        | ➖  | ➖  | 🟢  | 🟢 |
+| **<a href="https://supercowpowers.github.io/sageworks/api_classes/pipelines/" target="_blank">ML Pipelines</a>**        | ➖  | ➖  | ➖   | 🟢 |
 | **<a href="https://supercowpowers.github.io/sageworks/enterprise/project_branding/" target="_blank">Project Branding</a>** | ➖  | ➖  | ➖  | 🟢 |
 | **Prioritized Feature Requests** | ➖| ➖| ➖ |🟢|
 | **Pricing**            | ➖ | $1500*| $3000* | $4000* |
 
 \*<small>*USD per month, includes AWS setup, support, and training: Everything needed to accelerate your AWS ML Development team. Interested in Data Science/Engineering consulting? We have top notch [Consultants](https://supercowpowers.github.io/sageworks/enterprise/#data-engineeringscience-consulting) with a depth and breadth of AWS ML/DS/Engineering expertise.*</small>
 
 ## Try SageWorks
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 development with an Enterprise License! | | Free | Enterprise: Lite |
 Enterprise: Standard | Enterprise: Pro | |---|----------------|-------------|--
 ---------------|------------------| | **_P_y_t_h_o_n_ _A_P_I** | ð¢ | ð¢ | ð¢ |
 ð¢ | | **_S_a_g_e_W_o_r_k_s_ _R_E_P_L** | ð¢ | ð¢ | ð¢ | ð¢ | | **_D_a_s_h_b_o_a_r_d** |
 ð¢ | ð¢ | ð¢ | ð¢ | | **_A_W_S_ _O_n_b_o_a_r_d_i_n_g** | â | ð¢ | ð¢ | ð¢ | |
 **_D_a_s_h_b_o_a_r_d_ _P_l_u_g_i_n_s** | â | ð¢ | ð¢ | ð¢ | | **_C_u_s_t_o_m_ _P_a_g_e_s** | â |
 â | ð¢ | ð¢ | | **_T_h_e_m_e_s** | â | â | ð¢ | ð¢ | | **_M_L_ _P_i_p_e_l_i_n_e_s**
-| â | â | ð¢ | ð¢ | | **_P_r_o_j_e_c_t_ _B_r_a_n_d_i_n_g** | â | â | â | ð¢ | |
+| â | â | â | ð¢ | | **_P_r_o_j_e_c_t_ _B_r_a_n_d_i_n_g** | â | â | â | ð¢ | |
 **Prioritized Feature Requests** | â| â| â |ð¢| | **Pricing** | â |
 $1500*| $3000* | $4000* | \**USD per month, includes AWS setup, support, and
 training: Everything needed to accelerate your AWS ML Development team.
 Interested in Data Science/Engineering consulting? We have top notch
 [Consultants](https://supercowpowers.github.io/sageworks/enterprise/#data-
 engineeringscience-consulting) with a depth and breadth of AWS ML/DS/
 Engineering expertise.* ## Try SageWorks We encourage new users to try out the
```

### Comparing `sageworks-0.6.5/docs/enterprise/project_branding.md` & `sageworks-0.6.6/docs/enterprise/project_branding.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/enterprise/themes.md` & `sageworks-0.6.6/docs/enterprise/themes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/getting_started/index.md` & `sageworks-0.6.6/docs/getting_started/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/glue/index.md` & `sageworks-0.6.6/docs/glue/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/images/big_spider.png` & `sageworks-0.6.6/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/images/graph_representation.png` & `sageworks-0.6.6/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/images/powered_aws_dark_blue.png` & `sageworks-0.6.6/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/images/powered_aws_transparent.png` & `sageworks-0.6.6/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/images/powered_aws_white.png` & `sageworks-0.6.6/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.6.6/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/images/sageworks.png` & `sageworks-0.6.6/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/images/sageworks_concepts.png` & `sageworks-0.6.6/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/images/scp.png` & `sageworks-0.6.6/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/images/scp_labs.png` & `sageworks-0.6.6/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/images/small_spider.png` & `sageworks-0.6.6/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/index.md` & `sageworks-0.6.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/misc/faq.md` & `sageworks-0.6.6/docs/misc/faq.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/misc/general_info.md` & `sageworks-0.6.6/docs/misc/general_info.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/misc/sageworks_classes_concepts.md` & `sageworks-0.6.6/docs/misc/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/misc/scp_consulting.md` & `sageworks-0.6.6/docs/misc/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/plugins/index.md` & `sageworks-0.6.6/docs/plugins/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/plugins/plugin_api_changes.md` & `sageworks-0.6.6/docs/plugins/plugin_api_changes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/repl/index.md` & `sageworks-0.6.6/docs/repl/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/research/eda.md` & `sageworks-0.6.6/docs/blogs_research/eda.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/docs/research/htg.md` & `sageworks-0.6.6/docs/blogs_research/htg.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/datasource/datasource_query.py` & `sageworks-0.6.6/examples/datasource/datasource_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/datasource/datasource_stats.py` & `sageworks-0.6.6/examples/datasource/datasource_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/endpoint/endpoint_inference.py` & `sageworks-0.6.6/examples/endpoint/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/featureset/featureset_eda.py` & `sageworks-0.6.6/examples/featureset/featureset_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/featureset/featureset_query.py` & `sageworks-0.6.6/examples/featureset/featureset_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/full_ml_pipeline.py` & `sageworks-0.6.6/examples/full_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/glue/glue_hello_world.py` & `sageworks-0.6.6/examples/glue/glue_hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/glue/glue_hello_world_with_log.py` & `sageworks-0.6.6/examples/glue/glue_hello_world_with_log.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/glue/glue_load_s3_bucket.py` & `sageworks-0.6.6/examples/glue/glue_load_s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/meta/meta_model_metrics.py` & `sageworks-0.6.6/examples/meta/meta_model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/model/model_metrics.py` & `sageworks-0.6.6/examples/model/model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/model/onboard_model.py` & `sageworks-0.6.6/examples/model/onboard_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/monitor/monitor_usage.py` & `sageworks-0.6.6/examples/monitor/monitor_usage.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/pipelines/abalone_pipeline_v1.json` & `sageworks-0.6.6/examples/pipelines/abalone_pipeline_v1.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/pipelines/abalone_pipeline_v2.json` & `sageworks-0.6.6/examples/pipelines/abalone_pipeline_v2.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/pipelines/aqsol_pipeline_v1.json` & `sageworks-0.6.6/examples/pipelines/aqsol_pipeline_v1.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/pipelines/pipeline_manager.py` & `sageworks-0.6.6/examples/pipelines/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/plugins/pages/my_plugin_page.py` & `sageworks-0.6.6/examples/plugins/pages/my_plugin_page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/plugins/pages/plugin_page_1.py` & `sageworks-0.6.6/examples/plugins/pages/plugin_page_1.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/plugins/pages/plugin_page_2.py` & `sageworks-0.6.6/examples/plugins/pages/plugin_page_2.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/plugins/pages/plugin_page_3.py` & `sageworks-0.6.6/examples/plugins/pages/plugin_page_3.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/plugins/views/model_plugin_view.py` & `sageworks-0.6.6/examples/plugins/views/model_plugin_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/plugins/views/my_view_plugin.py` & `sageworks-0.6.6/examples/plugins/views/my_view_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/plugins/web_components/custom_plugin.py` & `sageworks-0.6.6/examples/plugins/web_components/custom_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/plugins/web_components/endpoint_plugin.py` & `sageworks-0.6.6/examples/plugins/web_components/endpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/plugins/web_components/endpoint_turbo.py` & `sageworks-0.6.6/examples/plugins/web_components/endpoint_turbo.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/plugins/web_components/model_markdown.py` & `sageworks-0.6.6/examples/plugins/web_components/model_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/plugins/web_components/model_plugin.py` & `sageworks-0.6.6/examples/plugins/web_components/model_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/storage/data_to_data.py` & `sageworks-0.6.6/examples/storage/data_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/storage/data_to_features.py` & `sageworks-0.6.6/examples/storage/data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/storage/endpoint_inference.py` & `sageworks-0.6.6/examples/storage/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/storage/hello_world_pipeline.py` & `sageworks-0.6.6/examples/storage/hello_world_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/storage/plugin_page_example.py` & `sageworks-0.6.6/examples/storage/plugin_page_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/storage/sagemaker_pipelines/all_steps.py` & `sageworks-0.6.6/examples/storage/sagemaker_pipelines/all_steps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/storage/sagemaker_pipelines/ml_pipeline.py` & `sageworks-0.6.6/examples/storage/sagemaker_pipelines/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py` & `sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py` & `sageworks-0.6.6/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/mkdocs.yml` & `sageworks-0.6.6/mkdocs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,19 @@
     - Meta: api_classes/meta.md
     - DataSource: api_classes/data_source.md
     - FeatureSet: api_classes/feature_set.md
     - Model: api_classes/model.md
     - Endpoint: api_classes/endpoint.md
     - Pipelines: api_classes/pipelines.md
     - Monitor: api_classes/monitor.md
+  - Blogs/Research: 
+    - OverView: blogs_research/index.md
+    - Residual Analysis: blogs_research/residual_analysis.md 
+    - Exploratory Data Analysis(EDA): blogs_research/eda.md
+    - High Target Gradients (HTG): blogs_research/htg.md
   - Core Classes: 
     - OverView: core_classes/overview.md
     - Artifacts: 
       - OverView: core_classes/artifacts/overview.md
       - AthenaSource: core_classes/artifacts/athena_source.md
       - FeatureSetCore: core_classes/artifacts/feature_set_core.md
       - ModelCore: core_classes/artifacts/model_core.md
@@ -36,17 +41,14 @@
       - OverView: plugins/index.md
       - API Changes: plugins/plugin_api_changes.md
   - SageWorks Enterprise: 
       - OverView: enterprise/index.md
       - Themes: enterprise/themes.md
       - Project Branding: enterprise/project_branding.md
   - FAQ:  misc/faq.md
-  - Research:
-      - EDA: research/eda.md
-      - HTG: research/htg.md
   - AWS Glue Jobs: glue/index.md 
   - AWS Setup: 
     - Developer SSO Setup: aws_setup/sso_setup.md
     - Full Pipeline Testing: aws_setup/full_pipeline.md
     - AWS Admin Initial Setup: aws_setup/core_stack.md
     - Dashboard Setup: aws_setup/dashboard_stack.md
     - Domain/SSL Cert Setup: aws_setup/domain_cert_setup.md
```

### Comparing `sageworks-0.6.5/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.6.6/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/notebooks/ML_Pipeline_with_SageWorks_2.ipynb` & `sageworks-0.6.6/notebooks/ML_Pipeline_with_SageWorks_2.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/notebooks/Outliers_in_SageWorks.ipynb` & `sageworks-0.6.6/notebooks/Outliers_in_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/notebooks/images/athena_query_aqsol.png` & `sageworks-0.6.6/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.6.6/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.6.6/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/notebooks/images/model_screenshot.png` & `sageworks-0.6.6/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/notebooks/images/sageworks_concepts.png` & `sageworks-0.6.6/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/notebooks/images/scp_labs.png` & `sageworks-0.6.6/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/ag_table_row_selection.py` & `sageworks-0.6.6/scripts/ag_table_row_selection.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/athena_ddl_mixed_case.py` & `sageworks-0.6.6/scripts/athena_ddl_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/copy_data_catalog_db.py` & `sageworks-0.6.6/scripts/copy_data_catalog_db.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/create_glue_workflow_with_trigger.py` & `sageworks-0.6.6/scripts/create_glue_workflow_with_trigger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/delete_redis_keys.py` & `sageworks-0.6.6/scripts/delete_redis_keys.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/glue_mixed_case.py` & `sageworks-0.6.6/scripts/glue_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/model_endpoint_sanity_check.py` & `sageworks-0.6.6/scripts/model_endpoint_sanity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/onboard_endpoints.py` & `sageworks-0.6.6/scripts/onboard_endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/onboard_models.py` & `sageworks-0.6.6/scripts/onboard_models.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/storage/dns_data_to_features.py` & `sageworks-0.6.6/scripts/storage/dns_data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/storage/generate_jsonl_data.py` & `sageworks-0.6.6/scripts/storage/generate_jsonl_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/scripts/test_feature_resolution.py` & `sageworks-0.6.6/scripts/test_feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/setup.cfg` & `sageworks-0.6.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/setup.py` & `sageworks-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/__init__.py` & `sageworks-0.6.6/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/dataframe/aggregation.py` & `sageworks-0.6.6/src/sageworks/algorithms/dataframe/aggregation.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/dataframe/data_source_eda.py` & `sageworks-0.6.6/src/sageworks/algorithms/dataframe/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/dataframe/dimensionality_reduction.py` & `sageworks-0.6.6/src/sageworks/algorithms/dataframe/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/dataframe/feature_resolution.py` & `sageworks-0.6.6/src/sageworks/algorithms/dataframe/feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/dataframe/feature_spider.py` & `sageworks-0.6.6/src/sageworks/algorithms/dataframe/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/dataframe/row_tagger.py` & `sageworks-0.6.6/src/sageworks/algorithms/dataframe/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/spark/Readme.md` & `sageworks-0.6.6/src/sageworks/algorithms/spark/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/sql/Readme.md` & `sageworks-0.6.6/src/sageworks/algorithms/sql/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/sql/column_stats.py` & `sageworks-0.6.6/src/sageworks/algorithms/sql/column_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/sql/correlations.py` & `sageworks-0.6.6/src/sageworks/algorithms/sql/correlations.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/sql/descriptive_stats.py` & `sageworks-0.6.6/src/sageworks/algorithms/sql/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/sql/outliers.py` & `sageworks-0.6.6/src/sageworks/algorithms/sql/outliers.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/sql/sample_rows.py` & `sageworks-0.6.6/src/sageworks/algorithms/sql/sample_rows.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/algorithms/sql/value_counts.py` & `sageworks-0.6.6/src/sageworks/algorithms/sql/value_counts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/api/__init__.py` & `sageworks-0.6.6/src/sageworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/api/data_source.py` & `sageworks-0.6.6/src/sageworks/api/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/api/endpoint.py` & `sageworks-0.6.6/src/sageworks/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/api/feature_set.py` & `sageworks-0.6.6/src/sageworks/api/feature_set.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/api/meta.py` & `sageworks-0.6.6/src/sageworks/api/meta.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/api/model.py` & `sageworks-0.6.6/src/sageworks/api/model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/api/monitor.py` & `sageworks-0.6.6/src/sageworks/api/monitor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/api/pipeline.py` & `sageworks-0.6.6/src/sageworks/api/pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/api/pipeline_manager.py` & `sageworks-0.6.6/src/sageworks/api/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py` & `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.6.6/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/artifacts/__init__.py` & `sageworks-0.6.6/src/sageworks/core/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/artifacts/artifact.py` & `sageworks-0.6.6/src/sageworks/core/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/artifacts/athena_source.py` & `sageworks-0.6.6/src/sageworks/core/artifacts/athena_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/artifacts/data_source_abstract.py` & `sageworks-0.6.6/src/sageworks/core/artifacts/data_source_abstract.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/artifacts/data_source_factory.py` & `sageworks-0.6.6/src/sageworks/core/artifacts/data_source_factory.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/artifacts/endpoint_core.py` & `sageworks-0.6.6/src/sageworks/core/artifacts/endpoint_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/artifacts/feature_set_core.py` & `sageworks-0.6.6/src/sageworks/core/artifacts/feature_set_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/artifacts/model_core.py` & `sageworks-0.6.6/src/sageworks/core/artifacts/model_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/artifacts/monitor_core.py` & `sageworks-0.6.6/src/sageworks/core/artifacts/monitor_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/pipelines/pipeline_executor.py` & `sageworks-0.6.6/src/sageworks/core/pipelines/pipeline_executor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/Readme.md` & `sageworks-0.6.6/src/sageworks/core/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/light/__init__.py` & `sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.6.6/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/light/clean_data.py` & `sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.6.6/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py` & `sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py` & `sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py` & `sageworks-0.6.6/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/features_to_model/features_to_model.py` & `sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/features_to_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.6.6/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.6.6/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/__init__.py` & `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py` & `sageworks-0.6.6/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/core/transforms/transform.py` & `sageworks-0.6.6/src/sageworks/core/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/experiments/view_manager.py` & `sageworks-0.6.6/src/sageworks/experiments/view_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/repl/sageworks_shell.py` & `sageworks-0.6.6/src/sageworks/repl/sageworks_shell.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/aws_utils.py` & `sageworks-0.6.6/src/sageworks/utils/aws_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/cache.py` & `sageworks-0.6.6/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/chem_utils.py` & `sageworks-0.6.6/src/sageworks/utils/chem_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/config_manager.py` & `sageworks-0.6.6/src/sageworks/utils/config_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/dashboard_metrics.py` & `sageworks-0.6.6/src/sageworks/utils/dashboard_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/datetime_utils.py` & `sageworks-0.6.6/src/sageworks/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.6.6/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/docker_utils.py` & `sageworks-0.6.6/src/sageworks/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/ecs_info.py` & `sageworks-0.6.6/src/sageworks/utils/ecs_info.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/endpoint_metrics.py` & `sageworks-0.6.6/src/sageworks/utils/endpoint_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/endpoint_utils.py` & `sageworks-0.6.6/src/sageworks/utils/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/extract_model_artifact.py` & `sageworks-0.6.6/src/sageworks/utils/extract_model_artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/glue_utils.py` & `sageworks-0.6.6/src/sageworks/utils/glue_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/license_manager.py` & `sageworks-0.6.6/src/sageworks/utils/license_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         """
 
         # Store the API Key for later use
         cls.api_key = api_key
 
         # Decode the API Key
         try:
-            decoded_license_key = base64.b64decode(api_key)
+            decoded_license_key = base64.urlsafe_b64decode(api_key)
             _license_data, signature = cls.extract_data_and_signature(decoded_license_key)
         except Exception as e:
             cls.log.critical(f"Failed to decode API Key: {e}")
             cls.log.critical("Please contact SageWorks support")
             raise FatalLicenseError()
 
         # Verify the signature of the API Key
```

### Comparing `sageworks-0.6.5/src/sageworks/utils/markdown_utils.py` & `sageworks-0.6.6/src/sageworks/utils/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/pandas_utils.py` & `sageworks-0.6.6/src/sageworks/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/plugin_manager.py` & `sageworks-0.6.6/src/sageworks/utils/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/redis_cache.py` & `sageworks-0.6.6/src/sageworks/utils/redis_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/repl_utils.py` & `sageworks-0.6.6/src/sageworks/utils/repl_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/s3_utils.py` & `sageworks-0.6.6/src/sageworks/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/sageworks_cache.py` & `sageworks-0.6.6/src/sageworks/utils/sageworks_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.6.6/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.6.6/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.6.6/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/symbols.py` & `sageworks-0.6.6/src/sageworks/utils/symbols.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/test_data_generator.py` & `sageworks-0.6.6/src/sageworks/utils/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/trace_calls.py` & `sageworks-0.6.6/src/sageworks/utils/trace_calls.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/utils/type_abbrev.py` & `sageworks-0.6.6/src/sageworks/utils/type_abbrev.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/views/artifacts_text_view.py` & `sageworks-0.6.6/src/sageworks/views/artifacts_text_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/views/artifacts_web_view.py` & `sageworks-0.6.6/src/sageworks/views/artifacts_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/views/data_source_web_view.py` & `sageworks-0.6.6/src/sageworks/views/data_source_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/views/endpoint_web_view.py` & `sageworks-0.6.6/src/sageworks/views/endpoint_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/views/feature_set_web_view.py` & `sageworks-0.6.6/src/sageworks/views/feature_set_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/views/model_web_view.py` & `sageworks-0.6.6/src/sageworks/views/model_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/views/view.py` & `sageworks-0.6.6/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/component_interface.py` & `sageworks-0.6.6/src/sageworks/web_components/component_interface.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.6.6/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/correlation_matrix.py` & `sageworks-0.6.6/src/sageworks/web_components/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/data_details_markdown.py` & `sageworks-0.6.6/src/sageworks/web_components/data_details_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/endpoint_details.py` & `sageworks-0.6.6/src/sageworks/web_components/endpoint_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/endpoint_metric_plots.py` & `sageworks-0.6.6/src/sageworks/web_components/endpoint_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/experiments/color_maps.py` & `sageworks-0.6.6/src/sageworks/web_components/experiments/color_maps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/experiments/compound_details.py` & `sageworks-0.6.6/src/sageworks/web_components/experiments/compound_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/experiments/dashboard_metric_plots.py` & `sageworks-0.6.6/src/sageworks/web_components/experiments/dashboard_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/experiments/data_table.py` & `sageworks-0.6.6/src/sageworks/web_components/experiments/data_table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/experiments/histogram.py` & `sageworks-0.6.6/src/sageworks/web_components/experiments/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/experiments/line_chart.py` & `sageworks-0.6.6/src/sageworks/web_components/experiments/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/experiments/outlier_plot.py` & `sageworks-0.6.6/src/sageworks/web_components/experiments/outlier_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/experiments/plugin_callbacks.py` & `sageworks-0.6.6/src/sageworks/web_components/experiments/plugin_callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/experiments/scatter_plot.py` & `sageworks-0.6.6/src/sageworks/web_components/experiments/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/model_details.py` & `sageworks-0.6.6/src/sageworks/web_components/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/model_plot.py` & `sageworks-0.6.6/src/sageworks/web_components/model_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/plugin_interface.py` & `sageworks-0.6.6/src/sageworks/web_components/plugin_interface.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/plugin_unit_test.py` & `sageworks-0.6.6/src/sageworks/web_components/plugin_unit_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/plugins/ag_table.py` & `sageworks-0.6.6/src/sageworks/web_components/plugins/ag_table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/plugins/license_details.py` & `sageworks-0.6.6/src/sageworks/web_components/plugins/license_details.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,23 @@
 # SageWorks Imports
 from sageworks.web_components.plugin_interface import PluginInterface, PluginPage, PluginInputType
 from sageworks.utils.license_manager import LicenseManager
 
 # Get the SageWorks logger
 log = logging.getLogger("sageworks")
 
+# Feature Information Dictionary
+FEATURES = {
+    "plugins": "Component Plugins",
+    "pages": "Fully Customizable Pages",
+    "themes": "Dark, Light, and Custom Themes",
+    "pipelines": "Machine Learning Pipelines (beta)",
+    "branding": "Company/Project User Interface Branding",
+}
+
 
 class LicenseDetails(PluginInterface):
     """License Details Markdown Component"""
 
     """Initialize this Plugin Component Class with required attributes"""
     auto_load_page = PluginPage.NONE
     plugin_input_type = PluginInputType.CUSTOM
@@ -28,21 +37,27 @@
             html.Div: A Container of Components for the Model Details
         """
         container = html.Div(
             id=component_id,
             children=[
                 html.H3(id=f"{component_id}-header", children="License: Loading..."),
                 dcc.Markdown(id=f"{component_id}-details", children="Waiting for Data...", dangerously_allow_html=True),
+                html.H3(id=f"{component_id}-support-header", children="Support: Loading..."),
+                dcc.Markdown(
+                    id=f"{component_id}-support-details", children="Waiting for Data...", dangerously_allow_html=True
+                ),
             ],
         )
 
         # Fill in plugin properties
         self.properties = [
             (f"{component_id}-header", "children"),
             (f"{component_id}-details", "children"),
+            (f"{component_id}-support-header", "children"),
+            (f"{component_id}-support-details", "children"),
         ]
 
         # Return the container
         return container
 
     def update_properties(self, license: dict, **kwargs) -> list:
         """Update the properties for the plugin.
@@ -56,31 +71,45 @@
         """
         # Update the header and the details
         header = "License Details"
 
         # See if we can connect to the License Server
         response = LicenseManager.contact_license_server()
         if response.status_code == 200:
-            details = "**License Server:** Connected<br>"
+            details = "**License Server:** 🟢 Connected<br>"
         else:
             # Note: This is 100% fine/expected (connecting to the license server is optional)
-            details = "**License Server:** Not connected<br>"
+            details = "**License Server:** 🔵 Not connected<br>"
 
         # Fill in the license details
         details += f"**License Id:** {license['license_id']}<br>"
-        details += f"**Company:** {license['license_id']}<br>"
+        details += f"**Company:** {license.get('company', 'Unknown')}<br>"
         details += f"**AWS Account:** {license['aws_account_id']}<br>"
         details += f"**Expiration:** {license['expires']}<br>"
         details += f"**License Tier:** {license.get('tier', 'Open Source')}<br>"
         details += "**Features:**\n"
-        for feature, value in license["features"].items():
-            details += f"  - **{feature}:** {value}\n"
+        if isinstance(license["features"], dict):
+            for feature, value in license["features"].items():
+                details += f"  - **{feature}:** {value}\n"
+        else:
+            for feature, description in FEATURES.items():
+                if feature in license["features"]:
+                    details += f"  - {description}  (**YES**)\n"
+                else:
+                    details += (
+                        f"  - {description}  ([UPGRADE](https://supercowpowers.github.io/sageworks/enterprise/))\n"
+                    )
+
+        # Fill in the support details
+        support_header = "Support Information"
+        support_details = "- **Email:** [support@supercowpowers.com](mailto:support@supercowpowers.com)\n"
+        support_details += "- **Chat:** [Discord](https://discord.gg/WHAJuz8sw8)\n"
 
         # Return the updated property values for the plugin
-        return [header, details]
+        return [header, details, support_header, support_details]
 
 
 if __name__ == "__main__":
     # This class takes in license details and generates a details Markdown component
     import dash
     from sageworks.utils.config_manager import ConfigManager
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sageworks-0.6.5/src/sageworks/web_components/plugins/model_details.py` & `sageworks-0.6.6/src/sageworks/web_components/plugins/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/plugins/pipeline_details.py` & `sageworks-0.6.6/src/sageworks/web_components/plugins/pipeline_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/regression_plot.py` & `sageworks-0.6.6/src/sageworks/web_components/regression_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/table.py` & `sageworks-0.6.6/src/sageworks/web_components/table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks/web_components/violin_plots.py` & `sageworks-0.6.6/src/sageworks/web_components/violin_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.6.6/src/sageworks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.6.5
+Version: 0.6.6
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sageworks-0.6.5/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.6.6/src/sageworks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,18 @@
 docs/aws_setup/aws_access_management.md
 docs/aws_setup/aws_tips_and_tricks.md
 docs/aws_setup/core_stack.md
 docs/aws_setup/dashboard_stack.md
 docs/aws_setup/domain_cert_setup.md
 docs/aws_setup/full_pipeline.md
 docs/aws_setup/sso_setup.md
+docs/blogs_research/eda.md
+docs/blogs_research/htg.md
+docs/blogs_research/index.md
+docs/blogs_research/residual_analysis.md
 docs/concepts/model_monitoring.md
 docs/core_classes/overview.md
 docs/core_classes/artifacts/artifact.md
 docs/core_classes/artifacts/athena_source.md
 docs/core_classes/artifacts/data_source_abstract.md
 docs/core_classes/artifacts/endpoint_core.md
 docs/core_classes/artifacts/feature_set_core.md
@@ -153,16 +157,14 @@
 docs/misc/faq.md
 docs/misc/general_info.md
 docs/misc/sageworks_classes_concepts.md
 docs/misc/scp_consulting.md
 docs/plugins/index.md
 docs/plugins/plugin_api_changes.md
 docs/repl/index.md
-docs/research/eda.md
-docs/research/htg.md
 examples/full_ml_pipeline.py
 examples/ag-grid/hello_world.py
 examples/datasource/datasource_from_df.py
 examples/datasource/datasource_from_s3.py
 examples/datasource/datasource_query.py
 examples/datasource/datasource_stats.py
 examples/datasource/datasource_to_featureset.py
```

### Comparing `sageworks-0.6.5/tests/artifacts/data_source_tests.py` & `sageworks-0.6.6/tests/artifacts/data_source_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/artifacts/endpoint_tests.py` & `sageworks-0.6.6/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/artifacts/feature_set_tests.py` & `sageworks-0.6.6/tests/artifacts/feature_set_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/artifacts/model_tests.py` & `sageworks-0.6.6/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/aws_account/aws_account_clamp_tests.py` & `sageworks-0.6.6/tests/aws_account/aws_account_clamp_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.6.6/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/connectors/data_catalog.py` & `sageworks-0.6.6/tests/connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/connectors/endpoints.py` & `sageworks-0.6.6/tests/connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/connectors/feature_store.py` & `sageworks-0.6.6/tests/connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/connectors/glue_jobs.py` & `sageworks-0.6.6/tests/connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/connectors/model_registry.py` & `sageworks-0.6.6/tests/connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/connectors/s3_bucket.py` & `sageworks-0.6.6/tests/connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/create_aqsol_artifacts.py` & `sageworks-0.6.6/tests/create_aqsol_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/create_basic_test_artifacts.py` & `sageworks-0.6.6/tests/create_basic_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/create_realtime_endpoint.py` & `sageworks-0.6.6/tests/create_realtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/create_training_adjusted_artifacts.py` & `sageworks-0.6.6/tests/create_training_adjusted_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/create_wine_artifacts.py` & `sageworks-0.6.6/tests/create_wine_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/delete_test_artifacts.py` & `sageworks-0.6.6/tests/delete_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/plugin_tests/crashing_plugin.py` & `sageworks-0.6.6/tests/plugin_tests/crashing_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/specific/capital_tests.py` & `sageworks-0.6.6/tests/specific/capital_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/specific/deletion_tests.py` & `sageworks-0.6.6/tests/specific/deletion_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/transforms/data_to_data_tests.py` & `sageworks-0.6.6/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/transforms/data_to_features_tests.py` & `sageworks-0.6.6/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/transforms/features_to_model_tests.py` & `sageworks-0.6.6/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/transforms/model_metrics_tests.py` & `sageworks-0.6.6/tests/transforms/model_metrics_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.6.6/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.6.6/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/web_components/confusion_matrix_test.py` & `sageworks-0.6.6/tests/web_components/confusion_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/web_components/correlation_matrix_test.py` & `sageworks-0.6.6/tests/web_components/correlation_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tests/web_components/plugin_interface_test.py` & `sageworks-0.6.6/tests/web_components/plugin_interface_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/tox.ini` & `sageworks-0.6.6/tox.ini`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/ui_testing/assets/custom.css` & `sageworks-0.6.6/ui_testing/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/ui_testing/table_comparison.py` & `sageworks-0.6.6/ui_testing/table_comparison.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/ui_testing/theme_switching.py` & `sageworks-0.6.6/ui_testing/theme_switching.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.5/ui_testing/theme_switching_2.py` & `sageworks-0.6.6/ui_testing/theme_switching_2.py`

 * *Files identical despite different names*

