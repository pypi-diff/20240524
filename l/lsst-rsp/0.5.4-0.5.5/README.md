# Comparing `tmp/lsst_rsp-0.5.4.tar.gz` & `tmp/lsst_rsp-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_rsp-0.5.4.tar", last modified: Thu May  9 23:59:25 2024, max compression
+gzip compressed data, was "lsst_rsp-0.5.5.tar", last modified: Thu May 23 22:50:44 2024, max compression
```

## Comparing `lsst_rsp-0.5.4.tar` & `lsst_rsp-0.5.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.571536 lsst_rsp-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.563536 lsst_rsp-0.5.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/.github/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.563536 lsst_rsp-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/.github/workflows/periodic-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-09 23:59:25.571536 lsst_rsp-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.563536 lsst_rsp-0.5.4/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/changelog.d/_template.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 23:59:25.571536 lsst_rsp-0.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.559536 lsst_rsp-0.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.563536 lsst_rsp-0.5.4/src/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.563536 lsst_rsp-0.5.4/src/lsst/rsp/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.563536 lsst_rsp-0.5.4/src/lsst/rsp/startup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/startup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/startup/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/startup/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/startup/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.567536 lsst_rsp-0.5.4/src/lsst/rsp/startup/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/startup/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/startup/models/noninteractive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.567536 lsst_rsp-0.5.4/src/lsst/rsp/startup/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/startup/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28044 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/startup/services/labrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.567536 lsst_rsp-0.5.4/src/lsst/rsp/startup/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/startup/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/startup/storage/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/startup/storage/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/src/lsst/rsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.571536 lsst_rsp-0.5.4/src/lsst_rsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-09 23:59:25.000000 lsst_rsp-0.5.4/src/lsst_rsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-09 23:59:25.000000 lsst_rsp-0.5.4/src/lsst_rsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 23:59:25.000000 lsst_rsp-0.5.4/src/lsst_rsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-09 23:59:25.000000 lsst_rsp-0.5.4/src/lsst_rsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-09 23:59:25.000000 lsst_rsp-0.5.4/src/lsst_rsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-09 23:59:25.000000 lsst_rsp-0.5.4/src/lsst_rsp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.567536 lsst_rsp-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/startup_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.559536 lsst_rsp-0.5.4/tests/support/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.567536 lsst_rsp-0.5.4/tests/support/files/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.559536 lsst_rsp-0.5.4/tests/support/files/client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.559536 lsst_rsp-0.5.4/tests/support/files/client/jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.567536 lsst_rsp-0.5.4/tests/support/files/client/jupyterlab/environment/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/client/jupyterlab/environment/EXTERNAL_INSTANCE_URL
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.567536 lsst_rsp-0.5.4/tests/support/files/client/jupyterlab/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/client/jupyterlab/secrets/token
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.567536 lsst_rsp-0.5.4/tests/support/files/etc/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/etc/dircolors.ansi-universal
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.571536 lsst_rsp-0.5.4/tests/support/files/etc/skel/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/etc/skel/.gitconfig
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/etc/skel/.pythonrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.571536 lsst_rsp-0.5.4/tests/support/files/etc/skel/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/etc/skel/notebooks/.user_setups
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.559536 lsst_rsp-0.5.4/tests/support/files/homedir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.571536 lsst_rsp-0.5.4/tests/support/files/homedir/.lsst/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/homedir/.lsst/aws-credentials.ini
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/homedir/.lsst/postgres-credentials.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.559536 lsst_rsp-0.5.4/tests/support/files/stack_top/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.571536 lsst_rsp-0.5.4/tests/support/files/stack_top/jupyterlab/
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/stack_top/jupyterlab/20-logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 23:59:25.571536 lsst_rsp-0.5.4/tests/support/files/stack_top/jupyterlab/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/stack_top/jupyterlab/secrets/aws-credentials.ini
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/support/files/stack_top/jupyterlab/secrets/postgres-credentials.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tests/version_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-09 23:59:14.000000 lsst_rsp-0.5.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.274438 lsst_rsp-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.266438 lsst_rsp-0.5.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/.github/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.266438 lsst_rsp-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/.github/workflows/periodic-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-23 22:50:44.274438 lsst_rsp-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.266438 lsst_rsp-0.5.5/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/changelog.d/_template.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:50:44.274438 lsst_rsp-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.262438 lsst_rsp-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.266438 lsst_rsp-0.5.5/src/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.266438 lsst_rsp-0.5.5/src/lsst/rsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.266438 lsst_rsp-0.5.5/src/lsst/rsp/startup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/startup/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/startup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/startup/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.266438 lsst_rsp-0.5.5/src/lsst/rsp/startup/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/startup/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/startup/models/noninteractive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.270438 lsst_rsp-0.5.5/src/lsst/rsp/startup/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/startup/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27878 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/startup/services/labrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.270438 lsst_rsp-0.5.5/src/lsst/rsp/startup/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/startup/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/startup/storage/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/startup/storage/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/src/lsst/rsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.274438 lsst_rsp-0.5.5/src/lsst_rsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-23 22:50:44.000000 lsst_rsp-0.5.5/src/lsst_rsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-23 22:50:44.000000 lsst_rsp-0.5.5/src/lsst_rsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:50:44.000000 lsst_rsp-0.5.5/src/lsst_rsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-23 22:50:44.000000 lsst_rsp-0.5.5/src/lsst_rsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-23 22:50:44.000000 lsst_rsp-0.5.5/src/lsst_rsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 22:50:44.000000 lsst_rsp-0.5.5/src/lsst_rsp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.270438 lsst_rsp-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11483 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/startup_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.262438 lsst_rsp-0.5.5/tests/support/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.270438 lsst_rsp-0.5.5/tests/support/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.262438 lsst_rsp-0.5.5/tests/support/files/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.262438 lsst_rsp-0.5.5/tests/support/files/client/jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.270438 lsst_rsp-0.5.5/tests/support/files/client/jupyterlab/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/client/jupyterlab/environment/EXTERNAL_INSTANCE_URL
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.270438 lsst_rsp-0.5.5/tests/support/files/client/jupyterlab/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/client/jupyterlab/secrets/token
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.270438 lsst_rsp-0.5.5/tests/support/files/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/etc/dircolors.ansi-universal
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.270438 lsst_rsp-0.5.5/tests/support/files/etc/skel/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/etc/skel/.gitconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/etc/skel/.pythonrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.270438 lsst_rsp-0.5.5/tests/support/files/etc/skel/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/etc/skel/notebooks/.user_setups
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.262438 lsst_rsp-0.5.5/tests/support/files/homedir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.274438 lsst_rsp-0.5.5/tests/support/files/homedir/.lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/homedir/.lsst/aws-credentials.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/homedir/.lsst/postgres-credentials.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.262438 lsst_rsp-0.5.5/tests/support/files/stack_top/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.274438 lsst_rsp-0.5.5/tests/support/files/stack_top/jupyterlab/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/stack_top/jupyterlab/20-logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:50:44.274438 lsst_rsp-0.5.5/tests/support/files/stack_top/jupyterlab/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/stack_top/jupyterlab/secrets/aws-credentials.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/support/files/stack_top/jupyterlab/secrets/postgres-credentials.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tests/version_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-23 22:50:39.000000 lsst_rsp-0.5.5/tox.ini
```

### Comparing `lsst_rsp-0.5.4/.github/CONTRIBUTING.md` & `lsst_rsp-0.5.5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/.github/workflows/ci.yaml` & `lsst_rsp-0.5.5/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/.github/workflows/periodic-ci.yaml` & `lsst_rsp-0.5.5/.github/workflows/periodic-ci.yaml`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/.gitignore` & `lsst_rsp-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/.pre-commit-config.yaml` & `lsst_rsp-0.5.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/CHANGELOG.md` & `lsst_rsp-0.5.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/LICENSE` & `lsst_rsp-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/PKG-INFO` & `lsst_rsp-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-rsp
-Version: 0.5.4
+Version: 0.5.5
 Summary: Utility functions for the Rubin Science Platform
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2021-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lsst_rsp-0.5.4/README.md` & `lsst_rsp-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/pyproject.toml` & `lsst_rsp-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/__init__.py` & `lsst_rsp-0.5.5/src/lsst/rsp/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/catalog.py` & `lsst_rsp-0.5.5/src/lsst/rsp/catalog.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/client.py` & `lsst_rsp-0.5.5/src/lsst/rsp/client.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/log.py` & `lsst_rsp-0.5.5/src/lsst/rsp/log.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/service.py` & `lsst_rsp-0.5.5/src/lsst/rsp/service.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/startup/constants.py` & `lsst_rsp-0.5.5/src/lsst/rsp/startup/constants.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/startup/exceptions.py` & `lsst_rsp-0.5.5/src/lsst/rsp/startup/exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/startup/models/noninteractive.py` & `lsst_rsp-0.5.5/src/lsst/rsp/startup/models/noninteractive.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/startup/services/labrunner.py` & `lsst_rsp-0.5.5/src/lsst/rsp/startup/services/labrunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,17 +197,14 @@
         )
 
     def _set_firefly_variables(self) -> None:
         self._logger.debug("Setting firefly variables")
         firefly_route = self._env.get("FIREFLY_ROUTE", "/firefly")
         self._env["FIREFLY_URL"] = self._externalize(firefly_route)
         self._logger.debug(f"Firefly URL -> '{self._env['FIREFLY_URL']}'")
-        # This determines the landing page on the Firefly service.  For
-        # the RSP, it's always `slate.html`.
-        self._env["FIREFLY_HTML"] = "slate.html"
 
     def _force_jupyter_prefer_env_path_false(self) -> None:
         # cf https://discourse.jupyter.org/t/jupyter-paths-priority-order/7771
         # and https://jupyter-core.readthedocs.io/en/latest/changelog.html#id63
         #
         # As long as we're running from the stack Python, we need to ensure
         # this is turned off.
```

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/startup/storage/command.py` & `lsst_rsp-0.5.5/src/lsst/rsp/startup/storage/command.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/startup/storage/logging.py` & `lsst_rsp-0.5.5/src/lsst/rsp/startup/storage/logging.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst/rsp/utils.py` & `lsst_rsp-0.5.5/src/lsst/rsp/utils.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/src/lsst_rsp.egg-info/PKG-INFO` & `lsst_rsp-0.5.5/src/lsst_rsp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-rsp
-Version: 0.5.4
+Version: 0.5.5
 Summary: Utility functions for the Rubin Science Platform
 Author-email: "Association of Universities for Research in Astronomy, Inc. (AURA)" <sqre-admin@lists.lsst.org>
 License: MIT License
         
         Copyright (c) 2021-2024 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lsst_rsp-0.5.4/src/lsst_rsp.egg-info/SOURCES.txt` & `lsst_rsp-0.5.5/src/lsst_rsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/tests/client_test.py` & `lsst_rsp-0.5.5/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/tests/conftest.py` & `lsst_rsp-0.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/tests/startup_test.py` & `lsst_rsp-0.5.5/tests/startup_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,14 @@
 
 @pytest.mark.usefixtures("_rsp_env")
 def test_set_firefly_variables(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setenv("EXTERNAL_INSTANCE_URL", "https://lab.example.com:8443")
     lr = LabRunner()
     lr._set_firefly_variables()
     assert lr._env["FIREFLY_URL"] == "https://lab.example.com:8443/firefly"
-    assert lr._env["FIREFLY_HTML"] == "slate.html"
 
 
 @pytest.mark.usefixtures("_rsp_env")
 def test_force_jupyter_prefer_env_path_false() -> None:
     lr = LabRunner()
     lr._force_jupyter_prefer_env_path_false()
     assert lr._env["JUPYTER_PREFER_ENV_PATH"] == "no"
```

### Comparing `lsst_rsp-0.5.4/tests/support/files/etc/dircolors.ansi-universal` & `lsst_rsp-0.5.5/tests/support/files/etc/dircolors.ansi-universal`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/tests/support/files/stack_top/jupyterlab/20-logging.py` & `lsst_rsp-0.5.5/tests/support/files/stack_top/jupyterlab/20-logging.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/tests/utils_test.py` & `lsst_rsp-0.5.5/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `lsst_rsp-0.5.4/tox.ini` & `lsst_rsp-0.5.5/tox.ini`

 * *Files identical despite different names*

