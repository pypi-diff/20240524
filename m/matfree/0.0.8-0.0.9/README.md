# Comparing `tmp/matfree-0.0.8.tar.gz` & `tmp/matfree-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matfree-0.0.8.tar", last modified: Wed Oct 11 07:19:53 2023, max compression
+gzip compressed data, was "matfree-0.0.9.tar", last modified: Thu Nov 23 10:29:57 2023, max compression
```

## Comparing `matfree-0.0.8.tar` & `matfree-0.0.9.tar`

### file list

```diff
@@ -1,97 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.451454 matfree-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.439454 matfree-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.443454 matfree-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-10-11 07:19:39.000000 matfree-0.0.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      910 2023-10-11 07:19:39.000000 matfree-0.0.8/.github/workflows/doc-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-10-11 07:19:39.000000 matfree-0.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-10-11 07:19:39.000000 matfree-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-10-11 07:19:39.000000 matfree-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-10-11 07:19:39.000000 matfree-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      494 2023-10-11 07:19:39.000000 matfree-0.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2023-10-11 07:19:53.451454 matfree-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2023-10-11 07:19:39.000000 matfree-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.443454 matfree-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.443454 matfree-0.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/api/decomp.md
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/api/hutchinson.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/api/lanczos.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/api/montecarlo.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/api/pinv.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/api/slq.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.443454 matfree-0.0.8/docs/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/benchmarks/control_variates.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/benchmarks/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/benchmarks/jacobian_squared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/control_variates.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.443454 matfree-0.0.8/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/dev/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/higher_moments.md
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.443454 matfree-0.0.8/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/log_determinants.md
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/pytree_logdeterminants.md
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2023-10-11 07:19:39.000000 matfree-0.0.8/docs/vector_calculus.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.443454 matfree-0.0.8/matfree/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-11 07:19:53.000000 matfree-0.0.8/matfree/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.447454 matfree-0.0.8/matfree/backend/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/control_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/func.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/np.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/plt.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/prng.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/time.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/backend/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/benchmark_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/decomp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/hutchinson.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/lanczos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/pinv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/slq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-10-11 07:19:39.000000 matfree-0.0.8/matfree/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.447454 matfree-0.0.8/matfree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2023-10-11 07:19:53.000000 matfree-0.0.8/matfree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-10-11 07:19:53.000000 matfree-0.0.8/matfree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 07:19:53.000000 matfree-0.0.8/matfree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-10-11 07:19:53.000000 matfree-0.0.8/matfree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-11 07:19:53.000000 matfree-0.0.8/matfree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2023-10-11 07:19:39.000000 matfree-0.0.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2023-10-11 07:19:39.000000 matfree-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-11 07:19:53.451454 matfree-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.447454 matfree-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.447454 matfree-0.0.8/tests/test_decomp/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_decomp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_decomp/test_svd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.447454 matfree-0.0.8/tests/test_hutchinson/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_hutchinson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_hutchinson/test_diagonal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_hutchinson/test_frobeniusnorm_squared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_hutchinson/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_hutchinson/test_trace_and_diagonal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_hutchinson/test_trace_moments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.447454 matfree-0.0.8/tests/test_lanczos/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_lanczos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_lanczos/test_bidiagonal_full_reortho.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_lanczos/test_tridiagonal_full_reortho.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.451454 matfree-0.0.8/tests/test_montecarlo/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_montecarlo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_montecarlo/test_estimate.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_montecarlo/test_multiestimate.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_montecarlo/test_van_der_corput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.451454 matfree-0.0.8/tests/test_pinv/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_pinv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_pinv/test_pseudo_inverse_correct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 07:19:53.451454 matfree-0.0.8/tests/test_slq/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_slq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_slq/test_logdet_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_slq/test_logdet_spd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_slq/test_logdet_spd_autodiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2023-10-11 07:19:39.000000 matfree-0.0.8/tests/test_slq/test_schatten_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.108858 matfree-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.096858 matfree-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.100858 matfree-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-11-23 10:29:47.000000 matfree-0.0.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2023-11-23 10:29:47.000000 matfree-0.0.9/.github/workflows/doc-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2023-11-23 10:29:47.000000 matfree-0.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-11-23 10:29:47.000000 matfree-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2023-11-23 10:29:47.000000 matfree-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-23 10:29:47.000000 matfree-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2023-11-23 10:29:47.000000 matfree-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2023-11-23 10:29:57.108858 matfree-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2023-11-23 10:29:47.000000 matfree-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.096858 matfree-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.100858 matfree-0.0.9/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2023-11-23 10:29:47.000000 matfree-0.0.9/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.100858 matfree-0.0.9/matfree/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-23 10:29:57.000000 matfree-0.0.9/matfree/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.104858 matfree-0.0.9/matfree/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/control_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/np.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/plt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/prng.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/backend/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/hutchinson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/pinv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/slq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-11-23 10:29:47.000000 matfree-0.0.9/matfree/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.108858 matfree-0.0.9/matfree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2023-11-23 10:29:57.000000 matfree-0.0.9/matfree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-11-23 10:29:57.000000 matfree-0.0.9/matfree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 10:29:57.000000 matfree-0.0.9/matfree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-11-23 10:29:57.000000 matfree-0.0.9/matfree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-23 10:29:57.000000 matfree-0.0.9/matfree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2023-11-23 10:29:47.000000 matfree-0.0.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2023-11-23 10:29:47.000000 matfree-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.104858 matfree-0.0.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-11-23 10:29:47.000000 matfree-0.0.9/scripts/generate_api_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2023-11-23 10:29:47.000000 matfree-0.0.9/scripts/readme_to_dev_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2023-11-23 10:29:47.000000 matfree-0.0.9/scripts/tutorials_to_py_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-23 10:29:57.108858 matfree-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.096858 matfree-0.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.104858 matfree-0.0.9/tests/test_decomp/
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_decomp/test_bidiagonal_full_reortho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_decomp/test_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_decomp/test_tridiagonal_full_reortho.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.104858 matfree-0.0.9/tests/test_hutchinson/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_hutchinson/test_diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_hutchinson/test_estimate_multiple_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_hutchinson/test_frobeniusnorm_squared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_hutchinson/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_hutchinson/test_trace_and_diagonal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_hutchinson/test_trace_moments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.104858 matfree-0.0.9/tests/test_pinv/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_pinv/test_pseudo_inverse_correct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.104858 matfree-0.0.9/tests/test_slq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_slq/test_logdet_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_slq/test_logdet_spd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2023-11-23 10:29:47.000000 matfree-0.0.9/tests/test_slq/test_schatten_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:29:57.108858 matfree-0.0.9/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2023-11-23 10:29:47.000000 matfree-0.0.9/tutorials/1_log_determinants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2023-11-23 10:29:47.000000 matfree-0.0.9/tutorials/2_pytree_logdeterminants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-11-23 10:29:47.000000 matfree-0.0.9/tutorials/3_uncertainty_quantification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-11-23 10:29:47.000000 matfree-0.0.9/tutorials/4_control_variates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2023-11-23 10:29:47.000000 matfree-0.0.9/tutorials/5_vector_calculus.py
```

### Comparing `matfree-0.0.8/.github/workflows/ci.yaml` & `matfree-0.0.9/.github/workflows/ci.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   test:
     name: Test with ${{ matrix.python-version }} on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     timeout-minutes: 10
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.9', '3.10', '3.11']
+        python-version: ['3.9', '3.10', '3.11', '3.12']
         os: [ubuntu-latest]
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
@@ -60,10 +60,10 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           pip install --upgrade pip
-          pip install .[doc]
+          pip install .[cpu,doc]
       - name: Build documentation
