# Comparing `tmp/invenio-cli-1.2.0.tar.gz` & `tmp/invenio-cli-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-cli-1.2.0.tar", last modified: Mon Oct  2 13:50:45 2023, max compression
+gzip compressed data, was "dist/invenio-cli-1.3.0.tar", last modified: Fri May 24 08:17:07 2024, max compression
```

## Comparing `invenio-cli-1.2.0.tar` & `invenio-cli-1.3.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (127)      359 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      821 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/cli/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/cli/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/cli/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/cli/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/cli/translations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     9590 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/services_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/translations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/commands/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/helpers/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/helpers/cookiecutter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/helpers/docker_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/helpers/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/helpers/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/helpers/process.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/invenio_cli/helpers/rdm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/invenio_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      837 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/commands/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1727 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/commands/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/commands/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11875 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/commands/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/commands/test_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/commands/test_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/tests/commands/testpkg/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/commands/testpkg/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 13:50:45.000000 invenio-cli-1.2.0/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/helpers/test_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/helpers/test_cookiecutter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/helpers/test_dockerhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/helpers/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/helpers/test_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-10-02 13:50:39.000000 invenio-cli-1.2.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/cli/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/cli/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/cli/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/cli/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/cli/translations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9590 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13100 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/services_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/translations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/commands/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/helpers/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/helpers/cookiecutter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/helpers/docker_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/helpers/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/helpers/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/helpers/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/invenio_cli/helpers/rdm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/invenio_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      837 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/commands/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1727 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/commands/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/commands/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/commands/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/commands/test_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/commands/test_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/tests/commands/testpkg/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/commands/testpkg/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:17:07.000000 invenio-cli-1.3.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/helpers/test_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/helpers/test_cookiecutter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/helpers/test_dockerhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/helpers/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/helpers/test_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-24 08:17:02.000000 invenio-cli-1.3.0/tests/test_cli.py
```

### Comparing `invenio-cli-1.2.0/.editorconfig` & `invenio-cli-1.3.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/CHANGES.rst` & `invenio-cli-1.3.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
     Invenio-Cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.3.0 (released 2024-05-24)
+
+- deps: pin docker to >=7.1.0 due to bug on requests
+- services: add instance path to env on setup
+
 Version 1.2.0 (released 2023-10-02)
 
 - reload on invenio.cfg changes
 
 Version 1.1.0 (released 2023-07-24)
 
 - add compatibility for docker compose v2
```

### Comparing `invenio-cli-1.2.0/CONTRIBUTING.rst` & `invenio-cli-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/LICENSE` & `invenio-cli-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/MANIFEST.in` & `invenio-cli-1.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/PKG-INFO` & `invenio-cli-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-cli
-Version: 1.2.0
+Version: 1.3.0
 Summary: "Invenio module to ease the creation and management of applications."
 Home-page: https://github.com/inveniosoftware/invenio-cli
 Author: CERN & Northwestern University
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019-2020 CERN.
@@ -108,14 +108,19 @@
         
             Invenio-Cli is free software; you can redistribute it and/or modify
             it under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.3.0 (released 2024-05-24)
+        
+        - deps: pin docker to >=7.1.0 due to bug on requests
+        - services: add instance path to env on setup
+        
         Version 1.2.0 (released 2023-10-02)
         
         - reload on invenio.cfg changes
         
         Version 1.1.0 (released 2023-07-24)
         
         - add compatibility for docker compose v2
