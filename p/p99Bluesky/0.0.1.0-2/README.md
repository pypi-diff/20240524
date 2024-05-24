# Comparing `tmp/p99bluesky-0.0.1.0.tar.gz` & `tmp/p99Bluesky-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p99bluesky-0.0.1.0.tar", last modified: Fri May 24 15:07:57 2024, max compression
+gzip compressed data, was "p99Bluesky-2.tar", last modified: Sat Mar 23 01:30:37 2024, max compression
```

## Comparing `p99bluesky-0.0.1.0.tar` & `p99Bluesky-2.tar`

### file list

```diff
@@ -1,108 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.741276 p99bluesky-0.0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.725276 p99bluesky-0.0.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.725276 p99bluesky-0.0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.725276 p99bluesky-0.0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.721276 p99bluesky-0.0.1.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.725276 p99bluesky-0.0.1.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.725276 p99bluesky-0.0.1.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2722 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.725276 p99bluesky-0.0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.725276 p99bluesky-0.0.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-05-24 15:07:57.741276 p99bluesky-0.0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/catalog-info.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/code
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.729276 p99bluesky-0.0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.729276 p99bluesky-0.0.1.0/docs/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.729276 p99bluesky-0.0.1.0/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/genindex.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.729276 p99bluesky-0.0.1.0/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.729276 p99bluesky-0.0.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.729276 p99bluesky-0.0.1.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.729276 p99bluesky-0.0.1.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:07:57.741276 p99bluesky-0.0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.721276 p99bluesky-0.0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.729276 p99bluesky-0.0.1.0/src/p99Bluesky/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-24 15:07:57.000000 p99bluesky-0.0.1.0/src/p99Bluesky/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.733276 p99bluesky-0.0.1.0/src/p99Bluesky/beamlines/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/beamlines/p99.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.733276 p99bluesky-0.0.1.0/src/p99Bluesky/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/devices/andor2Ad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.733276 p99bluesky-0.0.1.0/src/p99Bluesky/devices/epics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/devices/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/devices/epics/andor2_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/devices/epics/andor3_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.733276 p99bluesky-0.0.1.0/src/p99Bluesky/devices/epics/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/devices/epics/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/devices/epics/drivers/andor2_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/devices/epics/drivers/andor3_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.733276 p99bluesky-0.0.1.0/src/p99Bluesky/devices/p99/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/devices/p99/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/devices/p99/sample_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/devices/stages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.733276 p99bluesky-0.0.1.0/src/p99Bluesky/plans/
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/src/p99Bluesky/plans/ad_plans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.737276 p99bluesky-0.0.1.0/src/p99Bluesky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16575 2024-05-24 15:07:57.000000 p99bluesky-0.0.1.0/src/p99Bluesky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-24 15:07:57.000000 p99bluesky-0.0.1.0/src/p99Bluesky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:07:57.000000 p99bluesky-0.0.1.0/src/p99Bluesky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-24 15:07:57.000000 p99bluesky-0.0.1.0/src/p99Bluesky.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-24 15:07:57.000000 p99bluesky-0.0.1.0/src/p99Bluesky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 15:07:57.000000 p99bluesky-0.0.1.0/src/p99Bluesky.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.733276 p99bluesky-0.0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.733276 p99bluesky-0.0.1.0/tests/epics/
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/tests/epics/test_andor2_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:07:57.737276 p99bluesky-0.0.1.0/tests/jupyter_tests/
--rw-r--r--   0 runner    (1001) docker     (127)   368103 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/tests/jupyter_tests/andor2Ad_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/tests/jupyter_tests/andor2_controller_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/tests/jupyter_tests/andor2_driver_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   362909 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/tests/jupyter_tests/andor3Ad_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   122945 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/tests/jupyter_tests/stagetest.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/tests/test_andor2Ad.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/tests/test_p99_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-24 15:07:54.000000 p99bluesky-0.0.1.0/tests/test_stage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.165425 p99Bluesky-2/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-23 01:30:32.000000 p99Bluesky-2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.157425 p99Bluesky-2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-23 01:30:32.000000 p99Bluesky-2/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.157425 p99Bluesky-2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.157425 p99Bluesky-2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.153425 p99Bluesky-2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.157425 p99Bluesky-2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.157425 p99Bluesky-2/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2759 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.157425 p99Bluesky-2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-23 01:30:32.000000 p99Bluesky-2/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-23 01:30:32.000000 p99Bluesky-2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-23 01:30:32.000000 p99Bluesky-2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.157425 p99Bluesky-2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-23 01:30:32.000000 p99Bluesky-2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-23 01:30:32.000000 p99Bluesky-2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-23 01:30:32.000000 p99Bluesky-2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-23 01:30:32.000000 p99Bluesky-2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-23 01:30:32.000000 p99Bluesky-2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-23 01:30:32.000000 p99Bluesky-2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-03-23 01:30:37.165425 p99Bluesky-2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-23 01:30:32.000000 p99Bluesky-2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-23 01:30:32.000000 p99Bluesky-2/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.161425 p99Bluesky-2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.161425 p99Bluesky-2/docs/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.161425 p99Bluesky-2/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/genindex.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.161425 p99Bluesky-2/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.161425 p99Bluesky-2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.161425 p99Bluesky-2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.161425 p99Bluesky-2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-23 01:30:32.000000 p99Bluesky-2/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-23 01:30:32.000000 p99Bluesky-2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 01:30:37.165425 p99Bluesky-2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.153425 p99Bluesky-2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.161425 p99Bluesky-2/src/p99Bluesky/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-23 01:30:32.000000 p99Bluesky-2/src/p99Bluesky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-23 01:30:32.000000 p99Bluesky-2/src/p99Bluesky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-23 01:30:37.000000 p99Bluesky-2/src/p99Bluesky/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.165425 p99Bluesky-2/src/p99Bluesky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-03-23 01:30:37.000000 p99Bluesky-2/src/p99Bluesky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-23 01:30:37.000000 p99Bluesky-2/src/p99Bluesky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 01:30:37.000000 p99Bluesky-2/src/p99Bluesky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-23 01:30:37.000000 p99Bluesky-2/src/p99Bluesky.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-23 01:30:37.000000 p99Bluesky-2/src/p99Bluesky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-23 01:30:37.000000 p99Bluesky-2/src/p99Bluesky.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 01:30:37.165425 p99Bluesky-2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-23 01:30:32.000000 p99Bluesky-2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-23 01:30:32.000000 p99Bluesky-2/tests/test_cli.py
```

### Comparing `p99bluesky-0.0.1.0/.devcontainer/devcontainer.json` & `p99Bluesky-2/.devcontainer/devcontainer.json`

 * *Files 16% similar despite different names*

```diff
@@ -19,16 +19,15 @@
             "extensions": [
                 "ms-python.python",
                 "github.vscode-github-actions",
                 "tamasfe.even-better-toml",
                 "redhat.vscode-yaml",
                 "ryanluker.vscode-coverage-gutters",
                 "charliermarsh.ruff",
-                "ms-azuretools.vscode-docker",
-                "streetsidesoftware.code-spell-checker"
+                "ms-azuretools.vscode-docker"
             ]
         }
     },
     "features": {
         // Some default things like git config
         "ghcr.io/devcontainers/features/common-utils:2": {
             "upgradePackages": false
@@ -39,9 +38,9 @@
         "--net=host",
         // Make sure SELinux does not disable with access to host filesystems like tmp
         "--security-opt=label=disable"
     ],
     // Mount the parent as /workspaces so we can pip install peers as editable
     "workspaceMount": "source=${localWorkspaceFolder}/..,target=/workspaces,type=bind",
     // After the container is created, install the python project in editable form
-    "postCreateCommand": "git config --global --add safe.directory ${containerWorkspaceFolder} && pip install $([ -f dev-requirements.txt ] && echo '-c dev-requirements.txt') -e '.[dev]' && pre-commit install"
+    "postCreateCommand": "pip install $([ -f dev-requirements.txt ] && echo '-c dev-requirements.txt') -e '.[dev]' && pre-commit install"
 }
