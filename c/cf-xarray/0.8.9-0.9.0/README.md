# Comparing `tmp/cf_xarray-0.8.9.tar.gz` & `tmp/cf_xarray-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_xarray-0.8.9.tar", last modified: Wed Feb  7 01:04:58 2024, max compression
+gzip compressed data, was "cf_xarray-0.9.0.tar", last modified: Mon Feb 19 21:31:04 2024, max compression
```

## Comparing `cf_xarray-0.8.9.tar` & `cf_xarray-0.9.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.672607 cf_xarray-0.8.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.656607 cf_xarray-0.8.9/.binder/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.656607 cf_xarray-0.8.9/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.656607 cf_xarray-0.8.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.github/workflows/parse_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.github/workflows/testpypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/.tributors
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16508 2024-02-07 01:04:58.672607 cf_xarray-0.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.660607 cf_xarray-0.8.9/cf_xarray/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-07 01:04:58.000000 cf_xarray-0.8.9/cf_xarray/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)   103497 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)    24176 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21630 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/options.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.660607 cf_xarray-0.8.9/cf_xarray/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/scripts/make_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/scripts/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/sgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.664607 cf_xarray-0.8.9/cf_xarray/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66302 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/tests/test_accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/tests/test_coding.py
--rw-r--r--   0 runner    (1001) docker     (127)    17209 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/cf_xarray/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.668607 cf_xarray-0.8.9/cf_xarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16508 2024-02-07 01:04:58.000000 cf_xarray-0.8.9/cf_xarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-07 01:04:58.000000 cf_xarray-0.8.9/cf_xarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 01:04:58.000000 cf_xarray-0.8.9/cf_xarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-07 01:04:58.000000 cf_xarray-0.8.9/cf_xarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-07 01:04:58.000000 cf_xarray-0.8.9/cf_xarray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.664607 cf_xarray-0.8.9/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/ci/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/ci/environment-no-optional-deps.yml
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/ci/upstream-dev-env.yml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.668607 cf_xarray-0.8.9/doc/
--rw-r--r--   0 runner    (1001) docker     (127)    46836 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/2D_bounds_averaged.png
--rw-r--r--   0 runner    (1001) docker     (127)    62190 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/2D_bounds_error.png
--rw-r--r--   0 runner    (1001) docker     (127)    53236 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/2D_bounds_nonunique.png
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.668607 cf_xarray-0.8.9/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/_static/dataset-diagram-logo.tex
--rw-r--r--   0 runner    (1001) docker     (127)    48563 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/_static/full-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    33479 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    71840 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   130855 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/_static/rich-repr-example.png
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/bounds.md
--rw-r--r--   0 runner    (1001) docker     (127)    33785 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/cartopy_rotated_pole.png
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/coding.md
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/coord_axes.md
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/custom-criteria.md
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/dsg.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 01:04:58.668607 cf_xarray-0.8.9/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    23326 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/examples/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/flags.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/geometry.md
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/grid_mappings.md
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/howtouse.md
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/parametricz.md
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/plotting.md
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/provenance.md
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/selecting.md
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/sgrid_ugrid.md
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/units.md
--rw-r--r--   0 runner    (1001) docker     (127)    12727 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/doc/whats-new.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-02-07 01:04:30.000000 cf_xarray-0.8.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 01:04:58.672607 cf_xarray-0.8.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.406505 cf_xarray-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.390505 cf_xarray-0.9.0/.binder/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.390505 cf_xarray-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.394505 cf_xarray-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.github/workflows/parse_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.github/workflows/testpypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/.tributors
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16508 2024-02-19 21:31:04.406505 cf_xarray-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.394505 cf_xarray-0.9.0/cf_xarray/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-19 21:31:04.000000 cf_xarray-0.9.0/cf_xarray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103497 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24176 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21630 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.398505 cf_xarray-0.9.0/cf_xarray/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/scripts/make_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/scripts/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/sgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.398505 cf_xarray-0.9.0/cf_xarray/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66302 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/tests/test_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/tests/test_coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17209 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/cf_xarray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.406505 cf_xarray-0.9.0/cf_xarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16508 2024-02-19 21:31:04.000000 cf_xarray-0.9.0/cf_xarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-19 21:31:04.000000 cf_xarray-0.9.0/cf_xarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 21:31:04.000000 cf_xarray-0.9.0/cf_xarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-19 21:31:04.000000 cf_xarray-0.9.0/cf_xarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-19 21:31:04.000000 cf_xarray-0.9.0/cf_xarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.398505 cf_xarray-0.9.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/ci/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/ci/environment-no-optional-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/ci/upstream-dev-env.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.402505 cf_xarray-0.9.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)    46836 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/2D_bounds_averaged.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62190 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/2D_bounds_error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53236 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/2D_bounds_nonunique.png
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.406505 cf_xarray-0.9.0/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/_static/dataset-diagram-logo.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    48563 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/_static/full-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33479 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    71840 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   130855 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/_static/rich-repr-example.png
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/bounds.md
+-rw-r--r--   0 runner    (1001) docker     (127)    33785 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/cartopy_rotated_pole.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/coding.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/coord_axes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/custom-criteria.md
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/dsg.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 21:31:04.406505 cf_xarray-0.9.0/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    23326 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/flags.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/geometry.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/grid_mappings.md
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/howtouse.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/parametricz.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/provenance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/selecting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/sgrid_ugrid.md
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/units.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/doc/whats-new.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-02-19 21:30:40.000000 cf_xarray-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 21:31:04.406505 cf_xarray-0.9.0/setup.cfg
```

### Comparing `cf_xarray-0.8.9/.github/workflows/ci.yaml` & `cf_xarray-0.9.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/.github/workflows/parse_logs.py` & `cf_xarray-0.9.0/.github/workflows/parse_logs.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/.github/workflows/pypi.yaml` & `cf_xarray-0.9.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/.github/workflows/testpypi-release.yaml` & `cf_xarray-0.9.0/.github/workflows/testpypi-release.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/.github/workflows/upstream-dev-ci.yaml` & `cf_xarray-0.9.0/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/.gitignore` & `cf_xarray-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/.pre-commit-config.yaml` & `cf_xarray-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/.tributors` & `cf_xarray-0.9.0/.tributors`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/CITATION.cff` & `cf_xarray-0.9.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/LICENSE` & `cf_xarray-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/PKG-INFO` & `cf_xarray-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf_xarray
-Version: 0.8.9
+Version: 0.9.0
 Summary: A convenience wrapper for using CF attributes on xarray objects
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cf_xarray-0.8.9/README.rst` & `cf_xarray-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/accessor.py` & `cf_xarray-0.9.0/cf_xarray/accessor.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/coding.py` & `cf_xarray-0.9.0/cf_xarray/coding.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/criteria.py` & `cf_xarray-0.9.0/cf_xarray/criteria.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/datasets.py` & `cf_xarray-0.9.0/cf_xarray/datasets.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/formatting.py` & `cf_xarray-0.9.0/cf_xarray/formatting.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/geometry.py` & `cf_xarray-0.9.0/cf_xarray/geometry.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/helpers.py` & `cf_xarray-0.9.0/cf_xarray/helpers.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/options.py` & `cf_xarray-0.9.0/cf_xarray/options.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/scripts/make_doc.py` & `cf_xarray-0.9.0/cf_xarray/scripts/make_doc.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/sgrid.py` & `cf_xarray-0.9.0/cf_xarray/sgrid.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/tests/__init__.py` & `cf_xarray-0.9.0/cf_xarray/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/tests/test_accessor.py` & `cf_xarray-0.9.0/cf_xarray/tests/test_accessor.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/tests/test_coding.py` & `cf_xarray-0.9.0/cf_xarray/tests/test_coding.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/tests/test_geometry.py` & `cf_xarray-0.9.0/cf_xarray/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/tests/test_helpers.py` & `cf_xarray-0.9.0/cf_xarray/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/tests/test_scripts.py` & `cf_xarray-0.9.0/cf_xarray/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/tests/test_units.py` & `cf_xarray-0.9.0/cf_xarray/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/units.py` & `cf_xarray-0.9.0/cf_xarray/units.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/cf_xarray/utils.py` & `cf_xarray-0.9.0/cf_xarray/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,25 +11,43 @@
 
 try:
     import cftime
 except ImportError:
     cftime = None
 
 
+def _is_duck_dask_array(x):
+    """Return True if the input is a dask array."""
+    # Code copied and simplified from xarray < 2024.02 (xr.core.pycompat.is_duck_dask_array)
+    try:
+        from dask.base import is_dask_collection
+    except ImportError:
+        return False
+
+    return (
+        is_dask_collection(x)
+        and hasattr(x, "ndim")
+        and hasattr(x, "shape")
+        and hasattr(x, "dtype")
+        and (
+            (hasattr(x, "__array_function__") and hasattr(x, "__array_ufunc__"))
+            or hasattr(x, "__array_namespace__")
+        )
+    )
+
+
 def _contains_cftime_datetimes(array) -> bool:
     """Check if an array contains cftime.datetime objects"""
     # Copied / adapted from xarray.core.common
-    from xarray.core.pycompat import is_duck_dask_array
-
     if cftime is None:
         return False
     else:
         if array.dtype == np.dtype("O") and array.size > 0:
             sample = array.ravel()[0]
-            if is_duck_dask_array(sample):
+            if _is_duck_dask_array(sample):
                 sample = sample.compute()
                 if isinstance(sample, np.ndarray):
                     sample = sample.item()
             return isinstance(sample, cftime.datetime)
         else:
             return False
```

