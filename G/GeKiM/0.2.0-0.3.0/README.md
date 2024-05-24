# Comparing `tmp/gekim-0.2.0.tar.gz` & `tmp/gekim-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gekim-0.2.0.tar", last modified: Wed May 22 22:55:35 2024, max compression
+gzip compressed data, was "gekim-0.3.0.tar", last modified: Fri May 24 00:48:28 2024, max compression
```

## Comparing `gekim-0.2.0.tar` & `gekim-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,62 @@
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/GeKiM.egg-info/
--rw-r--r--   0 kyle      (1006) kyle      (1006)     3068 2024-05-22 22:55:35.000000 gekim-0.2.0/GeKiM.egg-info/PKG-INFO
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      644 2024-05-22 22:55:35.000000 gekim-0.2.0/GeKiM.egg-info/SOURCES.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        1 2024-05-22 22:55:35.000000 gekim-0.2.0/GeKiM.egg-info/dependency_links.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-22 22:55:35.000000 gekim-0.2.0/GeKiM.egg-info/requires.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)        6 2024-05-22 22:55:35.000000 gekim-0.2.0/GeKiM.egg-info/top_level.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)    35149 2024-01-05 21:34:29.000000 gekim-0.2.0/LICENSE
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       24 2024-05-22 22:55:03.000000 gekim-0.2.0/MANIFEST.in
--rw-r--r--   0 kyle      (1006) kyle      (1006)     3068 2024-05-22 22:55:35.887734 gekim-0.2.0/PKG-INFO
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     2318 2024-05-22 22:34:32.000000 gekim-0.2.0/README.md
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/gekim/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      131 2024-05-14 23:48:49.000000 gekim-0.2.0/gekim/__init__.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/gekim/analysis/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      136 2024-05-22 20:27:14.000000 gekim-0.2.0/gekim/analysis/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     1593 2024-05-15 19:36:51.000000 gekim-0.2.0/gekim/analysis/binding.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)    18178 2024-05-17 22:38:48.000000 gekim-0.2.0/gekim/analysis/covalent_inhibition.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     7479 2024-05-17 22:41:27.000000 gekim-0.2.0/gekim/analysis/fitting.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/gekim/schemes/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      134 2024-05-22 22:16:32.000000 gekim-0.2.0/gekim/schemes/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)    20744 2024-05-22 22:22:06.000000 gekim-0.2.0/gekim/schemes/n_state.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/gekim/simulators/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      191 2024-05-14 23:49:52.000000 gekim-0.2.0/gekim/simulators/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     1867 2024-05-15 23:52:27.000000 gekim-0.2.0/gekim/simulators/base_simulator.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     5217 2024-05-17 21:16:04.000000 gekim-0.2.0/gekim/simulators/gillespie.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)    19942 2024-05-17 19:41:44.000000 gekim-0.2.0/gekim/simulators/ode_solver.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/gekim/utils/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      111 2024-05-14 18:10:03.000000 gekim-0.2.0/gekim/utils/__init__.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     4177 2024-05-16 22:45:21.000000 gekim-0.2.0/gekim/utils/helpers.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     1877 2024-05-17 22:44:28.000000 gekim-0.2.0/gekim/utils/logging.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)     3553 2024-05-14 18:10:03.000000 gekim-0.2.0/gekim/utils/plotting.py
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       93 2024-05-22 21:49:09.000000 gekim-0.2.0/pyproject.toml
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-22 21:21:28.000000 gekim-0.2.0/requirements.txt
--rw-rw-r--   0 kyle      (1006) kyle      (1006)       38 2024-05-22 22:55:35.887734 gekim-0.2.0/setup.cfg
--rw-rw-r--   0 kyle      (1006) kyle      (1006)      904 2024-05-22 22:45:47.000000 gekim-0.2.0/setup.py
-drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-22 22:55:35.887734 gekim-0.2.0/tests/
--rw-rw-r--   0 kyle      (1006) kyle      (1006)    13184 2024-05-22 20:43:57.000000 gekim-0.2.0/tests/test_nstate_ode.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/GeKiM.egg-info/
+-rw-r--r--   0 kyle      (1006) kyle      (1006)     3064 2024-05-24 00:48:28.000000 gekim-0.3.0/GeKiM.egg-info/PKG-INFO
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     1258 2024-05-24 00:48:28.000000 gekim-0.3.0/GeKiM.egg-info/SOURCES.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        1 2024-05-24 00:48:28.000000 gekim-0.3.0/GeKiM.egg-info/dependency_links.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-24 00:48:28.000000 gekim-0.3.0/GeKiM.egg-info/requires.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        6 2024-05-24 00:48:28.000000 gekim-0.3.0/GeKiM.egg-info/top_level.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    35149 2024-01-05 21:34:29.000000 gekim-0.3.0/LICENSE
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       24 2024-05-22 22:55:03.000000 gekim-0.3.0/MANIFEST.in
+-rw-r--r--   0 kyle      (1006) kyle      (1006)     3064 2024-05-24 00:48:28.064759 gekim-0.3.0/PKG-INFO
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     2314 2024-05-23 22:14:30.000000 gekim-0.3.0/README.md
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      127 2024-05-23 23:54:52.000000 gekim-0.3.0/gekim/__init__.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/fields/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       92 2024-05-23 21:48:57.000000 gekim-0.3.0/gekim/fields/__init__.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/fields/bio/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       87 2024-05-23 21:54:53.000000 gekim-0.3.0/gekim/fields/bio/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     1028 2024-05-23 21:34:40.000000 gekim-0.3.0/gekim/fields/bio/binding.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:25.000000 gekim-0.3.0/gekim/fields/bio/cellular.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/fields/bio/enzyme/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       90 2024-05-23 21:52:20.000000 gekim-0.3.0/gekim/fields/bio/enzyme/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      582 2024-05-23 21:24:57.000000 gekim-0.3.0/gekim/fields/bio/enzyme/catalysis.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/fields/bio/enzyme/inhib/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       67 2024-05-23 21:53:06.000000 gekim-0.3.0/gekim/fields/bio/enzyme/inhib/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    18191 2024-05-23 21:35:20.000000 gekim-0.3.0/gekim/fields/bio/enzyme/inhib/irrev.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:23:49.000000 gekim-0.3.0/gekim/fields/bio/enzyme/inhib/rev.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:32.000000 gekim-0.3.0/gekim/fields/bio/folding.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:14.000000 gekim-0.3.0/gekim/fields/bio/pharmaco.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:27:22.000000 gekim-0.3.0/gekim/fields/bio/population.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.060759 gekim-0.3.0/gekim/fields/chem/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-24 00:08:58.000000 gekim-0.3.0/gekim/fields/chem/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:36:10.000000 gekim-0.3.0/gekim/fields/chem/atmospheric.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      112 2024-05-23 21:33:23.000000 gekim-0.3.0/gekim/fields/chem/chem.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:37:28.000000 gekim-0.3.0/gekim/fields/chem/electro.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:40:39.000000 gekim-0.3.0/gekim/fields/chem/flow.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:37:20.000000 gekim-0.3.0/gekim/fields/chem/surface.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/gekim/fields/phys/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       57 2024-05-23 21:49:53.000000 gekim-0.3.0/gekim/fields/phys/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:40:57.000000 gekim-0.3.0/gekim/fields/phys/photo.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:41:04.000000 gekim-0.3.0/gekim/fields/phys/plasma.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)        0 2024-05-23 21:38:45.000000 gekim-0.3.0/gekim/fields/phys/quantum.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      151 2024-05-23 21:39:48.000000 gekim-0.3.0/gekim/fields/phys/stat_mech.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/gekim/schemes/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      134 2024-05-22 22:16:32.000000 gekim-0.3.0/gekim/schemes/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    20744 2024-05-22 22:22:06.000000 gekim-0.3.0/gekim/schemes/n_state.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/gekim/simulators/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      191 2024-05-14 23:49:52.000000 gekim-0.3.0/gekim/simulators/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     1867 2024-05-15 23:52:27.000000 gekim-0.3.0/gekim/simulators/base_simulator.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     5290 2024-05-22 23:14:13.000000 gekim-0.3.0/gekim/simulators/gillespie.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    19942 2024-05-17 19:41:44.000000 gekim-0.3.0/gekim/simulators/ode_solver.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/gekim/utils/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      129 2024-05-23 16:25:14.000000 gekim-0.3.0/gekim/utils/__init__.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     7479 2024-05-17 22:41:27.000000 gekim-0.3.0/gekim/utils/fitting.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     4177 2024-05-16 22:45:21.000000 gekim-0.3.0/gekim/utils/helpers.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     1877 2024-05-17 22:44:28.000000 gekim-0.3.0/gekim/utils/logging.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)     3553 2024-05-14 18:10:03.000000 gekim-0.3.0/gekim/utils/plotting.py
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       93 2024-05-22 21:49:09.000000 gekim-0.3.0/pyproject.toml
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       77 2024-05-22 21:21:28.000000 gekim-0.3.0/requirements.txt
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)       38 2024-05-24 00:48:28.064759 gekim-0.3.0/setup.cfg
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)      904 2024-05-24 00:47:42.000000 gekim-0.3.0/setup.py
+drwxrwxr-x   0 kyle      (1006) kyle      (1006)        0 2024-05-24 00:48:28.064759 gekim-0.3.0/tests/
+-rw-rw-r--   0 kyle      (1006) kyle      (1006)    13184 2024-05-22 20:43:57.000000 gekim-0.3.0/tests/test_nstate_ode.py
```

### Comparing `gekim-0.2.0/GeKiM.egg-info/PKG-INFO` & `gekim-0.3.0/GeKiM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeKiM
-Version: 0.2.0
+Version: 0.3.0
 Summary: Generalized Kinetic Modeler: A Python package for modeling arbitrary kinetic schemes.
 Home-page: https://github.com/kghaby/GeKiM
 Author: Kyle Ghaby
 Author-email: kyleghaby@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
