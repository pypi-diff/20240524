# Comparing `tmp/DelayedArray-0.5.0.tar.gz` & `tmp/delayedarray-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DelayedArray-0.5.0.tar", last modified: Thu Feb  1 16:37:01 2024, max compression
+gzip compressed data, was "delayedarray-0.5.1.tar", last modified: Fri May 24 21:31:08 2024, max compression
```

## Comparing `DelayedArray-0.5.0.tar` & `delayedarray-0.5.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 16:37:01.514100 DelayedArray-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 16:37:01.494099 DelayedArray-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 16:37:01.498100 DelayedArray-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-02-01 16:37:01.514100 DelayedArray-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 16:37:01.498100 DelayedArray-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 16:37:01.502100 DelayedArray-0.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/docs/developers.md
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-01 16:37:01.514100 DelayedArray-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 16:37:01.494099 DelayedArray-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 16:37:01.510100 DelayedArray-0.5.0/src/DelayedArray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-02-01 16:37:01.000000 DelayedArray-0.5.0/src/DelayedArray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-02-01 16:37:01.000000 DelayedArray-0.5.0/src/DelayedArray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 16:37:01.000000 DelayedArray-0.5.0/src/DelayedArray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 16:37:01.000000 DelayedArray-0.5.0/src/DelayedArray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-01 16:37:01.000000 DelayedArray-0.5.0/src/DelayedArray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-01 16:37:01.000000 DelayedArray-0.5.0/src/DelayedArray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 16:37:01.506100 DelayedArray-0.5.0/src/delayedarray/
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/BinaryIsometricOp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/Cast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/Combine.py
--rw-r--r--   0 runner    (1001) docker     (127)    37295 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/DelayedArray.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/DelayedOp.py
--rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/Grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/RegularTicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/Round.py
--rw-r--r--   0 runner    (1001) docker     (127)    67456 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/SparseNdarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/Subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/Transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/UnaryIsometricOpSimple.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/UnaryIsometricOpWithArgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/_isometric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/apply_over_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/apply_over_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/chunk_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/create_dask_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/extract_dense_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/extract_sparse_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/is_masked.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/is_pristine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/is_sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/to_dense_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/to_scipy_sparse_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/to_sparse_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/src/delayedarray/wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 16:37:01.510100 DelayedArray-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_BinaryIsometricOp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_Cast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_Combine.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_DelayedArray.py
--rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_Grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_RegularTicks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_Round.py
--rw-r--r--   0 runner    (1001) docker     (127)    47490 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_SparseNdarray.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_Subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_Transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_UnaryIsometricOpSimple.py
--rw-r--r--   0 runner    (1001) docker     (127)    24508 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_UnaryIsometricOpWithArgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_apply_over_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_apply_over_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_extract_sparse_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_is_pristine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/test_to_scipy_sparse_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-02-01 16:35:31.000000 DelayedArray-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:31:08.825314 delayedarray-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-24 21:29:35.000000 delayedarray-0.5.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:31:08.805314 delayedarray-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:31:08.809314 delayedarray-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-24 21:29:35.000000 delayedarray-0.5.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-24 21:29:35.000000 delayedarray-0.5.1/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-24 21:29:35.000000 delayedarray-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-24 21:29:35.000000 delayedarray-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-24 21:29:35.000000 delayedarray-0.5.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-24 21:29:35.000000 delayedarray-0.5.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-24 21:29:35.000000 delayedarray-0.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-24 21:29:35.000000 delayedarray-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-24 21:29:35.000000 delayedarray-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-05-24 21:31:08.825314 delayedarray-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-05-24 21:29:35.000000 delayedarray-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:31:08.809314 delayedarray-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-24 21:29:35.000000 delayedarray-0.5.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:31:08.809314 delayedarray-0.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 21:29:35.000000 delayedarray-0.5.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-24 21:29:35.000000 delayedarray-0.5.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-24 21:29:35.000000 delayedarray-0.5.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-24 21:29:35.000000 delayedarray-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 21:29:35.000000 delayedarray-0.5.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-24 21:29:35.000000 delayedarray-0.5.1/docs/developers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-24 21:29:35.000000 delayedarray-0.5.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 21:29:35.000000 delayedarray-0.5.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-24 21:29:35.000000 delayedarray-0.5.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-24 21:29:35.000000 delayedarray-0.5.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-24 21:29:35.000000 delayedarray-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-24 21:31:08.825314 delayedarray-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-24 21:29:35.000000 delayedarray-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:31:08.805314 delayedarray-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:31:08.821314 delayedarray-0.5.1/src/DelayedArray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-05-24 21:31:08.000000 delayedarray-0.5.1/src/DelayedArray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-24 21:31:08.000000 delayedarray-0.5.1/src/DelayedArray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:31:08.000000 delayedarray-0.5.1/src/DelayedArray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:31:08.000000 delayedarray-0.5.1/src/DelayedArray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-24 21:31:08.000000 delayedarray-0.5.1/src/DelayedArray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 21:31:08.000000 delayedarray-0.5.1/src/DelayedArray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:31:08.817314 delayedarray-0.5.1/src/delayedarray/
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/BinaryIsometricOp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/Cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/Combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43246 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/DelayedArray.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/DelayedOp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22619 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/Grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/RegularTicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/Round.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73044 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/SparseNdarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/Subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/Transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/UnaryIsometricOpSimple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/UnaryIsometricOpWithArgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/_isometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/apply_over_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/apply_over_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/chunk_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/create_dask_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/extract_dense_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/extract_sparse_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/is_masked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/is_pristine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/is_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/to_dense_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/to_scipy_sparse_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/to_sparse_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-24 21:29:35.000000 delayedarray-0.5.1/src/delayedarray/wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:31:08.821314 delayedarray-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_BinaryIsometricOp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_Cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_Combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14536 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_DelayedArray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_Grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_RegularTicks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_Round.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47490 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_SparseNdarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_Subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_Transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_UnaryIsometricOpSimple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24508 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_UnaryIsometricOpWithArgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_apply_over_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_apply_over_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_extract_sparse_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_is_pristine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/test_to_scipy_sparse_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-24 21:29:35.000000 delayedarray-0.5.1/tox.ini
```

### Comparing `DelayedArray-0.5.0/.coveragerc` & `delayedarray-0.5.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/.github/workflows/pypi-publish.yml` & `delayedarray-0.5.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/.github/workflows/pypi-test.yml` & `delayedarray-0.5.1/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/.gitignore` & `delayedarray-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/.pre-commit-config.yaml` & `delayedarray-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/.readthedocs.yml` & `delayedarray-0.5.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/CHANGELOG.md` & `delayedarray-0.5.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/CONTRIBUTING.md` & `delayedarray-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/LICENSE.txt` & `delayedarray-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/PKG-INFO` & `delayedarray-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DelayedArray
-Version: 0.5.0
+Version: 0.5.1
 Summary: Delayed array operations from Bioconductor
 Home-page: https://github.com/biocpy/DelayedArray
 Author: Aaron Lun
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://biocpy.github.io/DelayedArray/
 Platform: any