-        run: make doc
+        run: make doc-build
```

### Comparing `matfree-0.0.8/.github/workflows/doc-publish.yml` & `matfree-0.0.9/.github/workflows/doc-publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -25,10 +25,10 @@
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           pip install --upgrade pip
           pip install .[cpu,doc]
       - name: Build the HTML docs
-        run: make doc
+        run: make doc-build
       - name: Publish the HTML docs
         run: mkdocs gh-deploy --force --clean --verbose
```

### Comparing `matfree-0.0.8/.github/workflows/release.yml` & `matfree-0.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.8/.gitignore` & `matfree-0.0.9/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,26 @@
+# Don't track the version
 matfree/_version.py
 
+# Don't track linter-caches
+.mypy_cache
+.ruff_cache
+.pytest_cache
+
+
+# Don't track the automatically generated docs (they are automatically generated)
+docs/index.md
+docs/API*/
+docs/Developer*/
+docs/Tutorial*/
+
 # Don't version jupyter notebooks. Track synced markdown files.
 *.ipynb
 
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `matfree-0.0.8/.pre-commit-config.yaml` & `matfree-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `matfree-0.0.8/LICENSE` & `matfree-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `matfree-0.0.8/docs/vector_calculus.md` & `matfree-0.0.9/tutorials/5_vector_calculus.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,104 +1,93 @@
-# Vector calculus
+"""Implement vector calculus in linear complexity.
 
-Implementing vector calculus with conventional algorithmic differentiation can be inefficient.
-For example, computing the divergence of a vector field requires computing the trace of a Jacobian.
-The divergence of a vector field is important when evaluating Laplacians of scalar functions.
+Implementing vector calculus with conventional
+algorithmic differentiation can be inefficient.
+For example, computing the divergence of a
+vector field requires computing the trace of a Jacobian.
+The divergence of a vector field is
+important when evaluating Laplacians of scalar functions.
 
-Here is how we can implement divergences and Laplacians without forming full Jacobian matrices:
+Here is how we can implement divergences and
+Laplacians without forming full Jacobian matrices:
+"""
 
+import jax
+import jax.numpy as jnp
 
+from matfree import hutchinson
 
-```python
->>> import jax
->>> import jax.numpy as jnp
->>> from matfree import hutchinson, montecarlo
+# ## Divergences and Laplacians
+#
+# The divergence of a vector field is the trace of its Jacobian.
+# The conventional implementation would look like this:
 
-```
 
-## Divergences and Laplacians
+def divergence_dense(vf):
+    """Compute the divergence of a vector field."""
 
-The divergence of a vector field is the trace of its Jacobian.
-The conventional implementation would look like this:
+    def div_fn(x):
+        J = jax.jacfwd(vf)
+        return jnp.trace(J(x))
 
-```python
+    return div_fn
 
->>> def divergence_dense(vf):
-...     """Compute the divergence of a vector field."""
-...
-...     def div_fn(x):
-...         J = jax.jacfwd(vf)
-...         return jnp.trace(J(x))
-...
-...     return div_fn
-...
 
-```
-This implementation computes the divergence of a vector field:
+# This implementation computes the divergence of a vector field:
 
-```python
->>> def fun(x):
-...     """A scalar valued function."""
-...     return jnp.dot(x, x) ** 2
-...
->>> x0 = jnp.arange(1.0, 4.0)
->>> gradient = jax.grad(fun)
->>> laplacian = divergence_dense(gradient)
->>> print(jax.hessian(fun)(x0))
-[[ 64.  16.  24.]
- [ 16.  88.  48.]
- [ 24.  48. 128.]]
 
