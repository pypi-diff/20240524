# Comparing `tmp/syngen-0.8.3.tar.gz` & `tmp/syngen-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.8.3.tar", last modified: Thu May 23 16:15:45 2024, max compression
+gzip compressed data, was "syngen-0.8.4.tar", last modified: Fri May 24 11:53:55 2024, max compression
```

## Comparing `syngen-0.8.3.tar` & `syngen-0.8.4.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.198746 syngen-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-23 16:14:28.000000 syngen-0.8.3/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 16:14:28.000000 syngen-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 16:14:28.000000 syngen-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26894 2024-05-23 16:15:45.198746 syngen-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24991 2024-05-23 16:14:28.000000 syngen-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-23 16:14:29.000000 syngen-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-23 16:15:45.198746 syngen-0.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.178746 syngen-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/config/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/config/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/context/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18411 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.186746 syngen-0.8.3/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   723510 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/img/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/script.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46709 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/mlflow_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/mlflow_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.190746 syngen-0.8.3/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    46231 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/ml/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/streamlit_app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/streamlit_app/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.194746 syngen-0.8.3/src/syngen/streamlit_app/css/
--rw-r--r--   0 runner    (1001) docker     (127)   707122 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.198746 syngen-0.8.3/src/syngen/streamlit_app/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.198746 syngen-0.8.3/src/syngen/streamlit_app/img/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/img/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.198746 syngen-0.8.3/src/syngen/streamlit_app/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/streamlit_app/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-23 16:14:29.000000 syngen-0.8.3/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:15:45.198746 syngen-0.8.3/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26894 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 16:15:45.000000 syngen-0.8.3/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.345022 syngen-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-24 11:52:29.000000 syngen-0.8.4/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-24 11:52:29.000000 syngen-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 11:52:29.000000 syngen-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27084 2024-05-24 11:53:55.345022 syngen-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25181 2024-05-24 11:52:29.000000 syngen-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-24 11:52:30.000000 syngen-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-24 11:53:55.345022 syngen-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.329022 syngen-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.333022 syngen-0.8.4/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.333022 syngen-0.8.4/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.333022 syngen-0.8.4/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/config/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/config/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.337022 syngen-0.8.4/src/syngen/ml/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.337022 syngen-0.8.4/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.337022 syngen-0.8.4/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.337022 syngen-0.8.4/src/syngen/ml/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18411 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.337022 syngen-0.8.4/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.337022 syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   723510 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.337022 syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.337022 syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.337022 syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/src/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/src/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/src/script.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.337022 syngen-0.8.4/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46709 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.341022 syngen-0.8.4/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.341022 syngen-0.8.4/src/syngen/ml/mlflow_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/mlflow_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.341022 syngen-0.8.4/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.341022 syngen-0.8.4/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.341022 syngen-0.8.4/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.341022 syngen-0.8.4/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/vae/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.341022 syngen-0.8.4/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/vae/models/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46231 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.341022 syngen-0.8.4/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.341022 syngen-0.8.4/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.341022 syngen-0.8.4/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/ml/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.341022 syngen-0.8.4/src/syngen/streamlit_app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.345022 syngen-0.8.4/src/syngen/streamlit_app/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/streamlit_app/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/streamlit_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.345022 syngen-0.8.4/src/syngen/streamlit_app/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   707122 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/streamlit_app/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.345022 syngen-0.8.4/src/syngen/streamlit_app/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/streamlit_app/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/streamlit_app/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.345022 syngen-0.8.4/src/syngen/streamlit_app/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/streamlit_app/img/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/streamlit_app/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/streamlit_app/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/streamlit_app/start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.345022 syngen-0.8.4/src/syngen/streamlit_app/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/streamlit_app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/streamlit_app/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-24 11:52:30.000000 syngen-0.8.4/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:53:55.345022 syngen-0.8.4/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27084 2024-05-24 11:53:55.000000 syngen-0.8.4/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-24 11:53:55.000000 syngen-0.8.4/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:53:55.000000 syngen-0.8.4/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-24 11:53:55.000000 syngen-0.8.4/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-24 11:53:55.000000 syngen-0.8.4/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 11:53:55.000000 syngen-0.8.4/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.8.3/LICENSE` & `syngen-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/PKG-INFO` & `syngen-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.8.3
+Version: 0.8.4
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -386,39 +386,43 @@
 <https://hub.docker.com/r/tdspora/syngen>
 
 To run dockerized code (see parameters description in *Training* and *Inference* sections) for one table call:
 
 ```bash
 docker pull tdspora/syngen
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=train \
   --table_name=TABLE_NAME \
   --source=./model_artifacts/YOUR_CSV_FILE.csv
 
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=infer \
   --table_name=TABLE_NAME
 ```
 
 PATH_TO_LOCAL_FOLDER is an absolute path to the folder where your original csv is stored.
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call.
 
 To run dockerized code by providing the metadata file simply call:
 
 ```bash
 docker pull tdspora/syngen
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=train \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=infer \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call, however, they will be
 overwritten by corresponding arguments in the metadata file.
@@ -464,22 +468,28 @@
 The provided environmental variables allow to track the training process, and the inference process, and store 
 the artifacts in the desired location.
 You can access the MLflow UI by navigating to the provided URL in your browser. If you store artifacts in remote storage,
 ensure that all necessary credentials are provided before using Mlflow.
 
 ```bash
 docker pull tdspora/syngen:latest
