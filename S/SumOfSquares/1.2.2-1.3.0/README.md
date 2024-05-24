# Comparing `tmp/SumOfSquares-1.2.2.tar.gz` & `tmp/sumofsquares-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SumOfSquares-1.2.2.tar", last modified: Wed Jun 28 01:54:45 2023, max compression
+gzip compressed data, was "sumofsquares-1.3.0.tar", last modified: Fri May 24 21:02:59 2024, max compression
```

## Comparing `SumOfSquares-1.2.2.tar` & `sumofsquares-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-06-28 01:54:45.717245 SumOfSquares-1.2.2/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1053 2022-04-29 18:49:06.000000 SumOfSquares-1.2.2/LICENSE
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3327 2023-06-28 01:54:45.717245 SumOfSquares-1.2.2/PKG-INFO
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1337 2022-12-30 02:25:15.000000 SumOfSquares-1.2.2/README.md
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1440 2023-06-28 01:48:11.000000 SumOfSquares-1.2.2/pyproject.toml
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       38 2023-06-28 01:54:45.717245 SumOfSquares-1.2.2/setup.cfg
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-06-28 01:54:45.717245 SumOfSquares-1.2.2/src/
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-06-28 01:54:45.717245 SumOfSquares-1.2.2/src/SumOfSquares/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)    10368 2022-12-30 03:23:20.000000 SumOfSquares-1.2.2/src/SumOfSquares/SoS.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)      374 2021-05-19 18:31:44.000000 SumOfSquares-1.2.2/src/SumOfSquares/__init__.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     4988 2022-12-30 03:02:36.000000 SumOfSquares-1.2.2/src/SumOfSquares/basis.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1466 2021-05-19 19:14:03.000000 SumOfSquares-1.2.2/src/SumOfSquares/util.py
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-06-28 01:54:45.717245 SumOfSquares-1.2.2/src/SumOfSquares.egg-info/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3327 2023-06-28 01:54:45.000000 SumOfSquares-1.2.2/src/SumOfSquares.egg-info/PKG-INFO
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)      373 2023-06-28 01:54:45.000000 SumOfSquares-1.2.2/src/SumOfSquares.egg-info/SOURCES.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)        1 2023-06-28 01:54:45.000000 SumOfSquares-1.2.2/src/SumOfSquares.egg-info/dependency_links.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       64 2023-06-28 01:54:45.000000 SumOfSquares-1.2.2/src/SumOfSquares.egg-info/requires.txt
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)       13 2023-06-28 01:54:45.000000 SumOfSquares-1.2.2/src/SumOfSquares.egg-info/top_level.txt
-drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2023-06-28 01:54:45.717245 SumOfSquares-1.2.2/tests/
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)      813 2022-04-29 19:31:17.000000 SumOfSquares-1.2.2/tests/test_basis.py
--rw-r--r--   0 chenyang  (1000) chenyang  (1000)     7234 2022-12-30 03:23:50.000000 SumOfSquares-1.2.2/tests/test_sos.py
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-05-24 21:02:59.385918 sumofsquares-1.3.0/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1058 2024-03-15 02:34:02.000000 sumofsquares-1.3.0/LICENSE
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3863 2024-05-24 21:02:59.385918 sumofsquares-1.3.0/PKG-INFO
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1585 2024-05-23 01:15:22.000000 sumofsquares-1.3.0/README.md
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1455 2024-05-24 21:01:04.000000 sumofsquares-1.3.0/pyproject.toml
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       38 2024-05-24 21:02:59.385918 sumofsquares-1.3.0/setup.cfg
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-05-24 21:02:59.382585 sumofsquares-1.3.0/src/
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-05-24 21:02:59.382585 sumofsquares-1.3.0/src/SumOfSquares/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)    12894 2024-05-24 19:20:38.000000 sumofsquares-1.3.0/src/SumOfSquares/SoS.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)      410 2024-05-24 18:49:16.000000 sumofsquares-1.3.0/src/SumOfSquares/__init__.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     5935 2024-05-24 20:22:24.000000 sumofsquares-1.3.0/src/SumOfSquares/basis.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1767 2024-05-24 18:59:52.000000 sumofsquares-1.3.0/src/SumOfSquares/util.py
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-05-24 21:02:59.385918 sumofsquares-1.3.0/src/SumOfSquares.egg-info/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     3863 2024-05-24 21:02:59.000000 sumofsquares-1.3.0/src/SumOfSquares.egg-info/PKG-INFO
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)      373 2024-05-24 21:02:59.000000 sumofsquares-1.3.0/src/SumOfSquares.egg-info/SOURCES.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)        1 2024-05-24 21:02:59.000000 sumofsquares-1.3.0/src/SumOfSquares.egg-info/dependency_links.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       83 2024-05-24 21:02:59.000000 sumofsquares-1.3.0/src/SumOfSquares.egg-info/requires.txt
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)       13 2024-05-24 21:02:59.000000 sumofsquares-1.3.0/src/SumOfSquares.egg-info/top_level.txt
+drwxr-xr-x   0 chenyang  (1000) chenyang  (1000)        0 2024-05-24 21:02:59.385918 sumofsquares-1.3.0/tests/
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     1448 2024-05-24 19:04:13.000000 sumofsquares-1.3.0/tests/test_basis.py
+-rw-r--r--   0 chenyang  (1000) chenyang  (1000)     8304 2024-05-24 20:57:23.000000 sumofsquares-1.3.0/tests/test_sos.py
```

### Comparing `SumOfSquares-1.2.2/LICENSE` & `sumofsquares-1.3.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 Chenyang Yuan
+Copyright 2020-2024 Chenyang Yuan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `SumOfSquares-1.2.2/PKG-INFO` & `sumofsquares-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: SumOfSquares
-Version: 1.2.2
+Version: 1.3.0
 Summary: Python implementation of Sum-of-Squares optimization built on picos
 Author-email: Chenyang Yuan <yuanchenyang@gmail.com>
 Maintainer-email: Chenyang Yuan <yuanchenyang@gmail.com>
-License: Copyright 2022 Chenyang Yuan
+License: Copyright 2020-2024 Chenyang Yuan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
@@ -18,17 +18,26 @@
 Project-URL: Source, https://github.com/yuanchenyang/SumOfSquares.py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: ConvexHull
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: sympy
+Requires-Dist: picos
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Provides-Extra: convexhull
+Requires-Dist: scipy; extra == "convexhull"
 
 SumOfSquares.py
 ---------------
 | **Documentation** | **Build Status** |
 |:-----------------:|:----------------:|
 | [![][docs-latest-img]][docs-latest-url] | [![Build Status][build-img]][build-url] |
 
@@ -66,7 +75,19 @@
 
 [More Examples](https://sums-of-squares.github.io/sos/index.html#python)
 
 [docs-latest-img]: https://img.shields.io/badge/docs-latest-blue.svg
 [docs-latest-url]: https://sums-of-squares.github.io/sos/index.html#python
 [build-img]: https://github.com/yuanchenyang/SumOfSquares.py/workflows/CI/badge.svg?branch=master
 [build-url]: https://github.com/yuanchenyang/SumOfSquares.py/actions?query=workflow%3ACI
+
+### Citation
+If you use this library in your work, please consider citing:
+
+```
+@software{Yuan_SumOfSquares_py,
+author = {Yuan, Chenyang},
+license = {MIT},
+title = {{SumOfSquares.py}},
+url = {https://github.com/yuanchenyang/SumOfSquares.py}
+}
+```
```

### Comparing `SumOfSquares-1.2.2/pyproject.toml` & `sumofsquares-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SumOfSquares"
-version = "1.2.2"
+version = "1.3.0"
 description = "Python implementation of Sum-of-Squares optimization built on picos"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   {name = "Chenyang Yuan", email = "yuanchenyang@gmail.com" }
 ]
