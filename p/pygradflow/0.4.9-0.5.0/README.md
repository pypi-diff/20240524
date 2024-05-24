# Comparing `tmp/pygradflow-0.4.9.tar.gz` & `tmp/pygradflow-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygradflow-0.4.9.tar", max compression
+gzip compressed data, was "pygradflow-0.5.0.tar", max compression
```

## Comparing `pygradflow-0.4.9.tar` & `pygradflow-0.5.0.tar`

### file list

```diff
@@ -1,44 +1,54 @@
--rw-r--r--   0        0        0    10847 2024-05-09 19:37:37.084144 pygradflow-0.4.9/LICENSE
--rw-r--r--   0        0        0      984 2024-05-09 19:37:37.084144 pygradflow-0.4.9/README.md
--rw-r--r--   0        0        0        0 2024-05-09 19:37:37.084144 pygradflow-0.4.9/pygradflow/__init__.py
--rw-r--r--   0        0        0      872 2024-05-09 19:37:37.084144 pygradflow-0.4.9/pygradflow/active_set.py
--rw-r--r--   0        0        0     4458 2024-05-09 19:37:37.084144 pygradflow-0.4.9/pygradflow/cons_problem.py
--rw-r--r--   0        0        0     1749 2024-05-09 19:37:37.084144 pygradflow-0.4.9/pygradflow/controller.py
--rw-r--r--   0        0        0     2487 2024-05-09 19:37:37.084144 pygradflow-0.4.9/pygradflow/deriv_check.py
--rw-r--r--   0        0        0     4645 2024-05-09 19:37:37.084144 pygradflow-0.4.9/pygradflow/display.py
--rw-r--r--   0        0        0     4839 2024-05-09 19:37:37.084144 pygradflow-0.4.9/pygradflow/eval.py
--rw-r--r--   0        0        0     6380 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/implicit_func.py
--rw-r--r--   0        0        0     5390 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/iterate.py
--rw-r--r--   0        0        0       55 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/log.py
--rw-r--r--   0        0        0     6570 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/newton.py
--rw-r--r--   0        0        0     5559 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/params.py
--rw-r--r--   0        0        0     5111 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/penalty.py
--rw-r--r--   0        0        0     5845 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/problem.py
--rw-r--r--   0        0        0        0 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/py.typed
--rw-r--r--   0        0        0     3378 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/runners/cutest_runner.py
--rw-r--r--   0        0        0      366 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/runners/instance.py
--rw-r--r--   0        0        0     2045 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/runners/qplib_runner.py
--rw-r--r--   0        0        0     8326 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/runners/runner.py
--rw-r--r--   0        0        0     5188 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/scale.py
--rw-r--r--   0        0        0    17435 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/solver.py
--rw-r--r--   0        0        0     1284 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/__init__.py
--rw-r--r--   0        0        0     4439 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/asymmetric_step_solver.py
--rw-r--r--   0        0        0     5877 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/box_control.py
--rw-r--r--   0        0        0     2710 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/cond_estimate.py
--rw-r--r--   0        0        0     2431 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/distance_ratio_control.py
--rw-r--r--   0        0        0     2058 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/exact_control.py
--rw-r--r--   0        0        0     3173 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/extended_step_solver.py
--rw-r--r--   0        0        0      543 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/fixed_control.py
--rw-r--r--   0        0        0     2669 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/linear_solver.py
--rw-r--r--   0        0        0     7537 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/opti_control.py
--rw-r--r--   0        0        0     2014 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/residuum_ratio_control.py
--rw-r--r--   0        0        0     2401 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/scaled_step_solver.py
--rw-r--r--   0        0        0     2467 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/standard_step_solver.py
--rw-r--r--   0        0        0     4697 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/step_control.py
--rw-r--r--   0        0        0     2048 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/step_solver.py
--rw-r--r--   0        0        0     4120 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/step/symmetric_step_solver.py
--rw-r--r--   0        0        0      380 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/timer.py
--rw-r--r--   0        0        0     1711 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/transform.py
--rw-r--r--   0        0        0      232 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pygradflow/util.py
--rw-r--r--   0        0        0     1138 2024-05-09 19:37:37.088144 pygradflow-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0    10847 2024-05-24 09:15:03.282932 pygradflow-0.5.0/LICENSE
+-rw-r--r--   0        0        0      984 2024-05-24 09:15:03.282932 pygradflow-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 09:15:03.282932 pygradflow-0.5.0/pygradflow/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-24 09:15:03.282932 pygradflow-0.5.0/pygradflow/active_set.py
+-rw-r--r--   0        0        0     1016 2024-05-24 09:15:03.282932 pygradflow-0.5.0/pygradflow/callbacks.py
+-rw-r--r--   0        0        0     4458 2024-05-24 09:15:03.282932 pygradflow-0.5.0/pygradflow/cons_problem.py
+-rw-r--r--   0        0        0     1749 2024-05-24 09:15:03.282932 pygradflow-0.5.0/pygradflow/controller.py
+-rw-r--r--   0        0        0     2431 2024-05-24 09:15:03.282932 pygradflow-0.5.0/pygradflow/deriv_check.py
+-rw-r--r--   0        0        0     9840 2024-05-24 09:15:03.282932 pygradflow-0.5.0/pygradflow/display.py
+-rw-r--r--   0        0        0     6359 2024-05-24 09:15:03.282932 pygradflow-0.5.0/pygradflow/eval.py
+-rw-r--r--   0        0        0     7472 2024-05-24 09:15:03.282932 pygradflow-0.5.0/pygradflow/implicit_func.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:15:03.282932 pygradflow-0.5.0/pygradflow/integration/__init__.py
+-rw-r--r--   0        0        0     1173 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/integration/events.py
+-rw-r--r--   0        0        0     3634 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/integration/flow.py
+-rw-r--r--   0        0        0    16999 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/integration/integration_solver.py
+-rw-r--r--   0        0        0     4330 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/integration/problem_switches.py
+-rw-r--r--   0        0        0     3458 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/integration/restricted_flow.py
+-rw-r--r--   0        0        0     5865 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/iterate.py
+-rw-r--r--   0        0        0       55 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/log.py
+-rw-r--r--   0        0        0     9309 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/newton.py
+-rw-r--r--   0        0        0     6017 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/params.py
+-rw-r--r--   0        0        0     5111 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/penalty.py
+-rw-r--r--   0        0        0     5845 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/problem.py
+-rw-r--r--   0        0        0        0 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/py.typed
+-rw-r--r--   0        0        0     1872 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/result.py
+-rw-r--r--   0        0        0     5157 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/runners/cutest_runner.py
+-rw-r--r--   0        0        0      521 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/runners/instance.py
+-rw-r--r--   0        0        0     2151 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/runners/qplib_runner.py
+-rw-r--r--   0        0        0     8600 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/runners/runner.py
+-rw-r--r--   0        0        0     7406 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/scale.py
+-rw-r--r--   0        0        0    12377 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/solver.py
+-rw-r--r--   0        0        0     1738 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/status.py
+-rw-r--r--   0        0        0     1284 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/step/__init__.py
+-rw-r--r--   0        0        0     4274 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/step/asymmetric_step_solver.py
+-rw-r--r--   0        0        0     7831 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/step/box_control.py
+-rw-r--r--   0        0        0     3416 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/step/box_solver.py
+-rw-r--r--   0        0        0     2710 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/step/cond_estimate.py
+-rw-r--r--   0        0        0     2431 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/step/distance_ratio_control.py
+-rw-r--r--   0        0        0     2058 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/step/exact_control.py
+-rw-r--r--   0        0        0     3101 2024-05-24 09:15:03.286932 pygradflow-0.5.0/pygradflow/step/extended_step_solver.py
+-rw-r--r--   0        0        0      543 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/step/fixed_control.py
+-rw-r--r--   0        0        0     2669 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/step/linear_solver.py
+-rw-r--r--   0        0        0     7326 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/step/opti_control.py
+-rw-r--r--   0        0        0     2014 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/step/residuum_ratio_control.py
+-rw-r--r--   0        0        0     2691 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/step/scaled_step_solver.py
+-rw-r--r--   0        0        0     2476 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/step/standard_step_solver.py
+-rw-r--r--   0        0        0     4713 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/step/step_control.py
+-rw-r--r--   0        0        0     2917 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/step/step_solver.py
+-rw-r--r--   0        0        0     4024 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/step/symmetric_step_solver.py
+-rw-r--r--   0        0        0      492 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/timer.py
+-rw-r--r--   0        0        0     3009 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/transform.py
+-rw-r--r--   0        0        0      846 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pygradflow/util.py
+-rw-r--r--   0        0        0     1158 2024-05-24 09:15:03.290932 pygradflow-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 pygradflow-0.5.0/PKG-INFO
```

### Comparing `pygradflow-0.4.9/LICENSE` & `pygradflow-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/README.md` & `pygradflow-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/active_set.py` & `pygradflow-0.5.0/pygradflow/active_set.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/cons_problem.py` & `pygradflow-0.5.0/pygradflow/cons_problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/controller.py` & `pygradflow-0.5.0/pygradflow/controller.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/deriv_check.py` & `pygradflow-0.5.0/pygradflow/deriv_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         self.invalid_deriv = np.logical_not(self.invalid_deriv)
         self.invalid_indices = np.where(self.invalid_deriv)[0]
 
         self.deriv_diffs = np.abs(self.expected_value - self.actual_value)
         self.max_deriv_diff = self.deriv_diffs.max()
 
         (num_rows, _) = self.deriv_diffs.shape
