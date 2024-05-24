# Comparing `tmp/cace-2.2.4.tar.gz` & `tmp/cace-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cace-2.2.4.tar", last modified: Thu May 23 10:10:14 2024, max compression
+gzip compressed data, was "cace-2.2.5.tar", last modified: Thu May 23 12:04:33 2024, max compression
```

## Comparing `cace-2.2.4.tar` & `cace-2.2.5.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.506706 cace-2.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.506706 cace-2.2.4/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.510706 cace-2.2.4/.github/actions/build_nix/
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-23 10:09:51.000000 cace-2.2.4/.github/actions/build_nix/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.510706 cace-2.2.4/.github/actions/check_space/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-23 10:09:51.000000 cace-2.2.4/.github/actions/check_space/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.514706 cace-2.2.4/.github/actions/setup_env/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 10:09:51.000000 cace-2.2.4/.github/actions/setup_env/action.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.514706 cace-2.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-23 10:09:51.000000 cace-2.2.4/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-05-23 10:09:51.000000 cace-2.2.4/.github/workflows/ci_nix.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 10:09:51.000000 cace-2.2.4/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-23 10:09:51.000000 cace-2.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-23 10:09:51.000000 cace-2.2.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-23 10:09:51.000000 cace-2.2.4/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-23 10:09:51.000000 cace-2.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-23 10:09:51.000000 cace-2.2.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-23 10:10:14.526706 cace-2.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-23 10:09:51.000000 cace-2.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.514706 cace-2.2.4/cace/
--rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-05-23 10:09:51.000000 cace-2.2.4/cace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-23 10:09:51.000000 cace-2.2.4/cace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-23 10:09:51.000000 cace-2.2.4/cace/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6297 2024-05-23 10:09:51.000000 cace-2.2.4/cace/cace_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    44151 2024-05-23 10:09:51.000000 cace-2.2.4/cace/cace_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.518706 cace-2.2.4/cace/common/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_calculate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_collate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26024 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_evaluate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_gensim.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14672 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_launch.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_makeplot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_measure.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10797 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_read.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46512 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_regenerate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8733 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_simulate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_unused.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    65589 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/cace_write.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7321 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/electrical_parameter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/layout_estimate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/netlist_precheck.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2540 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/physical_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/safe_eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14709 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/simulation_job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22283 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/simulation_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-05-23 10:09:51.000000 cace-2.2.4/cace/common/spiceunits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.522706 cace-2.2.4/cace/gui/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/consoletext.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29517 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/editparam.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26903 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/failreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3780 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/helpwindow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24388 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/rowwidget.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7191 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/simhints.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/textreport.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/tksimpledialog.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-23 10:09:51.000000 cace-2.2.4/cace/gui/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 10:09:51.000000 cace-2.2.4/cace/open_pdks_rev
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/cace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 10:10:14.000000 cace-2.2.4/cace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-23 10:09:51.000000 cace-2.2.4/default.nix
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.522706 cace-2.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-23 10:09:51.000000 cace-2.2.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-23 10:09:51.000000 cace-2.2.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.522706 cace-2.2.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.522706 cace-2.2.4/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/_static/cace_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/characterization.md
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.522706 cace-2.2.4/docs/source/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/dev/codebase.md
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/dev/coding_style.md
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/dev/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/docs/source/formats/
--rw-r--r--   0 runner    (1001) docker     (127)    22593 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/formats/format_description.md
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/formats/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/formats/schematic_description.md
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/docs/source/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/usage/cace_cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/usage/cace_gui.md
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/usage/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-23 10:09:51.000000 cace-2.2.4/docs/source/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-23 10:09:51.000000 cace-2.2.4/flake.lock
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-23 10:09:51.000000 cace-2.2.4/flake.nix
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/nix/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 10:09:51.000000 cace-2.2.4/nix/colab-env.nix
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-23 10:09:51.000000 cace-2.2.4/nix/create-shell.nix
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-23 10:09:51.000000 cace-2.2.4/nix/docker.nix
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-23 10:09:51.000000 cace-2.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 10:09:51.000000 cace-2.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 10:09:51.000000 cace-2.2.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 10:09:51.000000 cace-2.2.4/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:10:14.526706 cace-2.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-23 10:09:51.000000 cace-2.2.4/shell.nix
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:10:14.526706 cace-2.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 10:09:51.000000 cace-2.2.4/tests/context.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 10:09:51.000000 cace-2.2.4/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.939158 cace-2.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.919158 cace-2.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.919158 cace-2.2.5/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.923158 cace-2.2.5/.github/actions/build_nix/
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-23 12:04:08.000000 cace-2.2.5/.github/actions/build_nix/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.923158 cace-2.2.5/.github/actions/check_space/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-23 12:04:08.000000 cace-2.2.5/.github/actions/check_space/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.923158 cace-2.2.5/.github/actions/setup_env/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 12:04:08.000000 cace-2.2.5/.github/actions/setup_env/action.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.927158 cace-2.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-23 12:04:08.000000 cace-2.2.5/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10011 2024-05-23 12:04:08.000000 cace-2.2.5/.github/workflows/ci_nix.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 12:04:08.000000 cace-2.2.5/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-23 12:04:08.000000 cace-2.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-23 12:04:08.000000 cace-2.2.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-23 12:04:08.000000 cace-2.2.5/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-23 12:04:08.000000 cace-2.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-23 12:04:08.000000 cace-2.2.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-23 12:04:33.939158 cace-2.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-23 12:04:08.000000 cace-2.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.927158 cace-2.2.5/cace/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      623 2024-05-23 12:04:08.000000 cace-2.2.5/cace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-23 12:04:08.000000 cace-2.2.5/cace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-23 12:04:08.000000 cace-2.2.5/cace/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6461 2024-05-23 12:04:08.000000 cace-2.2.5/cace/cace_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44315 2024-05-23 12:04:08.000000 cace-2.2.5/cace/cace_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.931158 cace-2.2.5/cace/common/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19058 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_calculate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23616 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_collate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12819 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26024 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_evaluate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    70978 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_gensim.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14672 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_launch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_makeplot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12523 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_measure.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10797 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46512 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_regenerate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8733 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_simulate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_unused.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    65589 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/cace_write.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7321 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/electrical_parameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13039 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/layout_estimate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12310 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/netlist_precheck.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2540 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/physical_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/safe_eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14709 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/simulation_job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22283 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/simulation_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8949 2024-05-23 12:04:08.000000 cace-2.2.5/cace/common/spiceunits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.935158 cace-2.2.5/cace/gui/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1922 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/consoletext.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29517 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/editparam.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26903 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/failreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3780 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/helpwindow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24388 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/rowwidget.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7191 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/simhints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4221 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/textreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2450 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/tksimpledialog.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7674 2024-05-23 12:04:08.000000 cace-2.2.5/cace/gui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-23 12:04:08.000000 cace-2.2.5/cace/open_pdks_rev
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.939158 cace-2.2.5/cace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-23 12:04:33.000000 cace-2.2.5/cace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-23 12:04:33.000000 cace-2.2.5/cace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:04:33.000000 cace-2.2.5/cace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 12:04:33.000000 cace-2.2.5/cace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 12:04:33.000000 cace-2.2.5/cace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 12:04:33.000000 cace-2.2.5/cace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-23 12:04:08.000000 cace-2.2.5/default.nix
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.935158 cace-2.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-23 12:04:08.000000 cace-2.2.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-23 12:04:08.000000 cace-2.2.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.935158 cace-2.2.5/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.935158 cace-2.2.5/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   183493 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/_static/cace_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/characterization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.935158 cace-2.2.5/docs/source/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/dev/codebase.md
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/dev/coding_style.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/dev/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.935158 cace-2.2.5/docs/source/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)    22593 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/formats/format_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/formats/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/formats/schematic_description.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.935158 cace-2.2.5/docs/source/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/usage/cace_cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/usage/cace_gui.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/usage/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-23 12:04:08.000000 cace-2.2.5/docs/source/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-23 12:04:08.000000 cace-2.2.5/flake.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-23 12:04:08.000000 cace-2.2.5/flake.nix
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.939158 cace-2.2.5/nix/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 12:04:08.000000 cace-2.2.5/nix/colab-env.nix
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-23 12:04:08.000000 cace-2.2.5/nix/create-shell.nix
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-23 12:04:08.000000 cace-2.2.5/nix/docker.nix
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-23 12:04:08.000000 cace-2.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-23 12:04:08.000000 cace-2.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 12:04:08.000000 cace-2.2.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-23 12:04:08.000000 cace-2.2.5/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 12:04:33.939158 cace-2.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-23 12:04:08.000000 cace-2.2.5/shell.nix
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:04:33.939158 cace-2.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-23 12:04:08.000000 cace-2.2.5/tests/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 12:04:08.000000 cace-2.2.5/tests/test1.py
```

### Comparing `cace-2.2.4/.github/actions/build_nix/action.yml` & `cace-2.2.5/.github/actions/build_nix/action.yml`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/.github/actions/check_space/action.yml` & `cace-2.2.5/.github/actions/check_space/action.yml`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/.github/actions/setup_env/action.yml` & `cace-2.2.5/.github/actions/setup_env/action.yml`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/.github/workflows/ci.yaml` & `cace-2.2.5/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/.github/workflows/ci_nix.yml` & `cace-2.2.5/.github/workflows/ci_nix.yml`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/.github/workflows/pypi.yaml` & `cace-2.2.5/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/.readthedocs.yaml` & `cace-2.2.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/Changelog.md` & `cace-2.2.5/Changelog.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+# 2.2.5
+
+## CLI
+
+- Add `--version` argument
+
+## GUI
+
+- Add `--version` argument
+
 # 2.2.4
 
 ## Common
 
 - Add `markdown_summary`
 
 ## CLI
