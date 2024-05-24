# Comparing `tmp/dynamicio-5.0.0rc3.tar.gz` & `tmp/dynamicio-5.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicio-5.0.0rc3.tar", last modified: Tue Feb 27 13:31:11 2024, max compression
+gzip compressed data, was "dynamicio-5.0.0rc4.tar", last modified: Fri May 24 09:13:15 2024, max compression
```

## Comparing `dynamicio-5.0.0rc3.tar` & `dynamicio-5.0.0rc4.tar`

### file list

```diff
@@ -1,76 +1,83 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39394 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.439204 dynamicio-5.0.0rc3/demo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.439204 dynamicio-5.0.0rc3/demo/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      835 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      873 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      198 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/environment.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      972 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/io.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1904 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/runner_selection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.439204 dynamicio-5.0.0rc3/demo/src/runners/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/runners/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1203 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/runners/staging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1397 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/src/runners/transform.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/demo/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      820 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/constants.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/demo/tests/runners/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/runners/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/runners/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/runners/test_staging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      412 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/runners/test_transform.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2068 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/test_pipeline.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1180 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/demo/tests/test_runner_selection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/dynamicio/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3711 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/cli.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/dynamicio/config/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      134 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9530 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/io_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/dynamicio/config/pydantic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/pydantic/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1415 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/pydantic/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9295 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/pydantic/io_resources.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3270 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/config/pydantic/table_schema.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13784 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/core.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3172 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5841 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/metrics.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/dynamicio/mixins/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      321 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4875 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7816 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/with_kafka.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11316 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/with_local.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8017 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/with_postgres.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18850 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/mixins/with_s3.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/py.typed
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13239 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/dynamicio/validations.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.443204 dynamicio-5.0.0rc3/dynamicio.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1563 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      321 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-02-27 13:31:11.000000 dynamicio-5.0.0rc3/dynamicio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      705 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1924 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34498 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      469 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/constants.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:31:11.447204 dynamicio-5.0.0rc3/tests/mocking/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/mocking/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4755 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/mocking/io.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/mocking/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14102 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6460 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    43997 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_core.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6108 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_metrics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      485 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_table_schema.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16810 2024-02-27 13:30:58.000000 dynamicio-5.0.0rc3/tests/test_validations.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.792928 dynamicio-5.0.0rc4/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2024-05-24 09:13:15.788928 dynamicio-5.0.0rc4/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39394 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.784928 dynamicio-5.0.0rc4/demo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.784928 dynamicio-5.0.0rc4/demo/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      835 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/src/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      873 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/src/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      198 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/src/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/src/environment.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      972 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/src/io.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1904 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/src/runner_selection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.784928 dynamicio-5.0.0rc4/demo/src/runners/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/src/runners/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1203 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/src/runners/staging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1397 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/src/runners/transform.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.784928 dynamicio-5.0.0rc4/demo/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      820 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/tests/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/tests/constants.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.784928 dynamicio-5.0.0rc4/demo/tests/runners/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/tests/runners/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/tests/runners/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/tests/runners/test_staging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      412 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/tests/runners/test_transform.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2068 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/tests/test_pipeline.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1180 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/demo/tests/test_runner_selection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.784928 dynamicio-5.0.0rc4/dynamicio/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/__main__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3711 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/cli.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.788928 dynamicio-5.0.0rc4/dynamicio/config/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      134 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/config/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9530 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/config/io_config.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.788928 dynamicio-5.0.0rc4/dynamicio/config/pydantic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      408 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/config/pydantic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1415 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/config/pydantic/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9290 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/config/pydantic/io_resources.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3270 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/config/pydantic/table_schema.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13784 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/core.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3172 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5841 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/metrics.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.788928 dynamicio-5.0.0rc4/dynamicio/mixins/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      321 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/mixins/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4875 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/mixins/utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13627 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/mixins/with_kafka.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11316 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/mixins/with_local.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8015 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/mixins/with_postgres.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18850 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/mixins/with_s3.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/py.typed
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13239 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/dynamicio/validations.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.784928 dynamicio-5.0.0rc4/dynamicio.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39883 2024-05-24 09:13:15.000000 dynamicio-5.0.0rc4/dynamicio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1787 2024-05-24 09:13:15.000000 dynamicio-5.0.0rc4/dynamicio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-05-24 09:13:15.000000 dynamicio-5.0.0rc4/dynamicio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2024-05-24 09:13:15.000000 dynamicio-5.0.0rc4/dynamicio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      326 2024-05-24 09:13:15.000000 dynamicio-5.0.0rc4/dynamicio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2024-05-24 09:13:15.000000 dynamicio-5.0.0rc4/dynamicio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      705 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2024-05-24 09:13:15.792928 dynamicio-5.0.0rc4/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1924 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.788928 dynamicio-5.0.0rc4/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34498 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      469 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/constants.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.788928 dynamicio-5.0.0rc4/tests/mocking/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/mocking/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5068 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/mocking/io.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/mocking/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14102 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6425 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    43997 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_core.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6108 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_metrics.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:15.788928 dynamicio-5.0.0rc4/tests/test_mixins/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_mixins/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16626 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_mixins/test_kafka_mixins.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33927 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_mixins/test_local_mixins.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5526 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_mixins/test_mixin_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8795 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_mixins/test_postgres_mixins.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35816 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_mixins/test_s3_mixins.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      485 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_table_schema.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17759 2024-05-24 09:13:02.000000 dynamicio-5.0.0rc4/tests/test_validations.py
```

### Comparing `dynamicio-5.0.0rc3/LICENSE` & `dynamicio-5.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/PKG-INFO` & `dynamicio-5.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicio
-Version: 5.0.0rc3
+Version: 5.0.0rc4
 Summary: Panda's wrapper for IO operations
 Author: Christos Hadjinikolis, Radu Ghitescu
 Author-email: christos.hadjinikolis@gmail.com, radu.ghitescu@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicio-5.0.0rc3/README.md` & `dynamicio-5.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/demo/src/__init__.py` & `dynamicio-5.0.0rc4/demo/src/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/demo/src/__main__.py` & `dynamicio-5.0.0rc4/demo/src/__main__.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/demo/src/io.py` & `dynamicio-5.0.0rc4/demo/src/io.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/demo/src/runner_selection.py` & `dynamicio-5.0.0rc4/demo/src/runner_selection.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/demo/src/runners/staging.py` & `dynamicio-5.0.0rc4/demo/src/runners/staging.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/demo/src/runners/transform.py` & `dynamicio-5.0.0rc4/demo/src/runners/transform.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/demo/tests/conftest.py` & `dynamicio-5.0.0rc4/demo/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/demo/tests/test_pipeline.py` & `dynamicio-5.0.0rc4/demo/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/demo/tests/test_runner_selection.py` & `dynamicio-5.0.0rc4/demo/tests/test_runner_selection.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/__init__.py` & `dynamicio-5.0.0rc4/dynamicio/__init__.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/cli.py` & `dynamicio-5.0.0rc4/dynamicio/cli.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/config/io_config.py` & `dynamicio-5.0.0rc4/dynamicio/config/io_config.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/config/pydantic/config.py` & `dynamicio-5.0.0rc4/dynamicio/config/pydantic/config.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/config/pydantic/io_resources.py` & `dynamicio-5.0.0rc4/dynamicio/config/pydantic/io_resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """This module contains pylint models for physical data sources (places the bytes are being read from)."""
 
 import enum
 import posixpath
 from typing import Mapping, Optional, Union
 
 import pydantic