-        num_invalid_indices = self.invalid_indices.size
         self.col_index = col_index
 
     def __str__(self):
         num_invalid_indices = self.invalid_indices.shape[0]
 
         message = (
             f"Expected and actual (findiff) derivative "
```

### Comparing `pygradflow-0.4.9/pygradflow/eval.py` & `pygradflow-0.5.0/pygradflow/eval.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import math
+from enum import Enum, auto
 
 import numpy as np
 import scipy as sp
 
 from pygradflow.log import logger
 
 
@@ -31,118 +32,159 @@
     return warn
 
 
 warn_hessian_pattern = warn_once("Unsymmetric Hessian pattern")
 warn_hessian_values = warn_once("Hessian not numerically symmetric")
 
 
+class Component(Enum):
+    Obj = auto()
+    ObjGrad = auto()
+    Cons = auto()
+    ConsJac = auto()
+    LagHess = auto()
+
+    def name(self):
+        return {
+            Component.Obj: "Objective",
+            Component.ObjGrad: "Objective Gradient",
+            Component.Cons: "Constraints",
+            Component.ConsJac: "Constraint Jacobian",
+            Component.LagHess: "Lagrangian Hessian",
+        }[self]
+
+
 class Evaluator(abc.ABC):
-    @abc.abstractmethod
+    def __init__(self, problem, params):
+        self.problem = problem
+        self.dtype = params.dtype
+
+        self.reset_num_evals()
+
+    def reset_num_evals(self):
+        self.num_evals = {comp: 0 for comp in Component}
+
     def obj(self, x: np.ndarray) -> float:
+        self.num_evals[Component.Obj] += 1
+        return self._eval_obj(x)
+
+    def obj_grad(self, x: np.ndarray) -> np.ndarray:
+        self.num_evals[Component.ObjGrad] += 1
+        return self._eval_obj_grad(x)
+
+    def cons(self, x: np.ndarray) -> np.ndarray:
+        self.num_evals[Component.Cons] += 1
+        return self._eval_cons(x)
+
+    def cons_jac(self, x: np.ndarray) -> sp.sparse.spmatrix:
+        self.num_evals[Component.ConsJac] += 1
+        return self._eval_cons_jac(x)
+
+    def lag_hess(self, x: np.ndarray, lag: np.ndarray) -> sp.sparse.spmatrix:
+        self.num_evals[Component.LagHess] += 1
+        return self._eval_lag_hess(x, lag)
+
+    @abc.abstractmethod
+    def _eval_obj(self, x: np.ndarray) -> float:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def obj_grad(self, x: np.ndarray) -> np.ndarray:
+    def _eval_obj_grad(self, x: np.ndarray) -> np.ndarray:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def cons(self, x: np.ndarray) -> np.ndarray:
+    def _eval_cons(self, x: np.ndarray) -> np.ndarray:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def cons_jac(self, x: np.ndarray) -> sp.sparse.spmatrix:
+    def _eval_cons_jac(self, x: np.ndarray) -> sp.sparse.spmatrix:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def lag_hess(self, x: np.ndarray, lag: np.ndarray) -> sp.sparse.spmatrix:
+    def _eval_lag_hess(self, x: np.ndarray, lag: np.ndarray) -> sp.sparse.spmatrix:
         raise NotImplementedError()
 
 
 class SimpleEvaluator(Evaluator):
-    def __init__(self, problem, params):
-        self.problem = problem
-        self.dtype = params.dtype
-
-    def obj(self, x: np.ndarray) -> float:
+    def _eval_obj(self, x: np.ndarray) -> float:
         return self.problem.obj(x)
 
-    def obj_grad(self, x: np.ndarray) -> np.ndarray:
+    def _eval_obj_grad(self, x: np.ndarray) -> np.ndarray:
         return astype(self.problem.obj_grad(x), self.dtype)
 
-    def cons(self, x: np.ndarray) -> np.ndarray:
+    def _eval_cons(self, x: np.ndarray) -> np.ndarray:
         if self.problem.num_cons == 0:
             return np.array([], dtype=self.dtype)
 
         return astype(self.problem.cons(x), self.dtype)
 
-    def cons_jac(self, x: np.ndarray) -> sp.sparse.spmatrix:
+    def _eval_cons_jac(self, x: np.ndarray) -> sp.sparse.spmatrix:
         if self.problem.num_cons == 0:
             return sp.sparse.csr_matrix((0, self.problem.num_vars), dtype=self.dtype)
 
         return astype(self.problem.cons_jac(x), self.dtype)
 
-    def lag_hess(self, x: np.ndarray, lag: np.ndarray) -> sp.sparse.spmatrix:
+    def _eval_lag_hess(self, x: np.ndarray, lag: np.ndarray) -> sp.sparse.spmatrix:
         return astype(self.problem.lag_hess(x, lag), self.dtype)
 
 
 class ValidatingEvaluator(Evaluator):
     def __init__(self, problem, params):
-        self.problem = problem
-        self.dtype = params.dtype
+        super().__init__(problem, params)
         self.num_vars = problem.num_vars
         self.num_cons = problem.num_cons
 
-    def obj(self, x: np.ndarray) -> float:
+    def _eval_obj(self, x: np.ndarray) -> float:
         obj = self.problem.obj(x)
 
         if not math.isfinite(obj):
             raise EvalError("Infinite objective", x)
 
         return obj
 
-    def obj_grad(self, x: np.ndarray) -> np.ndarray:
+    def _eval_obj_grad(self, x: np.ndarray) -> np.ndarray:
         grad = self.problem.obj_grad(x)
 
         if grad.shape != (self.num_vars,):
             raise EvalError("Invalid shape of gradient", x)
 
         if not np.isfinite(grad).all():
             raise EvalError("Non-finite gradient", x)
 
         return astype(grad, self.dtype)
 
-    def cons(self, x: np.ndarray) -> np.ndarray:
+    def _eval_cons(self, x: np.ndarray) -> np.ndarray:
         if self.num_cons == 0:
             return np.array([], dtype=self.dtype)
 
         cons = self.problem.cons(x)
 
         if cons.shape != (self.num_cons,):
             raise EvalError("Invalid shape of constraints", x)
 
         if not np.isfinite(cons).all():
             raise EvalError("Non-finite constraints", x)
 
         return astype(cons, self.dtype)
 
-    def cons_jac(self, x: np.ndarray) -> sp.sparse.spmatrix:
+    def _eval_cons_jac(self, x: np.ndarray) -> sp.sparse.spmatrix:
         if self.num_cons == 0:
             return sp.sparse.csr_matrix((0, self.num_vars), dtype=self.dtype)
 
         cons_jac = self.problem.cons_jac(x)
 
         if cons_jac.shape != (self.num_cons, self.num_vars):
             raise EvalError("Invalid shape of Jacobian", x)
 
         if not np.isfinite(cons_jac.data).all():
             raise EvalError("Non-finite Jacobian", x)
 
         return astype(cons_jac, self.dtype)
 
-    def lag_hess(self, x: np.ndarray, lag: np.ndarray) -> sp.sparse.spmatrix:
+    def _eval_lag_hess(self, x: np.ndarray, lag: np.ndarray) -> sp.sparse.spmatrix:
         lag_hess = self.problem.lag_hess(x, lag)
 
         if lag_hess.shape != (self.num_vars, self.num_vars):
             raise EvalError("Invalid shape of Hessian", x)
 
         if not np.isfinite(lag_hess.data).all():
             raise EvalError("Non-finite Hessian", x)
@@ -163,7 +205,14 @@
         else:
             coo_data = coo_hess.data
             coo_T_data = coo_hess_T.data
             if not np.allclose(coo_data, coo_T_data):
                 warn_hessian_values()
 
         return astype(lag_hess, self.dtype)
+
+
+def create_evaluator(problem, params):
+    if params.validate_input:
+        return ValidatingEvaluator(problem, params)
+    else:
+        return SimpleEvaluator(problem, params)
```

### Comparing `pygradflow-0.4.9/pygradflow/implicit_func.py` & `pygradflow-0.5.0/pygradflow/implicit_func.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 from typing import Optional
 
 import numpy as np
 import scipy as sp
 
 from pygradflow.iterate import Iterate
 from pygradflow.problem import Problem
+from pygradflow.util import keep_rows
 
 
-class _Func(abc.ABC):
+class StepFunc(abc.ABC):
     def __init__(self, problem: Problem, iterate: Iterate, dt: float) -> None:
         self.problem = problem
         self.orig_iterate = iterate
         self.dt = dt
 
         self.n = problem.num_vars
         self.m = problem.num_cons
 
-    def compute_active_set(
-        self, x: np.ndarray, lb: np.ndarray, ub: np.ndarray
-    ) -> np.ndarray:
+    def compute_active_set_box(self, x: np.ndarray, lb: np.ndarray, ub: np.ndarray):
         """
         Compute the active set at the given point with respect to the
         given bounds.
 
         Parameters
         ----------
 
@@ -40,15 +39,15 @@
             outside the interval  :math:`[l_j, u_j]` and should be
             clipped to it during the projection.
         """
         assert (lb <= ub).all()
 
         return np.logical_or(x < lb - 1e-8, x > ub + 1e-8)
 
-    def project(
+    def project_box(
         self, x: np.ndarray, lb: np.ndarray, ub: np.ndarray, active_set: np.ndarray
     ) -> np.ndarray:
         assert active_set.dtype == bool
         assert active_set.shape == lb.shape
         assert (lb <= ub).all()
 
         p = np.copy(x)
@@ -62,36 +61,21 @@
 
     @abc.abstractmethod
     def value_at(
         self, iterate: Iterate, rho, active_set: Optional[np.ndarray] = None
     ) -> np.ndarray:
         raise NotImplementedError()
 
+    @abc.abstractmethod
+    def projection_initial(self, iterate: Iterate, rho: float) -> np.ndarray:
+        raise NotImplementedError()
 
-class ImplicitFunc(_Func):
-    def __init__(self, problem: Problem, iterate: Iterate, dt: float) -> None:
-        super().__init__(problem, iterate, dt)
-
-    def project(self, x: np.ndarray, active_set: np.ndarray):
-        problem = self.problem
-        lb = problem.var_lb
-        ub = problem.var_ub
-
-        return super().project(x, lb, ub, active_set)
-
-    def compute_active_set(self, x: np.ndarray):
-        problem = self.problem
-        lb = problem.var_lb
-        ub = problem.var_ub
-        return super().compute_active_set(x, lb, ub)
-
-    def projection_initial(self, iterate: Iterate, rho: float):
-        x_0 = self.orig_iterate.x
-        dt = self.dt
-        return x_0 - dt * iterate.aug_lag_deriv_x(rho)
+    @abc.abstractmethod
+    def compute_active_set(self, x: np.ndarray) -> np.ndarray:
+        raise NotImplementedError()
 
     def apply_project_deriv(self, mat: sp.sparse.spmatrix, active_set: np.ndarray):
         problem = self.problem
         lb = problem.var_lb
         ub = problem.var_ub
         (num_rows, _) = mat.shape
 
@@ -101,34 +85,41 @@
         assert (lb <= ub).all()
 
         assert (lb != np.inf).all()
         assert (ub != -np.inf).all()
 
         assert (num_rows,) == lb.shape
 
-        mat = mat.tocoo()
-
         inactive_set = np.logical_not(active_set)
-        inactive_indices = np.where(inactive_set)[0]
+        proj_mat = keep_rows(mat, inactive_set)
 
-        alive_indices = np.isin(mat.row, inactive_indices)
+        return proj_mat
 
-        assert inactive_set[mat.row[alive_indices]].all()
 
-        next_rows = mat.row[alive_indices]
-        next_cols = mat.col[alive_indices]
-        next_entries = mat.data[alive_indices]
+class ImplicitFunc(StepFunc):
+    def __init__(self, problem: Problem, iterate: Iterate, dt: float) -> None:
+        super().__init__(problem, iterate, dt)
 
-        proj_mat = sp.sparse.coo_matrix(
-            (next_entries, (next_rows, next_cols)), mat.shape
-        )
+    def project(self, x: np.ndarray, active_set: np.ndarray):
+        problem = self.problem
+        lb = problem.var_lb
+        ub = problem.var_ub
 
-        assert inactive_set[proj_mat.row].all()
+        return super().project_box(x, lb, ub, active_set)
 
-        return proj_mat
+    def compute_active_set(self, x: np.ndarray):
+        problem = self.problem
+        lb = problem.var_lb
+        ub = problem.var_ub
+        return super().compute_active_set_box(x, lb, ub)
+
+    def projection_initial(self, iterate: Iterate, rho: float):
+        x_0 = self.orig_iterate.x
+        dt = self.dt
+        return x_0 - dt * iterate.aug_lag_deriv_x(rho)
 
     # @override
     def value_at(self, iterate, rho, active_set=None):
         y_0 = self.orig_iterate.y
         dt = self.dt
 
         p = self.projection_initial(iterate, rho)
@@ -176,15 +167,15 @@
 
         hess = iterate.aug_lag_deriv_xx(rho)
         jac = iterate.aug_lag_deriv_xy()
 
         return self.deriv(jac, hess, active_set)
 
 
-class ScaledImplicitFunc(_Func):
+class ScaledImplicitFunc(StepFunc):
     def __init__(self, problem: Problem, iterate: Iterate, dt: float) -> None:
         super().__init__(problem, iterate, dt)
         self.lamb = 1.0 / dt
         params = iterate.params
         self.lb = (self.lamb * problem.var_lb).astype(params.dtype)
         self.ub = (self.lamb * problem.var_ub).astype(params.dtype)
 
@@ -206,11 +197,54 @@
     def projection_initial(self, iterate: Iterate, rho: float):
         x_0 = self.orig_iterate.x
         lamb = self.lamb
 
         return lamb * x_0 - iterate.aug_lag_deriv_x(rho)
 
     def project(self, x: np.ndarray, active_set: np.ndarray):
-        return super().project(x, self.lb, self.ub, active_set)
+        return super().project_box(x, self.lb, self.ub, active_set)
 
     def compute_active_set(self, x: np.ndarray):
-        return super().compute_active_set(x, self.lb, self.ub)
+        return super().compute_active_set_box(x, self.lb, self.ub)
+
+    def deriv(
+        self, jac: sp.sparse.spmatrix, hess: sp.sparse.spmatrix, active_set: np.ndarray
+    ):
+        n = self.n
+        m = self.m
+        dt = self.dt
+        lamb = 1.0 / dt
+
+        assert active_set is not None
+        params = self.orig_iterate.params
+
+        F_11 = sp.sparse.diags([lamb], shape=(n, n), dtype=params.dtype)
+
+        F_11 = lamb * sp.sparse.eye(n, dtype=params.dtype)
+        F_11 += self.apply_project_deriv(hess, active_set)
+
+        F_12 = self.apply_project_deriv(jac.T, active_set)
+
+        assert F_11.dtype == params.dtype
+        assert F_12.dtype == params.dtype
+
+        F_21 = -jac
+
+        F_22 = sp.sparse.diags([lamb], shape=(m, m), dtype=params.dtype)
+
+        deriv = sp.sparse.bmat([[F_11, F_12], [F_21, F_22]], format="csc")
+
+        assert deriv.dtype == params.dtype
+
+        return deriv
+
+    def deriv_at(
+        self, iterate: Iterate, rho: float, active_set: Optional[np.ndarray] = None
+    ):
+        if active_set is None:
+            p = self.projection_initial(iterate, rho)
+            active_set = self.compute_active_set(p)
+
+        hess = iterate.aug_lag_deriv_xx(rho)
+        jac = iterate.aug_lag_deriv_xy()
+
+        return self.deriv(jac, hess, active_set)
```

### Comparing `pygradflow-0.4.9/pygradflow/iterate.py` & `pygradflow-0.5.0/pygradflow/iterate.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,18 @@
 
         if eval:
             self.eval = eval
         else:
             self.eval = SimpleEvaluator(problem, params)
         self.problem = problem
 
+    @property
+    def z(self):
+        return np.concatenate((self.x, self.y))
+
     def copy(self) -> "Iterate":
         return Iterate(
             self.problem, self.params, np.copy(self.x), np.copy(self.y), self.eval
         )
 
     def clipped(self) -> "Iterate":
         var_lb = self.problem.var_lb
@@ -64,16 +68,16 @@
     def cons(self) -> np.ndarray:
         return _read_only(self.eval.cons(self.x))
 
     @functools.cached_property
     def cons_jac(self) -> sp.sparse.spmatrix:
         return self.eval.cons_jac(self.x)
 
-    def lag_hess(self, lag: np.ndarray) -> sp.sparse.spmatrix:
-        return self.eval.lag_hess(self.x, lag)
+    def lag_hess(self, y: np.ndarray) -> sp.sparse.spmatrix:
+        return self.eval.lag_hess(self.x, y)
 
     def aug_lag_violation(self, rho: float) -> float:
         cv = self.cons
         return rho / 2.0 * np.dot(cv, cv)
 
     def aug_lag_dual(self) -> float:
         cv = self.cons
@@ -171,7 +175,17 @@
 
     def is_feasible(self, tol):
         return (self.cons_violation <= tol) and (self.bound_violation <= tol)
 
     @property
     def total_res(self) -> float:
         return max(self.cons_violation, self.bound_violation, self.stat_res)
+
+    def obj_nonlin(self, other: "Iterate") -> float:
+        dx = other.x - self.x
+        next_obj = self.obj + np.dot(dx, self.obj_grad)
+        return abs(other.obj - next_obj) / np.dot(dx, dx)
+
+    def cons_nonlin(self, other: "Iterate") -> np.ndarray:
+        dx = other.x - self.x
+        next_cons = self.cons + self.cons_jac.dot(dx)
+        return (other.cons - next_cons) / np.dot(dx, dx)
```

### Comparing `pygradflow-0.4.9/pygradflow/newton.py` & `pygradflow-0.5.0/pygradflow/newton.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import abc
 
 import numpy as np
 import scipy as sp
 
-from pygradflow.implicit_func import ImplicitFunc
 from pygradflow.iterate import Iterate
 from pygradflow.log import logger as lgg
 from pygradflow.params import NewtonType, Params
 from pygradflow.problem import Problem
 from pygradflow.step import step_solver
 from pygradflow.step.step_solver import StepResult, StepSolver
 
@@ -18,15 +17,14 @@
     def __init__(
         self, problem: Problem, orig_iterate: Iterate, dt: float, rho: float
     ) -> None:
         self.problem = problem
         self.orig_iterate = orig_iterate
         self.dt = dt
         self.rho = rho
-        self.func = ImplicitFunc(problem, orig_iterate, dt)
 
     @property
     def params(self) -> Params:
         return self.orig_iterate.params
 
     @abc.abstractmethod
     def step(self, iterate: Iterate) -> StepResult:
@@ -44,14 +42,15 @@
         problem: Problem,
         orig_iterate: Iterate,
         dt: float,
         rho: float,
         step_solver: StepSolver,
     ) -> None:
         super().__init__(problem, orig_iterate, dt, rho)
+        self.func = step_solver.func
 
         self.step_solver = step_solver
         p = self.func.projection_initial(orig_iterate, rho)
         active_set = self.func.compute_active_set(p)
 
         self.step_solver.update_active_set(active_set)
         self.step_solver.update_derivs(orig_iterate)
@@ -72,14 +71,15 @@
         problem: Problem,
         orig_iterate: Iterate,
         dt: float,
         rho: float,
         step_solver: StepSolver,
     ) -> None:
         super().__init__(problem, orig_iterate, dt, rho)
