# Comparing `tmp/pytest_logikal-3.2.0.tar.gz` & `tmp/pytest_logikal-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_logikal-3.2.0.tar", last modified: Thu May 23 18:05:51 2024, max compression
+gzip compressed data, was "pytest_logikal-3.2.1.tar", last modified: Thu May 23 19:40:10 2024, max compression
```

## Comparing `pytest_logikal-3.2.0.tar` & `pytest_logikal-3.2.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:05:51.640828 pytest_logikal-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-23 18:05:51.640828 pytest_logikal-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/entry_points.ini
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:05:51.636829 pytest_logikal-3.2.0/pytest_logikal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/bandit.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/bandit_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/black.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:05:51.636829 pytest_logikal-3.2.0/pytest_logikal/browser/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/browser/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/browser/chrome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/browser/chromium.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/browser/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/browser/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/browser/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/browser/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/css.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/css_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/file_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/isort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/js.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/js_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/migration.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/node_install.py
--rw-r--r--   0 runner    (1001) docker     (127)    98728 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/pylint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/svg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/translations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/pytest_logikal/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:05:51.640828 pytest_logikal-3.2.0/pytest_logikal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-23 18:05:51.000000 pytest_logikal-3.2.0/pytest_logikal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-23 18:05:51.000000 pytest_logikal-3.2.0/pytest_logikal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:05:51.000000 pytest_logikal-3.2.0/pytest_logikal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-23 18:05:51.000000 pytest_logikal-3.2.0/pytest_logikal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-23 18:05:51.000000 pytest_logikal-3.2.0/pytest_logikal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 18:05:51.000000 pytest_logikal-3.2.0/pytest_logikal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:05:51.636829 pytest_logikal-3.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:05:51.636829 pytest_logikal-3.2.0/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/requirements/extras/black.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/requirements/extras/browser.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-23 18:05:35.000000 pytest_logikal-3.2.0/requirements/extras/django.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:05:51.640828 pytest_logikal-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:40:10.790958 pytest_logikal-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-23 19:40:10.790958 pytest_logikal-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/entry_points.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:40:10.786958 pytest_logikal-3.2.1/pytest_logikal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/bandit_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/black.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:40:10.786958 pytest_logikal-3.2.1/pytest_logikal/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/browser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/browser/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/browser/chromium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/browser/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/browser/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/browser/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/browser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/css.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/css_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/file_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/isort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/js.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/js_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/node_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98728 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/translations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/pytest_logikal/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:40:10.790958 pytest_logikal-3.2.1/pytest_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-05-23 19:40:10.000000 pytest_logikal-3.2.1/pytest_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-23 19:40:10.000000 pytest_logikal-3.2.1/pytest_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:40:10.000000 pytest_logikal-3.2.1/pytest_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-23 19:40:10.000000 pytest_logikal-3.2.1/pytest_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-23 19:40:10.000000 pytest_logikal-3.2.1/pytest_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 19:40:10.000000 pytest_logikal-3.2.1/pytest_logikal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:40:10.786958 pytest_logikal-3.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:40:10.786958 pytest_logikal-3.2.1/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/requirements/extras/black.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/requirements/extras/browser.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-23 19:39:52.000000 pytest_logikal-3.2.1/requirements/extras/django.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:40:10.790958 pytest_logikal-3.2.1/setup.cfg
```

### Comparing `pytest_logikal-3.2.0/LICENSE.txt` & `pytest_logikal-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/PKG-INFO` & `pytest_logikal-3.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 3.2.0
+Version: 3.2.1
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -55,30 +55,27 @@
 Requires-Dist: logikal-utils~=1.1
 Requires-Dist: pyorbs~=2.1
 Requires-Dist: termcolor~=2.4
 Provides-Extra: black
 Requires-Dist: black==24.4.2; extra == "black"
 Provides-Extra: browser
 Requires-Dist: requests~=2.32; extra == "browser"
-Requires-Dist: types-requests~=2.32; extra == "browser"
 Requires-Dist: tqdm~=4.66; extra == "browser"