```

### Comparing `DelayedArray-0.5.0/README.md` & `delayedarray-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/docs/Makefile` & `delayedarray-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/docs/conf.py` & `delayedarray-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/docs/developers.md` & `delayedarray-0.5.1/docs/developers.md`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/docs/index.md` & `delayedarray-0.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/pyproject.toml` & `delayedarray-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/setup.cfg` & `delayedarray-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/setup.py` & `delayedarray-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/DelayedArray.egg-info/PKG-INFO` & `delayedarray-0.5.1/src/DelayedArray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DelayedArray
-Version: 0.5.0
+Version: 0.5.1
 Summary: Delayed array operations from Bioconductor
 Home-page: https://github.com/biocpy/DelayedArray
 Author: Aaron Lun
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://biocpy.github.io/DelayedArray/
 Platform: any
```

### Comparing `DelayedArray-0.5.0/src/DelayedArray.egg-info/SOURCES.txt` & `delayedarray-0.5.1/src/DelayedArray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/BinaryIsometricOp.py` & `delayedarray-0.5.1/src/delayedarray/BinaryIsometricOp.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/Cast.py` & `delayedarray-0.5.1/src/delayedarray/Cast.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/Combine.py` & `delayedarray-0.5.1/src/delayedarray/Combine.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/DelayedArray.py` & `delayedarray-0.5.1/src/delayedarray/DelayedArray.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Sequence, Tuple, Union, Optional, List, Callable
 import numpy