+        self.func = step_solver.func
         self.step_solver = step_solver
 
     def step(self, iterate: Iterate) -> StepResult:
         p = self.func.projection_initial(iterate, self.rho)
         active_set = self.func.compute_active_set(p)
 
         self.step_solver.update_active_set(active_set)
@@ -93,14 +93,15 @@
     Computes step based on the matrix given in terms of the *current*
     iterate. Requires evaluation of the derivative and a factorization
     at each step.
     """
 
     def __init__(self, problem, active_set, orig_iterate, dt, rho):
         super().__init__(problem, orig_iterate, dt, rho)
+        self.func = step_solver.func
 
         assert active_set.dtype == bool
         assert active_set.shape == problem.var_lb.shape
 
         self.active_set = active_set
 
         logger.info(
@@ -120,15 +121,15 @@
         xn, yn = self.split_sol(s)
         x = iterate.x
         y = iterate.y
 
         dx = x - xn
         dy = y - yn
 
-        return StepResult(iterate, dx, dy)
+        return StepResult(iterate, dx, dy, active_set=self.active_set)
 
     @staticmethod
     def active_set_from_iterate(problem, iterate):
         lb = problem.var_lb
         ub = problem.var_ub
 
         x = iterate.x
@@ -189,34 +190,121 @@
         problem: Problem,
         orig_iterate: Iterate,
         dt: float,
         rho: float,
         step_solver: StepSolver,
     ) -> None:
         super().__init__(problem, orig_iterate, dt, rho)
+        self.func = step_solver.func
 
         self.step_solver = step_solver
         self.step_solver.update_derivs(orig_iterate)
 
     def step(self, iterate):
         p = self.func.projection_initial(iterate, self.rho)
         active_set = self.func.compute_active_set(p)
 
         self.step_solver.update_active_set(active_set)
 
         return self.step_solver.solve(iterate)
 
 
+class GlobalizedNewtonMethod(NewtonMethod):
+    """
+    Globalized Newton method with Armijo line search. Globalization
+    is based on the underlying function of the step solver.
+    """
+
+    def __init__(
+        self,
+        problem: Problem,
+        orig_iterate: Iterate,
+        dt: float,
+        rho: float,
+        step_solver: StepSolver,
+    ) -> None:
+        super().__init__(problem, orig_iterate, dt, rho)
+        self.func = step_solver.func
+        self.step_solver = step_solver
+
+    def _set_iterate(self, iterate):
+        self.step_solver.update_derivs(iterate)
+        p = self.func.projection_initial(iterate, self.rho)
+        active_set = self.func.compute_active_set(p)
+        self.step_solver.update_active_set(active_set)
+
+    def step(self, iterate):
+        problem = self.problem
+        params = iterate.params
+
+        self._set_iterate(iterate)
+
+        step_result = self.step_solver.solve(self.orig_iterate)
+
+        # Armijo line search:
+        alpha = 1.0
+
+        func_value = self.func.value_at(iterate, self.rho)
+        res_value = 0.5 * np.dot(func_value, func_value)
+
+        # TODO: Create a method in the step function
+        # to compute a forward product instead to make
+        # everything more efficient
+        func_deriv = self.func.deriv_at(iterate, self.rho)
+        func_grad = func_deriv.T @ func_value
+
+        func_grad_x = func_grad[: problem.num_vars]
+        func_grad_y = func_grad[problem.num_vars :]
+
+        dx = step_result.dx
+        dy = step_result.dy
+
+        inner_product = np.dot(func_grad_x, dx) + np.dot(func_grad_y, dy)
+
+        max_it = 30
+
+        for it in range(max_it):
+            next_iterate = Iterate(
+                problem, params, iterate.x - dx, iterate.y - dy, iterate.eval
+            )
+
+            next_func_value = self.func.value_at(next_iterate, self.rho)
+            next_res_value = 0.5 * np.dot(next_func_value, next_func_value)
+
+            if np.isclose(next_res_value, 0.0):
+                break
+
+            if next_res_value <= res_value + (1e-4 * alpha * inner_product):
+                break
+
+            alpha *= 0.5
+            dx = alpha * step_result.dx
+            dy = alpha * step_result.dy
+
+        else:
+            raise Exception("Line search failed to converge")
+
+        logger.debug("Line search converged in %d iterations", it + 1)
+
+        next_x = iterate.x + dx
+        active_set = self.func.compute_active_set(next_x)
+
+        return StepResult(self.orig_iterate, dx, dy, active_set, rcond=None)
+
+
 def newton_method(
     problem: Problem, params: Params, iterate: Iterate, dt: float, rho: float
 ) -> NewtonMethod:
     assert dt > 0.0
     assert rho > 0.0
 
     solver = step_solver(problem, params, iterate, dt, rho)
 
     if params.newton_type == NewtonType.Simplified:
         return SimplifiedNewtonMethod(problem, iterate, dt, rho, solver)
     elif params.newton_type == NewtonType.Full:
         return FullNewtonMethod(problem, iterate, dt, rho, solver)
     elif params.newton_type == NewtonType.ActiveSet:
         return ActiveSetNewtonMethod(problem, iterate, dt, rho, solver)
+    else:
+        assert params.newton_type == NewtonType.Globalized
+        return GlobalizedNewtonMethod(problem, iterate, dt, rho, solver)
```

### Comparing `pygradflow-0.4.9/pygradflow/params.py` & `pygradflow-0.5.0/pygradflow/params.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import dataclasses
 import enum
+import typing
 from dataclasses import dataclass
 from enum import Enum, Flag, auto
-from typing import Optional
+from typing import Any, Callable, Optional
+
+if typing.TYPE_CHECKING:
+    from .scale import Scaling
 
 import numpy as np
 
 
 class NewtonType(Enum):
     """
     The Newton method to be used to solve the semi-smooth systems.
@@ -26,14 +30,19 @@
     """
     ActiveSet = auto()
     """
     Newton method with fixed derivative, but changing active sets.
     Requires refactorizations but no reevaluations of the derivatives
     """
 
+    Globalized = auto()
+    """
+    Globalizes the Newton method by using an Armijo line search
+    """
+
 
 class StepSolverType(Enum):
     """
     Step solver type to be used throughout computations
     """
 
     Standard = auto()
@@ -136,14 +145,24 @@
     """
 
     GradJac = auto()
     """
     Scale based on gradient and equilibration of constraint Jacobian
     """
 
+    KKT = auto()
+    """
+    Compute scales based on the equilibration of the KKT matrix
+    """
+
+    Nominal = auto()
+    """
+    Scaled based on values of the variable and constraint values
+    """
+
     Custom = auto()
     """
     User-provided custom scaling
     """
 
 
 @dataclass
@@ -175,39 +194,40 @@
     local_infeas_tol: float = 1e-8
 
     newton_type: NewtonType = NewtonType.Simplified
     newton_tol: float = 1e-8
 
     step_control_type: StepControlType = StepControlType.DistanceRatio
 
-    step_solver: object = None
+    step_solver: Optional[Callable[..., Any]] = None
     step_solver_type: StepSolverType = StepSolverType.Symmetric
     linear_solver_type: LinearSolverType = LinearSolverType.LU
     penalty_update: PenaltyUpdate = PenaltyUpdate.DualNorm
 
     deriv_check: DerivCheck = DerivCheck.NoCheck
     deriv_pert: float = 1e-8
     deriv_tol: float = 1e-4
 
     precision: Precision = Precision.Double
 
     scaling_type: ScalingType = ScalingType.NoScaling
-    scaling: object = None
+    scaling: Optional["Scaling"] = None
 
     validate_input: bool = True
 
     iteration_limit: Optional[int] = None
     time_limit: float = float(np.inf)
     display_interval: float = 0.1
 
     # lower bound on objective function value,
     # used to detect unbounded problems
     obj_lower_limit: float = -1e10
 
     report_rcond: bool = False
+    collect_path: bool = False
 
     def __post_init__(self):
         # Convert enum strings to enum values
         for key, attr in self.annotations():
             if isinstance(attr, enum.EnumMeta):
                 val = getattr(self, key)
                 if isinstance(val, str):
```

### Comparing `pygradflow-0.4.9/pygradflow/penalty.py` & `pygradflow-0.5.0/pygradflow/penalty.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/problem.py` & `pygradflow-0.5.0/pygradflow/problem.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/runners/cutest_runner.py` & `pygradflow-0.5.0/pygradflow/runners/cutest_runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import logging
+from functools import cached_property
 
 import numpy as np
 import pycutest
 
 from pygradflow.solver import Problem, Solver
 
 from .instance import Instance
 from .runner import Runner
 
 formatter = logging.Formatter("%(asctime)s:%(name)s:%(levelname)s:%(message)s")
 
 
+def cutest_is_ne_prob(name):
+    return name.endswith("NE")
+
+
 def cutest_map_inf(x):
     cutest_inf = 1e20
     y = np.copy(x)
     y[y == cutest_inf] = np.inf
     y[y == -cutest_inf] = -np.inf
     return y
 
 
 class UnconstrainedCUTEstProblem(Problem):
     def __init__(self, instance):
         self.instance = instance
         var_lb = cutest_map_inf(instance.bl)
         var_ub = cutest_map_inf(instance.bu)
-        super().__init__(var_lb, var_ub, num_cons=instance.m)
+        assert instance.m == 0
+        super().__init__(var_lb, var_ub, num_cons=0)
 
     def obj(self, x):
         return self.instance.obj(x)
 
     def obj_grad(self, x):
         obj, grad = self.instance.obj(x, gradient=True)
         return grad
@@ -83,51 +89,110 @@
         return self.instance.x0
 
     @property
     def y0(self):
         return self.instance.v0
 
 
+# Nonlinear equations: Goal is to minimize the violation
+# 1/2 ||c(x)||^2 subject to problem bounds. Constraint
+# functions are used to access the residuals and their derivatives
+class NECUTEstProblem(Problem):
+    def __init__(self, instance):
+        self.instance = instance
+        var_lb = cutest_map_inf(instance.bl)
+        var_ub = cutest_map_inf(instance.bu)
+
+        super().__init__(var_lb, var_ub, num_cons=0)
+
+    @cached_property
+    def problem(self):
+        return pycutest.import_problem(self.name, drop_fixed_variables=True)
+
+    def obj(self, x):
+        residuals = self.instance.cons(x)
+        return 0.5 * np.dot(residuals, residuals)
+
+    def obj_grad(self, x):
+        residuals, jac = self.instance.scons(x, gradient=True)
+        return jac.T.dot(residuals)
+
+    def lag_hess(self, x, y):
+        _, jac = self.instance.scons(x, gradient=True)
+        return jac.T.dot(jac)
+
+    @property
+    def x0(self):
+        return self.instance.x0
+
+    @property
+    def y0(self):
+        return np.zeros((self.num_cons,))
+
+
 class CUTestInstance(Instance):
     def __init__(self, instance):
         self.instance = instance
 
