# Comparing `tmp/beamlime-23.3.0.dev0.tar.gz` & `tmp/beamlime-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beamlime-23.3.0.dev0.tar", last modified: Thu Mar 16 15:18:05 2023, max compression
+gzip compressed data, was "beamlime-24.5.0.tar", last modified: Fri May 24 12:27:59 2024, max compression
```

## Comparing `beamlime-23.3.0.dev0.tar` & `beamlime-24.5.0.tar`

### file list

```diff
@@ -1,49 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 15:18:05.929273 beamlime-23.3.0.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 15:18:05.925273 beamlime-23.3.0.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 15:18:05.925273 beamlime-23.3.0.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      824 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1563 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1720 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      863 2023-03-16 15:18:05.929273 beamlime-23.3.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 15:18:05.929273 beamlime-23.3.0.dev0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      572 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      499 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/requirements/wheels.txt
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-03-16 15:18:05.933273 beamlime-23.3.0.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 15:18:05.925273 beamlime-23.3.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 15:18:05.929273 beamlime-23.3.0.dev0/src/beamlime/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 15:18:05.929273 beamlime-23.3.0.dev0/src/beamlime/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2292 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/config/dump.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 15:18:05.929273 beamlime-23.3.0.dev0/src/beamlime/resources/
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/default-setting.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      794 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 15:18:05.929273 beamlime-23.3.0.dev0/src/beamlime/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1366 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/templates/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      377 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/templates/data-stream-interface.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/templates/data-stream-mapping.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/templates/internal-stream.yaml
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/templates/kafka.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      747 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/templates/loaders.py
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/templates/target.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/src/beamlime/resources/templates/workflow.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-16 15:18:05.929273 beamlime-23.3.0.dev0/src/beamlime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      863 2023-03-16 15:18:05.000000 beamlime-23.3.0.dev0/src/beamlime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-03-16 15:18:05.000000 beamlime-23.3.0.dev0/src/beamlime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-16 15:18:05.000000 beamlime-23.3.0.dev0/src/beamlime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-16 15:18:05.000000 beamlime-23.3.0.dev0/src/beamlime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-16 15:18:05.000000 beamlime-23.3.0.dev0/src/beamlime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-03-16 15:17:56.000000 beamlime-23.3.0.dev0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.192670 beamlime-24.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-24 12:27:49.000000 beamlime-24.5.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.168669 beamlime-24.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-24 12:27:49.000000 beamlime-24.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.172670 beamlime-24.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-24 12:27:49.000000 beamlime-24.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-24 12:27:49.000000 beamlime-24.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-24 12:27:49.000000 beamlime-24.5.0/.github/workflows/nightly_at_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-24 12:27:49.000000 beamlime-24.5.0/.github/workflows/nightly_at_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 12:27:49.000000 beamlime-24.5.0/.github/workflows/python-version-ci
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-24 12:27:49.000000 beamlime-24.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-24 12:27:49.000000 beamlime-24.5.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-24 12:27:49.000000 beamlime-24.5.0/.github/workflows/unpinned.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-24 12:27:49.000000 beamlime-24.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-24 12:27:49.000000 beamlime-24.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-24 12:27:49.000000 beamlime-24.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-24 12:27:49.000000 beamlime-24.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-24 12:27:49.000000 beamlime-24.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 12:27:49.000000 beamlime-24.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-24 12:27:59.192670 beamlime-24.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-24 12:27:49.000000 beamlime-24.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.172670 beamlime-24.5.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-24 12:27:49.000000 beamlime-24.5.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.172670 beamlime-24.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.172670 beamlime-24.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/_static/anaconda-icon.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/_static/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.172670 beamlime-24.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/_templates/class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/_templates/module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.172670 beamlime-24.5.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/about/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14129 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/about/ess-instruments.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/about/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.172670 beamlime-24.5.0/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.172670 beamlime-24.5.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/developer/async_programming.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27547 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/developer/benchmark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/developer/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.176669 beamlime-24.5.0/docs/environments/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.176669 beamlime-24.5.0/docs/environments/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/environments/conda/dev-env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/environments/conda/test-env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/environments/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/environments/kafka.md
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.176669 beamlime-24.5.0/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/resources/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/resources/draw_logo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.176669 beamlime-24.5.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/user-guide/getting-started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-24 12:27:49.000000 beamlime-24.5.0/docs/user-guide/live_data_reduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-24 12:27:49.000000 beamlime-24.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.180670 beamlime-24.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/basetest.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/basetest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/make_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/nightly.in
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/nightly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/stream.in
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/stream.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-24 12:27:49.000000 beamlime-24.5.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.180670 beamlime-24.5.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-24 12:27:49.000000 beamlime-24.5.0/resources/draw_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-24 12:27:49.000000 beamlime-24.5.0/resources/draw_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 12:27:59.192670 beamlime-24.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.164669 beamlime-24.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.180670 beamlime-24.5.0/src/beamlime/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.184670 beamlime-24.5.0/src/beamlime/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/applications/_nexus_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/applications/_random_data_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9426 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/applications/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/applications/daemons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/applications/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.184670 beamlime-24.5.0/src/beamlime/constructors/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/constructors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/constructors/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/constructors/inspectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22444 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/constructors/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.184670 beamlime-24.5.0/src/beamlime/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/core/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/core/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/empty_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.184670 beamlime-24.5.0/src/beamlime/executables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/executables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/executables/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/executables/prototypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.184670 beamlime-24.5.0/src/beamlime/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/logging/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/logging/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/logging/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/logging/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-24 12:27:49.000000 beamlime-24.5.0/src/beamlime/stateless_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.192670 beamlime-24.5.0/src/beamlime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-24 12:27:59.000000 beamlime-24.5.0/src/beamlime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-24 12:27:59.000000 beamlime-24.5.0/src/beamlime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:27:59.000000 beamlime-24.5.0/src/beamlime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-24 12:27:59.000000 beamlime-24.5.0/src/beamlime.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 12:27:59.000000 beamlime-24.5.0/src/beamlime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 12:27:59.000000 beamlime-24.5.0/src/beamlime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.184670 beamlime-24.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.188670 beamlime-24.5.0/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/applications/multiple_modules_datagroup.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/applications/nexus_helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/applications/test_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55255 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/applications/ymir_detectors.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.188670 beamlime-24.5.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/benchmarks/loader_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/benchmarks/runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.188670 beamlime-24.5.0/tests/constructors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/constructors/factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/constructors/inspection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/constructors/provider_context_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/constructors/provider_decorator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/constructors/provider_group_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/constructors/provider_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/constructors/singleton_provider_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.188670 beamlime-24.5.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/core/schedulers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.168669 beamlime-24.5.0/tests/helpers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.188670 beamlime-24.5.0/tests/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.188670 beamlime-24.5.0/tests/helpers/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/applications/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.188670 beamlime-24.5.0/tests/helpers/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/benchmarks/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/benchmarks/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/benchmarks/ess_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/benchmarks/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/benchmarks/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/benchmarks/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.188670 beamlime-24.5.0/tests/helpers/tests/executables/
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/executables/kafka_topic_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.192670 beamlime-24.5.0/tests/helpers/tests/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/logging/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/logging/dummy_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.192670 beamlime-24.5.0/tests/helpers/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/helpers/tests/providers/preset_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:27:59.192670 beamlime-24.5.0/tests/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/logging/log_mixin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/logging/logging_resources_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/logging/logging_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-24 12:27:49.000000 beamlime-24.5.0/tests/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-24 12:27:49.000000 beamlime-24.5.0/tox.ini
```

### Comparing `beamlime-23.3.0.dev0/.pre-commit-config.yaml` & `beamlime-24.5.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,46 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.5.0
     hooks:
       - id: check-added-large-files
       - id: check-json
         exclude: asv.conf.json