-from pydantic import BaseModel, model_validator
+from pydantic import BaseModel
 
 import dynamicio.config.pydantic.table_schema as table_spec
 
 
 @enum.unique
 class DataBackendType(str, enum.Enum):
     """Input file types."""
@@ -89,15 +89,15 @@
             else:
                 # Assuming an environment config
                 remapped_value["environments"][key] = value
         return remapped_value
 
 
 class IOEnvironment(BaseModel):
-    """A section specifiing an data source backed by a particular data backend."""
+    """A section specifying an data source backed by a particular data backend."""
 
     _parent: Optional[IOBinding] = None  # noqa: F821
     options: Mapping = pydantic.Field(default_factory=dict)
     data_backend_type: DataBackendType = pydantic.Field(alias="type", const=None)
 
     class Config:
         """Additional pydantic configuration for the model."""
@@ -133,15 +133,15 @@
 class LocalBatchDataSubSection(BaseModel):
     """Config section for local batch data (multiple input files)."""
 
     path_prefix: Optional[str] = None
     dynamic_file_path: Optional[str] = None
     file_type: FileType
 
-    @model_validator(mode="before")
+    @pydantic.root_validator(pre=True)
     def check_path_fields(cls, values):
         """Check that only one of path_prefix or dynamic_file_path is provided & they meet format requirements."""
         path_prefix = values.get("path_prefix")
         dynamic_file_path = values.get("dynamic_file_path")
 
         # Check for mutual exclusivity
         if path_prefix and dynamic_file_path:
@@ -184,15 +184,15 @@
     """Config section for s3 prefix data source (multiple s3 objects)."""
 
     path_prefix: Optional[str] = None
     dynamic_file_path: Optional[str] = None
     file_type: FileType
     bucket: str
 
-    @model_validator(mode="before")
+    @pydantic.root_validator(pre=True)
     def check_path_fields(cls, values):
         """Check that only one of path_prefix or dynamic_file_path is provided & they meet format requirements."""
         path_prefix = values.get("path_prefix")
         dynamic_file_path = values.get("dynamic_file_path")
 
         # Check for mutual exclusivity
         if path_prefix and dynamic_file_path:
@@ -266,8 +266,8 @@
 
 class PostgresDataEnvironment(IOEnvironment):
     """Parent section for postgres data source."""
 
     postgres: PostgresDataSubSection
 
 
-IOBinding.model_rebuild()
+IOBinding.update_forward_refs()
```

### Comparing `dynamicio-5.0.0rc3/dynamicio/config/pydantic/table_schema.py` & `dynamicio-5.0.0rc4/dynamicio/config/pydantic/table_schema.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/core.py` & `dynamicio-5.0.0rc4/dynamicio/core.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/errors.py` & `dynamicio-5.0.0rc4/dynamicio/errors.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/metrics.py` & `dynamicio-5.0.0rc4/dynamicio/metrics.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/mixins/utils.py` & `dynamicio-5.0.0rc4/dynamicio/mixins/utils.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/mixins/with_local.py` & `dynamicio-5.0.0rc4/dynamicio/mixins/with_local.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/mixins/with_postgres.py` & `dynamicio-5.0.0rc4/dynamicio/mixins/with_postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         connection_string = f"postgresql://{db_user}:{db_password}@{db_host}:{db_port}/{db_name}"
 
         assert self.sources_config.dynamicio_schema is not None, "The schema must be specified for SQL tables"
         model = self._generate_model_from_schema(self.sources_config.dynamicio_schema)
 
         is_truncate_and_append = self.options.get("truncate_and_append", False)
 