-from numpy import array, dtype, integer, issubdtype, ndarray, prod, array2string
+from numpy import dtype, ndarray, array2string
 from collections import namedtuple
 
 from .SparseNdarray import SparseNdarray
 from .BinaryIsometricOp import BinaryIsometricOp
 from .Cast import Cast
 from .Combine import Combine
 from .Round import Round
@@ -20,15 +20,15 @@
 from .create_dask_array import create_dask_array
 from .chunk_grid import chunk_grid
 from .is_sparse import is_sparse
 from .is_masked import is_masked
 
 from ._subset import _getitem_subset_preserves_dimensions, _getitem_subset_discards_dimensions, _repr_subset
 from ._isometric import translate_ufunc_to_op_simple, translate_ufunc_to_op_with_args
-from ._statistics import array_mean, array_var, array_sum, _create_offset_multipliers
+from ._statistics import array_mean, array_var, array_sum, _create_offset_multipliers, array_any, array_all
 
 __author__ = "ltla"
 __copyright__ = "ltla"
 __license__ = "MIT"
 
 
 def _wrap_isometric_with_args(x, other, operation, right):
@@ -251,14 +251,29 @@
             seed = _extract_seed(args[0])
             if "decimals" in kwargs:
                 decimals = kwargs["decimals"]
             else:
                 decimals = 0
             return DelayedArray(Round(seed, decimals=decimals))
 
+        if func == numpy.mean:
+            return self.mean(**kwargs)
+
+        if func == numpy.sum:
+            return self.sum(**kwargs)
+
+        if func == numpy.var:
+            return self.var(**kwargs)
+
+        if func == numpy.any:
+            return self.any(**kwargs)
+
+        if func == numpy.all:
+            return self.all(**kwargs)
+
         if func == numpy.shape:
             return self.shape 
 
         raise NotImplementedError(f"'{func.__name__}' is not implemented!")
 
     def astype(self, dtype, **kwargs):
         """See :py:meth:`~numpy.ndarray.astype` for details.
@@ -687,14 +702,74 @@
         """Take the absolute value of the contents of a ``DelayedArray``.
 
         Returns:
             A ``DelayedArray`` containing the delayed absolute value operation.
         """
         return DelayedArray(UnaryIsometricOpSimple(self._seed, operation="abs"))
 
+    def __or__(self, other) -> "DelayedArray":
+        """Element-wise OR with something.
+
+        Args:
+            other:
+                A numeric scalar;
+                or a NumPy array with dimensions as described in
+                :py:class:`~delayedarray.UnaryIsometricOpWithArgs.UnaryIsometricOpWithArgs`;
+                or a ``DelayedArray`` of the same dimensions as :py:attr:`~shape`.
+
+        Returns:
+            A ``DelayedArray`` containing the delayed OR operation.
+        """
+        return _wrap_isometric_with_args(self, other, operation="logical_or", right=True)
+
+    def __ror__(self, other) -> "DelayedArray":
+        """Element-wise OR with the right-hand-side of a ``DelayedArray``.
+
+        Args:
+            other:
+                A numeric scalar;
+                or a NumPy array with dimensions as described in
+                :py:class:`~delayedarray.UnaryIsometricOpWithArgs.UnaryIsometricOpWithArgs`;
+                or a ``DelayedArray`` of the same dimensions as :py:attr:`~shape`.
+
+        Returns:
+            A ``DelayedArray`` containing the delayed OR operation.
+        """
+        return _wrap_isometric_with_args(self, other, operation="logical_or", right=False)
+
+    def __and__(self, other) -> "DelayedArray":
+        """Element-wise AND with something.
+
+        Args:
+            other:
+                A numeric scalar;
+                or a NumPy array with dimensions as described in
+                :py:class:`~delayedarray.UnaryIsometricOpWithArgs.UnaryIsometricOpWithArgs`;
+                or a ``DelayedArray`` of the same dimensions as :py:attr:`~shape`.
+
+        Returns:
+            A ``DelayedArray`` containing the delayed AND operation.
+        """
+        return _wrap_isometric_with_args(self, other, operation="logical_and", right=True)
+
+    def __rand__(self, other) -> "DelayedArray":
+        """Element-wise AND with the right-hand-side of a ``DelayedArray``.
+
+        Args:
+            other:
+                A numeric scalar;
+                or a NumPy array with dimensions as described in
+                :py:class:`~delayedarray.UnaryIsometricOpWithArgs.UnaryIsometricOpWithArgs`;
+                or a ``DelayedArray`` of the same dimensions as :py:attr:`~shape`.
+
+        Returns:
+            A ``DelayedArray`` containing the delayed AND operation.
+        """
+        return _wrap_isometric_with_args(self, other, operation="logical_and", right=False)
+
     # Subsetting.
     def __getitem__(self, subset: Tuple[Union[slice, Sequence], ...]) -> Union["DelayedArray", ndarray]:
         """Take a subset of this ``DelayedArray``. This follows the same logic as NumPy slicing and will generate a
         :py:class:`~delayedarray.Subset.Subset` object when the subset operation preserves the dimensionality of the
         seed, i.e., ``args`` is defined using the :py:meth:`~numpy.ix_` function.
 
         Args:
@@ -828,14 +903,87 @@
                 axis=axis, 
                 dtype=dtype, 
                 ddof=ddof,
                 reduce_over_x=lambda x, axes, op : _reduce(x, axes, op, buffer_size),
                 masked=is_masked(self),
             )
 
+    def any(self, axis: Optional[Union[int, Tuple[int, ...]]] = None, dtype: Optional[numpy.dtype] = None, buffer_size: int = 1e8) -> numpy.ndarray:
+        """Test whether any array element along a given axis evaluates to True.
+
+        Compute this test across the ``DelayedArray``, possibly over a
+        given axis or set of axes. If the seed has a ``any()`` method, that
+        method is called directly with the supplied arguments.
+
+        Args:
+            axis: 
+                A single integer specifying the axis over which to test
+                for any. Alternatively, a tuple (multiple axes) or None (no
+                axes), see :py:func:`~numpy.any` for details.
+
+            dtype:
+                NumPy type for the output array. If None, this is automatically
+                chosen based on the type of the ``DelayedArray``, see
+                :py:func:`~numpy.any` for details.
+
+            buffer_size:
+                Buffer size in bytes to use for block processing. Larger values
+                generally improve speed at the cost of memory.
+
+        Returns:
+            A NumPy array containing the boolean values. If ``axis = None``, this will
+            be a NumPy scalar instead.
+        """
+        if hasattr(self._seed, "any"):
+            return self._seed.any(axis=axis).astype(dtype)
+        else:
+            return array_any(
+                self, 
+                axis=axis, 
+                dtype=dtype, 
+                reduce_over_x=lambda x, axes, op : _reduce(x, axes, op, buffer_size),
+                masked=is_masked(self),
+            )
+
+    def all(self, axis: Optional[Union[int, Tuple[int, ...]]] = None, dtype: Optional[numpy.dtype] = None, buffer_size: int = 1e8) -> numpy.ndarray:
+        """Test whether all array elements along a given axis evaluate to True.
+
+        Compute this test across the ``DelayedArray``, possibly over a
+        given axis or set of axes. If the seed has a ``all()`` method, that
+        method is called directly with the supplied arguments.
+
+        Args:
+            axis: 
+                A single integer specifying the axis over which to test 
+                for all. Alternatively, a tuple (multiple axes) or None (no
+                axes), see :py:func:`~numpy.all` for details.
+
+            dtype:
+                NumPy type for the output array. If None, this is automatically
+                chosen based on the type of the ``DelayedArray``, see
+                :py:func:`~numpy.all` for details.
+
+            buffer_size:
+                Buffer size in bytes to use for block processing. Larger values
+                generally improve speed at the cost of memory.
+
+        Returns:
+            A NumPy array containing the boolean values. If ``axis = None``, this will
+            be a NumPy scalar instead.
+        """
+        if hasattr(self._seed, "all"):
+            return self._seed.all(axis=axis).astype(dtype)
+        else:
+            return array_all(
+                self, 
+                axis=axis, 
+                dtype=dtype, 
+                reduce_over_x=lambda x, axes, op : _reduce(x, axes, op, buffer_size),
+                masked=is_masked(self),
+            )
 
 @extract_dense_array.register
 def extract_dense_array_DelayedArray(x: DelayedArray, subset: Tuple[Sequence[int], ...]) -> numpy.ndarray:
     """See :py:meth:`~delayedarray.extract_dense_array.extract_dense_array`."""
     return extract_dense_array(x._seed, subset)