-        props = pycutest.problem_properties(instance)
+        props = pycutest.problem_properties(self.instance)
 
         num_vars = props["n"]
         num_cons = props["m"]
 
         if num_cons is None:
             num_cons = 0
 
         super().__init__(instance, num_vars, num_cons)
 
-    def solve(self, params):
-        problem = pycutest.import_problem(self.name, drop_fixed_variables=True)
+    def cutest_problem(self):
+        return pycutest.import_problem(self.name, drop_fixed_variables=True)
+
+    def x0(self):
+        cutest_problem = self.cutest_problem()
+        return cutest_problem.x0
 
-        if problem.m == 0:
-            problem = UnconstrainedCUTEstProblem(problem)
+    def problem(self):
+        cutest_problem = self.cutest_problem()
+
+        is_ne = cutest_is_ne_prob(self.name)
+
+        if is_ne:
+            return NECUTEstProblem(cutest_problem)
+        elif cutest_problem.m == 0:
+            return UnconstrainedCUTEstProblem(cutest_problem)
         else:
-            problem = ConstrainedCUTEstProblem(problem)
+            return ConstrainedCUTEstProblem(cutest_problem)
 
+    def solve(self, params):
+        problem = self.problem()
         solver = Solver(problem, params)
         return solver.solve(problem.x0, problem.y0)
 
 
 class CUTestRunner(Runner):
     def __init__(self):
         super().__init__(name="cutest")
 
+    def parser(self):
+        parser = super().parser()
+
+        parser.add_argument("--ignore_ne_probs", action="store_true")
+
+        return parser
+
     def get_instances(self, args):
         instances = pycutest.find_problems()
         filtered_instances = []
 
         for instance in instances:
             props = pycutest.problem_properties(instance)
 
+            if args.ignore_ne_probs and cutest_is_ne_prob(instance):
+                continue
+
             if props["m"] == "variable":
                 continue
 
             if props["n"] == "variable":
                 continue
 
             filtered_instances.append(CUTestInstance(instance))
```

### Comparing `pygradflow-0.4.9/pygradflow/runners/qplib_runner.py` & `pygradflow-0.5.0/pygradflow/runners/qplib_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,19 +50,25 @@
         super().__init__(description.name, description.num_vars, description.num_cons)
 
     @property
     def filename(self):
         return self.description.filename
 
     def solve(self, params):
-        qproblem = pyqplib.read_problem(self.filename)
-        problem = QPLIBProblem(qproblem)
+        problem = self.problem()
         solver = Solver(problem, params)
         return solver.solve(problem.x0, problem.y0)
 
+    def problem(self):
+        qproblem = pyqplib.read_problem(self.filename)
+        return QPLIBProblem(qproblem)
+
+    def x0(self):
+        return self.problem().x0
+
 
 class QPLIBRunner(Runner):
     def __init__(self):
         super().__init__(name="qplib")
 
     def get_instances(self, args):
         instances = []
```

### Comparing `pygradflow-0.4.9/pygradflow/runners/runner.py` & `pygradflow-0.5.0/pygradflow/runners/runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 import datetime
 import enum
 import itertools
 import logging
 import os
 from abc import ABC, abstractmethod
 from concurrent.futures import FIRST_COMPLETED, ProcessPoolExecutor, wait
-from multiprocessing import TimeoutError, cpu_count
-from multiprocessing.pool import ThreadPool
+from multiprocessing import cpu_count
 
 import numpy as np
 
 from pygradflow.log import logger
 from pygradflow.params import Params
 from pygradflow.solver import SolverStatus
 
 run_logger = logging.getLogger(__name__)
 
 formatter = logging.Formatter("%(asctime)s:%(name)s:%(levelname)s:%(message)s")
 
 
-def try_solve_instance(instance, params, log_filename, verbose):
-    try:
-        logger.handlers.clear()
+def solve_instance(instance, params, log_filename, verbose):
+    logger.handlers.clear()
+
+    np.seterr(divide="raise", over="raise", invalid="raise")
+
+    handler = logging.FileHandler(log_filename)
+    handler.setFormatter(formatter)
+    logger.addHandler(handler)
 
-        handler = logging.FileHandler(log_filename)
+    if verbose:
+        handler = logging.StreamHandler()
         handler.setFormatter(formatter)
         logger.addHandler(handler)
 
-        if verbose:
-            handler = logging.StreamHandler()
-            handler.setFormatter(formatter)
-            logger.addHandler(handler)
-
-        logger.setLevel(logging.INFO)
-
-        logging.captureWarnings(True)
-        warn_logger = logging.getLogger("py.warnings")
-        warn_logger.addHandler(handler)
-        warn_logger.setLevel(logging.WARN)
+    logger.setLevel(logging.INFO)
 
-        def solve():
-            return instance.solve(params)
+    logging.captureWarnings(True)
+    warn_logger = logging.getLogger("py.warnings")
+    warn_logger.addHandler(handler)
+    warn_logger.setLevel(logging.WARN)
 
+    return instance.solve(params)
+
+
+def try_solve_instance(instance, params, log_filename, verbose):
+    try:
         # No time limit
         if params.time_limit == np.inf:
-            return (instance, solve())
+            return (instance, solve_instance(instance, params, log_filename, verbose))
+
+        with ProcessPoolExecutor(1) as pool:
+            future = pool.submit(
+                solve_instance, instance, params, log_filename, verbose
+            )
+            done, _ = wait([future], timeout=(params.time_limit + 10))
+
+            if len(done) == 0:
+                logger.error("Reached timeout, aborting")
+                return (instance, "timeout")
 
-        # Solve in thread pool so we can
-        # await the result
-        thread_pool = ThreadPool(1)
-
-        try:
-            res = thread_pool.apply_async(solve)
-            result = res.get(params.time_limit)
+            result = next(iter(done)).result()
             return (instance, result)
-        except TimeoutError:
-            logger.error("Reached timeout, aborting")
-            return (instance, "timeout")
+
     except Exception as exc:
         logger.error("Error solving %s", instance.name)
         logger.exception(exc, exc_info=(type(exc), exc, exc.__traceback__))
         return (instance, "error")
 
 
 class Runner(ABC):
@@ -118,22 +122,18 @@
                 done, futures = wait(futures, return_when=FIRST_COMPLETED)
 
                 for item in done:
                     yield item.result()
 
     def solve_instances(self, instances, args):
         # yields sequence of tuples of (instance, result) for each instance
-        results = []
-
         run_logger.info("Solving %d instances", len(instances))
 
         params = self.create_params(args)
 
-        verbose = args.verbose
-
         if args.parallel is not None:
             yield from self.solve_instances_parallel(instances, args, params)
         else:
             yield from self.solve_instances_sequential(instances, args, params)
 
     def filter_instances(self, args):
         instances = []
@@ -141,32 +141,29 @@
         max_size = args.max_size
         name = args.name
 
         for instance in self.get_instances(args):
             if max_size is not None and instance.size > max_size:
                 continue
 
+            if args.unconstrained and instance.num_cons > 0:
+                continue
+
             if name is not None and name != instance.name:
                 continue
 
             instances.append(instance)
 
         return instances
 
     def parser(self):
         import argparse
 
         parser = argparse.ArgumentParser()
 
-        parser.add_argument("--output", type=str)
-        parser.add_argument("--max_size", type=int)
-        parser.add_argument("--name", type=str)
-        parser.add_argument("--verbose", action="store_true")
-        parser.add_argument("--parallel", nargs="?", type=int, const=True)
-
         group = parser.add_argument_group(title="parameters")
 
         default_params = Params()
 
         for key, attr in default_params.annotations():
             name = f"--{key}"
             if isinstance(attr, enum.EnumMeta):
@@ -180,14 +177,23 @@
                 group.add_argument(
                     name,
                     default=default_value,
                     type=attr,
                     help="Default: %(default)s",
                 )
 
+        group = parser.add_argument_group(title="runner")
+
+        parser.add_argument("--output", type=str)
+        parser.add_argument("--max_size", type=int)
+        parser.add_argument("--name", type=str)
+        parser.add_argument("--unconstrained", action="store_true")
+        parser.add_argument("--verbose", action="store_true")
+        parser.add_argument("--parallel", nargs="?", type=int, const=True)
+
         return parser
 
     def output_filename(self, args, filename):
         return os.path.join(args.output, filename)
 
     def main(self):
         run_logger.setLevel(logging.INFO)
```

### Comparing `pygradflow-0.4.9/pygradflow/solver.py` & `pygradflow-0.5.0/pygradflow/integration/integration_solver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,582 +1,519 @@
-import time
 from enum import Enum, auto
-from typing import Optional, cast
+from typing import List, Optional, cast
 
 import numpy as np
+import scipy as sp
 
-from pygradflow.display import Format, problem_display
-from pygradflow.eval import Evaluator, SimpleEvaluator, ValidatingEvaluator
+from pygradflow.display import (
+    Format,
+    StateData,
+    integrator_display,
+    print_problem_stats,
+)
+from pygradflow.integration.events import (
+    ConvergedResult,
+    EventResultType,
+    FilterChangedResult,
+    PenaltyResult,
+    UnboundedResult,
+)
+from pygradflow.integration.flow import Flow, func_neg, func_pos, lazy_func
+from pygradflow.integration.problem_switches import SwitchTrigger, TriggerType
+from pygradflow.integration.restricted_flow import RestrictedFlow
 from pygradflow.iterate import Iterate
 from pygradflow.log import logger
-from pygradflow.newton import newton_method
-from pygradflow.params import Params, ScalingType
-from pygradflow.penalty import penalty_strategy
-from pygradflow.problem import Problem
-from pygradflow.scale import Scaling
-from pygradflow.step.step_control import (
-    StepController,
-    StepControlResult,
-    step_controller,
-)
+from pygradflow.params import Params
+from pygradflow.result import SolverResult
+from pygradflow.status import SolverStatus
 from pygradflow.timer import Timer
 from pygradflow.transform import Transformation
 
 
-class SolverStatus(Enum):
-    Optimal = auto()
-    """
-    The algorithm has converged to a solution satisfying
-    the optimality conditions according to given tolerances
-    """
-
-    IterationLimit = auto()
-    """
-    Reached the iteration limit precribed by the algorithmic
-    parameters
-    """
-
-    TimeLimit = auto()
-    """
-    Reached the time limit precribed by the algorithmic
-    parameters
-    """
-
+class IntegrationStatus(Enum):
+    Converged = auto()
     Unbounded = auto()
-    """
-    Problem appearst unbounded (found feasible point with extremely
-    small objective value)
-    """
-
-    LocallyInfeasible = auto()
-    """
-    Local infeasibility detected (found infeasible point being
-    a local minimum with respect to constraint violation)
-    """
+    Event = auto()
+    Finished = auto()
+    Penalty = auto()
 
-    @staticmethod
-    def short_name(status):
+    def name(self):
         return {
-            SolverStatus.Optimal: "optimal",
-            SolverStatus.IterationLimit: "iteration_limit",
-            SolverStatus.TimeLimit: "time_limit",
-            SolverStatus.Unbounded: "unbounded",
-            SolverStatus.LocallyInfeasible: "infeasible",
-        }[status]
+            IntegrationStatus.Converged: "Converged",
+            IntegrationStatus.Unbounded: "Unbounded",
+            IntegrationStatus.Event: "Event",
+            IntegrationStatus.Finished: "Finished",
+            IntegrationStatus.Penalty: "Penalty",
+        }[self]
 
-    @staticmethod
-    def description(status):
-        return {
-            SolverStatus.Optimal: "Converged to first-order optimal solution",
-            SolverStatus.IterationLimit: "Reached iteration limit",
-            SolverStatus.TimeLimit: "Reached time limit",
-            SolverStatus.Unbounded: "Problem appears unbounded",
-            SolverStatus.LocallyInfeasible: "Local infeasibility detected",
-        }[status]
-
-    @staticmethod
-    def success(status):
-        """
-        Returns
-        -------
-        bool
-            Whether the status indicates a successful solve
-        """
-        return status == SolverStatus.Optimal
-
-
-class SolverResult:
-    """
-    The result of a solution of a :py:class:`pygradflow.problem.Problem`
-    instance with a :py:class:`pygradflow.solver.Solver`
-    """
 
+class IntegrationResult:
     def __init__(
         self,
-        x: np.ndarray,
-        y: np.ndarray,
-        d: np.ndarray,
-        status: SolverStatus,
-        iterations: int,
-        num_accepted_steps: int,
-        total_time: float,
-        dist_factor: float,
+        status,
+        dist,
+        t_next,
+        z_next,
+        filter_next,
+        num_steps,
+        num_func_evals,
+        num_jac_evals,
     ):
