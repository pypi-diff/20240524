# Comparing `tmp/mpspy-0.1.1.tar.gz` & `tmp/mpspy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpspy-0.1.1.tar", max compression
+gzip compressed data, was "mpspy-0.1.2.tar", max compression
```

## Comparing `mpspy-0.1.1.tar` & `mpspy-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-05-24 13:59:42.927204 mpspy-0.1.1/LICENSE
--rw-r--r--   0        0        0      423 2024-05-24 13:59:42.927204 mpspy-0.1.1/README.md
--rw-r--r--   0        0        0      129 2024-05-24 13:59:42.927204 mpspy-0.1.1/mpspy/__init__.py
--rw-r--r--   0        0        0       52 2024-05-24 13:59:42.927204 mpspy-0.1.1/mpspy/log.py
--rw-r--r--   0        0        0    11757 2024-05-24 13:59:42.927204 mpspy-0.1.1/mpspy/reader.py
--rw-r--r--   0        0        0      387 2024-05-24 13:59:42.927204 mpspy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 mpspy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-24 14:31:22.427909 mpspy-0.1.2/LICENSE
+-rw-r--r--   0        0        0      423 2024-05-24 14:31:22.427909 mpspy-0.1.2/README.md
+-rw-r--r--   0        0        0      150 2024-05-24 14:31:22.431908 mpspy-0.1.2/mpspy/__init__.py
+-rw-r--r--   0        0        0      979 2024-05-24 14:31:22.431908 mpspy-0.1.2/mpspy/instance.py
+-rw-r--r--   0        0        0       52 2024-05-24 14:31:22.431908 mpspy-0.1.2/mpspy/log.py
+-rw-r--r--   0        0        0    10715 2024-05-24 14:31:22.431908 mpspy-0.1.2/mpspy/reader.py
+-rw-r--r--   0        0        0      387 2024-05-24 14:31:22.431908 mpspy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 mpspy-0.1.2/PKG-INFO
```

### Comparing `mpspy-0.1.1/LICENSE` & `mpspy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mpspy-0.1.1/mpspy/reader.py` & `mpspy-0.1.2/mpspy/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import gzip
 from collections import OrderedDict, defaultdict
 from enum import Enum, auto
 
 import numpy as np
 import scipy as sp
 
+from .instance import Instance, VarType
 from .log import logger
 
 
 class ReadError:
     def __init__(self, filename, line):
         self.filename = filename
         self.line = line
@@ -19,31 +20,14 @@
 
 class ConsType(Enum):
     LowerBound = auto()
     UpperBound = auto()
     Equation = auto()
 
 
-class VarType(Enum):
-    Integer = auto()
-    Continuous = auto()
-
-
-def run_once(func):
-    has_run = [False]
-
-    def wrapped_func(*args, **kwds):
-        if has_run[0]:
-            return
-        has_run[0] = True
-        return func(*args, **kwds)
-
-    return wrapped_func
-
-
 def default_cons_lb(cons_type):
     if cons_type == ConsType.UpperBound:
         return -np.inf
     else:
         return 0.0
 
 
@@ -82,44 +66,14 @@
         self.rhs = defaultdict(lambda: 0)
         self.var_types = dict()
         self.lower_bounds = OrderedDict()
         self.upper_bounds = OrderedDict()
         self.is_integer = False
 
 
-class Instance:
-    def __init__(self, var_lb, var_ub, var_types, obj, cons_lb, cons_ub, coeffs):
-
-        (self.num_cons, self.num_vars) = coeffs.shape
-
-        assert var_lb.shape == (self.num_vars,)
-        assert var_ub.shape == (self.num_vars,)
-        assert obj.shape == (self.num_vars,)
-
-        assert len(var_types) == self.num_vars
-
-        assert cons_lb.shape == (self.num_cons,)
-        assert cons_ub.shape == (self.num_cons,)
-
-        assert sp.sparse.issparse(coeffs)
-
-        self.var_lb = var_lb
-        self.var_ub = var_ub
-        self.var_type = var_types
-        self.obj = obj
-        self.cons_lb = cons_lb
-        self.cons_ub = cons_ub
-        self.coeffs = coeffs
-
-    def __str__(self):
-        return (
-            f"Instance with {self.num_vars} variables and {self.num_cons} constraints"
-        )
-
-
 def parse_row(tokens, state):
 
     assert len(tokens) == 2
 
     if tokens[0] == "N":
         if state.first_obj_name is None:
             state.first_obj_name = tokens[1]
@@ -380,17 +334,18 @@
         coeff_rows += [i] * num_coeffs
         coeff_data += cons_var_values
 
     coeffs = sp.sparse.coo_matrix(
         (coeff_data, (coeff_rows, coeff_cols)), shape=(num_cons, num_vars)
     )
 
+    name = state.name
     var_types = state.var_types
 
-    return Instance(var_lb, var_ub, var_types, obj, cons_lb, cons_ub, coeffs)
+    return Instance(name, var_lb, var_ub, var_types, obj, cons_lb, cons_ub, coeffs)
 
 
 def parse_line(section, tokens, state):
     assert section is not None
 
     if section == Section.ROWS:
         parse_row(tokens, state)
```

### Comparing `mpspy-0.1.1/PKG-INFO` & `mpspy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpspy
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
```

