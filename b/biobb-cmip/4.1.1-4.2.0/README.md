# Comparing `tmp/biobb_cmip-4.1.1.tar.gz` & `tmp/biobb_cmip-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_cmip-4.1.1.tar", last modified: Thu Feb 29 14:09:16 2024, max compression
+gzip compressed data, was "biobb_cmip-4.2.0.tar", last modified: Fri May 24 08:15:02 2024, max compression
```

## Comparing `biobb_cmip-4.1.1.tar` & `biobb_cmip-4.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-02-29 14:09:16.271296 biobb_cmip-4.1.1/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:33:12.000000 biobb_cmip-4.1.1/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       79 2022-05-26 11:33:12.000000 biobb_cmip-4.1.1/MANIFEST.in
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6257 2024-02-29 14:09:16.271057 biobb_cmip-4.1.1/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5220 2024-02-29 14:07:34.000000 biobb_cmip-4.1.1/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-02-29 14:09:16.267854 biobb_cmip-4.1.1/biobb_cmip/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       61 2024-02-29 14:06:58.000000 biobb_cmip-4.1.1/biobb_cmip/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-02-29 14:09:16.269668 biobb_cmip-4.1.1/biobb_cmip/cmip/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      125 2023-09-15 13:20:41.000000 biobb_cmip-4.1.1/biobb_cmip/cmip/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6389 2023-09-15 13:15:32.000000 biobb_cmip-4.1.1/biobb_cmip/cmip/cmip_ignore_residues.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6440 2023-08-02 09:01:49.000000 biobb_cmip-4.1.1/biobb_cmip/cmip/cmip_prepare_pdb.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7692 2023-08-02 09:01:49.000000 biobb_cmip-4.1.1/biobb_cmip/cmip/cmip_prepare_structure.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    22063 2023-09-15 13:20:08.000000 biobb_cmip-4.1.1/biobb_cmip/cmip/cmip_run.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10582 2023-09-15 13:19:47.000000 biobb_cmip-4.1.1/biobb_cmip/cmip/cmip_titration.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    25756 2023-09-15 13:18:17.000000 biobb_cmip-4.1.1/biobb_cmip/cmip/common.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-02-29 14:09:16.270361 biobb_cmip-4.1.1/biobb_cmip/cmip/dat/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    32705 2022-05-26 11:33:12.000000 biobb_cmip-4.1.1/biobb_cmip/cmip/dat/aa.lib
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    24096 2022-05-26 11:33:12.000000 biobb_cmip-4.1.1/biobb_cmip/cmip/dat/nuc.lib
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      766 2022-05-26 11:33:12.000000 biobb_cmip-4.1.1/biobb_cmip/cmip/dat/solv.vdwprm
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      611 2022-05-26 11:33:12.000000 biobb_cmip-4.1.1/biobb_cmip/cmip/dat/vdwprm
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-02-29 14:09:16.270517 biobb_cmip-4.1.1/biobb_cmip/test/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:33:12.000000 biobb_cmip-4.1.1/biobb_cmip/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-02-29 14:09:16.270759 biobb_cmip-4.1.1/biobb_cmip/utils/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:33:12.000000 biobb_cmip-4.1.1/biobb_cmip/utils/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6319 2023-09-15 13:19:34.000000 biobb_cmip-4.1.1/biobb_cmip/utils/representation.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-02-29 14:09:16.268697 biobb_cmip-4.1.1/biobb_cmip.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6257 2024-02-29 14:09:16.000000 biobb_cmip-4.1.1/biobb_cmip.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      707 2024-02-29 14:09:16.000000 biobb_cmip-4.1.1/biobb_cmip.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2024-02-29 14:09:16.000000 biobb_cmip-4.1.1/biobb_cmip.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      303 2024-02-29 14:09:16.000000 biobb_cmip-4.1.1/biobb_cmip.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       71 2024-02-29 14:09:16.000000 biobb_cmip-4.1.1/biobb_cmip.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       11 2024-02-29 14:09:16.000000 biobb_cmip-4.1.1/biobb_cmip.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2024-02-29 14:09:16.271348 biobb_cmip-4.1.1/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1774 2024-02-29 14:06:19.000000 biobb_cmip-4.1.1/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:15:02.646075 biobb_cmip-4.2.0/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:33:12.000000 biobb_cmip-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       79 2022-05-26 11:33:12.000000 biobb_cmip-4.2.0/MANIFEST.in
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6796 2024-05-24 08:15:02.645803 biobb_cmip-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5759 2024-05-24 08:13:35.000000 biobb_cmip-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:15:02.641554 biobb_cmip-4.2.0/biobb_cmip/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       61 2024-05-24 08:13:17.000000 biobb_cmip-4.2.0/biobb_cmip/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:15:02.643418 biobb_cmip-4.2.0/biobb_cmip/cmip/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573      125 2023-09-15 13:20:41.000000 biobb_cmip-4.2.0/biobb_cmip/cmip/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6389 2023-09-15 13:15:32.000000 biobb_cmip-4.2.0/biobb_cmip/cmip/cmip_ignore_residues.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6440 2023-08-02 09:01:49.000000 biobb_cmip-4.2.0/biobb_cmip/cmip/cmip_prepare_pdb.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7692 2023-08-02 09:01:49.000000 biobb_cmip-4.2.0/biobb_cmip/cmip/cmip_prepare_structure.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    22062 2024-03-05 15:03:52.000000 biobb_cmip-4.2.0/biobb_cmip/cmip/cmip_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10582 2023-09-15 13:19:47.000000 biobb_cmip-4.2.0/biobb_cmip/cmip/cmip_titration.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    25756 2023-09-15 13:18:17.000000 biobb_cmip-4.2.0/biobb_cmip/cmip/common.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:15:02.644900 biobb_cmip-4.2.0/biobb_cmip/cmip/dat/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    32705 2022-05-26 11:33:12.000000 biobb_cmip-4.2.0/biobb_cmip/cmip/dat/aa.lib
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    24096 2022-05-26 11:33:12.000000 biobb_cmip-4.2.0/biobb_cmip/cmip/dat/nuc.lib
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      766 2022-05-26 11:33:12.000000 biobb_cmip-4.2.0/biobb_cmip/cmip/dat/solv.vdwprm
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      611 2022-05-26 11:33:12.000000 biobb_cmip-4.2.0/biobb_cmip/cmip/dat/vdwprm
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:15:02.645230 biobb_cmip-4.2.0/biobb_cmip/test/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:33:12.000000 biobb_cmip-4.2.0/biobb_cmip/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:15:02.645493 biobb_cmip-4.2.0/biobb_cmip/utils/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:33:12.000000 biobb_cmip-4.2.0/biobb_cmip/utils/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6319 2023-09-15 13:19:34.000000 biobb_cmip-4.2.0/biobb_cmip/utils/representation.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 08:15:02.642511 biobb_cmip-4.2.0/biobb_cmip.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6796 2024-05-24 08:15:02.000000 biobb_cmip-4.2.0/biobb_cmip.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      707 2024-05-24 08:15:02.000000 biobb_cmip-4.2.0/biobb_cmip.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2024-05-24 08:15:02.000000 biobb_cmip-4.2.0/biobb_cmip.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      303 2024-05-24 08:15:02.000000 biobb_cmip-4.2.0/biobb_cmip.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       71 2024-05-24 08:15:02.000000 biobb_cmip-4.2.0/biobb_cmip.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       11 2024-05-24 08:15:02.000000 biobb_cmip-4.2.0/biobb_cmip.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2024-05-24 08:15:02.646125 biobb_cmip-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1774 2024-05-24 08:13:04.000000 biobb_cmip-4.2.0/setup.py
```

### Comparing `biobb_cmip-4.1.1/LICENSE` & `biobb_cmip-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/PKG-INFO` & `biobb_cmip-4.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb_cmip
-Version: 4.1.1
+Version: 4.2.0
 Summary: biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.
 Home-page: https://github.com/bioexcel/biobb_cmip
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-cmip.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -15,24 +15,24 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: biobb_common==4.1.0
+Requires-Dist: biobb_common==4.2.0
 Requires-Dist: mdanalysis>=2.0.0
 Requires-Dist: biobb_structure_checking==3.13.4
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_cmip?label=Version)](https://GitHub.com/bioexcel/biobb_cmip/tags/)
 [![](https://img.shields.io/pypi/v/biobb-cmip.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-cmip/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_cmip?label=Conda)](https://anaconda.org/bioconda/biobb_cmip)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_cmip?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_cmip)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_cmip?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_cmip)
 [![](https://img.shields.io/pypi/pyversions/biobb-cmip.svg?label=Python%20Versions)](https://pypi.org/project/biobb-cmip/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_cmip)
 
 [![](https://readthedocs.org/projects/biobb-cmip/badge/?version=latest&label=Docs)](https://biobb-cmip.readthedocs.io/en/latest/?badge=latest)
@@ -43,86 +43,93 @@
 
 [![](https://docs.bioexcel.eu/biobb_cmip/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_cmip/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_cmip/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_cmip/coverage/)
 [![](https://docs.bioexcel.eu/biobb_cmip/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_cmip/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_cmip?label=Last%20Commit)](https://github.com/bioexcel/biobb_cmip/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_cmip.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_cmip/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_cmip
 
 ### Introduction
 Biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-cmip.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_cmip>=4.1.1"
+        pip install "biobb_cmip>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_cmip>=4.1.1"
+        conda install -c bioconda "biobb_cmip>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-cmip.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_cmip:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_cmip:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_cmip:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_cmip:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_cmip.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-cmip.readthedocs.io/en/latest/command_line.html).
 
 
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

### Comparing `biobb_cmip-4.1.1/README.md` & `biobb_cmip-4.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_cmip?label=Version)](https://GitHub.com/bioexcel/biobb_cmip/tags/)
 [![](https://img.shields.io/pypi/v/biobb-cmip.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-cmip/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_cmip?label=Conda)](https://anaconda.org/bioconda/biobb_cmip)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_cmip?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_cmip)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_cmip?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_cmip)
 [![](https://img.shields.io/pypi/pyversions/biobb-cmip.svg?label=Python%20Versions)](https://pypi.org/project/biobb-cmip/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_cmip)
 
 [![](https://readthedocs.org/projects/biobb-cmip/badge/?version=latest&label=Docs)](https://biobb-cmip.readthedocs.io/en/latest/?badge=latest)
@@ -18,86 +18,93 @@
 
 [![](https://docs.bioexcel.eu/biobb_cmip/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_cmip/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_cmip/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_cmip/coverage/)
 [![](https://docs.bioexcel.eu/biobb_cmip/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_cmip/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_cmip?label=Last%20Commit)](https://github.com/bioexcel/biobb_cmip/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_cmip.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_cmip/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_cmip
 
 ### Introduction
 Biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-cmip.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_cmip>=4.1.1"
+        pip install "biobb_cmip>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_cmip>=4.1.1"
+        conda install -c bioconda "biobb_cmip>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-cmip.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_cmip:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_cmip:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_cmip:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_cmip:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_cmip.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-cmip.readthedocs.io/en/latest/command_line.html).
 
 
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

### Comparing `biobb_cmip-4.1.1/biobb_cmip/cmip/cmip_ignore_residues.py` & `biobb_cmip-4.2.0/biobb_cmip/cmip/cmip_ignore_residues.py`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/biobb_cmip/cmip/cmip_prepare_pdb.py` & `biobb_cmip-4.2.0/biobb_cmip/cmip/cmip_prepare_pdb.py`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/biobb_cmip/cmip/cmip_prepare_structure.py` & `biobb_cmip-4.2.0/biobb_cmip/cmip/cmip_prepare_structure.py`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/biobb_cmip/cmip/cmip_run.py` & `biobb_cmip-4.2.0/biobb_cmip/cmip/cmip_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Args:
         input_pdb_path (str): Path to the input PDB file. File type: input. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_cmip/master/biobb_cmip/test/data/cmip/1kim_h.pdb>`_. Accepted formats: pdb (edam:format_1476).
         input_probe_pdb_path (str) (Optional): Path to the input probe file in PDB format. File type: input. Accepted formats: pdb (edam:format_1476).
         output_pdb_path (str) (Optional): Path to the output PDB file. File type: output. `Sample file <https://raw.githubusercontent.com/bioexcel/biobb_cmip/master/biobb_cmip/test/reference/cmip/1kim_neutral.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_grd_path (str) (Optional): Path to the output grid file in GRD format. File type: output. Accepted formats: grd (edam:format_2330).
         output_cube_path (str) (Optional): Path to the output grid file in cube format. File type: output. Accepted formats: cube (edam:format_2330).
         output_rst_path (str) (Optional): Path to the output restart file. File type: output. Accepted formats: txt (edam:format_2330).
-        input_rst_path (str) (Optional): Path to the input restart file. File type: output. Accepted formats: txt (edam:format_2330).
+        input_rst_path (str) (Optional): Path to the input restart file. File type: input. Accepted formats: txt (edam:format_2330).
         output_byat_path (str) (Optional): Path to the output atom by atom energy file. File type: output. Accepted formats: txt (edam:format_2330), out (edam:format_2330).
         output_log_path (str) (Optional): Path to the output CMIP log file LOG. File type: output. `Sample file <https://github.com/bioexcel/biobb_cmip/raw/master/biobb_cmip/test/reference/cmip/ref_cmip.log>`_. Accepted formats: log (edam:format_2330).
         input_vdw_params_path (str) (Optional): Path to the CMIP input Van der Waals force parameters, if not provided the CMIP conda installation one is used ("$CONDA_PREFIX/share/cmip/dat/vdwprm"). File type: input. Accepted formats: txt (edam:format_2330).
         input_params_path (str) (Optional): Path to the CMIP input parameters file. File type: input. Accepted formats: txt (edam:format_2330).
         output_json_box_path (str) (Optional): Path to the output CMIP box in JSON format. File type: output. `Sample file <https://github.com/bioexcel/biobb_cmip/raw/master/biobb_cmip/test/reference/cmip/ref_box.json>`_. Accepted formats: json (edam:format_3464).
         output_json_external_box_path (str) (Optional): Path to the output external CMIP box in JSON format. File type: output. `Sample file <https://github.com/bioexcel/biobb_cmip/raw/master/biobb_cmip/test/reference/cmip/ref_box.json>`_. Accepted formats: json (edam:format_3464).
         input_json_box_path (str) (Optional): Path to the input CMIP box in JSON format. File type: input. `Sample file <https://github.com/bioexcel/biobb_cmip/raw/master/biobb_cmip/test/reference/cmip/ref_box.json>`_. Accepted formats: json (edam:format_3464).
```

### Comparing `biobb_cmip-4.1.1/biobb_cmip/cmip/cmip_titration.py` & `biobb_cmip-4.2.0/biobb_cmip/cmip/cmip_titration.py`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/biobb_cmip/cmip/common.py` & `biobb_cmip-4.2.0/biobb_cmip/cmip/common.py`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/biobb_cmip/cmip/dat/aa.lib` & `biobb_cmip-4.2.0/biobb_cmip/cmip/dat/aa.lib`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/biobb_cmip/cmip/dat/nuc.lib` & `biobb_cmip-4.2.0/biobb_cmip/cmip/dat/nuc.lib`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/biobb_cmip/cmip/dat/solv.vdwprm` & `biobb_cmip-4.2.0/biobb_cmip/cmip/dat/solv.vdwprm`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/biobb_cmip/cmip/dat/vdwprm` & `biobb_cmip-4.2.0/biobb_cmip/cmip/dat/vdwprm`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/biobb_cmip/utils/representation.py` & `biobb_cmip-4.2.0/biobb_cmip/utils/representation.py`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/biobb_cmip.egg-info/PKG-INFO` & `biobb_cmip-4.2.0/biobb_cmip.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb-cmip
-Version: 4.1.1
+Version: 4.2.0
 Summary: biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.
 Home-page: https://github.com/bioexcel/biobb_cmip
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-cmip.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -15,24 +15,24 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: biobb_common==4.1.0
+Requires-Dist: biobb_common==4.2.0
 Requires-Dist: mdanalysis>=2.0.0
 Requires-Dist: biobb_structure_checking==3.13.4
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_cmip?label=Version)](https://GitHub.com/bioexcel/biobb_cmip/tags/)
 [![](https://img.shields.io/pypi/v/biobb-cmip.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-cmip/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_cmip?label=Conda)](https://anaconda.org/bioconda/biobb_cmip)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_cmip?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_cmip)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_cmip?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_cmip:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_cmip)
 [![](https://img.shields.io/pypi/pyversions/biobb-cmip.svg?label=Python%20Versions)](https://pypi.org/project/biobb-cmip/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_cmip)
 
 [![](https://readthedocs.org/projects/biobb-cmip/badge/?version=latest&label=Docs)](https://biobb-cmip.readthedocs.io/en/latest/?badge=latest)
@@ -43,86 +43,93 @@
 
 [![](https://docs.bioexcel.eu/biobb_cmip/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_cmip/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_cmip/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_cmip/coverage/)
 [![](https://docs.bioexcel.eu/biobb_cmip/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_cmip/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_cmip?label=Last%20Commit)](https://github.com/bioexcel/biobb_cmip/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_cmip.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_cmip/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_cmip
 
 ### Introduction
 Biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-cmip.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_cmip>=4.1.1"
+        pip install "biobb_cmip>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_cmip>=4.1.1"
+        conda install -c bioconda "biobb_cmip>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-cmip.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-cmip.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_cmip:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_cmip:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_cmip:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_cmip:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_cmip.sif https://depot.galaxyproject.org/singularity/biobb_cmip:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_cmip.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-cmip.readthedocs.io/en/latest/command_line.html).
 
 
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

### Comparing `biobb_cmip-4.1.1/biobb_cmip.egg-info/SOURCES.txt` & `biobb_cmip-4.2.0/biobb_cmip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_cmip-4.1.1/setup.py` & `biobb_cmip-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_cmip",
-    version="4.1.1",
+    version="4.2.0",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="biobb_cmip is the Biobb module collection to compute classical molecular interaction potentials.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_cmip",
     project_urls={
         "Documentation": "http://biobb-cmip.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
     include_package_data=True,
     install_requires=[
-        'biobb_common==4.1.0',
+        'biobb_common==4.2.0',
         'mdanalysis>=2.0.0',
         'biobb_structure_checking==3.13.4'
     ],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "cmip_run = biobb_cmip.cmip.cmip_run:main",
```