-Requires-Dist: types-tqdm~=4.66; extra == "browser"
 Requires-Dist: selenium==4.21.0; extra == "browser"
 Requires-Dist: xdg~=5.1; extra == "browser"
 Provides-Extra: django
 Requires-Dist: Babel~=2.14; extra == "django"
 Requires-Dist: Django~=4.2; extra == "django"
 Requires-Dist: django-stubs~=4.2; extra == "django"
 Requires-Dist: django-migration-linter~=5.1; extra == "django"
 Requires-Dist: djlint==1.34.1; extra == "django"
 Requires-Dist: pylint-django==2.5.5; extra == "django"
 Requires-Dist: pytest-django==4.8.0; extra == "django"
 Requires-Dist: pytest-factoryboy==2.7.0; extra == "django"
 Requires-Dist: requests~=2.32; extra == "django"
-Requires-Dist: types-requests~=2.32; extra == "django"
 Requires-Dist: logikal-utils[docker]~=1.1; extra == "django"
 
 pytest-logikal
 ==============
 Common tools for Python testing implemented as a `pytest <https://docs.pytest.org/>`_ plugin.
 
 Getting Started
```

### Comparing `pytest_logikal-3.2.0/entry_points.ini` & `pytest_logikal-3.2.1/entry_points.ini`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pyproject.toml` & `pytest_logikal-3.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/bandit.py` & `pytest_logikal-3.2.1/pytest_logikal/bandit.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/black.py` & `pytest_logikal-3.2.1/pytest_logikal/black.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/browser/base.py` & `pytest_logikal-3.2.1/pytest_logikal/browser/base.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/browser/chrome.py` & `pytest_logikal-3.2.1/pytest_logikal/browser/chrome.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/browser/chromium.py` & `pytest_logikal-3.2.1/pytest_logikal/browser/chromium.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/browser/edge.py` & `pytest_logikal-3.2.1/pytest_logikal/browser/edge.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/browser/plugin.py` & `pytest_logikal-3.2.1/pytest_logikal/browser/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/browser/scenarios.py` & `pytest_logikal-3.2.1/pytest_logikal/browser/scenarios.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/browser/utils.py` & `pytest_logikal-3.2.1/pytest_logikal/browser/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/build.py` & `pytest_logikal-3.2.1/pytest_logikal/build.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/core.py` & `pytest_logikal-3.2.1/pytest_logikal/core.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/css.py` & `pytest_logikal-3.2.1/pytest_logikal/css.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/css_config.yml` & `pytest_logikal-3.2.1/pytest_logikal/css_config.yml`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/django.py` & `pytest_logikal-3.2.1/pytest_logikal/django.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/docs.py` & `pytest_logikal-3.2.1/pytest_logikal/docs.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/file_checker.py` & `pytest_logikal-3.2.1/pytest_logikal/file_checker.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/html.py` & `pytest_logikal-3.2.1/pytest_logikal/html.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/isort.py` & `pytest_logikal-3.2.1/pytest_logikal/isort.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/js.py` & `pytest_logikal-3.2.1/pytest_logikal/js.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/js_config.yml` & `pytest_logikal-3.2.1/pytest_logikal/js_config.yml`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/licenses.py` & `pytest_logikal-3.2.1/pytest_logikal/licenses.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/migration.py` & `pytest_logikal-3.2.1/pytest_logikal/migration.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/node_install.py` & `pytest_logikal-3.2.1/pytest_logikal/node_install.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/package-lock.json` & `pytest_logikal-3.2.1/pytest_logikal/package-lock.json`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/plugin.py` & `pytest_logikal-3.2.1/pytest_logikal/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/pylint.py` & `pytest_logikal-3.2.1/pytest_logikal/pylint.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/requirements.py` & `pytest_logikal-3.2.1/pytest_logikal/requirements.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/style.py` & `pytest_logikal-3.2.1/pytest_logikal/style.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/svg.py` & `pytest_logikal-3.2.1/pytest_logikal/svg.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/translations.py` & `pytest_logikal-3.2.1/pytest_logikal/translations.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/utils.py` & `pytest_logikal-3.2.1/pytest_logikal/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal/validator.py` & `pytest_logikal-3.2.1/pytest_logikal/validator.py`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal.egg-info/PKG-INFO` & `pytest_logikal-3.2.1/pytest_logikal.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 3.2.0
+Version: 3.2.1
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -55,30 +55,27 @@
 Requires-Dist: logikal-utils~=1.1
 Requires-Dist: pyorbs~=2.1
 Requires-Dist: termcolor~=2.4
 Provides-Extra: black
 Requires-Dist: black==24.4.2; extra == "black"
 Provides-Extra: browser
 Requires-Dist: requests~=2.32; extra == "browser"
-Requires-Dist: types-requests~=2.32; extra == "browser"
 Requires-Dist: tqdm~=4.66; extra == "browser"
-Requires-Dist: types-tqdm~=4.66; extra == "browser"
 Requires-Dist: selenium==4.21.0; extra == "browser"
 Requires-Dist: xdg~=5.1; extra == "browser"
 Provides-Extra: django
 Requires-Dist: Babel~=2.14; extra == "django"
 Requires-Dist: Django~=4.2; extra == "django"
 Requires-Dist: django-stubs~=4.2; extra == "django"
 Requires-Dist: django-migration-linter~=5.1; extra == "django"
 Requires-Dist: djlint==1.34.1; extra == "django"
 Requires-Dist: pylint-django==2.5.5; extra == "django"
 Requires-Dist: pytest-django==4.8.0; extra == "django"
 Requires-Dist: pytest-factoryboy==2.7.0; extra == "django"
 Requires-Dist: requests~=2.32; extra == "django"
-Requires-Dist: types-requests~=2.32; extra == "django"
 Requires-Dist: logikal-utils[docker]~=1.1; extra == "django"
 
 pytest-logikal
 ==============
 Common tools for Python testing implemented as a `pytest <https://docs.pytest.org/>`_ plugin.
 
 Getting Started