```

### Comparing `DelayedArray-0.5.0/src/delayedarray/Grid.py` & `delayedarray-0.5.1/src/delayedarray/Grid.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/RegularTicks.py` & `delayedarray-0.5.1/src/delayedarray/RegularTicks.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/Round.py` & `delayedarray-0.5.1/src/delayedarray/Round.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/SparseNdarray.py` & `delayedarray-0.5.1/src/delayedarray/SparseNdarray.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     _allocate_unmasked_ndarray, 
     _allocate_maybe_masked_ndarray, 
     _convert_to_unmasked_1darray, 
     _convert_to_maybe_masked_1darray,
     _concatenate_unmasked_ndarrays,
     _concatenate_maybe_masked_ndarrays
 )
-from ._statistics import array_mean, array_var, array_sum, _create_offset_multipliers
+from ._statistics import array_mean, array_var, array_sum, _create_offset_multipliers, array_all, array_any
 
 __author__ = "ltla"
 __copyright__ = "ltla"
 __license__ = "MIT"
 
 
 class SparseNdarray:
@@ -661,14 +661,79 @@
     def __abs__(self):
         """Take the absolute value of the contents of a ``SparseNdarray``.
 
         Returns:
             A ``SparseNdarray`` containing the delayed absolute value operation.
         """
         return _transform_sparse_array_from_SparseNdarray(self, lambda l, i, v : (i, abs(v)), self._dtype)
+    
+    def __or__(self, other) -> Union["SparseNdarray", numpy.ndarray]:
+        """Element-wise OR with something.
+
+        Args:
+            other:
+                A numeric scalar;
+                or a NumPy array with dimensions as described in
+                :py:class:`~delayedarray.UnaryIsometricOpWithArgs.UnaryIsometricOpWithArgs`;
+                or a ``DelayedArray`` of the same dimensions as :py:attr:`~shape`.
+
+        Returns:
+            Array containing the result of the check.
+            This may or may not be sparse depending on ``other``.
+        """
+        return _operate_with_args_on_SparseNdarray(self, other, operation="logical_or", right=True)
+
+    def __ror__(self, other) -> Union["SparseNdarray", numpy.ndarray]:
+        """Element-wise OR with the right-hand-side of a ``DelayedArray``.
+
+        Args:
+            other:
+                A numeric scalar;
+                or a NumPy array with dimensions as described in
+                :py:class:`~delayedarray.UnaryIsometricOpWithArgs.UnaryIsometricOpWithArgs`;
+                or a ``DelayedArray`` of the same dimensions as :py:attr:`~shape`.
+
+        Returns:
+            Array containing the result of the check.
+            This may or may not be sparse depending on ``other``.
+        """
+        return _operate_with_args_on_SparseNdarray(self, other, operation="logical_or", right=False)
+
+    def __and__(self, other) -> Union["SparseNdarray", numpy.ndarray]:
+        """Element-wise AND with something.
+
+        Args:
+            other:
+                A numeric scalar;
+                or a NumPy array with dimensions as described in
+                :py:class:`~delayedarray.UnaryIsometricOpWithArgs.UnaryIsometricOpWithArgs`;
+                or a ``DelayedArray`` of the same dimensions as :py:attr:`~shape`.
+
+        Returns:
+            Array containing the result of the check.
+            This may or may not be sparse depending on ``other``.
+        """
+        return _operate_with_args_on_SparseNdarray(self, other, operation="logical_and", right=True)
+
+    def __rand__(self, other) -> Union["SparseNdarray", numpy.ndarray]:
+        """Element-wise AND with the right-hand-side of a ``DelayedArray``.
+
+        Args:
+            other:
+                A numeric scalar;
+                or a NumPy array with dimensions as described in
+                :py:class:`~delayedarray.UnaryIsometricOpWithArgs.UnaryIsometricOpWithArgs`;
+                or a ``DelayedArray`` of the same dimensions as :py:attr:`~shape`.
+
+        Returns:
+            Array containing the result of the check.
+            This may or may not be sparse depending on ``other``.
+        """
+        return _operate_with_args_on_SparseNdarray(self, other, operation="logical_and", right=False)
+
 
     # Subsetting.
     def __getitem__(self, subset: Tuple[Union[slice, Sequence], ...]) -> Union["SparseNdarray", numpy.ndarray]:
         """Take a subset of this ``SparseNdarray``. This follows the same logic as NumPy slicing and will generate a
         :py:class:`~delayedarray.Subset.Subset` object when the subset operation preserves the dimensionality of the
         seed, i.e., ``args`` is defined using the :py:meth:`~numpy.ix_` function.
 
@@ -756,14 +821,29 @@
             else:
                 axes = list(range(len(self._shape) - 1, -1, -1))
             return _transpose_SparseNdarray(self, axes)
 
         if func == numpy.round:
             return _transform_sparse_array_from_SparseNdarray(self, lambda l, i, v : (i, func(v, **kwargs)), self._dtype)
 
+        if func == numpy.mean:
+            return self.mean(**kwargs)
+
+        if func == numpy.sum:
+            return self.sum(**kwargs)
+
+        if func == numpy.var:
+            return self.var(**kwargs)
+
+        if func == numpy.any:
+            return self.any(**kwargs)
+
+        if func == numpy.all:
+            return self.all(**kwargs)
+
         raise NotImplementedError(f"'{func.__name__}' is not implemented!")
 
 
     def astype(self, dtype: numpy.dtype, **kwargs) -> "SparseNdarray":
         """See :py:meth:`~numpy.ndarray.astype` for details.
 
         All keyword arguments are currently ignored.