-docker run --rm -it -e MLFLOW_TRACKING_URI='http://localhost:5000' \
+docker run --rm -it \
+  --user $(id -u):$(id -g) \
+  -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
-  -e MLFLOW_EXPERIMENT_NAME=test_name -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
+  -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 
-docker run --rm -it -e MLFLOW_TRACKING_URI='http://localhost:5000' \
+docker run --rm -it \
+  --user $(id -u):$(id -g) \
+  -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
-  -e MLFLOW_EXPERIMENT_NAME=test_name -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
+  -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
 ## Contribution
 
 We welcome contributions from the community to help us improve and maintain our public GitHub repository. We appreciate any feedback, bug reports, or feature requests, and we encourage developers to submit fixes or new features using issues.
```

### Comparing `syngen-0.8.3/README.md` & `syngen-0.8.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -328,39 +328,43 @@
 <https://hub.docker.com/r/tdspora/syngen>
 
 To run dockerized code (see parameters description in *Training* and *Inference* sections) for one table call:
 
 ```bash
 docker pull tdspora/syngen
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=train \
   --table_name=TABLE_NAME \
   --source=./model_artifacts/YOUR_CSV_FILE.csv
 
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=infer \
   --table_name=TABLE_NAME
 ```
 
 PATH_TO_LOCAL_FOLDER is an absolute path to the folder where your original csv is stored.
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call.
 
 To run dockerized code by providing the metadata file simply call:
 
 ```bash
 docker pull tdspora/syngen
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=train \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=infer \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call, however, they will be
 overwritten by corresponding arguments in the metadata file.
@@ -406,22 +410,28 @@
 The provided environmental variables allow to track the training process, and the inference process, and store 
 the artifacts in the desired location.
 You can access the MLflow UI by navigating to the provided URL in your browser. If you store artifacts in remote storage,
 ensure that all necessary credentials are provided before using Mlflow.
 
 ```bash
 docker pull tdspora/syngen:latest
-docker run --rm -it -e MLFLOW_TRACKING_URI='http://localhost:5000' \
+docker run --rm -it \
+  --user $(id -u):$(id -g) \
+  -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
-  -e MLFLOW_EXPERIMENT_NAME=test_name -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
+  -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 
-docker run --rm -it -e MLFLOW_TRACKING_URI='http://localhost:5000' \
+docker run --rm -it \
+  --user $(id -u):$(id -g) \
+  -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
-  -e MLFLOW_EXPERIMENT_NAME=test_name -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
+  -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
 ## Contribution
 
 We welcome contributions from the community to help us improve and maintain our public GitHub repository. We appreciate any feedback, bug reports, or feature requests, and we encourage developers to submit fixes or new features using issues.
```

#### html2text {}

```diff
@@ -228,27 +228,28 @@
 --metadata_path="./examples/example-metadata/housing_metadata.yaml" ``` If `--
 metadata_path` is present and the metadata contains the necessary parameters,
 other CLI parameters will be ignored.
 ### Docker images The train and inference components of syngen is available as
 public docker image:
 hub.docker.com/r/tdspora/syngen> To run dockerized code (see parameters
 description in *Training* and *Inference* sections) for one table call: ```bash
