# Comparing `tmp/doped-2.4.2.tar.gz` & `tmp/doped-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doped-2.4.2.tar", last modified: Mon May 13 15:16:37 2024, max compression
+gzip compressed data, was "doped-2.4.3.tar", last modified: Fri May 24 18:23:54 2024, max compression
```

## Comparing `doped-2.4.2.tar` & `doped-2.4.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:16:37.404386 doped-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 15:15:07.000000 doped-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-05-13 15:16:37.404386 doped-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-13 15:15:07.000000 doped-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:16:37.396386 doped-2.4.2/doped/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:16:37.396386 doped-2.4.2/doped/VASP_sets/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-13 15:15:07.000000 doped-2.4.2/doped/VASP_sets/DefectSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 15:15:07.000000 doped-2.4.2/doped/VASP_sets/HSESet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 15:15:07.000000 doped-2.4.2/doped/VASP_sets/PBEsol_ConvergenceSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-13 15:15:07.000000 doped-2.4.2/doped/VASP_sets/PotcarSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-13 15:15:07.000000 doped-2.4.2/doped/VASP_sets/RelaxSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-13 15:15:07.000000 doped-2.4.2/doped/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   117131 2024-05-13 15:15:07.000000 doped-2.4.2/doped/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    95322 2024-05-13 15:15:07.000000 doped-2.4.2/doped/chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    88382 2024-05-13 15:15:07.000000 doped-2.4.2/doped/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    28951 2024-05-13 15:15:07.000000 doped-2.4.2/doped/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)   108002 2024-05-13 15:15:07.000000 doped-2.4.2/doped/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)   147387 2024-05-13 15:15:07.000000 doped-2.4.2/doped/thermodynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:16:37.400386 doped-2.4.2/doped/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 15:15:07.000000 doped-2.4.2/doped/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-13 15:15:07.000000 doped-2.4.2/doped/utils/displacement.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)    24728 2024-05-13 15:15:07.000000 doped-2.4.2/doped/utils/displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-13 15:15:07.000000 doped-2.4.2/doped/utils/doped.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)    30685 2024-05-13 15:15:07.000000 doped-2.4.2/doped/utils/eigenvalues.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-13 15:15:07.000000 doped-2.4.2/doped/utils/legacy_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)    62400 2024-05-13 15:15:07.000000 doped-2.4.2/doped/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    39178 2024-05-13 15:15:07.000000 doped-2.4.2/doped/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-05-13 15:15:07.000000 doped-2.4.2/doped/utils/supercells.py
--rw-r--r--   0 runner    (1001) docker     (127)    69846 2024-05-13 15:15:07.000000 doped-2.4.2/doped/utils/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)   148776 2024-05-13 15:15:07.000000 doped-2.4.2/doped/utils/wyckpos.dat
--rw-r--r--   0 runner    (1001) docker     (127)   117889 2024-05-13 15:15:07.000000 doped-2.4.2/doped/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:16:37.400386 doped-2.4.2/doped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14743 2024-05-13 15:16:37.000000 doped-2.4.2/doped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 15:16:37.000000 doped-2.4.2/doped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:16:37.000000 doped-2.4.2/doped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-13 15:16:37.000000 doped-2.4.2/doped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 15:16:37.000000 doped-2.4.2/doped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-13 15:15:09.000000 doped-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:16:37.404386 doped-2.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:16:37.400386 doped-2.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   152828 2024-05-13 15:15:12.000000 doped-2.4.2/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    38044 2024-05-13 15:15:12.000000 doped-2.4.2/tests/test_chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-13 15:15:12.000000 doped-2.4.2/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-13 15:15:12.000000 doped-2.4.2/tests/test_displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)   165582 2024-05-13 15:15:12.000000 doped-2.4.2/tests/test_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-05-13 15:15:12.000000 doped-2.4.2/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    97854 2024-05-13 15:15:12.000000 doped-2.4.2/tests/test_thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)    82287 2024-05-13 15:15:12.000000 doped-2.4.2/tests/test_vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-13 15:15:12.000000 doped-2.4.2/tests/test_wyckoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:23:54.656915 doped-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 18:22:28.000000 doped-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-05-24 18:23:54.656915 doped-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-05-24 18:22:28.000000 doped-2.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:23:54.644915 doped-2.4.3/doped/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:23:54.648915 doped-2.4.3/doped/VASP_sets/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-24 18:22:29.000000 doped-2.4.3/doped/VASP_sets/DefectSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-24 18:22:29.000000 doped-2.4.3/doped/VASP_sets/HSESet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-24 18:22:29.000000 doped-2.4.3/doped/VASP_sets/PBEsol_ConvergenceSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-24 18:22:29.000000 doped-2.4.3/doped/VASP_sets/PotcarSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-24 18:22:29.000000 doped-2.4.3/doped/VASP_sets/RelaxSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-24 18:22:29.000000 doped-2.4.3/doped/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117131 2024-05-24 18:22:29.000000 doped-2.4.3/doped/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95322 2024-05-24 18:22:29.000000 doped-2.4.3/doped/chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88382 2024-05-24 18:22:29.000000 doped-2.4.3/doped/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28951 2024-05-24 18:22:29.000000 doped-2.4.3/doped/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108002 2024-05-24 18:22:29.000000 doped-2.4.3/doped/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)   147387 2024-05-24 18:22:29.000000 doped-2.4.3/doped/thermodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:23:54.652915 doped-2.4.3/doped/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-24 18:22:29.000000 doped-2.4.3/doped/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-24 18:22:29.000000 doped-2.4.3/doped/utils/displacement.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)    24728 2024-05-24 18:22:29.000000 doped-2.4.3/doped/utils/displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-24 18:22:29.000000 doped-2.4.3/doped/utils/doped.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)    30685 2024-05-24 18:22:29.000000 doped-2.4.3/doped/utils/eigenvalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-24 18:22:29.000000 doped-2.4.3/doped/utils/legacy_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62400 2024-05-24 18:22:29.000000 doped-2.4.3/doped/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39178 2024-05-24 18:22:29.000000 doped-2.4.3/doped/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31851 2024-05-24 18:22:29.000000 doped-2.4.3/doped/utils/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71032 2024-05-24 18:22:29.000000 doped-2.4.3/doped/utils/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148776 2024-05-24 18:22:29.000000 doped-2.4.3/doped/utils/wyckpos.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   117889 2024-05-24 18:22:29.000000 doped-2.4.3/doped/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:23:54.652915 doped-2.4.3/doped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-05-24 18:23:54.000000 doped-2.4.3/doped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-24 18:23:54.000000 doped-2.4.3/doped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:23:54.000000 doped-2.4.3/doped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-24 18:23:54.000000 doped-2.4.3/doped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 18:23:54.000000 doped-2.4.3/doped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-24 18:22:31.000000 doped-2.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:23:54.656915 doped-2.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:23:54.652915 doped-2.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   152828 2024-05-24 18:22:34.000000 doped-2.4.3/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38044 2024-05-24 18:22:34.000000 doped-2.4.3/tests/test_chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-24 18:22:34.000000 doped-2.4.3/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-24 18:22:34.000000 doped-2.4.3/tests/test_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)   165582 2024-05-24 18:22:34.000000 doped-2.4.3/tests/test_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-05-24 18:22:34.000000 doped-2.4.3/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97854 2024-05-24 18:22:34.000000 doped-2.4.3/tests/test_thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82287 2024-05-24 18:22:34.000000 doped-2.4.3/tests/test_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-24 18:22:34.000000 doped-2.4.3/tests/test_wyckoff.py
```

### Comparing `doped-2.4.2/LICENSE` & `doped-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/PKG-INFO` & `doped-2.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doped
-Version: 2.4.2
+Version: 2.4.3
 Summary: Python package to setup, process and analyse solid-state defect calculations with VASP
 Author-email: Seán Kavanagh <skavanagh@seas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2021 Seán Kavanagh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tabulate
 Requires-Dist: matplotlib>=3.5.2
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: pymatgen>=2023.11.12
-Requires-Dist: spglib<=2.0.2
+Requires-Dist: spglib>=2.4.0
 Requires-Dist: pymatgen-analysis-defects>=2023.8.22
 Requires-Dist: shakenbreak>=3.3.1
 Requires-Dist: pandas
 Requires-Dist: pydefect>=0.8.1
 Requires-Dist: filelock
 Requires-Dist: vise>=0.9.0
 Requires-Dist: easyunfold>=0.3.6