->>> print(laplacian(x0))
-280.0
+def fun(x):
+    """Evaluate a scalar valued function."""
+    return jnp.dot(x, x) ** 2
 
-```
 
-But the implementation above requires $O(d^2)$ storage because it evaluates the dense Jacobian.
-This is problematic for high-dimensional problems.
+x0 = jnp.arange(1.0, 4.0)
+gradient = jax.grad(fun)
+laplacian = divergence_dense(gradient)
+print(jax.hessian(fun)(x0))
+print(laplacian(x0))
 
-## Matrix-free implementation
 
-If we have access to Jacobian-vector products (which we usually do), we can use matrix-free trace estimation
-to approximate divergences and Laplacians without forming full Jacobians:
+# But the implementation above requires $O(d^2)$ storage
+# because it evaluates the dense Jacobian.
+# This is problematic for high-dimensional problems.
+#
+# ## Matrix-free implementation
+#
+# If we have access to Jacobian-vector products (which we usually do),
+# we can use matrix-free trace estimation
+# to approximate divergences and Laplacians without forming full Jacobians:
+#
 
 
-```python
+def divergence_matfree(vf, /, *, num):
+    """Compute the divergence with Hutchinson's estimator."""
 
->>> def divergence_matfree(vf, *, key, sample_fun):
-...     """Estimate the divergence of a vector field."""
-...
-...     def div_fn(x):
-...         def jvp(v):
-...             _vf_val, jvp_val = jax.jvp(fun=vf, primals=(x,), tangents=(v,))
-...             return jvp_val
-...
-...         return hutchinson.trace(jvp, key=key, sample_fun=sample_fun)
-...
-...     return div_fn
-...
+    def divergence(k, x):
+        _fx, jvp = jax.linearize(vf, x)
+        integrand_laplacian = hutchinson.integrand_trace(jvp)
+        normal = hutchinson.sampler_normal(x, num=num)
+        estimator = hutchinson.hutchinson(integrand_laplacian, sample_fun=normal)
+        return estimator(k)
 
-```
-The difference to the above implementation is that `divergence_matfree` does not form dense Jacobians.
-It requires $O(d)$ memory and  $O(d N)$ operations (for $N$ Monte-Carlo samples).
-For large-scale problems, it may be the only way of computing Laplacians reliably.
+    return divergence
 
-```python
->>> laplacian_dense = divergence_dense(gradient)
->>>
->>> normal = montecarlo.normal(shape=(3,))
->>> key = jax.random.PRNGKey(1)
->>> laplacian_matfree = divergence_matfree(gradient, key=key, sample_fun=normal)
->>>
->>> print(jnp.round(laplacian_dense(x0), 1))
-280.0
 
->>> print(jnp.round(laplacian_matfree(x0), 1))
-278.4
+# -
+# The difference to the "naive" implementation is that the implicit one
+# does not form dense Jacobians. It requires $O(d)$ memory and
+# $O(d N)$ operations (for $N$ Monte-Carlo samples).
+# For large-scale problems, it may be the only way of computing Laplacians reliably.
 
-```
+laplacian_matfree = divergence_matfree(gradient, num=10_000)
+print(laplacian(x0))
+print(laplacian_matfree(jax.random.PRNGKey(1), x0))
 
-In summary, compute matrix-free linear algebra and algorithmic differentiation to implement vector calculus.
 
-## Jacobian diagonals
-
-If we replace trace estimation with diagonal estimation, we can compute the diagonal of Jacobian matrices in $O(d)$ memory and $O(dN)$ operations
+# In summary, compute matrix-free linear algebra
+# and algorithmic differentiation to implement vector calculus.
+#
+# ## Diagonals of Jacobians
+#
+# If we replace trace estimation with diagonal estimation,
+# we can compute the diagonal of Jacobian matrices in
+# $O(d)$ memory and $O(dN)$ operations.
```

### Comparing `matfree-0.0.8/matfree/backend/control_flow.py` & `matfree-0.0.9/matfree/backend/control_flow.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.8/matfree/backend/func.py` & `matfree-0.0.9/matfree/backend/func.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.8/matfree/backend/linalg.py` & `matfree-0.0.9/matfree/backend/linalg.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.8/matfree/backend/np.py` & `matfree-0.0.9/matfree/backend/np.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-"""NumPy-style API."""
+"""NumPy-style API.
 
-# In here, we loosely follow the Array API:
-#
-# https://data-apis.org/array-api/2022.12/
-#
-# But deviate in a few points:
-# * The functions here do not have all the arguments specified in the API
-#   (we only wrap the arguments we need)
-# * Our current version of diag/diagonal is slightly different
-# * We do not use methods on Array types, e.g. shape(), dtype(). Instead
-#   these are functions. (Not all backends might always follow this method interface.)
-# * We do not implement any constants (e.g. NaN, Pi). Instead, these are methods.
-# * We call max/min/amax/amin array_max and elementwise_max.
-#   This is more verbose than what the array API suggests.
+In here, we loosely follow the Array API:
+
+https://data-apis.org/array-api/2022.12/
+
+But deviate in a few points:
+* The functions here do not have all the arguments specified in the API
+  (we only wrap the arguments we need)
+* Our current version of diag/diagonal is slightly different
+* We do not use methods on Array types, e.g. shape(), dtype(). Instead,
+  these are functions. (Not all backends might always follow this method interface.)
+* We do not implement any constants (e.g. NaN, Pi). Instead, these are functions.
+* We call max/min/amax/amin array_max and elementwise_max.
+  This is more verbose than what the array API suggests.
+
+"""
 
 import jax.numpy as jnp
 
 # Creation functions:
 
 
 def arange(start, /, stop=None, step=1):