-        self._x = x
-        self._y = y
-        self._d = d
-        self._status = status
-        self.iterations = iterations
-        self.num_accepted_steps = num_accepted_steps
-        self.total_time = total_time
-        self.dist_factor = dist_factor
-
-    @property
-    def status(self) -> SolverStatus:
-        """
-        The status of the solve as a :py:class:`pygradflow.solver.SolverStatus`
-        """
-        return self._status
-
-    @property
-    def x(self) -> np.ndarray:
-        """
-        The primal solution :math:`x \\in \\mathbb{R}^{n}`
-        """
-        return self._x
-
-    @property
-    def y(self) -> np.ndarray:
-        """
-        The dual solution :math:`y \\in \\mathbb{R}^{m}`
-        """
-        return self._y
-
-    @property
-    def d(self) -> np.ndarray:
-        """
-        The dual solution :math:`d \\in \\mathbb{R}^{n}`
-        with respect to the variable bounds
-        """
-        return self._d
-
-    def __repr__(self) -> str:
-        return "SolverResult(status={0})".format(self.status)
-
-    @property
-    def success(self):
-        return SolverStatus.success(self.status)
-
-
-header_interval = 25
-
-
-class Solver:
-    """
-    Solves a :py:class:`pygradflow.problem.Problem` instance according
-    to the given :py:class:`pygradflow.params.Params`.
-    The solver attempts to find a solution given by
-    vectors :math:`x \\in \\mathbb{R}^{n}`,
-    :math:`y \\in \\mathbb{R}^{m}`, and :math:`d \\in \\mathbb{R}^{n}`,
-    approximately satisfying the stationarity
-     .. math::
-        \\begin{align}
-            \\nabla_x f(x) + y^{T} J_c(x) + d = 0,
-        \\end{align}
-
-    feasibility
-
-     .. math::
-        \\begin{align}
-            \\quad & l \\leq c(x) \\leq u \\\\
-            \\quad & l^x \\leq x \\leq u^x \\\\
-        \\end{align}
-
-    and complementarity
-
-     .. math::
-        \\begin{align}
-            y_i
-            \\begin{cases}
-                \\geq 0 & \\text{ if } c(x)_i = u_i \\\\
-                \\leq 0 & \\text{ if } c(x)_i = l_i \\\\
-                = 0 & \\text{ otherwise }
-            \\end{cases} \\\\
-            d_j
-            \\begin{cases}
-                \\geq 0 & \\text{ if } x_j = u^x_j \\\\
-                \\leq 0 & \\text{ if } x_j = l^x_j \\\\
-                = 0 & \\text{ otherwise }
-            \\end{cases}
-        \\end{align}
+        self.status = status
+        self.dist = dist
+        self.num_steps = num_steps
+        self.num_func_evals = num_func_evals
+        self.num_jac_evals = num_jac_evals
+        self.t = t_next
+        self.z = z_next
+        self.filter = filter_next
 
-    conditions.
-    """
 
-    def __init__(
-        self,
-        problem: Problem,
-        params: Params = Params(),
-    ) -> None:
-        """
-        Creates a new solver
-
-        Parameters
-        ----------
-        problem: pygradflow.problem.Problem
-            The problem to be solved
-        params: pygradflow.params.Params
-            Parameters used by the solver
-        """
+class IntegrationSolver:
+    def __init__(self, problem, params=Params()):
         self.orig_problem = problem
         self.params = params
+        self.path: Optional[List[np.ndarray]] = None
 
-    def compute_step(
-        self,
-        controller: StepController,
-        iterate: Iterate,
-        dt: float,
-        display: bool,
-        timer: Timer,
-    ) -> StepControlResult:
+    def create_events(self, result, triggers):
+        all_events = []
+
+        for i, trigger in enumerate(triggers):
+            t_events = result.t_events[i]
+            z_events = result.y_events[i]
+
+            for t, z in zip(t_events, z_events):
+                all_events.append(SwitchTrigger(t, z, trigger))
+
+        all_events.sort(key=lambda e: e.time)
+        return all_events
+
+    def create_filter(self, z, rho):
         problem = self.problem
-        params = self.params
-        assert self.rho != -1.0
+        x = z[: problem.num_vars]
+        lb = problem.var_lb
+        ub = problem.var_ub
 
-        method = newton_method(problem, params, iterate, dt, self.rho)
+        at_lb = Flow.isclose(x, lb)
+        at_ub = Flow.isclose(x, ub)
+        at_bounds = np.logical_or(at_lb, at_ub)
 
-        def next_steps():
-            curr_iterate = iterate
-            while True:
-                next_step = method.step(curr_iterate)
-                yield next_step
-                curr_iterate = next_step.iterate
+        dx = self.flow.neg_aug_lag_deriv_x(z, rho)
 
-        return controller.compute_step(
-            iterate, self.rho, dt, next_steps(), display, timer
-        )
+        active_lower = np.logical_and(at_lb, dx < 0)
+        active_upper = np.logical_and(at_ub, dx > 0)
 
-    def _deriv_check(self, x: np.ndarray, y: np.ndarray) -> None:
-        from pygradflow.deriv_check import deriv_check
-        from pygradflow.params import DerivCheck
+        fixed_indices = np.logical_or(active_lower, active_upper)
 
-        eval = self.evaluator
-        params = self.params
-        deriv_check_type = params.deriv_check
+        dx_zero = Flow.isclose(dx, 0.0)
+        ambiguous = np.logical_and(dx_zero, at_bounds)
 
-        if deriv_check_type == DerivCheck.NoCheck:
-            return
+        if not (ambiguous.any()):
+            return np.logical_not(fixed_indices)
 
-        if deriv_check_type & DerivCheck.CheckFirst:
-            logger.info("Checking objective derivative")
-            deriv_check(lambda x: eval.obj(x), x, eval.obj_grad(x), params)
-
-            logger.info("Checking constraint derivative")
-            deriv_check(lambda x: eval.cons(x), x, eval.cons_jac(x), params)
-
-        if deriv_check_type & DerivCheck.CheckSecond:
-            logger.info("Checking Hessian")
-
-            deriv_check(
-                lambda x: eval.obj_grad(x) + eval.cons_jac(x).T.dot(y),
-                x,
-                eval.lag_hess(x, y),
-                params,
-            )
+        ddx = self.flow.rhs_deriv_x(z, rho)
+        if Flow.isclose(ddx[ambiguous], 0.0).any():
+            raise Exception("Degenerate bound")
+
+        ambiguous_lb = np.logical_and(at_lb, dx_zero)
+        fixed_indices[ambiguous_lb] = ddx[ambiguous_lb] < 0
+
+        ambiguous_ub = np.logical_and(at_ub, dx_zero)
+        fixed_indices[ambiguous_ub] = ddx[ambiguous_lb] > 0
+
+        return np.logical_not(fixed_indices)
+
+    def _check_bounds(self, z):
+        problem = self.problem
+        x = z[: problem.num_vars]
+
+        lb = problem.var_lb
+        ub = problem.var_ub
+
+        between = np.logical_and(lb <= x, x <= ub)
+        at_lb = Flow.isclose(x, lb)
+        at_ub = Flow.isclose(x, ub)
+
+        valid = np.logical_or(between, np.logical_or(at_lb, at_ub))
+
+        assert valid.all()
+
+    def _check_filter(self, z, filter, rho):
+        assert (filter == self.create_filter(z, rho)).all()
+
+    def handle_events(self, events, restricted_flow, rho):
+        problem = self.problem
+        lb = problem.var_lb
+        ub = problem.var_ub
+        filter = restricted_flow.filter
+        flow = restricted_flow.flow
+
+        logger.debug("Handling %d events", len(events))
+
+        for event in events:
+            z_event = event.state
+            t_event = event.time
+
+            self._check_bounds(z_event)
+
+            @lazy_func
+            def rhs():
+                return flow.rhs(z_event, rho)
+
+            @lazy_func
+            def rhs_deriv():
+                return flow.rhs_deriv_x(z_event, rho)
+
+            if event.type == TriggerType.LB:
+                j = event.index
+                logger.debug("State %d reached lower bound at time %f", j, event.time)
 
-        logger.info("Finished derivative check")
+                assert filter[j]
+                assert Flow.isclose(z_event[j], lb[j])
+                assert func_neg(rhs, rhs_deriv, j)
+
+                return FilterChangedResult(t_event, z_event, filter, j)
+
+            elif event.type == TriggerType.UB:
+                j = event.index
+                logger.debug("State %d reached upper bound at time %f", j, event.time)
+
+                assert filter[j]
+                assert Flow.isclose(z_event[j], ub[j])
+                assert func_pos(rhs, rhs_deriv, j)
+
+                return FilterChangedResult(t_event, z_event, filter, j)
+
+            elif event.type == TriggerType.GRAD_FIXED:
+                j = event.index
+                logger.debug(
+                    "Gradient entry of fixed %d changed sign at time %f", j, event.time
+                )
+
+                at_lb = Flow.isclose(z_event[j], lb[j])
+                at_ub = Flow.isclose(z_event[j], ub[j])
+
+                assert not (filter[j])
+
+                if at_lb:
+                    assert func_pos(rhs, rhs_deriv, j)
+                elif at_ub:
+                    assert func_neg(rhs, rhs_deriv, j)
+
+                return FilterChangedResult(t_event, z_event, filter, j)
+
+            elif event.type == TriggerType.UNBOUNDED:
+                params = self.params
+                (x_event, y_event) = self.flow.split_states(z_event)
+                iterate_event = Iterate(problem, params, x_event, y_event)
+
+                if iterate_event.is_feasible(params.opt_tol):
+                    return UnboundedResult(t_event, z_event)
+
+            elif event.type == TriggerType.PENALTY:
+                (x_event, y_event) = self.flow.split_states(z_event)
+                return PenaltyResult(t_event, z_event)
+            else:
+                assert event.type == TriggerType.CONVERGED
+                logger.debug("Convergence achieved at time %f", event.time)
+                return ConvergedResult(t_event, z_event)
+
+        return None
 
     def print_result(
         self,
         total_time: float,
         status: SolverStatus,
         iterate: Iterate,
         iterations: int,
-        accepted_steps: int,
         dist_factor: float,
     ) -> None:
         rho = self.rho
 
         desc = "{:>45s}".format(SolverStatus.description(status))
 
         status_desc = Format.redgreen(desc, SolverStatus.success(status), bold=True)
         status_name = Format.bold("{:>20s}".format("Status"))
 
         logger.info("%20s: %45s", status_name, status_desc)
         logger.info("%20s: %45s", "Time", f"{total_time:.2f}s")
         logger.info("%20s: %45d", "Iterations", iterations)
-        logger.info("%20s: %45d", "Accepted steps", accepted_steps)
 
         logger.info("%20s: %45e", "Distance factor", dist_factor)
 
         logger.info("%20s: %45e", "Objective", iterate.obj)
         logger.info("%20s: %45e", "Aug Lag violation", iterate.aug_lag_violation(rho))
         logger.info("%20s: %45e", "Aug Lag dual", iterate.aug_lag_dual())
 
         logger.info("%20s: %45e", "Constraint violation", iterate.cons_violation)
         logger.info("%20s: %45e", "Dual violation", iterate.stat_res)
 
-    def _create_initial_iterate(
-        self, x0: Optional[np.ndarray], y0: Optional[np.ndarray]
-    ):
-        params = self.params
-        dtype = params.dtype
-        orig_problem = self.orig_problem
-        problem = self.problem
-
-        orig_lb = orig_problem.var_lb
-        orig_ub = orig_problem.var_ub
-
-        if x0 is None:
-            orig_n = orig_problem.num_vars
-            x_init = np.zeros((orig_n,), dtype=dtype)
-            np.clip(x_init, orig_lb, orig_ub, out=x_init)
-        else:
-            if (x0 > orig_ub).any() or (x0 < orig_lb).any():
-                logger.warning("Initial point violates variable bounds")
-                x0 = np.clip(x0, orig_lb, orig_ub)
-
-            x_init = cast(np.ndarray, x0)
-
-        if y0 is None:
-            orig_m = orig_problem.num_cons
-            y_init = np.zeros((orig_m,), dtype=dtype)
-        else:
-            y_init = cast(np.ndarray, y0)
+        eval = self.evaluator
 
-        transform = self.transform
-        (x_init, y_init) = transform.transform_sol(x_init, y_init)
+        eval_name = Format.bold("{:>20s}".format("Evaluations"))
+        logger.info("%20s", eval_name)
 
-        x = x_init.astype(dtype)
-        y = y_init.astype(dtype)
+        for component, num_evals in eval.num_evals.items():
+            name = component.name()
+            logger.info("%20s: %45d", name, num_evals)
+
+    def perform_integration(
+        self, curr_t, curr_z, curr_filter, rho
+    ) -> IntegrationResult:
+        # We want to integrate to +oo...
+        next_t = curr_t + 1e10
+
+        restricted_flow = RestrictedFlow(self.flow, curr_filter)
+        event_triggers = restricted_flow.create_event_triggers(curr_z, rho)
+
+        # Check consistency
+        (curr_x, curr_y) = self.flow.split_states(curr_z)
+        assert self.flow.is_boxed(curr_x)
+        restricted_flow.check_point(curr_z, rho)
+
+        ivp_result = sp.integrate.solve_ivp(
+            restricted_flow.rhs_func(rho),
+            (curr_t, next_t),
+            curr_z,
+            method="BDF",
+            jac=restricted_flow.rhs_jac_func(rho),
+            events=event_triggers,
+        )
 