```

### Comparing `p99bluesky-0.0.1.0/.github/CONTRIBUTING.md` & `p99Bluesky-2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `p99Bluesky-2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `p99Bluesky-2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/.github/actions/install_requirements/action.yml` & `p99Bluesky-2/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/.github/dependabot.yml` & `p99Bluesky-2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/.github/pages/make_switcher.py` & `p99Bluesky-2/.github/pages/make_switcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import json
 import logging
 from argparse import ArgumentParser
 from pathlib import Path
 from subprocess import CalledProcessError, check_output
+from typing import List, Optional
 
 
-def report_output(stdout: bytes, label: str) -> list[str]:
+def report_output(stdout: bytes, label: str) -> List[str]:
     ret = stdout.decode().strip().split("\n")
     print(f"{label}: {ret}")
     return ret
 
 
-def get_branch_contents(ref: str) -> list[str]:
+def get_branch_contents(ref: str) -> List[str]:
     """Get the list of directories in a branch."""
     stdout = check_output(["git", "ls-tree", "-d", "--name-only", ref])
     return report_output(stdout, "Branch contents")
 
 
-def get_sorted_tags_list() -> list[str]:
+def get_sorted_tags_list() -> List[str]:
     """Get a list of sorted tags in descending order from the repository."""
     stdout = check_output(["git", "tag", "-l", "--sort=-v:refname"])
     return report_output(stdout, "Tags list")
 
 