```

### Comparing `matfree-0.0.8/matfree/backend/prng.py` & `matfree-0.0.9/matfree/backend/prng.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.8/matfree/lanczos.py` & `matfree-0.0.9/matfree/decomp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Lanczos-style algorithms."""
+"""Matrix decomposition algorithms."""
 
 from matfree.backend import containers, control_flow, linalg, np
 from matfree.backend.typing import Array, Callable, Tuple
 
 
 class _Alg(containers.NamedTuple):
     """Matrix decomposition algorithm."""
@@ -16,15 +16,15 @@
     extract: Callable
     """Extract the solution from the state of the algorithm."""
 
     lower_upper: Tuple[int, int]
     """Range of the for-loop used to decompose a matrix."""
 
 
-def tridiagonal_full_reortho(depth, /):
+def lanczos_tridiag_full_reortho(depth, /):
     """Construct an implementation of **tridiagonalisation**.
 
     Uses pre-allocation. Fully reorthogonalise vectors at every step.
 
     This algorithm assumes a **symmetric matrix**.
 
     Decompose a matrix into a product of orthogonal-**tridiagonal**-orthogonal matrices.
@@ -79,15 +79,15 @@
     def extract(state: State, /):
         _, basis, (diag, offdiag), _ = state
         return basis, (diag, offdiag)
 
     return _Alg(init=init, step=apply, extract=extract, lower_upper=(0, depth + 1))
 
 
-def bidiagonal_full_reortho(depth, /, matrix_shape):
+def lanczos_bidiag_full_reortho(depth, /, matrix_shape):
     """Construct an implementation of **bidiagonalisation**.
 
     Uses pre-allocation. Fully reorthogonalise vectors at every step.
 
     Works for **arbitrary matrices**. No symmetry required.
 
     Decompose a matrix into a product of orthogonal-**bidiagonal**-orthogonal matrices.
@@ -155,7 +155,100 @@
     return vec, coeffs
 
 
 def _gram_schmidt_orthogonalise(vec1, vec2):
     coeff = linalg.vecdot(vec1, vec2)
     vec_ortho = vec1 - coeff * vec2
     return vec_ortho, coeff
+
+
+def svd_approx(
+    v0: Array, depth: int, Av: Callable, vA: Callable, matrix_shape: Tuple[int, ...]
+):
+    """Approximate singular value decomposition.
+
+    Uses GKL with full reorthogonalisation to bi-diagonalise the target matrix
+    and computes the full SVD of the (small) bidiagonal matrix.
+
+    Parameters
+    ----------
+    v0:
+        Initial vector for Golub-Kahan-Lanczos bidiagonalisation.
+    depth:
+        Depth of the Krylov space constructed by Golub-Kahan-Lanczos bidiagonalisation.
+        Choosing `depth = min(nrows, ncols) - 1` would yield behaviour similar to
+        e.g. `np.linalg.svd`.
+    Av:
+        Matrix-vector product function.
+    vA:
+        Vector-matrix product function.
+    matrix_shape:
+        Shape of the matrix involved in matrix-vector and vector-matrix products.
+    """
+    # Factorise the matrix
+    algorithm = lanczos_bidiag_full_reortho(depth, matrix_shape=matrix_shape)
+    u, (d, e), vt, _ = decompose_fori_loop(v0, Av, vA, algorithm=algorithm)
+
+    # Compute SVD of factorisation
+    B = _bidiagonal_dense(d, e)
+    U, S, Vt = linalg.svd(B, full_matrices=False)
+
+    # Combine orthogonal transformations
+    return u @ U, S, Vt @ vt
+
+
+def _bidiagonal_dense(d, e):
+    diag = linalg.diagonal_matrix(d)
+    offdiag = linalg.diagonal_matrix(e, 1)
+    return diag + offdiag
+
+
+class _DecompAlg(containers.NamedTuple):
+    """Matrix decomposition algorithm."""
+
+    init: Callable
+    """Initialise the state of the algorithm. Usually, this involves pre-allocation."""
+
+    step: Callable
+    """Compute the next iteration."""
+
+    extract: Callable
+    """Extract the solution from the state of the algorithm."""
+
+    lower_upper: Tuple[int, int]
+    """Range of the for-loop used to decompose a matrix."""
+
+
+AlgorithmType = Tuple[Callable, Callable, Callable, Tuple[int, int]]
+"""Decomposition algorithm type.
+
+For example, the output of
+[matfree.decomp.lanczos_tridiag_full_reortho(...)][matfree.decomp.lanczos_tridiag_full_reortho].
+"""
+
+
+# all arguments are positional-only because we will rename arguments a lot
+def decompose_fori_loop(v0, *matvec_funs, algorithm: AlgorithmType):
+    r"""Decompose a matrix purely based on matvec-products with A.
+
+    The behaviour of this function is equivalent to
+
+    ```python
+    def decompose(v0, *matvec_funs, algorithm):
+        init, step, extract, (lower, upper) = algorithm
+        state = init(v0)
+        for _ in range(lower, upper):
+            state = step(state, *matvec_funs)
+        return extract(state)
+    ```
+
+    but the implementation uses JAX' fori_loop.
+    """
+    # todo: turn the "practically equivalent" bit above into a doctest.
+    init, step, extract, (lower, upper) = algorithm
+    init_val = init(v0)
+
+    def body_fun(_, s):
+        return step(s, *matvec_funs)
+
+    result = control_flow.fori_loop(lower, upper, body_fun=body_fun, init_val=init_val)
+    return extract(result)
```

### Comparing `matfree-0.0.8/matfree/pinv.py` & `matfree-0.0.9/matfree/pinv.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.8/matfree/slq.py` & `matfree-0.0.9/matfree/slq.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,96 +1,114 @@
-"""Stochastic Lanczos quadrature."""
+"""Stochastic Lanczos quadrature.
 