```

### Comparing `invenio-cli-1.2.0/README.rst` & `invenio-cli-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/docs/Makefile` & `invenio-cli-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/docs/conf.py` & `invenio-cli-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/docs/index.rst` & `invenio-cli-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/docs/make.bat` & `invenio-cli-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/cli/assets.py` & `invenio-cli-1.3.0/invenio_cli/cli/assets.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/cli/cli.py` & `invenio-cli-1.3.0/invenio_cli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/cli/containers.py` & `invenio-cli-1.3.0/invenio_cli/cli/containers.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/cli/install.py` & `invenio-cli-1.3.0/invenio_cli/cli/install.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/cli/packages.py` & `invenio-cli-1.3.0/invenio_cli/cli/packages.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/cli/services.py` & `invenio-cli-1.3.0/invenio_cli/cli/services.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/cli/translations.py` & `invenio-cli-1.3.0/invenio_cli/cli/translations.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/cli/utils.py` & `invenio-cli-1.3.0/invenio_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/__init__.py` & `invenio-cli-1.3.0/invenio_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/assets.py` & `invenio-cli-1.3.0/invenio_cli/commands/assets.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/commands.py` & `invenio-cli-1.3.0/invenio_cli/commands/commands.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/containers.py` & `invenio-cli-1.3.0/invenio_cli/commands/containers.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/install.py` & `invenio-cli-1.3.0/invenio_cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/local.py` & `invenio-cli-1.3.0/invenio_cli/commands/local.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/packages.py` & `invenio-cli-1.3.0/invenio_cli/commands/packages.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/requirements.py` & `invenio-cli-1.3.0/invenio_cli/commands/requirements.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/services.py` & `invenio-cli-1.3.0/invenio_cli/commands/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio module to ease the creation and management of applications."""
 
 import click
 
 from invenio_cli.commands.translations import TranslationsCommands
+from invenio_cli.helpers.env import env
 
 from ..helpers.docker_helper import DockerHelper
 from ..helpers.process import ProcessResponse
 from ..helpers.rdm import rdm_version
 from .commands import Commands
 from .services_health import HEALTHCHECKS, ServicesHealthCommands
 from .steps import CommandStep, FunctionStep
@@ -30,15 +31,19 @@
             cli_config.get_project_shortname(), local=True
         )
 
     def ensure_containers_running(self):
         """Ensures containers are running."""
         project_shortname = self.cli_config.get_project_shortname()
 
-        self.docker_helper.start_containers()
+        instance_path = self.cli_config.get_instance_path()
+        # Set environment variable for the instance path, it might be needed by docker services
+        with env(INSTANCE_PATH=str(instance_path)):
+
+            self.docker_helper.start_containers()
 
         services = ["redis", self.cli_config.get_db_type(), "search"]
         for service in services:
             ready = ServicesHealthCommands.wait_for_service(
                 service,
                 project_shortname=project_shortname,
                 print_func=lambda msg: click.secho(msg, fg="yellow"),
```

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/services_health.py` & `invenio-cli-1.3.0/invenio_cli/commands/services_health.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/steps.py` & `invenio-cli-1.3.0/invenio_cli/commands/steps.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/translations.py` & `invenio-cli-1.3.0/invenio_cli/commands/translations.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/commands/upgrade.py` & `invenio-cli-1.3.0/invenio_cli/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/helpers/cli_config.py` & `invenio-cli-1.3.0/invenio_cli/helpers/cli_config.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/helpers/cookiecutter_wrapper.py` & `invenio-cli-1.3.0/invenio_cli/helpers/cookiecutter_wrapper.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/helpers/docker_helper.py` & `invenio-cli-1.3.0/invenio_cli/helpers/docker_helper.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/helpers/env.py` & `invenio-cli-1.3.0/invenio_cli/helpers/env.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/helpers/filesystem.py` & `invenio-cli-1.3.0/invenio_cli/helpers/filesystem.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/helpers/process.py` & `invenio-cli-1.3.0/invenio_cli/helpers/process.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli/helpers/rdm.py` & `invenio-cli-1.3.0/invenio_cli/helpers/rdm.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/invenio_cli.egg-info/PKG-INFO` & `invenio-cli-1.3.0/invenio_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-cli
-Version: 1.2.0
+Version: 1.3.0
 Summary: "Invenio module to ease the creation and management of applications."
 Home-page: https://github.com/inveniosoftware/invenio-cli
 Author: CERN & Northwestern University
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2019-2020 CERN.
@@ -108,14 +108,19 @@
         
             Invenio-Cli is free software; you can redistribute it and/or modify
             it under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 1.3.0 (released 2024-05-24)
+        
+        - deps: pin docker to >=7.1.0 due to bug on requests
+        - services: add instance path to env on setup
+        
         Version 1.2.0 (released 2023-10-02)
         
         - reload on invenio.cfg changes
         
         Version 1.1.0 (released 2023-07-24)
         
         - add compatibility for docker compose v2
```

### Comparing `invenio-cli-1.2.0/invenio_cli.egg-info/SOURCES.txt` & `invenio-cli-1.3.0/invenio_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/run-tests.sh` & `invenio-cli-1.3.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/setup.cfg` & `invenio-cli-1.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	Babel>=2.8
 	cookiecutter>=2.0.0,<2.2.0
 	click>=7.1.1,<8.2
 	click-default-group>=1.2.2,<2.0.0
-	docker>=4.1.0,<7.0.0
+	docker>=7.1.0,<8.0.0
 	pipfile>=0.0.2
 	pipenv>=2020.6.2
 	PyYAML>=5.1.2
 	pynpm>=0.1.2
 	virtualenv>=20.0.35
 
 [options.extras_require]
```

### Comparing `invenio-cli-1.2.0/tests/commands/conftest.py` & `invenio-cli-1.3.0/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/tests/commands/test_commands.py` & `invenio-cli-1.3.0/tests/commands/test_commands.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/tests/commands/test_containers.py` & `invenio-cli-1.3.0/tests/commands/test_containers.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/tests/commands/test_local.py` & `invenio-cli-1.3.0/tests/commands/test_local.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/tests/commands/test_requirements.py` & `invenio-cli-1.3.0/tests/commands/test_requirements.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/tests/commands/test_steps.py` & `invenio-cli-1.3.0/tests/commands/test_steps.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/tests/helpers/test_cli_config.py` & `invenio-cli-1.3.0/tests/helpers/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/tests/helpers/test_cookiecutter_wrapper.py` & `invenio-cli-1.3.0/tests/helpers/test_cookiecutter_wrapper.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/tests/helpers/test_dockerhelper.py` & `invenio-cli-1.3.0/tests/helpers/test_dockerhelper.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/tests/helpers/test_env.py` & `invenio-cli-1.3.0/tests/helpers/test_env.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/tests/helpers/test_filesystem.py` & `invenio-cli-1.3.0/tests/helpers/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `invenio-cli-1.2.0/tests/test_cli.py` & `invenio-cli-1.3.0/tests/test_cli.py`

 * *Files identical despite different names*