-docker pull tdspora/syngen docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/src/
-model_artifacts tdspora/syngen \ --task=train \ --table_name=TABLE_NAME \ --
-source=./model_artifacts/YOUR_CSV_FILE.csv docker run --rm \ -
-v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \ --task=infer \ --
-table_name=TABLE_NAME ``` PATH_TO_LOCAL_FOLDER is an absolute path to the
-folder where your original csv is stored. You can add any arguments listed in
-the corresponding sections for infer and training processes in the CLI call. To
-run dockerized code by providing the metadata file simply call: ```bash docker
-pull tdspora/syngen docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/src/
+docker pull tdspora/syngen docker run --rm \ --user $(id -u):$(id -g) \ -
+v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \ --task=train \ --
+table_name=TABLE_NAME \ --source=./model_artifacts/YOUR_CSV_FILE.csv docker run
+--rm \ --user $(id -u):$(id -g) \ -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts
+tdspora/syngen \ --task=infer \ --table_name=TABLE_NAME ```
+PATH_TO_LOCAL_FOLDER is an absolute path to the folder where your original csv
+is stored. You can add any arguments listed in the corresponding sections for
+infer and training processes in the CLI call. To run dockerized code by
+providing the metadata file simply call: ```bash docker pull tdspora/syngen
+docker run --rm \ --user $(id -u):$(id -g) \ -v PATH_TO_LOCAL_FOLDER:/src/
 model_artifacts tdspora/syngen \ --task=train \ --metadata_path=./
-model_artifacts/PATH_TO_METADATA_YAML docker run --rm \ -
-v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \ --task=infer \ --
-metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` You can add any
+model_artifacts/PATH_TO_METADATA_YAML docker run --rm \ --user $(id -u):$(id -
+g) \ -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \ --task=infer
+\ --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` You can add any
 arguments listed in the corresponding sections for infer and training processes
 in the CLI call, however, they will be overwritten by corresponding arguments
 in the metadata file. #### UI web interface You can access the streamlit UI web
 interface by running the following command after installing the library with
 the UI option: ```bash pip install syngen[ui] ``` then create a python file and
 insert the code provided below into it: ```python from syngen import
 streamlit_app streamlit_app.start() ``` run the python file: ```bash python
@@ -264,21 +265,23 @@
 environment variable to the name you prefer for the experiment. When using
 Docker, ensure the environmental variables are set before running the
 container. The provided environmental variables allow to track the training
 process, and the inference process, and store the artifacts in the desired
 location. You can access the MLflow UI by navigating to the provided URL in
 your browser. If you store artifacts in remote storage, ensure that all
 necessary credentials are provided before using Mlflow. ```bash docker pull
-tdspora/syngen:latest docker run --rm -it -e MLFLOW_TRACKING_URI='http://
-localhost:5000' \ -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION
-\ -e MLFLOW_EXPERIMENT_NAME=test_name -v PATH_TO_LOCAL_FOLDER:/src/
+tdspora/syngen:latest docker run --rm -it \ --user $(id -u):$(id -g) \ -
+e MLFLOW_TRACKING_URI='http://localhost:5000' \ -
+e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \ -
+e MLFLOW_EXPERIMENT_NAME=test_name \ -v PATH_TO_LOCAL_FOLDER:/src/
 model_artifacts tdspora/syngen \ --metadata_path=./model_artifacts/
-PATH_TO_METADATA_YAML docker run --rm -it -e MLFLOW_TRACKING_URI='http://
-localhost:5000' \ -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION
-\ -e MLFLOW_EXPERIMENT_NAME=test_name -v PATH_TO_LOCAL_FOLDER:/src/
+PATH_TO_METADATA_YAML docker run --rm -it \ --user $(id -u):$(id -g) \ -
+e MLFLOW_TRACKING_URI='http://localhost:5000' \ -
+e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \ -
+e MLFLOW_EXPERIMENT_NAME=test_name \ -v PATH_TO_LOCAL_FOLDER:/src/
 model_artifacts tdspora/syngen \ --metadata_path=./model_artifacts/
 PATH_TO_METADATA_YAML ``` ## Contribution We welcome contributions from the
 community to help us improve and maintain our public GitHub repository. We
 appreciate any feedback, bug reports, or feature requests, and we encourage
 developers to submit fixes or new features using issues. If you have found a
 bug or have a feature request, please submit an issue to our GitHub repository.
 Please provide as much detail as possible, including steps to reproduce the
```

