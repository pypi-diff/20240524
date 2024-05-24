# Comparing `tmp/aapp_runner-0.10.0.tar.gz` & `tmp/aapp_runner-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aapp_runner-0.10.0.tar", last modified: Tue Jan 11 14:18:17 2022, max compression
+gzip compressed data, was "aapp_runner-0.11.0.tar", last modified: Fri May 24 09:11:42 2024, max compression
```

## Comparing `aapp_runner-0.10.0.tar` & `aapp_runner-0.11.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:18:17.466414 aapp_runner-0.10.0/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (121)     6367 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/.gitchangelog.rc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:18:17.462414 aapp_runner-0.10.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:18:17.462414 aapp_runner-0.10.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      495 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/.github/workflows/deploy-sdist.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1295 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-01-11 14:18:17.466414 aapp_runner-0.10.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1172 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/RELEASING.md
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/TODO.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:18:17.462414 aapp_runner-0.10.0/aapp_runner/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/aapp_runner_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     8515 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/config_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10188 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/do_ana_correction.py
--rw-r--r--   0 runner    (1001) docker     (121)     7801 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/do_atovpp_and_avh2hirs_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     6230 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/do_atovs_calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4115 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/do_avhrr_calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)    23276 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/do_commutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6541 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/do_hirs_calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/do_iasi_calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6735 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14290 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/read_aapp_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5548 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/rename_aapp_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:18:17.466414 aapp_runner-0.10.0/aapp_runner/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4005 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/tests/test_ana.py
--rw-r--r--   0 runner    (1001) docker     (121)    37307 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5294 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/tests/test_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4926 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/tests/test_tle_satpos_prepare.py
--rw-r--r--   0 runner    (1001) docker     (121)    26973 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/aapp_runner/tle_satpos_prepare.py
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-01-11 14:18:17.000000 aapp_runner-0.10.0/aapp_runner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:18:17.462414 aapp_runner-0.10.0/aapp_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-01-11 14:18:17.000000 aapp_runner-0.10.0/aapp_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-01-11 14:18:17.000000 aapp_runner-0.10.0/aapp_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-11 14:18:17.000000 aapp_runner-0.10.0/aapp_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-11 14:18:17.000000 aapp_runner-0.10.0/aapp_runner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-01-11 14:18:17.000000 aapp_runner-0.10.0/aapp_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-01-11 14:18:17.000000 aapp_runner-0.10.0/aapp_runner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:18:17.466414 aapp_runner-0.10.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)    35546 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/bin/aapp_dr_runner.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    30261 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/bin/test.py
--rw-r--r--   0 runner    (1001) docker     (121)    30090 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/changelog.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:18:17.466414 aapp_runner-0.10.0/continuous_integration/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/continuous_integration/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:18:17.466414 aapp_runner-0.10.0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     6005 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 14:18:17.466414 aapp_runner-0.10.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     7433 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/examples/aapp-processing.yaml-template
--rw-r--r--   0 runner    (1001) docker     (121)     3306 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/examples/aapp_config.cfg_template
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/examples/log_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-01-11 14:18:17.466414 aapp_runner-0.10.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2320 2022-01-11 14:18:12.000000 aapp_runner-0.10.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:11:42.552081 aapp_runner-0.11.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/.gitchangelog.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:11:42.544081 aapp_runner-0.11.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:11:42.544081 aapp_runner-0.11.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/.github/workflows/deploy-sdist.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-24 09:11:42.552081 aapp_runner-0.11.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/RELEASING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/TODO.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:11:42.548081 aapp_runner-0.11.0/aapp_runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/aapp_runner_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/config_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10188 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/do_ana_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/do_atovpp_and_avh2hirs_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/do_atovs_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/do_avhrr_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23276 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/do_commutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/do_hirs_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/do_iasi_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14290 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/read_aapp_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/rename_aapp_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:11:42.548081 aapp_runner-0.11.0/aapp_runner/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/tests/test_ana.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37307 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/tests/test_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/tests/test_tle_satpos_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26973 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/aapp_runner/tle_satpos_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-24 09:11:42.000000 aapp_runner-0.11.0/aapp_runner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:11:42.548081 aapp_runner-0.11.0/aapp_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-24 09:11:42.000000 aapp_runner-0.11.0/aapp_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-24 09:11:42.000000 aapp_runner-0.11.0/aapp_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:11:42.000000 aapp_runner-0.11.0/aapp_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:11:42.000000 aapp_runner-0.11.0/aapp_runner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-24 09:11:42.000000 aapp_runner-0.11.0/aapp_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 09:11:42.000000 aapp_runner-0.11.0/aapp_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:11:42.552081 aapp_runner-0.11.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35432 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/bin/aapp_dr_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30261 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/bin/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30090 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/changelog.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:11:42.552081 aapp_runner-0.11.0/continuous_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/continuous_integration/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:11:42.552081 aapp_runner-0.11.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:11:42.552081 aapp_runner-0.11.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/examples/aapp-processing.yaml-template
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/examples/aapp_config.cfg_template
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/examples/log_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-24 09:11:42.552081 aapp_runner-0.11.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-24 09:11:38.000000 aapp_runner-0.11.0/setup.py
```

### Comparing `aapp_runner-0.10.0/.gitchangelog.rc` & `aapp_runner-0.11.0/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/.github/PULL_REQUEST_TEMPLATE.md` & `aapp_runner-0.11.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/.github/workflows/ci.yaml` & `aapp_runner-0.11.0/.github/workflows/ci.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
   test:
     runs-on: ${{ matrix.os }}
     continue-on-error: ${{ matrix.experimental }}
     strategy:
       fail-fast: true
       matrix:
         os: ["ubuntu-latest", "macos-latest"]
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.10", "3.11", "3.12"]
         experimental: [false]
         include:
-          - python-version: "3.10"
+          - python-version: "3.12"
             os: "ubuntu-latest"
             experimental: true
 
     env:
       PYTHON_VERSION: ${{ matrix.python-version }}
       OS: ${{ matrix.os }}
       UNSTABLE: ${{ matrix.experimental }}
@@ -39,15 +39,14 @@
 
       - name: Install unstable dependencies
         if: matrix.experimental == true
         shell: bash -l {0}
         run: |
           python -m pip install \
           --no-deps --pre --upgrade \
-          git+https://github.com/jswhit/pygrib \
           git+https://github.com/pytroll/posttroll \
           git+https://github.com/pytroll/trollsift;
 
       - name: Install Pytroll-aapp-runner
         shell: bash -l {0}
         run: |
           pip install --no-deps -e .
```

### Comparing `aapp_runner-0.10.0/CHANGELOG.md` & `aapp_runner-0.11.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-## Version 0.9.3 (2022/01/08)
+## Version 0.11.0 (2024/05/24)
+
+
+### Pull Requests Merged
+
+#### Features added
+
+* [PR 31](https://github.com/pytroll/pytroll-aapp-runner/pull/31) - Remove unnecessary dependencies
+
+In this release 1 pull request was closed.
+
+
+## Version 0.10.0 (2022/01/08)
 
 
 ### Pull Requests Merged
 
 #### Bugs fixed
 
 * [PR 27](https://github.com/pytroll/pytroll-aapp-runner/pull/27) - Correct message level duplicate scene
```

### Comparing `aapp_runner-0.10.0/LICENSE` & `aapp_runner-0.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/PKG-INFO` & `aapp_runner-0.11.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: aapp_runner
-Version: 0.10.0
+Version: 0.11.0
 Summary: Pytroll runner for AAPP
 Home-page: https://github.com/pytroll/pytroll-aapp-runner
 Author: The Pytroll Team
 Author-email: pytroll@googlegroups.com
 License: GPLv3
-Description: pytroll-aapp-runner
-        ===================
-        
-        [![Build status](https://github.com/pytroll/pytroll-aapp-runner/workflows/CI/badge.svg?branch=main)](https://github.com/pytroll/pytroll-aapp-runner/workflows/CI/badge.svg?branch=main)
-        [![Coverage Status](https://coveralls.io/repos/github/pytroll/pytroll-aapp-runner/badge.svg?branch=main)](https://coveralls.io/github/pytroll/pytroll-aapp-runner?branch=main)
-        
-        
-        A pytroll runner supporting real-time processing of Direct Readout or regional
-        (RARS type) AVHRR and ATOVS data from level-0 to level-1 using the NWPSAF/AAPP
-        package.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
+License-File: LICENSE
+
+pytroll-aapp-runner
+===================
+
+[![Build status](https://github.com/pytroll/pytroll-aapp-runner/workflows/CI/badge.svg?branch=main)](https://github.com/pytroll/pytroll-aapp-runner/workflows/CI/badge.svg?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/pytroll/pytroll-aapp-runner/badge.svg?branch=main)](https://coveralls.io/github/pytroll/pytroll-aapp-runner?branch=main)
+
+
+A pytroll runner supporting real-time processing of Direct Readout or regional
+(RARS type) AVHRR and ATOVS data from level-0 to level-1 using the NWPSAF/AAPP
+package.
+
```

### Comparing `aapp_runner-0.10.0/README.md` & `aapp_runner-0.11.0/README.md`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/RELEASING.md` & `aapp_runner-0.11.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/__init__.py` & `aapp_runner-0.11.0/aapp_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/aapp_runner_tools.py` & `aapp_runner-0.11.0/aapp_runner/aapp_runner_tools.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/config_helpers.py` & `aapp_runner-0.11.0/aapp_runner/config_helpers.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/do_ana_correction.py` & `aapp_runner-0.11.0/aapp_runner/do_ana_correction.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/do_atovpp_and_avh2hirs_processing.py` & `aapp_runner-0.11.0/aapp_runner/do_atovpp_and_avh2hirs_processing.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/do_atovs_calibration.py` & `aapp_runner-0.11.0/aapp_runner/do_atovs_calibration.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/do_avhrr_calibration.py` & `aapp_runner-0.11.0/aapp_runner/do_avhrr_calibration.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/do_commutation.py` & `aapp_runner-0.11.0/aapp_runner/do_commutation.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/do_hirs_calibration.py` & `aapp_runner-0.11.0/aapp_runner/do_hirs_calibration.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/do_iasi_calibration.py` & `aapp_runner-0.11.0/aapp_runner/do_iasi_calibration.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/exceptions.py` & `aapp_runner-0.11.0/aapp_runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/helper_functions.py` & `aapp_runner-0.11.0/aapp_runner/helper_functions.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/read_aapp_config.py` & `aapp_runner-0.11.0/aapp_runner/read_aapp_config.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/rename_aapp_filenames.py` & `aapp_runner-0.11.0/aapp_runner/rename_aapp_filenames.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/tests/test_ana.py` & `aapp_runner-0.11.0/aapp_runner/tests/test_ana.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/tests/test_config.py` & `aapp_runner-0.11.0/aapp_runner/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/tests/test_helper_functions.py` & `aapp_runner-0.11.0/aapp_runner/tests/test_helper_functions.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/tests/test_tle_satpos_prepare.py` & `aapp_runner-0.11.0/aapp_runner/tests/test_tle_satpos_prepare.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner/tle_satpos_prepare.py` & `aapp_runner-0.11.0/aapp_runner/tle_satpos_prepare.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/aapp_runner.egg-info/PKG-INFO` & `aapp_runner-0.11.0/aapp_runner.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: aapp-runner
-Version: 0.10.0
+Version: 0.11.0
 Summary: Pytroll runner for AAPP
 Home-page: https://github.com/pytroll/pytroll-aapp-runner
 Author: The Pytroll Team
 Author-email: pytroll@googlegroups.com
 License: GPLv3
-Description: pytroll-aapp-runner
-        ===================
-        
-        [![Build status](https://github.com/pytroll/pytroll-aapp-runner/workflows/CI/badge.svg?branch=main)](https://github.com/pytroll/pytroll-aapp-runner/workflows/CI/badge.svg?branch=main)
-        [![Coverage Status](https://coveralls.io/repos/github/pytroll/pytroll-aapp-runner/badge.svg?branch=main)](https://coveralls.io/github/pytroll/pytroll-aapp-runner?branch=main)
-        
-        
-        A pytroll runner supporting real-time processing of Direct Readout or regional
-        (RARS type) AVHRR and ATOVS data from level-0 to level-1 using the NWPSAF/AAPP
-        package.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
+License-File: LICENSE
+
+pytroll-aapp-runner
+===================
+
+[![Build status](https://github.com/pytroll/pytroll-aapp-runner/workflows/CI/badge.svg?branch=main)](https://github.com/pytroll/pytroll-aapp-runner/workflows/CI/badge.svg?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/pytroll/pytroll-aapp-runner/badge.svg?branch=main)](https://coveralls.io/github/pytroll/pytroll-aapp-runner?branch=main)
+
+
+A pytroll runner supporting real-time processing of Direct Readout or regional
+(RARS type) AVHRR and ATOVS data from level-0 to level-1 using the NWPSAF/AAPP
+package.
+
```

### Comparing `aapp_runner-0.10.0/aapp_runner.egg-info/SOURCES.txt` & `aapp_runner-0.11.0/aapp_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/bin/aapp_dr_runner.py` & `aapp_runner-0.11.0/bin/aapp_dr_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -697,16 +697,15 @@
         LOG.debug("Handeling file for sending: {}".format(file))
         msg_to_send = {}
         try:
             msg_to_send = msg.data.copy()
             if 'dataset' in msg_to_send:
                 del msg_to_send['dataset']
 
-            msg_to_send['uri'] = "file://{}{}".format(config['aapp_processes'][
-                config.process_name]['message_providing_server'], file['file'])
+            msg_to_send['uri'] = file['file']
 
             msg_to_send['filename'] = os.path.basename(file['file'])
             msg_to_send['uid'] = os.path.basename(file['file'])
             msg_to_send['sensor'] = config['aapp_static_configuration']['sensor_name_converter'].get(
                 file['sensor'], file['sensor'])
             msg_to_send['orbit_number'] = config['orbit_number']
             msg_to_send['format'] = "AAPP"
```

### Comparing `aapp_runner-0.10.0/bin/test.py` & `aapp_runner-0.11.0/bin/test.py`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/changelog.rst` & `aapp_runner-0.11.0/changelog.rst`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/doc/index.rst` & `aapp_runner-0.11.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/examples/aapp-processing.yaml-template` & `aapp_runner-0.11.0/examples/aapp-processing.yaml-template`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/examples/aapp_config.cfg_template` & `aapp_runner-0.11.0/examples/aapp_config.cfg_template`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/examples/log_config.yaml` & `aapp_runner-0.11.0/examples/log_config.yaml`

 * *Files identical despite different names*

### Comparing `aapp_runner-0.10.0/setup.py` & `aapp_runner-0.11.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 with open('./README.md', 'r') as fd:
     long_description = fd.read()
 
 description = 'Pytroll runner for AAPP'
 
-requires = ['posttroll', 'netifaces', 'trollsift', 'pytroll-schedule', 'setuptools_scm']
+requires = ['posttroll', 'trollsift', 'setuptools_scm']
 test_requires = ['mock']
 
 
 setup(name="aapp_runner",
       description=description,
       author='The Pytroll Team',
       author_email='pytroll@googlegroups.com',
```