+      - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
         exclude: conda/meta.yaml
       - id: detect-private-key
       - id: trailing-whitespace
         args: [ --markdown-linebreak-ext=md ]
-  - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-        name: isort (python)
-  - repo: https://github.com/psf/black
-    rev: 23.1.0
-    hooks:
-      - id: black
+        exclude: '\.svg'
   - repo: https://github.com/kynan/nbstripout
     rev: 0.6.0
     hooks:
       - id: nbstripout
         types: [ "jupyter" ]
         args: [ "--drop-empty-cells",
                 "--extra-keys 'metadata.language_info.version cell.metadata.jp-MarkdownHeadingCollapsed cell.metadata.pycharm'" ]
-  - repo: https://github.com/pycqa/flake8
-    rev: 4.0.1
-    hooks:
-      - id: flake8
-        types: ["python"]
-        additional_dependencies: ["flake8-bugbear==22.10.27"]
-  - repo: https://github.com/pycqa/bandit
-    rev: 1.7.4
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.3
     hooks:
-      - id: bandit
-        additional_dependencies: ["bandit[toml]"]
-        args: ["-c", "pyproject.toml"]
+      - id: ruff
+        args: [ --fix ]
+        types_or: [ python, pyi, jupyter ]
+      - id: ruff-format
+        types_or: [ python, pyi ]
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.6
     hooks:
       - id: codespell
         additional_dependencies:
           - tomli
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-no-eval
-        exclude: "object_list.py"
       - id: python-no-log-warn
       - id: python-use-type-annotations
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
       - id: text-unicode-replacement-char
```

### Comparing `beamlime-23.3.0.dev0/requirements/static.txt` & `beamlime-24.5.0/requirements/static.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SHA1:5a0b1bb22ae805d8aebba0f3bf05ab91aceae0d8
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
-cfgv==3.3.1
+cfgv==3.4.0
     # via pre-commit
-distlib==0.3.6
+distlib==0.3.8
     # via virtualenv
-filelock==3.9.0
+filelock==3.14.0
     # via virtualenv
-identify==2.5.18
+identify==2.5.36
     # via pre-commit
-nodeenv==1.7.0
+nodeenv==1.8.0
     # via pre-commit
-platformdirs==3.1.0
+platformdirs==4.2.2
     # via virtualenv
-pre-commit==3.1.1
+pre-commit==3.7.1
     # via -r static.in
-pyyaml==6.0
+pyyaml==6.0.1
     # via pre-commit
-virtualenv==20.20.0
+virtualenv==20.26.2
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