-        return Iterate(problem, params, x, y, self.evaluator)
+        assert ivp_result.success, "Failed integration"
+        assert (ivp_result.y[:, 0] == curr_z).all()
 
-    def _create_scaling(self, x0):
-        params = self.params
-        problem = self.orig_problem
+        events = self.create_events(ivp_result, event_triggers)
+        event_result = self.handle_events(events, restricted_flow, rho)
 
-        scaling_type = params.scaling_type
+        status = IntegrationStatus.Finished
+        next_filter = curr_filter
 
-        if params.scaling is not None:
-            assert scaling_type == ScalingType.Custom
-            return params.scaling
-
-        if scaling_type == ScalingType.NoScaling:
-            return None
-        elif scaling_type == ScalingType.GradJac:
-            obj_grad = problem.obj_grad(x0)
-            cons_jac = None
-            if problem.num_cons > 0:
-                cons_jac = problem.cons_jac(x0)
-
-            return Scaling.from_grad_jac(obj_grad, cons_jac)
-        elif scaling_type == ScalingType.Custom:
-            raise ValueError("Custom scaling requires explicit scaling")
+        if event_result is None:
+            next_t = ivp_result.t[-1]
+            next_z = ivp_result.y[:, -1]
         else:
-            raise ValueError(f"Unknown scaling type {scaling_type}")
-
-    def _create_transformed_problem(self, x0):
-        self.scaling = self._create_scaling(x0)
+            next_z = event_result.z
+            next_t = event_result.t
 
-        orig_problem = self.orig_problem
-        params = self.params
+            if event_result.type == EventResultType.CONVERGED:
+                logger.debug("Convergence achieved")
+                status = IntegrationStatus.Converged
+            elif event_result.type == EventResultType.UNBOUNDED:
+                logger.debug("Unboundedness detected")
+                status = IntegrationStatus.Unbounded
+            elif event_result.type == EventResultType.FILTER_CHANGED:
+                logger.debug("Filter changed")
+                status = IntegrationStatus.Event
+                next_filter = event_result.filter
+            elif event_result.type == EventResultType.FREE_GRAD_ZERO:
+                logger.debug("Free gradient entry %d became zero", event_result.j)
+                status = IntegrationStatus.Event
+            else:
+                assert event_result.type == EventResultType.PENALTY
+                logger.debug("Penalty event")
+                status = IntegrationStatus.Penalty
+
+        (next_x, next_y) = self.flow.split_states(next_z)
 
-        self.transform = Transformation(orig_problem, params, self.scaling)
-        self.problem = self.transform.trans_problem
+        not_filter = np.logical_not(curr_filter)
 
-        pass
+        assert (next_x[not_filter] == curr_x[not_filter]).all()
 
-    def _check_terminate(self, iterate, iteration, timer):
-        params = self.params
+        assert self.flow.is_approx_boxed(next_x)
 
-        if (params.iteration_limit is not None) and (
-            iteration >= params.iteration_limit
-        ):
-            logger.debug("Iteration limit reached")
-            return SolverStatus.IterationLimit
-
-        if timer.reached_time_limit():
-            logger.debug("Reached time limit")
-            return SolverStatus.TimeLimit
-
-        if iterate.total_res <= params.opt_tol:
-            logger.debug("Convergence achieved")
-            return SolverStatus.Optimal
-
-        if iterate.locally_infeasible(params.opt_tol, params.local_infeas_tol):
-            logger.debug("Local infeasibility detected")
-            return SolverStatus.LocallyInfeasible
-
-        if (iterate.obj <= params.obj_lower_limit) and (
-            iterate.is_feasible(params.opt_tol)
-        ):
-            logger.debug("Unboundedness detected")
-            return SolverStatus.Unbounded
-
-    def solve(
-        self, x0: Optional[np.ndarray] = None, y0: Optional[np.ndarray] = None
-    ) -> SolverResult:
-        """
-        Solves the problem starting from the given primal / dual point
-
-        Parameters
-        ----------
-        x0: np.ndarray
-            The initial primal point :math:`x_0 \\in \\mathbb{R}^{n}`
-        y0: np.ndarray
-            The initial dual point :math:`y_0 \\in \\mathbb{R}^{m}`
-
-        Returns
-        -------
-        pygradflow.solver.SolverResult
-            The result of the solving process, including primal and dual
-            solutions
-        """
+        next_x = np.clip(next_x, self.problem.var_lb, self.problem.var_ub)
+        next_z = np.concatenate((next_x, next_y))
 
-        self._create_transformed_problem(x0)
         params = self.params
-        problem = self.problem
 
-        if params.validate_input:
-            self.evaluator: Evaluator = ValidatingEvaluator(self.problem, params)
-        else:
-            self.evaluator = SimpleEvaluator(self.problem, params)
+        if params.collect_path:
+            assert self.path is not None
+            path = cast(List[np.ndarray], self.path)
+            assert (path[-1][:, -1] == curr_z).all()
+            assert (path[-1][:, -1] == ivp_result.y[:, 0]).all()
+            path.append(ivp_result.y[:, 1:])
+            path[-1][:, -1] = next_z
+
+        dist = np.linalg.norm(
+            (ivp_result.y[:, 1:] - ivp_result.y[:, :-1]), axis=0
+        ).sum()
 
-        self.penalty = penalty_strategy(self.problem, params)
-        self.rho = -1.0
+        return IntegrationResult(
+            status,
+            dist,
+            next_t,
+            next_z,
+            next_filter,
+            num_steps=ivp_result.t.size,
+            num_func_evals=ivp_result.nfev,
+            num_jac_evals=ivp_result.njev,
+        )
 
-        display = problem_display(problem, params)
+    def solve(self, x0: Optional[np.ndarray] = None, y0: Optional[np.ndarray] = None):
 
-        n = problem.num_vars
-        m = problem.num_cons
+        self.transform = Transformation(self.orig_problem, self.params, x0, y0)
 
-        iterate = self._create_initial_iterate(x0, y0)
+        self.problem = self.transform.trans_problem
+        self.evaluator = self.transform.evaluator
 
-        logger.info("Solving problem with {0} variables, {1} constraints".format(n, m))
+        problem = self.problem
+        params = self.params
+        self.flow = Flow(problem, params, self.evaluator)
+        self.rho = self.params.rho
 
-        lamb = params.lamb_init
+        initial_iterate = self.transform.initial_iterate
 
-        controller = step_controller(problem, params)
+        self.path = [initial_iterate.z[:, None]]
 
-        self._deriv_check(iterate.x, iterate.y)
+        print_problem_stats(problem, initial_iterate)
 
-        self.rho = self.penalty.initial(iterate)
+        x_init = initial_iterate.x
+        y_init = initial_iterate.y
 
-        logger.debug("Initial Aug Lag: %.10e", iterate.aug_lag(self.rho))
+        curr_z = np.concatenate((x_init, y_init))
+        curr_t = 0.0
+        curr_filter = self.create_filter(curr_z, self.rho)
 
         status = None
-        start_time = time.time()
-        last_time = start_time
-        line_diff = 0
         iteration = 0
-
-        logger.info(display.header)
-
         path_dist = 0.0
-        initial_iterate = iterate
         accepted_steps = 0
-        iteration = 0
-
-        last_active_set = None
-        last_display_iteration = -1
 
         timer = Timer(params.time_limit)
 
+        display = integrator_display(problem, params)
+        logger.info(display.header)
+
         while True:
-            status = self._check_terminate(iterate, iteration, timer)
-            if status is not None:
+            self._check_filter(curr_z, curr_filter, self.rho)
+            self._check_bounds(curr_z)
+
+            restricted_flow = RestrictedFlow(self.flow, curr_filter)
+            curr_res = restricted_flow.residuum(curr_z)
+
+            if curr_res <= params.opt_tol:
+                logger.debug("Iterate is optimal")
+                status = SolverStatus.Optimal
                 break
 
-            curr_time = time.time()
-            display_iterate = curr_time - last_time >= params.display_interval
+            logger.debug("Iteration %d: value: %s", iteration, curr_z)
 
-            step_result = self.compute_step(
-                controller, iterate, 1.0 / lamb, display_iterate, timer
+            logger.debug(
+                "State: %s, filter: %s, grad: %s",
+                curr_z,
+                curr_filter,
+                self.flow.rhs(curr_z, self.rho),
             )
 
-            x = iterate.x
-            y = iterate.y
-
-            next_iterate = step_result.iterate
-            accept = step_result.accepted
-            lamb = step_result.lamb
-
-            if lamb >= params.lamb_max:
-                raise Exception(
-                    f"Inverse step size {lamb} exceeded maximum {params.lamb_max} (incorrect derivatives?)"
-                )
+            if timer.reached_time_limit():
+                logger.debug("Reached time limit")
+                status = SolverStatus.TimeLimit
+                break
 
-            primal_step_norm = np.linalg.norm(next_iterate.x - iterate.x)
-            dual_step_norm = np.linalg.norm(next_iterate.y - iterate.y)
+            (curr_x, curr_y) = self.flow.split_states(curr_z)
 
-            if display_iterate:
-                last_time = curr_time
-                line_diff += 1
+            curr_it = Iterate(problem, params, curr_x, curr_y)
 
-                state = dict()
-                state["iterate"] = iterate
+            if curr_it.locally_infeasible(params.opt_tol, params.local_infeas_tol):
+                logger.debug("Local infeasibility detected")
+                status = SolverStatus.LocallyInfeasible
+                break
 
-                def compute_last_active_set():
-                    if last_display_iteration + 1 == iteration:
-                        return last_active_set
-                    return None
+            if (curr_it.obj <= params.obj_lower_limit) and (
+                curr_it.is_feasible(params.opt_tol)
+            ):
+                logger.debug("Unboundedness detected")
+                status = SolverStatus.Unbounded
+                break
 
-                state["last_active_set"] = compute_last_active_set
-                state["curr_active_set"] = lambda: step_result.active_set
+            result = self.perform_integration(curr_t, curr_z, curr_filter, self.rho)
+            path_dist += result.dist
 
+            if display.should_display():
+                state = StateData()
+                curr_x, curr_y = self.flow.split_states(curr_z)
+                iterate = curr_it
+                state["iterate"] = iterate
+                state["filter"] = curr_filter
                 state["aug_lag"] = lambda: iterate.aug_lag(self.rho)
-                state["obj"] = lambda: iterate.obj()
-                state["iter"] = lambda: iteration + 1
-                state["primal_step_norm"] = lambda: primal_step_norm
-                state["dual_step_norm"] = lambda: dual_step_norm
-                state["lamb"] = lambda: lamb
-                state["step_accept"] = lambda: accept
-                state["rcond"] = lambda: step_result.rcond
+                state["obj"] = lambda: iterate.obj
+                state["iter"] = iteration + 1
+                state["num_func_evals"] = result.num_func_evals
+                state["num_jac_evals"] = result.num_jac_evals
+                state["num_steps"] = result.num_steps
+                state["dt"] = result.t - curr_t
+                state["step_type"] = result.status
 
                 logger.info(display.row(state))
-                last_display_iteration = iteration
 
-            if accept:
-                # Accept
-                next_rho = self.penalty.update(iterate, next_iterate)
+            iteration += 1
 
-                if next_rho != self.rho:
-                    logger.debug(
-                        "Updating penalty parameter from %e to %e", self.rho, next_rho
-                    )
-                    self.rho = next_rho
+            curr_z = result.z
+            curr_t = result.t
+            curr_filter = result.filter
 
-                delta = iterate.dist(next_iterate)
+            if result.status == IntegrationStatus.Converged:
+                status = SolverStatus.Optimal
+                break
+            elif result.status == IntegrationStatus.Unbounded:
+                status = SolverStatus.Unbounded
+                break
+            elif result.status == IntegrationStatus.Penalty:
+                # Continuation criterion is violated => update penalty parameter
+                logger.debug(
+                    "Updating penalty parameter %f -> %f", self.rho, 10 * self.rho
+                )
+                self.rho *= 10
+                curr_filter = self.create_filter(curr_z, self.rho)
 
-                iterate = next_iterate
+            if (params.iteration_limit is not None) and (
+                iteration >= params.iteration_limit
+            ):
+                status = SolverStatus.IterationLimit
+                logger.debug("Iteration limit reached")
+                break
 
-                path_dist += primal_step_norm + dual_step_norm
-                accepted_steps += 1
+        (curr_x, curr_y) = self.flow.split_states(curr_z)
+        iterate = Iterate(problem, params, curr_x, curr_y)
 
-                if (lamb <= params.lamb_term) and (delta <= params.opt_tol):
-                    logger.debug("Convergence achieved")
-                    status = SolverStatus.Optimal
-                    break
+        result_props = dict()
 
-            iteration += 1
-            last_active_set = step_result.active_set
-            # last_active_set = iterate.active_set
+        if params.collect_path:
+            complete_path = np.hstack(self.path)
+            self.path = None
 
-        total_time = timer.elapsed()
+            num_vars = problem.num_vars
 
-        direct_dist = iterate.dist(initial_iterate)
+            result_props["path"] = complete_path
+            result_props["primal_path"] = complete_path[:num_vars, :]
+            result_props["dual_path"] = complete_path[num_vars:, :]
 
-        assert path_dist >= direct_dist
+        x = iterate.x
+        y = iterate.y
+        d = iterate.bounds_dual
 
-        dist_factor = path_dist / direct_dist if direct_dist != 0.0 else 1.0
         iterations = iteration
 
-        assert status is not None
+        logger.debug("Status: %s", status)
 
-        self.print_result(
-            total_time=total_time,
-            status=status,
-            iterate=iterate,
-            iterations=iterations,
-            accepted_steps=accepted_steps,
-            dist_factor=dist_factor,
-        )
+        direct_dist = iterate.dist(initial_iterate)
 
-        x = iterate.x
-        y = iterate.y
-        d = iterate.bounds_dual
+        total_time = timer.elapsed()
+
+        dist_factor = path_dist / direct_dist if direct_dist != 0.0 else 1.0
 
-        transform = self.transform
+        self.print_result(total_time, status, iterate, iterations, dist_factor)
 
-        (x, y, d) = transform.restore_sol(x, y, d)
+        (x, y, d) = self.transform.restore_sol(x, y, d)
 
         return SolverResult(
             x,
             y,
             d,
             status,
             iterations=iterations,
             num_accepted_steps=accepted_steps,
             total_time=total_time,
             dist_factor=dist_factor,
+            **result_props,
         )
```

### Comparing `pygradflow-0.4.9/pygradflow/step/__init__.py` & `pygradflow-0.5.0/pygradflow/step/__init__.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/step/asymmetric_step_solver.py` & `pygradflow-0.5.0/pygradflow/step/asymmetric_step_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,21 @@
         rho: float,
     ) -> None:
         super().__init__(problem, params, orig_iterate, dt, rho)
 
         assert dt > 0.0
         assert rho > 0.0
 
