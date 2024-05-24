# Comparing `tmp/biobb_structure_utils-4.1.0.tar.gz` & `tmp/biobb_structure_utils-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_structure_utils-4.1.0.tar", last modified: Wed Sep 13 08:29:35 2023, max compression
+gzip compressed data, was "biobb_structure_utils-4.2.0.tar", last modified: Fri May 24 13:12:03 2024, max compression
```

## Comparing `biobb_structure_utils-4.1.0.tar` & `biobb_structure_utils-4.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-13 08:29:35.840877 biobb_structure_utils-4.1.0/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:35:44.000000 biobb_structure_utils-4.1.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7082 2023-09-13 08:29:35.840714 biobb_structure_utils-4.1.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6123 2023-09-13 08:25:40.000000 biobb_structure_utils-4.1.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-13 08:29:35.836724 biobb_structure_utils-4.1.0/biobb_structure_utils/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       73 2023-09-13 08:25:16.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-13 08:29:35.837831 biobb_structure_utils-4.1.0/biobb_structure_utils/gro_lib/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:35:44.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/gro_lib/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15565 2023-04-13 10:43:11.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/gro_lib/gro.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-13 08:29:35.837978 biobb_structure_utils-4.1.0/biobb_structure_utils/test/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:35:44.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-13 08:29:35.840522 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      317 2022-08-16 11:55:52.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7071 2023-04-13 10:46:32.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/cat_pdb.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9691 2023-04-13 11:08:25.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/closest_residues.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7010 2023-04-13 11:13:57.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7378 2023-04-13 11:21:45.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_atoms.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8019 2023-04-13 11:23:10.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_chain.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8276 2023-04-13 11:24:44.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_heteroatoms.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8100 2023-04-13 11:27:39.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_model.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7688 2023-04-13 11:27:50.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_molecule.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7675 2023-04-13 11:29:05.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_residues.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6312 2023-04-13 11:30:06.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/remove_ligand.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7914 2023-04-13 11:31:01.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/remove_molecules.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5394 2023-04-13 11:31:50.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/remove_pdb_water.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9476 2023-04-13 12:38:54.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/renumber_structure.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5249 2023-04-13 12:39:36.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/sort_gro_residues.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7987 2023-04-13 12:40:29.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/str_check_add_hydrogens.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8381 2023-04-11 08:03:58.000000 biobb_structure_utils-4.1.0/biobb_structure_utils/utils/structure_check.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-09-13 08:29:35.837571 biobb_structure_utils-4.1.0/biobb_structure_utils.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7082 2023-09-13 08:29:35.000000 biobb_structure_utils-4.1.0/biobb_structure_utils.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1239 2023-09-13 08:29:35.000000 biobb_structure_utils-4.1.0/biobb_structure_utils.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-09-13 08:29:35.000000 biobb_structure_utils-4.1.0/biobb_structure_utils.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1035 2023-09-13 08:29:35.000000 biobb_structure_utils-4.1.0/biobb_structure_utils.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       53 2023-09-13 08:29:35.000000 biobb_structure_utils-4.1.0/biobb_structure_utils.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       22 2023-09-13 08:29:35.000000 biobb_structure_utils-4.1.0/biobb_structure_utils.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-09-13 08:29:35.840930 biobb_structure_utils-4.1.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2612 2023-09-13 08:24:39.000000 biobb_structure_utils-4.1.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:12:03.437381 biobb_structure_utils-4.2.0/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:35:44.000000 biobb_structure_utils-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     7703 2024-05-24 13:12:03.437154 biobb_structure_utils-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6661 2024-05-24 13:11:09.000000 biobb_structure_utils-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:12:03.433486 biobb_structure_utils-4.2.0/biobb_structure_utils/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573       73 2024-05-24 13:11:00.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:12:03.434501 biobb_structure_utils-4.2.0/biobb_structure_utils/gro_lib/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:35:44.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/gro_lib/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    15565 2023-04-13 10:43:11.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/gro_lib/gro.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:12:03.434660 biobb_structure_utils-4.2.0/biobb_structure_utils/test/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:35:44.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:12:03.436894 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573      317 2022-08-16 11:55:52.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7134 2024-05-24 13:02:59.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/cat_pdb.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9691 2023-04-13 11:08:25.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/closest_residues.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     7010 2023-04-13 11:13:57.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7464 2024-05-24 13:02:59.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_atoms.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8019 2023-04-13 11:23:10.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_chain.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8350 2024-05-24 13:02:59.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_heteroatoms.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8100 2023-04-13 11:27:39.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_model.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7688 2023-04-13 11:27:50.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_molecule.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7746 2024-05-24 13:02:59.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_residues.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6372 2024-05-24 13:02:59.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/remove_ligand.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7984 2024-05-24 13:02:59.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/remove_molecules.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5394 2023-04-13 11:31:50.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/remove_pdb_water.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9527 2024-05-24 13:02:59.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/renumber_structure.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5308 2024-05-24 13:02:59.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/sort_gro_residues.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7987 2023-04-13 12:40:29.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/str_check_add_hydrogens.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8381 2023-04-11 08:03:58.000000 biobb_structure_utils-4.2.0/biobb_structure_utils/utils/structure_check.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:12:03.434271 biobb_structure_utils-4.2.0/biobb_structure_utils.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     7703 2024-05-24 13:12:03.000000 biobb_structure_utils-4.2.0/biobb_structure_utils.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1239 2024-05-24 13:12:03.000000 biobb_structure_utils-4.2.0/biobb_structure_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2024-05-24 13:12:03.000000 biobb_structure_utils-4.2.0/biobb_structure_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1035 2024-05-24 13:12:03.000000 biobb_structure_utils-4.2.0/biobb_structure_utils.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       53 2024-05-24 13:12:03.000000 biobb_structure_utils-4.2.0/biobb_structure_utils.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       22 2024-05-24 13:12:03.000000 biobb_structure_utils-4.2.0/biobb_structure_utils.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2024-05-24 13:12:03.437434 biobb_structure_utils-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2612 2024-05-24 13:10:53.000000 biobb_structure_utils-4.2.0/setup.py
```

### Comparing `biobb_structure_utils-4.1.0/LICENSE` & `biobb_structure_utils-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/PKG-INFO` & `biobb_structure_utils-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: biobb_structure_utils
-Version: 4.1.0
+Version: 4.2.0
 Summary: biobb_structure_utils is the Biobb module collection to perform basic manipulations on 3d structures.
 Home-page: https://github.com/bioexcel/biobb_structure_utils
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_structure_utils.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-structure-utils.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.2.0
+Requires-Dist: biobb_structure_checking==3.13.4
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_structure_utils?label=Version)](https://GitHub.com/bioexcel/biobb_structure_utils/tags/)
 [![](https://img.shields.io/pypi/v/biobb-structure-utils.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-structure-utils/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_structure_utils?label=Conda)](https://anaconda.org/bioconda/biobb_structure_utils)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_structure_utils?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_structure_utils)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_structure_utils?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_structure_utils)
 [![](https://img.shields.io/pypi/pyversions/biobb-structure-utils.svg?label=Python%20Versions)](https://pypi.org/project/biobb-structure-utils/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_structure_utils)
 
 [![](https://readthedocs.org/projects/biobb-structure-utils/badge/?version=latest&label=Docs)](https://biobb-structure-utils.readthedocs.io/en/latest/?badge=latest)
@@ -40,85 +42,91 @@
 
 [![](https://docs.bioexcel.eu/biobb_structure_utils/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_structure_utils/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_structure_utils/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_structure_utils/coverage/)
 [![](https://docs.bioexcel.eu/biobb_structure_utils/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_structure_utils/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_structure_utils?label=Last%20Commit)](https://github.com/bioexcel/biobb_structure_utils/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_structure_utils.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_structure_utils/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
 
 # biobb_structure_utils
 
 ### Introduction
 Biobb_structure_utils is the Biobb module collection to modify or extract information from a PDB structure file, such as pulling out a particular model or chain, removing water molecules or ligands, or renumbering or sorting atoms or residues. Biobb (BioExcel building blocks) packages are Python building blocks that create new layer of compatibility and interoperability over popular bioinformatics tools. The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](https://biobb-structure-utils.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_structure_utils>=4.1.0"
+        pip install "biobb_structure_utils>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-structure-utils.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_structure_utils>=4.1.0"
+        conda install -c bioconda "biobb_structure_utils>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-structure-utils.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-structure-utils.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_structure_utils:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_structure_utils:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_structure_utils:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_structure_utils:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_structure_utils.sif https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_structure_utils.sif https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_structure_utils.sif <command>
 
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-structure-utils.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ### Acknolegements
 This software uses functions to read and modify GRO files based in the [GROPY](https://github.com/caizkun/gropy) library created by Zhikun Cai (caizkun@gmail.com) under the [MIT](https://github.com/caizkun/gropy/blob/master/LICENSE). In this project [GROPY](https://github.com/caizkun/gropy) has been adapted to Python 3 and our own needs.
```

### Comparing `biobb_structure_utils-4.1.0/README.md` & `biobb_structure_utils-4.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_structure_utils?label=Version)](https://GitHub.com/bioexcel/biobb_structure_utils/tags/)
 [![](https://img.shields.io/pypi/v/biobb-structure-utils.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-structure-utils/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_structure_utils?label=Conda)](https://anaconda.org/bioconda/biobb_structure_utils)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_structure_utils?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_structure_utils)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_structure_utils?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_structure_utils)
 [![](https://img.shields.io/pypi/pyversions/biobb-structure-utils.svg?label=Python%20Versions)](https://pypi.org/project/biobb-structure-utils/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_structure_utils)
 
 [![](https://readthedocs.org/projects/biobb-structure-utils/badge/?version=latest&label=Docs)](https://biobb-structure-utils.readthedocs.io/en/latest/?badge=latest)
@@ -18,85 +18,91 @@
 
 [![](https://docs.bioexcel.eu/biobb_structure_utils/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_structure_utils/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_structure_utils/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_structure_utils/coverage/)
 [![](https://docs.bioexcel.eu/biobb_structure_utils/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_structure_utils/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_structure_utils?label=Last%20Commit)](https://github.com/bioexcel/biobb_structure_utils/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_structure_utils.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_structure_utils/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
 
 # biobb_structure_utils
 
 ### Introduction
 Biobb_structure_utils is the Biobb module collection to modify or extract information from a PDB structure file, such as pulling out a particular model or chain, removing water molecules or ligands, or renumbering or sorting atoms or residues. Biobb (BioExcel building blocks) packages are Python building blocks that create new layer of compatibility and interoperability over popular bioinformatics tools. The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](https://biobb-structure-utils.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_structure_utils>=4.1.0"
+        pip install "biobb_structure_utils>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-structure-utils.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_structure_utils>=4.1.0"
+        conda install -c bioconda "biobb_structure_utils>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-structure-utils.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-structure-utils.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_structure_utils:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_structure_utils:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_structure_utils:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_structure_utils:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_structure_utils.sif https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_structure_utils.sif https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_structure_utils.sif <command>
 
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-structure-utils.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ### Acknolegements
 This software uses functions to read and modify GRO files based in the [GROPY](https://github.com/caizkun/gropy) library created by Zhikun Cai (caizkun@gmail.com) under the [MIT](https://github.com/caizkun/gropy/blob/master/LICENSE). In this project [GROPY](https://github.com/caizkun/gropy) has been adapted to Python 3 and our own needs.
```

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/gro_lib/gro.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/gro_lib/gro.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/cat_pdb.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/cat_pdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from biobb_structure_utils.utils.common import check_input_path, check_output_path
 
 
 class CatPDB(BiobbObject):
     """
     | biobb_structure_utils CatPDB
     | Class to concat two PDB structures in a single PDB file.
+    | Class to concat two PDB structures in a single PDB file.
 
     Args:
         input_structure1 (str): Input structure 1 file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/data/utils/cat_protein.pdb>`_. Accepted formats: pdb (edam:format_1476), pdbqt (edam:format_1476).
         input_structure2 (str): Input structure 2 file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/data/utils/cat_ligand.pdb>`_. Accepted formats: pdb (edam:format_1476), pdbqt (edam:format_1476).
         output_structure_path (str): Output protein file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/reference/utils/ref_cat_pdb.pdb>`_. Accepted formats: pdb (edam:format_1476), pdbqt (edam:format_1476).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
```

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/closest_residues.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/closest_residues.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/common.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/common.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_atoms.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from biobb_structure_utils.utils.common import PDB_SERIAL_RECORDS
 
 
 class ExtractAtoms(BiobbObject):
     """
     | biobb_structure_utils ExtractAtoms
     | Class to extract atoms from a 3D structure.
+    | Extracts all atoms from a 3D structure that match a regular expression pattern.
 
     Args:
         input_structure_path (str): Input structure file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/data/utils/2vgb.pdb>`_. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         output_structure_path (str): Output structure file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/reference/utils/OE2_atoms.pdb>`_. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **regular_expression_pattern** (*str*) - ("^D") Python style regular expression matching the selected atom names.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
```

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_chain.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_chain.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_heteroatoms.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_heteroatoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from biobb_structure_utils.utils.common import check_input_path, check_format_heteroatoms, check_output_path, create_biopython_residue, create_output_file
 
 
 class ExtractHeteroAtoms(BiobbObject):
     """
     | biobb_structure_utils ExtractHeteroAtoms
     | Class to extract hetero-atoms from a 3D structure using Biopython.
+    | Extracts a list of heteroatoms from a 3D structure using Biopython.
 
     Args:
         input_structure_path (str): Input structure file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/data/utils/extract_heteroatom.pdb>`_. Accepted formats: pdb (edam:format_1476), pdbqt (edam:format_1476).
         output_heteroatom_path (str): Output heteroatom file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/reference/utils/ref_extract_heteroatom.pdb>`_. Accepted formats: pdb (edam:format_1476), pdbqt (edam:format_1476).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **heteroatoms** (*list*) - (None) List of dictionaries with the name | res_id | chain | model of the heteroatoms to be extracted. Format: [{"name": "ZZ7", "res_id": "302", "chain": "B", "model": "1"}]. If empty, all the heteroatoms of the structure will be returned.
             * **water** (*bool*) - (False) Add or not waters.
```

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_model.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_model.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_molecule.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_molecule.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/extract_residues.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/extract_residues.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from biobb_structure_utils.utils.common import check_input_path, check_output_path, create_residues_list, create_biopython_residue, create_output_file
 
 
 class ExtractResidues(BiobbObject):
     """
     | biobb_structure_utils ExtractResidues
     | Class to extract residues from a 3D structure using Biopython.
+    | Extracts a list of residues from a 3D structure using Biopython.
 
     Args:
         input_structure_path (str): Input structure file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/data/utils/extract_heteroatom.pdb>`_. Accepted formats: pdb (edam:format_1476), pdbqt (edam:format_1476).
         output_residues_path (str): Output residues file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/reference/utils/ref_extract_residues.pdb>`_. Accepted formats: pdb (edam:format_1476), pdbqt (edam:format_1476).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **residues** (*list*) - (None) List of comma separated res_id (will extract all residues that match the res_id) or list of dictionaries with the name | res_id  | chain | model of the residues to be extracted. Format: [{"name": "HIS", "res_id": "72", "chain": "A", "model": "1"}].
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
```

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/remove_ligand.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/remove_ligand.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from biobb_structure_utils.gro_lib.gro import Gro
 
 
 class RemoveLigand(BiobbObject):
     """
     | biobb_structure_utils RemoveLigand
     | Class to remove the selected ligand atoms from a 3D structure.
+    | Remove the selected ligand atoms from a 3D structure.
 
     Args:
         input_structure_path (str): Input structure file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/data/utils/WT_aq4_md_1.pdb>`_. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         output_structure_path (str): Output structure file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/reference/utils/WT_apo_md_1.pdb>`_. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **ligand** (*str*) - ("AQ4") Residue code of the ligand to be removed.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
```

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/remove_molecules.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/remove_molecules.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from biobb_structure_utils.utils.common import check_input_path, check_output_path, create_residues_list, create_biopython_residue, create_output_file
 
 
 class RemoveMolecules(BiobbObject):
     """
     | biobb_structure_utils RemoveMolecules
     | Class to remove molecules from a 3D structure using Biopython.
+    | Remove a list of molecules from a 3D structure using Biopython.
 
     Args:
         input_structure_path (str): Input structure file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/data/utils/2vgb.pdb>`_. Accepted formats: pdb (edam:format_1476), pdbqt (edam:format_1476).
         output_molecules_path (str): Output molcules file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/reference/utils/ref_remove_molecules.pdb>`_. Accepted formats: pdb (edam:format_1476), pdbqt (edam:format_1476).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **molecules** (*list*) - (None) List of comma separated res_id (will remove all molecules that match the res_id) or list of dictionaries with the name | res_id  | chain | model of the molecules to be removed. Format: [{"name": "HIS", "res_id": "72", "chain": "A", "model": "1"}].
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
```

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/remove_pdb_water.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/remove_pdb_water.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/renumber_structure.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/renumber_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from biobb_structure_utils.utils.common import PDB_SERIAL_RECORDS
 
 
 class RenumberStructure(BiobbObject):
     """
     | biobb_structure_utils RenumberStructure
     | Class to renumber atomic indexes from a 3D structure.
+    | Renumber atomic indexes from a 3D structure.
 
     Args:
         input_structure_path (str): Input structure file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/data/utils/cl3.noH.pdb>`_. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         output_structure_path (str): Output structure file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/reference/utils/renum_cl3_noH.pdb>`_. Accepted formats: pdb (edam:format_1476), gro (edam:format_2033).
         output_mapping_json_path (str): Output mapping json file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/reference/utils/cl3_output_mapping_json_path.json>`_. Accepted formats: json (edam:format_3464).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **renumber_residues** (*bool*) - (True) Residue code of the ligand to be removed.
```

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/sort_gro_residues.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/sort_gro_residues.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from biobb_structure_utils.gro_lib.gro import Gro
 
 
 class SortGroResidues(BiobbObject):
     """
     | biobb_structure_utils SortGroResidues
     | Class to sort the selected residues from a GRO 3D structure.
+    | Sorts the selected residues from a GRO 3D structure.
 
     Args:
         input_gro_path (str): Input GRO file path. File type: input. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/data/utils/WT_aq4_md_1.gro>`_. Accepted formats: gro (edam:format_2033).
         output_gro_path (str): Output sorted GRO file path. File type: output. `Sample file <https://github.com/bioexcel/biobb_structure_utils/raw/master/biobb_structure_utils/test/reference/utils/WT_aq4_md_sorted.gro>`_. Accepted formats: gro (edam:format_2033).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **residue_name_list** (*list*) - (["NA", "CL", "SOL"]) Ordered residue name list.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
```

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/str_check_add_hydrogens.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/str_check_add_hydrogens.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils/utils/structure_check.py` & `biobb_structure_utils-4.2.0/biobb_structure_utils/utils/structure_check.py`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils.egg-info/PKG-INFO` & `biobb_structure_utils-4.2.0/biobb_structure_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: biobb-structure-utils
-Version: 4.1.0
+Version: 4.2.0
 Summary: biobb_structure_utils is the Biobb module collection to perform basic manipulations on 3d structures.
 Home-page: https://github.com/bioexcel/biobb_structure_utils
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_structure_utils.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-structure-utils.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.2.0
+Requires-Dist: biobb_structure_checking==3.13.4
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_structure_utils?label=Version)](https://GitHub.com/bioexcel/biobb_structure_utils/tags/)
 [![](https://img.shields.io/pypi/v/biobb-structure-utils.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-structure-utils/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_structure_utils?label=Conda)](https://anaconda.org/bioconda/biobb_structure_utils)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_structure_utils?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_structure_utils)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_structure_utils?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_structure_utils)
 [![](https://img.shields.io/pypi/pyversions/biobb-structure-utils.svg?label=Python%20Versions)](https://pypi.org/project/biobb-structure-utils/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_structure_utils)
 
 [![](https://readthedocs.org/projects/biobb-structure-utils/badge/?version=latest&label=Docs)](https://biobb-structure-utils.readthedocs.io/en/latest/?badge=latest)
@@ -40,85 +42,91 @@
 
 [![](https://docs.bioexcel.eu/biobb_structure_utils/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_structure_utils/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_structure_utils/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_structure_utils/coverage/)
 [![](https://docs.bioexcel.eu/biobb_structure_utils/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_structure_utils/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_structure_utils?label=Last%20Commit)](https://github.com/bioexcel/biobb_structure_utils/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_structure_utils.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_structure_utils/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
 
 # biobb_structure_utils
 
 ### Introduction
 Biobb_structure_utils is the Biobb module collection to modify or extract information from a PDB structure file, such as pulling out a particular model or chain, removing water molecules or ligands, or renumbering or sorting atoms or residues. Biobb (BioExcel building blocks) packages are Python building blocks that create new layer of compatibility and interoperability over popular bioinformatics tools. The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](https://biobb-structure-utils.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_structure_utils>=4.1.0"
+        pip install "biobb_structure_utils>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-structure-utils.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_structure_utils>=4.1.0"
+        conda install -c bioconda "biobb_structure_utils>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-structure-utils.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-structure-utils.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_structure_utils:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_structure_utils:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_structure_utils:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_structure_utils:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_structure_utils.sif https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_structure_utils.sif https://depot.galaxyproject.org/singularity/biobb_structure_utils:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_structure_utils.sif <command>
 
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-structure-utils.readthedocs.io/en/latest/command_line.html).
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ### Acknolegements
 This software uses functions to read and modify GRO files based in the [GROPY](https://github.com/caizkun/gropy) library created by Zhikun Cai (caizkun@gmail.com) under the [MIT](https://github.com/caizkun/gropy/blob/master/LICENSE). In this project [GROPY](https://github.com/caizkun/gropy) has been adapted to Python 3 and our own needs.
```

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils.egg-info/SOURCES.txt` & `biobb_structure_utils-4.2.0/biobb_structure_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/biobb_structure_utils.egg-info/entry_points.txt` & `biobb_structure_utils-4.2.0/biobb_structure_utils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_structure_utils-4.1.0/setup.py` & `biobb_structure_utils-4.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_structure_utils",
-    version="4.1.0",
+    version="4.2.0",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="biobb_structure_utils is the Biobb module collection to perform basic manipulations on 3d structures.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_structure_utils",
     project_urls={
-        "Documentation": "http://biobb_structure_utils.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-structure-utils.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==4.1.0', 'biobb_structure_checking==3.13.4'],
+    install_requires=['biobb_common==4.2.0', 'biobb_structure_checking==3.13.4'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "cat_pdb = biobb_structure_utils.utils.cat_pdb:main",
             "closest_residues = biobb_structure_utils.utils.closest_residues:main",
             "extract_atoms = biobb_structure_utils.utils.extract_atoms:main",
             "extract_chain = biobb_structure_utils.utils.extract_chain:main",
```

