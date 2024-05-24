# Comparing `tmp/structuretoolkit-0.0.8.tar.gz` & `tmp/structuretoolkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structuretoolkit-0.0.8.tar", last modified: Mon Aug 14 00:31:07 2023, max compression
+gzip compressed data, was "structuretoolkit-0.0.9.tar", last modified: Mon Sep  4 20:04:25 2023, max compression
```

## Comparing `structuretoolkit-0.0.8.tar` & `structuretoolkit-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 00:31:07.475188 structuretoolkit-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-14 00:31:07.475188 structuretoolkit-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-14 00:31:07.475188 structuretoolkit-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-08-14 00:31:07.000000 structuretoolkit-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 00:31:07.479189 structuretoolkit-0.0.8/structuretoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-14 00:31:07.479189 structuretoolkit-0.0.8/structuretoolkit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 00:31:07.475188 structuretoolkit-0.0.8/structuretoolkit/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/analyse/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    47409 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/analyse/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/analyse/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/analyse/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/analyse/spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/analyse/strain.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/analyse/symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 00:31:07.475188 structuretoolkit-0.0.8/structuretoolkit/build/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/build/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/build/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/build/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/build/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/build/surface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 00:31:07.475188 structuretoolkit-0.0.8/structuretoolkit/common/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/common/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/common/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/common/pymatgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/common/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)    30805 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/structuretoolkit/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 00:31:07.471188 structuretoolkit-0.0.8/structuretoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-14 00:31:07.000000 structuretoolkit-0.0.8/structuretoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-14 00:31:07.000000 structuretoolkit-0.0.8/structuretoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-14 00:31:07.000000 structuretoolkit-0.0.8/structuretoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-14 00:31:07.000000 structuretoolkit-0.0.8/structuretoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-14 00:31:07.000000 structuretoolkit-0.0.8/structuretoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-14 00:31:07.475188 structuretoolkit-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/tests/test_aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/tests/test_analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/tests/test_compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/tests/test_high_index_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    24622 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/tests/test_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/tests/test_pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/tests/test_pyxtal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/tests/test_strain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/tests/test_visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-08-14 00:31:01.000000 structuretoolkit-0.0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 20:04:25.384247 structuretoolkit-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (999)     1593 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)       75 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)     1081 2023-09-04 20:04:25.384247 structuretoolkit-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2442 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (999)      198 2023-09-04 20:04:25.384247 structuretoolkit-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1861 2023-09-04 20:04:25.000000 structuretoolkit-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 20:04:25.384247 structuretoolkit-0.0.9/structuretoolkit/
+-rw-r--r--   0 runner    (1001) docker     (999)     1953 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      496 2023-09-04 20:04:25.384247 structuretoolkit-0.0.9/structuretoolkit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 20:04:25.380247 structuretoolkit-0.0.9/structuretoolkit/analyse/
+-rw-r--r--   0 runner    (1001) docker     (999)     1603 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2086 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/analyse/distance.py
+-rw-r--r--   0 runner    (1001) docker     (999)    47409 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/analyse/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1530 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/analyse/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9818 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/analyse/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (999)    25280 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/analyse/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9295 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/analyse/strain.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13603 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/analyse/symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 20:04:25.380247 structuretoolkit-0.0.9/structuretoolkit/build/
+-rw-r--r--   0 runner    (1001) docker     (999)      364 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3871 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/build/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6853 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/build/compound.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4169 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/build/random.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5646 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/build/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6876 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/build/surface.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 20:04:25.384247 structuretoolkit-0.0.9/structuretoolkit/common/
+-rw-r--r--   0 runner    (1001) docker     (999)      435 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)       41 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/common/error.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7649 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/common/helper.py
+-rw-r--r--   0 runner    (1001) docker     (999)      492 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/common/pymatgen.py
+-rw-r--r--   0 runner    (1001) docker     (999)      429 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/common/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (999)    30805 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/structuretoolkit/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 20:04:25.380247 structuretoolkit-0.0.9/structuretoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     1081 2023-09-04 20:04:25.000000 structuretoolkit-0.0.9/structuretoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1246 2023-09-04 20:04:25.000000 structuretoolkit-0.0.9/structuretoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 20:04:25.000000 structuretoolkit-0.0.9/structuretoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      355 2023-09-04 20:04:25.000000 structuretoolkit-0.0.9/structuretoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       17 2023-09-04 20:04:25.000000 structuretoolkit-0.0.9/structuretoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 20:04:25.384247 structuretoolkit-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)     1202 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/tests/test_aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (999)    14011 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/tests/test_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5512 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/tests/test_compound.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2236 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/tests/test_high_index_surface.py
+-rw-r--r--   0 runner    (1001) docker     (999)    24622 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/tests/test_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (999)    23084 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/tests/test_pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2404 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/tests/test_pyxtal.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2209 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/tests/test_strain.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9401 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (999)      718 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/tests/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (999)    68611 2023-09-04 20:04:22.000000 structuretoolkit-0.0.9/versioneer.py
```

### Comparing `structuretoolkit-0.0.8/LICENSE` & `structuretoolkit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/PKG-INFO` & `structuretoolkit-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structuretoolkit
-Version: 0.0.8
+Version: 0.0.9
 Summary: structuretoolkit - to analyse, build and visualise atomistic structures.
 Home-page: https://github.com/pyiron/structuretoolkit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `structuretoolkit-0.0.8/README.md` & `structuretoolkit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/setup.py` & `structuretoolkit-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,22 +29,22 @@
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
         'ase>=3.22.1',
         'matplotlib>=3.7.2',  # ase already requires matplotlib
         'numpy>=1.23.5',  # ase already requires numpy