-        self.active_set = None
-        self.jac = None
-        self.hess = None
-
-    def reset_deriv(self) -> None:
-        self.deriv = None
-        self.solver = None
-
     def update_derivs(self, iterate: Iterate) -> None:
-        self.jac = copy.copy(iterate.aug_lag_deriv_xy())
-        self.hess = copy.copy(iterate.aug_lag_deriv_xx(rho=0.0))
+        self._jac = copy.copy(iterate.aug_lag_deriv_xy())
+        self._hess = copy.copy(iterate.aug_lag_deriv_xx(rho=0.0))
         self.reset_deriv()
 
     def update_active_set(self, active_set: np.ndarray) -> None:
-        self.active_set = copy.copy(active_set)
+        self._active_set = copy.copy(active_set)
         self.reset_deriv()
 
     def overwrite_active_rows(self, matrix):
         m = self.m
         n = self.n
 
         active_set = self.active_set
@@ -141,16 +133,16 @@
             var_sol = sol[:n]
             var_sol[active_set] = b0
             return sol
 
         return initial_sol
 
     def solve_scaled(self, b0, b1, b2t):
-        if self.deriv is None:
-            self.deriv = self.compute_deriv(self.active_set)
+        if self._deriv is None:
+            self._deriv = self.compute_deriv(self.active_set)
 
         if self.solver is None:
             self.solver = self.linear_solver(self.deriv)
 
         params = self.params
 
         rhs = self.compute_rhs(b0, b1, b2t)
```

### Comparing `pygradflow-0.4.9/pygradflow/step/box_control.py` & `pygradflow-0.5.0/pygradflow/step/box_control.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-import time
-
 import cyipopt
 import numpy as np
+import scipy as sp
 from scipy.optimize import Bounds, minimize
 
 from pygradflow.implicit_func import ImplicitFunc
 from pygradflow.iterate import Iterate
 from pygradflow.step.step_control import (
     StepController,
     StepControlResult,
     StepSolverError,
 )
 