@@ -868,14 +948,72 @@
             axis=axis, 
             dtype=dtype,
             ddof=ddof,
             reduce_over_x=_reduce_SparseNdarray,
             masked=self._is_masked,
         )
 
+    def any(self, axis: Optional[Union[int, Tuple[int, ...]]] = None, dtype: Optional[numpy.dtype] = None) -> numpy.ndarray:
+        """Test whether any array element along a given axis evaluates to True.
+
+        Compute this test across the ``SparseNdarray``, possibly over a
+        given axis or set of axes. If the seed has a ``any()`` method, that
+        method is called directly with the supplied arguments.
+
+        Args:
+            axis: 
+                A single integer specifying the axis over which to test
+                for any. Alternatively, a tuple (multiple axes) or None
+                (no axes), see :py:func:`~numpy.any` for details.
+
+            dtype:
+                NumPy type for the output array. If None, this is automatically
+                chosen based on the type of the ``SparseNdarray``, see
+                :py:func:`~numpy.any` for details.
+
+        Returns:
+            A NumPy array containing the variances. If ``axis = None``,
+            this will be a NumPy scalar instead.
+        """
+        return array_any(
+            self, 
+            axis=axis, 
+            dtype=dtype, 
+            reduce_over_x=_reduce_SparseNdarray,
+            masked=self._is_masked,
+        )
+
+    def all(self, axis: Optional[Union[int, Tuple[int, ...]]] = None, dtype: Optional[numpy.dtype] = None) -> numpy.ndarray:
+        """Test whether all array elements along a given axis evaluate to True.
+
+        Compute this test across the ``SparseNdarray``, possibly over a
+        given axis or set of axes. If the seed has a ``all()`` method, that
+        method is called directly with the supplied arguments.
+        Args:
+            axis: 
+                A single integer specifying the axis over which to test
+                for any. Alternatively, a tuple (multiple axes) or None
+                (no axes), see :py:func:`~numpy.any` for details.
+
+            dtype:
+                NumPy type for the output array. If None, this is automatically
+                chosen based on the type of the ``SparseNdarray``, see
+                :py:func:`~numpy.any` for details.
+
+        Returns:
+            A NumPy array containing the variances. If ``axis = None``,
+            this will be a NumPy scalar instead.
+        """
+        return array_all(
+            self, 
+            axis=axis, 
+            dtype=dtype, 
+            reduce_over_x=_reduce_SparseNdarray,
+            masked=self._is_masked,
+        )
 
     # Other stuff
     def __copy__(self) -> "SparseNdarray":
         """
         Returns:
             A deep copy of this object.
         """