```

### Comparing `cace-2.2.4/LICENSE` & `cace-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/Makefile` & `cace-2.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/PKG-INFO` & `cace-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.2.4
+Version: 2.2.5
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.2.4 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.5 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `cace-2.2.4/README.md` & `cace-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/__init__.py` & `cace-2.2.5/cace/__init__.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/__main__.py` & `cace-2.2.5/cace/__main__.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/__version__.py` & `cace-2.2.5/cace/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = '2.2.4'
+__version__ = '2.2.5'
 
 if __name__ == '__main__':
     print(__version__, end='')
```

### Comparing `cace-2.2.4/cace/cace_cli.py` & `cace-2.2.5/cace/cace_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import os
 import sys
 import json
 import time
 import signal
 import argparse
 
+from .__version__ import __version__
+
 from .common.simulation_manager import SimulationManager
 
 
 def cli():
     """
     Read a text file in CACE (ASCII) format 4.0, run
     simulations and analysis on electrical and physical
@@ -33,14 +35,19 @@
         prog='cace',
         description="""This program parses the CACE characterization 
         file, runs simulations, and can output a modified file annotated with 
         characterization results.""",
         epilog='Online documentation at: https://cace.readthedocs.io/',
     )
 
+    # version number
+    parser.add_argument(
+        '--version', action='version', version=f'%(prog)s {__version__}'
+    )
+
     # positional argument
     parser.add_argument(
         'datasheet', nargs='?', help='format 4.0 ASCII CACE file'
     )
 
     # positional argument, optional
     parser.add_argument('outfile', nargs='?', help='name of the file to write')
```

### Comparing `cace-2.2.4/cace/cace_gui.py` & `cace-2.2.5/cace/cace_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 import argparse
 import datetime
 
 import tkinter
 from tkinter import ttk
 from tkinter import filedialog
 
+from .__version__ import __version__
+
 from .gui.style import init_style
 from .gui.tksimpledialog import *
 from .gui.tooltip import *
 from .gui.consoletext import ConsoleText
 from .gui.helpwindow import HelpWindow
 from .gui.failreport import FailReport
 from .gui.textreport import TextReport
@@ -1192,14 +1194,19 @@
     parser = argparse.ArgumentParser(
         prog='cace-gui',
         description="""Graphical interface for the Circuit Automatic Characterization Engine,
         an analog and mixed-signal design flow system.""",
         epilog='Online documentation at: https://cace.readthedocs.io/',
     )
 
+    # version number
+    parser.add_argument(
+        '--version', action='version', version=f'%(prog)s {__version__}'
+    )
+
     # positional argument, optional
     parser.add_argument(
         'datasheet',
         nargs='?',
         help='text or JSON file with the specification of the circuit',
     )
```

### Comparing `cace-2.2.4/cace/common/cace_calculate.py` & `cace-2.2.5/cace/common/cace_calculate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_collate.py` & `cace-2.2.5/cace/common/cace_collate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_compat.py` & `cace-2.2.5/cace/common/cace_compat.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_evaluate.py` & `cace-2.2.5/cace/common/cace_evaluate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_gensim.py` & `cace-2.2.5/cace/common/cace_gensim.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_launch.py` & `cace-2.2.5/cace/common/cace_launch.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_makeplot.py` & `cace-2.2.5/cace/common/cace_makeplot.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_measure.py` & `cace-2.2.5/cace/common/cace_measure.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_read.py` & `cace-2.2.5/cace/common/cace_read.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_regenerate.py` & `cace-2.2.5/cace/common/cace_regenerate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_simulate.py` & `cace-2.2.5/cace/common/cace_simulate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_unused.txt` & `cace-2.2.5/cace/common/cace_unused.txt`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/cace_write.py` & `cace-2.2.5/cace/common/cace_write.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/electrical_parameter.py` & `cace-2.2.5/cace/common/electrical_parameter.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/layout_estimate.py` & `cace-2.2.5/cace/common/layout_estimate.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/netlist_precheck.py` & `cace-2.2.5/cace/common/netlist_precheck.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/physical_parameter.py` & `cace-2.2.5/cace/common/physical_parameter.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/safe_eval.py` & `cace-2.2.5/cace/common/safe_eval.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/simulation_job.py` & `cace-2.2.5/cace/common/simulation_job.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/simulation_manager.py` & `cace-2.2.5/cace/common/simulation_manager.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/common/spiceunits.py` & `cace-2.2.5/cace/common/spiceunits.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/gui/consoletext.py` & `cace-2.2.5/cace/gui/consoletext.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/gui/editparam.py` & `cace-2.2.5/cace/gui/editparam.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/gui/failreport.py` & `cace-2.2.5/cace/gui/failreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/gui/helpwindow.py` & `cace-2.2.5/cace/gui/helpwindow.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/gui/rowwidget.py` & `cace-2.2.5/cace/gui/rowwidget.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/gui/settings.py` & `cace-2.2.5/cace/gui/settings.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/gui/simhints.py` & `cace-2.2.5/cace/gui/simhints.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/gui/style.py` & `cace-2.2.5/cace/gui/style.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/gui/textreport.py` & `cace-2.2.5/cace/gui/textreport.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/gui/tksimpledialog.py` & `cace-2.2.5/cace/gui/tksimpledialog.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace/gui/tooltip.py` & `cace-2.2.5/cace/gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/cace.egg-info/PKG-INFO` & `cace-2.2.5/cace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cace
-Version: 2.2.4
+Version: 2.2.5
 Summary: Circuit Automatic Characterization Engine
 Author-email: Tim Edwards <tim@efabless.com>, Leo Moser <leo.moser@efabless.com>
 Project-URL: Homepage, https://github.com/efabless/cace
 Project-URL: Issues, https://github.com/efabless/cace/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cace Version: 2.2.4 Summary: Circuit Automatic
+Metadata-Version: 2.1 Name: cace Version: 2.2.5 Summary: Circuit Automatic
 Characterization Engine Author-email: Tim Edwards
 efabless.com>, Leo Moser
 efabless.com> Project-URL: Homepage, https://github.com/efabless/cace Project-
 URL: Issues, https://github.com/efabless/cace/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
```

### Comparing `cace-2.2.4/cace.egg-info/SOURCES.txt` & `cace-2.2.5/cace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/default.nix` & `cace-2.2.5/default.nix`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/docs/Makefile` & `cace-2.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/docs/make.bat` & `cace-2.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/docs/source/_static/cace_screenshot.png` & `cace-2.2.5/docs/source/_static/cace_screenshot.png`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/docs/source/characterization.md` & `cace-2.2.5/docs/source/characterization.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/docs/source/conf.py` & `cace-2.2.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/docs/source/formats/format_description.md` & `cace-2.2.5/docs/source/formats/format_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/docs/source/formats/schematic_description.md` & `cace-2.2.5/docs/source/formats/schematic_description.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/docs/source/index.md` & `cace-2.2.5/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/docs/source/usage/cace_cli.md` & `cace-2.2.5/docs/source/usage/cace_cli.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/docs/source/usage/cace_gui.md` & `cace-2.2.5/docs/source/usage/cace_gui.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/docs/source/usage/getting_started.md` & `cace-2.2.5/docs/source/usage/getting_started.md`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/flake.lock` & `cace-2.2.5/flake.lock`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/flake.nix` & `cace-2.2.5/flake.nix`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/nix/colab-env.nix` & `cace-2.2.5/nix/colab-env.nix`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/nix/create-shell.nix` & `cace-2.2.5/nix/create-shell.nix`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/nix/docker.nix` & `cace-2.2.5/nix/docker.nix`

 * *Files identical despite different names*

### Comparing `cace-2.2.4/pyproject.toml` & `cace-2.2.5/pyproject.toml`

 * *Files identical despite different names*