-max_num_it = 10000
-max_num_linesearch_it = 40
-t_init = 1.0
-beta = 0.5
-
 
 class BoxReducedProblem(cyipopt.Problem):
     """
     Solves the primal-dual proximally regularized box-reduced problem
      .. math::
         \\begin{align}
             \\min_{x \\in \\mathbb{R}^{n}, w \\in \\mathbb{R}^{n}} \\quad
@@ -59,78 +53,123 @@
 
     def constraint(self, x):
         return np.array([])
 
     def jacobian(self, x):
         return np.empty((0, self.num_vars))
 
+    def hessianstructure(self):
+        x0 = self.x0
+        hess = self.step_controller.hessian(self.iterate, x0, self.lamb, self.rho)
+        hess = hess.tocoo()
+        rows = hess.row
+        cols = hess.col
+
+        hess_filter = rows >= cols
+
+        return rows[hess_filter], cols[hess_filter]
+
+    def hessian(self, x, lag, obj_factor):
+        hess = self.step_controller.hessian(self.iterate, x, self.lamb, self.rho)
+        hess = hess.tocoo()
+
+        rows = hess.row
+        cols = hess.col
+        data = hess.data
+
+        hess_filter = rows >= cols
+
+        return data[hess_filter]
+
     def set_options(self, timer):
         import logging
 
         logging.getLogger("cyipopt").setLevel(logging.WARNING)
         self.add_option("print_level", 0)
-        # self.add_option("derivative_test", "first-order")
-        self.add_option("hessian_approximation", "limited-memory")
+        # self.add_option("derivative_test", "second-order")
+        # self.add_option("hessian_approximation", "limited-memory")
+        # self.add_option("max_iter", 10)
 
         remaining = timer.remaining()
 
         if remaining <= 0.0:
             raise StepSolverError("Time limit reached")
         elif np.isfinite(remaining):
             self.add_option("max_cpu_time", remaining)
 
-    def solve(self, timer):
-        iterate = self.iterate
+    @property
+    def x0(self):
+        return self.iterate.x
 
+    def solve(self, timer):
         self.set_options(timer)
-        x0 = iterate.x
+        x0 = self.x0
 
         # Solve using Ipopt
         x, info = super().solve(x0)
 
         if info["status"] != 0:
             raise StepSolverError("Ipopt failed to solve the problem")
 
         return x
 
 
 class BoxReducedController(StepController):
 
     def objective(self, iterate, x, lamb, rho):
+        eval = iterate.eval
         xhat = iterate.x
         yhat = iterate.y
 
-        obj = self.problem.obj(x)
-        cons = self.problem.cons(x)
+        obj = eval.obj(x)
+        cons = eval.cons(x)
 
         dx = x - xhat
         dx_norm_sq = np.dot(dx, dx)
 
         w = -1 / lamb * cons
         dy = w - yhat
         dy_norm_sq = np.dot(dy, dy)
 
         curr_obj = obj + 0.5 * rho * np.dot(cons, cons)
         curr_obj += 0.5 * lamb * (dx_norm_sq + dy_norm_sq)
 
         return curr_obj
 
     def gradient(self, iterate, x, lamb, rho):
+        eval = iterate.eval
         xhat = iterate.x
         yhat = iterate.y
 
-        obj_grad = self.problem.obj_grad(x)
-        cons = self.problem.cons(x)
-        cons_jac = self.problem.cons_jac(x)
+        obj_grad = eval.obj_grad(x)
+        cons = eval.cons(x)
+        cons_jac = eval.cons_jac(x)
 
         dx = x - xhat
         cons_jac_factor = (rho + (1 / lamb)) * cons + yhat
         return obj_grad + lamb * dx + cons_jac.T.dot(cons_jac_factor)
 
-    def solve_step(self, iterate, rho, dt, timer):
+    def hessian(self, iterate, x, lamb, rho):
+        eval = iterate.eval
+        (n,) = x.shape
+
+        yhat = iterate.y
+
+        cons = eval.cons(x)
+        jac = eval.cons_jac(x)
+        cons_factor = 1 / lamb + rho
+        y = cons_factor * cons + yhat
+
+        hess = eval.lag_hess(x, y)
+        hess += sp.sparse.diags([lamb], shape=(n, n))
+        hess += cons_factor * (jac.T @ jac)
+
+        return hess
+
+    def solve_step_scipy(self, iterate, rho, dt, timer):
         problem = self.problem
 
         x = iterate.x
         lamb = 1.0 / dt
 
         lb = problem.var_lb
         ub = problem.var_ub
@@ -167,30 +206,57 @@
         )
 
         if not result.success:
             raise StepSolverError("Scipy failed to solve the problem")
 
         return result.x
 
+    def solve_step_ipopt(self, iterate, rho, dt, timer):
+        lamb = 1.0 / dt
+        reduced_problem = BoxReducedProblem(self, iterate, lamb, rho)
+        return reduced_problem.solve(timer=timer)
+
+    def solve_step_box(self, iterate, rho, dt, timer):
+        from .box_solver import BoxSolverError, solve_box_constrained
+
+        problem = self.problem
+        lamb = 1.0 / dt
+
+        def objective(x):
+            return self.objective(iterate, x, lamb, rho)
+
+        def gradient(x):
+            return self.gradient(iterate, x, lamb, rho)
+
+        def hessian(x):
+            return self.hessian(iterate, x, lamb, rho)
+
+        try:
+            return solve_box_constrained(
+                iterate.x, objective, gradient, hessian, problem.var_lb, problem.var_ub
+            )
+        except BoxSolverError as e:
+            raise StepSolverError("Box-constrained solver failed to converge") from e
+
     def step(
         self, iterate, rho: float, dt: float, next_steps, display: bool, timer
     ) -> StepControlResult:
 
         lamb = 1.0 / dt
 
         problem = self.problem
         params = self.params
 
-        # reduced_problem = BoxReducedProblem(self, iterate, lamb, rho)
-        # x = reduced_problem.solve(timer=timer)
+        # x = self.solve_step_ipopt(iterate, rho, dt, timer)
 
-        # TODO: The minimize function shipped with scipy
+        # Note: The minimize function shipped with scipy
         # do not consistently produce high-quality solutions,
         # causing the optimization of the overall problem to fail.
-        x = self.solve_step(iterate, rho, dt, timer=timer)
+        # x = self.solve_step_scipy(iterate, rho, dt, timer)
+        x = self.solve_step_box(iterate, rho, dt, timer)
 
         cons = problem.cons(x)
         w = (-1 / lamb) * cons
         y = iterate.y - w
 
         next_iterate = Iterate(problem, params, x, y, iterate.eval)
```

### Comparing `pygradflow-0.4.9/pygradflow/step/cond_estimate.py` & `pygradflow-0.5.0/pygradflow/step/cond_estimate.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/step/distance_ratio_control.py` & `pygradflow-0.5.0/pygradflow/step/distance_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/step/exact_control.py` & `pygradflow-0.5.0/pygradflow/step/exact_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/step/extended_step_solver.py` & `pygradflow-0.5.0/pygradflow/step/extended_step_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,14 @@
         rho: float,
     ) -> None:
         super().__init__(problem, params, orig_iterate, dt, rho)
 
         assert dt > 0.0
         assert rho > 0.0
 
-        self.active_set = None
-        self.jac = None
-        self.hess = None
-
     def extract_rows(
         self, mat: sp.sparse.spmatrix, row_filter: np.ndarray
     ) -> sp.sparse.spmatrix:
         mat = mat.tocsc()
         return mat[row_filter, :]
 
     def _compute_deriv(self) -> None:
@@ -74,35 +70,34 @@
 
         blocks = [
             [trans_active_mat, None],
             [filtered_hess, trans_filtered_jac],
             [jac, lower_mat],
         ]
 
-        self.deriv = sp.sparse.bmat(blocks, format="csc")
+        self._deriv = sp.sparse.bmat(blocks, format="csc")
 
         assert self.deriv.shape == (n + m, n + m)
         assert self.deriv.dtype == self.params.dtype
 
     def solve_scaled(self, b0, b1, b2t):
         params = self.params
-        if self.deriv is None:
+        if self._deriv is None:
             self._compute_deriv()
 
-        if self.solver is None:
-            self.solver = self.linear_solver(self.deriv)
-
         n = self.n
         m = self.m
 
         rhs = np.concatenate((b0, b1, b2t))
 
         assert rhs.shape == (n + m,)
 
         try:
+            if self.solver is None:
+                self.solver = self.linear_solver(self.deriv)
             sol = self.solver.solve(rhs)
         except LinearSolverError as e:
             raise StepSolverError from e
 
         dx = sol[:n]
         dy = sol[n:]
```

### Comparing `pygradflow-0.4.9/pygradflow/step/fixed_control.py` & `pygradflow-0.5.0/pygradflow/step/fixed_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/step/linear_solver.py` & `pygradflow-0.5.0/pygradflow/step/linear_solver.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/step/opti_control.py` & `pygradflow-0.5.0/pygradflow/step/opti_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import math
 
 import cyipopt
 import numpy as np
 
 from pygradflow.eval import EvalError, astype
-from pygradflow.implicit_func import ImplicitFunc
 from pygradflow.iterate import Iterate
 from pygradflow.step.step_control import (
     StepController,
     StepControlResult,
     StepSolverError,
 )
 
@@ -251,16 +250,10 @@
 
         lamb = 1.0 / dt
         implicit_problem = ImplicitProblem(iterate, lamb, rho)
         (x, y) = implicit_problem.solve(timer=timer)
 
         next_iterate = Iterate(problem, params, x, y, iterate.eval)
 
-        implicit_func = ImplicitFunc(problem, iterate, dt)
-
-        value = implicit_func.value_at(next_iterate, rho)
-
-        residuum = np.linalg.norm(value)
-
         return StepControlResult(
             next_iterate, 0.5 * lamb, active_set=None, rcond=None, accepted=True
         )
```

### Comparing `pygradflow-0.4.9/pygradflow/step/residuum_ratio_control.py` & `pygradflow-0.5.0/pygradflow/step/residuum_ratio_control.py`

 * *Files identical despite different names*

### Comparing `pygradflow-0.4.9/pygradflow/step/scaled_step_solver.py` & `pygradflow-0.5.0/pygradflow/step/scaled_step_solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import copy
-from typing import Optional, Tuple
+from typing import Optional, Tuple, cast
 
 import numpy as np
+import scipy as sp
 
 from pygradflow.implicit_func import ScaledImplicitFunc
 from pygradflow.iterate import Iterate
 from pygradflow.params import Params
 from pygradflow.problem import Problem
 from pygradflow.step.step_solver import StepResult, StepSolver
 
@@ -17,21 +18,26 @@
         params: Params,
         orig_iterate: Iterate,
         dt: float,
         rho: float,
     ) -> None:
         super().__init__(problem, params)
 
-        self.problem = problem
         self.orig_iterate = orig_iterate
-        self.func = ScaledImplicitFunc(problem, orig_iterate, dt)
+        self._func = ScaledImplicitFunc(problem, orig_iterate, dt)
+
+        self._deriv: Optional[sp.sparse.spmatrix] = None
 
         self.dt = dt
         self.rho = rho
 
+    @property
+    def func(self) -> ScaledImplicitFunc:
+        return self._func
+
     def initial_rhs(
         self, iterate: Iterate
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         n = self.n
         m = self.m
 
         rhs = self.func.value_at(iterate, self.rho, self.active_set)
@@ -54,24 +60,29 @@
 
     def solve_scaled(
         self, b0, b1, b2t
     ) -> Tuple[np.ndarray, np.ndarray, Optional[float]]:
         raise NotImplementedError()
 
     def reset_deriv(self) -> None:
-        self.deriv = None
+        self._deriv = None
         self.solver = None
 
+    @property
+    def deriv(self) -> sp.sparse.spmatrix:
+        assert self._deriv is not None
+        return cast(sp.sparse.spmatrix, self._deriv)
+
     def update_derivs(self, iterate: Iterate) -> None:
-        self.jac = copy.copy(iterate.aug_lag_deriv_xy())
-        self.hess = copy.copy(iterate.aug_lag_deriv_xx(rho=0.0))
+        self._jac = copy.copy(iterate.aug_lag_deriv_xy())
+        self._hess = copy.copy(iterate.aug_lag_deriv_xx(rho=0.0))
         self.reset_deriv()
 
     def update_active_set(self, active_set: np.ndarray) -> None:
-        self.active_set = copy.copy(active_set)
+        self._active_set = copy.copy(active_set)
         self.reset_deriv()
 
     def solve(self, iterate: Iterate) -> StepResult:
         (b0, b1, b2) = self.initial_rhs(iterate)
 
         n = self.n
         m = self.m
```

### Comparing `pygradflow-0.4.9/pygradflow/step/standard_step_solver.py` & `pygradflow-0.5.0/pygradflow/step/standard_step_solver.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,51 +24,52 @@
         orig_iterate: Iterate,
         dt: float,
         rho: float,
     ) -> None:
         super().__init__(problem, params)
 
         self.orig_iterate = orig_iterate
-        self.func = ImplicitFunc(problem, orig_iterate, dt)
+        self._func = ImplicitFunc(problem, orig_iterate, dt)
 
-        self.active_set = None
-        self.jac = None
-        self.hess = None
         self.rho = rho
 
+    @property
+    def func(self) -> ImplicitFunc:
+        return self._func
+
     def _compute_deriv(self) -> None:
         assert self.active_set is not None
         assert self.jac is not None
         assert self.hess is not None
 
         self.deriv = self.func.deriv(self.jac, self.hess, self.active_set)
 
     def _reset_deriv(self) -> None:
         self.deriv = None
         self.solver = None
 
     def update_derivs(self, iterate: Iterate) -> None:
-        self.jac = copy.copy(iterate.aug_lag_deriv_xy())
-        self.hess = copy.copy(iterate.aug_lag_deriv_xx(self.rho))
+        self._jac = copy.copy(iterate.aug_lag_deriv_xy())
+        self._hess = copy.copy(iterate.aug_lag_deriv_xx(self.rho))
         self._reset_deriv()
 
     def update_active_set(self, active_set: np.ndarray) -> None:
-        self.active_set = copy.copy(active_set)
+        self._active_set = copy.copy(active_set)
         self._reset_deriv()
 
     def solve(self, iterate: Iterate) -> StepResult:
         if self.deriv is None:
             self._compute_deriv()
 
-        if self.solver is None:
-            self.solver = self.linear_solver(self.deriv)
-
         rhs = self.func.value_at(iterate, self.rho, self.active_set)
 
         try:
+            if self.solver is None:
+                self.solver = self.linear_solver(self.deriv)
+
             sol = self.solver.solve(rhs)
         except LinearSolverError as e:
             raise StepSolverError from e
 
         n = self.n
         m = self.m
```

### Comparing `pygradflow-0.4.9/pygradflow/step/step_control.py` & `pygradflow-0.5.0/pygradflow/step/step_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import logging
 from typing import Iterator, Optional
 
 import numpy as np
 
-from pygradflow.display import inner_display
+from pygradflow.display import StateData, inner_display
 from pygradflow.implicit_func import ImplicitFunc
 from pygradflow.iterate import Iterate
 from pygradflow.log import logger
 from pygradflow.params import Params, StepControlType
 from pygradflow.problem import Problem
 from pygradflow.step.step_solver import StepResult
 from pygradflow.timer import Timer
@@ -105,15 +105,15 @@
 
     def display_step(self, iteration, step):
         level = logger.getEffectiveLevel()
         if not self.display or level > logging.DEBUG:
             return
 
         iterate = step.iterate
-        state = dict()
+        state = StateData()
         state["iter"] = lambda: iteration
         state["residuum"] = lambda: self.res_func(iterate)
         state["dist"] = lambda: step.diff
         state["active_set_size"] = lambda: step.active_set.sum()
         logger.debug("     %s", self.display.row(state))
```

### Comparing `pygradflow-0.4.9/pygradflow/step/step_solver.py` & `pygradflow-0.5.0/pygradflow/step/step_solver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import abc
 import functools
+from typing import Optional, cast
 
 import numpy as np
 import scipy as sp
 
+from pygradflow.implicit_func import StepFunc
 from pygradflow.iterate import Iterate
 from pygradflow.params import Params
 from pygradflow.problem import Problem
 from pygradflow.step.linear_solver import LinearSolver, LinearSolverError
 from pygradflow.util import norm_mult
 
 
@@ -39,21 +41,44 @@
 class StepSolver(abc.ABC):
     def __init__(self, problem: Problem, params: Params) -> None:
         self.problem = problem
         self.params = params
         self.n = problem.num_vars
         self.m = problem.num_cons
 
+        self._active_set: Optional[np.ndarray] = None
+        self._jac: Optional[sp.sparse.spmatrix] = None
+        self._hess: Optional[sp.sparse.spmatrix] = None
+
+        self.solver: Optional[LinearSolver] = None
+
+    @property
+    def active_set(self) -> np.ndarray:
+        assert self._active_set is not None
+        return cast(np.ndarray, self._active_set)
+
+    @property
+    def jac(self) -> sp.sparse.spmatrix:
+        assert self._jac is not None
+        return cast(sp.sparse.spmatrix, self._jac)
+
+    @property
+    def hess(self) -> sp.sparse.spmatrix:
+        assert self._hess is not None
+        return cast(sp.sparse.spmatrix, self._hess)
+
     def linear_solver(self, mat: sp.sparse.spmatrix) -> LinearSolver:
         from .linear_solver import linear_solver
 
         solver_type = self.params.linear_solver_type
         return linear_solver(mat, solver_type)
 
-    def estimate_rcond(self, mat: sp.sparse.spmatrix, solver: LinearSolver) -> float:
+    def estimate_rcond(
+        self, mat: sp.sparse.spmatrix, solver: LinearSolver
+    ) -> Optional[float]:
         from .cond_estimate import ConditionEstimator
 
         estimator = ConditionEstimator(mat, solver, self.params)
         rcond = None
 
         try:
             rcond = estimator.estimate_rcond()
@@ -62,14 +87,19 @@
 
         return rcond
 
     @abc.abstractmethod
     def update_active_set(self, active_set: np.ndarray):
         raise NotImplementedError()
 
+    @property
+    @abc.abstractmethod
+    def func(self) -> StepFunc:
+        raise NotImplementedError()
+
     @abc.abstractmethod
     def update_derivs(self, iterate: Iterate):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def solve(self, iterate: Iterate) -> StepResult:
         raise NotImplementedError()
```

### Comparing `pygradflow-0.4.9/pygradflow/step/symmetric_step_solver.py` & `pygradflow-0.5.0/pygradflow/step/symmetric_step_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,40 +19,35 @@
         rho: float,
     ) -> None:
         super().__init__(problem, params, orig_iterate, dt, rho)
 
         assert dt > 0.0
         assert rho > 0.0
 
-        self.active_set = None
-        self.jac = None
-        self.hess = None
-
     def compute_hess_jac(self) -> None:
         inactive_indices = np.where(np.logical_not(self.active_set))[0]
 
         lamb = 1.0 / self.dt
 
         n = self.n
 
-        hess = self.hess + sp.sparse.diags(
+        hess = self._hess + sp.sparse.diags(
             [lamb], shape=(n, n), dtype=self.params.dtype
         )
 
         hess_rows = hess.tocsr()[inactive_indices, :]
         self.hess_rows = hess_rows.tocsc()
 
     def update_derivs(self, iterate: Iterate) -> None:
         super().update_derivs(iterate)
-        self.jac = self.jac.tocsc()
+        self._jac = self.jac.tocsc()
 
     def reset_deriv(self) -> None:
         super().reset_deriv()
         self.hess_rows = None
-        self.deriv = None
 
     def compute_deriv(self, active_set: np.ndarray) -> sp.sparse.spmatrix:
         inactive_indices = np.where(np.logical_not(self.active_set))[0]
         lamb = 1.0 / self.dt
         rho = self.rho
 
         m = self.m
@@ -129,22 +124,21 @@
             rcond = self.estimate_rcond(self.deriv, self.solver)
 
         return (dx, dy, rcond)
 
     def solve_deriv(
         self, active_set: np.ndarray, deriv: sp.sparse.spmatrix, rhs: np.ndarray
     ) -> np.ndarray:
-        if self.solver is None:
-            self.solver = self.linear_solver(self.deriv)
-
         try:
+            if self.solver is None:
+                self.solver = self.linear_solver(self.deriv)
             sol = self.solver.solve(rhs)
         except LinearSolverError as e:
             raise StepSolverError from e
 
         return sol
 
     def solve_active_set(self, active_set: np.ndarray, rhs: np.ndarray) -> np.ndarray:
-        if self.deriv is None:
-            self.deriv = self.compute_deriv(self.active_set)
+        if self._deriv is None:
+            self._deriv = self.compute_deriv(self.active_set)
 
         return self.solve_deriv(self.active_set, self.deriv, rhs)
```

### Comparing `pygradflow-0.4.9/pyproject.toml` & `pygradflow-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygradflow"
-version = "0.4.9"
+version = "0.5.0"
 description = "PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs."
 authors = ["Christoph Hansknecht <christoph.hansknecht@tu-clausthal.de>"]
 readme = "README.md"
 repository = "https://github.com/chrhansk/pygradflow"
 documentation = "https://pygradflow.readthedocs.io"
 
 
@@ -20,25 +20,26 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-isort = "^3.1.0"
 pytest-black = "^0.3.12"
 mypy = "^1.7.1"
 types-pyyaml = "^6.0.12"
 pytest-timeout = "^2.3.1"
+pyflakes = "^3.2.0"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 
 [tool.poetry.group.bench]
 optional = true
 
 [tool.poetry.group.bench.dependencies]
 pyqplib = "^0.1.3"
-pycutest = "^1.5.1"
+pycutest = "^1.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `pygradflow-0.4.9/PKG-INFO` & `pygradflow-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygradflow
-Version: 0.4.9
+Version: 0.5.0
 Summary: PyGradFlow is a simple implementation of the sequential homotopy method to be used to solve general nonlinear programs.
 Home-page: https://github.com/chrhansk/pygradflow
 Author: Christoph Hansknecht
 Author-email: christoph.hansknecht@tu-clausthal.de
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

