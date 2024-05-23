# Comparing `tmp/psi4_step-2024.5.23.1.tar.gz` & `tmp/psi4_step-2024.5.23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psi4_step-2024.5.23.1.tar", last modified: Thu May 23 15:11:25 2024, max compression
+gzip compressed data, was "psi4_step-2024.5.23.2.tar", last modified: Thu May 23 18:26:09 2024, max compression
```

## Comparing `psi4_step-2024.5.23.1.tar` & `psi4_step-2024.5.23.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:25.407536 psi4_step-2024.5.23.1/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-23 15:11:25.407536 psi4_step-2024.5.23.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:25.399536 psi4_step-2024.5.23.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:25.399536 psi4_step-2024.5.23.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:25.399536 psi4_step-2024.5.23.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9473 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:25.399536 psi4_step-2024.5.23.1/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:25.399536 psi4_step-2024.5.23.1/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:25.399536 psi4_step-2024.5.23.1/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:25.407536 psi4_step-2024.5.23.1/psi4_step/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 15:11:25.407536 psi4_step-2024.5.23.1/psi4_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    52653 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/accelerated_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/accelerated_optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/accelerated_optimization_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:25.407536 psi4_step-2024.5.23.1/psi4_step/data/
--rwxr-xr-x   0 runner    (1001) docker     (127)    12556 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/data/MOPAC_PM7_Hessian.flow
--rwxr-xr-x   0 runner    (1001) docker     (127)    11273 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/data/MOPAC_PM7_SPE.flow
--rwxr-xr-x   0 runner    (1001) docker     (127)    12933 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/data/MOPAC_PM7_surrogate.flow
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/data/opt_log.out
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/data/psi4.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/data/seamm-psi4.yml
--rw-r--r--   0 runner    (1001) docker     (127)    17818 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/initialization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/initialization_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/optimization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/optimization_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19732 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/psi4.py
--rw-r--r--   0 runner    (1001) docker     (127)    91066 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/psi4_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/psi4_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/psi4_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/thermochemistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/thermochemistry_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/thermochemistry_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/tk_accelerated_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/tk_initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/tk_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/tk_psi4.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/psi4_step/tk_thermochemistry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:25.407536 psi4_step-2024.5.23.1/psi4_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-05-23 15:11:25.000000 psi4_step-2024.5.23.1/psi4_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-23 15:11:25.000000 psi4_step-2024.5.23.1/psi4_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:11:25.000000 psi4_step-2024.5.23.1/psi4_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-23 15:11:25.000000 psi4_step-2024.5.23.1/psi4_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 15:11:25.000000 psi4_step-2024.5.23.1/psi4_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 15:11:25.000000 psi4_step-2024.5.23.1/psi4_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:11:12.000000 psi4_step-2024.5.23.1/psi4_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-23 15:11:25.407536 psi4_step-2024.5.23.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:11:25.407536 psi4_step-2024.5.23.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/tests/test_psi4_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-23 15:11:09.000000 psi4_step-2024.5.23.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:09.215137 psi4_step-2024.5.23.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-05-23 18:26:09.215137 psi4_step-2024.5.23.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:09.203137 psi4_step-2024.5.23.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:09.203137 psi4_step-2024.5.23.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    20790 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79373 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    68255 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63967 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32355 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:09.203137 psi4_step-2024.5.23.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9473 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:09.207137 psi4_step-2024.5.23.2/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:09.207137 psi4_step-2024.5.23.2/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:09.207137 psi4_step-2024.5.23.2/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:09.215137 psi4_step-2024.5.23.2/psi4_step/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 18:26:09.215137 psi4_step-2024.5.23.2/psi4_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52736 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/accelerated_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/accelerated_optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/accelerated_optimization_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:09.215137 psi4_step-2024.5.23.2/psi4_step/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12556 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/data/MOPAC_PM7_Hessian.flow
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11273 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/data/MOPAC_PM7_SPE.flow
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12933 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/data/MOPAC_PM7_surrogate.flow
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/data/opt_log.out
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/data/psi4.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/data/seamm-psi4.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/initialization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/initialization_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/optimization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/optimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19732 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/psi4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91061 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/psi4_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/psi4_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/psi4_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/thermochemistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/thermochemistry_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/thermochemistry_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/tk_accelerated_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/tk_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/tk_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/tk_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/psi4_step/tk_thermochemistry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:09.215137 psi4_step-2024.5.23.2/psi4_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-05-23 18:26:09.000000 psi4_step-2024.5.23.2/psi4_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-23 18:26:09.000000 psi4_step-2024.5.23.2/psi4_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:26:09.000000 psi4_step-2024.5.23.2/psi4_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-23 18:26:09.000000 psi4_step-2024.5.23.2/psi4_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 18:26:09.000000 psi4_step-2024.5.23.2/psi4_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 18:26:09.000000 psi4_step-2024.5.23.2/psi4_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:25:55.000000 psi4_step-2024.5.23.2/psi4_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-23 18:26:09.215137 psi4_step-2024.5.23.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:26:09.215137 psi4_step-2024.5.23.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/tests/test_psi4_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-23 18:25:52.000000 psi4_step-2024.5.23.2/versioneer.py
```

### Comparing `psi4_step-2024.5.23.1/CONTRIBUTING.rst` & `psi4_step-2024.5.23.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/HISTORY.rst` & `psi4_step-2024.5.23.2/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 =======
 History
 =======