```

### Comparing `DelayedArray-0.5.0/src/delayedarray/Subset.py` & `delayedarray-0.5.1/src/delayedarray/Subset.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/Transpose.py` & `delayedarray-0.5.1/src/delayedarray/Transpose.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/UnaryIsometricOpSimple.py` & `delayedarray-0.5.1/src/delayedarray/UnaryIsometricOpSimple.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/UnaryIsometricOpWithArgs.py` & `delayedarray-0.5.1/src/delayedarray/UnaryIsometricOpWithArgs.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/__init__.py` & `delayedarray-0.5.1/src/delayedarray/__init__.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/_isometric.py` & `delayedarray-0.5.1/src/delayedarray/_isometric.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         "arcsinh",
         "arccosh",
         "arctanh",
         "ceil",
         "floor",
         "trunc",
         "sign",
+        "isnan"
     ]
 )
 
 
 def _infer_along_with_args(shape: Tuple[int, ...], value):
     along = None
     if not isinstance(value, numpy.ndarray) or len(value.shape) == 0:
```

### Comparing `DelayedArray-0.5.0/src/delayedarray/_mask.py` & `delayedarray-0.5.1/src/delayedarray/_mask.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/_subset.py` & `delayedarray-0.5.1/src/delayedarray/_subset.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/apply_over_blocks.py` & `delayedarray-0.5.1/src/delayedarray/apply_over_blocks.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/apply_over_dimension.py` & `delayedarray-0.5.1/src/delayedarray/apply_over_dimension.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/chunk_grid.py` & `delayedarray-0.5.1/src/delayedarray/chunk_grid.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/create_dask_array.py` & `delayedarray-0.5.1/src/delayedarray/create_dask_array.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/extract_dense_array.py` & `delayedarray-0.5.1/src/delayedarray/extract_dense_array.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/extract_sparse_array.py` & `delayedarray-0.5.1/src/delayedarray/extract_sparse_array.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/is_masked.py` & `delayedarray-0.5.1/src/delayedarray/is_masked.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/is_sparse.py` & `delayedarray-0.5.1/src/delayedarray/is_sparse.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/to_dense_array.py` & `delayedarray-0.5.1/src/delayedarray/to_dense_array.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/to_scipy_sparse_matrix.py` & `delayedarray-0.5.1/src/delayedarray/to_scipy_sparse_matrix.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/to_sparse_array.py` & `delayedarray-0.5.1/src/delayedarray/to_sparse_array.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/src/delayedarray/wrap.py` & `delayedarray-0.5.1/src/delayedarray/wrap.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_BinaryIsometricOp.py` & `delayedarray-0.5.1/tests/test_BinaryIsometricOp.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_Cast.py` & `delayedarray-0.5.1/tests/test_Cast.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_Combine.py` & `delayedarray-0.5.1/tests/test_Combine.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_Grid.py` & `delayedarray-0.5.1/tests/test_Grid.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_RegularTicks.py` & `delayedarray-0.5.1/tests/test_RegularTicks.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_Round.py` & `delayedarray-0.5.1/tests/test_Round.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_SparseNdarray.py` & `delayedarray-0.5.1/tests/test_SparseNdarray.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_Subset.py` & `delayedarray-0.5.1/tests/test_Subset.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_Transpose.py` & `delayedarray-0.5.1/tests/test_Transpose.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_UnaryIsometricOpSimple.py` & `delayedarray-0.5.1/tests/test_UnaryIsometricOpSimple.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_UnaryIsometricOpWithArgs.py` & `delayedarray-0.5.1/tests/test_UnaryIsometricOpWithArgs.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_apply_over_blocks.py` & `delayedarray-0.5.1/tests/test_apply_over_blocks.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_apply_over_dimension.py` & `delayedarray-0.5.1/tests/test_apply_over_dimension.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_extract_sparse_array.py` & `delayedarray-0.5.1/tests/test_extract_sparse_array.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/test_to_scipy_sparse_matrix.py` & `delayedarray-0.5.1/tests/test_to_scipy_sparse_matrix.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tests/utils.py` & `delayedarray-0.5.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `DelayedArray-0.5.0/tox.ini` & `delayedarray-0.5.1/tox.ini`

 * *Files identical despite different names*