@@ -18,15 +18,15 @@
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: setuptools>=67.8.0
 Requires-Dist: sympy>=1.12
 
 # GeKiM (Generalized Kinetic Modeler)
 
 ## Description
-GeKiM (Generalized Kinetic Modeler) is a Python package designed for creating, interpreting, and modeling arbitrary kinetic schemes. Schemes are defined by the user in a dictionary of species and transitions, which is used to initialize an instance of the NState class. Choose (or make) and initialize a simulator for the instance and run it. Included applications are focused on covalent inhibition.
+GeKiM (Generalized Kinetic Modeler) is a Python package designed for creating, interpreting, and modeling arbitrary kinetic schemes. Schemes are defined by the user in a dictionary of species and transitions, which is used to initialize an instance of the NState class. Choose (or make) and initialize a simulator for the instance and run it. Field-specific practices are found in gekim/fields.
 
 ## Installation
 With pip:
 ```bash
 pip install gekim
 ```
 
@@ -37,15 +37,15 @@
 pip install .
 ```
 
 ## Usage
 Here is a basic example of how to use GeKiM to create and simulate a kinetic system:
 ```python
 import gekim as gk
-from gekim.analysis import covalent_inhibition as ci
+from gekim.fields.bio.enzyme.inhib import irrev as ii 
 
 # Define your kinetic scheme in a configuration dictionary
 concI0,concE0 = 100,1
 scheme = {
     'species': {
         "I": {"y0": concI0, "label": "I"},
         "E": {"y0": concE0, "label": "E"},
@@ -66,15 +66,15 @@
 system.set_simulator(gk.simulators.ODESolver)
 system.simulator.simulate() 
 
 # Fit the data to experimental models to extract mock-experimental measurements
 final_state = system.species["EI"].simout["y"]
 all_bound = system.sum_species_simout(blacklist=["E","I"])
 
-fit_output = ci.kobs_uplim_fit_to_occ_final_wrt_t(
+fit_output = ii.kobs_uplim_fit_to_occ_final_wrt_t(
     t,final_state,nondefault_params={"Etot":{"fix":concE0}})
 
 print(f"Fit: {fit_output.fitted_params}\n")
 ```
 For more detailed examples, please refer to the examples directory.
 
 ## Documentation
```

### Comparing `gekim-0.2.0/LICENSE` & `gekim-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gekim-0.2.0/PKG-INFO` & `gekim-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeKiM
-Version: 0.2.0
+Version: 0.3.0
 Summary: Generalized Kinetic Modeler: A Python package for modeling arbitrary kinetic schemes.
 Home-page: https://github.com/kghaby/GeKiM
 Author: Kyle Ghaby
 Author-email: kyleghaby@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
@@ -18,15 +18,15 @@
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: setuptools>=67.8.0
 Requires-Dist: sympy>=1.12
 
 # GeKiM (Generalized Kinetic Modeler)
 
 ## Description
-GeKiM (Generalized Kinetic Modeler) is a Python package designed for creating, interpreting, and modeling arbitrary kinetic schemes. Schemes are defined by the user in a dictionary of species and transitions, which is used to initialize an instance of the NState class. Choose (or make) and initialize a simulator for the instance and run it. Included applications are focused on covalent inhibition.
+GeKiM (Generalized Kinetic Modeler) is a Python package designed for creating, interpreting, and modeling arbitrary kinetic schemes. Schemes are defined by the user in a dictionary of species and transitions, which is used to initialize an instance of the NState class. Choose (or make) and initialize a simulator for the instance and run it. Field-specific practices are found in gekim/fields.
 
 ## Installation
 With pip:
 ```bash
 pip install gekim
 ```
 
@@ -37,15 +37,15 @@
 pip install .
 ```
 
 ## Usage
 Here is a basic example of how to use GeKiM to create and simulate a kinetic system:
 ```python
 import gekim as gk
-from gekim.analysis import covalent_inhibition as ci
+from gekim.fields.bio.enzyme.inhib import irrev as ii 
 
 # Define your kinetic scheme in a configuration dictionary
 concI0,concE0 = 100,1
 scheme = {
     'species': {
         "I": {"y0": concI0, "label": "I"},
         "E": {"y0": concE0, "label": "E"},
@@ -66,15 +66,15 @@
 system.set_simulator(gk.simulators.ODESolver)
 system.simulator.simulate() 
 
 # Fit the data to experimental models to extract mock-experimental measurements
 final_state = system.species["EI"].simout["y"]
 all_bound = system.sum_species_simout(blacklist=["E","I"])
 
-fit_output = ci.kobs_uplim_fit_to_occ_final_wrt_t(
+fit_output = ii.kobs_uplim_fit_to_occ_final_wrt_t(
     t,final_state,nondefault_params={"Etot":{"fix":concE0}})
 
 print(f"Fit: {fit_output.fitted_params}\n")
 ```
 For more detailed examples, please refer to the examples directory.
 
 ## Documentation
```

### Comparing `gekim-0.2.0/README.md` & `gekim-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # GeKiM (Generalized Kinetic Modeler)
 
 ## Description
-GeKiM (Generalized Kinetic Modeler) is a Python package designed for creating, interpreting, and modeling arbitrary kinetic schemes. Schemes are defined by the user in a dictionary of species and transitions, which is used to initialize an instance of the NState class. Choose (or make) and initialize a simulator for the instance and run it. Included applications are focused on covalent inhibition.
+GeKiM (Generalized Kinetic Modeler) is a Python package designed for creating, interpreting, and modeling arbitrary kinetic schemes. Schemes are defined by the user in a dictionary of species and transitions, which is used to initialize an instance of the NState class. Choose (or make) and initialize a simulator for the instance and run it. Field-specific practices are found in gekim/fields.
 
 ## Installation
 With pip:
 ```bash
 pip install gekim
 ```
 
@@ -16,15 +16,15 @@
 pip install .
 ```
 
 ## Usage
 Here is a basic example of how to use GeKiM to create and simulate a kinetic system:
 ```python
 import gekim as gk
-from gekim.analysis import covalent_inhibition as ci
+from gekim.fields.bio.enzyme.inhib import irrev as ii 
 
 # Define your kinetic scheme in a configuration dictionary
 concI0,concE0 = 100,1
 scheme = {
     'species': {
         "I": {"y0": concI0, "label": "I"},
         "E": {"y0": concE0, "label": "E"},
@@ -45,15 +45,15 @@
 system.set_simulator(gk.simulators.ODESolver)
 system.simulator.simulate() 
 
 # Fit the data to experimental models to extract mock-experimental measurements
 final_state = system.species["EI"].simout["y"]
 all_bound = system.sum_species_simout(blacklist=["E","I"])
 
-fit_output = ci.kobs_uplim_fit_to_occ_final_wrt_t(
+fit_output = ii.kobs_uplim_fit_to_occ_final_wrt_t(
     t,final_state,nondefault_params={"Etot":{"fix":concE0}})
 
 print(f"Fit: {fit_output.fitted_params}\n")
 ```
 For more detailed examples, please refer to the examples directory.
 
 ## Documentation
```

### Comparing `gekim-0.2.0/gekim/analysis/binding.py` & `gekim-0.3.0/gekim/fields/bio/binding.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,28 +40,8 @@
         Returns
         -------
         float
             The calculated equilibrium constant (Keq)
         """
         return kon / koff
 
-    @staticmethod
-    def KM(kon, koff, kcat):
-        """
-        KM (i.e. Michaelis-Menten constant, KA, Khalf, KD (not to be confused with Kd)) calculation.
-        
-        Parameters
-        ----------
-        kon : float
-            On-rate constant (CONC^-1*TIME^-1)
-        koff : float
-            Off-rate constant (TIME^-1)
-        kcat : float
-            Irreversible catalysis rate constant
-        
-        Returns
-        -------
-        float
-            The calculated Michaelis-Menten constant (KM)
-        """
-        return (koff + kcat) / kon
```

### Comparing `gekim-0.2.0/gekim/analysis/covalent_inhibition.py` & `gekim-0.3.0/gekim/fields/bio/enzyme/inhib/irrev.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from scipy.optimize import curve_fit
 from scipy.stats import gaussian_kde
-from ..utils.helpers import update_dict_with_subset
-from .fitting import detect_bad_fit, FitOutput, _normalize_params, _unnormalize_popt, _extract_fit_info, _prepare_output
+from .....utils.helpers import update_dict_with_subset
+from .....utils.fitting import detect_bad_fit, FitOutput, _normalize_params, _unnormalize_popt, _extract_fit_info, _prepare_output
 
 #TODO: fit to scheme. meaning yuo make a scheme without values for the transitions and fit it to occ data to see what values of rates satisfy curve
 #TODO: detect trivial solutions for curve fitting, like if all values are the same, or if all values are 0, or if all values are 1.
 #TODO: time arrays that are not evenly spaced will hurt curve fitting.
 #TODO: refactor fitting. kobs fitting shares lots
 
 def occ_final_wrt_t(t,kobs,Etot,uplim=1):
```

### Comparing `gekim-0.2.0/gekim/analysis/fitting.py` & `gekim-0.3.0/gekim/utils/fitting.py`

 * *Files identical despite different names*

### Comparing `gekim-0.2.0/gekim/schemes/n_state.py` & `gekim-0.3.0/gekim/schemes/n_state.py`

 * *Files identical despite different names*

### Comparing `gekim-0.2.0/gekim/simulators/base_simulator.py` & `gekim-0.3.0/gekim/simulators/base_simulator.py`

 * *Files identical despite different names*

### Comparing `gekim-0.2.0/gekim/simulators/gillespie.py` & `gekim-0.3.0/gekim/simulators/gillespie.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 from .base_simulator import BaseSimulator
 
     #TODO: add an option called "continue" which takes an integer which points to the index of the run that its continuing from
-    #TODO: precompile algo
+    #TODO: precompile (repeatable) algo in c or fortran
     #TODO: S2.alt1 breaks this from negative rates somehow
     #TODO: running prob? and test more
     #TODO: type hints on algo
     #TODO: 2S I goes neg
+    #TODO: warn if transition is not linear
 
 class Gillespie(BaseSimulator):
     """
     Gillespie's algorithm for stochastic simulation.
     Does not work if any transitions are > (pseudo-)first order.  
     """
     def setup(self):
```

### Comparing `gekim-0.2.0/gekim/simulators/ode_solver.py` & `gekim-0.3.0/gekim/simulators/ode_solver.py`

 * *Files identical despite different names*

### Comparing `gekim-0.2.0/gekim/utils/helpers.py` & `gekim-0.3.0/gekim/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `gekim-0.2.0/gekim/utils/logging.py` & `gekim-0.3.0/gekim/utils/logging.py`

 * *Files identical despite different names*

### Comparing `gekim-0.2.0/gekim/utils/plotting.py` & `gekim-0.3.0/gekim/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `gekim-0.2.0/setup.py` & `gekim-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='GeKiM', 
-    version='0.2.0', 
+    version='0.3.0', 
     author='Kyle Ghaby', 
     author_email='kyleghaby@gmail.com',  
     description='Generalized Kinetic Modeler: A Python package for modeling arbitrary kinetic schemes.',  
     long_description=open('README.md').read(),  
     long_description_content_type='text/markdown',
     url='https://github.com/kghaby/GeKiM', 
     packages=find_packages(),
```

### Comparing `gekim-0.2.0/tests/test_nstate_ode.py` & `gekim-0.3.0/tests/test_nstate_ode.py`

 * *Files identical despite different names*