@@ -39,14 +39,14 @@
 [project.urls]
 "Homepage" = "https://github.com/yuanchenyang/SumOfSquares.py"
 "Bug Tracker" = "https://github.com/yuanchenyang/SumOfSquares.py/issues"
 "Documentation" = "https://sums-of-squares.github.io/sos/index.html#python"
 "Source" = "https://github.com/yuanchenyang/SumOfSquares.py"
 
 [project.optional-dependencies] # Optional
-#dev = []
+dev = ["build", "twine"]
 test = ["pytest", "pytest-cov"]
 ConvexHull = ["scipy"]
 
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
```

### Comparing `SumOfSquares-1.2.2/src/SumOfSquares/SoS.py` & `sumofsquares-1.3.0/src/SumOfSquares/SoS.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from __future__ import annotations # for type hinting
+
 import math
 import picos as pic
 import sympy as sp
 import numpy as np
 from picos import Problem
 from collections import defaultdict
 from operator import floordiv, and_
 from itertools import combinations
+from typing import List, Optional
 
 from .util import *
 from .basis import Basis, poly_variable
 
 class SOSProblem(Problem):
     '''Defines an Sum of Squares problem, a subclass of picos.Problem.
     (also see: https://gitlab.com/picos-api/picos/-/issues/138 for an
@@ -18,52 +21,62 @@
     def __init__(self, *args, **kwargs):
         '''Takes same arguments as picos.Problem
         '''
         Problem.__init__(self, *args, **kwargs)
         self._sym_var_map = {}
         self._sos_constraints = {}
         self._sos_const_count = 0
+        self._aux_var_count = 0
         self._pexpect_count = 0
 
-    def __getitem__(self, sym):
-        assert isinstance(sym, sp.Symbol), f'{s} must be a sympy symbol!'
+    def __getitem__(self, sym: sp.Symbol) -> pic.RealVariable:
+        assert isinstance(sym, sp.Symbol), f'{sym} must be a sympy symbol!'
         return self.sym_to_var(sym)
 
-    def sym_to_var(self, sym):
+    def sym_to_var(self, sym: sp.Symbol) -> pic.RealVariable:
         '''Map between a sympy symbol to a unique picos variable. As sympy
         symbols are hashable, each symbol is assigned a unique picos variable.
         A new picos variable is created if it previously doesn't exist.
         '''
         if sym not in self._sym_var_map:
             self._sym_var_map[sym] = pic.RealVariable(repr(sym))
         return self._sym_var_map[sym]
 
-    def sp_to_picos(self, expr):
+    def subs_with_sol(self, expr: sp.Expr) -> sp.Expr:
+        ''' Substitute symbols in sympy expression with values obtained from
+        solving the problem'''
+        syms_with_values = [(sym, var.value)
+                            for sym, var in self._sym_var_map.items()
+                            if var.value is not None]
+        return expr.subs(syms_with_values)
+
+    def sp_to_picos(self, expr: sp.Expr) -> pic.expressions.Expression:
         '''Converts a sympy affine expression to a picos expression, converting
         numeric values to floats, and sympy symbols to picos variables.
         '''
         if expr.func == sp.Symbol:
             return self.sym_to_var(expr)
         elif expr.func == sp.Add:
             return sum(map(self.sp_to_picos, expr.args))
         elif expr.func == sp.Mul:
             return prod(map(self.sp_to_picos, expr.args))
         else:
             return pic.Constant(float(expr))
 
-    def sp_mat_to_picos(self, mat):
+    def sp_mat_to_picos(self, mat: sp.Matrix) -> pic.expressions.Expression:
         '''Converts a sympy matrix a picos affine expression, converting
         numeric values to floats, and sympy symbols to picos variables.
         '''
         num_rows, num_cols = mat.shape
         # Use picos operator overloading
         return reduce(floordiv, [reduce(and_, map(self.sp_to_picos, mat.row(r)))
                                  for r in range(num_rows)])
 
-    def add_sos_constraint(self, expr, variables, name='', sparse=False):
+    def add_sos_constraint(self, expr: sp.Expr, variables: List[sp.Symbol],
+                           name: str='', sparse: bool=False) -> SOSConstraint:
         '''Adds a constraint that the polynomial EXPR is a Sum-of-Squares. EXPR
         is a sympy expression treated as a polynomial in VARIABLES. Any symbols
         in EXPR not in VARIABLES are converted to picos variables
         (see SOSProblem.sym_to_var). Can optionally name the constraint with
         NAME. SPARSE uses Newton polytope reduction to do computations in a
         reduced-size basis. Returns a SOSConstraint object.
         '''
@@ -82,15 +95,35 @@
         for mono, pairs in basis.sos_sym_entries.items():
             coeff = mono_to_coeffs.get(mono, 0)
             self.add_constraint(sum(Q[i,j] for i,j in pairs) == coeff)
 
         pic_const = self.add_constraint(Q >> 0)
         return SOSConstraint(pic_const, Q, basis, variables, deg)
 
-    def get_pexpect(self, variables, deg, hom=False, name=''):
+    def add_matrix_sos_constraint(self, mat: sp.Matrix, variables: List[sp.Symbol],
+                                  name: str='', sparse: bool=False, aux_var_name: str=''
+                                  ) -> SOSConstraint:
+        '''Adds a constraint that MAT is sum of squares. This is done by
+        defining a polynomial (using auxillary variables) that is sum of squares
+        iff MAT is a sum of squares matrix.
+        '''
+        n, m = mat.shape
+        assert n == m, 'Matrix must be square!'
+
+        self._aux_var_count += 1
+        aux_var_name = aux_var_name or f'_y{self._aux_var_count}'
+        aux_vars = list(sp.symbols(f'{aux_var_name}_:{n}'))
+
+        y = sp.Matrix([aux_vars])
+        p = (y @ mat @ y.T)[0] # p is sos iff mat is a sos matrix
+        return self.add_sos_constraint(p, aux_vars + variables, name=name, sparse=sparse)
+
+    def get_pexpect(self, variables: List[sp.Symbol], deg:int,
+                    hom: bool=False, name: str=''
+                    ) -> Callable[[sp.Expr], pic.expressions.Expression]:
         '''Returns a degree DEG pseudoexpectation operator. This operator is a
         function that takes in a polynomial of at most degree DEG in VARIABLES,
         and returns a picos affine expression. If HOM=True, this polynomial must
         also be homogeneous. This operator has the property that
         pexpect(p(x)^2) >= 0 for any suitable polynomial p(x).
 
         Since the return value of pexpect(p(x)) is a picos expression, it can be