### Comparing `syngen-0.8.3/setup.cfg` & `syngen-0.8.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/infer.py` & `syngen-0.8.4/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/config/configurations.py` & `syngen-0.8.4/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/config/validation.py` & `syngen-0.8.4/src/syngen/ml/config/validation.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/context/context.py` & `syngen-0.8.4/src/syngen/ml/context/context.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/convertor/convertor.py` & `syngen-0.8.4/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.8.4/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/handlers/handlers.py` & `syngen-0.8.4/src/syngen/ml/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg` & `syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/metrics/accuracy_test/src/main.css` & `syngen-0.8.4/src/syngen/ml/metrics/accuracy_test/src/main.css`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.8.4/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.8.4/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.8.4/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/metrics/utils.py` & `syngen-0.8.4/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/mlflow_tracker/mlflow_tracker.py` & `syngen-0.8.4/src/syngen/ml/mlflow_tracker/mlflow_tracker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/reporters/reporters.py` & `syngen-0.8.4/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/strategies/strategies.py` & `syngen-0.8.4/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/utils/__init__.py` & `syngen-0.8.4/src/syngen/ml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/utils/utils.py` & `syngen-0.8.4/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.8.4/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/vae/models/dataset.py` & `syngen-0.8.4/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/vae/models/features.py` & `syngen-0.8.4/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/vae/models/model.py` & `syngen-0.8.4/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.8.4/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.8.4/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/ml/worker/worker.py` & `syngen-0.8.4/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/streamlit_app/css/style.css` & `syngen-0.8.4/src/syngen/streamlit_app/css/style.css`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/streamlit_app/handlers/handlers.py` & `syngen-0.8.4/src/syngen/streamlit_app/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/streamlit_app/img/favicon.svg` & `syngen-0.8.4/src/syngen/streamlit_app/img/favicon.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/streamlit_app/img/logo.svg` & `syngen-0.8.4/src/syngen/streamlit_app/img/logo.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/streamlit_app/run.py` & `syngen-0.8.4/src/syngen/streamlit_app/run.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/streamlit_app/start.py` & `syngen-0.8.4/src/syngen/streamlit_app/start.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/streamlit_app/utils/utils.py` & `syngen-0.8.4/src/syngen/streamlit_app/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen/train.py` & `syngen-0.8.4/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen.egg-info/PKG-INFO` & `syngen-0.8.4/src/syngen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.8.3
+Version: 0.8.4
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -386,39 +386,43 @@
 <https://hub.docker.com/r/tdspora/syngen>
 
 To run dockerized code (see parameters description in *Training* and *Inference* sections) for one table call:
 
 ```bash
 docker pull tdspora/syngen
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=train \
   --table_name=TABLE_NAME \
   --source=./model_artifacts/YOUR_CSV_FILE.csv
 
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=infer \
   --table_name=TABLE_NAME
 ```
 
 PATH_TO_LOCAL_FOLDER is an absolute path to the folder where your original csv is stored.
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call.
 
 To run dockerized code by providing the metadata file simply call:
 
 ```bash
 docker pull tdspora/syngen
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=train \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 
 docker run --rm \
+  --user $(id -u):$(id -g) \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --task=infer \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call, however, they will be
 overwritten by corresponding arguments in the metadata file.
@@ -464,22 +468,28 @@
 The provided environmental variables allow to track the training process, and the inference process, and store 
 the artifacts in the desired location.
 You can access the MLflow UI by navigating to the provided URL in your browser. If you store artifacts in remote storage,
 ensure that all necessary credentials are provided before using Mlflow.
 
 ```bash
 docker pull tdspora/syngen:latest
-docker run --rm -it -e MLFLOW_TRACKING_URI='http://localhost:5000' \
+docker run --rm -it \
+  --user $(id -u):$(id -g) \
+  -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
-  -e MLFLOW_EXPERIMENT_NAME=test_name -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
+  -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 
-docker run --rm -it -e MLFLOW_TRACKING_URI='http://localhost:5000' \
+docker run --rm -it \
+  --user $(id -u):$(id -g) \
+  -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
-  -e MLFLOW_EXPERIMENT_NAME=test_name -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
+  -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
 ## Contribution
 
 We welcome contributions from the community to help us improve and maintain our public GitHub repository. We appreciate any feedback, bug reports, or feature requests, and we encourage developers to submit fixes or new features using issues.
```

### Comparing `syngen-0.8.3/src/syngen.egg-info/SOURCES.txt` & `syngen-0.8.4/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syngen-0.8.3/src/syngen.egg-info/requires.txt` & `syngen-0.8.4/src/syngen.egg-info/requires.txt`

 * *Files identical despite different names*