-from matfree import decomp, lanczos, montecarlo
-from matfree.backend import func, linalg, np
+The [slq][matfree.slq] module extends the integrands
+in [hutchinson][matfree.hutchinson] to those that implement
+stochastic Lanczos quadrature.
+"""
 
+from matfree import decomp
+from matfree.backend import func, linalg, np, tree_util
 
-def logdet_spd(*args, **kwargs):
-    """Estimate the log-determinant of a symmetric, positive definite matrix."""
-    return trace_of_matfun_spd(np.log, *args, **kwargs)
 
+def integrand_logdet_spd(order, matvec, /):
+    """Construct the integrand for the log-determinant.
 
-def trace_of_matfun_spd(matfun, order, Av, /, **kwargs):
-    """Compute the trace of the function of a symmetric matrix."""
-    quadratic_form = _quadratic_form_slq_spd(matfun, order, Av)
-    return montecarlo.estimate(quadratic_form, **kwargs)
+    This function assumes a symmetric, positive definite matrix.
+    """
+    return integrand_slq_spd(np.log, order, matvec)
 
 
-def _quadratic_form_slq_spd(matfun, order, Av, /):
+def integrand_slq_spd(matfun, order, matvec, /):
     """Quadratic form for stochastic Lanczos quadrature.
 
-    Assumes a symmetric, positive definite matrix.
+    This function assumes a symmetric, positive definite matrix.
     """
 
     def quadform(v0, /):
-        algorithm = lanczos.tridiagonal_full_reortho(order)
-        _, tridiag = decomp.decompose_fori_loop(v0, Av, algorithm=algorithm)
+        v0_flat, v_unflatten = tree_util.ravel_pytree(v0)
+
+        def matvec_flat(v_flat):
+            v = v_unflatten(v_flat)
+            Av = matvec(v)
+            flat, unflatten = tree_util.ravel_pytree(Av)
+            return flat
+
+        algorithm = decomp.lanczos_tridiag_full_reortho(order)
+        _, tridiag = decomp.decompose_fori_loop(
+            v0_flat, matvec_flat, algorithm=algorithm
+        )
         (diag, off_diag) = tridiag
 
         # todo: once jax supports eigh_tridiagonal(eigvals_only=False),
         #  use it here. Until then: an eigen-decomposition of size (order + 1)
         #  does not hurt too much...
         diag = linalg.diagonal_matrix(diag)
         offdiag1 = linalg.diagonal_matrix(off_diag, -1)
         offdiag2 = linalg.diagonal_matrix(off_diag, 1)
         dense_matrix = diag + offdiag1 + offdiag2
         eigvals, eigvecs = linalg.eigh(dense_matrix)
 
         # Since Q orthogonal (orthonormal) to v0, Q v = Q[0],
         # and therefore (Q v)^T f(D) (Qv) = Q[0] * f(diag) * Q[0]
-        (dim,) = v0.shape
+        (dim,) = v0_flat.shape
 
         fx_eigvals = func.vmap(matfun)(eigvals)
         return dim * linalg.vecdot(eigvecs[0, :], fx_eigvals * eigvecs[0, :])
 
     return quadform
 
 
-def logdet_product(*args, **kwargs):
-    r"""Compute the log-determinant of a product of matrices.
+def integrand_logdet_product(depth, matvec, vecmat, /):
+    r"""Construct the integrand for the log-determinant of a matrix-product.
 
     Here, "product" refers to $X = A^\top A$.
     """
-    return trace_of_matfun_product(np.log, *args, **kwargs)
+    return integrand_slq_product(np.log, depth, matvec, vecmat)
 
 
-def schatten_norm(*args, power, **kwargs):
-    r"""Compute the Schatten-p norm of a matrix via stochastic Lanczos quadrature."""
+def integrand_schatten_norm(power, depth, matvec, vecmat, /):
+    r"""Construct the integrand for the p-th power of the Schatten-p norm."""
 
     def matfun(x):
         """Matrix-function for Schatten-p norms."""
         return x ** (power / 2)
 
-    trace = trace_of_matfun_product(matfun, *args, **kwargs)
-    return trace ** (1 / power)
-
+    return integrand_slq_product(matfun, depth, matvec, vecmat)
 
