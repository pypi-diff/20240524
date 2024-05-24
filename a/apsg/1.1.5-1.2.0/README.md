# Comparing `tmp/apsg-1.1.5.tar.gz` & `tmp/apsg-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apsg-1.1.5.tar", last modified: Wed May 15 10:32:58 2024, max compression
+gzip compressed data, was "apsg-1.2.0.tar", last modified: Fri May 24 19:34:50 2024, max compression
```

## Comparing `apsg-1.1.5.tar` & `apsg-1.2.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.700753 apsg-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-15 10:32:50.000000 apsg-1.1.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-15 10:32:50.000000 apsg-1.1.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-05-15 10:32:50.000000 apsg-1.1.5/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-15 10:32:50.000000 apsg-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-15 10:32:50.000000 apsg-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-05-15 10:32:58.700753 apsg-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-15 10:32:50.000000 apsg-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.688753 apsg-1.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.database.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.feature.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.helpers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.math.rst
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.pandas.rst
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/apsg.plotting.rst
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/automodules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-15 10:32:50.000000 apsg-1.1.5/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-15 10:32:50.000000 apsg-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-15 10:32:58.700753 apsg-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-15 10:32:50.000000 apsg-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.684753 apsg-1.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.688753 apsg-1.1.5/src/apsg/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.692753 apsg-1.1.5/src/apsg/database/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/database/_alchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/database/_sdbread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.692753 apsg-1.1.5/src/apsg/decorator/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/decorator/_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.692753 apsg-1.1.5/src/apsg/feature/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56059 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_geodata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_paleomag.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_tensor2.py
--rw-r--r--   0 runner    (1001) docker     (127)    27973 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/feature/_tensor3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.692753 apsg-1.1.5/src/apsg/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/helpers/_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/helpers/_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/helpers/_notation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.696753 apsg-1.1.5/src/apsg/math/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/math/_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    16476 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/math/_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.696753 apsg-1.1.5/src/apsg/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/pandas/_pandas_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.696753 apsg-1.1.5/src/apsg/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_fabricplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_paleomagplots.py
--rw-r--r--   0 runner    (1001) docker     (127)    21059 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_plot_artists.py
--rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_projection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12809 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_roseplot.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_stereogrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    36506 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/plotting/_stereonet.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 10:32:50.000000 apsg-1.1.5/src/apsg/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.696753 apsg-1.1.5/src/apsg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15153 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 10:32:58.000000 apsg-1.1.5/src/apsg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:58.696753 apsg-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 10:32:50.000000 apsg-1.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-15 10:32:50.000000 apsg-1.1.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-05-15 10:32:50.000000 apsg-1.1.5/tests/test_apsg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-15 10:32:50.000000 apsg-1.1.5/tests/test_tensors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.911320 apsg-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-24 19:34:42.000000 apsg-1.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-24 19:34:42.000000 apsg-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-24 19:34:42.000000 apsg-1.2.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-24 19:34:42.000000 apsg-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-24 19:34:42.000000 apsg-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-05-24 19:34:50.911320 apsg-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-24 19:34:42.000000 apsg-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.903319 apsg-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/apsg.database.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/apsg.feature.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/apsg.helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/apsg.math.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/apsg.pandas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/apsg.plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/automodules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-24 19:34:42.000000 apsg-1.2.0/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-24 19:34:42.000000 apsg-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-24 19:34:50.915320 apsg-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-24 19:34:42.000000 apsg-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.899319 apsg-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.903319 apsg-1.2.0/src/apsg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.907319 apsg-1.2.0/src/apsg/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/database/_alchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/database/_sdbread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.907319 apsg-1.2.0/src/apsg/decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/decorator/_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.907319 apsg-1.2.0/src/apsg/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56059 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/feature/_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/feature/_geodata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14911 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/feature/_paleomag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/feature/_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/feature/_tensor2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27973 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/feature/_tensor3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.907319 apsg-1.2.0/src/apsg/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/helpers/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/helpers/_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/helpers/_notation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.907319 apsg-1.2.0/src/apsg/math/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/math/_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16476 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/math/_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.911320 apsg-1.2.0/src/apsg/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/pandas/_pandas_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.911320 apsg-1.2.0/src/apsg/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18863 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/plotting/_fabricplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/plotting/_paleomagplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21059 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/plotting/_plot_artists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/plotting/_projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12809 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/plotting/_roseplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/plotting/_stereogrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36489 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/plotting/_stereonet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-24 19:34:42.000000 apsg-1.2.0/src/apsg/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.911320 apsg-1.2.0/src/apsg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-05-24 19:34:50.000000 apsg-1.2.0/src/apsg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-24 19:34:50.000000 apsg-1.2.0/src/apsg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:34:50.000000 apsg-1.2.0/src/apsg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-24 19:34:50.000000 apsg-1.2.0/src/apsg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-24 19:34:50.000000 apsg-1.2.0/src/apsg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 19:34:50.000000 apsg-1.2.0/src/apsg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:50.911320 apsg-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:34:42.000000 apsg-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-24 19:34:42.000000 apsg-1.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-05-24 19:34:42.000000 apsg-1.2.0/tests/test_apsg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-24 19:34:42.000000 apsg-1.2.0/tests/test_tensors.py
```

### Comparing `apsg-1.1.5/CONTRIBUTING.md` & `apsg-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/HISTORY.md` & `apsg-1.2.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changes
 