-def get_versions(ref: str, add: str | None) -> list[str]:
+def get_versions(ref: str, add: Optional[str]) -> List[str]:
     """Generate the file containing the list of all GitHub Pages builds."""
     # Get the directories (i.e. builds) from the GitHub Pages branch
     try:
         builds = set(get_branch_contents(ref))
     except CalledProcessError:
         builds = set()
         logging.warning(f"Cannot get {ref} contents")
@@ -36,15 +37,15 @@
     if add:
         builds.add(add)
 
     # Get a sorted list of tags
     tags = get_sorted_tags_list()
 
     # Make the sorted versions list from main branches and tags
-    versions: list[str] = []
+    versions: List[str] = []
     for version in ["master", "main"] + tags:
         if version in builds:
             versions.append(version)
             builds.remove(version)
 
     # Add in anything that is left to the bottom
     versions += sorted(builds)
```

### Comparing `p99bluesky-0.0.1.0/.github/workflows/_check.yml` & `p99Bluesky-2/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/.github/workflows/_dist.yml` & `p99Bluesky-2/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/.github/workflows/_docs.yml` & `p99Bluesky-2/.github/workflows/_docs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -43,12 +43,12 @@
       - name: Write switcher.json
         run: python .github/pages/make_switcher.py --add $DOCS_VERSION ${{ github.repository }} .github/pages/switcher.json
 
       - name: Publish Docs to gh-pages
         if: github.ref_type == 'tag' || github.ref_name == 'main'
         # We pin to the SHA, not the tag, for security reasons.
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: peaceiris/actions-gh-pages@4f9cc6602d3f66b9c108549d475ec49e8ef4d45e # v4.0.0
+        uses: peaceiris/actions-gh-pages@373f7f263a76c20808c831209c920827a82a2847 # v3.9.3
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
```

### Comparing `p99bluesky-0.0.1.0/.github/workflows/_release.yml` & `p99Bluesky-2/.github/workflows/_release.yml`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,14 @@
             zip -r docs.zip $GITHUB_REF_NAME
             rm -rf $GITHUB_REF_NAME
           fi
 
       - name: Create GitHub Release
         # We pin to the SHA, not the tag, for security reasons.
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: softprops/action-gh-release@69320dbe05506a9a39fc8ae11030b214ec2d1f87 # v0.1.15
+        uses: softprops/action-gh-release@9d7c94cfd0a1f3ed45544c887983e9fa900f0564 # v0.1.15
         with:
           prerelease: ${{ contains(github.ref_name, 'a') || contains(github.ref_name, 'b') || contains(github.ref_name, 'rc') }}
           files: "*"
           generate_release_notes: true
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `p99bluesky-0.0.1.0/.github/workflows/_test.yml` & `p99Bluesky-2/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/.github/workflows/ci.yml` & `p99Bluesky-2/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
   test:
     needs: check
     if: needs.check.outputs.branch-pr == ''
     strategy:
       matrix:
         runs-on: ["ubuntu-latest"] # can add windows-latest, macos-latest
