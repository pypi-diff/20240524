# Comparing `tmp/biobb_gromacs-4.1.1.tar.gz` & `tmp/biobb_gromacs-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_gromacs-4.1.1.tar", last modified: Sat Sep 30 22:02:28 2023, max compression
+gzip compressed data, was "biobb_gromacs-4.2.0.tar", last modified: Fri May 24 10:41:45 2024, max compression
```

## Comparing `biobb_gromacs-4.1.1.tar` & `biobb_gromacs-4.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-30 22:02:28.006234 biobb_gromacs-4.1.1/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2022-09-01 17:04:45.000000 biobb_gromacs-4.1.1/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     6277 2023-09-30 22:02:28.005710 biobb_gromacs-4.1.1/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     5356 2023-09-30 22:00:19.000000 biobb_gromacs-4.1.1/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-30 22:02:27.995342 biobb_gromacs-4.1.1/biobb_gromacs/
--rw-r--r--   0 pau        (501) staff       (20)       84 2023-09-30 21:59:18.000000 biobb_gromacs-4.1.1/biobb_gromacs/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-30 22:02:28.003260 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/
--rwxr-xr-x   0 pau        (501) staff       (20)      154 2023-02-23 12:14:24.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)     9475 2023-09-28 08:13:58.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/common.py
--rwxr-xr-x   0 pau        (501) staff       (20)     8029 2023-09-28 08:17:59.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/editconf.py
--rwxr-xr-x   0 pau        (501) staff       (20)    10544 2023-09-28 08:18:01.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/genion.py
--rwxr-xr-x   0 pau        (501) staff       (20)     8279 2023-09-28 08:18:01.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/genrestr.py
--rwxr-xr-x   0 pau        (501) staff       (20)     8421 2023-09-28 08:18:02.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/gmxselect.py
--rwxr-xr-x   0 pau        (501) staff       (20)    12898 2023-09-28 08:18:00.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/grompp.py
--rwxr-xr-x   0 pau        (501) staff       (20)    16322 2023-09-08 09:07:29.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/grompp_mdrun.py
--rwxr-xr-x   0 pau        (501) staff       (20)     7736 2023-09-28 08:18:02.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/make_ndx.py
--rwxr-xr-x   0 pau        (501) staff       (20)    15596 2023-09-28 08:18:00.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/mdrun.py
--rwxr-xr-x   0 pau        (501) staff       (20)     9733 2023-09-28 08:18:01.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/pdb2gmx.py
--rwxr-xr-x   0 pau        (501) staff       (20)     9593 2023-09-28 08:18:01.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/solvate.py
--rwxr-xr-x   0 pau        (501) staff       (20)     7538 2023-09-28 08:18:02.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs/trjcat.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-30 22:02:28.004856 biobb_gromacs-4.1.1/biobb_gromacs/gromacs_extra/
--rw-r--r--   0 pau        (501) staff       (20)       66 2023-02-23 12:23:19.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs_extra/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)     9224 2023-02-23 12:23:35.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs_extra/append_ligand.py
--rwxr-xr-x   0 pau        (501) staff       (20)     9357 2023-02-23 12:21:22.000000 biobb_gromacs-4.1.1/biobb_gromacs/gromacs_extra/ndx2resttop.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-30 22:02:28.005242 biobb_gromacs-4.1.1/biobb_gromacs/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2022-09-01 17:04:44.000000 biobb_gromacs-4.1.1/biobb_gromacs/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-09-30 22:02:27.997831 biobb_gromacs-4.1.1/biobb_gromacs.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     6277 2023-09-30 22:02:27.000000 biobb_gromacs-4.1.1/biobb_gromacs.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      869 2023-09-30 22:02:27.000000 biobb_gromacs-4.1.1/biobb_gromacs.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-09-30 22:02:27.000000 biobb_gromacs-4.1.1/biobb_gromacs.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)      645 2023-09-30 22:02:27.000000 biobb_gromacs-4.1.1/biobb_gromacs.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       20 2023-09-30 22:02:27.000000 biobb_gromacs-4.1.1/biobb_gromacs.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       14 2023-09-30 22:02:27.000000 biobb_gromacs-4.1.1/biobb_gromacs.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2023-09-30 22:02:28.006423 biobb_gromacs-4.1.1/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     2118 2023-09-30 21:58:41.000000 biobb_gromacs-4.1.1/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:41:45.808770 biobb_gromacs-4.2.0/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2022-09-01 17:04:45.000000 biobb_gromacs-4.2.0/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     6817 2024-05-24 10:41:45.808080 biobb_gromacs-4.2.0/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     5896 2024-05-24 10:31:09.000000 biobb_gromacs-4.2.0/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:41:45.793683 biobb_gromacs-4.2.0/biobb_gromacs/
+-rw-r--r--   0 pau        (501) staff       (20)      135 2024-05-24 10:29:44.000000 biobb_gromacs-4.2.0/biobb_gromacs/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:41:45.803282 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/
+-rwxr-xr-x   0 pau        (501) staff       (20)      402 2024-05-21 10:48:47.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)     9491 2024-02-14 11:08:31.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/common.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     8083 2024-05-13 20:51:08.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/editconf.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    10976 2024-05-13 22:29:45.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/genion.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     8520 2024-05-14 07:43:58.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/genrestr.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     8421 2023-09-28 08:18:02.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/gmxselect.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    12898 2024-04-04 23:14:11.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/grompp.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    16322 2023-09-08 09:07:29.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/grompp_mdrun.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     7736 2023-09-28 08:18:02.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/make_ndx.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    15590 2024-04-30 13:12:33.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/mdrun.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     9782 2024-03-14 10:21:21.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/pdb2gmx.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     9593 2023-09-28 08:18:01.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/solvate.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     7538 2023-09-28 08:18:02.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs/trjcat.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:41:45.806766 biobb_gromacs-4.2.0/biobb_gromacs/gromacs_extra/
+-rw-r--r--   0 pau        (501) staff       (20)      121 2024-05-21 10:49:21.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs_extra/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)     9288 2024-05-13 20:52:20.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs_extra/append_ligand.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     9357 2023-02-23 12:21:22.000000 biobb_gromacs-4.2.0/biobb_gromacs/gromacs_extra/ndx2resttop.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:41:45.807456 biobb_gromacs-4.2.0/biobb_gromacs/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2022-09-01 17:04:44.000000 biobb_gromacs-4.2.0/biobb_gromacs/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:41:45.795876 biobb_gromacs-4.2.0/biobb_gromacs.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     6817 2024-05-24 10:41:45.000000 biobb_gromacs-4.2.0/biobb_gromacs.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      869 2024-05-24 10:41:45.000000 biobb_gromacs-4.2.0/biobb_gromacs.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-24 10:41:45.000000 biobb_gromacs-4.2.0/biobb_gromacs.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)      645 2024-05-24 10:41:45.000000 biobb_gromacs-4.2.0/biobb_gromacs.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       20 2024-05-24 10:41:45.000000 biobb_gromacs-4.2.0/biobb_gromacs.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       14 2024-05-24 10:41:45.000000 biobb_gromacs-4.2.0/biobb_gromacs.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-24 10:41:45.808982 biobb_gromacs-4.2.0/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     2118 2024-05-24 10:28:50.000000 biobb_gromacs-4.2.0/setup.py
```

### Comparing `biobb_gromacs-4.1.1/LICENSE` & `biobb_gromacs-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_gromacs-4.1.1/PKG-INFO` & `biobb_gromacs-4.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: biobb_gromacs
-Version: 4.1.1
+Version: 4.2.0
 Summary: biobb_gromacs is the Biobb module collection to perform molecular dynamics simulations.
 Home-page: https://github.com/bioexcel/biobb_gromacs
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_gromacs.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-gromacs.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_gromacs?label=Version)](https://GitHub.com/bioexcel/biobb_gromacs/tags/)
 [![](https://img.shields.io/pypi/v/biobb-gromacs.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-gromacs/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_gromacs?label=Conda)](https://anaconda.org/bioconda/biobb_gromacs)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_gromacs?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_gromacs)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_gromacs?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_gromacs:4.1.1--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_gromacs:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_gromacs)
 [![](https://img.shields.io/pypi/pyversions/biobb-gromacs.svg?label=Python%20Versions)](https://pypi.org/project/biobb-gromacs/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_gromacs)
 
 [![](https://readthedocs.org/projects/biobb-gromacs/badge/?version=latest&label=Docs)](https://biobb-gromacs.readthedocs.io/en/latest/?badge=latest)
@@ -40,87 +40,95 @@
 
 [![](https://docs.bioexcel.eu/biobb_gromacs/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_gromacs/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_gromacs/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_gromacs/coverage/)
 [![](https://docs.bioexcel.eu/biobb_gromacs/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_gromacs/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_gromacs?label=Last%20Commit)](https://github.com/bioexcel/biobb_gromacs/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_gromacs.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_gromacs/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
+
 
 # biobb_gromacs
 
 ### Introduction
 biobb_gromacs is the Biobb module collection to perform molecular dynamics simulations using the GROMACS MD suite.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-gromacs.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2023.3
+v4.2.0 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_gromacs>=4.1.1"
+        pip install "biobb_gromacs>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-gromacs.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_gromacs>=4.1.1"
+        conda install -c bioconda "biobb_gromacs>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-gromacs.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-gromacs.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_gromacs:4.1.1--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_gromacs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_gromacs:4.1.1--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_gromacs:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_gromacs.sif https://depot.galaxyproject.org/singularity/biobb_gromacs:4.1.1--pyhdfd78af_1
+        singularity pull --name biobb_gromacs.sif https://depot.galaxyproject.org/singularity/biobb_gromacs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_gromacs.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-gromacs.readthedocs.io/en/latest/command_line.html).
 
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_gromacs-4.1.1/README.md` & `biobb_gromacs-4.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_gromacs?label=Version)](https://GitHub.com/bioexcel/biobb_gromacs/tags/)
 [![](https://img.shields.io/pypi/v/biobb-gromacs.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-gromacs/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_gromacs?label=Conda)](https://anaconda.org/bioconda/biobb_gromacs)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_gromacs?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_gromacs)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_gromacs?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_gromacs:4.1.1--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_gromacs:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_gromacs)
 [![](https://img.shields.io/pypi/pyversions/biobb-gromacs.svg?label=Python%20Versions)](https://pypi.org/project/biobb-gromacs/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_gromacs)
 
 [![](https://readthedocs.org/projects/biobb-gromacs/badge/?version=latest&label=Docs)](https://biobb-gromacs.readthedocs.io/en/latest/?badge=latest)
@@ -18,87 +18,95 @@
 
 [![](https://docs.bioexcel.eu/biobb_gromacs/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_gromacs/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_gromacs/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_gromacs/coverage/)
 [![](https://docs.bioexcel.eu/biobb_gromacs/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_gromacs/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_gromacs?label=Last%20Commit)](https://github.com/bioexcel/biobb_gromacs/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_gromacs.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_gromacs/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
+
 
 # biobb_gromacs
 
 ### Introduction
 biobb_gromacs is the Biobb module collection to perform molecular dynamics simulations using the GROMACS MD suite.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-gromacs.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2023.3
+v4.2.0 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_gromacs>=4.1.1"
+        pip install "biobb_gromacs>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-gromacs.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_gromacs>=4.1.1"
+        conda install -c bioconda "biobb_gromacs>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-gromacs.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-gromacs.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_gromacs:4.1.1--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_gromacs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_gromacs:4.1.1--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_gromacs:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_gromacs.sif https://depot.galaxyproject.org/singularity/biobb_gromacs:4.1.1--pyhdfd78af_1
+        singularity pull --name biobb_gromacs.sif https://depot.galaxyproject.org/singularity/biobb_gromacs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_gromacs.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-gromacs.readthedocs.io/en/latest/command_line.html).
 
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/common.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
                 value = re_match.group('value')
                 mdp_dict[parameter] = value
 
     return mdp_dict
 
 
 def mdp_preset(sim_type: str) -> Dict[str, str]:
-    mdp_dict = {}
+    mdp_dict: Dict[str, str] = {}
     if not sim_type or sim_type == 'index':
         return mdp_dict
 
     minimization = (sim_type == 'minimization') or (sim_type == 'ions')
     nvt = (sim_type == 'nvt')
     npt = (sim_type == 'npt')
     free = (sim_type == 'free')
```

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/editconf.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/editconf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """Module containing the Editconf class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_gromacs.gromacs.common import get_gromacs_version
+from typing import Optional, Dict
 
 
 class Editconf(BiobbObject):
     """
     | biobb_gromacs Editconf
     | Wrapper class for the `GROMACS editconf <http://manual.gromacs.org/current/onlinehelp/gmx-editconf.html>`_ module.
     | The GROMACS solvate module generates a box around the selected structure.
@@ -50,15 +51,15 @@
             * version: >5.1
             * license: LGPL 2.1
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_gro_path: str, output_gro_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_gro_path: str, output_gro_path: str, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -71,15 +72,15 @@
         self.distance_to_molecule = properties.get('distance_to_molecule', 1.0)
         self.box_vector_lenghts = properties.get('box_vector_lenghts')
         self.box_type = properties.get('box_type', 'cubic')
         self.center_molecule = properties.get('center_molecule', True)
 
         # Properties common in all GROMACS BB
         self.gmx_lib = properties.get('gmx_lib', None)
-        self.binary_path = properties.get('binary_path', 'gmx')
+        self.binary_path: str = properties.get('binary_path', 'gmx')
         self.gmx_nobackup = properties.get('gmx_nobackup', True)
         self.gmx_nocopyright = properties.get('gmx_nocopyright', True)
         if self.gmx_nobackup:
             self.binary_path += ' -nobackup'
         if self.gmx_nocopyright:
             self.binary_path += ' -nocopyright'
         if not self.container_path:
@@ -117,31 +118,31 @@
         if self.center_molecule:
             self.cmd.append('-c')
             fu.log('Centering molecule in the box.', self.out_log, self.global_log)
 
         fu.log("Box type: %s" % self.box_type, self.out_log, self.global_log)
 
         if self.gmx_lib:
-            self.env_vars_dict['GMXLIB'] = self.gmx_lib
+            self.env_vars_dict = self.gmx_lib
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
-        self.tmp_files.append(self.stage_io_dict.get("unique_dir"))
+        self.tmp_files.append(str(self.stage_io_dict.get("unique_dir")))
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def editconf(input_gro_path: str, output_gro_path: str, properties: dict = None, **kwargs) -> int:
+def editconf(input_gro_path: str, output_gro_path: str, properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`Editconf <gromacs.editconf.Editconf>` class and
     execute the :meth:`launch() <gromacs.editconf.Editconf.launch>` method."""
 
     return Editconf(input_gro_path=input_gro_path, output_gro_path=output_gro_path,
                     properties=properties, **kwargs).launch()
```

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/genion.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/genion.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import argparse
 from pathlib import Path
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_gromacs.gromacs.common import get_gromacs_version
+from typing import Optional, Dict, Union
 
 
 class Genion(BiobbObject):
     """
     | biobb_gromacs Genion
     | Wrapper class for the `GROMACS genion <http://manual.gromacs.org/current/onlinehelp/gmx-genion.html>`_ module.
     | The GROMACS genion module randomly replaces solvent molecules with monoatomic ions. The group of solvent molecules should be continuous and all molecules should have the same number of atoms.
@@ -57,16 +58,16 @@
             * version: >5.1
             * license: LGPL 2.1
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_tpr_path: str, output_gro_path: str, input_top_zip_path: str,
-                 output_top_zip_path: str, input_ndx_path: str = None, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_tpr_path: Union[str, Path], output_gro_path: Union[str, Path], input_top_zip_path: Union[str, Path],
+                 output_top_zip_path: Union[str, Path], input_ndx_path: Optional[Union[str, Path]] = None, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -86,19 +87,19 @@
 
         # Properties common in all GROMACS BB
         self.gmx_lib = properties.get('gmx_lib', None)
         self.binary_path = properties.get('binary_path', 'gmx')
         self.gmx_nobackup = properties.get('gmx_nobackup', True)
         self.gmx_nocopyright = properties.get('gmx_nocopyright', True)
         if self.gmx_nobackup:
-            self.binary_path += ' -nobackup'
+            self.binary_path = f"{self.binary_path} -nobackup"
         if self.gmx_nocopyright:
-            self.binary_path += ' -nocopyright'
+            self.binary_path = f"{self.binary_path} -nocopyright"
         if not self.container_path:
-            self.gmx_version = get_gromacs_version(self.binary_path)
+            self.gmx_version = get_gromacs_version(str(self.binary_path))
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
@@ -112,18 +113,18 @@
         self.stage_files()
 
         # Unzip topology to topology_out
         top_file = fu.unzip_top(zip_file=self.input_top_zip_path, out_log=self.out_log)
         top_dir = str(Path(top_file).parent)
 
         if self.container_path:
-            shutil.copytree(top_dir, Path(self.stage_io_dict.get("unique_dir")).joinpath(Path(top_dir).name))
+            shutil.copytree(top_dir, Path(str(self.stage_io_dict.get("unique_dir"))).joinpath(Path(top_dir).name))
             top_file = str(Path(self.container_volume_path).joinpath(Path(top_dir).name, Path(top_file).name))
 
-        self.cmd = [self.binary_path, 'genion',
+        self.cmd = [str(self.binary_path), 'genion',
                     '-s', self.stage_io_dict["in"]["input_tpr_path"],
                     '-o', self.stage_io_dict["out"]["output_gro_path"],
                     '-p', top_file]
 
         if self.stage_io_dict["in"].get("input_ndx_path") and Path(
                 self.stage_io_dict["in"].get("input_ndx_path")).exists():
             self.cmd.append('-n')
@@ -151,56 +152,57 @@
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         if self.container_path:
-            top_file = str(Path(self.stage_io_dict.get("unique_dir")).joinpath(Path(top_dir).name, Path(top_file).name))
+            top_file = str(Path(str(self.stage_io_dict.get("unique_dir"))).joinpath(Path(top_dir).name, Path(top_file).name))
 
         # zip topology
         fu.log('Compressing topology to: %s' % self.stage_io_dict["out"]["output_top_zip_path"],
                self.out_log, self.global_log)
         fu.zip_top(zip_file=self.io_dict["out"]["output_top_zip_path"], top_file=top_file, out_log=self.out_log)
 
         # Remove temporal files
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir"), top_dir, self.io_dict['in'].get("stdin_file_path")])
+        self.tmp_files.extend([str(self.stage_io_dict.get("unique_dir")), top_dir, str(self.io_dict['in'].get("stdin_file_path"))])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=True)
         return self.return_code
 
 
-def genion(input_tpr_path: str, output_gro_path: str, input_top_zip_path: str,
-           output_top_zip_path: str, properties: dict = None, **kwargs) -> int:
+def genion(input_tpr_path: Union[str, Path], output_gro_path: Union[str, Path], input_top_zip_path: Union[str, Path],
+           output_top_zip_path: Union[str, Path], input_ndx_path: Optional[Union[str, Path]] = None, properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`Genion <gromacs.genion.Genion>` class and
         execute the :meth:`launch() <gromacs.genion.Genion.launch>` method."""
     return Genion(input_tpr_path=input_tpr_path, output_gro_path=output_gro_path,
                   input_top_zip_path=input_top_zip_path, output_top_zip_path=output_top_zip_path,
-                  properties=properties, **kwargs).launch()
+                  input_ndx_path=input_ndx_path, properties=properties, **kwargs).launch()
 
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Wrapper for the GROMACS genion module.",
                                      formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('-c', '--config', required=False, help="This file can be a YAML file, JSON file or JSON string")
 
     # Specific args of each building block
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_tpr_path', required=True)
     required_args.add_argument('--output_gro_path', required=True)
     required_args.add_argument('--input_top_zip_path', required=True)
     required_args.add_argument('--output_top_zip_path', required=True)
+    parser.add_argument('--input_ndx_path', required=False)
 
     args = parser.parse_args()
     config = args.config if args.config else None
     properties = settings.ConfReader(config=config).get_prop_dic()
 
     # Specific call of each building block
     genion(input_tpr_path=args.input_tpr_path, output_gro_path=args.output_gro_path,
            input_top_zip_path=args.input_top_zip_path, output_top_zip_path=args.output_top_zip_path,
-           properties=properties)
+           input_ndx_path=args.input_ndx_path, properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/genrestr.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/genrestr.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """Module containing the Genrestr class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_gromacs.gromacs.common import get_gromacs_version
+from pathlib import Path
+from typing import Union, Optional, Dict
 
 
 class Genrestr(BiobbObject):
     """
     | biobb_gromacs Genrestr
     | Wrapper of the `GROMACS genrestr <http://manual.gromacs.org/current/onlinehelp/gmx-genrestr.html>`_ module.
     | The GROMACS genrestr module, produces an #include file for a topology containing a list of atom numbers and three force constants for the x-, y-, and z-direction based on the contents of the -f file. A single isotropic force constant may be given on the command line instead of three components.
@@ -49,16 +51,16 @@
             * version: >5.1
             * license: LGPL 2.1
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_structure_path: str, output_itp_path: str, input_ndx_path: str = None,
-                 properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_structure_path: Union[str, Path], output_itp_path: Union[str, Path],
+                 input_ndx_path: Optional[Union[str, Path]] = None, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -73,19 +75,19 @@
 
         # Properties common in all GROMACS BB
         self.gmx_lib = properties.get('gmx_lib', None)
         self.binary_path = properties.get('binary_path', 'gmx')
         self.gmx_nobackup = properties.get('gmx_nobackup', True)
         self.gmx_nocopyright = properties.get('gmx_nocopyright', True)
         if self.gmx_nobackup:
-            self.binary_path += ' -nobackup'
+            self.binary_path = f"{self.binary_path}  -nobackup"
         if self.gmx_nocopyright:
-            self.binary_path += ' -nocopyright'
+            self.binary_path = f"{self.binary_path} -nocopyright"
         if not self.container_path:
-            self.gmx_version = get_gromacs_version(self.binary_path)
+            self.gmx_version = get_gromacs_version(str(self.binary_path))
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self) -> int:
@@ -94,15 +96,15 @@
         # Setup Biobb
         if self.check_restart():
             return 0
 
         self.io_dict['in']['stdin_file_path'] = fu.create_stdin_file(f'{self.restrained_group}')
         self.stage_files()
 
-        self.cmd = [self.binary_path, "genrestr",
+        self.cmd = [str(self.binary_path), "genrestr",
                     "-f", self.stage_io_dict["in"]["input_structure_path"],
                     "-o", self.stage_io_dict["out"]["output_itp_path"]]
 
         if not isinstance(self.force_constants, str):
             self.force_constants = " ".join(map(str, self.force_constants))
 
         self.cmd.append("-fc")
@@ -122,23 +124,23 @@
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # Remove temporal files
-        self.tmp_files.extend([self.stage_io_dict.get("unique_dir"), self.io_dict['in'].get("stdin_file_path")])
+        self.tmp_files.extend([str(self.stage_io_dict.get("unique_dir")), str(self.io_dict['in'].get("stdin_file_path"))])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
         return self.return_code
 
 
-def genrestr(input_structure_path: str, output_itp_path: str,
-             input_ndx_path: str = None, properties: dict = None, **kwargs) -> int:
+def genrestr(input_structure_path: Union[str, Path], output_itp_path: Union[str, Path],
+             input_ndx_path: Optional[Union[str, Path]] = None, properties: Optional[Dict] = None, **kwargs) -> int:
     """Create :class:`Genrestr <gromacs.genrestr.Genrestr>` class and
     execute the :meth:`launch() <gromacs.genrestr.Genrestr.launch>` method."""
 
     return Genrestr(input_structure_path=input_structure_path, output_itp_path=output_itp_path,
                     input_ndx_path=input_ndx_path, properties=properties, **kwargs).launch()
```

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/gmxselect.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/gmxselect.py`

 * *Files identical despite different names*

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/grompp.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/grompp.py`

 * *Files identical despite different names*

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/grompp_mdrun.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/grompp_mdrun.py`

 * *Files identical despite different names*

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/make_ndx.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/make_ndx.py`

 * *Files identical despite different names*

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/mdrun.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/mdrun.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,16 +88,14 @@
             "in": {"input_tpr_path": input_tpr_path, "input_cpt_path": input_cpt_path},
             "out": {"output_trr_path": output_trr_path, "output_gro_path": output_gro_path,
                     "output_edr_path": output_edr_path, "output_log_path": output_log_path,
                     "output_xtc_path": output_xtc_path, "output_cpt_path": output_cpt_path,
                     "output_dhdl_path": output_dhdl_path}
         }
 
-        #
-
         # Properties specific for BB
         # general mpi properties
         self.mpi_bin = properties.get('mpi_bin')
         self.mpi_np = properties.get('mpi_np')
         self.mpi_flags = properties.get('mpi_flags')
         # gromacs cpu mpi/openmp properties
         self.num_threads = str(properties.get('num_threads', ''))
@@ -109,15 +107,15 @@
         self.gpu_id = str(properties.get('gpu_id', ''))
         self.gpu_tasks = str(properties.get('gpu_tasks', ''))
         # gromacs
         self.checkpoint_time = properties.get('checkpoint_time')
 
         # Properties common in all GROMACS BB
         self.gmx_lib = properties.get('gmx_lib', None)
-        self.binary_path = properties.get('binary_path', 'gmx')
+        self.binary_path: str = properties.get('binary_path', 'gmx')
         self.gmx_nobackup = properties.get('gmx_nobackup', True)
         self.gmx_nocopyright = properties.get('gmx_nocopyright', True)
         if self.gmx_nobackup:
             self.binary_path += ' -nobackup'
         if self.gmx_nocopyright:
             self.binary_path += ' -nocopyright'
         if (not self.mpi_bin) and (not self.container_path):
```

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/pdb2gmx.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/pdb2gmx.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 from biobb_gromacs.gromacs.common import get_gromacs_version
+from typing import Optional, Dict
 
 
 class Pdb2gmx(BiobbObject):
     """
     | biobb_gromacs Pdb2gmx
     | Wrapper class for the `GROMACS pdb2gmx <http://manual.gromacs.org/current/onlinehelp/gmx-pdb2gmx.html>`_ module.
     | The GROMACS pdb2gmx module, reads a .pdb (or .gro) file, reads some database files, adds hydrogens to the molecules and generates coordinates in GROMACS (GROMOS), or optionally .pdb, format and a topology in GROMACS format. These files can subsequently be processed to generate a run input file.
@@ -53,15 +54,15 @@
             * version: >5.1
             * license: LGPL 2.1
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
-    def __init__(self, input_pdb_path: str, output_gro_path: str, output_top_zip_path: str, properties: dict = None,
+    def __init__(self, input_pdb_path: str, output_gro_path: str, output_top_zip_path: str, properties: Optional[Dict] = None,
                  **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
@@ -78,15 +79,15 @@
         self.force_field = properties.get('force_field', 'amber99sb-ildn')
         self.ignh = properties.get('ignh', False)
         self.his = properties.get('his', None)
         self.merge = properties.get('merge', False)
 
         # Properties common in all GROMACS BB
         self.gmx_lib = properties.get('gmx_lib', None)
-        self.binary_path = properties.get('binary_path', 'gmx')
+        self.binary_path: str = properties.get('binary_path', 'gmx')
         self.gmx_nobackup = properties.get('gmx_nobackup', True)
         self.gmx_nocopyright = properties.get('gmx_nocopyright', True)
         if self.gmx_nobackup:
             self.binary_path += ' -nobackup'
         if self.gmx_nocopyright:
             self.binary_path += ' -nocopyright'
         if not self.container_path:
```

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/solvate.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/solvate.py`

 * *Files identical despite different names*

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs/trjcat.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs/trjcat.py`

 * *Files identical despite different names*

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs_extra/append_ligand.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs_extra/append_ligand.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 """Module containing the AppendLigand class and the command line interface."""
 import re
 import argparse
 import shutil
 from pathlib import Path
+from typing import Optional, Dict
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools import file_utils as fu
 from biobb_common.tools.file_utils import launchlogger
 
 
 class AppendLigand(BiobbObject):
@@ -43,15 +44,15 @@
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
     """
 
     def __init__(self, input_top_zip_path: str, input_itp_path: str, output_top_zip_path: str,
-                 input_posres_itp_path: str = None, properties: dict = None, **kwargs) -> None:
+                 input_posres_itp_path: Optional[str] = None, properties: Optional[Dict] = None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
@@ -72,17 +73,17 @@
     def launch(self) -> int:
         """Execute the :class:`AppendLigand <gromacs_extra.append_ligand.AppendLigand>` object."""
         # Setup Biobb
         if self.check_restart():
             return 0
 
         # Unzip topology
-        top_file = fu.unzip_top(zip_file=self.io_dict['in'].get("input_top_zip_path"), out_log=self.out_log)
+        top_file = fu.unzip_top(zip_file=str(self.io_dict['in'].get("input_top_zip_path")), out_log=self.out_log)
         top_dir = str(Path(top_file).parent)
-        itp_name = str(Path(self.io_dict['in'].get("input_itp_path")).name)
+        itp_name = str(Path(str(self.io_dict['in'].get("input_itp_path"))).name)
 
         with open(top_file) as top_f:
             top_lines = top_f.readlines()
             top_f.close()
         fu.rm(top_file)
 
         forcefield_pattern = r'#include.*forcefield.itp\"'
```

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs/gromacs_extra/ndx2resttop.py` & `biobb_gromacs-4.2.0/biobb_gromacs/gromacs_extra/ndx2resttop.py`

 * *Files identical despite different names*

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs.egg-info/PKG-INFO` & `biobb_gromacs-4.2.0/biobb_gromacs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: biobb-gromacs
-Version: 4.1.1
+Version: 4.2.0
 Summary: biobb_gromacs is the Biobb module collection to perform molecular dynamics simulations.
 Home-page: https://github.com/bioexcel/biobb_gromacs
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
-Project-URL: Documentation, http://biobb_gromacs.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-gromacs.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_gromacs?label=Version)](https://GitHub.com/bioexcel/biobb_gromacs/tags/)
 [![](https://img.shields.io/pypi/v/biobb-gromacs.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-gromacs/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_gromacs?label=Conda)](https://anaconda.org/bioconda/biobb_gromacs)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_gromacs?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_gromacs)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_gromacs?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_gromacs:4.1.1--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_gromacs:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_gromacs)
 [![](https://img.shields.io/pypi/pyversions/biobb-gromacs.svg?label=Python%20Versions)](https://pypi.org/project/biobb-gromacs/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_gromacs)
 
 [![](https://readthedocs.org/projects/biobb-gromacs/badge/?version=latest&label=Docs)](https://biobb-gromacs.readthedocs.io/en/latest/?badge=latest)
@@ -40,87 +40,95 @@
 
 [![](https://docs.bioexcel.eu/biobb_gromacs/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_gromacs/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_gromacs/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_gromacs/coverage/)
 [![](https://docs.bioexcel.eu/biobb_gromacs/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_gromacs/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_gromacs?label=Last%20Commit)](https://github.com/bioexcel/biobb_gromacs/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_gromacs.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_gromacs/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
+
 
 # biobb_gromacs
 
 ### Introduction
 biobb_gromacs is the Biobb module collection to perform molecular dynamics simulations using the GROMACS MD suite.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-gromacs.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2023.3
+v4.2.0 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_gromacs>=4.1.1"
+        pip install "biobb_gromacs>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-gromacs.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_gromacs>=4.1.1"
+        conda install -c bioconda "biobb_gromacs>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-gromacs.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-gromacs.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_gromacs:4.1.1--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_gromacs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_gromacs:4.1.1--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_gromacs:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_gromacs.sif https://depot.galaxyproject.org/singularity/biobb_gromacs:4.1.1--pyhdfd78af_1
+        singularity pull --name biobb_gromacs.sif https://depot.galaxyproject.org/singularity/biobb_gromacs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_gromacs.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-gromacs.readthedocs.io/en/latest/command_line.html).
 
 
 ### Copyright & Licensing
 This software has been developed in the [MMB group](http://mmb.irbbarcelona.org) at the [BSC](http://www.bsc.es/) & [IRB](https://www.irbbarcelona.org/) for the [European BioExcel](http://bioexcel.eu/), funded by the European Commission (EU H2020 [823830](http://cordis.europa.eu/projects/823830), EU H2020 [675728](http://cordis.europa.eu/projects/675728)).
 
-* (c) 2015-2023 [Barcelona Supercomputing Center](https://www.bsc.es/)
-* (c) 2015-2023 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
+* (c) 2015-2024 [Barcelona Supercomputing Center](https://www.bsc.es/)
+* (c) 2015-2024 [Institute for Research in Biomedicine](https://www.irbbarcelona.org/)
 
 Licensed under the
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file LICENSE for details.
 
 ![](https://bioexcel.eu/wp-content/uploads/2019/04/Bioexcell_logo_1080px_transp.png "Bioexcel")
```

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs.egg-info/SOURCES.txt` & `biobb_gromacs-4.2.0/biobb_gromacs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_gromacs-4.1.1/biobb_gromacs.egg-info/entry_points.txt` & `biobb_gromacs-4.2.0/biobb_gromacs.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_gromacs-4.1.1/setup.py` & `biobb_gromacs-4.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_gromacs",
-    version="4.1.1",
+    version="4.2.0",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="biobb_gromacs is the Biobb module collection to perform molecular dynamics simulations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_gromacs",
     project_urls={
-        "Documentation": "http://biobb_gromacs.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-gromacs.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==4.1.0'],
+    install_requires=['biobb_common==4.2.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "editconf = biobb_gromacs.gromacs.editconf:main",
             "genion = biobb_gromacs.gromacs.genion:main",
             "genrestr = biobb_gromacs.gromacs.genrestr:main",
             "grompp = biobb_gromacs.gromacs.grompp:main",
```

