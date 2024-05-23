# Comparing `tmp/fenics-smart-2.1.7.tar.gz` & `tmp/fenics_smart-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics-smart-2.1.7.tar", last modified: Wed Oct 18 21:34:56 2023, max compression
+gzip compressed data, was "fenics_smart-2.2.0.tar", last modified: Thu May 23 21:38:23 2024, max compression
```

## Comparing `fenics-smart-2.1.7.tar` & `fenics_smart-2.2.0.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 21:34:56.219382 fenics-smart-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18504 2023-10-18 21:34:56.219382 fenics-smart-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 21:34:56.211382 fenics-smart-2.1.7/fenics_smart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18504 2023-10-18 21:34:56.000000 fenics-smart-2.1.7/fenics_smart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-10-18 21:34:56.000000 fenics-smart-2.1.7/fenics_smart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 21:34:56.000000 fenics-smart-2.1.7/fenics_smart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-10-18 21:34:56.000000 fenics-smart-2.1.7/fenics_smart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-18 21:34:56.000000 fenics-smart-2.1.7/fenics_smart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-18 21:34:56.219382 fenics-smart-2.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 21:34:56.215382 fenics-smart-2.1.7/smart/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11679 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16278 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    27643 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/mesh_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    89698 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    64824 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/model_assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)    20131 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11458 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/smart/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 21:34:56.215382 fenics-smart-2.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/tests/test_compartment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2023-10-18 21:34:36.000000 fenics-smart-2.1.7/tests/test_species.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:23.796665 fenics_smart-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18559 2024-05-23 21:38:23.796665 fenics_smart-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:23.792665 fenics_smart-2.2.0/fenics_smart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18559 2024-05-23 21:38:23.000000 fenics_smart-2.2.0/fenics_smart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-23 21:38:23.000000 fenics_smart-2.2.0/fenics_smart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:38:23.000000 fenics_smart-2.2.0/fenics_smart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-23 21:38:23.000000 fenics_smart-2.2.0/fenics_smart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 21:38:23.000000 fenics_smart-2.2.0/fenics_smart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:38:23.796665 fenics_smart-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:23.792665 fenics_smart-2.2.0/smart/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11679 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18259 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62546 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/mesh_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95853 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73607 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/model_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20776 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/smart/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:23.792665 fenics_smart-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/tests/test_compartment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/tests/test_curv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/tests/test_mesh_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-23 21:38:14.000000 fenics_smart-2.2.0/tests/test_species.py
```

### Comparing `fenics-smart-2.1.7/LICENSE` & `fenics_smart-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.7/PKG-INFO` & `fenics_smart-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-smart
-Version: 2.1.7
+Version: 2.2.0
 Summary: Spatial Modeling Algorithms for Reactions and Transport (SMART) is a high-performance finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes in biological cells.
 Author-email: Justin Laughlin <justinglaughlin@gmail.com>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         
@@ -66,19 +66,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.16.0
 Requires-Dist: pandas
 Requires-Dist: Pint
 Requires-Dist: scipy>=1.1.0
 Requires-Dist: sympy
-Requires-Dist: dataclasses
 Requires-Dist: cached-property
 Requires-Dist: tabulate
 Requires-Dist: termcolor
-Requires-Dist: termplotlib
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: docs
 Requires-Dist: jupyter-book==0.15.1; extra == "docs"
 Requires-Dist: sphinx-autoapi==2.0.1; extra == "docs"
 Requires-Dist: astroid<3; extra == "docs"