-        python-version: ["3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
         include:
           # Include one that runs in the dev environment
           - runs-on: "ubuntu-latest"
             python-version: "dev"
       fail-fast: false
     uses: ./.github/workflows/_test.yml
     with:
```

### Comparing `p99bluesky-0.0.1.0/.gitignore` & `p99Bluesky-2/.gitignore`

 * *Files 21% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 cov.xml
 .pytest_cache/
 .mypy_cache/
-.ipynb_checkpoints
+
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `p99bluesky-0.0.1.0/.pre-commit-config.yaml` & `p99Bluesky-2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/.vscode/launch.json` & `p99Bluesky-2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/LICENSE` & `p99Bluesky-2/LICENSE`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/PKG-INFO` & `p99Bluesky-2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p99Bluesky
-Version: 0.0.1.0
+Version: 2
 Summary: p99 sandbox
 Author-email: Raymond Fan <raymond.fan@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,34 +204,22 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/Relm-Arrowny/p99Bluesky
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ophyd
-Requires-Dist: ophyd-async>=0.3a5
-Requires-Dist: bluesky
-Requires-Dist: pyepics
-Requires-Dist: dataclasses-json
-Requires-Dist: pillow
-Requires-Dist: zocalo
-Requires-Dist: requests
-Requires-Dist: graypy
-Requires-Dist: pydantic
-Requires-Dist: opencv-python-headless
-Requires-Dist: aioca
-Requires-Dist: p4p
-Requires-Dist: numpy
-Requires-Dist: dls-dodal>=1.25
 Provides-Extra: dev
 Requires-Dist: copier; extra == "dev"
 Requires-Dist: myst-parser; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
@@ -239,29 +227,14 @@
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: h5py; extra == "dev"
-Requires-Dist: ipython; extra == "dev"
-Requires-Dist: ipywidgets; extra == "dev"
-Requires-Dist: matplotlib; extra == "dev"
-Requires-Dist: numpydoc; extra == "dev"
-Requires-Dist: pickleshare; extra == "dev"
-Requires-Dist: pyside6; extra == "dev"
-Requires-Dist: pytest-faulthandler; extra == "dev"
-Requires-Dist: pytest-rerunfailures; extra == "dev"
-Requires-Dist: pytest-timeout; extra == "dev"
-Requires-Dist: types-pyyaml; extra == "dev"
-Requires-Dist: jupyter; extra == "dev"
-Requires-Dist: softioc; extra == "dev"
-Requires-Dist: cothread; extra == "dev"
 
 [![CI](https://github.com/Relm-Arrowny/p99Bluesky/actions/workflows/ci.yml/badge.svg)](https://github.com/Relm-Arrowny/p99Bluesky/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/Relm-Arrowny/p99Bluesky/branch/main/graph/badge.svg)](https://codecov.io/gh/Relm-Arrowny/p99Bluesky)
 [![PyPI](https://img.shields.io/pypi/v/p99Bluesky.svg)](https://pypi.org/project/p99Bluesky)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # p99Bluesky
```

### Comparing `p99bluesky-0.0.1.0/README.md` & `p99Bluesky-2/README.md`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/docs/conf.py` & `p99Bluesky-2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `p99Bluesky-2/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/docs/images/dls-logo.svg` & `p99Bluesky-2/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/docs/index.md` & `p99Bluesky-2/docs/index.md`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/docs/tutorials/installation.md` & `p99Bluesky-2/docs/tutorials/installation.md`

 * *Files identical despite different names*

### Comparing `p99bluesky-0.0.1.0/pyproject.toml` & `p99Bluesky-2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,39 +3,26 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "p99Bluesky"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "p99 sandbox"
-dependencies = [
-    "ophyd",
-    "ophyd-async>=0.3a5",
-    "bluesky",
-    "pyepics",
-    "dataclasses-json",
-    "pillow",
-    "zocalo",
-    "requests",
-    "graypy",
-    "pydantic",
-    "opencv-python-headless", # For pin-tip detection.
-    "aioca",                  # Required for CA support with ophyd-async.
-    "p4p",                    # Required for PVA support with ophyd-async.
-    "numpy",
-    "dls-dodal>=1.25",
-]
+dependencies = [] # Add project dependencies here, e.g. ["click", "numpy"]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = [
     "copier",
     "myst-parser",
     "pipdeptree",
     "pre-commit",
@@ -45,31 +32,14 @@
     "pytest-cov",
     "ruff",
     "sphinx-autobuild",
     "sphinx-copybutton",
     "sphinx-design",
     "tox-direct",
     "types-mock",
-    "pytest-asyncio",
-    #===========================
-    "h5py",
-    "ipython",
-    "ipywidgets",
-    "matplotlib",
-    "numpydoc",
-    "pickleshare",
-    "pyside6",
-    "pytest-faulthandler",
-    "pytest-rerunfailures",
-    "pytest-timeout",
-    "types-pyyaml",
-    "jupyter",
-    "softioc",
-    "cothread",
-
 ]
 
 [project.scripts]
 p99Bluesky = "p99Bluesky.__main__:main"
 
 [project.urls]
 GitHub = "https://github.com/Relm-Arrowny/p99Bluesky"