+2024.5.23.2 -- Bugfix: incorrect name for gradients
+   * There was a typo in the name for the gradients, such that they could not be output
+     to Results.json.
+   * The units for the energy and gradients in Results.json were incorrect.
+     
 2024.5.23.1 -- Internal fix for creating Docker image.
 
 2024.5.23 -- Added standard energy and gradients to results
    * Added 'energy' and 'gradients' to optional results to support e.g. Energy Scan
    * Fixed crashing bug in description of the Energy substep.
      
 2024.3.17 -- Updated the installer
```

### Comparing `psi4_step-2024.5.23.1/LICENSE` & `psi4_step-2024.5.23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/PKG-INFO` & `psi4_step-2024.5.23.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psi4_step
-Version: 2024.5.23.1
+Version: 2024.5.23.2
 Summary: A SEAMM plug-in to setup, run and analyze quantum chemistry calculations using Psi4
 Home-page: https://github.com/molssi-seamm/psi4_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Psi4,DFT,quantum chemistry,CCSD
 Platform: Linux
@@ -96,14 +96,19 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.23.2 -- Bugfix: incorrect name for gradients
+   * There was a typo in the name for the gradients, such that they could not be output
+     to Results.json.
+   * The units for the energy and gradients in Results.json were incorrect.
+     
 2024.5.23.1 -- Internal fix for creating Docker image.
 
 2024.5.23 -- Added standard energy and gradients to results
    * Added 'energy' and 'gradients' to optional results to support e.g. Energy Scan
    * Fixed crashing bug in description of the Energy substep.
      
 2024.3.17 -- Updated the installer
```

### Comparing `psi4_step-2024.5.23.1/README.rst` & `psi4_step-2024.5.23.2/README.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/Makefile` & `psi4_step-2024.5.23.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/_static/SEAMM inverted.png` & `psi4_step-2024.5.23.2/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/_static/SEAMM logo.png` & `psi4_step-2024.5.23.2/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/_static/molssi_main_logo.png` & `psi4_step-2024.5.23.2/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/_static/molssi_main_logo_inverted_white.png` & `psi4_step-2024.5.23.2/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/_static/molssi_square.png` & `psi4_step-2024.5.23.2/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/_static/nsf.png` & `psi4_step-2024.5.23.2/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/conf.py` & `psi4_step-2024.5.23.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/developer_guide/installation.rst` & `psi4_step-2024.5.23.2/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/getting_started/index.rst` & `psi4_step-2024.5.23.2/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/index.rst` & `psi4_step-2024.5.23.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/docs/make.bat` & `psi4_step-2024.5.23.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/__init__.py` & `psi4_step-2024.5.23.2/psi4_step/__init__.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/accelerated_optimization.py` & `psi4_step-2024.5.23.2/psi4_step/accelerated_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from pathlib import Path
 import pkg_resources
 import sys
 import textwrap
 import traceback
 
 import numpy as np
