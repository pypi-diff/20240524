# Comparing `tmp/ncopt-0.0.1.tar.gz` & `tmp/ncopt-0.2.0.tar.gz`

## Comparing `ncopt-0.0.1.tar` & `ncopt-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ncopt-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 ncopt-0.0.1/CITATION.cff
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 ncopt-0.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ncopt-0.0.1/data/checkpoints/README.md
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 ncopt-0.0.1/data/checkpoints/max2d.pt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ncopt-0.0.1/data/img/README.md
--rw-r--r--   0        0        0    18147 2020-02-02 00:00:00.000000 ncopt-0.0.1/data/img/checkpoint.png
--rw-r--r--   0        0        0    84858 2020-02-02 00:00:00.000000 ncopt-0.0.1/data/img/rosenbrock.png
--rw-r--r--   0        0        0   111582 2020-02-02 00:00:00.000000 ncopt-0.0.1/data/img/timings_residual.png
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ncopt-0.0.1/examples/example_checkpoint.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 ncopt-0.0.1/examples/example_residual.py
--rwxr-xr-x   0        0        0     2839 2020-02-02 00:00:00.000000 ncopt-0.0.1/examples/example_rosenbrock.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 ncopt-0.0.1/scripts/timing_rosenbrock.py
--rwxr-xr-x   0        0        0     3275 2020-02-02 00:00:00.000000 ncopt-0.0.1/scripts/train_max_fun.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/__about__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/__init__.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/plot_utils.py
--rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/utils.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/functions/__init__.py
--rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/functions/main.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/functions/max_linear.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/functions/norm_residual.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/functions/quadratic.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/functions/rosenbrock.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/sqpgs/README.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/sqpgs/__init__.py
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/sqpgs/cvxpy_subproblem.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/sqpgs/defaults.py
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/sqpgs/main.py
--rw-r--r--   0        0        0     8929 2020-02-02 00:00:00.000000 ncopt-0.0.1/src/ncopt/sqpgs/osqp_subproblem.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 ncopt-0.0.1/tests/test_functions.py
--rw-r--r--   0        0        0     6156 2020-02-02 00:00:00.000000 ncopt-0.0.1/tests/test_jacobians.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 ncopt-0.0.1/tests/test_quadratic.py
--rwxr-xr-x   0        0        0     1557 2020-02-02 00:00:00.000000 ncopt-0.0.1/tests/test_rosenbrock.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 ncopt-0.0.1/tests/test_subproblem.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 ncopt-0.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 ncopt-0.0.1/LICENSE
--rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 ncopt-0.0.1/README.md
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 ncopt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 ncopt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ncopt-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 ncopt-0.2.0/CITATION.cff
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 ncopt-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ncopt-0.2.0/data/checkpoints/README.md
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 ncopt-0.2.0/data/checkpoints/max2d.pt
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ncopt-0.2.0/data/img/README.md
+-rw-r--r--   0        0        0    18147 2020-02-02 00:00:00.000000 ncopt-0.2.0/data/img/checkpoint.png
+-rw-r--r--   0        0        0    84858 2020-02-02 00:00:00.000000 ncopt-0.2.0/data/img/rosenbrock.png
+-rw-r--r--   0        0        0   111582 2020-02-02 00:00:00.000000 ncopt-0.2.0/data/img/timings_residual.png
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 ncopt-0.2.0/examples/example_checkpoint.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 ncopt-0.2.0/examples/example_residual.py
+-rwxr-xr-x   0        0        0     2839 2020-02-02 00:00:00.000000 ncopt-0.2.0/examples/example_rosenbrock.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 ncopt-0.2.0/scripts/timing_rosenbrock.py
+-rwxr-xr-x   0        0        0     3275 2020-02-02 00:00:00.000000 ncopt-0.2.0/scripts/train_max_fun.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/__about__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/__init__.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/plot_utils.py
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/utils.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/functions/__init__.py
+-rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/functions/main.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/functions/max_linear.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/functions/norm_residual.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/functions/quadratic.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/functions/rosenbrock.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/sqpgs/README.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/sqpgs/__init__.py
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/sqpgs/cvxpy_subproblem.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/sqpgs/defaults.py
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/sqpgs/main.py
+-rw-r--r--   0        0        0     8929 2020-02-02 00:00:00.000000 ncopt-0.2.0/src/ncopt/sqpgs/osqp_subproblem.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 ncopt-0.2.0/tests/test_functions.py
+-rw-r--r--   0        0        0     6156 2020-02-02 00:00:00.000000 ncopt-0.2.0/tests/test_jacobians.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 ncopt-0.2.0/tests/test_quadratic.py
+-rwxr-xr-x   0        0        0     1557 2020-02-02 00:00:00.000000 ncopt-0.2.0/tests/test_rosenbrock.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 ncopt-0.2.0/tests/test_subproblem.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 ncopt-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 ncopt-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 ncopt-0.2.0/README.md
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 ncopt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 ncopt-0.2.0/PKG-INFO
```

### Comparing `ncopt-0.0.1/.github/workflows/build.yml` & `ncopt-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/data/checkpoints/max2d.pt` & `ncopt-0.2.0/data/checkpoints/max2d.pt`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/data/img/checkpoint.png` & `ncopt-0.2.0/data/img/checkpoint.png`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/data/img/rosenbrock.png` & `ncopt-0.2.0/data/img/rosenbrock.png`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/data/img/timings_residual.png` & `ncopt-0.2.0/data/img/timings_residual.png`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/examples/example_checkpoint.py` & `ncopt-0.2.0/examples/example_checkpoint.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/examples/example_residual.py` & `ncopt-0.2.0/examples/example_residual.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/examples/example_rosenbrock.py` & `ncopt-0.2.0/examples/example_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/scripts/timing_rosenbrock.py` & `ncopt-0.2.0/scripts/timing_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/scripts/train_max_fun.py` & `ncopt-0.2.0/scripts/train_max_fun.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/plot_utils.py` & `ncopt-0.2.0/src/ncopt/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/utils.py` & `ncopt-0.2.0/src/ncopt/utils.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/functions/main.py` & `ncopt-0.2.0/src/ncopt/functions/main.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/functions/max_linear.py` & `ncopt-0.2.0/src/ncopt/functions/max_linear.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/functions/norm_residual.py` & `ncopt-0.2.0/src/ncopt/functions/norm_residual.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/functions/quadratic.py` & `ncopt-0.2.0/src/ncopt/functions/quadratic.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/functions/rosenbrock.py` & `ncopt-0.2.0/src/ncopt/functions/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/sqpgs/README.md` & `ncopt-0.2.0/src/ncopt/sqpgs/README.md`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/sqpgs/cvxpy_subproblem.py` & `ncopt-0.2.0/src/ncopt/sqpgs/cvxpy_subproblem.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/sqpgs/defaults.py` & `ncopt-0.2.0/src/ncopt/sqpgs/defaults.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/sqpgs/main.py` & `ncopt-0.2.0/src/ncopt/sqpgs/main.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/src/ncopt/sqpgs/osqp_subproblem.py` & `ncopt-0.2.0/src/ncopt/sqpgs/osqp_subproblem.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/tests/test_functions.py` & `ncopt-0.2.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/tests/test_jacobians.py` & `ncopt-0.2.0/tests/test_jacobians.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/tests/test_quadratic.py` & `ncopt-0.2.0/tests/test_quadratic.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/tests/test_rosenbrock.py` & `ncopt-0.2.0/tests/test_rosenbrock.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/tests/test_subproblem.py` & `ncopt-0.2.0/tests/test_subproblem.py`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/.gitignore` & `ncopt-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/LICENSE` & `ncopt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/README.md` & `ncopt-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/pyproject.toml` & `ncopt-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ncopt-0.0.1/PKG-INFO` & `ncopt-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ncopt
-Version: 0.0.1
+Version: 0.2.0
 Summary: Constrained optimization for Pytorch using the SQP-GS algorithm.
 Project-URL: Documentation, https://github.com/fabian-sp/ncOPT#readme
 Project-URL: Issues, https://github.com/fabian-sp/ncOPT/issues
 Project-URL: Source, https://github.com/fabian-sp/ncOPT
 Author: Philipp Schiele
 Author-email: Fabian Schaipp <fabian.schaipp@tum.de>
 License-Expression: BSD-3-Clause
```