@@ -91,16 +61,14 @@
     --tb=native -vv --doctest-modules --doctest-glob="*.rst"
     """
 # https://iscinumpy.gitlab.io/post/bound-version-constraints/#watch-for-warnings
 filterwarnings = "error"
 # Doctest python code in docs, python code in src docstrings, test functions in tests
 testpaths = "docs src tests"
 
-asyncio_mode = "auto"
-
 [tool.coverage.run]
 data_file = "/tmp/p99Bluesky.coverage"
 
 [tool.coverage.paths]
 # Tests are run from installed location, map back to the src directory
 source = ["src", "**/site-packages/"]
```

### Comparing `p99bluesky-0.0.1.0/src/p99Bluesky.egg-info/PKG-INFO` & `p99Bluesky-2/src/p99Bluesky.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p99Bluesky
-Version: 0.0.1.0
+Version: 2
 Summary: p99 sandbox
 Author-email: Raymond Fan <raymond.fan@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,34 +204,22 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/Relm-Arrowny/p99Bluesky
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ophyd
-Requires-Dist: ophyd-async>=0.3a5
-Requires-Dist: bluesky
-Requires-Dist: pyepics
-Requires-Dist: dataclasses-json
-Requires-Dist: pillow
-Requires-Dist: zocalo
-Requires-Dist: requests
-Requires-Dist: graypy
-Requires-Dist: pydantic
-Requires-Dist: opencv-python-headless
-Requires-Dist: aioca
-Requires-Dist: p4p
-Requires-Dist: numpy
-Requires-Dist: dls-dodal>=1.25
 Provides-Extra: dev
 Requires-Dist: copier; extra == "dev"
 Requires-Dist: myst-parser; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pydata-sphinx-theme>=0.12; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
@@ -239,29 +227,14 @@
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: sphinx-autobuild; extra == "dev"
 Requires-Dist: sphinx-copybutton; extra == "dev"
 Requires-Dist: sphinx-design; extra == "dev"
 Requires-Dist: tox-direct; extra == "dev"
 Requires-Dist: types-mock; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: h5py; extra == "dev"
-Requires-Dist: ipython; extra == "dev"
-Requires-Dist: ipywidgets; extra == "dev"
-Requires-Dist: matplotlib; extra == "dev"
-Requires-Dist: numpydoc; extra == "dev"
-Requires-Dist: pickleshare; extra == "dev"
-Requires-Dist: pyside6; extra == "dev"
-Requires-Dist: pytest-faulthandler; extra == "dev"
-Requires-Dist: pytest-rerunfailures; extra == "dev"
-Requires-Dist: pytest-timeout; extra == "dev"
-Requires-Dist: types-pyyaml; extra == "dev"
-Requires-Dist: jupyter; extra == "dev"
-Requires-Dist: softioc; extra == "dev"
-Requires-Dist: cothread; extra == "dev"
 
 [![CI](https://github.com/Relm-Arrowny/p99Bluesky/actions/workflows/ci.yml/badge.svg)](https://github.com/Relm-Arrowny/p99Bluesky/actions/workflows/ci.yml)
 [![Coverage](https://codecov.io/gh/Relm-Arrowny/p99Bluesky/branch/main/graph/badge.svg)](https://codecov.io/gh/Relm-Arrowny/p99Bluesky)
 [![PyPI](https://img.shields.io/pypi/v/p99Bluesky.svg)](https://pypi.org/project/p99Bluesky)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 # p99Bluesky
```