+### 1.2.0 (master)
+ * sqlalchemy and pandas added to requirements
+ * quicknet fault bug fixed
+
 ### 1.1.5 (May 15 2024)
  * paleomag Core .dd bug fixed
  * fix round-off domain math error for acosd and asind
 
 ### 1.1.4 (Dec 13 2023)
  * Ellipsoid repr bugfix
```

### Comparing `apsg-1.1.5/LICENSE` & `apsg-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/PKG-INFO` & `apsg-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsg
-Version: 1.1.5
+Version: 1.2.0
 Summary: APSG - The package for structural geologists
 Home-page: https://github.com/ondrolexa/apsg
 Author: Ondrej Lexa
 Author-email: lexa.ondrej@gmail.com
 License: MIT
 Project-URL: Documentation, https://apsg.readthedocs.io/
 Project-URL: Source Code, https://github.com/ondrolexa/apsg/
@@ -19,24 +19,25 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
+Requires-Dist: sqlalchemy
+Requires-Dist: pandas
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: ipykernel; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: black; extra == "test"
 Provides-Extra: extra
 Requires-Dist: jupyterlab; extra == "extra"
-Requires-Dist: pandas; extra == "extra"
 
 <img src="https://ondrolexa.github.io/apsg/apsg_banner.svg" alt="APSG logo" width="300px"/>
 
 [![PyPI - Version](https://img.shields.io/pypi/v/apsg)](https://pypi.org/project/apsg)
 [![Conda](https://img.shields.io/conda/v/conda-forge/apsg)](https://anaconda.org/conda-forge/apsg)
 [![Documentation Status](https://readthedocs.org/projects/apsg/badge/?version=stable)](https://apsg.readthedocs.io/en/stable/?badge=stable)
 [![DOI](https://zenodo.org/badge/24879346.svg)](https://zenodo.org/badge/latestdoi/24879346)
@@ -135,14 +136,18 @@
 ## License
 
 APSG is free software: you can redistribute it and/or modify it under the terms of the MIT License. A copy of this license is provided in ``LICENSE`` file.
 
 
 # Changes
 
+### 1.2.0 (master)
+ * sqlalchemy and pandas added to requirements
+ * quicknet fault bug fixed
+
 ### 1.1.5 (May 15 2024)
  * paleomag Core .dd bug fixed
  * fix round-off domain math error for acosd and asind
 
 ### 1.1.4 (Dec 13 2023)
  * Ellipsoid repr bugfix
```

### Comparing `apsg-1.1.5/README.md` & `apsg-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/docs/Makefile` & `apsg-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/docs/apsg.database.rst` & `apsg-1.2.0/docs/apsg.database.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/docs/conf.py` & `apsg-1.2.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,17 +65,17 @@
 copyright = "2023, Ondrej Lexa"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = "1.1"
+version = "1.2"
 # The full version, including alpha/beta/rc tags.
-release = "1.1.5"
+release = "1.2.0"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to
 # some non-false value, then it is used:
```

### Comparing `apsg-1.1.5/docs/contributing.rst` & `apsg-1.2.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/docs/index.rst` & `apsg-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/docs/installation.rst` & `apsg-1.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/docs/make.bat` & `apsg-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/setup.py` & `apsg-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open(path.join(CURRENT_PATH, "HISTORY.md")) as file:
     history = file.read()
 
 setup(
     name="apsg",
-    version="1.1.5",
+    version="1.2.0",
     description="APSG - The package for structural geologists",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/markdown",
     author="Ondrej Lexa",
     author_email="lexa.ondrej@gmail.com",
     url="https://github.com/ondrolexa/apsg",
     license="MIT",
@@ -33,19 +33,19 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
     ],
     packages=find_packages(where="src"),
     package_dir={"": "src"},
-    install_requires=["numpy", "matplotlib", "scipy"],
+    install_requires=["numpy", "matplotlib", "scipy", "sqlalchemy", "pandas"],
     extras_require={
         "docs": ["sphinx", "ipykernel", "nbsphinx"],
         "test": ["pytest", "black"],
-        "extra": ["jupyterlab", "pandas"],
+        "extra": ["jupyterlab"],
     },
     project_urls={
         "Documentation": "https://apsg.readthedocs.io/",
         "Source Code": "https://github.com/ondrolexa/apsg/",
         "Bug Tracker": "https://github.com/ondrolexa/apsg/issues/",
     },
     entry_points="""
```

### Comparing `apsg-1.1.5/src/apsg/__init__.py` & `apsg-1.2.0/src/apsg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,10 +94,10 @@
     "VollmerPlot",
     "RamsayPlot",
     "FlinnPlot",
     "HsuPlot",
     "quicknet",
 )
 
-__version__ = "1.1.5"
+__version__ = "1.2.0"
 __author__ = "Ondrej Lexa"
 __email__ = "lexa.ondrej@gmail.com"
```

### Comparing `apsg-1.1.5/src/apsg/config.py` & `apsg-1.2.0/src/apsg/config.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/database/_alchemy.py` & `apsg-1.2.0/src/apsg/database/_alchemy.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/database/_sdbread.py` & `apsg-1.2.0/src/apsg/database/_sdbread.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/decorator/_decorator.py` & `apsg-1.2.0/src/apsg/decorator/_decorator.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/feature/__init__.py` & `apsg-1.2.0/src/apsg/feature/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/feature/_container.py` & `apsg-1.2.0/src/apsg/feature/_container.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/feature/_geodata.py` & `apsg-1.2.0/src/apsg/feature/_geodata.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/feature/_paleomag.py` & `apsg-1.2.0/src/apsg/feature/_paleomag.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/feature/_statistics.py` & `apsg-1.2.0/src/apsg/feature/_statistics.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/feature/_tensor2.py` & `apsg-1.2.0/src/apsg/feature/_tensor2.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/feature/_tensor3.py` & `apsg-1.2.0/src/apsg/feature/_tensor3.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/helpers/__init__.py` & `apsg-1.2.0/src/apsg/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/helpers/_math.py` & `apsg-1.2.0/src/apsg/helpers/_math.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/helpers/_notation.py` & `apsg-1.2.0/src/apsg/helpers/_notation.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/math/_matrix.py` & `apsg-1.2.0/src/apsg/math/_matrix.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/math/_vector.py` & `apsg-1.2.0/src/apsg/math/_vector.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/pandas/_pandas_api.py` & `apsg-1.2.0/src/apsg/pandas/_pandas_api.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/plotting/__init__.py` & `apsg-1.2.0/src/apsg/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/plotting/_fabricplot.py` & `apsg-1.2.0/src/apsg/plotting/_fabricplot.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/plotting/_paleomagplots.py` & `apsg-1.2.0/src/apsg/plotting/_paleomagplots.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/plotting/_plot_artists.py` & `apsg-1.2.0/src/apsg/plotting/_plot_artists.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/plotting/_projection.py` & `apsg-1.2.0/src/apsg/plotting/_projection.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/plotting/_roseplot.py` & `apsg-1.2.0/src/apsg/plotting/_roseplot.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/plotting/_stereogrid.py` & `apsg-1.2.0/src/apsg/plotting/_stereogrid.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg/plotting/_stereonet.py` & `apsg-1.2.0/src/apsg/plotting/_stereonet.py`

 * *Files 0% similar despite different names*

```diff
@@ -936,56 +936,56 @@
             ``FoliationSet``, ``LineationSet``, ``PairSet`` or ``FaultSet``.
 
     Keyword Args:
         savefig (bool): True to save figure. Default `False`
         filename (str): filename for figure. Default `stereonet.png`
         savefig_kwargs (dict): dict passed to ``plt.savefig``
         fol_as_pole (bool): True to plot planar features as poles,
-            False for plotting as great circle. Default `True`
+            False for plotting as great circle. Default `False`
 
     Example:
         >>> l = linset.random_fisher(position=lin(120, 50))
         >>> f = folset.random_fisher(position=lin(300, 40))
-        >>> quicknet(f, l, fol_as_pole=False)
+        >>> quicknet(f, l)
     """
     savefig = kwargs.get("savefig", False)
     filename = kwargs.get("filename", "stereonet.png")
     savefig_kwargs = kwargs.get("savefig_kwargs", {})
-    fol_as_pole = kwargs.get("fol_as_pole", True)
+    fol_as_pole = kwargs.get("fol_as_pole", False)
     s = StereoNet(**kwargs)
     for arg in args:
         if isinstance(arg, Vector3):
             if isinstance(arg, Foliation):
                 if fol_as_pole:
                     s.pole(arg)
                 else:
                     s.great_circle(arg)
             elif isinstance(arg, Lineation):
                 s.line(arg)
             else:
                 s.vector(arg)
-        elif isinstance(arg, Pair):
-            s.pair(arg)
         elif isinstance(arg, Fault):
             s.fault(arg)
+        elif isinstance(arg, Pair):
+            s.pair(arg)
         elif isinstance(arg, Cone):
             s.cone(arg)
         elif isinstance(arg, Vector3Set):
             if isinstance(arg, FoliationSet):
                 if fol_as_pole:
                     s.pole(arg)
                 else:
                     s.great_circle(arg)
             elif isinstance(arg, LineationSet):
                 s.line(arg)
             else:
                 s.vector(arg)
-        elif isinstance(arg, PairSet):
-            s.pair(arg)
         elif isinstance(arg, FaultSet):
             s.fault(arg)
+        elif isinstance(arg, PairSet):
+            s.pair(arg)
         else:
             print(f"{type(arg)} not supported.")
     if savefig:
         s.savefig(filename, **savefig_kwargs)
     else:
         s.show()
```

### Comparing `apsg-1.1.5/src/apsg/shell.py` & `apsg-1.2.0/src/apsg/shell.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/src/apsg.egg-info/PKG-INFO` & `apsg-1.2.0/src/apsg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apsg
-Version: 1.1.5
+Version: 1.2.0
 Summary: APSG - The package for structural geologists
 Home-page: https://github.com/ondrolexa/apsg
 Author: Ondrej Lexa
 Author-email: lexa.ondrej@gmail.com
 License: MIT
 Project-URL: Documentation, https://apsg.readthedocs.io/
 Project-URL: Source Code, https://github.com/ondrolexa/apsg/
@@ -19,24 +19,25 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
+Requires-Dist: sqlalchemy
+Requires-Dist: pandas
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: ipykernel; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: black; extra == "test"
 Provides-Extra: extra
 Requires-Dist: jupyterlab; extra == "extra"
-Requires-Dist: pandas; extra == "extra"
 
 <img src="https://ondrolexa.github.io/apsg/apsg_banner.svg" alt="APSG logo" width="300px"/>
 
 [![PyPI - Version](https://img.shields.io/pypi/v/apsg)](https://pypi.org/project/apsg)
 [![Conda](https://img.shields.io/conda/v/conda-forge/apsg)](https://anaconda.org/conda-forge/apsg)
 [![Documentation Status](https://readthedocs.org/projects/apsg/badge/?version=stable)](https://apsg.readthedocs.io/en/stable/?badge=stable)
 [![DOI](https://zenodo.org/badge/24879346.svg)](https://zenodo.org/badge/latestdoi/24879346)
@@ -135,14 +136,18 @@
 ## License
 
 APSG is free software: you can redistribute it and/or modify it under the terms of the MIT License. A copy of this license is provided in ``LICENSE`` file.
 
 
 # Changes
 
+### 1.2.0 (master)
+ * sqlalchemy and pandas added to requirements
+ * quicknet fault bug fixed
+
 ### 1.1.5 (May 15 2024)
  * paleomag Core .dd bug fixed
  * fix round-off domain math error for acosd and asind
 
 ### 1.1.4 (Dec 13 2023)
  * Ellipsoid repr bugfix
```

### Comparing `apsg-1.1.5/src/apsg.egg-info/SOURCES.txt` & `apsg-1.2.0/src/apsg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/tests/conftest.py` & `apsg-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/tests/test_apsg.py` & `apsg-1.2.0/tests/test_apsg.py`

 * *Files identical despite different names*

### Comparing `apsg-1.1.5/tests/test_tensors.py` & `apsg-1.2.0/tests/test_tensors.py`

 * *Files identical despite different names*