-import optking
+
+# import optking
 from scipy.optimize import minimize, OptimizeResult
 from scipy.optimize._optimize import (
     _prepare_scalar_function,
     _status_message,
     _epsilon,
     vecnorm,
     _line_search_wolfe12,
@@ -259,15 +260,15 @@
                     if converged:
                         printer.normal("Converged!!!!!!")
                         break
                 else:
                     printer.normal("NOT Converged!!!!!!")
         else:
             # Iterate
-            molecule = configuration.to_qcschema_dict()
+            # molecule = configuration.to_qcschema_dict()
             optking_options = {
                 "step_type": P["optimization method"],
                 "g_convergence": P["geometry convergence"],
                 "opt_coordinates": P["coordinates"],
                 "hess_update": P["hessian update"],
             }
             if P["recalc hessian"] == "every step":
@@ -279,15 +280,16 @@
             else:
                 optking_options["full_hess_every"] = P["recalc hessian"]
 
             # "max_force_g_convergence": 4.5e-04,
             # "rms_force_g_convergence": 3.0e-04,
             # "intrafrag_hess": "SIMPLE",
 
-            optimizer = optking.CustomHelper(molecule, optking_options)
+            # optimizer = optking.CustomHelper(molecule, optking_options)
+            optimizer = None
 
             # The initial coordinates as NUMPY array. Psi4 may reorient, so need
             # to run and cache the first results
             for self.iteration in range(max_iterations + 1):
                 subdirectory = directory / f"step_{self.iteration:03d}"
                 subdirectory.mkdir(parents=True, exist_ok=True)
 
@@ -373,26 +375,27 @@
     def _surrogate_optimization(self, directory):
         """Optimize using MOPAC gradients shifted by real ones."""
         debug = False
 
         # Handle the system
         _, configuration = self.get_system_configuration()
 
-        molecule = configuration.to_qcschema_dict()
-        # "g_convergence": "gau",
-        optking_options = {
-            "opt_coordinates": "cartesian",
-            "g_convergence": "cfour",
-            "max_force_g_convergence": 4.5e-04,
-            "rms_force_g_convergence": 3.0e-04,
-            "FULL_HESS_EVERY": 1,
-            "intrafrag_hess": "SIMPLE",
-        }
+        # molecule = configuration.to_qcschema_dict()
+        # # "g_convergence": "gau",
+        # optking_options = {
+        #     "opt_coordinates": "cartesian",
+        #     "g_convergence": "cfour",
+        #     "max_force_g_convergence": 4.5e-04,
+        #     "rms_force_g_convergence": 3.0e-04,
+        #     "FULL_HESS_EVERY": 1,
+        #     "intrafrag_hess": "SIMPLE",
+        # }
         # "hess_update": "none",
-        optimizer = optking.CustomHelper(molecule, optking_options)
+        # optimizer = optking.CustomHelper(molecule, optking_options)
+        optimizer = None
 
         # First calculate the derivatives with both Psi4 and MOPAC
         xyz0 = np.array(optimizer.geom).flatten()
         factor = Q_(1.0, "a_0").m_as("Å")
 
         xyz = xyz0 * factor
         configuration.atoms.set_coordinates(xyz.reshape(configuration.n_atoms, 3))
```

### Comparing `psi4_step-2024.5.23.1/psi4_step/accelerated_optimization_parameters.py` & `psi4_step-2024.5.23.2/psi4_step/accelerated_optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/accelerated_optimization_step.py` & `psi4_step-2024.5.23.2/psi4_step/accelerated_optimization_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/data/MOPAC_PM7_Hessian.flow` & `psi4_step-2024.5.23.2/psi4_step/data/MOPAC_PM7_Hessian.flow`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/data/MOPAC_PM7_SPE.flow` & `psi4_step-2024.5.23.2/psi4_step/data/MOPAC_PM7_SPE.flow`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/data/MOPAC_PM7_surrogate.flow` & `psi4_step-2024.5.23.2/psi4_step/data/MOPAC_PM7_surrogate.flow`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/data/psi4.ini` & `psi4_step-2024.5.23.2/psi4_step/data/psi4.ini`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/data/references.bib` & `psi4_step-2024.5.23.2/psi4_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/energy.py` & `psi4_step-2024.5.23.2/psi4_step/energy.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,17 +332,19 @@
     variables[item] = array_variable(item).np.tolist()
 arrays = wfn.array_variables()
 for item in arrays:
     variables[item] = wfn.array_variable(item).np.tolist()
 variables["Eelec"] = Eelec
 variables["energy"] = Eelec
 try:
-    variables["gradient"] = np.array(G).tolist()
-except Exception:
-    pass
+    variables["gradients"] = np.array(G).tolist()
+except Exception as e:
+    print("Problem with gradients!")
+    print(e)
+
 variables["_method"] = "{method}"
 variables["_method_string"] = "{method_string}"
 
 
 with open("{filename}", "w") as fd:
     json.dump(fix_multipoles(variables), fd, sort_keys=True, indent=3)
 """
```

### Comparing `psi4_step-2024.5.23.1/psi4_step/energy_parameters.py` & `psi4_step-2024.5.23.2/psi4_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/energy_step.py` & `psi4_step-2024.5.23.2/psi4_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/initialization.py` & `psi4_step-2024.5.23.2/psi4_step/initialization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/initialization_parameters.py` & `psi4_step-2024.5.23.2/psi4_step/initialization_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/initialization_step.py` & `psi4_step-2024.5.23.2/psi4_step/initialization_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/installer.py` & `psi4_step-2024.5.23.2/psi4_step/installer.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/optimization.py` & `psi4_step-2024.5.23.2/psi4_step/optimization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/optimization_parameters.py` & `psi4_step-2024.5.23.2/psi4_step/optimization_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/optimization_step.py` & `psi4_step-2024.5.23.2/psi4_step/optimization_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/optimizer.py` & `psi4_step-2024.5.23.2/psi4_step/optimizer.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/psi4.py` & `psi4_step-2024.5.23.2/psi4_step/psi4.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/psi4_metadata.py` & `psi4_step-2024.5.23.2/psi4_step/psi4_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1625,21 +1625,21 @@
 """
 metadata["results"] = {
     "energy": {
         "description": "The total energy",
         "dimensionality": "scalar",
         "property": "total energy#Psi4#{model}",
         "type": "float",
-        "units": "kJ/mol",
+        "units": "E_h",
     },
     "gradients": {
         "description": "The gradients",
         "dimensionality": "[3, n_atoms]",
         "type": "float",
-        "units": "kJ/mol/Å",
+        "units": "E_h/a_0",
     },
     "(T) CORRECTION ENERGY": {
         "calculation": ["energy", "optimization", "thermochemistry", "vibrations"],
         "description": "",
         "dimensionality": "scalar",
         "methods": ["ccsd(t)"],
         "type": "float",
```

### Comparing `psi4_step-2024.5.23.1/psi4_step/psi4_parameters.py` & `psi4_step-2024.5.23.2/psi4_step/psi4_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/psi4_step.py` & `psi4_step-2024.5.23.2/psi4_step/psi4_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/thermochemistry.py` & `psi4_step-2024.5.23.2/psi4_step/thermochemistry.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/thermochemistry_parameters.py` & `psi4_step-2024.5.23.2/psi4_step/thermochemistry_parameters.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/thermochemistry_step.py` & `psi4_step-2024.5.23.2/psi4_step/thermochemistry_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/tk_accelerated_optimization.py` & `psi4_step-2024.5.23.2/psi4_step/tk_accelerated_optimization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/tk_energy.py` & `psi4_step-2024.5.23.2/psi4_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/tk_initialization.py` & `psi4_step-2024.5.23.2/psi4_step/tk_initialization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/tk_optimization.py` & `psi4_step-2024.5.23.2/psi4_step/tk_optimization.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/tk_psi4.py` & `psi4_step-2024.5.23.2/psi4_step/tk_psi4.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step/tk_thermochemistry.py` & `psi4_step-2024.5.23.2/psi4_step/tk_thermochemistry.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step.egg-info/PKG-INFO` & `psi4_step-2024.5.23.2/psi4_step.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psi4_step
-Version: 2024.5.23.1
+Version: 2024.5.23.2
 Summary: A SEAMM plug-in to setup, run and analyze quantum chemistry calculations using Psi4
 Home-page: https://github.com/molssi-seamm/psi4_step
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Psi4,DFT,quantum chemistry,CCSD
 Platform: Linux
@@ -96,14 +96,19 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2024.5.23.2 -- Bugfix: incorrect name for gradients
+   * There was a typo in the name for the gradients, such that they could not be output
+     to Results.json.
+   * The units for the energy and gradients in Results.json were incorrect.
+     
 2024.5.23.1 -- Internal fix for creating Docker image.
 
 2024.5.23 -- Added standard energy and gradients to results
    * Added 'energy' and 'gradients' to optional results to support e.g. Energy Scan
    * Fixed crashing bug in description of the Energy substep.
      
 2024.3.17 -- Updated the installer
```

### Comparing `psi4_step-2024.5.23.1/psi4_step.egg-info/SOURCES.txt` & `psi4_step-2024.5.23.2/psi4_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/psi4_step.egg-info/entry_points.txt` & `psi4_step-2024.5.23.2/psi4_step.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/setup.py` & `psi4_step-2024.5.23.2/setup.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/tests/test_psi4_step.py` & `psi4_step-2024.5.23.2/tests/test_psi4_step.py`

 * *Files identical despite different names*

### Comparing `psi4_step-2024.5.23.1/versioneer.py` & `psi4_step-2024.5.23.2/versioneer.py`

 * *Files identical despite different names*