-def trace_of_matfun_product(matfun, order, *matvec_funs, matrix_shape, **kwargs):
-    r"""Compute the trace of a function of a product of matrices.
 
-    Here, "product" refers to $X = A^\top A$.
-    """
-    quadratic_form = _quadratic_form_slq_product(
-        matfun, order, *matvec_funs, matrix_shape=matrix_shape
-    )
-    return montecarlo.estimate(quadratic_form, **kwargs)
-
-
-def _quadratic_form_slq_product(matfun, depth, *matvec_funs, matrix_shape):
-    r"""Quadratic form for stochastic Lanczos quadrature.
+def integrand_slq_product(matfun, depth, matvec, vecmat, /):
+    r"""Construct the integrand for the trace of a function of a matrix-product.
 
     Instead of the trace of a function of a matrix,
     compute the trace of a function of the product of matrices.
     Here, "product" refers to $X = A^\top A$.
     """
 
     def quadform(v0, /):
+        v0_flat, v_unflatten = tree_util.ravel_pytree(v0)
+
+        def matvec_flat(v_flat):
+            v = v_unflatten(v_flat)
+            Av = matvec(v)
+            flat, unflatten = tree_util.ravel_pytree(Av)
+            return flat, tree_util.partial_pytree(unflatten)
+
+        w0_flat, w_unflatten = func.eval_shape(matvec_flat, v0_flat)
+        matrix_shape = (*np.shape(w0_flat), *np.shape(v0_flat))
+
+        def vecmat_flat(w_flat):
+            w = w_unflatten(w_flat)
+            wA = vecmat(w)
+            return tree_util.ravel_pytree(wA)[0]
+
         # Decompose into orthogonal-bidiag-orthogonal
-        algorithm = lanczos.bidiagonal_full_reortho(depth, matrix_shape=matrix_shape)
-        output = decomp.decompose_fori_loop(v0, *matvec_funs, algorithm=algorithm)
+        algorithm = decomp.lanczos_bidiag_full_reortho(depth, matrix_shape=matrix_shape)
+        output = decomp.decompose_fori_loop(
+            v0_flat, lambda v: matvec_flat(v)[0], vecmat_flat, algorithm=algorithm
+        )
         u, (d, e), vt, _ = output
 
         # Compute SVD of factorisation
         B = _bidiagonal_dense(d, e)
         _, S, Vt = linalg.svd(B, full_matrices=False)
 
         # Since Q orthogonal (orthonormal) to v0, Q v = Q[0],
```

### Comparing `matfree-0.0.8/matfree/test_util.py` & `matfree-0.0.9/matfree/test_util.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.8/mkdocs.yml` & `matfree-0.0.9/mkdocs.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,63 @@
 ---
 site_name: matfree documentation
 repo_url: https://github.com/pnkraemer/matfree
 repo_name: pnkraemer/matfree
-nav:
-  - Get started: index.md
-  - Tutorials:
-      - control_variates.md
-      - log_determinants.md
-      - higher_moments.md
-      - vector_calculus.md
-      - pytree_logdeterminants.md
-  - API documentation:
-      - matfree.montecarlo: api/montecarlo.md
-      - matfree.decomp: api/decomp.md
-      - matfree.lanczos: api/lanczos.md
-      - matfree.hutchinson: api/hutchinson.md
-      - matfree.slq: api/slq.md
-      - matfree.pinv: api/pinv.md
-  - Developer documentation: dev/index.md
-  - Benchmarks: benchmarks/index.md
 theme:
   name: material
   palette:
-
-    # Palette toggle for light mode
     - media: '(prefers-color-scheme: light)'
       scheme: default
       primary: white
       toggle:
         icon: material/brightness-7
         name: Switch to dark mode
-
-    # Palette toggle for dark mode
     - media: '(prefers-color-scheme: light)'
       scheme: slate
       primary: black
       toggle:
         icon: material/brightness-4
         name: Switch to light mode
   font:
     text: Fira Sans
   features: [navigation.sections, navigation.footer]
 plugins:
   - search
+  - mkdocs-jupyter:
+      include: ['*.py']
+      execute: true
+      allow_errors: false
   - mkdocstrings:
       handlers:
         python:
           options:
             show_root_heading: true
             show_root_toc_entry: true
             show_root_full_path: true
             show_root_members_full_path: true
-            show_object_full_path: false
-            show_category_heading: true
+            show_object_full_path: true
+            show_category_heading: false
             docstring_style: numpy
             show_if_no_docstring: true
             members_order: alphabetical
             annotations_path: brief
             show_signature: true
             show_signature_annotations: true
             separate_signature: false
             docstring_section_style: list
+            show_source: false
 watch: [matfree]
 extra:
   social:
-    - icon: fontawesome/brands/twitter
+    - icon: fontawesome/brands/x-twitter
       link: https://twitter.com/@pnkraemer
-      name: Nico
+      name: pnkraemer on X
+    - icon: fontawesome/brands/github
+      link: https://github.com/pnkraemer
+      name: pnkraemer on GitHub
   generator: false
 copyright: Copyright &copy; 2023 Nicholas Krämer
 markdown_extensions:
   - pymdownx.superfences
   - pymdownx.arithmatex:
       generic: true
 extra_javascript:
```

### Comparing `matfree-0.0.8/pyproject.toml` & `matfree-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dynamic = ["version"]
 
 
 [project.optional-dependencies]
 cpu = [
     "jax[cpu]",
@@ -41,14 +42,16 @@
     "black",
 ]
 doc = [
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings",
     "mkdocstrings-python",
+    "mkdocs-jupyter",
+    "mkdocs-awesome-pages-plugin",
     "matplotlib",
     "tqdm",
 ]
 full = [
     "matfree[cpu]",
     "matfree[test]",
     "matfree[lint]",
@@ -118,23 +121,15 @@
     "B905",
     # Magic methods don't need a docstring:
     "D105",
 ]
 
 [tool.ruff.per-file-ignores]
 # We don't write docstrings for the backend
-"matfree/backend/control_flow.py" = ["D103"]
-"matfree/backend/func.py" = ["D103"]
-"matfree/backend/linalg.py" = ["D103"]
-"matfree/backend/np.py" = ["D103"]
-"matfree/backend/plt.py" = ["D103"]
-"matfree/backend/prng.py" = ["D103"]
-"matfree/backend/progressbar.py" = ["D103"]
-"matfree/backend/testing.py" = ["D103"]
-"matfree/backend/time.py" = ["D103"]
+"matfree/backend/*.py" = ["D103"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 
 [tool.isort]
 multi_line_output = "3"
```

### Comparing `matfree-0.0.8/tests/test_decomp/test_svd.py` & `matfree-0.0.9/tests/test_decomp/test_svd.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def Av(v):
         return A @ v
 
     def vA(v):
         return v @ A
 
     v0 = np.ones((ncols,))
-    U, S, Vt = decomp.svd(v0, depth, Av, vA, matrix_shape=np.shape(A))
+    U, S, Vt = decomp.svd_approx(v0, depth, Av, vA, matrix_shape=np.shape(A))
     U_, S_, Vt_ = linalg.svd(A, full_matrices=False)
 
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
     assert np.allclose(S, S_)  # strict "allclose"
 
     assert np.shape(U) == np.shape(U_)
     assert np.shape(Vt) == np.shape(Vt_)
```

### Comparing `matfree-0.0.8/tests/test_lanczos/test_bidiagonal_full_reortho.py` & `matfree-0.0.9/tests/test_decomp/test_bidiagonal_full_reortho.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for GKL bidiagonalisation."""
 