@@ -98,14 +96,15 @@
 Requires-Dist: fenics-smart[pyvista]; extra == "all"
 
 [![Test fenics_smart](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml)
 [![PyPI](https://img.shields.io/pypi/v/fenics-smart)](https://pypi.org/project/fenics-smart/)
 [![Deploy static content to Pages](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml)
 [![pre-commit](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10019463.svg)](https://doi.org/10.5281/zenodo.10019463)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05580/status.svg)](https://doi.org/10.21105/joss.05580)
 # Spatial Modeling Algorithms for Reaction-Transport [systems|models|equations]
 
 ## Statement of Need
 
 *Spatial Modeling Algorithms for Reactions and Transport* (SMART) is a finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes,
 especially tailored to modeling such systems within biological cells.
 SMART is based on the [FEniCS finite element library](https://fenicsproject.org/), provides a symbolic representation
@@ -186,15 +185,15 @@
 Upon pushing new code to the SMART repository, a number of tests run:
 * pre-commit tests.
     - Install `pre-commit`: `python3 -m pip install pre-commit`
     - Run pre-commit hooks: `pre-commit run --all`
 * unit tests (can be found in `tests` folder): test initialization of compartment, species, and parameter objects.
     - Install test dependencies: `python3 -m pip install fenics-smart[test]`. Alternatively, if you have already installed SMART, you can install `pytest` and `pytest-cov` using `python3 -m pip install pytest pytest-cov`.
     - Run tests from the root of the repository: `python3 -m pytest`
-* Examples 1-6: All 6 examples are run when building the docs. These serve as Contiuous Integration (CI) tests; within each run, there is a regression test comparing the output values from the simulation with values obtained from a previous build of SMART. Outputs from examples 2 and 3 are also compared to analytical solutions to demonstrate the accuracy of SMART simulations.
+* Examples 1-6: All 6 examples are run when building the docs. These serve as Continuous Integration (CI) tests; within each run, there is a regression test comparing the output values from the simulation with values obtained from a previous build of SMART. Outputs from examples 2 and 3 are also compared to analytical solutions to demonstrate the accuracy of SMART simulations.
 * Example 2 - 3D
 * Example 3 with MPI: Example 3 is run using MPI to run differently sized meshes in parallel (each process is assigned a single mesh).
 
 ## Contributing guidelines
 
 Detailed contributing guidelines are given [here](https://rangamanilabucsd.github.io/smart/CONTRIBUTING.html).
```

### Comparing `fenics-smart-2.1.7/README.md` & `fenics_smart-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [![Test fenics_smart](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml)
 [![PyPI](https://img.shields.io/pypi/v/fenics-smart)](https://pypi.org/project/fenics-smart/)
 [![Deploy static content to Pages](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml)
 [![pre-commit](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10019463.svg)](https://doi.org/10.5281/zenodo.10019463)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05580/status.svg)](https://doi.org/10.21105/joss.05580)
 # Spatial Modeling Algorithms for Reaction-Transport [systems|models|equations]
 
 ## Statement of Need
 
 *Spatial Modeling Algorithms for Reactions and Transport* (SMART) is a finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes,
 especially tailored to modeling such systems within biological cells.
 SMART is based on the [FEniCS finite element library](https://fenicsproject.org/), provides a symbolic representation
@@ -87,15 +88,15 @@
 Upon pushing new code to the SMART repository, a number of tests run:
 * pre-commit tests.
     - Install `pre-commit`: `python3 -m pip install pre-commit`
     - Run pre-commit hooks: `pre-commit run --all`
 * unit tests (can be found in `tests` folder): test initialization of compartment, species, and parameter objects.
     - Install test dependencies: `python3 -m pip install fenics-smart[test]`. Alternatively, if you have already installed SMART, you can install `pytest` and `pytest-cov` using `python3 -m pip install pytest pytest-cov`.
     - Run tests from the root of the repository: `python3 -m pytest`
-* Examples 1-6: All 6 examples are run when building the docs. These serve as Contiuous Integration (CI) tests; within each run, there is a regression test comparing the output values from the simulation with values obtained from a previous build of SMART. Outputs from examples 2 and 3 are also compared to analytical solutions to demonstrate the accuracy of SMART simulations.
+* Examples 1-6: All 6 examples are run when building the docs. These serve as Continuous Integration (CI) tests; within each run, there is a regression test comparing the output values from the simulation with values obtained from a previous build of SMART. Outputs from examples 2 and 3 are also compared to analytical solutions to demonstrate the accuracy of SMART simulations.
 * Example 2 - 3D
 * Example 3 with MPI: Example 3 is run using MPI to run differently sized meshes in parallel (each process is assigned a single mesh).
 
 ## Contributing guidelines
 
 Detailed contributing guidelines are given [here](https://rangamanilabucsd.github.io/smart/CONTRIBUTING.html).
```

### Comparing `fenics-smart-2.1.7/fenics_smart.egg-info/PKG-INFO` & `fenics_smart-2.2.0/fenics_smart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenics-smart
-Version: 2.1.7
+Version: 2.2.0
 Summary: Spatial Modeling Algorithms for Reactions and Transport (SMART) is a high-performance finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes in biological cells.
 Author-email: Justin Laughlin <justinglaughlin@gmail.com>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
         
@@ -66,19 +66,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.16.0
 Requires-Dist: pandas
 Requires-Dist: Pint
 Requires-Dist: scipy>=1.1.0
 Requires-Dist: sympy
-Requires-Dist: dataclasses
 Requires-Dist: cached-property
 Requires-Dist: tabulate
 Requires-Dist: termcolor
-Requires-Dist: termplotlib
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: docs
 Requires-Dist: jupyter-book==0.15.1; extra == "docs"
 Requires-Dist: sphinx-autoapi==2.0.1; extra == "docs"
 Requires-Dist: astroid<3; extra == "docs"
@@ -98,14 +96,15 @@
 Requires-Dist: fenics-smart[pyvista]; extra == "all"
 
 [![Test fenics_smart](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/test_fenics_smart.yml)
 [![PyPI](https://img.shields.io/pypi/v/fenics-smart)](https://pypi.org/project/fenics-smart/)
 [![Deploy static content to Pages](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/build_docs.yml)
 [![pre-commit](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/RangamaniLabUCSD/smart/actions/workflows/pre-commit.yml)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10019463.svg)](https://doi.org/10.5281/zenodo.10019463)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05580/status.svg)](https://doi.org/10.21105/joss.05580)
 # Spatial Modeling Algorithms for Reaction-Transport [systems|models|equations]
 
 ## Statement of Need
 
 *Spatial Modeling Algorithms for Reactions and Transport* (SMART) is a finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes,
 especially tailored to modeling such systems within biological cells.
 SMART is based on the [FEniCS finite element library](https://fenicsproject.org/), provides a symbolic representation
@@ -186,15 +185,15 @@
 Upon pushing new code to the SMART repository, a number of tests run:
 * pre-commit tests.
     - Install `pre-commit`: `python3 -m pip install pre-commit`
     - Run pre-commit hooks: `pre-commit run --all`
 * unit tests (can be found in `tests` folder): test initialization of compartment, species, and parameter objects.
     - Install test dependencies: `python3 -m pip install fenics-smart[test]`. Alternatively, if you have already installed SMART, you can install `pytest` and `pytest-cov` using `python3 -m pip install pytest pytest-cov`.
     - Run tests from the root of the repository: `python3 -m pytest`
-* Examples 1-6: All 6 examples are run when building the docs. These serve as Contiuous Integration (CI) tests; within each run, there is a regression test comparing the output values from the simulation with values obtained from a previous build of SMART. Outputs from examples 2 and 3 are also compared to analytical solutions to demonstrate the accuracy of SMART simulations.
+* Examples 1-6: All 6 examples are run when building the docs. These serve as Continuous Integration (CI) tests; within each run, there is a regression test comparing the output values from the simulation with values obtained from a previous build of SMART. Outputs from examples 2 and 3 are also compared to analytical solutions to demonstrate the accuracy of SMART simulations.
 * Example 2 - 3D
 * Example 3 with MPI: Example 3 is run using MPI to run differently sized meshes in parallel (each process is assigned a single mesh).
 
 ## Contributing guidelines
 
 Detailed contributing guidelines are given [here](https://rangamanilabucsd.github.io/smart/CONTRIBUTING.html).
```

### Comparing `fenics-smart-2.1.7/pyproject.toml` & `fenics_smart-2.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [build-system] # Require setuptool version due to https://github.com/pypa/setuptools/issues/2938
 requires = ["setuptools>=61.0.0", "wheel"]
 
 [project]
 name = "fenics-smart"
-version = "2.1.7"
+version = "2.2.0"
 description = "Spatial Modeling Algorithms for Reactions and Transport (SMART) is a high-performance finite-element-based simulation package for model specification and numerical simulation of spatially-varying reaction-transport processes in biological cells."
 authors = [{ name = "Justin Laughlin", email = "justinglaughlin@gmail.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "numpy>=1.16.0",
     "pandas",
     "Pint",
     "scipy>=1.1.0",
     "sympy",
-    "dataclasses",
     "cached-property",
     "tabulate",
     "termcolor",
-    "termplotlib",
 ]
 
 
 [project.urls]
 homepage = "https://rangamanilabucsd.github.io/smart"
 repository = "https://github.com/RangamaniLabUCSD/smart"
```

### Comparing `fenics-smart-2.1.7/smart/common.py` & `fenics_smart-2.2.0/smart/common.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.7/smart/config.py` & `fenics_smart-2.2.0/smart/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,15 @@
             "level": "DEBUG",
             # Don't send it up my namespace for additional handling
             "propagate": False,
         },
         "pint": {"level": "ERROR"},
         "FFC": {"level": "WARNING"},
         "UFL": {"level": "WARNING"},
+        "UFL_LEGACY": {"level": "WARNING"},
         "dolfin": {"level": "INFO"},
         "dijitso": {"level": "INFO"},
     },
     "root": {"handlers": ["root_console"], "level": "INFO"},
 }
 
 
@@ -298,17 +299,17 @@
         "sinh": ufl.sinh,
         "tanh": ufl.tanh,
         "acos": d.acos,
         "asin": d.asin,
         "atan": d.atan,
         "atan2": ufl.atan_2,
         "sqrt": d.sqrt,
-        "ln": d.ln,
+        "log": d.ln,
         "abs": ufl.algebra.Abs,
-        "sign": ufl.sign,
+        "dsign": ufl.sign,
         "pi": d.pi,
         "erf": d.erf,
     },
 }
 
 
 class BaseConfig:
@@ -370,18 +371,20 @@
     """
     Various flags
 
     Args:
         allow_unused_components: Allow parameters not defined in any reaction to be
             defined in any model.
         print_verbose_info: Print detailed information about a model
+        axisymmetric_model: 2D mesh describes an axisymmetric geometry about the axis r = 0
     """
 
     allow_unused_components: bool = False
     print_verbose_info: bool = True
+    axisymmetric_model: bool = False
 
 
 @dataclass
 class Config:
     """
     Configuration settings.
```

### Comparing `fenics-smart-2.1.7/smart/deprecation.py` & `fenics_smart-2.2.0/smart/deprecation.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.7/smart/mesh.py` & `fenics_smart-2.2.0/smart/mesh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Wrapper around dolfin mesh class to define parent and child meshes for SMART simulations.
 """
 from typing import Dict, FrozenSet
 import logging
-
+from pathlib import Path
 import dolfin as d
 import numpy as np
 from cached_property import cached_property
 
 
 logger = logging.getLogger(__name__)
 
@@ -53,14 +53,15 @@
     @property
     def is_surface(self):
         return self.dimensionality < self.parent_mesh.max_dim
 
     # Number of entities
     def get_num_entities(self, dimension):
         "Get the number of entities in this mesh with a certain topological dimension"
+        self.dolfin_mesh.init(dimension)
         return self.dolfin_mesh.topology().size(dimension)
 
     @cached_property
     def num_cells(self):
         return self.get_num_entities(self.dimensionality)
 
     @cached_property
@@ -143,42 +144,67 @@
 
     Args:
         mesh_filename (str): Name of mesh file
         mesh_filetype (str): Extension of mesh, either 'xml' or 'hdf5'
         parent_mesh (str): Name of mesh
         use_partition (bool): If `hdf5` mesh file is loaded,
           choose if mesh should be read in with its current partition
+        curvature (MeshFunction): either provided as a MeshFunction or given
+          as an xml or xdmf file containing a vertex mesh function of type double
+        extra_keys (list): list of names of extra keys to load from hdf5 mesh
+          file, specifying other subdomains besides main compartments (optional)
     """
 
     mesh_filename: str
     mesh_filetype: str
     child_meshes: Dict[str, "ChildMesh"]
     parent_mesh: "ParentMesh"
     use_partition: bool
+    curvature: d.MeshFunction
+    extra_keys: list = []
 
     def __init__(
         self,
         mesh_filename: str,
         mesh_filetype,
         name,
         use_partition=False,
         mpi_comm=d.MPI.comm_world,
+        curvature=None,
+        extra_keys=[],
     ):
         super().__init__(name)
         self.use_partition = use_partition
         self.mpi_comm = mpi_comm
+        self.extra_keys = extra_keys
         if mesh_filetype == "xml":
+            if len(self.extra_keys) > 0:
+                raise NotImplementedError("Loading extra keys from xml not implemented")
             self.load_mesh_from_xml(mesh_filename)
         elif mesh_filetype == "hdf5":
             self.load_mesh_from_hdf5(mesh_filename, use_partition)
         self.mesh_filename = mesh_filename
         self.mesh_filetype = mesh_filetype
 
         self.child_meshes = dict()
         self.parent_mesh = self
+        if isinstance(curvature, (str, Path)) and Path(curvature).is_file():
+            # Load curvature from file
+            if Path(curvature).suffix == ".xdmf":
+                self.curvature = d.MeshFunction("double", self.dolfin_mesh, 0)
+                with d.XDMFFile(str(curvature)) as curv_file:
+                    curv_file.read(self.curvature)
+            elif Path(curvature).suffix == ".xml":
+                self.curvature = d.MeshFunction("double", self.dolfin_mesh, str(curvature))
+                self.curvature.array()[np.where(self.curvature.array() > 1e9)[0]] = 0
+            else:
+                raise TypeError(f"Unable to read curvatures from {Path(curvature).suffix} file")
+        else:
+            # Otherwise just take what we got
+            self.curvature = curvature
 
     def get_mesh_from_id(self, id):
         "Find the mesh that has the matching id."
         # find the mesh in that has the matching id
         for mesh in self.all_meshes.values():
             if mesh.id == id:
                 return mesh
@@ -207,22 +233,36 @@
         # mesh, mfs = common.read_hdf5(hdf5_filename)
         self.dolfin_mesh = d.Mesh(comm)
         hdf5 = d.HDF5File(self.dolfin_mesh.mpi_comm(), mesh_filename, "r")
         hdf5.read(self.dolfin_mesh, "/mesh", use_partition)
 
         if comm.size > 1:
             d.MPI.comm_world.Barrier()
-        hdf5.close()
 
         self.dimensionality = self.dolfin_mesh.topology().dim()
         self.dolfin_mesh.init(self.dimensionality - 1)
         self.dolfin_mesh.init(self.dimensionality - 1, self.dimensionality)
 
         logger.info(f'HDF5 mesh, "{self.name}", successfully loaded from file: {mesh_filename}!')
 
+        # if extra keys are provided, load these as subdomains
+        self.subdomains = []
+        mesh = self.dolfin_mesh
+        if len(self.extra_keys) > 0:
+            for key in self.extra_keys:
+                cur_dim = int(key[-1])
+                mf_cur = d.MeshFunction("size_t", mesh, cur_dim)
+                hdf5.read(mf_cur, f"/{key}")
+                self.subdomains.append(mf_cur)
+        hdf5.close()
+
+        logger.info(
+            f"{len(self.subdomains)} subdomains successfully loaded from file: {mesh_filename}!"
+        )
+
     def _read_parent_mesh_function_from_file(self, dim):
         if self.mesh_filetype == "xml":
             mf = d.MeshFunction("size_t", self.dolfin_mesh, dim, value=self.dolfin_mesh.domains())
         elif self.mesh_filetype == "hdf5":
             mf = d.MeshFunction("size_t", self.dolfin_mesh, dim, value=0)
             # with d.HDF5File(self.dolfin_mesh.mpi_comm(), self.mesh_filename, 'r') as hdf5:
             # hdf5.read(mf, f'/mesh/{dim}')
@@ -427,15 +467,15 @@
             0
         ]  # indices of our cells that intersect
         # indices of parent facets that intersect
         parent_indices = mesh_to_parent[indices]
         self.intersection_map_parent[mesh_id_set].array()[parent_indices] = 1
 
     def get_intersection_submesh(self, mesh_id_set: FrozenSet[int]):
-        self.intersection_submesh[mesh_id_set] = d.MeshView.create(
+        self.intersection_submesh[mesh_id_set] = d.create_meshview(
             self.intersection_map_parent[mesh_id_set], 1
         )
         self.intersection_submesh[mesh_id_set].init()
         self.intersection_dx[mesh_id_set] = d.Measure("dx", self.intersection_submesh[mesh_id_set])
 
     def set_parent_mesh(self, parent_mesh):
         # remove existing parent mesh if not None
@@ -445,8 +485,8 @@
         self.parent_mesh = parent_mesh
         # add self to parent mesh's list of children meshes
         if self.parent_mesh:
             self.parent_mesh.child_meshes.update({self.name: self})
 
     def extract_submesh(self):
         mf_type = "cells" if self.is_volume else "facets"
-        self.dolfin_mesh = d.MeshView.create(self.parent_mesh.mf[mf_type], self.primary_marker)
+        self.dolfin_mesh = d.create_meshview(self.parent_mesh.mf[mf_type], self.primary_marker)
```

### Comparing `fenics-smart-2.1.7/smart/model.py` & `fenics_smart-2.2.0/smart/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,48 +4,54 @@
 from collections import OrderedDict as odict
 from dataclasses import dataclass
 from decimal import Decimal
 from itertools import chain
 import logging
 
 import dolfin as d
+from dolfin.common.timer import timed
 import numpy as np
 import pandas
 import petsc4py.PETSc as PETSc
 import sympy as sym
 from cached_property import cached_property
 from sympy.parsing.sympy_parser import parse_expr
 from tabulate import tabulate
+from scipy import integrate
+from sympy.utilities.lambdify import lambdify
+from pathlib import Path
+import re
 
 try:
     from ufl_legacy.algorithms.ad import expand_derivatives
     from ufl_legacy.form import sub_forms_by_domain
 except ImportError:
     from ufl.algorithms.ad import expand_derivatives
     from ufl.form import sub_forms_by_domain
 
-from .common import Stopwatch
-from .common import sub
+from .common import Stopwatch, sub
 from .config import Config
 from .mesh import ChildMesh, ParentMesh
 from .model_assembly import (
     Compartment,
     CompartmentContainer,
     FluxContainer,
     Form,
     FormContainer,
     Parameter,
     ParameterContainer,
     Reaction,
     ReactionContainer,
     Species,
     SpeciesContainer,
+    create_restriction,
     empty_sbmodel,
     ParameterType,
 )
+
 from .solvers import smartSNESProblem
 from .units import unit
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -181,14 +187,17 @@
         if self.mpi_size > 1:
             logger.info(
                 f"CPU {self.mpi_rank}: Model '{self.name}' "
                 f"has been parallelized (size={self.mpi_size}).",
                 extra=dict(format_type="log_urgent"),
             )
 
+        # Initialize load_init_time for use in loading initial conditions from file
+        self.load_init_time = None
+
     @property
     def mpi_am_i_root(self):
         """Returns True if current process is root"""
         return self.mpi_rank == self.mpi_root
 
     @property
     def child_meshes(self):
@@ -206,26 +215,27 @@
     def max_dim(self):
         """Returns maximum dimension in current model"""
         dim = max([comp.dimensionality for comp in self.cc])
         self.max_dim = dim
         self.parent_mesh.max_dim = dim
         return dim
 
+    @timed("Initialize Model")
     def initialize(self, initialize_solver=True):
         """Main model initialization function, split into 5 subfunctions"""
 
         # Solver related parameters
         self._base_t = Decimal("0." + (self.config.solver["time_precision"] - 1) * "0" + "1")
         self.t = self.rounded_decimal(0.0)
         self.dt = self.rounded_decimal(self.config.solver["initial_dt"])
         self.final_t = self.rounded_decimal(self.config.solver["final_t"])
         assert self.config.solver["time_precision"] in range(1, 30)
 
-        self.T = d.Constant(self.t)
-        self.dT = d.Constant(self.dt)
+        self.T = d.Constant(self.t, name="t")
+        self.dT = d.Constant(self.dt, name="dT")
         self.tvec = [self.t]
         self.dtvec = [self.dt]
 
         self._init_1()
         self._init_2()
         self._init_3()
         self._init_4()
@@ -235,28 +245,32 @@
         if self.config.flags["print_verbose_info"]:
             self.pc.print()
             self.sc.print()
             self.cc.print()
             self.print_meshes()
             self.rc.print()
 
+    @timed("Initialize model step 1")
     def _init_1(self):
         """Checking validity of model"""
+
         logger.debug("Checking validity of model (step 1 of ZZ)", extra=dict(format_type="title"))
         self._init_1_1_check_mesh_dimensionality()
         self._init_1_2_check_namespace_conflicts()
         self._init_1_3_check_parameter_dimensionality()
         logger.debug(
             "Step 1 of initialization completed successfully!",
             extra=dict(text_color="magenta"),
         )
 
+    @timed("Initialize model step 2")
     def _init_2(self):
         """Cross-container dependent initializations
         (requires information from multiple containers)"""
+
         logger.debug(
             "Cross-Container Dependent Initializations (step 2 of ZZ)",
             extra=dict(
                 format_type="title",
             ),
         )
         self._init_2_1_reactions_to_symbolic_strings()
@@ -267,14 +281,15 @@
         self._init_2_6_link_species_to_compartments()
         self._init_2_7_get_species_compartment_indices()
         logger.debug(
             "Step 2 of initialization completed " "successfully!",
             extra=dict(text_color="magenta"),
         )
 
+    @timed("Initialize model step 3")
     def _init_3(self):
         """Mesh-related initializations"""
         logger.debug(
             "Mesh-related Initializations (step 3 of ZZ)",
             extra=dict(format_type="title"),
         )
         self._init_3_1_define_child_meshes()
@@ -286,26 +301,29 @@
         # self._init_3_6_get_intersection_submeshes()
         self._init_3_7_get_integration_measures()
         logger.debug(
             "Step 3 of initialization completed successfully!",
             extra=dict(format_type="log_important"),
         )
 
+    @timed("Initialize model step 4")
     def _init_4(self):
         """Dolfin function initializations"""
+
         logger.debug("Dolfin Initializations (step 4 of ZZ)", extra=dict(format_type="title"))
         self._init_4_0_initialize_dolfin_parameters()
         self._init_4_1_get_active_compartments()
         self._init_4_2_define_dolfin_function_spaces()
         self._init_4_3_define_dolfin_functions()
         self._init_4_4_get_species_u_v_V_dofmaps()
         self._init_4_5_name_functions()
         self._init_4_6_check_dolfin_function_validity()
         self._init_4_7_set_initial_conditions()
 
+    @timed("Initialize model step 5")
     def _init_5(self, initialize_solver):
         """Convert reactions to fluxes and define variational form.
         If initialize_solver is true, also initialize solver.
         """
         logger.debug(
             "Dolfin fluxes, forms, and problems+solvers (step 5 of ZZ)",
             extra=dict(
@@ -452,14 +470,20 @@
                 if reaction.eqn_r_str:
                     reaction.eqn_r_str = reaction._parse_custom_reaction(reaction.eqn_r_str)
 
             else:
                 raise ValueError(
                     "Reaction %s does not seem to have an associated equation" % reaction.name
                 )
+            if reaction.eqn_f_str == "":
+                reaction.eqn_str = f"-{reaction.eqn_r_str}"
+            elif reaction.eqn_r_str == "":
+                reaction.eqn_str = f"{reaction.eqn_f_str}"
+            else:
+                reaction.eqn_str = f"{reaction.eqn_f_str}-{reaction.eqn_r_str}"
 
     def _init_2_2_check_reaction_validity(self):
         """Confirms that all reactions have parameters/species defined"""
         logger.debug(
             "Make sure all reactions have parameters/species defined",
             extra=dict(format_type="log"),
         )
@@ -468,20 +492,28 @@
             for eqn_str in [reaction.eqn_f_str, reaction.eqn_r_str]:
                 if not eqn_str:
                     continue
                 eqn = parse_expr(eqn_str)
                 var_set = {str(x) for x in eqn.free_symbols}
                 param_set = var_set.intersection(self.pc.keys)
                 species_set = var_set.intersection(self.sc.keys)
-                if len(param_set) + len(species_set) != len(var_set):
-                    diff_set = var_set.difference(param_set.union(species_set))
-                    raise NameError(
-                        f"Reaction {reaction.name} refers to a parameter or "
-                        f"species ({diff_set}) that is not in the model."
-                    )
+                if "curv" in var_set:
+                    if len(param_set) + len(species_set) + 1 != len(var_set):
+                        diff_set = var_set.difference(param_set.union(species_set))
+                        raise NameError(
+                            f"Reaction {reaction.name} refers to a parameter or "
+                            f"species ({diff_set}) that is not in the model."
+                        )
+                else:
+                    if len(param_set) + len(species_set) != len(var_set):
+                        diff_set = var_set.difference(param_set.union(species_set))
+                        raise NameError(
+                            f"Reaction {reaction.name} refers to a parameter or "
+                            f"species ({diff_set}) that is not in the model."
+                        )
 
     def _init_2_3_link_reaction_properties(self):
         """Link parameters, species, and compartments to reactions"""
         logger.debug(
             "Linking parameters, species, and compartments to reactions",
             extra=dict(format_type="log"),
         )
@@ -711,23 +743,28 @@
         Therefore, once the model is initialized, changing a parameter's
         value does not change the underlying dolfin object.
         Values must be assigned via :code:`parameter.dolfin_constant.assign()`
         """
         # Create a dolfin.Constant() for constant parameters
         for parameter in self.pc.values:
             if parameter.type == ParameterType.constant:
-                parameter.dolfin_constant = d.Constant(parameter.value)
+                parameter.dolfin_constant = d.Constant(parameter.value, name=parameter.name)
+            elif parameter.type == ParameterType.expression and parameter.is_space_dependent:
+                # use higher degree to avoid interpolation error
+                parameter.dolfin_expression = d.Expression(
+                    sym.printing.ccode(parameter.sym_expr), t=self.T, degree=3
+                )
             elif parameter.type == ParameterType.expression and not parameter.use_preintegration:
                 parameter.dolfin_expression = d.Expression(
                     sym.printing.ccode(parameter.sym_expr), t=self.T, degree=1
                 )
             elif parameter.type == ParameterType.expression and parameter.use_preintegration:
-                parameter.dolfin_constant = d.Constant(parameter.value)
+                parameter.dolfin_constant = d.Constant(parameter.value, name=parameter.name)
             elif parameter.type == ParameterType.from_file:
-                parameter.dolfin_constant = d.Constant(parameter.value)
+                parameter.dolfin_constant = d.Constant(parameter.value, name=parameter.name)
 
     def _init_4_1_get_active_compartments(self):
         """Arrange the compartments based on the number of degrees of freedom they have
         (We want to have the highest number of dofs first)
         """
         # addressing https://github.com/justinlaughlin/smart/issues/36
         self._active_compartments = list(self.cc.Dict.values())
@@ -781,14 +818,22 @@
                     dim=compartment.num_species,
                 )
             else:
                 compartment.V = d.FunctionSpace(
                     self.child_meshes[compartment.name].dolfin_mesh, "P", 1
                 )
 
+            if self.parent_mesh.curvature is not None:
+                scalarFunctionSpace = d.FunctionSpace(
+                    self.child_meshes[compartment.name].dolfin_mesh, "P", 1
+                )
+                compartment.curv_func = self.mf0_to_fun(
+                    self.parent_mesh.curvature, scalarFunctionSpace
+                )
+
         self.V = [compartment.V for compartment in self._active_compartments]
         # Make the MixedFunctionSpace
         self.W = d.MixedFunctionSpace(*self.V)
 
     def _init_4_3_define_dolfin_functions(self):
         """Define test functions and trial functions in the mixed function space
 
@@ -939,19 +984,29 @@
                     species.initial_condition, str
                 ):
                     self.dolfin_set_function_values(species, ukey, species.initial_condition)
                 else:
                     self.dolfin_set_function_values(
                         species, ukey, species.initial_condition_expression
                     )
+                if species.has_subdomain:
+                    # restrict to specified subdomain
+                    u_cur = self.cc[species.compartment_name].u[ukey]
+                    u_new = create_restriction(u_cur, species.subdomain_data, species.subdomain_val)
+                    values = u_cur.vector().get_local()
+                    values_new = u_new.vector().get_local()
+                    values[species.dof_map] = values_new[species.dof_map]
+                    u_cur.vector().set_local(values)
+                    u_cur.vector().apply("insert")
 
     def _init_5_1_reactions_to_fluxes(self):
         """Convert reactions to flux objects"""
         logger.debug("Convert reactions to flux objects", extra=dict(format_type="log"))
         for reaction in self.rc:
+            reaction.axisymm = self.config.flags["axisymmetric_model"]
             reaction.reaction_to_fluxes()
             self.fc.add(reaction.fluxes)
 
     def _init_5_2_create_variational_forms(self):
         """
         Setup the variational forms in dolfin
         Forms:
@@ -987,67 +1042,84 @@
                     flux_form_units,
                     True,
                     linearity_dict,
                 )
             )
 
         for species in self.sc:
+            x = d.SpatialCoordinate(species.compartment.dolfin_mesh)
             u = species._usplit["u"]
             # ut = species.ut
             # un = species.u['n']
             un = species._usplit["n"]
             v = species.v
             D = species.D
             dx = species.compartment.mesh.dx
+            Dform_units = (
+                species.diffusion_units
+                * species.concentration_units
+                * species.compartment.compartment_units ** (species.compartment.dimensionality - 2)
+            )
+            mass_form_units = (
+                species.concentration_units
+                / unit.s
+                * species.compartment.compartment_units**species.compartment.dimensionality
+            )
             # diffusion term
             if species.D == 0:
                 logger.debug(
                     f"Species {species.name} has a diffusion coefficient of 0. "
                     "Skipping creation of diffusive form.",
                     extra=dict(format_type="log"),
                 )
             else:
-                Dform = D * d.inner(d.grad(u), d.grad(v)) * dx
+                if Dform_units != mass_form_units:  # unit conversion for consistency
+                    diffusion_conversion = species.diffusion_units.to(
+                        species.compartment.compartment_units**2 / unit.s
+                    )
+                    D *= diffusion_conversion.magnitude
+                D_constant = d.Constant(D, name=f"D_{species.name}")
+                if self.config.flags["axisymmetric_model"]:
+                    Dform = x[0] * D_constant * d.inner(d.grad(u), d.grad(v)) * dx
+                else:
+                    Dform = D_constant * d.inner(d.grad(u), d.grad(v)) * dx
                 # exponent is -2 because of two gradients
-                Dform_units = (
-                    species.diffusion_units
-                    * species.concentration_units
-                    * species.compartment.compartment_units
-                    ** (species.compartment.dimensionality - 2)
-                )
+
                 self.forms.add(
                     Form(
                         f"diffusion_{species.name}",
                         Dform,
                         species,
                         "diffusion",
                         Dform_units,
                         True,
                         linear_wrt_comp,
                     )
                 )
+
             # mass (time derivative) terms
-            Muform = (u) * v / self.dT * dx
-            mass_form_units = (
-                species.concentration_units
-                / unit.s
-                * species.compartment.compartment_units**species.compartment.dimensionality
-            )
+            if self.config.flags["axisymmetric_model"]:
+                Muform = x[0] * (u) * v / self.dT * dx
+            else:
+                Muform = (u) * v / self.dT * dx
             self.forms.add(
                 Form(
                     f"mass_u_{species.name}",
                     Muform,
                     species,
                     "mass_u",
                     mass_form_units,
                     True,
                     linear_wrt_comp,
                 )
             )
-            Munform = (-un) * v / self.dT * dx
+            if self.config.flags["axisymmetric_model"]:
+                Munform = x[0] * (-un) * v / self.dT * dx
+            else:
+                Munform = (-un) * v / self.dT * dx
             self.forms.add(
                 Form(
                     f"mass_un_{species.name}",
                     Munform,
                     species,
                     "mass_un",
                     mass_form_units,
@@ -1127,14 +1199,15 @@
             self.problem = smartSNESProblem(
                 self.u["u"],
                 self.Fblocks_all,
                 self.Jblocks_all,
                 self._active_compartments,
                 self._all_compartments,
                 self.stopwatches,
+                self,
             )
 
             self.problem.init_petsc_matnest()
             self.problem.init_petsc_vecnest()
             if len(self.problem.global_sizes) == 1:
                 self._ubackend = u[0].vector().vec().copy()
             else:
@@ -1238,101 +1311,18 @@
             Ib0 = Fb0.integrals()[0].integrand()
             # (ufl.Indexed(Argument))) vs ufl.Indexed(ListTensor(ufl.Indexed(Argument)))
             I0.ufl_operands[0] == Ib0.ufl_operands[0] -> False
             I0.ufl_operands[1] == Ib0.ufl_operands[1] -> True
             I0.ufl_operands[0] == Ib0.ufl_operands[0](1) -> True
         """
 
-        # blocks/partitions are by compartment, not species
-        Fblock = d.extract_blocks(Fsum)
-
-        # =====================================================================
-        # doflin.fem.problem.MixedNonlinearVariationalProblem()
-        # =====================================================================
-        # basically is a wrapper around the cpp class that finalizes preparing
-        # F and J into the right format
-        # TODO: add dirichlet BCs
-
-        # Add in placeholders for empty blocks of F
-        if len(Fblock) != len(u):
-            Ftemp = [None for i in range(len(u))]
-            for Fi in Fblock:
-                Ftemp[Fi.arguments()[0].part()] = Fi
-            Fblock = Ftemp
-
-        # debug attempt
-        J = []
-        for Fi in Fblock:
-            for uj in u:
-                if Fi is None:
-                    # pass
-                    J.append(None)
-                else:
-                    dFdu = expand_derivatives(d.derivative(Fi, uj))
-                    J.append(dFdu)
-
-        # Check number of blocks in the residual and solution are coherent
-        assert len(J) == len(u) * len(u)
-        assert len(Fblock) == len(u)
-
-        # Decompose F blocks into subforms based on domain of integration
-        # Fblock = [F0, F1, ... , Fn] where the index is the compartment index
-        # Flist  = [[F0(Omega_0), F0(Omega_1)], ..., [Fn(Omega_n)]]
-        # If a form has integrals on multiple domains, they are split into a list
-        Flist = list()
-        for idx, Fi in enumerate(Fblock):
-            if Fi is None or Fi.empty():
-                logger.warning(
-                    f"F{idx} = F[{self.cc.get_index(idx).name}]) is empty",
-                    extra=dict(format_type="warning"),
-                )
-                Flist.append([d.cpp.fem.Form(1, 0)])
-            else:
-                Fs = []
-                for Fsub in sub_forms_by_domain(Fi):
-                    if Fsub is None or Fsub.empty():
-                        domain = self.get_mesh_by_id(Fsub.mesh().id()).name
-                        logger.warning(
-                            f"F{idx} = F[{self.cc.get_index(idx).name}] "
-                            "is empty on integration domain {domain}",
-                            extra=dict(format_type="logred"),
-                        )
-                        Fs.append(d.cpp.fem.Form(1, 0))
-                    else:
-                        Fs.append(d.Form(Fsub))
-                Flist.append(Fs)
-
-        # Decompose J blocks into subforms based on domain of integration
-        Jlist = list()
-        for idx, Ji in enumerate(J):
-            idx_i, idx_j = divmod(idx, len(u))
-            if Ji is None or Ji.empty():
-                logger.warning(
-                    f"J{idx_i}{idx_j} = dF[{self.cc.get_index(idx_i).name}])"
-                    f"/du[{self.cc.get_index(idx_j).name}] is empty",
-                    extra=dict(format_type="logred"),
-                )
-                Jlist.append([d.cpp.fem.Form(2, 0)])
-            else:
-                Js = []
-                for Jsub in sub_forms_by_domain(Ji):
-                    if Jsub is None or Jsub.empty():
-                        domain = self.get_mesh_by_id(Jsub.mesh().id()).name
-                        logger.warning(
-                            f"J{idx_i}{idx_j} = dF[{self.cc.get_index(idx_i).name}])"
-                            f"/du[{self.cc.get_index(idx_j).name}]"
-                            f"is empty on integration domain {domain}",
-                            extra=dict(format_type="logred"),
-                        )
-                    Js.append(d.Form(Jsub))
-                Jlist.append(Js)
-
+        Flist = self.get_block_F(Fsum, u)
+        Jlist = self.get_block_J(Fsum, u)
         global_sizes = [uj.function_space().dim() for uj in u]
 
-        # return Flist, Jlist
         return Flist, Jlist, global_sizes
 
     def get_global_sizes(self, u):
         """Return total number of dof for current model"""
         return [uj.function_space().dim() for uj in u]
 
     def get_block_F(self, Fsum, u):
@@ -1350,33 +1340,34 @@
             Fblock = Ftemp
 
         assert len(Fblock) == len(u)
         # Decompose F blocks into subforms based on domain of integration
         # Fblock = [F0, F1, ... , Fn] where the index is the compartment index
         # Flist  = [[F0(Omega_0), F0(Omega_1)], ..., [Fn(Omega_n)]]
         # If a form has integrals on multiple domains, they are split into a list
+        # If Fi(Omega_j) is not defined, None is inserted
         Flist = list()
         for idx, Fi in enumerate(Fblock):
             if Fi is None or Fi.empty():
                 logger.warning(
                     f"F{idx} = F[{self.cc.get_index(idx).name}]) is empty",
                     extra=dict(format_type="warning"),
                 )
-                Flist.append([d.cpp.fem.Form(1, 0)])
+                Flist.append([None])
             else:
                 Fs = []
                 for Fsub in sub_forms_by_domain(Fi):
                     if Fsub is None or Fsub.empty():
                         domain = self.get_mesh_by_id(Fsub.mesh().id()).name
                         logger.warning(
                             f"F{idx} = F[{self.cc.get_index(idx).name}] is empty "
                             f"on integration domain {domain}",
                             extra=dict(format_type="logred"),
                         )
-                        Fs.append(d.cpp.fem.Form(1, 0))
+                        Fs.append(None)
                     else:
                         Fs.append(d.Form(Fsub))
                 Flist.append(Fs)
 
         return Flist
 
     def get_block_J(self, Fsum, u):
@@ -1574,14 +1565,17 @@
         if not self._failed_to_converge:
             # check if there is a manually prescribed time-step size
             self.adjust_dt_if_prescribed()
             self.adjust_dt_if_pass_tfinal()  # adjust dt so that it doesn't pass tfinal
         if self.dt <= 0:
             raise ValueError("dt is <= 0")
 
+        # update equation variables (necessary for mass conservation workaround)
+        for fname, f in self.fc.items:
+            f.equation_variables.update()
         # Take a step forward in time and update time-dependent parameters
         # update time-dependent parameters
 
         # march forward in time and update time-dependent parameters
         self.forward_time_step()
         logger.info(
             f"Beginning time-step {self.idx} [time={self.t}, dt={self.dt}]",
@@ -1592,15 +1586,16 @@
         )
         self.update_time_dependent_parameters()
         if self.config.solver["use_snes"]:
             logger.info("Solving using PETSc.SNES Solver", dict(format_type="log"))
             self.stopwatches["snes all"].start()
 
             # Solve
-            self.solver.solve(None, self._ubackend)
+            with PETSc.Log.Event("solve"):
+                self.solver.solve(None, self._ubackend)
 
             # Store/compute timings
             logger.info(
                 f"Completed time-step {self.idx} [time={self.t}, dt={self.dt}]",
                 extra=dict(
                     new_lines=[1, 0],
                     format_type="solverstep",
@@ -1788,15 +1783,15 @@
             self.dtvec,
         ]:  # , self.residuals]:
             data.pop()
         # Undo the solution to the previous time-step
         self.update_solution(ukeys=["u"], unew="n")
 
     def update_time_dependent_parameters(self):
-        r"""
+        """
         Updates all time dependent parameters. Time-dependent parameters are
         either defined either symbolically or through a data file, and each of
         these can either be defined as a direct function of :math:`t, p(t)`, or a
         "pre-integrated expression", :math:`\int_{t_n}^{t_{n+1}} P(\tau) d\tau`, which allows for
         exact integration when the expression the parameter appears in doesn't rely
         on any other time-dependet variables. This may be useful for guaranteeing
         a certain amount of flux independent of time-stepping.
@@ -1848,28 +1843,46 @@
                     # We never want time to extrapolate beyond the provided data.
                     if t < t_data[0] or t > t_data[-1]:
                         raise Exception("Parameter cannot be extrapolated beyond provided data.")
                     # Just in case... return a nan if value is outside of bounds
                     new_value = float(np.interp(t, t_data, p_data, left=np.nan, right=np.nan))
                     logger.debug(
                         f"Time-dependent parameter {parameter_name} updated by data. "
-                        "New value is {new_value}",
+                        f"New value is {new_value}",
                         extra=dict(format_type="log"),
                     )
 
             if parameter.use_preintegration:
                 if parameter.type == ParameterType.expression:
-                    a = parameter.preint_sym_expr.subs({"t": tn}).evalf()
-                    b = parameter.preint_sym_expr.subs({"t": t}).evalf()
-                    new_value = float((b - a) / dt)
-                    logger.debug(
-                        f"Time-dependent parameter {parameter_name} updated by "
-                        "pre-integrated expression. New value is {new_value}",
-                        extra=dict(format_type="log"),
-                    )
+                    if parameter.preint_sym_expr is None:  # then numerically approximate integral
+                        a = parameter.int_vec[-1]
+                        tsym = sym.symbols("t")
+                        intval, err = integrate.quad(lambdify(tsym, parameter.sym_expr), tn, t)
+                        b = a + intval
+                        parameter.int_vec.append(b)
+                    else:
+                        a = parameter.preint_sym_expr.subs({"t": tn}).evalf()
+                        b = parameter.preint_sym_expr.subs({"t": t}).evalf()
+                    if parameter.is_space_dependent:
+                        parameter.dolfin_expression = d.Expression(
+                            sym.printing.ccode((b - a) / dt), degree=3
+                        )
+                        logger.debug(
+                            f"Time-dependent parameter {parameter_name} updated by "
+                            f"pre-integrated expression",
+                            extra=dict(format_type="log"),
+                        )
+                        continue
+                    else:
+                        new_value = float((b - a) / dt)
+                        logger.debug(
+                            f"Time-dependent parameter {parameter_name} updated by "
+                            f"pre-integrated expression. New value is {new_value}",
+                            extra=dict(format_type="log"),
+                        )
                 if parameter.type == ParameterType.from_file:
                     int_data = parameter.preint_sampling_data
                     a = np.interp(tn, int_data[:, 0], int_data[:, 1], left=np.nan, right=np.nan)
                     b = np.interp(t, int_data[:, 0], int_data[:, 1], left=np.nan, right=np.nan)
                     new_value = float((b - a) / dt)
                     logger.debug(
                         f"Time-dependent parameter {parameter_name} updated by "
@@ -1931,20 +1944,95 @@
     def dolfin_set_function_values(self, sp, ukey, unew):
         """Set values for dolfin function (usually for initial condition)
         Input unew should either be an expression giving the spatial dependence
         of u, a constant (float), or a vector of values.
         :code:`d.assign(uold, unew)` works when uold is a subfunction
         :code:`uold.assign(unew)` does not (it will replace the entire function)
         """
-        if isinstance(unew, d.Expression):
+        if isinstance(unew, str):
+            # then this still needs to have free symbols inserted
+            x, y, z = (sym.Symbol(f"x[{i}]") for i in range(3))
+            # Parse the given string to create a sympy expression
+            sym_expr = parse_expr(unew).subs({"x": x, "y": y, "z": z})
+            free_symbols = [str(x) for x in sym_expr.free_symbols]
+            if not {"x[0]", "x[1]", "x[2]", "curv"}.issuperset(free_symbols):
+                # could add other keywords for spatial dependence in the future
+                raise NotImplementedError
+            else:
+                x = d.SpatialCoordinate(sp.compartment.dolfin_mesh)
+                curv = sp.compartment.curv_func
+                full_expr = d.Expression(sym.printing.ccode(sym_expr), curv=curv, degree=1)
+                ufunc = d.interpolate(full_expr, sp.V)
+                d.assign(sp.u[ukey], ufunc)
+        elif isinstance(unew, d.Expression):
             uinterp = d.interpolate(unew, sp.V)
             d.assign(sp.u[ukey], uinterp)
         elif isinstance(unew, (float, int)):
             uinterp = d.interpolate(d.Constant(unew), sp.V)
             d.assign(sp.u[ukey], uinterp)
+        elif isinstance(unew, Path):
+            assert Path(
+                unew
+            ).is_file(), f"{str(unew)} could not be found for loading initial conditions"
+            logger.debug(f"Loading initial condition for {sp.name} from file")
+            if unew.suffix == ".h5":
+                h5Cur = str(unew)
+                xdmfCur = h5Cur[0:-2] + "xdmf"
+            elif unew.suffix == ".xdmf":
+                xdmfCur = str(unew)
+                h5Cur = xdmfCur[0:-4] + "h5"
+            else:
+                raise TypeError(
+                    f"{str(unew)} is an unrecognized file type for loading initial conditions"
+                )
+
+            # load the time vec from xdmf file
+            xdmf_file = open(xdmfCur, "r")
+            xdmf_string = xdmf_file.read()
+            found_pattern = re.findall(r"Time Value=\"?[^\s]+", xdmf_string)
+            tVec = []
+            for i in range(len(found_pattern)):
+                tVec.append(float(found_pattern[i][12:-1]))
+            if self.load_init_time is None:
+                if len(tVec) == 0:
+                    raise ValueError(f"Could not load time from {xdmfCur}")
+                elif len(tVec) == 1:
+                    self.load_init_time = tVec[0]
+                    self.load_init_idx = 0
+                else:
+                    self.load_init_time = tVec[-2]
+                    self.load_init_idx = len(tVec) - 2
+                # set to current time
+                self.t = self.rounded_decimal(self.load_init_time)
+                self.T.assign(self.t)
+
+            assert np.isclose(
+                tVec[self.load_init_idx], self.load_init_time
+            ), "Time value does not match load in value"
+
+            cur_file = d.HDF5File(self.parent_mesh.mpi_comm, h5Cur, "r")
+            if not cur_file.has_dataset(f"VisualisationVector/{self.load_init_idx}"):
+                raise TypeError(
+                    f"Unable to read initial condition for {sp.name} from file {str(unew)}"
+                )
+            start_vec = d.Vector()
+            cur_file.read(start_vec, f"VisualisationVector/{self.load_init_idx}", True)
+            cur_file.close()
+            vec = self.cc[sp.compartment_name].u[ukey].vector()
+            orig_vals = vec.get_local()
+            start_vals = start_vec.get_local()
+            mesh_map = d.dof_to_vertex_map(sp.V)[:]
+            start_vals = start_vals[mesh_map]  # reorder to match dof ordering
+            if len(start_vals) != len(sp.dof_map):
+                raise ValueError(
+                    f"Vector from {str(unew)} does not match function space for {sp.name}"
+                )
+            orig_vals[sp.dof_map] = start_vals
+            vec.set_local(orig_vals)
+            vec.apply("insert")
         elif len(sp.dof_map) == len(unew):
             # unew must be an N x 4 array: [X, Y, Z, function_values]
             u = self.cc[sp.compartment_name].u[ukey]
             dof_coord = sp.V.tabulate_dof_coordinates()  # coordinates for the current dof
             mesh_coord = unew[:, 0:3]  # x,y,z coordinates for initial condition
             function_values = unew[:, 3]
             # nearest neighbor interpolation
@@ -2070,7 +2158,44 @@
                     df = pandas.concat([df, tempseries.to_frame().T], ignore_index=True)
 
             print(tabulate(df, headers="keys", tablefmt=tablefmt))
 
     def rounded_decimal(self, x):
         """Round time value to specified decimal point"""
         return Decimal(x).quantize(self._base_t)
+
+    def mf0_to_fun(self, mf0, V):
+        """
+        Convert vertex mesh function over parent mesh to a dolfin function
+        over a single compartment.
+        """
+        dfunc = d.Function(V)
+        mesh_ref = self.parent_mesh.dolfin_mesh
+        bmesh = V.mesh()
+        store_map = bmesh.topology().mapping()[mesh_ref.id()].vertex_map()
+        values = dfunc.vector().get_local()
+        for j in range(len(store_map)):
+            cur_sub_idx = d.vertex_to_dof_map(V)[j]
+            values[cur_sub_idx] = mf0.array()[store_map[j]]
+        dfunc.vector().set_local(values)
+        dfunc.vector().apply("insert")
+        return dfunc
+
+    def adjust_dt(self):
+        if self.idx_nl[-1] in [0, 1]:
+            dt_scale = 1.1
+        elif self.idx_nl[-1] in [2, 3, 4]:
+            dt_scale = 1.05
+        elif self.idx_nl[-1] in [5, 6, 7, 8, 9, 10]:
+            dt_scale = 1.0
+        # decrease time step
+        elif self.idx_nl[-1] in [11, 12, 13, 14, 15, 16, 17, 18, 19, 20]:
+            dt_scale = 0.8
+        elif self.idx_nl[-1] >= 20:
+            dt_scale = 0.5
+        # further adjustments depending on linear iterations
+        # if self.idx_l[-1] <= 5 and dt_scale >= 1.0:
+        #     dt_scale *= 1.05
+        # if self.idx_l[-1] >= 10:
+        #     dt_scale = min(dt_scale * 0.8, 0.8)
+        dt_cur = float(self.dt) * dt_scale
+        self.set_dt(dt_cur)
```

### Comparing `fenics-smart-2.1.7/smart/model_assembly.py` & `fenics_smart-2.2.0/smart/model_assembly.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Classes for parameters, species, compartments, reactions, fluxes, and forms.
 Model class contains functions to efficiently solve a system.
 """
 import dataclasses
 import logging
 import numbers
-import sys
 from collections import OrderedDict as odict
 from dataclasses import dataclass
 from enum import Enum
 from pprint import pformat
 from textwrap import wrap
 from typing import Any, List, Optional, Union
 import warnings
@@ -23,17 +22,19 @@
     import ufl_legacy as ufl
 except ImportError:
     import ufl
 from cached_property import cached_property
 from sympy import Symbol, integrate
 from sympy.parsing.sympy_parser import parse_expr
 from tabulate import tabulate
+from pathlib import Path
 
 from . import common
 from .config import global_settings as gset
+from .config import base_format
 from .units import quantity_to_unit, unit, unit_to_quantity
 
 __all__ = [
     "empty_sbmodel",
     "sbmodel_from_locals",
     "Compartment",
     "Parameter",
@@ -214,43 +215,100 @@
 
         return df
 
     def print_to_latex(
         self,
         properties_to_print=None,
         max_col_width=None,
-        sig_figs=2,
-        return_df=True,
+        sig_figs=3,
+        return_df=False,
     ):
         """
         Print object properties in latex format.
         Requires latex packages :code:`\siunitx` and :code:`\longtable`
         """
 
         df = self.get_pandas_dataframe_formatted(
             properties_to_print=properties_to_print,
             max_col_width=max_col_width,
             sig_figs=sig_figs,
         )
+        df = df.copy(deep=True)
 
         # Change certain df entries to best format for display
-        for col in df.columns:
-            # Convert quantity objects to unit
-            if isinstance(df[col][0], pint.Quantity):
-                # if tablefmt=='latex':
-                df[col] = df[col].apply(lambda x: f"${x:0.{sig_figs}e~Lx}$")
+        for name in df.index:
+            if "_" in name:
+                new_name = name.replace("_", "\_")
+                df = df.rename(index={name: new_name})
+
+        for row in range(df.shape[0]):
+            for col in range(df.shape[1]):
+                if df.columns[col] == "eqn_str":
+                    cur_str = df.iat[row, col]
+                    cur_str = "$" + cur_str + "$"
+                    cur_str = cur_str.replace("**", "^")
+                    idx = 0
+                    while idx < len(cur_str):
+                        if cur_str[idx] == "_":
+                            cur_str = cur_str[0 : idx + 1] + "{" + cur_str[idx + 1 :]
+                            isMath = False
+                            testIdx = idx + 2
+                            while not isMath:
+                                if not (cur_str[testIdx].isalnum() or cur_str[testIdx] == "_"):
+                                    if cur_str[testIdx] == "*":
+                                        cur_str = cur_str[0:testIdx] + "} " + cur_str[testIdx + 1 :]
+                                    else:
+                                        cur_str = cur_str[0:testIdx] + "}" + cur_str[testIdx:]
+                                    isMath = True
+                                else:
+                                    testIdx += 1
+                            idx = testIdx + 2
+                        elif cur_str[idx] == "*":
+                            cur_str = cur_str[0:idx] + " " + cur_str[idx + 1 :]
+                            idx += 1
+                        else:
+                            idx += 1
+                    df.iloc[row, col] = cur_str
+                elif isinstance(df.iat[row, col], str):
+                    cur_str = df.iat[row, col]
+                    if "_" in cur_str:
+                        df.iloc[row, col] = cur_str.replace("_", "\_")
+                elif isinstance(df.iat[row, col], list):
+                    cur_str = str(df.iat[row, col])
+                    cur_str = cur_str.replace("_", "\_")
+                    new_list = list(cur_str)
+                    quoteCount = 0
+                    # switch every other quote to an opening quote `
+                    for i in range(len(new_list)):
+                        if new_list[i] == "'":
+                            quoteCount += 1
+                            if np.mod(quoteCount, 2):
+                                new_list[i] = "`"
+                    cur_str = "".join(new_list)
+                    df.iloc[row, col] = cur_str
+                # Convert quantity objects to unit
+                elif isinstance(df.iat[row, col], pint.Quantity):
+                    x = df.iat[row, col]
+                    if isinstance(x.magnitude, str):
+                        df.iloc[row, col] = f"{x:s~P}"
+                    else:
+                        df.iloc[row, col] = f"${x:0.{sig_figs}e~Lx}$"
 
-            if col == "idx":
-                df = df.drop("idx", axis=1)
+        for i, col in enumerate(df.columns):
+            if hasattr(self, "print_names"):
+                df = df.rename(columns={col: self.print_names[i]})
+            else:
+                if "_" in col:
+                    df = df.rename(columns={col: col.replace("_", "\_")})
 
         if return_df:
             return df
         else:
             with pandas.option_context("max_colwidth", 1000):
-                logger.info(df.to_latex(escape=False, longtable=True, index=False))
+                logger.info(df.to_latex(escape=False, longtable=True, index=True))
 
     def get_pandas_dataframe_formatted(
         self,
         properties_to_print: Optional[Union[str, List[str]]] = None,
         max_col_width=50,
         sig_figs=2,
     ):
@@ -265,15 +323,15 @@
 
         if properties_to_print:
             df = df[properties_to_print]
 
         # add new lines to df entries (type str) that exceed max col width
         if max_col_width:
             for col in df.columns:
-                if isinstance(df[col][0], str):
+                if isinstance(df[col].iloc[0], str):
                     df[col] = df[col].apply(lambda x: "\n".join(wrap(x, max_col_width)))
 
         # remove leading underscores from df column names (used for cached properties)
         for col in df.columns:
             # if isinstance(df[col][0], str) and col[0] == '_':
             if col[0] == "_":
                 df.rename(columns={col: col[1:]}, inplace=True)
@@ -293,34 +351,41 @@
         df = self.get_pandas_dataframe_formatted(
             properties_to_print=properties_to_print,
             max_col_width=max_col_width,
             sig_figs=sig_figs,
         )
 
         # # Change certain df entries to best format for printing
-        for col in df.columns:
-            # Convert quantity objects to unit
-            if isinstance(df[col][0], pint.Quantity):
-                # if tablefmt=='latex':
-                df[col] = df[col].apply(lambda x: f"{x:0.{sig_figs}e~P}")
+        for row in range(df.shape[0]):
+            for col in range(df.shape[1]):
+                if isinstance(df.iat[row, col], pint.Quantity):
+                    x = df.iat[row, col]
+                    if isinstance(x.magnitude, str):
+                        df.iloc[row, col] = f"{x:s~P}"
+                    else:
+                        df.iloc[row, col] = f"{x:0.{sig_figs}e~P}"
 
         # print to file
         if filename is None:
-            logger.info(
-                tabulate(df, headers="keys", tablefmt=tablefmt),
-                extra=dict(format_type="table"),
-            )
+            if hasattr(self, "print_names"):
+                logger.info(
+                    tabulate(df, headers=self.print_names, tablefmt=tablefmt),
+                    extra=dict(format_type="table"),
+                )
+            else:
+                logger.info(
+                    tabulate(df, headers="keys", tablefmt=tablefmt),
+                    extra=dict(format_type="table"),
+                )
         else:
-            original_stdout = sys.stdout  # Save a reference to the original standard output
-            with open(filename, "w") as f:  # TODO: Add this to logging
-                # Change the standard output to the file we created.
-                sys.stdout = f
-                print("This message will be written to a file.")
-                print(tabulate(df, headers="keys", tablefmt=tablefmt))  # ,
-                sys.stdout = original_stdout  # Reset the standard output to its original value
+            file_handler = logging.FileHandler(filename)
+            file_handler.setFormatter(logging.Formatter(base_format))
+            logger.addHandler(file_handler)
+            logger.info(tabulate(df, headers="keys", tablefmt=tablefmt))  # ,
+            logger.removeHandler(file_handler)
 
     def __str__(self):
         df = self.get_pandas_dataframe(properties_to_print=self.properties_to_print)
         df = df[self.properties_to_print]
 
         return tabulate(df, headers="keys", tablefmt="fancy_grid")
 
@@ -413,30 +478,31 @@
 
 
 class ParameterContainer(ObjectContainer):
     def __init__(self):
         super().__init__(Parameter)
 
         self.properties_to_print = [
-            "_quantity",
-            "is_time_dependent",
-            "sym_expr",
+            "_print_val",
             "notes",
-            "group",
+        ]
+        self.print_names = [
+            "Value/Equation",
+            "Description",
         ]
 
     def print(
         self,
         tablefmt="fancy_grid",
         properties_to_print=None,
         filename=None,
         max_col_width=50,
     ):
         for s in self:
-            s.quantity
+            s.print_val
         super().print(tablefmt, self.properties_to_print, filename, max_col_width)
 
 
 @dataclass
 class Parameter(ObjectInstance):
     """
     Parameter objects contain information for the various parameters involved in reactions,
@@ -503,14 +569,15 @@
 
     name: str
     value: float
     unit: pint.Unit
     group: str = ""
     notes: str = ""
     use_preintegration: bool = False
+    sym_expr: str = ""
 
     def to_dict(self):
         """Convert to a dict that can be used to recreate the object."""
         keys_to_keep = [
             "name",
             "value",
             "unit",
@@ -593,14 +660,15 @@
         name,
         sym_expr,
         unit,
         preint_sym_expr=None,
         group="",
         notes="",
         use_preintegration=False,
+        numerical_int=False,
     ):
         """
         Use sympy to parse time-dependent expression for parameter
         Note that the user can provide a symbolic expression for preintegration
         There was previously a concern that the preintegration expression would no longer be valid
         if the parameter appears in another time-dependent expression.
         However, in the current version of SMART, there is no way to include a time-dependent
@@ -619,50 +687,55 @@
         x, y, z = (Symbol(f"x[{i}]") for i in range(3))
         sym_expr = sym_expr.subs({"x": x, "y": y, "z": z})
 
         # Check if expression is time/space dependent
         free_symbols = [str(x) for x in sym_expr.free_symbols]
         is_time_dependent = "t" in free_symbols
         is_space_dependent = not {"x[0]", "x[1]", "x[2]"}.isdisjoint(set(free_symbols))
-        if is_space_dependent:
-            raise NotImplementedError
         # For now, parameters can only be defined in terms of time/space
         if not {"x[0]", "x[1]", "x[2]", "t"}.issuperset(free_symbols):
             raise NotImplementedError
 
-        # TODO: fix this when implementing space dependent parameters
-        if is_time_dependent:
+        if is_time_dependent and not is_space_dependent:
             value = float(sym_expr.subs({"t": 0.0}))
 
+        if is_space_dependent:
+            dolfin_expression = d.Expression(sym.printing.ccode(sym_expr), t=0.0, degree=3)
+            value = float(sym_expr.subs({"t": 0.0, "x[0]": 0.0, "x[1]": 0.0, "x[2]": 0.0}))
+
         parameter = cls(
             name,
             value,
             unit,
             group=group,
             notes=notes,
             use_preintegration=use_preintegration,
         )
 
         if use_preintegration:
             if preint_sym_expr:
                 if isinstance(preint_sym_expr, str):
                     preint_sym_expr = parse_expr(preint_sym_expr)
                 preint_sym_expr = preint_sym_expr.subs({"x": x, "y": y, "z": z})
+            elif numerical_int:
+                preint_sym_expr = None
+                parameter.int_vec = [0.0]
             else:
                 # try to integrate
                 t = Symbol("t")
                 preint_sym_expr = integrate(sym_expr, t)
             parameter.preint_sym_expr = preint_sym_expr
 
         parameter.free_symbols = free_symbols
         parameter.sym_expr = sym_expr
         parameter.is_time_dependent = is_time_dependent
         parameter.is_space_dependent = is_space_dependent
+        if is_space_dependent:
+            parameter.dolfin_expression = dolfin_expression
 
-        # parameter.dolfin_expression = d.Expression(sym.printing.ccode(sym_expr), t=0.0, degree=1)
         parameter.type = ParameterType.expression
         parameter.__post_init__()
         logger.debug(
             f"Time-dependent parameter {name} evaluated from expression.",
             extra=dict(format_type="log"),
         )
 
@@ -693,24 +766,32 @@
         self._check_input_type_validity()
         self._convert_pint_unit_to_quantity()
         self.check_validity()
         self.value_vector = np.array([0, self.value])
 
     @property
     def dolfin_quantity(self):
-        if hasattr(self, "dolfin_expression") and not self.use_preintegration:
+        if hasattr(self, "dolfin_expression"):
             return self.dolfin_expression * self.unit
         else:
             return self.dolfin_constant * self.unit
 
     @property
     def quantity(self):
         self._quantity = self.value * self.unit
         return self._quantity
 
+    @property
+    def print_val(self):
+        if self.sym_expr == "":
+            self._print_val = self.value * self.unit
+        else:
+            self._print_val = str(self.sym_expr) * self.unit
+        return self._print_val
+
     def check_validity(self):
         """Confirm that time-dependent parameter is defined in terms of time"""
         if self.is_time_dependent:
             if all(
                 [x in ("", None) for x in [self.sampling_file, self.sym_expr, self.preint_sym_expr]]
             ):
                 raise ValueError(
@@ -718,53 +799,38 @@
                     "but is not defined in terms of time."
                 )
 
 
 class SpeciesContainer(ObjectContainer):
     def __init__(self):
         super().__init__(Species)
-        self.properties_to_print = ["compartment_name", "dof_index", "_Diffusion"]
+        self.properties_to_print = [
+            "compartment_name",
+            "_Diffusion",
+            "_Initial_Concentration",
+        ]
+        self.print_names = [
+            "Compartment",
+            "D",
+            "Initial condition",
+        ]
 
     def print(
         self,
         tablefmt="fancy_grid",
         properties_to_print=None,
         filename=None,
         max_col_width=50,
     ):
         for s in self:
             s.D_quantity
             s.latex_name
+            s.initial_condition_quantity
         super().print(tablefmt, self.properties_to_print, filename, max_col_width)
 
-    def print_to_latex(
-        self,
-        properties_to_print=None,
-        max_col_width=None,
-        sig_figs=2,
-        return_df=False,
-    ):
-        properties_to_print = ["_latex_name"]
-        properties_to_print.extend(self.properties_to_print)
-        df = super().print_to_latex(properties_to_print, max_col_width, sig_figs, return_df=True)
-        # fix dof_index
-        for col in df.columns:
-            if col == "dof_index":
-                df[col] = df[col].astype(int)
-        # fix name
-        # get the column of df that contains the name
-        # this can be more robust
-        # df.columns
-
-        if return_df:
-            return df
-        else:
-            with pandas.option_context("max_colwidth", 1000):
-                logger.info(df.to_latex(escape=False, longtable=True, index=False))
-
 
 @dataclass
 class Species(ObjectInstance):
     """
     Each Species object contains information for one state variable in the model
     (can be a molecule, receptor open probability, membrane voltage, etc.)
 
@@ -797,15 +863,14 @@
     diffusion_units: pint.Unit
     compartment_name: str
     group: str = ""
 
     def to_dict(self):
         "Convert to a dict that can be used to recreate the object."
         keys_to_keep = [
-            "name",
             "initial_condition",
             "concentration_units",
             "D",
             "diffusion_units",
             "compartment_name",
             "group",
         ]
@@ -822,33 +887,42 @@
         self.is_in_a_reaction = False
         self.is_an_added_species = False
         self.dof_map = None
         self.u = dict()
         self._usplit = dict()
         self.ut = None
         self.v = None
+        self.has_subdomain = False
 
         if isinstance(self.initial_condition, float):
             pass
         elif isinstance(self.initial_condition, int):
             self.initial_condition = float(self.initial_condition)
         elif isinstance(self.initial_condition, str):
             x, y, z = (Symbol(f"x[{i}]") for i in range(3))
             # Parse the given string to create a sympy expression
             sym_expr = parse_expr(self.initial_condition).subs({"x": x, "y": y, "z": z})
 
             # Check if expression is space dependent
             free_symbols = [str(x) for x in sym_expr.free_symbols]
-            if not {"x[0]", "x[1]", "x[2]"}.issuperset(free_symbols):
+            if "curv" in free_symbols:
+                # then keep as string to put in curvature dependence later after loading mesh
+                self.initial_condition_expression = self.initial_condition
+            elif not {"x[0]", "x[1]", "x[2]"}.issuperset(free_symbols):
                 raise NotImplementedError
-            logger.debug(
-                f"Creating dolfin object for space-dependent initial condition {self.name}",
-                extra=dict(format_type="log"),
-            )
-            self.initial_condition_expression = d.Expression(sym.printing.ccode(sym_expr), degree=1)
+            else:
+                logger.debug(
+                    f"Creating dolfin object for space-dependent initial condition {self.name}",
+                    extra=dict(format_type="log"),
+                )
+                self.initial_condition_expression = d.Expression(
+                    sym.printing.ccode(sym_expr), degree=1
+                )
+        elif isinstance(self.initial_condition, Path):
+            pass  # keep as path
         else:
             raise TypeError("initial_condition must be a float or string.")
 
         self._convert_pint_quantity_to_unit()
         self._check_input_type_validity()
         self._convert_pint_unit_to_quantity()
         self.check_validity()
@@ -872,14 +946,19 @@
         # checking units
         if not self.diffusion_units.check("[length]^2/[time]"):
             raise ValueError(
                 f"Units of diffusion coefficient for species {self.name} must "
                 "be dimensionally equivalent to [length]^2/[time]."
             )
 
+    def restrict_to_subdomain(self, mf, mfval):
+        self.has_subdomain = True
+        self.subdomain_data = mf
+        self.subdomain_val = mfval
+
     @cached_property
     def vscalar(self):
         return d.TestFunction(common.sub(self.compartment.V, 0, True))
 
     @property
     def dolfin_quantity(self):
         return self._usplit["u"] * self.concentration_units
@@ -914,24 +993,29 @@
 
 
 class CompartmentContainer(ObjectContainer):
     def __init__(self):
         super().__init__(Compartment)
 
         self.properties_to_print = [
-            "_mesh_id",
             "dimensionality",
             "num_species",
             "_num_vertices",
-            "_num_dofs",
-            "_num_dofs_local",
             "_num_cells",
             "cell_marker",
             "_nvolume",
         ]
+        self.print_names = [
+            "Dimensionality",
+            "Species",
+            "Vertices",
+            "Cells",
+            "Marker value",
+            "Size",
+        ]
 
     def print(
         self,
         tablefmt="fancy_grid",
         properties_to_print=None,
         filename=None,
         max_col_width=50,
@@ -1081,15 +1165,21 @@
         return self._num_dofs_local
 
 
 class ReactionContainer(ObjectContainer):
     def __init__(self):
         super().__init__(Reaction)
 
-        self.properties_to_print = ["lhs", "rhs", "eqn_f_str", "eqn_r_str"]
+        self.properties_to_print = ["lhs", "rhs", "eqn_str", "topology"]
+        self.print_names = [
+            "Reactants",
+            "Products",
+            "Equation",
+            "Type",
+        ]
 
     def print(
         self,
         tablefmt="fancy_grid",
         properties_to_print=None,
         filename=None,
         max_col_width=50,
@@ -1159,15 +1249,19 @@
     species_map: dict = dataclasses.field(default_factory=dict)
     flux_scaling: dict = dataclasses.field(default_factory=dict)
     reaction_type: str = "mass_action"
     explicit_restriction_to_domain: str = ""
     track_value: bool = False
     eqn_f_str: str = ""
     eqn_r_str: str = ""
+    eqn_str: str = ""
+    topology: str = ""
     group: str = ""
+    axisymm: bool = False
+    has_subdomain: bool = False
 
     def to_dict(self):
         "Convert to a dict that can be used to recreate the object."
         keys_to_keep = [
             "name",
             "lhs",
             "rhs",
@@ -1175,15 +1269,17 @@
             "species_map",
             "flux_scaling",
             "reaction_type",
             "explicit_restriction_to_domain",
             "track_value",
             "eqn_f_str",
             "eqn_r_str",
+            "eqn_str",
             "group",
+            "axisymm",
         ]
         return {key: self.__dict__[key] for key in keys_to_keep}
 
     @classmethod
     def from_dict(cls, input_dict):
         return cls(**input_dict)
 
@@ -1278,19 +1374,31 @@
                 self.species_stoich[species_name] *= self.flux_scaling[species_name]
 
         for species_name, stoich in self.species_stoich.items():
             species = self.species[species_name]
             if self.eqn_f_str:
                 flux_name = self.name + f" [{species_name} (f)]"
                 eqn = stoich * parse_expr(self.eqn_f_str)
-                self.fluxes.update({flux_name: Flux(flux_name, species, eqn, self)})
+                self.fluxes.update({flux_name: Flux(flux_name, species, eqn, self, self.axisymm)})
+                self.fluxes[flux_name].has_subdomain = self.has_subdomain
+                if self.has_subdomain:  # then copy over subdomain data to flux
+                    self.fluxes[flux_name].subdomain_data = self.subdomain_data
+                    self.fluxes[flux_name].subdomain_val = self.subdomain_val
             if self.eqn_r_str:
                 flux_name = self.name + f" [{species_name} (r)]"
                 eqn = -stoich * parse_expr(self.eqn_r_str)
-                self.fluxes.update({flux_name: Flux(flux_name, species, eqn, self)})
+                self.fluxes.update({flux_name: Flux(flux_name, species, eqn, self, self.axisymm)})
+                if self.has_subdomain:  # then copy over subdomain data to flux
+                    self.fluxes[flux_name].subdomain_data = self.subdomain_data
+                    self.fluxes[flux_name].subdomain_val = self.subdomain_val
+
+    def restrict_to_subdomain(self, mf, mfval):
+        self.has_subdomain = True
+        self.subdomain_data = mf
+        self.subdomain_val = mfval
 
 
 class FluxContainer(ObjectContainer):
     def __init__(self):
         super().__init__(Flux)
 
         self.properties_to_print = [
@@ -1319,20 +1427,23 @@
     explicitly initialized by the user.
     Each flux object contains:
 
     * name: string (created as reaction name + species name + (f) or (r))
     * destination_species: flux increases or decreases this species
     * equation: directionality * stoichiometry * reaction string
     * reaction: reaction object this flux comes from
+    * axisymm: True if axisymmetric shape is being represented
     """
 
     name: str
     destination_species: Species
     equation: sym.Expr
     reaction: Reaction
+    axisymm: bool = False
+    has_subdomain: bool = False
 
     def check_validity(self):
         "No validity checks for flux objects currently"
         pass
 
     def __post_init__(self):
         # for nice printing
@@ -1453,16 +1564,14 @@
         For fluxes that contribute to the PDE terms, units should be
         (concentration_units / time)
         If the units dimensionality does not match the expected form, an error is thrown;
         if the dimensionality matches, but the units scaling is not 1.0
         (e.g. if we have a flux specified as nM/s, but concentration_units are defined as uM),
         then self.unit_scale_factor is set to the appropriate factor
         (1000 in the example where we need to convert nM -> uM)
-        NOTE: All unit checks are completed using pint, which may not be compatible with
-        certain functions such as sign().
         """
         concentration_units = self.destination_species.concentration_units
         compartment_units = self.destination_compartment.compartment_units
         diffusion_units = self.destination_species.diffusion_units
 
         # The expected units
         if self.is_boundary_condition:
@@ -1554,60 +1663,111 @@
     @property
     def equation_variables(self):
         variables = {
             variable.name: variable.dolfin_quantity
             for variable in {**self.parameters, **self.species}.values()
         }
         variables.update({"unit_scale_factor": self.unit_scale_factor})
+        free_symbols = [str(x) for x in self.equation.free_symbols]
+        if "curv" in free_symbols:
+            self.curv = self.surface.curv_func * unit.dimensionless
+            variables.update({"curv": self.curv})
         return variables
 
     def equation_lambda_eval(self, input_type="quantity"):
         """Evaluates the equation lambda function using either the quantity
         (value * units), the value, or the units.
         The values and units are evaluated separately and then combined
         because some expressions don't work well
         with pint quantity types.
         """
         # This is an attempt to make the equation lambda work with pint quantities
-        # note - throws an error when it doesn't return a float
-        # (happens when it returns 0 from sign function, for instance)
+        # note - for this eval to work, all variables in the expression must be defined
+        # dolfin quantities and all functions must match one in the list in the config module.
         self._equation_quantity = self.equation_lambda(**self.equation_variables)
         if input_type == "quantity":
             return self._equation_quantity
         elif input_type == "value":
             return self._equation_quantity.magnitude
         elif input_type == "units":
             return unit_to_quantity(self._equation_quantity.units)
 
     # Seems like setting this as a @property doesn't cause fenics to recompile
 
     @property
     def form(self):
         """-1 factor because terms are defined as if they were on the
         lhs of the equation :math:`F(u;v)=0`"""
-        return (
-            d.Constant(-1)
-            * self.equation_lambda_eval(input_type="value")
-            * self.destination_species.v
-            * self.measure
-        )
+        x = d.SpatialCoordinate(self.destination_compartment.dolfin_mesh)
+        if self.has_subdomain:
+            if hasattr(self, "surface"):
+                funcSpace = d.FunctionSpace(self.surface.dolfin_mesh, "P", 1)
+            else:  # then should be volume reaction, assertion to be sure
+                assert self.destination_compartment == list(self.source_compartments.values())[0]
+                funcSpace = d.FunctionSpace(self.destination_compartment.dolfin_mesh, "P", 1)
+            # check that subdomain mesh fcn dim matches function space topological dim
+            assert self.subdomain_data.dim() == funcSpace.mesh().topology().dim()
+            u_mask = d.interpolate(d.Constant(-1.0, name="-1"), funcSpace)
+            u_mask_new = create_restriction(u_mask, self.subdomain_data, self.subdomain_val)
+            mult = u_mask_new
+        else:
+            mult = d.Constant(-1.0, name="-1")
+        if self.axisymm:
+            return (
+                mult
+                * x[0]
+                * self.equation_lambda_eval(input_type="value")
+                * self.destination_species.v
+                * self.measure
+            )
+        else:
+            return (
+                mult
+                * self.equation_lambda_eval(input_type="value")
+                * self.destination_species.v
+                * self.measure
+            )
 
     @property
     def scalar_form(self):
         """
         Defines scalar form for given flux.
         If the destination species is a vector function,
         the assembled form will be a vector of size NDOF.
         """
-        return (
-            d.Constant(-1)
-            * self.equation_lambda_eval(input_type="value")
-            * self.destination_species.vscalar
-            * self.measure
-        )
+        x = d.SpatialCoordinate(self.destination_compartment.dolfin_mesh)
+        if self.has_subdomain:
+            if hasattr(self, "surface"):
+                funcSpace = d.FunctionSpace(self.surface.dolfin_mesh, "P", 1)
+            else:  # then should be volume reaction, assertion to be sure
+                assert self.destination_compartment == list(self.source_compartments.values())[0]
+                funcSpace = d.FunctionSpace(self.destination_compartment.dolfin_mesh, "P", 1)
+            # check that subdomain mesh fcn dim matches function space topological dim
+            assert self.subdomain_data.dim() == funcSpace.mesh().topology().dim()
+            u_mask = d.interpolate(d.Constant(-1.0, name="-1"), funcSpace)
+            u_mask.rename(self.name + "_subdomain_mask", self.name + "_subdomain_mask")
+            u_mask_new = create_restriction(u_mask, self.subdomain_data, self.subdomain_val)
+            mult = u_mask_new
+        else:
+            mult = d.Constant(-1.0, name="-1")
+        if self.axisymm:
+            return (
+                mult
+                * x[0]
+                * self.equation_lambda_eval(input_type="value")
+                * self.destination_species.vscalar
+                * self.measure
+            )
+        else:
+            return (
+                mult
+                * self.equation_lambda_eval(input_type="value")
+                * self.destination_species.vscalar
+                * self.measure
+            )
 
     @property
     def assembled_flux(self):
         """Attempt to convert flux units to molecules_per_second for printing."""
         try:
             self._assembled_flux = -1 * (
                 d.assemble(self.scalar_form).sum() * self.equation_units * self.measure_units
@@ -1688,28 +1848,28 @@
         return self.form_scaling_dolfin_constant * self.form_
 
     @property
     def lhs(self):
         if self.is_lhs:
             return self.form
         else:
-            return d.Constant(-1) * self.form
+            return d.Constant(-1, name="-1") * self.form
 
     @property
     def rhs(self):
         if self.is_lhs:
-            return d.Constant(-1) * self.form
+            return d.Constant(-1, name="-1") * self.form
         else:
             return self.form
 
     def __post_init__(self):
         self.compartment = self.species.compartment
         self._compartment_name = self.compartment.name
 
-        self.form_scaling_dolfin_constant = d.Constant(self.form_scaling)
+        self.form_scaling_dolfin_constant = d.Constant(self.form_scaling, name=f"scale_{self.name}")
 
         self._convert_pint_quantity_to_unit()
         self._check_input_type_validity()
         self._convert_pint_unit_to_quantity()
 
     @property
     def integrals(self):
@@ -1731,17 +1891,51 @@
     # FIXME: Add typing
     # Initialize containers
     pc, sc, cc, rc = empty_sbmodel()
     parameters = [x for x in local_values if isinstance(x, Parameter)]
     species = [x for x in local_values if isinstance(x, Species)]
     compartments = [x for x in local_values if isinstance(x, Compartment)]
     reactions = [x for x in local_values if isinstance(x, Reaction)]
-    # we just reverse the list so that the order is the same as how they were defined
-    parameters.reverse()
-    species.reverse()
-    compartments.reverse()
-    reactions.reverse()
     pc.add(parameters)
     sc.add(species)
     cc.add(compartments)
     rc.add(reactions)
     return pc, sc, cc, rc
+
+
+def create_restriction(u: d.Function, mesh_function: d.MeshFunction, value: np.integer):
+    """
+    Restrict a function on a submesh to a subset of parent entities
+    (same dimension as the submesh)
+
+    :param u: Function on submesh
+    :param mesh_function: MeshFunction marking the subset of parent entities
+    (same dimension as the cells of the submesh)
+    :param value: Value in MeshFunction marking the subset of parent entities
+    :return: New restricted function
+    """
+    submesh = u.function_space().mesh()
+
+    # Compute local cells in submesh marked by parent meshtag
+    # using first map to run without specifying parent mesh id
+    sub_to_parent_map = submesh.topology().mapping()[mesh_function.mesh().id()].cell_map()
+    marked_sub_entities = mesh_function.array()[sub_to_parent_map] == value
+    local_indices = np.flatnonzero(marked_sub_entities)
+
+    # Find all degrees of freedom to transfer data from
+    V = u.function_space()
+    u_new = d.Function(u.function_space())
+    vector = u_new.vector()
+    dof_list = [V.dofmap().cell_dofs(cell) for cell in local_indices]
+    if len(dof_list) == 0:
+        transfer_dofs = np.array([])
+    else:
+        transfer_dofs = np.unique(np.hstack(dof_list))
+    im = V.dofmap().index_map()
+    num_local = im.local_range()[1] - im.local_range()[0]
+
+    # Filter out dofs that are not local
+    transfer_dofs = np.array([dof for dof in transfer_dofs if dof < num_local])
+    vector[transfer_dofs] = u.vector()[transfer_dofs]
+    vector.apply("insert")
+
+    return u_new
```

### Comparing `fenics-smart-2.1.7/smart/solvers.py` & `fenics_smart-2.2.0/smart/solvers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """SMART module interfacing with PETSc SNES solver"""
 import logging
 from typing import Dict, List, Optional
 
 import dolfin as d
+from dolfin.common.timer import timed
 import petsc4py.PETSc as p
 
 from .common import Stopwatch
 from .model_assembly import Compartment
 
 logger = logging.getLogger(__name__)
 
@@ -36,30 +37,34 @@
         active_compartments: List of compartments used in the variational form.
         all_compartments: List of all compartments in model.
         stopwatches: Dictionary of stop-watches (stopwatch_name: stopwatch-class).
             Must include at least `snes jacobian assemble`, `snes residual assemble`
             and `snes initialize zero matrices`
     """
 
+    @timed("Initialize smartSNESProblem")
     def __init__(
         self,
         u: d.Function,
         Fforms: List[List[d.Form]],
         Jforms_all: List[List[d.Form]],
         active_compartments: List[Compartment],
         all_compartments: List[Compartment],
         stopwatches: Dict[str, Stopwatch],
+        model,
     ):
         self.u = u
         self.Fforms = Fforms
         self.Jforms_all = Jforms_all
         # for convenience, the mixed function space (model.V)
         self.W = [usub.function_space() for usub in u._functions]
         self.dim = len(self.Fforms)
 
+        self.model = model
+
         assert len(self.Jforms_all) == self.dim**2
 
         # Extract MPI communicator from one of the underlying meshes
         assert len(self.u._functions) >= 1
         self.comm = self.u._functions[0].function_space().mesh().mpi_comm()
         self.rank = self.comm.rank
         self.size = self.comm.size
@@ -109,14 +114,15 @@
                     self.empty_forms.append((i, j))
         if len(self.empty_forms) > 0:
             logger.debug(
                 f"Forms {self.empty_forms} are empty. Skipping assembly.",
                 extra=dict(format_type="data"),
             )
 
+    @timed("Initialize PETSc Nested Matrix")
     def init_petsc_matnest(self):
         Jforms = self.Jforms_all
         dim = self.dim
         Jpetsc = []
         for i in range(dim):
             for j in range(dim):
                 ij = i * dim + j
@@ -191,37 +197,38 @@
             # self.Jpetsc_nest = self.d_to_p(d.PETScNestMatrix(Jpetsc))
         self.Jpetsc_nest.assemble()
         logger.info(f"Jpetsc_nest assembled, size = {self.Jpetsc_nest.size}")
 
     def d_to_p(self, dolfin_matrix):
         return d.as_backend_type(dolfin_matrix).mat()
 
+    @timed("Initialize PETSc Nested Vector")
     def init_petsc_vecnest(self):
         dim = self.dim
         logger.info("Initializing block residual vector", extra=dict(format_type="assembly"))
 
         Fpetsc = []
         for j in range(dim):
             Fsum = None
-            for k in range(len(self.Fforms[j])):
-                if self.Fforms[j][k].function_space(0) is None:
+            for k, form in enumerate(self.Fforms[j]):
+                if form is None:
                     logger.warning(
-                        f"{self.Fjk_name(j,k)}] has no function space",
+                        f"{self.Fjk_name(j,k)}] is not defined",
                         extra=dict(format_type="log"),
                     )
                     continue
-
+                # Note: This could be simplified once add_values in assemble mixed is fixed
                 tensor = d.PETScVector(self.comm)
 
                 if Fsum is None:
-                    Fsum = d.assemble_mixed(self.Fforms[j][k], tensor=tensor)
+                    Fsum = d.assemble_mixed(form, tensor=tensor)
                 else:
                     # Fsum.axpy(1, d.assemble_mixed(self.Fforms[j][k], tensor=tensor).vec(),
                     # structure=Fsum.Structure.DIFFERENT_NONZERO_PATTERN)
-                    Fsum += d.assemble_mixed(self.Fforms[j][k], tensor=tensor)
+                    Fsum += d.assemble_mixed(form, tensor=tensor)
 
             if Fsum is None:
                 logger.debug(
                     f"{self.Fjk_name(j)} is empty - initializing as empty PETSc "
                     f"Vector with local size {self.local_sizes[j]} "
                     f"and global size {self.global_sizes[j]}",
                     extra=dict(format_type="log"),
@@ -233,27 +240,31 @@
         if self.is_single_domain:
             # We can't use a nest vector
             self.Fpetsc_nest = d.PETScVector(Fpetsc[0]).vec()
         else:
             self.Fpetsc_nest = p.Vec().createNest(Fpetsc, comm=self.comm)
         self.Fpetsc_nest.assemble()
 
+    @timed("SNES Assemble Jacobian Nested Matrix")
     def assemble_Jnest(self, Jnest):
         """Assemble Jacobian nest matrix.
 
         Args:
             Jnest : petsc4py.Mat
                 PETSc nest matrix representing the Jacobian
 
 
         """
+
         logger.debug("Assembling block Jacobian", extra=dict(format_type="assembly"))
         self.stopwatches["snes jacobian assemble"].start()
         dim = self.dim
 
+        # forms are updated for ODE solutions in
+        # assemble_Fnest, as that is executed first
         Jform = self.Jforms_all
 
         # Get the petsc sub matrices, convert to dolfin wrapper, assemble forms using
         # dolfin wrapper as tensor
         for i in range(dim):
             for j in range(dim):
                 if (i, j) in self.empty_forms:
@@ -312,14 +323,15 @@
 
                 self.print_Jijk_info(i, j, k=None, tensor=Jij_petsc)
 
         Jnest.assemble()
 
         self.stopwatches["snes jacobian assemble"].pause()
 
+    @timed("SNES Assemble Residual Nest Vector")
     def assemble_Fnest(self, Fnest):
         """
         Assemble residual nest vector
 
         Arguments:
             Fnest : petsc4py.Vec
                 PETSc nest vector representing the residual
@@ -332,22 +344,26 @@
             Fj_petsc = [Fnest]
         else:
             Fj_petsc = Fnest.getNestSubVecs()
         Fvecs = []
 
         for j in range(dim):
             Fvecs.append([])
-            for k in range(len(self.Fforms[j])):
-                # , tensor=d.PETScVector(Fvecs[idx]))
-                Fvecs[j].append(d.as_backend_type(d.assemble_mixed(self.Fforms[j][k])))
-            # TODO: could probably speed this up by not using axpy if there is only one subform
-            # sum the vectors
+            # NOTE: This can be simplified once add_values is fixed
+            for k, form in enumerate(self.Fforms[j]):
+                if form is None:
+                    logger.warning(
+                        f"{self.Fjk_name(j,k)}] is not defined",
+                        extra=dict(format_type="log"),
+                    )
+                    continue
+                Fvecs[j].append(d.as_backend_type(d.assemble_mixed(form)))
             Fj_petsc[j].zeroEntries()
-            for k in range(len(self.Fforms[j])):
-                Fj_petsc[j].axpy(1, Fvecs[j][k].vec())
+            for k, vec in enumerate(Fvecs[j]):
+                Fj_petsc[j].axpy(1, vec.vec())
 
         Fnest.assemble()
         self.stopwatches["snes residual assemble"].pause()
 
     def copy_u(self, unest):
         if self.is_single_domain:
             uvecs = [unest]
@@ -362,14 +378,15 @@
         self.copy_u(u)
         self.assemble_Fnest(Fnest)
 
     def J(self, snes, u, Jnest, P):
         self.copy_u(u)
         self.assemble_Jnest(Jnest)
 
+    @timed("SNES Initialize Zero Matrices")
     def init_petsc_matrix(self, i, j, nnz_guess=None, set_lgmap=False, assemble=False):
         """
         Initialize a PETSc matrix with appropriate structure
 
         Args:
             i,j : indices of the block
             nnz_guess : number of non-zeros (per row) to guess for the matrix
@@ -402,28 +419,30 @@
 
         if assemble:
             M.assemble()
         self.stopwatches["snes initialize zero matrices"].pause()
 
         return M
 
+    @timed("SNES Initialize Zero Vectors")
     def init_petsc_vector(self, j, assemble=False):
         """Initialize a dolfin wrapped PETSc vector with appropriate structure
 
         Args:
             j : index
             assemble : whether to assemble the vector or not (Boolean)
         """
         V = p.Vec().create(comm=self.comm)
         V.setSizes((self.local_sizes[j], self.global_sizes[j]))
         V.setUp()
         # V.setLGMap(self.lgmaps_petsc[j])
 
         if assemble:
             V.assemble()
+
         return V
 
     def Jijk_name(self, i: int, j: int, k: Optional[int] = None):
         """Get a string representation of an entry of the Jacobian.
 
         Args:
             i: Row index
```

### Comparing `fenics-smart-2.1.7/smart/units.py` & `fenics_smart-2.2.0/smart/units.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.7/smart/utils.py` & `fenics_smart-2.2.0/smart/utils.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.7/smart/visualization.py` & `fenics_smart-2.2.0/smart/visualization.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.7/tests/test_compartment.py` & `fenics_smart-2.2.0/tests/test_compartment.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.7/tests/test_parameter.py` & `fenics_smart-2.2.0/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `fenics-smart-2.1.7/tests/test_species.py` & `fenics_smart-2.2.0/tests/test_species.py`

 * *Files identical despite different names*