```

### Comparing `pytest_logikal-3.2.0/pytest_logikal.egg-info/SOURCES.txt` & `pytest_logikal-3.2.1/pytest_logikal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/pytest_logikal.egg-info/entry_points.txt` & `pytest_logikal-3.2.1/pytest_logikal.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/requirements/build.txt.lock` & `pytest_logikal-3.2.1/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `pytest_logikal-3.2.0/requirements/dev.txt.lock` & `pytest_logikal-3.2.1/requirements/dev.txt.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: e189ad6b93754b6df783fa8060dce845e5d8090ead3f4b22f46bfc947929765a
+##  Requirements hash: b5c0c6a8423982fb191e4a4b7ce26b8ddf09f1b48516c768f10ea42127568847
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 appdirs==1.4.4
 asgiref==3.8.1
 astroid==3.2.2
```

### Comparing `pytest_logikal-3.2.0/requirements/docs.txt.lock` & `pytest_logikal-3.2.1/requirements/docs.txt.lock`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 569e4a42677a7862a3c16175b3497fe03a500929bcf719b0839e3f3cfe62d036
+##  Requirements hash: 14df854ee235c9b9ee04307d564bc3dd77ec6e5b9834525bbe7118471a0d1bfe
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 appdirs==1.4.4
 asgiref==3.8.1
 astroid==3.2.2
@@ -110,16 +110,14 @@
 tomli==2.0.1
 tomlkit==0.12.5
 tqdm==4.66.4
 trio==0.25.1
 trio-websocket==0.11.1
 types-pytz==2024.1.0.20240417
 types-PyYAML==6.0.12.20240311
-types-requests==2.32.0.20240523
-types-tqdm==4.66.0.20240417
 typing_extensions==4.11.0
 urllib3==2.2.1
 wcwidth==0.2.13
 wheel==0.43.0
 wsproto==1.2.0
 xdg==5.1.1
 zipp==3.18.2
```