-from matfree import decomp, lanczos, test_util
+from matfree import decomp, test_util
 from matfree.backend import linalg, np, prng, testing
 
 
 @testing.fixture()
 def A(nrows, ncols, num_significant_singular_vals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
@@ -14,20 +14,20 @@
     return test_util.asymmetric_matrix_from_singular_values(d, nrows=nrows, ncols=ncols)
 
 
 @testing.parametrize("nrows", [50])
 @testing.parametrize("ncols", [49])
 @testing.parametrize("num_significant_singular_vals", [4])
 @testing.parametrize("order", [6])  # ~1.5 * num_significant_eigvals
-def test_bidiagonal_full_reortho(A, order):
+def test_lanczos_bidiag_full_reortho(A, order):
     """Test that Lanczos tridiagonalisation yields an orthogonal-tridiagonal decomp."""
     nrows, ncols = np.shape(A)
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(ncols,))
-    alg = lanczos.bidiagonal_full_reortho(order, matrix_shape=np.shape(A))
+    alg = decomp.lanczos_bidiag_full_reortho(order, matrix_shape=np.shape(A))
 
     def Av(v):
         return A @ v
 
     def vA(v):
         return v @ A
 
@@ -70,34 +70,34 @@
 @testing.parametrize("num_significant_singular_vals", [3])
 def test_error_too_high_depth(A):
     """Assert that a ValueError is raised when the depth exceeds the matrix size."""
     nrows, ncols = np.shape(A)
     max_depth = min(nrows, ncols) - 1
 
     with testing.raises(ValueError):
-        _ = lanczos.bidiagonal_full_reortho(max_depth + 1, matrix_shape=np.shape(A))
+        _ = decomp.lanczos_bidiag_full_reortho(max_depth + 1, matrix_shape=np.shape(A))
 
 
 @testing.parametrize("nrows", [5])
 @testing.parametrize("ncols", [3])
 @testing.parametrize("num_significant_singular_vals", [3])
 def test_error_too_low_depth(A):
     """Assert that a ValueError is raised when the depth is negative."""
     min_depth = 0
     with testing.raises(ValueError):
-        _ = lanczos.bidiagonal_full_reortho(min_depth - 1, matrix_shape=np.shape(A))
+        _ = decomp.lanczos_bidiag_full_reortho(min_depth - 1, matrix_shape=np.shape(A))
 
 
 @testing.parametrize("nrows", [15])
 @testing.parametrize("ncols", [3])
 @testing.parametrize("num_significant_singular_vals", [3])
 def test_no_error_zero_depth(A):
     """Assert the corner case of zero-depth does not raise an error."""
     nrows, ncols = np.shape(A)
-    algorithm = lanczos.bidiagonal_full_reortho(0, matrix_shape=np.shape(A))
+    algorithm = decomp.lanczos_bidiag_full_reortho(0, matrix_shape=np.shape(A))
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(ncols,))
 
     def Av(v):
         return A @ v
 
     def vA(v):