### Comparing `cf_xarray-0.8.9/cf_xarray.egg-info/PKG-INFO` & `cf_xarray-0.9.0/cf_xarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf_xarray
-Version: 0.8.9
+Version: 0.9.0
 Summary: A convenience wrapper for using CF attributes on xarray objects
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cf_xarray-0.8.9/cf_xarray.egg-info/SOURCES.txt` & `cf_xarray-0.9.0/cf_xarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/2D_bounds_averaged.png` & `cf_xarray-0.9.0/doc/2D_bounds_averaged.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/2D_bounds_error.png` & `cf_xarray-0.9.0/doc/2D_bounds_error.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/2D_bounds_nonunique.png` & `cf_xarray-0.9.0/doc/2D_bounds_nonunique.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/Makefile` & `cf_xarray-0.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/_static/dataset-diagram-logo.tex` & `cf_xarray-0.9.0/doc/_static/dataset-diagram-logo.tex`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/_static/full-logo.png` & `cf_xarray-0.9.0/doc/_static/full-logo.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/_static/logo.png` & `cf_xarray-0.9.0/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/_static/logo.svg` & `cf_xarray-0.9.0/doc/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/_static/rich-repr-example.png` & `cf_xarray-0.9.0/doc/_static/rich-repr-example.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/api.rst` & `cf_xarray-0.9.0/doc/api.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/bounds.md` & `cf_xarray-0.9.0/doc/bounds.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/cartopy_rotated_pole.png` & `cf_xarray-0.9.0/doc/cartopy_rotated_pole.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/coding.md` & `cf_xarray-0.9.0/doc/coding.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/conf.py` & `cf_xarray-0.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/contributing.rst` & `cf_xarray-0.9.0/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/coord_axes.md` & `cf_xarray-0.9.0/doc/coord_axes.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/custom-criteria.md` & `cf_xarray-0.9.0/doc/custom-criteria.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/dsg.md` & `cf_xarray-0.9.0/doc/dsg.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/examples/introduction.ipynb` & `cf_xarray-0.9.0/doc/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/flags.md` & `cf_xarray-0.9.0/doc/flags.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/grid_mappings.md` & `cf_xarray-0.9.0/doc/grid_mappings.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/howtouse.md` & `cf_xarray-0.9.0/doc/howtouse.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/index.rst` & `cf_xarray-0.9.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/make.bat` & `cf_xarray-0.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/parametricz.md` & `cf_xarray-0.9.0/doc/parametricz.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/plotting.md` & `cf_xarray-0.9.0/doc/plotting.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/provenance.md` & `cf_xarray-0.9.0/doc/provenance.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/quickstart.md` & `cf_xarray-0.9.0/doc/quickstart.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/roadmap.rst` & `cf_xarray-0.9.0/doc/roadmap.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/selecting.md` & `cf_xarray-0.9.0/doc/selecting.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/sgrid_ugrid.md` & `cf_xarray-0.9.0/doc/sgrid_ugrid.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/units.md` & `cf_xarray-0.9.0/doc/units.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.9/doc/whats-new.rst` & `cf_xarray-0.9.0/doc/whats-new.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. currentmodule:: xarray
 
 What's New
 ----------
 
+v0.8.10 (unreleased)
+====================
+- Fix methods in ``utils`` to work with xarray >= 2024.02.0. By `Pascal Bourgault`_.
+
 v0.8.9 (Feb 06, 2023)
 =====================
 - Convert integer (e.g. ``1``) units to string (e.g. ``"1"``) for pint. By `Justus Magin`_.
 
 v0.8.8 (Jan 19, 2023)
 =====================
 - Add conversion between CF geometries and Shapely objects for polygons. By `Julia Signell`_.
```

### Comparing `cf_xarray-0.8.9/pyproject.toml` & `cf_xarray-0.9.0/pyproject.toml`

 * *Files identical despite different names*

