# Comparing `tmp/biobb_chemistry-4.1.0.tar.gz` & `tmp/biobb_chemistry-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_chemistry-4.1.0.tar", last modified: Wed Sep  6 13:46:38 2023, max compression
+gzip compressed data, was "biobb_chemistry-4.2.0.tar", last modified: Fri May 24 08:01:29 2024, max compression
```

## Comparing `biobb_chemistry-4.1.0.tar` & `biobb_chemistry-4.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 13:46:38.399393 biobb_chemistry-4.1.0/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:32:59.000000 biobb_chemistry-4.1.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     6331 2023-09-06 13:46:38.399213 biobb_chemistry-4.1.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5422 2023-09-06 13:43:47.000000 biobb_chemistry-4.1.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 13:46:38.395693 biobb_chemistry-4.1.0/biobb_chemistry/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       92 2023-09-06 13:42:52.000000 biobb_chemistry-4.1.0/biobb_chemistry/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 13:46:38.397461 biobb_chemistry-4.1.0/biobb_chemistry/acpype/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      115 2023-04-12 10:12:09.000000 biobb_chemistry-4.1.0/biobb_chemistry/acpype/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11692 2023-04-12 09:11:11.000000 biobb_chemistry-4.1.0/biobb_chemistry/acpype/acpype_params_ac.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10624 2023-04-12 09:17:02.000000 biobb_chemistry-4.1.0/biobb_chemistry/acpype/acpype_params_cns.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10652 2023-04-12 09:21:55.000000 biobb_chemistry-4.1.0/biobb_chemistry/acpype/acpype_params_gmx.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9951 2023-04-12 09:19:47.000000 biobb_chemistry-4.1.0/biobb_chemistry/acpype/acpype_params_gmx_opls.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5952 2023-04-12 09:24:34.000000 biobb_chemistry-4.1.0/biobb_chemistry/acpype/common.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 13:46:38.398069 biobb_chemistry-4.1.0/biobb_chemistry/ambertools/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       82 2023-04-12 10:12:03.000000 biobb_chemistry-4.1.0/biobb_chemistry/ambertools/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     1940 2023-04-12 09:27:12.000000 biobb_chemistry-4.1.0/biobb_chemistry/ambertools/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11314 2023-04-12 09:30:04.000000 biobb_chemistry-4.1.0/biobb_chemistry/ambertools/reduce_add_hydrogens.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7059 2023-04-12 09:32:00.000000 biobb_chemistry-4.1.0/biobb_chemistry/ambertools/reduce_remove_hydrogens.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 13:46:38.398932 biobb_chemistry-4.1.0/biobb_chemistry/babelm/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      111 2023-04-12 10:12:14.000000 biobb_chemistry-4.1.0/biobb_chemistry/babelm/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12095 2023-04-12 09:34:28.000000 biobb_chemistry-4.1.0/biobb_chemistry/babelm/babel_add_hydrogens.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12124 2023-04-12 09:36:18.000000 biobb_chemistry-4.1.0/biobb_chemistry/babelm/babel_convert.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9947 2023-04-12 09:39:23.000000 biobb_chemistry-4.1.0/biobb_chemistry/babelm/babel_minimize.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12135 2023-04-12 09:41:05.000000 biobb_chemistry-4.1.0/biobb_chemistry/babelm/babel_remove_hydrogens.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8059 2023-04-12 09:42:23.000000 biobb_chemistry-4.1.0/biobb_chemistry/babelm/common.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 13:46:38.399061 biobb_chemistry-4.1.0/biobb_chemistry/test/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:32:59.000000 biobb_chemistry-4.1.0/biobb_chemistry/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-06 13:46:38.396540 biobb_chemistry-4.1.0/biobb_chemistry.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     6331 2023-09-06 13:46:38.000000 biobb_chemistry-4.1.0/biobb_chemistry.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573      996 2023-09-06 13:46:38.000000 biobb_chemistry-4.1.0/biobb_chemistry.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-09-06 13:46:38.000000 biobb_chemistry-4.1.0/biobb_chemistry.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      712 2023-09-06 13:46:38.000000 biobb_chemistry-4.1.0/biobb_chemistry.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2023-09-06 13:46:38.000000 biobb_chemistry-4.1.0/biobb_chemistry.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       16 2023-09-06 13:46:38.000000 biobb_chemistry-4.1.0/biobb_chemistry.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-09-06 13:46:38.399438 biobb_chemistry-4.1.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2130 2023-09-06 13:42:29.000000 biobb_chemistry-4.1.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:01:29.623134 biobb_chemistry-4.2.0/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:32:59.000000 biobb_chemistry-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6905 2024-05-24 08:01:29.622912 biobb_chemistry-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5961 2024-05-24 07:59:15.000000 biobb_chemistry-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:01:29.619748 biobb_chemistry-4.2.0/biobb_chemistry/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       92 2024-05-24 07:59:03.000000 biobb_chemistry-4.2.0/biobb_chemistry/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:01:29.621305 biobb_chemistry-4.2.0/biobb_chemistry/acpype/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      115 2023-04-12 10:12:09.000000 biobb_chemistry-4.2.0/biobb_chemistry/acpype/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11692 2023-04-12 09:11:11.000000 biobb_chemistry-4.2.0/biobb_chemistry/acpype/acpype_params_ac.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11407 2024-03-12 09:16:51.000000 biobb_chemistry-4.2.0/biobb_chemistry/acpype/acpype_params_cns.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10652 2023-04-12 09:21:55.000000 biobb_chemistry-4.2.0/biobb_chemistry/acpype/acpype_params_gmx.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9951 2023-04-12 09:19:47.000000 biobb_chemistry-4.2.0/biobb_chemistry/acpype/acpype_params_gmx_opls.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7366 2024-03-12 09:16:51.000000 biobb_chemistry-4.2.0/biobb_chemistry/acpype/common.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:01:29.621849 biobb_chemistry-4.2.0/biobb_chemistry/ambertools/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       82 2023-04-12 10:12:03.000000 biobb_chemistry-4.2.0/biobb_chemistry/ambertools/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     1940 2023-04-12 09:27:12.000000 biobb_chemistry-4.2.0/biobb_chemistry/ambertools/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11314 2023-04-12 09:30:04.000000 biobb_chemistry-4.2.0/biobb_chemistry/ambertools/reduce_add_hydrogens.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7059 2023-04-12 09:32:00.000000 biobb_chemistry-4.2.0/biobb_chemistry/ambertools/reduce_remove_hydrogens.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:01:29.622578 biobb_chemistry-4.2.0/biobb_chemistry/babelm/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      111 2023-04-12 10:12:14.000000 biobb_chemistry-4.2.0/biobb_chemistry/babelm/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12115 2024-03-12 09:16:51.000000 biobb_chemistry-4.2.0/biobb_chemistry/babelm/babel_add_hydrogens.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12124 2023-04-12 09:36:18.000000 biobb_chemistry-4.2.0/biobb_chemistry/babelm/babel_convert.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9947 2023-04-12 09:39:23.000000 biobb_chemistry-4.2.0/biobb_chemistry/babelm/babel_minimize.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12135 2023-04-12 09:41:05.000000 biobb_chemistry-4.2.0/biobb_chemistry/babelm/babel_remove_hydrogens.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8059 2023-04-12 09:42:23.000000 biobb_chemistry-4.2.0/biobb_chemistry/babelm/common.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:01:29.622693 biobb_chemistry-4.2.0/biobb_chemistry/test/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:32:59.000000 biobb_chemistry-4.2.0/biobb_chemistry/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:01:29.620556 biobb_chemistry-4.2.0/biobb_chemistry.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6905 2024-05-24 08:01:29.000000 biobb_chemistry-4.2.0/biobb_chemistry.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      996 2024-05-24 08:01:29.000000 biobb_chemistry-4.2.0/biobb_chemistry.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2024-05-24 08:01:29.000000 biobb_chemistry-4.2.0/biobb_chemistry.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      712 2024-05-24 08:01:29.000000 biobb_chemistry-4.2.0/biobb_chemistry.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2024-05-24 08:01:29.000000 biobb_chemistry-4.2.0/biobb_chemistry.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       16 2024-05-24 08:01:29.000000 biobb_chemistry-4.2.0/biobb_chemistry.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2024-05-24 08:01:29.623177 biobb_chemistry-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2130 2024-05-24 07:58:52.000000 biobb_chemistry-4.2.0/setup.py
```

### Comparing `biobb_chemistry-4.1.0/LICENSE` & `biobb_chemistry-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/PKG-INFO` & `biobb_chemistry-4.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,13 @@
-Metadata-Version: 2.1
-Name: biobb_chemistry
-Version: 4.1.0
-Summary: Biobb_chemistry is the Biobb module collection to perform chemistry over molecular dynamics simulations.
-Home-page: https://github.com/bioexcel/biobb_chemistry
-Author: Biobb developers
-Author-email: genis.bayarri@irbbarcelona.org
-Project-URL: Documentation, https://biobb-chemistry.readthedocs.io/en/latest/
-Project-URL: Bioexcel, https://bioexcel.eu/
-Keywords: Bioinformatics Workflows BioExcel Compatibility
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_chemistry?label=Version)](https://GitHub.com/bioexcel/biobb_chemistry/tags/)
 [![](https://img.shields.io/pypi/v/biobb-chemistry.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-chemistry/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_chemistry?label=Conda)](https://anaconda.org/bioconda/biobb_chemistry)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_chemistry?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_chemistry)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_chemistry?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_chemistry:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_chemistry:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_chemistry)
 [![](https://img.shields.io/pypi/pyversions/biobb-chemistry.svg?label=Python%20Versions)](https://pypi.org/project/biobb-chemistry/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_chemistry)
 
 [![](https://readthedocs.org/projects/biobb-chemistry/badge/?version=latest&label=Docs)](https://biobb-chemistry.readthedocs.io/en/latest/?badge=latest)
@@ -39,85 +18,92 @@
 
 [![](https://docs.bioexcel.eu/biobb_chemistry/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_chemistry/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_chemistry/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_chemistry/coverage/)
 [![](https://docs.bioexcel.eu/biobb_chemistry/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_chemistry/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_chemistry?label=Last%20Commit)](https://github.com/bioexcel/biobb_chemistry/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_chemistry.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_chemistry/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_chemistry
 
 ### Introduction
 Biobb_chemistry is the Biobb module collection to perform chemistry over molecular dynamics simulations.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_chemistry.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-chemistry.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_chemistry>=4.1.0"
+        pip install "biobb_chemistry>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-chemistry.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_chemistry>=4.1.0"
+        conda install -c bioconda "biobb_chemistry>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-chemistry.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-chemistry.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_chemistry:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_chemistry:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_chemistry:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_chemistry:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_chemistry.sif https://depot.galaxyproject.org/singularity/biobb_chemistry:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_chemistry.sif https://depot.galaxyproject.org/singularity/biobb_chemistry:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_chemistry.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-chemistry.readthedocs.io/en/latest/command_line.html).
 
 
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

### Comparing `biobb_chemistry-4.1.0/README.md` & `biobb_chemistry-4.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,35 @@
+Metadata-Version: 2.1
+Name: biobb_chemistry
+Version: 4.2.0
+Summary: Biobb_chemistry is the Biobb module collection to perform chemistry over molecular dynamics simulations.
+Home-page: https://github.com/bioexcel/biobb_chemistry
+Author: Biobb developers
+Author-email: genis.bayarri@irbbarcelona.org
+Project-URL: Documentation, https://biobb-chemistry.readthedocs.io/en/latest/
+Project-URL: Bioexcel, https://bioexcel.eu/
+Keywords: Bioinformatics Workflows BioExcel Compatibility
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: biobb_common==4.2.0
+
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_chemistry?label=Version)](https://GitHub.com/bioexcel/biobb_chemistry/tags/)
 [![](https://img.shields.io/pypi/v/biobb-chemistry.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-chemistry/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_chemistry?label=Conda)](https://anaconda.org/bioconda/biobb_chemistry)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_chemistry?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_chemistry)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_chemistry?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_chemistry:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_chemistry:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_chemistry)
 [![](https://img.shields.io/pypi/pyversions/biobb-chemistry.svg?label=Python%20Versions)](https://pypi.org/project/biobb-chemistry/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_chemistry)
 
 [![](https://readthedocs.org/projects/biobb-chemistry/badge/?version=latest&label=Docs)](https://biobb-chemistry.readthedocs.io/en/latest/?badge=latest)
@@ -18,85 +40,92 @@
 
 [![](https://docs.bioexcel.eu/biobb_chemistry/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_chemistry/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_chemistry/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_chemistry/coverage/)
 [![](https://docs.bioexcel.eu/biobb_chemistry/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_chemistry/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_chemistry?label=Last%20Commit)](https://github.com/bioexcel/biobb_chemistry/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_chemistry.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_chemistry/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_chemistry
 
 ### Introduction
 Biobb_chemistry is the Biobb module collection to perform chemistry over molecular dynamics simulations.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_chemistry.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-chemistry.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_chemistry>=4.1.0"
+        pip install "biobb_chemistry>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-chemistry.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_chemistry>=4.1.0"
+        conda install -c bioconda "biobb_chemistry>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-chemistry.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-chemistry.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_chemistry:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_chemistry:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_chemistry:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_chemistry:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_chemistry.sif https://depot.galaxyproject.org/singularity/biobb_chemistry:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_chemistry.sif https://depot.galaxyproject.org/singularity/biobb_chemistry:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_chemistry.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-chemistry.readthedocs.io/en/latest/command_line.html).
 
 
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

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/acpype/acpype_params_ac.py` & `biobb_chemistry-4.2.0/biobb_chemistry/acpype/acpype_params_ac.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/acpype/acpype_params_cns.py` & `biobb_chemistry-4.2.0/biobb_chemistry/acpype/acpype_params_cns.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python3
 
 """Module containing the AcpypeParamsCNS class and the command line interface."""
 import argparse
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
-from biobb_chemistry.acpype.common import get_binary_path, check_input_path, check_output_path, get_basename, get_charge, create_unique_name, get_default_value, process_output
+from biobb_chemistry.acpype.common import get_binary_path, check_input_path, check_output_path, get_basename, get_charge, create_unique_name, get_default_value, process_output_cns
 
 
 class AcpypeParamsCNS(BiobbObject):
     """
     | biobb_chemistry AcpypeParamsCNS
     | This class is a wrapper of `Acpype <https://github.com/alanwilter/acpype>`_ tool for small molecule parameterization for CNS/XPLOR MD package.
     | Generation of topologies for CNS/XPLOR. Acpype is a tool based in Python to use Antechamber to generate topologies for chemical compounds and to interface with others python applications like CCPN or ARIA. `Visit the official page <https://github.com/alanwilter/acpype>`_.
 
     Args:
         input_path (str): Path to the input file. File type: input. `Sample file <https://github.com/bioexcel/biobb_chemistry/raw/master/biobb_chemistry/test/data/acpype/acpype.params.mol2>`_. Accepted formats: pdb (edam:format_1476), mdl (edam:format_3815), mol2 (edam:format_3816).
         output_path_par (str): Path to the PAR output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_chemistry/raw/master/biobb_chemistry/test/reference/acpype/ref_acpype.cns.par>`_. Accepted formats: par (edam:format_3881).
         output_path_inp (str): Path to the INP output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_chemistry/raw/master/biobb_chemistry/test/reference/acpype/ref_acpype.cns.inp>`_. Accepted formats: inp (edam:format_3878).
         output_path_top (str): Path to the TOP output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_chemistry/raw/master/biobb_chemistry/test/reference/acpype/ref_acpype.cns.top>`_. Accepted formats: top (edam:format_3881).
+        output_path_pdb (str): Path to the PDB output file. File type: output. `Sample file <https://github.com/bioexcel/biobb_chemistry/raw/master/biobb_chemistry/test/reference/acpype/ref_acpype.cns.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **basename** (*str*) - ("BBB") A basename for the project (folder and output files).
             * **charge** (*int*) - (0) [-20~20|1] Net molecular charge, for gas default is 0. If None the charge is guessed by acpype.
             * **binary_path** (*str*) - ("acpype") Path to the acpype executable binary.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
             * **container_path** (*str*) - (None) Container path definition.
@@ -40,39 +41,40 @@
                 'basename': 'BBB',
                 'charge': 0
             }
             acpype_params_cns(input_path='/path/to/myStructure.mol2',
                             output_path_par='/path/to/newPAR.par',
                             output_path_inp='/path/to/newINP.inp',
                             output_path_top='/path/to/newTOP.top',
+                            output_path_top='/path/to/newPDB.pdb',
                             properties=prop)
 
     Info:
         * wrapped_software:
             * name: Acpype
             * version: 2019.10.05.12.26
             * license: GNU
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
 
-    def __init__(self, input_path, output_path_par, output_path_inp, output_path_top,
+    def __init__(self, input_path, output_path_par, output_path_inp, output_path_top, output_path_pdb,
                  properties=None, **kwargs) -> None:
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
             "in": {"input_path": input_path},
-            "out": {"output_path_par": output_path_par, "output_path_inp": output_path_inp, "output_path_top": output_path_top}
+            "out": {"output_path_par": output_path_par, "output_path_inp": output_path_inp, "output_path_top": output_path_top, "output_path_pdb": output_path_pdb}
         }
 
         # Properties specific for BB
         self.basename = properties.get('basename', 'BBB')
         self.charge = properties.get('charge', '')
         self.binary_path = get_binary_path(properties, 'binary_path')
         self.properties = properties
@@ -83,18 +85,20 @@
 
     def check_data_params(self, out_log, err_log):
         """ Checks all the input/output paths and parameters """
         self.io_dict["in"]["input_path"] = check_input_path(self.io_dict["in"]["input_path"], out_log, self.__class__.__name__)
         self.io_dict["out"]["output_path_par"] = check_output_path(self.io_dict["out"]["output_path_par"], 'par', out_log, self.__class__.__name__)
         self.io_dict["out"]["output_path_inp"] = check_output_path(self.io_dict["out"]["output_path_inp"], 'inp', out_log, self.__class__.__name__)
         self.io_dict["out"]["output_path_top"] = check_output_path(self.io_dict["out"]["output_path_top"], 'top', out_log, self.__class__.__name__)
+        self.io_dict["out"]["output_path_pdb"] = check_output_path(self.io_dict["out"]["output_path_pdb"], 'pdb', out_log, self.__class__.__name__)
         self.output_files = {
             'par': self.io_dict["out"]["output_path_par"],
             'inp': self.io_dict["out"]["output_path_inp"],
             'top': self.io_dict["out"]["output_path_top"],
+            'pdb': self.io_dict["out"]["output_path_pdb"],
         }
 
     def create_cmd(self, container_io_dict, out_log, err_log):
         """Creates the command line instruction using the properties file settings"""
         instructions_list = []
 
         # generating output path
@@ -144,63 +148,68 @@
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
         # move files to output_path and removes temporary folder
         if self.container_path:
-            process_output(self.unique_name,
-                           self.stage_io_dict['unique_dir'],
-                           self.remove_tmp,
-                           self.basename,
-                           get_default_value(self.__class__.__name__),
-                           self.output_files, self.out_log)
+            process_output_cns(
+                self.unique_name,
+                self.stage_io_dict['unique_dir'],
+                self.remove_tmp,
+                self.basename,
+                get_default_value(self.__class__.__name__),
+                self.output_files, self.out_log)
         else:
-            process_output(self.unique_name,
-                           self.basename + "." + self.unique_name + ".acpype",
-                           self.remove_tmp,
-                           self.basename,
-                           get_default_value(self.__class__.__name__),
-                           self.output_files, self.out_log)
+            process_output_cns(
+                self.unique_name,
+                self.basename + "." + self.unique_name + ".acpype",
+                self.remove_tmp,
+                self.basename,
+                get_default_value(self.__class__.__name__),
+                self.output_files, self.out_log)
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
 
-def acpype_params_cns(input_path: str, output_path_par: str, output_path_inp: str, output_path_top: str, properties: dict = None, **kwargs) -> int:
+def acpype_params_cns(input_path: str, output_path_par: str, output_path_inp: str, output_path_top: str, output_path_pdb: str, properties: dict = None, **kwargs) -> int:
     """Execute the :class:`AcpypeParamsCNS <acpype.acpype_params_cns.AcpypeParamsCNS>` class and
     execute the :meth:`launch() <acpype.acpype_params_cns.AcpypeParamsCNS.launch>` method."""
 
     return AcpypeParamsCNS(input_path=input_path,
                            output_path_par=output_path_par,
                            output_path_inp=output_path_inp,
                            output_path_top=output_path_top,
+                           output_path_pdb=output_path_pdb,
                            properties=properties, **kwargs).launch()
 
 
 def main():
     """Command line execution of this building block. Please check the command line documentation."""
     parser = argparse.ArgumentParser(description="Small molecule parameterization for CNS/XPLOR MD package.", formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args of each building block
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_path', required=True, help='Path to the input file. Accepted formats: pdb, mdl, mol2.')
     required_args.add_argument('--output_path_par', required=True, help='Path to the PAR output file. Accepted formats: par.')
     required_args.add_argument('--output_path_inp', required=True, help='Path to the INP output file. Accepted formats: inp.')
     required_args.add_argument('--output_path_top', required=True, help='Path to the TOP output file. Accepted formats: top.')
+    required_args.add_argument('--output_path_pdb', required=True, help='Path to the PDB output file. Accepted formats: pdb.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call of each building block
     acpype_params_cns(input_path=args.input_path,
                       output_path_par=args.output_path_par,
                       output_path_inp=args.output_path_inp,
                       output_path_top=args.output_path_top,
+                      output_path_pdb=args.output_path_pdb,
                       properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/acpype/acpype_params_gmx.py` & `biobb_chemistry-4.2.0/biobb_chemistry/acpype/acpype_params_gmx.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/acpype/acpype_params_gmx_opls.py` & `biobb_chemistry-4.2.0/biobb_chemistry/acpype/acpype_params_gmx_opls.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/acpype/common.py` & `biobb_chemistry-4.2.0/biobb_chemistry/acpype/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -147,11 +147,40 @@
                 with open(file_name) as f:
                     newText = f.read().replace(basename + '_GMX.itp', PurePath(output_files['itp']).name)
                 with open(file_name, "w") as f:
                     f.write(newText)
             shutil.copy(file_name, output_files[file_extension[1:]])
             fu.log('File %s succesfully created' % output_files[file_extension[1:]], out_log)
 
+
+def process_output_cns(unique_name, files_folder, remove_tmp, basename, class_params, output_files, out_log):
+    """ Moves and removes temporal files generated by the wrapper """
+    path = files_folder
+    suffix = class_params['suffix']
+    src_files = glob.glob(path + '/' + basename + '.' + unique_name + suffix + '*')
+
+    # copy files for the requested topology to the output_path
+    for file_name in src_files:
+        # replace random name by original name in all files
+        with fileinput.FileInput(file_name, inplace=True) as file:
+            for line in file:
+                print(line.replace(basename + '.' + unique_name, basename), end='')
+
+        if (Path(file_name).is_file()):
+            file_extension = PurePath(file_name).suffix
+            fu.log('Files: %s' % str(file_name), out_log)
+            shutil.copy(file_name, output_files[file_extension[1:]])
+            fu.log('File %s succesfully created' % output_files[file_extension[1:]], out_log)
+
+    file_extension = ".pdb"
+    file_name = path + '/' + basename + '.' + unique_name + "_NEW.pdb"
+    with open(file_name) as f:
+        newText = f.read().replace(basename + '_NEW.pdb', PurePath(output_files['pdb']).name)
+    with open(file_name, "w") as f:
+        f.write(newText)
+    shutil.copy(file_name, output_files[file_extension[1:]])
+    fu.log('File %s succesfully created' % output_files[file_extension[1:]], out_log)
+
     if remove_tmp:
         # remove temporary folder
         fu.rm(files_folder)
         fu.log('Removed temporary folder: %s' % files_folder, out_log)
```

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/ambertools/common.py` & `biobb_chemistry-4.2.0/biobb_chemistry/ambertools/common.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/ambertools/reduce_add_hydrogens.py` & `biobb_chemistry-4.2.0/biobb_chemistry/ambertools/reduce_add_hydrogens.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/ambertools/reduce_remove_hydrogens.py` & `biobb_chemistry-4.2.0/biobb_chemistry/ambertools/reduce_remove_hydrogens.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/babelm/babel_add_hydrogens.py` & `biobb_chemistry-4.2.0/biobb_chemistry/babelm/babel_add_hydrogens.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,22 +119,21 @@
 
         # checking pH
         p = get_ph(self.ph, out_log)
 
         # adding H
         hydrogens = '-h'
 
-        instructions_list.append(hydrogens)
-
         # adding pH
         ph = ''
         if p:
             ph = '-p ' + p
-
-        instructions_list.append(ph)
+            instructions_list.append(ph)
+        else:
+            instructions_list.append(hydrogens)
 
         return instructions_list
 
     @launchlogger
     def launch(self) -> int:
         """Execute the :class:`BabelAddHydrogens <babelm.babel_add_hydrogens.BabelAddHydrogens>` babelm.babel_add_hydrogens.BabelAddHydrogens object."""
```

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/babelm/babel_convert.py` & `biobb_chemistry-4.2.0/biobb_chemistry/babelm/babel_convert.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/babelm/babel_minimize.py` & `biobb_chemistry-4.2.0/biobb_chemistry/babelm/babel_minimize.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/babelm/babel_remove_hydrogens.py` & `biobb_chemistry-4.2.0/biobb_chemistry/babelm/babel_remove_hydrogens.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry/babelm/common.py` & `biobb_chemistry-4.2.0/biobb_chemistry/babelm/common.py`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry.egg-info/PKG-INFO` & `biobb_chemistry-4.2.0/biobb_chemistry.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb-chemistry
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_chemistry is the Biobb module collection to perform chemistry over molecular dynamics simulations.
 Home-page: https://github.com/bioexcel/biobb_chemistry
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
 Project-URL: Documentation, https://biobb-chemistry.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -14,21 +14,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.2.0
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_chemistry?label=Version)](https://GitHub.com/bioexcel/biobb_chemistry/tags/)
 [![](https://img.shields.io/pypi/v/biobb-chemistry.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-chemistry/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_chemistry?label=Conda)](https://anaconda.org/bioconda/biobb_chemistry)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_chemistry?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_chemistry)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_chemistry?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_chemistry:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_chemistry:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_chemistry)
 [![](https://img.shields.io/pypi/pyversions/biobb-chemistry.svg?label=Python%20Versions)](https://pypi.org/project/biobb-chemistry/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_chemistry)
 
 [![](https://readthedocs.org/projects/biobb-chemistry/badge/?version=latest&label=Docs)](https://biobb-chemistry.readthedocs.io/en/latest/?badge=latest)
@@ -39,85 +40,92 @@
 
 [![](https://docs.bioexcel.eu/biobb_chemistry/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_chemistry/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_chemistry/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_chemistry/coverage/)
 [![](https://docs.bioexcel.eu/biobb_chemistry/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_chemistry/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_chemistry?label=Last%20Commit)](https://github.com/bioexcel/biobb_chemistry/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_chemistry.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_chemistry/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_chemistry
 
 ### Introduction
 Biobb_chemistry is the Biobb module collection to perform chemistry over molecular dynamics simulations.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_chemistry.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-chemistry.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_chemistry>=4.1.0"
+        pip install "biobb_chemistry>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-chemistry.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_chemistry>=4.1.0"
+        conda install -c bioconda "biobb_chemistry>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-chemistry.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-chemistry.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_chemistry:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_chemistry:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_chemistry:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_chemistry:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_chemistry.sif https://depot.galaxyproject.org/singularity/biobb_chemistry:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_chemistry.sif https://depot.galaxyproject.org/singularity/biobb_chemistry:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_chemistry.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-chemistry.readthedocs.io/en/latest/command_line.html).
 
 
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

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry.egg-info/SOURCES.txt` & `biobb_chemistry-4.2.0/biobb_chemistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/biobb_chemistry.egg-info/entry_points.txt` & `biobb_chemistry-4.2.0/biobb_chemistry.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_chemistry-4.1.0/setup.py` & `biobb_chemistry-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_chemistry",
-    version="4.1.0",
+    version="4.2.0",
     author="Biobb developers",
     author_email="genis.bayarri@irbbarcelona.org",
     description="Biobb_chemistry is the Biobb module collection to perform chemistry over molecular dynamics simulations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_chemistry",
     project_urls={
         "Documentation": "https://biobb-chemistry.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==4.1.0'],
+    install_requires=['biobb_common==4.2.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "acpype_params_ac = biobb_chemistry.acpype.acpype_params_ac:main",
             "acpype_params_cns = biobb_chemistry.acpype.acpype_params_cns:main",
             "acpype_params_gmx_opls = biobb_chemistry.acpype.acpype_params_gmx_opls:main",
             "acpype_params_gmx = biobb_chemistry.acpype.acpype_params_gmx:main",
```