```

### Comparing `matfree-0.0.8/tests/test_lanczos/test_tridiagonal_full_reortho.py` & `matfree-0.0.9/tests/test_decomp/test_tridiagonal_full_reortho.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Tests for Lanczos functionality."""
 
-from matfree import decomp, lanczos, test_util
+from matfree import decomp, test_util
 from matfree.backend import linalg, np, prng, testing
 
 
 @testing.fixture()
 def A(n, num_significant_eigvals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
@@ -18,15 +18,15 @@
 @testing.parametrize("num_significant_eigvals", [6])
 def test_max_order(A):
     """If m == n, the matrix should be equal to the full tridiagonal."""
     n, _ = np.shape(A)
     order = n - 1
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
-    alg = lanczos.tridiagonal_full_reortho(order)
+    alg = decomp.lanczos_tridiag_full_reortho(order)
     Q, (d_m, e_m) = decomp.decompose_fori_loop(v0, lambda v: A @ v, algorithm=alg)
 
     # Lanczos is not stable.
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
 
     # Since full-order mode: Q must be unitary
     assert np.shape(Q) == (order + 1, n)
@@ -59,15 +59,15 @@
 @testing.parametrize("num_significant_eigvals", [4])
 @testing.parametrize("order", [6])  # ~1.5 * num_significant_eigvals
 def test_identity(A, order):
     """Test that Lanczos tridiagonalisation yields an orthogonal-tridiagonal decomp."""
     n, _ = np.shape(A)
     key = prng.prng_key(1)
     v0 = prng.normal(key, shape=(n,))
-    alg = lanczos.tridiagonal_full_reortho(order)
+    alg = decomp.lanczos_tridiag_full_reortho(order)
     Q, tridiag = decomp.decompose_fori_loop(v0, lambda v: A @ v, algorithm=alg)
     (d_m, e_m) = tridiag
 
     # Lanczos is not stable.
     tols_decomp = {"atol": 1e-5, "rtol": 1e-5}
 
     assert np.shape(Q) == (order + 1, n)
```

### Comparing `matfree-0.0.8/tests/test_pinv/test_pseudo_inverse_correct.py` & `matfree-0.0.9/tests/test_pinv/test_pseudo_inverse_correct.py`

 * *Files identical despite different names*

### Comparing `matfree-0.0.8/tests/test_slq/test_logdet_product.py` & `matfree-0.0.9/tests/test_slq/test_logdet_spd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-"""Test slq.logdet_prod()."""
+"""Tests for Lanczos functionality."""
 
-from matfree import montecarlo, slq, test_util
+from matfree import hutchinson, slq, test_util
 from matfree.backend import linalg, np, prng, testing
 
 
 @testing.fixture()
-def A(nrows, ncols, num_significant_singular_vals):
+def A(n, num_significant_eigvals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
-    n = min(nrows, ncols)
-    d = np.arange(n) + 1.0
-    d = d.at[num_significant_singular_vals:].set(0.001)
-    return test_util.asymmetric_matrix_from_singular_values(d, nrows=nrows, ncols=ncols)
-
-
-@testing.parametrize("nrows", [50])
-@testing.parametrize("ncols", [30])
-@testing.parametrize("num_significant_singular_vals", [30])
-@testing.parametrize("order", [20])
-def test_logdet_product(A, order):
-    """Assert that logdet_product yields an accurate estimate."""
-    _, ncols = np.shape(A)
-    key = prng.prng_key(3)
-    fun = montecarlo.normal(shape=(ncols,))
-    received = slq.logdet_product(
-        order,
-        lambda v: A @ v,
-        lambda v: A.T @ v,
-        matrix_shape=np.shape(A),
-        key=key,
-        num_samples_per_batch=200,
-        num_batches=2,
-        sample_fun=fun,
-    )
-    expected = linalg.slogdet(A.T @ A)[1]
+    d = np.arange(n) / n + 1.0
+    d = d.at[num_significant_eigvals:].set(0.001)
+
+    return test_util.symmetric_matrix_from_eigenvalues(d)
+
+
+@testing.parametrize("n", [200])
+@testing.parametrize("num_significant_eigvals", [30])
+@testing.parametrize("order", [10])
+# usually: ~1.5 * num_significant_eigvals.
+# But logdet seems to converge sooo much faster.
+def test_logdet_spd(A, order):
+    """Assert that the log-determinant estimation matches the true log-determinant."""
+    n, _ = np.shape(A)
+
+    def matvec(x):
+        return {"fx": A @ x["fx"]}
+
+    key = prng.prng_key(1)
+    args_like = {"fx": np.ones((n,), dtype=float)}
+    sampler = hutchinson.sampler_normal(args_like, num=10)
+    integrand = slq.integrand_logdet_spd(order, matvec)
+    estimate = hutchinson.hutchinson(integrand, sampler)
+    received = estimate(key)
+
+    expected = linalg.slogdet(A)[1]
     print_if_assert_fails = ("error", np.abs(received - expected), "target:", expected)
     assert np.allclose(received, expected, atol=1e-2, rtol=1e-2), print_if_assert_fails
```

### Comparing `matfree-0.0.8/tests/test_slq/test_schatten_norm.py` & `matfree-0.0.9/tests/test_slq/test_schatten_norm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Test Schatten norm implementations."""
 
-from matfree import montecarlo, slq, test_util
+from matfree import hutchinson, slq, test_util
 from matfree.backend import linalg, np, prng, testing
 
 
 @testing.fixture()
 def A(nrows, ncols, num_significant_singular_vals):
     """Make a positive definite matrix with certain spectrum."""
     # 'Invent' a spectrum. Use the number of pre-defined eigenvalues.
@@ -16,27 +16,24 @@
 
 @testing.parametrize("nrows", [30])
 @testing.parametrize("ncols", [30])
 @testing.parametrize("num_significant_singular_vals", [30])
 @testing.parametrize("order", [20])
 @testing.parametrize("power", [1, 2, 5])
 def test_schatten_norm(A, order, power):
-    """Assert that schatten_norm yields an accurate estimate."""
+    """Assert that the Schatten norm is accurate."""
     _, s, _ = linalg.svd(A, full_matrices=False)
-    expected = np.sum(s**power) ** (1 / power)
+    expected = np.sum(s**power)
 
     _, ncols = np.shape(A)
-    key = prng.prng_key(1)
-    fun = montecarlo.normal(shape=(ncols,))
-    received = slq.schatten_norm(
-        order,
-        lambda v: A @ v,
-        lambda v: A.T @ v,
-        power=power,
-        matrix_shape=np.shape(A),
-        key=key,
-        num_samples_per_batch=100,
-        num_batches=5,
-        sample_fun=fun,
+    args_like = np.ones((ncols,), dtype=float)
+    sampler = hutchinson.sampler_normal(args_like, num=500)
+    integrand = slq.integrand_schatten_norm(
+        power, order, lambda v: A @ v, lambda v: A.T @ v
     )
+    estimate = hutchinson.hutchinson(integrand, sampler)
+
+    key = prng.prng_key(1)
+    received = estimate(key)
+
     print_if_assert_fails = ("error", np.abs(received - expected), "target:", expected)
     assert np.allclose(received, expected, atol=1e-2, rtol=1e-2), print_if_assert_fails
```

