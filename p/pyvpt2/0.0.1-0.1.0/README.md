# Comparing `tmp/pyvpt2-0.0.1.tar.gz` & `tmp/pyvpt2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvpt2-0.0.1.tar", last modified: Wed Apr 24 20:27:37 2024, max compression
+gzip compressed data, was "pyvpt2-0.1.0.tar", last modified: Fri May 24 14:11:12 2024, max compression
```

## Comparing `pyvpt2-0.0.1.tar` & `pyvpt2-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2024-04-24 20:27:37.497285 pyvpt2-0.0.1/
--rw-r--r--   0 philip    (1000) philip    (1000)     3555 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 philip    (1000) philip    (1000)     1464 2024-03-29 01:22:57.000000 pyvpt2-0.0.1/LICENSE
--rw-r--r--   0 philip    (1000) philip    (1000)      119 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/MANIFEST.in
--rw-r--r--   0 philip    (1000) philip    (1000)     1569 2024-04-24 20:27:37.497285 pyvpt2-0.0.1/PKG-INFO
--rw-r--r--   0 philip    (1000) philip    (1000)     1302 2024-03-29 01:22:57.000000 pyvpt2-0.0.1/README.md
--rw-r--r--   0 philip    (1000) philip    (1000)      759 2024-04-24 18:04:57.000000 pyvpt2-0.0.1/pyproject.toml
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2024-04-24 20:27:37.492285 pyvpt2-0.0.1/pyvpt2/
--rw-r--r--   0 philip    (1000) philip    (1000)      164 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/__init__.py
--rw-r--r--   0 philip    (1000) philip    (1000)      654 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/constants.py
--rw-r--r--   0 philip    (1000) philip    (1000)     4539 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/fermi_solver.py
--rw-r--r--   0 philip    (1000) philip    (1000)    23726 2024-04-11 17:31:05.000000 pyvpt2-0.0.1/pyvpt2/quartic.py
--rw-r--r--   0 philip    (1000) philip    (1000)     2369 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/schema.py
--rw-r--r--   0 philip    (1000) philip    (1000)    10630 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/task_base.py
--rw-r--r--   0 philip    (1000) philip    (1000)     5040 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/task_planner.py
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2024-04-24 20:27:37.496285 pyvpt2-0.0.1/pyvpt2/tests/
--rw-r--r--   0 philip    (1000) philip    (1000)      113 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/__init__.py
--rw-r--r--   0 philip    (1000) philip    (1000)     8377 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/test_fermi_solver.py
--rw-r--r--   0 philip    (1000) philip    (1000)     1832 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/test_h2co.py
--rw-r--r--   0 philip    (1000) philip    (1000)     1486 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/test_h2o.py
--rw-r--r--   0 philip    (1000) philip    (1000)     1337 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/test_h2o_cbs.py
--rw-r--r--   0 philip    (1000) philip    (1000)     1631 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/test_h2o_multilevel.py
--rw-r--r--   0 philip    (1000) philip    (1000)     2075 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/test_h2o_qcng.py
--rw-r--r--   0 philip    (1000) philip    (1000)     2054 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/test_h2o_snowflake.py
--rw-r--r--   0 philip    (1000) philip    (1000)     2509 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/test_h2o_snowflake2.py
--rw-r--r--   0 philip    (1000) philip    (1000)     1119 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/test_hcn.py
--rw-r--r--   0 philip    (1000) philip    (1000)     1325 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/test_hf.py
--rw-r--r--   0 philip    (1000) philip    (1000)     1525 2024-03-27 17:41:33.000000 pyvpt2-0.0.1/pyvpt2/tests/test_polyad.py
--rw-r--r--   0 philip    (1000) philip    (1000)    29246 2024-04-14 19:50:04.000000 pyvpt2-0.0.1/pyvpt2/vpt2.py
-drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2024-04-24 20:27:37.496285 pyvpt2-0.0.1/pyvpt2.egg-info/
--rw-r--r--   0 philip    (1000) philip    (1000)     1569 2024-04-24 20:27:37.000000 pyvpt2-0.0.1/pyvpt2.egg-info/PKG-INFO
--rw-r--r--   0 philip    (1000) philip    (1000)      691 2024-04-24 20:27:37.000000 pyvpt2-0.0.1/pyvpt2.egg-info/SOURCES.txt
--rw-r--r--   0 philip    (1000) philip    (1000)        1 2024-04-24 20:27:37.000000 pyvpt2-0.0.1/pyvpt2.egg-info/dependency_links.txt
--rw-r--r--   0 philip    (1000) philip    (1000)       26 2024-04-24 20:27:37.000000 pyvpt2-0.0.1/pyvpt2.egg-info/top_level.txt
--rw-r--r--   0 philip    (1000) philip    (1000)       38 2024-04-24 20:27:37.497285 pyvpt2-0.0.1/setup.cfg
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2024-05-24 14:11:12.132211 pyvpt2-0.1.0/
+-rw-r--r--   0 philip    (1000) philip    (1000)     3555 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 philip    (1000) philip    (1000)     1464 2024-03-29 01:22:57.000000 pyvpt2-0.1.0/LICENSE
+-rw-r--r--   0 philip    (1000) philip    (1000)      119 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/MANIFEST.in
+-rw-r--r--   0 philip    (1000) philip    (1000)     1725 2024-05-24 14:11:12.131211 pyvpt2-0.1.0/PKG-INFO
+-rw-r--r--   0 philip    (1000) philip    (1000)     1458 2024-04-30 12:49:20.000000 pyvpt2-0.1.0/README.md
+-rw-r--r--   0 philip    (1000) philip    (1000)      759 2024-04-24 18:04:57.000000 pyvpt2-0.1.0/pyproject.toml
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2024-05-24 14:11:12.127211 pyvpt2-0.1.0/pyvpt2/
+-rw-r--r--   0 philip    (1000) philip    (1000)      164 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/__init__.py
+-rw-r--r--   0 philip    (1000) philip    (1000)      654 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/constants.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     4539 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/fermi_solver.py
+-rw-r--r--   0 philip    (1000) philip    (1000)    23726 2024-04-11 17:31:05.000000 pyvpt2-0.1.0/pyvpt2/quartic.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     2509 2024-05-24 13:46:07.000000 pyvpt2-0.1.0/pyvpt2/schema.py
+-rw-r--r--   0 philip    (1000) philip    (1000)    10630 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/task_base.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     5040 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/task_planner.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2024-05-24 14:11:12.130211 pyvpt2-0.1.0/pyvpt2/tests/
+-rw-r--r--   0 philip    (1000) philip    (1000)      113 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/__init__.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     8377 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/test_fermi_solver.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     1832 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/test_h2co.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     1486 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/test_h2o.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     1337 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/test_h2o_cbs.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     1631 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/test_h2o_multilevel.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     2075 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/test_h2o_qcng.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     2054 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/test_h2o_snowflake.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     2509 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/test_h2o_snowflake2.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     1119 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/test_hcn.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     1325 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/test_hf.py
+-rw-r--r--   0 philip    (1000) philip    (1000)     1525 2024-03-27 17:41:33.000000 pyvpt2-0.1.0/pyvpt2/tests/test_polyad.py
+-rw-r--r--   0 philip    (1000) philip    (1000)    29246 2024-04-14 19:50:04.000000 pyvpt2-0.1.0/pyvpt2/vpt2.py
+drwxr-xr-x   0 philip    (1000) philip    (1000)        0 2024-05-24 14:11:12.130211 pyvpt2-0.1.0/pyvpt2.egg-info/
+-rw-r--r--   0 philip    (1000) philip    (1000)     1725 2024-05-24 14:11:12.000000 pyvpt2-0.1.0/pyvpt2.egg-info/PKG-INFO
+-rw-r--r--   0 philip    (1000) philip    (1000)      691 2024-05-24 14:11:12.000000 pyvpt2-0.1.0/pyvpt2.egg-info/SOURCES.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)        1 2024-05-24 14:11:12.000000 pyvpt2-0.1.0/pyvpt2.egg-info/dependency_links.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)       26 2024-05-24 14:11:12.000000 pyvpt2-0.1.0/pyvpt2.egg-info/top_level.txt
+-rw-r--r--   0 philip    (1000) philip    (1000)       38 2024-05-24 14:11:12.132211 pyvpt2-0.1.0/setup.cfg
```

### Comparing `pyvpt2-0.0.1/CODE_OF_CONDUCT.md` & `pyvpt2-0.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/LICENSE` & `pyvpt2-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/PKG-INFO` & `pyvpt2-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyvpt2
-Version: 0.0.1
+Version: 0.1.0
 Summary: Package to calculate VPT2 anharmonic frequencies.
 Author-email: Philip Nelson <pmnelson@gatech.edu>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pyVPT2
 ==============================
 [//]: # (Badges)
-![CI workflow](https://github.com/philipmnel/pyvpt2/actions/workflows/CI.yaml/badge.svg)
+[![CI](https://img.shields.io/github/actions/workflow/status/philipmnel/pyvpt2/CI.yaml?logo=github)](https://github.com/philipmnel/pyvpt2/actions?query=workflow%3ACI)
+[![Docs](https://img.shields.io/github/actions/workflow/status/philipmnel/pyvpt2/CI.yaml?label=docs&logo=readthedocs&logoColor=white)](https://philipmnel.github.io/pyvpt2/)
 [![codecov](https://codecov.io/gh/philipmnel/pyvpt2/branch/main/graph/badge.svg?token=goQRxdntmS)](https://codecov.io/gh/philipmnel/pyvpt2)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/philipmnel/pyvpt2/blob/main/LICENSE)
-[![Docs](https://img.shields.io/badge/Documentation-red)](https://philipmnel.github.io/pyvpt2/)
+
 
 ### About
 pyVPT2 is a package to calculate VPT2 vibrational frequencies using psi4 or qcengine. Cubic/quartic constants can be optionally computed in a distributed parallel fashion using QCFractal.
 
 For usage check the [documentation](https://philipmnel.github.io/pyvpt2/).
 
 Disclaimer: This codebase is still under active development.
```

### Comparing `pyvpt2-0.0.1/README.md` & `pyvpt2-0.1.0/pyvpt2.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,25 @@
+Metadata-Version: 2.1
+Name: pyvpt2
+Version: 0.1.0
+Summary: Package to calculate VPT2 anharmonic frequencies.
+Author-email: Philip Nelson <pmnelson@gatech.edu>
+License: BSD-3-Clause
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 pyVPT2
 ==============================
 [//]: # (Badges)
-![CI workflow](https://github.com/philipmnel/pyvpt2/actions/workflows/CI.yaml/badge.svg)
+[![CI](https://img.shields.io/github/actions/workflow/status/philipmnel/pyvpt2/CI.yaml?logo=github)](https://github.com/philipmnel/pyvpt2/actions?query=workflow%3ACI)
+[![Docs](https://img.shields.io/github/actions/workflow/status/philipmnel/pyvpt2/CI.yaml?label=docs&logo=readthedocs&logoColor=white)](https://philipmnel.github.io/pyvpt2/)
 [![codecov](https://codecov.io/gh/philipmnel/pyvpt2/branch/main/graph/badge.svg?token=goQRxdntmS)](https://codecov.io/gh/philipmnel/pyvpt2)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/philipmnel/pyvpt2/blob/main/LICENSE)
-[![Docs](https://img.shields.io/badge/Documentation-red)](https://philipmnel.github.io/pyvpt2/)
+
 
 ### About
 pyVPT2 is a package to calculate VPT2 vibrational frequencies using psi4 or qcengine. Cubic/quartic constants can be optionally computed in a distributed parallel fashion using QCFractal.
 
 For usage check the [documentation](https://philipmnel.github.io/pyvpt2/).
 
 Disclaimer: This codebase is still under active development.
```

### Comparing `pyvpt2-0.0.1/pyproject.toml` & `pyvpt2-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/constants.py` & `pyvpt2-0.1.0/pyvpt2/constants.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/fermi_solver.py` & `pyvpt2-0.1.0/pyvpt2/fermi_solver.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/quartic.py` & `pyvpt2-0.1.0/pyvpt2/quartic.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/schema.py` & `pyvpt2-0.1.0/pyvpt2/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,28 @@
     from pydantic import Field, conlist
 
 from qcelemental.models import Molecule
 from qcelemental.models.basemodels import ProtoModel
 from qcelemental.models.common_models import Model, Provenance
 from qcelemental.models.procedures import QCInputSpecification
 from qcelemental.models.types import Array
+from importlib.metadata import version, PackageNotFoundError
 
-#from pyvpt2 import __version__
-
+try:
+    __version__ = version("package-name")
+except PackageNotFoundError:
+    __version__ = "unknown"
 
 def provenance_stamp() -> Dict[str, str]:
     """
     Return provenance stamp for pyvpt2
     """
     provenance = {
         "creator": "pyVPT2",
-        "version": 0.0,
+        "version": __version__,
         "routine": "VPT2"
     }
     return provenance
 
 class VPTInput(ProtoModel):
     molecule: Molecule = Field(..., description="Input molecule")
     keywords: Dict[str, Any] = Field({}, description="pyVPT2 keywords")
```

### Comparing `pyvpt2-0.0.1/pyvpt2/task_base.py` & `pyvpt2-0.1.0/pyvpt2/task_base.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/task_planner.py` & `pyvpt2-0.1.0/pyvpt2/task_planner.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/tests/test_fermi_solver.py` & `pyvpt2-0.1.0/pyvpt2/tests/test_fermi_solver.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/tests/test_h2co.py` & `pyvpt2-0.1.0/pyvpt2/tests/test_h2co.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/tests/test_h2o.py` & `pyvpt2-0.1.0/pyvpt2/tests/test_h2o.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/tests/test_h2o_cbs.py` & `pyvpt2-0.1.0/pyvpt2/tests/test_h2o_cbs.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/tests/test_h2o_multilevel.py` & `pyvpt2-0.1.0/pyvpt2/tests/test_h2o_multilevel.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/tests/test_h2o_qcng.py` & `pyvpt2-0.1.0/pyvpt2/tests/test_h2o_qcng.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/tests/test_h2o_snowflake.py` & `pyvpt2-0.1.0/pyvpt2/tests/test_h2o_snowflake.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/tests/test_h2o_snowflake2.py` & `pyvpt2-0.1.0/pyvpt2/tests/test_h2o_snowflake2.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/tests/test_hcn.py` & `pyvpt2-0.1.0/pyvpt2/tests/test_hcn.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/tests/test_hf.py` & `pyvpt2-0.1.0/pyvpt2/tests/test_hf.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/tests/test_polyad.py` & `pyvpt2-0.1.0/pyvpt2/tests/test_polyad.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2/vpt2.py` & `pyvpt2-0.1.0/pyvpt2/vpt2.py`

 * *Files identical despite different names*

### Comparing `pyvpt2-0.0.1/pyvpt2.egg-info/SOURCES.txt` & `pyvpt2-0.1.0/pyvpt2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