-        'scipy>=1.11.1',  # ase already requires scipy
+        'scipy>=1.11.2',  # ase already requires scipy
     ],
     extras_require={
-        "grainboundary": ['aimsgb>=1.0.3', 'pymatgen>=2023.7.20'],
+        "grainboundary": ['aimsgb>=1.0.3', 'pymatgen>=2023.8.10'],
         "pyscal": ['pyscal2>=2.10.18'],
         "nglview": ['nglview>=3.0.6'],
-        "plotly": ['plotly>=5.15.0'],
+        "plotly": ['plotly>=5.16.1'],
         "clusters": ['scikit-learn>=1.3.0'],
         "symmetry": ['spglib>=2.0.2'],
-        "surface": ['spglib>=2.0.2', 'pymatgen>=2023.7.20'],
+        "surface": ['spglib>=2.0.2', 'pymatgen>=2023.8.10'],
         "phonopy": ['phonopy>=2.20.0', 'spglib>=2.0.2'],
-        "pyxtal": ['pyxtal>=0.5.9']
+        "pyxtal": ['pyxtal>=0.6.0']
     },
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `structuretoolkit-0.0.8/structuretoolkit/__init__.py` & `structuretoolkit-0.0.9/structuretoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/analyse/__init__.py` & `structuretoolkit-0.0.9/structuretoolkit/analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/analyse/distance.py` & `structuretoolkit-0.0.9/structuretoolkit/analyse/distance.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/analyse/neighbors.py` & `structuretoolkit-0.0.9/structuretoolkit/analyse/neighbors.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/analyse/phonopy.py` & `structuretoolkit-0.0.9/structuretoolkit/analyse/phonopy.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/analyse/pyscal.py` & `structuretoolkit-0.0.9/structuretoolkit/analyse/pyscal.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/analyse/spatial.py` & `structuretoolkit-0.0.9/structuretoolkit/analyse/spatial.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/analyse/strain.py` & `structuretoolkit-0.0.9/structuretoolkit/analyse/strain.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/analyse/symmetry.py` & `structuretoolkit-0.0.9/structuretoolkit/analyse/symmetry.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/build/aimsgb.py` & `structuretoolkit-0.0.9/structuretoolkit/build/aimsgb.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/build/compound.py` & `structuretoolkit-0.0.9/structuretoolkit/build/compound.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/build/random.py` & `structuretoolkit-0.0.9/structuretoolkit/build/random.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/build/sqs.py` & `structuretoolkit-0.0.9/structuretoolkit/build/sqs.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/build/surface.py` & `structuretoolkit-0.0.9/structuretoolkit/build/surface.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/common/helper.py` & `structuretoolkit-0.0.9/structuretoolkit/common/helper.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit/visualize.py` & `structuretoolkit-0.0.9/structuretoolkit/visualize.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/structuretoolkit.egg-info/PKG-INFO` & `structuretoolkit-0.0.9/structuretoolkit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structuretoolkit
-Version: 0.0.8
+Version: 0.0.9
 Summary: structuretoolkit - to analyse, build and visualise atomistic structures.
 Home-page: https://github.com/pyiron/structuretoolkit
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `structuretoolkit-0.0.8/structuretoolkit.egg-info/SOURCES.txt` & `structuretoolkit-0.0.9/structuretoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/tests/test_aimsgb.py` & `structuretoolkit-0.0.9/tests/test_aimsgb.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/tests/test_analyse.py` & `structuretoolkit-0.0.9/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/tests/test_compound.py` & `structuretoolkit-0.0.9/tests/test_compound.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/tests/test_high_index_surface.py` & `structuretoolkit-0.0.9/tests/test_high_index_surface.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/tests/test_neighbors.py` & `structuretoolkit-0.0.9/tests/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/tests/test_pyscal.py` & `structuretoolkit-0.0.9/tests/test_pyscal.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/tests/test_pyxtal.py` & `structuretoolkit-0.0.9/tests/test_pyxtal.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/tests/test_strain.py` & `structuretoolkit-0.0.9/tests/test_strain.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/tests/test_symmetry.py` & `structuretoolkit-0.0.9/tests/test_symmetry.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/tests/test_visualize.py` & `structuretoolkit-0.0.9/tests/test_visualize.py`

 * *Files identical despite different names*

### Comparing `structuretoolkit-0.0.8/versioneer.py` & `structuretoolkit-0.0.9/versioneer.py`

 * *Files identical despite different names*