@@ -97,16 +97,22 @@
 ![https://github.com/openjournals/joss-reviews/issues/6433](docs/JOSS/doped_JOSS_figure.png)
 **(a)** Optimal supercell generation comparison. **(b)** Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-size correction plot, **(d)** defect formation energy diagram, **(e)** chemical potential / stability region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi level / carrier concentration heatmap plots from `doped`. Automated plots of **(i,j)** single-particle eigenvalues and **(k)** site
 displacements from DFT supercell calculations. See the [JOSS paper](https://doi.org/10.21105/joss.06433) for more details.
 
 ## Installation
 ```bash
 pip install doped  # install doped and dependencies
+conda install -c conda-forge spglib  # bundle C libraries with spglib
 ```
 
+Note that either `conda install -c conda-forge spglib` or
+`pip install git+https://github.com/spglib/spglib --config-settings=cmake.define.SPGLIB_SHARED_LIBS=OFF`
+should be used after `pip install doped`, which ensures that the correct C libraries are bundled with
+`spglib`, to prevent unnecessary warnings.
+
 Alternatively if desired, `doped` can also be installed from `conda` with:
 
 ```bash
   conda install -c conda-forge doped
   pip install pydefect  # pydefect not available on conda, so needs to be installed with pip or otherwise, if using the eFNV correction
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: doped Version: 2.4.2 Summary: Python package to
+Metadata-Version: 2.1 Name: doped Version: 2.4.3 Summary: Python package to
 setup, process and analyse solid-state defect calculations with VASP Author-
 email: SeÃ¡n Kavanagh
 seas.harvard.edu> License: MIT License Copyright (c) 2021 SeÃ¡n Kavanagh
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -23,15 +23,15 @@
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
 Engineering :: Information Analysis Classifier: Topic :: Scientific/Engineering
 :: Physics Classifier: Topic :: Scientific/Engineering :: Chemistry Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
 >=3.9 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: tabulate Requires-Dist: matplotlib>=3.5.2 Requires-Dist: numpy>=1.21.0
-Requires-Dist: pymatgen>=2023.11.12 Requires-Dist: spglib<=2.0.2 Requires-Dist:
+Requires-Dist: pymatgen>=2023.11.12 Requires-Dist: spglib>=2.4.0 Requires-Dist:
 pymatgen-analysis-defects>=2023.8.22 Requires-Dist: shakenbreak>=3.3.1
 Requires-Dist: pandas Requires-Dist: pydefect>=0.8.1 Requires-Dist: filelock
 Requires-Dist: vise>=0.9.0 Requires-Dist: easyunfold>=0.3.6 Provides-Extra:
 tests Requires-Dist: pytest<8.2; extra == "tests" Requires-Dist: pytest-
 mpl>=0.16.1; extra == "tests" Provides-Extra: docs Requires-Dist: sphinx; extra
 == "docs" Requires-Dist: sphinx-book-theme; extra == "docs" Requires-Dist:
 sphinx_design; extra == "docs" Provides-Extra: analysis Requires-Dist:
@@ -87,28 +87,33 @@
 (d)** defect formation energy diagram, **(e)** chemical potential / stability
 region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier
 concentrations vs. annealing temperature and **(h)** Fermi level / carrier
 concentration heatmap plots from `doped`. Automated plots of **(i,j)** single-
 particle eigenvalues and **(k)** site displacements from DFT supercell
 calculations. See the [JOSS paper](https://doi.org/10.21105/joss.06433) for
 more details. ## Installation ```bash pip install doped # install doped and
-dependencies ``` Alternatively if desired, `doped` can also be installed from
-`conda` with: ```bash conda install -c conda-forge doped pip install pydefect #
-pydefect not available on conda, so needs to be installed with pip or
-otherwise, if using the eFNV correction ``` If you haven't done so already, you
-will need to set up your VASP `POTCAR` files and `Materials Project` API with
-`pymatgen` using the `.pmgrc.yaml` file, in order for `doped` to automatically
-generate VASP input files for defect calculations and determine competing
-phases for chemical potentials. See the docs [Installation](https://
-doped.readthedocs.io/en/latest/Installation.html) page for details on this. ##
-Citation If you use `doped` in your research, please cite: - S. R. Kavanagh et
-al. [doped: Python toolkit for robust and repeatable charged defect supercell
-calculations](https://doi.org/10.21105/joss.06433). _Journal of Open Source
-Software_ 9 (96), 6433, **2024** ## `ShakeNBreak` As shown in the `doped`
-tutorials, it is highly recommended to use the [`ShakeNBreak`](https://
+dependencies conda install -c conda-forge spglib # bundle C libraries with
+spglib ``` Note that either `conda install -c conda-forge spglib` or `pip
+install git+https://github.com/spglib/spglib --config-
+settings=cmake.define.SPGLIB_SHARED_LIBS=OFF` should be used after `pip install
+doped`, which ensures that the correct C libraries are bundled with `spglib`,
+to prevent unnecessary warnings. Alternatively if desired, `doped` can also be
+installed from `conda` with: ```bash conda install -c conda-forge doped pip
+install pydefect # pydefect not available on conda, so needs to be installed
+with pip or otherwise, if using the eFNV correction ``` If you haven't done so
+already, you will need to set up your VASP `POTCAR` files and `Materials
+Project` API with `pymatgen` using the `.pmgrc.yaml` file, in order for `doped`
+to automatically generate VASP input files for defect calculations and
+determine competing phases for chemical potentials. See the docs [Installation]
+(https://doped.readthedocs.io/en/latest/Installation.html) page for details on
+this. ## Citation If you use `doped` in your research, please cite: - S. R.
+Kavanagh et al. [doped: Python toolkit for robust and repeatable charged defect
+supercell calculations](https://doi.org/10.21105/joss.06433). _Journal of Open
+Source Software_ 9 (96), 6433, **2024** ## `ShakeNBreak` As shown in the
+`doped` tutorials, it is highly recommended to use the [`ShakeNBreak`](https://
 shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects
 in solids, to ensure you have identified the groundstate structures of your
 defects. As detailed in the [theory paper](https://doi.org/10.1038/s41524-023-
 00973-1), skipping this step can result in drastically incorrect formation
 energies, transition levels, carrier capture (basically any property associated
 with defects). This approach is followed in the [doped example notebook](https:
 //github.com/SMTG-Bham/doped/blob/main/dope_workflow_example.ipynb), with a
```

### Comparing `doped-2.4.2/README.md` & `doped-2.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,22 @@
 ![https://github.com/openjournals/joss-reviews/issues/6433](docs/JOSS/doped_JOSS_figure.png)
 **(a)** Optimal supercell generation comparison. **(b)** Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-size correction plot, **(d)** defect formation energy diagram, **(e)** chemical potential / stability region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi level / carrier concentration heatmap plots from `doped`. Automated plots of **(i,j)** single-particle eigenvalues and **(k)** site
 displacements from DFT supercell calculations. See the [JOSS paper](https://doi.org/10.21105/joss.06433) for more details.
 
 ## Installation
 ```bash
 pip install doped  # install doped and dependencies
+conda install -c conda-forge spglib  # bundle C libraries with spglib
 ```
 
+Note that either `conda install -c conda-forge spglib` or
+`pip install git+https://github.com/spglib/spglib --config-settings=cmake.define.SPGLIB_SHARED_LIBS=OFF`
+should be used after `pip install doped`, which ensures that the correct C libraries are bundled with
+`spglib`, to prevent unnecessary warnings.
+
 Alternatively if desired, `doped` can also be installed from `conda` with:
 
 ```bash
   conda install -c conda-forge doped
   pip install pydefect  # pydefect not available on conda, so needs to be installed with pip or otherwise, if using the eFNV correction
 ```
```

#### html2text {}

```diff
@@ -47,28 +47,33 @@
 (d)** defect formation energy diagram, **(e)** chemical potential / stability
 region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier
 concentrations vs. annealing temperature and **(h)** Fermi level / carrier
 concentration heatmap plots from `doped`. Automated plots of **(i,j)** single-
 particle eigenvalues and **(k)** site displacements from DFT supercell
 calculations. See the [JOSS paper](https://doi.org/10.21105/joss.06433) for
 more details. ## Installation ```bash pip install doped # install doped and
-dependencies ``` Alternatively if desired, `doped` can also be installed from
-`conda` with: ```bash conda install -c conda-forge doped pip install pydefect #
-pydefect not available on conda, so needs to be installed with pip or
-otherwise, if using the eFNV correction ``` If you haven't done so already, you
-will need to set up your VASP `POTCAR` files and `Materials Project` API with
-`pymatgen` using the `.pmgrc.yaml` file, in order for `doped` to automatically
-generate VASP input files for defect calculations and determine competing
-phases for chemical potentials. See the docs [Installation](https://
-doped.readthedocs.io/en/latest/Installation.html) page for details on this. ##
-Citation If you use `doped` in your research, please cite: - S. R. Kavanagh et
-al. [doped: Python toolkit for robust and repeatable charged defect supercell
-calculations](https://doi.org/10.21105/joss.06433). _Journal of Open Source
-Software_ 9 (96), 6433, **2024** ## `ShakeNBreak` As shown in the `doped`
-tutorials, it is highly recommended to use the [`ShakeNBreak`](https://
+dependencies conda install -c conda-forge spglib # bundle C libraries with
+spglib ``` Note that either `conda install -c conda-forge spglib` or `pip
+install git+https://github.com/spglib/spglib --config-
+settings=cmake.define.SPGLIB_SHARED_LIBS=OFF` should be used after `pip install
+doped`, which ensures that the correct C libraries are bundled with `spglib`,
+to prevent unnecessary warnings. Alternatively if desired, `doped` can also be
+installed from `conda` with: ```bash conda install -c conda-forge doped pip
+install pydefect # pydefect not available on conda, so needs to be installed
+with pip or otherwise, if using the eFNV correction ``` If you haven't done so
+already, you will need to set up your VASP `POTCAR` files and `Materials
+Project` API with `pymatgen` using the `.pmgrc.yaml` file, in order for `doped`
+to automatically generate VASP input files for defect calculations and
+determine competing phases for chemical potentials. See the docs [Installation]
+(https://doped.readthedocs.io/en/latest/Installation.html) page for details on
+this. ## Citation If you use `doped` in your research, please cite: - S. R.
+Kavanagh et al. [doped: Python toolkit for robust and repeatable charged defect
+supercell calculations](https://doi.org/10.21105/joss.06433). _Journal of Open
+Source Software_ 9 (96), 6433, **2024** ## `ShakeNBreak` As shown in the
+`doped` tutorials, it is highly recommended to use the [`ShakeNBreak`](https://
 shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects
 in solids, to ensure you have identified the groundstate structures of your
 defects. As detailed in the [theory paper](https://doi.org/10.1038/s41524-023-
 00973-1), skipping this step can result in drastically incorrect formation
 energies, transition levels, carrier capture (basically any property associated
 with defects). This approach is followed in the [doped example notebook](https:
 //github.com/SMTG-Bham/doped/blob/main/dope_workflow_example.ipynb), with a
```

### Comparing `doped-2.4.2/doped/VASP_sets/DefectSet.yaml` & `doped-2.4.3/doped/VASP_sets/DefectSet.yaml`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/VASP_sets/HSESet.yaml` & `doped-2.4.3/doped/VASP_sets/HSESet.yaml`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/VASP_sets/PotcarSet.yaml` & `doped-2.4.3/doped/VASP_sets/PotcarSet.yaml`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/VASP_sets/RelaxSet.yaml` & `doped-2.4.3/doped/VASP_sets/RelaxSet.yaml`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/__init__.py` & `doped-2.4.3/doped/__init__.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/analysis.py` & `doped-2.4.3/doped/analysis.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/chemical_potentials.py` & `doped-2.4.3/doped/chemical_potentials.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/core.py` & `doped-2.4.3/doped/core.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/corrections.py` & `doped-2.4.3/doped/corrections.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/generation.py` & `doped-2.4.3/doped/generation.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/thermodynamics.py` & `doped-2.4.3/doped/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/utils/displacement.mplstyle` & `doped-2.4.3/doped/utils/displacement.mplstyle`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/utils/displacements.py` & `doped-2.4.3/doped/utils/displacements.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/utils/doped.mplstyle` & `doped-2.4.3/doped/utils/doped.mplstyle`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/utils/eigenvalues.py` & `doped-2.4.3/doped/utils/eigenvalues.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/utils/legacy_corrections.py` & `doped-2.4.3/doped/utils/legacy_corrections.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/utils/parsing.py` & `doped-2.4.3/doped/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/utils/plotting.py` & `doped-2.4.3/doped/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/utils/supercells.py` & `doped-2.4.3/doped/utils/supercells.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/utils/symmetry.py` & `doped-2.4.3/doped/utils/symmetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,46 @@
     _get_bulk_supercell,
     _get_defect_supercell,
     _get_defect_supercell_bulk_site_coords,
     _get_unrelaxed_defect_structure,
 )
 
 
+def _set_spglib_warnings_env_var():
+    """
+    Set the SPGLIB environment variable to suppress spglib warnings.
+    """
+    os.environ["SPGLIB_WARNING"] = "OFF"
+
+
+def _check_spglib_version():
+    """
+    Check the versions of spglib and its C libraries, and raise a warning if
+    the correct installation instructions have not been followed.
+    """
+    import spglib
+
+    python_version = spglib.__version__
+    c_version = spglib.spg_get_version_full()
+
+    if python_version != c_version:
+        warnings.warn(
+            f"Your spglib Python version (spglib.__version__ = {python_version}) does not match its C "
+            f"library version (spglib.spg_get_version_full() = {c_version}). This can lead to unnecessary "
+            f"spglib warning messages, but can be avoided by installing spglib with `conda install -c "
+            f"conda-forge spglib` or `pip install git+https://github.com/spglib/spglib "
+            f"--config-settings=cmake.define.SPGLIB_SHARED_LIBS=OFF` as detailed in the doped "
+            f"installation instructions: https://doped.readthedocs.io/en/latest/Installation.html"
+        )
+
+
+_check_spglib_version()
+_set_spglib_warnings_env_var()
+
+
 def _round_floats(obj, places=5):
     """
     Recursively round floats in a dictionary to ``places`` decimal places.
     """
     if isinstance(obj, float):
         return _custom_round(obj, places) + 0.0
     if isinstance(obj, dict):
```

### Comparing `doped-2.4.2/doped/utils/wyckpos.dat` & `doped-2.4.3/doped/utils/wyckpos.dat`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped/vasp.py` & `doped-2.4.3/doped/vasp.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/doped.egg-info/PKG-INFO` & `doped-2.4.3/doped.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doped
-Version: 2.4.2
+Version: 2.4.3
 Summary: Python package to setup, process and analyse solid-state defect calculations with VASP
 Author-email: Seán Kavanagh <skavanagh@seas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2021 Seán Kavanagh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tabulate
 Requires-Dist: matplotlib>=3.5.2
 Requires-Dist: numpy>=1.21.0
 Requires-Dist: pymatgen>=2023.11.12
-Requires-Dist: spglib<=2.0.2
+Requires-Dist: spglib>=2.4.0
 Requires-Dist: pymatgen-analysis-defects>=2023.8.22
 Requires-Dist: shakenbreak>=3.3.1
 Requires-Dist: pandas
 Requires-Dist: pydefect>=0.8.1
 Requires-Dist: filelock
 Requires-Dist: vise>=0.9.0
 Requires-Dist: easyunfold>=0.3.6
@@ -97,16 +97,22 @@
 ![https://github.com/openjournals/joss-reviews/issues/6433](docs/JOSS/doped_JOSS_figure.png)
 **(a)** Optimal supercell generation comparison. **(b)** Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-size correction plot, **(d)** defect formation energy diagram, **(e)** chemical potential / stability region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi level / carrier concentration heatmap plots from `doped`. Automated plots of **(i,j)** single-particle eigenvalues and **(k)** site
 displacements from DFT supercell calculations. See the [JOSS paper](https://doi.org/10.21105/joss.06433) for more details.
 
 ## Installation
 ```bash
 pip install doped  # install doped and dependencies
+conda install -c conda-forge spglib  # bundle C libraries with spglib
 ```
 
+Note that either `conda install -c conda-forge spglib` or
+`pip install git+https://github.com/spglib/spglib --config-settings=cmake.define.SPGLIB_SHARED_LIBS=OFF`
+should be used after `pip install doped`, which ensures that the correct C libraries are bundled with
+`spglib`, to prevent unnecessary warnings.
+
 Alternatively if desired, `doped` can also be installed from `conda` with:
 
 ```bash
   conda install -c conda-forge doped
   pip install pydefect  # pydefect not available on conda, so needs to be installed with pip or otherwise, if using the eFNV correction
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: doped Version: 2.4.2 Summary: Python package to
+Metadata-Version: 2.1 Name: doped Version: 2.4.3 Summary: Python package to
 setup, process and analyse solid-state defect calculations with VASP Author-
 email: SeÃ¡n Kavanagh
 seas.harvard.edu> License: MIT License Copyright (c) 2021 SeÃ¡n Kavanagh
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -23,15 +23,15 @@
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
 Engineering :: Information Analysis Classifier: Topic :: Scientific/Engineering
 :: Physics Classifier: Topic :: Scientific/Engineering :: Chemistry Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
 >=3.9 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: tabulate Requires-Dist: matplotlib>=3.5.2 Requires-Dist: numpy>=1.21.0
-Requires-Dist: pymatgen>=2023.11.12 Requires-Dist: spglib<=2.0.2 Requires-Dist:
+Requires-Dist: pymatgen>=2023.11.12 Requires-Dist: spglib>=2.4.0 Requires-Dist:
 pymatgen-analysis-defects>=2023.8.22 Requires-Dist: shakenbreak>=3.3.1
 Requires-Dist: pandas Requires-Dist: pydefect>=0.8.1 Requires-Dist: filelock
 Requires-Dist: vise>=0.9.0 Requires-Dist: easyunfold>=0.3.6 Provides-Extra:
 tests Requires-Dist: pytest<8.2; extra == "tests" Requires-Dist: pytest-
 mpl>=0.16.1; extra == "tests" Provides-Extra: docs Requires-Dist: sphinx; extra
 == "docs" Requires-Dist: sphinx-book-theme; extra == "docs" Requires-Dist:
 sphinx_design; extra == "docs" Provides-Extra: analysis Requires-Dist:
@@ -87,28 +87,33 @@
 (d)** defect formation energy diagram, **(e)** chemical potential / stability
 region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier
 concentrations vs. annealing temperature and **(h)** Fermi level / carrier
 concentration heatmap plots from `doped`. Automated plots of **(i,j)** single-
 particle eigenvalues and **(k)** site displacements from DFT supercell
 calculations. See the [JOSS paper](https://doi.org/10.21105/joss.06433) for
 more details. ## Installation ```bash pip install doped # install doped and
-dependencies ``` Alternatively if desired, `doped` can also be installed from
-`conda` with: ```bash conda install -c conda-forge doped pip install pydefect #
-pydefect not available on conda, so needs to be installed with pip or
-otherwise, if using the eFNV correction ``` If you haven't done so already, you
-will need to set up your VASP `POTCAR` files and `Materials Project` API with
-`pymatgen` using the `.pmgrc.yaml` file, in order for `doped` to automatically
-generate VASP input files for defect calculations and determine competing
-phases for chemical potentials. See the docs [Installation](https://
-doped.readthedocs.io/en/latest/Installation.html) page for details on this. ##
-Citation If you use `doped` in your research, please cite: - S. R. Kavanagh et
-al. [doped: Python toolkit for robust and repeatable charged defect supercell
-calculations](https://doi.org/10.21105/joss.06433). _Journal of Open Source
-Software_ 9 (96), 6433, **2024** ## `ShakeNBreak` As shown in the `doped`
-tutorials, it is highly recommended to use the [`ShakeNBreak`](https://
+dependencies conda install -c conda-forge spglib # bundle C libraries with
+spglib ``` Note that either `conda install -c conda-forge spglib` or `pip
+install git+https://github.com/spglib/spglib --config-
+settings=cmake.define.SPGLIB_SHARED_LIBS=OFF` should be used after `pip install
+doped`, which ensures that the correct C libraries are bundled with `spglib`,
+to prevent unnecessary warnings. Alternatively if desired, `doped` can also be
+installed from `conda` with: ```bash conda install -c conda-forge doped pip
+install pydefect # pydefect not available on conda, so needs to be installed
+with pip or otherwise, if using the eFNV correction ``` If you haven't done so
+already, you will need to set up your VASP `POTCAR` files and `Materials
+Project` API with `pymatgen` using the `.pmgrc.yaml` file, in order for `doped`
+to automatically generate VASP input files for defect calculations and
+determine competing phases for chemical potentials. See the docs [Installation]
+(https://doped.readthedocs.io/en/latest/Installation.html) page for details on
+this. ## Citation If you use `doped` in your research, please cite: - S. R.
+Kavanagh et al. [doped: Python toolkit for robust and repeatable charged defect
+supercell calculations](https://doi.org/10.21105/joss.06433). _Journal of Open
+Source Software_ 9 (96), 6433, **2024** ## `ShakeNBreak` As shown in the
+`doped` tutorials, it is highly recommended to use the [`ShakeNBreak`](https://
 shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects
 in solids, to ensure you have identified the groundstate structures of your
 defects. As detailed in the [theory paper](https://doi.org/10.1038/s41524-023-
 00973-1), skipping this step can result in drastically incorrect formation
 energies, transition levels, carrier capture (basically any property associated
 with defects). This approach is followed in the [doped example notebook](https:
 //github.com/SMTG-Bham/doped/blob/main/dope_workflow_example.ipynb), with a
```

### Comparing `doped-2.4.2/doped.egg-info/SOURCES.txt` & `doped-2.4.3/doped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/pyproject.toml` & `doped-2.4.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "doped"
-version = "2.4.2"
+version = "2.4.3"
 description = "Python package to setup, process and analyse solid-state defect calculations with VASP"
 authors = [{name = "Seán Kavanagh", email = "skavanagh@seas.harvard.edu"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -18,16 +18,19 @@
     ]
 requires-python = ">=3.9"
 dependencies = [
     "tabulate",
     "matplotlib>=3.5.2",
     "numpy>=1.21.0",
     "pymatgen>=2023.11.12",  # limiting factor: POTCAR_STATS_PATH available from pymatgen.io.vasp.inputs
-    "spglib<=2.0.2",  # dependent of pymatgen, but explicitly set to <=2.0.2 here to avoid unnecessary warnings
-    # see https://github.com/spglib/spglib/issues/338; remove this limit when issue resolved
+    "spglib>=2.4.0",  # previously explicitly set to <=2.0.2 to avoid unnecessary warnings
+    # (https://github.com/spglib/spglib/issues/338) but causing dependency issues
+    # (https://github.com/SMTG-Bham/doped/issues/73), being worked on in
+    # https://github.com/spglib/spglib/issues/462 -- update Troubleshooting.rst and spglib warning in
+    # doped.utils.symmetry when finally resolved
     "pymatgen-analysis-defects>=2023.8.22",
     "shakenbreak>=3.3.1",
     "pandas",
     "pydefect>=0.8.1",  # for Kumagai (eFNV) correction & PHS analysis
     "filelock",
     "vise>=0.9.0",  # for eigenvalue analysis, >=0.9.0 required for SOC compatibility
     "easyunfold>=0.3.6",  # for efficient PROCAR parsing (and supporting SOC),
```

### Comparing `doped-2.4.2/tests/test_analysis.py` & `doped-2.4.3/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/tests/test_chemical_potentials.py` & `doped-2.4.3/tests/test_chemical_potentials.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/tests/test_corrections.py` & `doped-2.4.3/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/tests/test_displacements.py` & `doped-2.4.3/tests/test_displacements.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/tests/test_generation.py` & `doped-2.4.3/tests/test_generation.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/tests/test_plotting.py` & `doped-2.4.3/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/tests/test_thermodynamics.py` & `doped-2.4.3/tests/test_thermodynamics.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/tests/test_vasp.py` & `doped-2.4.3/tests/test_vasp.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.2/tests/test_wyckoff.py` & `doped-2.4.3/tests/test_wyckoff.py`

 * *Files identical despite different names*