@@ -117,15 +150,21 @@
 
         def pexpect(p):
             poly = sp.poly(p, variables)
             basis.check_can_represent(poly)
             return self.sp_mat_to_picos(basis.sos_sym_poly_repr(poly)) | X
         return pexpect
 
-def poly_opt_prob(vars, obj, eqs=None, ineqs=None, ineq_prods=False, deg=None, sparse=False):
+def poly_opt_prob(vars       : List[sp.Symbol],
+                  obj        : sp.Expr,
+                  eqs        : Optional[List[sp.Expr]] = None,
+                  ineqs      : Optional[List[sp.Expr]] = None,
+                  ineq_prods : bool = False,
+                  deg        : Optional[int] = None,
+                  sparse     : bool = False) -> SOSProblem:
     '''Formulates and returns a degree DEG Sum-of-Squares relaxation of a polynomial
     optimization problem in variables VARS that mininizes OBJ subject to
     equality constraints EQS (g(x) = 0) and inequality constraints INEQS (h(x)
     >= 0). INEQ_PRODS determines if products of inequalities are used. SPARSE
     uses Newton polytope reduction to do computations in a reduced-size
     basis. Returns an instance of SOSProblem.
 
@@ -157,15 +196,21 @@
                     f += s * prod(comb)
 
     # Much faster after using sp.expand
     prob.add_sos_constraint(sp.expand(obj - gamma - f), vars, sparse=sparse)
     prob.set_objective('max', gamma_p)
     return prob
 
-def poly_cert_prob(vars, poly, eqs=None, ineqs=None, ineq_prods=False, deg=None, sparse=False):
+def poly_cert_prob(vars       : List[sp.Symbol],
+                   poly       : sp.Expr,
+                   eqs        : Optional[List[sp.expr]] = None,
+                   ineqs      : Optional[List[sp.expr]] = None,
+                   ineq_prods : bool = False,
+                   deg        : Optional[int] = None,
+                   sparse     : bool = False) -> SOSProblem:
     '''Formulates and returns a degree DEG Sum-of-Squares relaxation of a polynomial
     optimization problem in variables VARS that certifies POLY is a sum of
     squares on the set defined by EQS and INEQS. INEQ_PRODS determines if
     products of inequalities are used. SPARSE uses Newton polytope reduction to
     do computations in a reduced-size basis. Returns an instance of SOSProblem.
 
     '''
@@ -199,15 +244,20 @@
 
 class SOSConstraint:
     '''Defines a Sum-of-Squares constraint, returned by
     SOSProblem.add_sos_constraint. Holds information about the SoS constraint
     and its dual, and allows one to compute the pseudoexpectation of any
     polynomial.
     '''
-    def __init__(self, pic_const, Q, basis, symbols, deg):
+    def __init__(self,
+                 pic_const: pic.constraints.Constraint,
+                 Q        : pic.expressions.variables.SymmetricVariable,
+                 basis    : Basis,
+                 symbols  : List[sp.Symbol],
+                 deg      : int):
         self.pic_const = pic_const
         self.Q = Q
         self.basis = basis
         self.symbols = symbols
         self.b_sym = basis.to_sym(symbols)
         self.deg = deg
 
@@ -216,28 +266,28 @@
         '''Optimization variable Q where p(x) = b^T Q b, where p(x) is polynomial
         constrained to be SoS, and b is the basis.'''
         if self.Q.value is None:
             raise ValueError('Missing value for sos constraint variable!'
                              ' (is the problem solved?)')
         return self.Q.value
 
-    def get_chol_factor(self):
+    def get_chol_factor(self) -> np.array:
         '''Returns L, the Cholesky factorization of Q = LL^T. Adds a small
         multiple of identity to Q if it has small negative eigenvalues.
         '''
         mineig = min(min(np.linalg.eigh(self.Qval)[0]), 0)
         return np.linalg.cholesky(self.Qval - np.eye(len(self.basis))*mineig*1.1)
 
-    def get_sos_decomp(self, precision=3):
+    def get_sos_decomp(self, precision: int=3) -> sp.Matrix:
         '''Returns a vector containing the sum of squares decompositon of this
         constraint'''
         L = sp.Matrix(self.get_chol_factor())
         S = (L.T @ sp.Matrix(self.b_sym)).applyfunc(lambda x: x**2)
         return round_sympy_expr(S, precision)
 
-    def pexpect(self, expr):
+    def pexpect(self, expr: sp.Expr) -> sp.Expr:
         '''Computes the pseudoexpectation of a given polynomial EXPR'''
         poly = sp.poly(expr, self.symbols)
         self.basis.check_can_represent(poly)
         Qp = self.basis.sos_sym_poly_repr(poly)
         X = sp.Matrix(len(self.basis), len(self.basis), self.pic_const.dual)
         return sum(sp.matrix_multiply_elementwise(X, Qp))
```

### Comparing `SumOfSquares-1.2.2/src/SumOfSquares/basis.py` & `sumofsquares-1.3.0/src/SumOfSquares/basis.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,66 @@
+from __future__ import annotations # for type hinting Basis
+
 import sympy as sp
 import numpy as np
 import math
 from collections import defaultdict
+from typing import Iterable, Tuple, List
 
 from .util import *
 
-def basis_hom(n, d):
+def basis_hom(n: int, d: int) -> Iterable[Tuple[int]]:
     '''Generator for a homogeneous polynomial basis for n variables of degree d,
     represented as a list of tuples (same as sympy), so that:
     len(list(basis_hom(n,d))) == binom(n+d-1, d)
     '''
     if n == 1:
         yield (d,)
     elif d == 0:
         yield (0,)*n
     else:
         for di in range(d+1):
             for b in basis_hom(n-1, di):
                 yield b + (d-di,)
 
-def basis_inhom(n, d):
+def basis_inhom(n: int, d: int) -> Iterable[Tuple[int]]:
     '''Generator for an inhomogeneous polynomial basis for n variables of
     degree d, represented as a list of tuples (same as sympy), so that:
     len(list(basis(n,d))) == binom(n+d, d)
     '''
     for b in basis_hom(n+1, d):
         yield b[:-1]
 
 class Basis():
-    def __init__(self, monoms):
+    def __init__(self, monoms: List[Tuple[int]]):
         '''Initializes a basis using a sequence of tuples representing monomials
         '''
         self.monoms = monoms
         self.deg = max(sum(m) for m in self.monoms)
         self.nvars = len(monoms[0])
         self.is_hom = sum(sum(m) != self.deg for m in self.monoms) == 0
 
         # A map from a monomial m (represented as tuple) to list of pairs (i, j)
         # for all such pairs where m = basis[i]*basis[j].
         self.sos_sym_entries = defaultdict(list)
         for i, bi in enumerate(self):
             for j, bj in enumerate(self):
                  self.sos_sym_entries[sum_tuple(bi, bj)].append((i, j))
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.monoms)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterable[Tuple[int]]:
         return iter(self.monoms)
 
-    def from_degree(nvars, deg, hom=False):
+    def from_degree(nvars: int, deg: int, hom: bool=False) -> Basis:
         '''Constructs a basis by specifying the number of variables and degree'''
         return Basis(list((basis_hom if hom else basis_inhom)(nvars, deg)))
 
-    def from_poly_lex(poly, sparse=True):
+    def from_poly_lex(poly: sp.Poly, sparse: bool=True) -> Basis:
         '''Returns a basis from a polynomial compatible with SoS,
         ordering monomials in lexicographic order'''
         poly_deg = poly.total_degree()
         monoms = np.array(poly.monoms())/2
         full_basis = Basis.from_degree(len(poly.gens), math.ceil(poly_deg / 2),
                                        is_hom(poly, poly_deg))
         if sparse and len(monoms) >= 3: # Newton polytope sparsity reduction
@@ -71,52 +74,67 @@
             hull = ConvexHull(np.apply_along_axis(proj, 1, monoms))
             def in_hull(pt): # Point lies in affine subspace and convex hull
                 return np.linalg.norm(proj_(pt)) < 1e-9 and \
                     sum(hull.equations.dot(np.append(proj(pt), 1)) > 1e-9) == 0
             return Basis(list(filter(in_hull, full_basis.monoms)))
         return full_basis
 
-    def to_sym(self, syms):
+    def to_sym(self, syms: List[sp.Expr]) -> List[sp.Expr]:
         '''Convert basis to a list of symbolic monomials
         '''
         if self.nvars != len(syms):
             raise ValueError('Mismatched basis size!')
         return [prod(s**m for s,m in zip(syms, mono)) for mono in self]
 
-    def check_can_represent(self, poly):
+    def check_can_represent(self, poly: sp.Poly):
         '''Check if sympy polynomial POLY can be represented by this basis.
         Raises an error otherwise.'''
         if poly.total_degree() > self.deg * 2:
            raise ValueError(f'Polynomial degree must be at most {self.deg*2}!')
 
         if self.is_hom and not is_hom(poly, self.deg * 2):
             raise ValueError(f'Polynomial must be homogeneous of degree {self.deg * 2}!')
 
         extra_monoms = len(set(poly.monoms()) - set(self.sos_sym_entries.keys()))
         if extra_monoms > 0:
             raise ValueError(f'{extra_monoms} monomials in polynomial'\
                              ' are not in basis!')
 
 
-    def sos_sym_poly_repr(self, poly):
+    def sos_sym_poly_repr(self, poly: sp.Poly) -> sp.Matrix:
         '''Given a polynomial p, returns a SoS-symmetric representation
         Qp where p(x) = b(x)^T Qp b(x), in terms of this basis.
         Qp is returned as a sympy matrix.
         '''
         Qp = sp.zeros(len(self), len(self))
         for monom, coeff in zip(poly.monoms(), poly.coeffs()):
             entries = self.sos_sym_entries[monom]
             for i, j in entries:
                 Qp[i,j] = coeff/len(entries)
         return Qp
 
 
-def poly_variable(name, variables, deg, hom=False):
+def poly_variable(name: str, variables: List[sp.Symbol], deg: int,
+                  hom: bool=False) -> sp.Expr:
     '''Returns a (possibly homogeneous) degree DEG polynomial in VARIABLES,
     with a variable (a sympy symbol) named using NAME for each coefficient. Used
     in Sum-of-Squares relaxations for polynomial optimization.
     '''
+    if hom and deg == 0:
+        return 0
     variables = sorted(variables, key=str) # use lex order
     basis = Basis.from_degree(len(variables), deg, hom=hom)
     coeffs = sp.symbols(f'{name}_:{len(basis)}')
     return sum(coeff * prod(var**power for var, power in zip(variables, monom))
                for monom, coeff in zip(basis, coeffs))
+
+def matrix_variable(name: str, variables: List[sp.Symbol], deg: int, dim: int,
+                    hom: bool=False, sym: bool=True) -> sp.Matrix:
+    '''Returns a (symmetric) matrix variable of size dim x dim'''
+    arr = [[None] * dim for _ in range(dim)]
+    for i in range(dim):
+        for j in range(dim):
+            if j < i and sym:
+                arr[i][j] = arr[j][i]
+            else:
+                arr[i][j] = poly_variable(f'{name}[{i}][{j}]', variables, deg, hom=hom)
+    return sp.Matrix(arr)
```

### Comparing `SumOfSquares-1.2.2/src/SumOfSquares/util.py` & `sumofsquares-1.3.0/src/SumOfSquares/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 import sympy as sp
 import numpy as np
 import math
 from operator import mul
 from functools import reduce
 from itertools import combinations
+from typing import Iterable, List, Optional, Tuple
 
 def prod(seq):
     return reduce(mul, seq, 1)
 
-def factorial(n):
+def factorial(n: int) -> int:
     return prod(range(1, n+1))
 
-def binom(n, d):
+def binom(n: int, d: int) -> int:
     assert n >= d, f'invalid binom({n}, {d})!'
     return factorial(n)//factorial(n-d)//factorial(d)
 
-def sum_tuple(t1, t2):
+def sum_tuple(t1: tuple, t2: tuple) -> tuple:
     return tuple(a1+a2 for a1, a2 in zip(t1, t2))
 
-def is_hom(poly, deg):
+def is_hom(poly: sp.Poly, deg: int) -> bool:
     '''Determines if a polynomial POLY is homogeneous of degree DEG'''
+    if deg == 0:
+        return poly == 0
     return sum(sum(m) != deg for m in poly.monoms()) == 0
 
-def round_sympy_expr(expr, precision=3):
+def round_sympy_expr(expr: sp.Expr, precision: int=3) -> sp.Expr:
     '''Rounds all numbers in a sympy expression to stated precision'''
     return expr.xreplace({n : round(n, precision) for n in expr.atoms(sp.Number)})
 
-def poly_degree(p, variables):
+def poly_degree(p: sp.Expr, variables: List[sp.Symbol]) -> int:
     '''Returns the max degree of P when treated as a polynomial in VARIABLES'''
     return sp.poly(p, variables).total_degree()
 
-def orth(M):
+def orth(M: np.array) -> Tuple[np.array, np.array]:
     _, D, V = np.linalg.svd(M)
     return V[D >= 1e-9], V[D < 1e-9]
 
-def get_poly_degree(vars, polys, deg=None):
+def get_poly_degree(vars, polys: List[sp.Poly], deg: Optional[int]=None) -> int:
     '''Given a vector of polynomials POLY, return minimum degree to run sum of
     squares, or check if DEG is above such minimum degree if provided'''
     max_deg = max(map(lambda p: poly_degree(p, vars), polys))
     if deg is None:
         deg = math.ceil(max_deg/2)
     if 2*deg < max_deg:
         raise ValueError(f'Degree of relaxation 2*{deg} less than maximum degree {max_deg}')
```

### Comparing `SumOfSquares-1.2.2/src/SumOfSquares.egg-info/PKG-INFO` & `sumofsquares-1.3.0/src/SumOfSquares.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: SumOfSquares
-Version: 1.2.2
+Version: 1.3.0
 Summary: Python implementation of Sum-of-Squares optimization built on picos
 Author-email: Chenyang Yuan <yuanchenyang@gmail.com>
 Maintainer-email: Chenyang Yuan <yuanchenyang@gmail.com>
-License: Copyright 2022 Chenyang Yuan
+License: Copyright 2020-2024 Chenyang Yuan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
@@ -18,17 +18,26 @@
 Project-URL: Source, https://github.com/yuanchenyang/SumOfSquares.py
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: ConvexHull
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: sympy
+Requires-Dist: picos
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Provides-Extra: convexhull
+Requires-Dist: scipy; extra == "convexhull"
 
 SumOfSquares.py
 ---------------
 | **Documentation** | **Build Status** |
 |:-----------------:|:----------------:|
 | [![][docs-latest-img]][docs-latest-url] | [![Build Status][build-img]][build-url] |
 
@@ -66,7 +75,19 @@
 
 [More Examples](https://sums-of-squares.github.io/sos/index.html#python)
 
 [docs-latest-img]: https://img.shields.io/badge/docs-latest-blue.svg
 [docs-latest-url]: https://sums-of-squares.github.io/sos/index.html#python
 [build-img]: https://github.com/yuanchenyang/SumOfSquares.py/workflows/CI/badge.svg?branch=master
 [build-url]: https://github.com/yuanchenyang/SumOfSquares.py/actions?query=workflow%3ACI
+
+### Citation
+If you use this library in your work, please consider citing:
+
+```
+@software{Yuan_SumOfSquares_py,
+author = {Yuan, Chenyang},
+license = {MIT},
+title = {{SumOfSquares.py}},
+url = {https://github.com/yuanchenyang/SumOfSquares.py}
+}
+```
```

### Comparing `SumOfSquares-1.2.2/tests/test_sos.py` & `sumofsquares-1.3.0/tests/test_sos.py`

 * *Files 10% similar despite different names*

```diff
@@ -179,9 +179,38 @@
         prob1.solve(solver=self.solver)
 
         # Infeasible when products of inequalities are not considered
         prob2 = poly_cert_prob([x,y], x*y, ineqs=[x, y, 1-x-y], ineq_prods=False, deg=1)
         with self.assertRaises(pic.SolutionFailure):
             prob2.solve(solver=self.solver)
 
+    def test_matrix_poly(self):
+        x, y = sp.symbols('x y')
+        n = 3
+        deg = 2
+
+        M = matrix_variable('M', [x, y], deg, n)
+        prob = SOSProblem()
+        prob.add_matrix_sos_constraint(sp.eye(n) - M, [x, y])
+        prob.set_objective('max', prob.sym_to_var(M[0].coeff(x**2)))
+        prob.solve(solver=self.solver)
+        self.assertAlmostEqual(prob.subs_with_sol(M)[0].coeff(x**2), 0, 7)
+
+        P = sp.Matrix([ [x**2-x*x+2, x], [x, x**2]])
+        prob = SOSProblem()
+        const = prob.add_matrix_sos_constraint(P, [x])
+        prob.solve()
+
+    def test_matrix_poly_infeasible(self):
+        x, y, z = sp.symbols('x y z')
+        choi_mat = sp.Matrix([
+            [x**2 + 2*y**2, -x*y         , -x*z         ],
+            [-x*y         , y**2 + 2*z**2, -y*z         ],
+            [-x*z         , -y*z         , z**2 + 2*x**2],
+        ])
+        prob = SOSProblem()
+        const = prob.add_matrix_sos_constraint(choi_mat, [x, y, z])
+        with self.assertRaises(pic.SolutionFailure):
+            prob.solve(solver=self.solver)
+
 if __name__ == '__main__':
     unittest.main()
```