-        logger.info(f"[postgres] Started downloading table: {self.sources_config.dynamicio_schema.name} from: {db_host}:{db_name}")
+        logger.info(f"[postgres] Started uploading table: {self.sources_config.dynamicio_schema.name} from: {db_host}:{db_name}")
         with session_for(connection_string) as session:
             self._write_to_database(session, model.__tablename__, df, is_truncate_and_append)  # type: ignore
 
     @staticmethod
     def _write_to_database(session: SqlAlchemySession, table_name: str, df: pd.DataFrame, is_truncate_and_append: bool):
         """Write a dataframe to any database provided a session with a data model and a table name.
```

### Comparing `dynamicio-5.0.0rc3/dynamicio/mixins/with_s3.py` & `dynamicio-5.0.0rc4/dynamicio/mixins/with_s3.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio/validations.py` & `dynamicio-5.0.0rc4/dynamicio/validations.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/dynamicio.egg-info/PKG-INFO` & `dynamicio-5.0.0rc4/dynamicio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamicio
-Version: 5.0.0rc3
+Version: 5.0.0rc4
 Summary: Panda's wrapper for IO operations
 Author: Christos Hadjinikolis, Radu Ghitescu
 Author-email: christos.hadjinikolis@gmail.com, radu.ghitescu@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `dynamicio-5.0.0rc3/dynamicio.egg-info/SOURCES.txt` & `dynamicio-5.0.0rc4/dynamicio.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -54,8 +54,14 @@
 tests/test_config.py
 tests/test_core.py
 tests/test_metrics.py
 tests/test_table_schema.py
 tests/test_validations.py
 tests/mocking/__init__.py
 tests/mocking/io.py
-tests/mocking/models.py
+tests/mocking/models.py
+tests/test_mixins/__init__.py
+tests/test_mixins/test_kafka_mixins.py
+tests/test_mixins/test_local_mixins.py
+tests/test_mixins/test_mixin_utils.py
+tests/test_mixins/test_postgres_mixins.py
+tests/test_mixins/test_s3_mixins.py
```

### Comparing `dynamicio-5.0.0rc3/pyproject.toml` & `dynamicio-5.0.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/setup.py` & `dynamicio-5.0.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/tests/conftest.py` & `dynamicio-5.0.0rc4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/tests/mocking/io.py` & `dynamicio-5.0.0rc4/tests/mocking/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # pylint: disable=missing-class-docstring, missing-module-docstring, missing-function-docstring
+from typing import Callable, Optional
+from unittest.mock import MagicMock
 
 from dynamicio import UnifiedIO
 from dynamicio.core import SCHEMA_FROM_FILE
 
 
 class ReadS3IO(UnifiedIO):
     schema = {"id": "int64"}
@@ -113,19 +115,23 @@
 
 
 class WriteKeyedKafkaIO(UnifiedIO):
     schema = {"key": "object", "id": "object", "foo": "object", "bar": "int64", "baz": "object"}
 
 
 class MockKafkaProducer:
-    def __init__(self):
+    def __init__(self, **kwargs):
         self.my_stream = []
+        self.config = kwargs  # Store the config to ensure it can accept any options
+        self.produce_call_count = 0
 
-    def send(self, topic: str, value: dict, key: str = None):  # pylint: disable=unused-argument
+    def produce(self, topic: str, key: Optional[bytes], value: bytes, on_delivery: Callable):  # pylint: disable=unused-argument
         self.my_stream.append({"key": key, "value": value})
+        on_delivery(None, MagicMock())
+        self.produce_call_count += 1
 
     def flush(self):
         pass
 
     def close(self):
         pass
```

### Comparing `dynamicio-5.0.0rc3/tests/mocking/models.py` & `dynamicio-5.0.0rc4/tests/mocking/models.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/tests/test_cli.py` & `dynamicio-5.0.0rc4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/tests/test_config.py` & `dynamicio-5.0.0rc4/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # pylint: disable=missing-module-docstring, missing-class-docstring, missing-function-docstring, R0801
 import io
-import json
 import os
 
 import pytest
 import yaml
 
 from dynamicio.config.io_config import IOConfig, SafeDynamicResourceLoader, SafeDynamicSchemaLoader
 from tests import constants
@@ -17,15 +16,15 @@
         input_config = IOConfig(
             path_to_source_yaml=(os.path.join(constants.TEST_RESOURCES, "definitions/test_input.yaml")),
             env_identifier="LOCAL",
             dynamic_vars=constants,
         )
 
         # When
-        yaml_dict = json.loads(input_config.config.model_dump_json())
+        yaml_dict = input_config.config.dict()
         # Then
         assert yaml_dict == expected_input_yaml_dict
 
     @pytest.mark.unit
     def test_config_io_get_schema_definition_returns_a_schema_definition_from_a_source_config(self, expected_schema_definition):
         # Given
         input_config = IOConfig(
```

### Comparing `dynamicio-5.0.0rc3/tests/test_core.py` & `dynamicio-5.0.0rc4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/tests/test_metrics.py` & `dynamicio-5.0.0rc4/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dynamicio-5.0.0rc3/tests/test_validations.py` & `dynamicio-5.0.0rc4/tests/test_validations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # pylint: disable=missing-module-docstring, missing-class-docstring, missing-function-docstring, too-many-public-methods
+import os
+
 import pytest
 
+from dynamicio.config import IOConfig
 from dynamicio.validations import (
     has_acceptable_percentage_of_nulls,
     has_no_null_values,
     has_unique_values,
     is_between,
     is_greater_than,
     is_greater_than_or_equal,
     is_in,
     is_lower_than,
     is_lower_than_or_equal,
 )
+from tests import constants
+from tests.mocking.io import ReadS3CsvIO
 
 
 class TestHasUniqueValues:
     @pytest.mark.unit
     def test_returns_true_if_column_has_no_duplicate_values(self, input_df):
         # Given
         df = input_df
@@ -444,7 +449,28 @@
         df = input_df
 
         # When
         validation = is_between("TEST", df, column="weight_b", lower=4, upper=10)
 
         # Then
         assert validation.valid is True and validation.value == 0 and validation.message == "All values of TEST[weight_b] is between 4 and 10 thresholds"
+
+
+class TestRegressions:
+    """Tests for regressions discovered in v4.3.0 release."""
+
+    @pytest.mark.unit
+    def test_missing_validations_and_metrics(self):
+        """Test that dynamicio works with schemas without validations specified."""
+        # Given
+        input_config = IOConfig(
+            path_to_source_yaml=(os.path.join(constants.TEST_RESOURCES, "definitions/input.yaml")),
+            env_identifier="LOCAL",
+            dynamic_vars=constants,
+        ).get(source_key="PRODUCTS")
+        io_instance = ReadS3CsvIO(source_config=input_config, apply_schema_validations=True, log_schema_metrics=True)
+
+        # When
+        data = io_instance.read()
+
+        # Then
+        assert data.to_dict() == {"id": {0: 1, 1: 2, 2: 3, 3: 4, 4: 5, 5: 6, 6: 7, 7: 8, 8: 9, 9: 10, 10: 11, 11: 12, 12: 13, 13: 14, 14: 15}}
```

