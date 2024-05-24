# Comparing `tmp/biobb_pdb_tools-4.1.1.tar.gz` & `tmp/biobb_pdb_tools-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_pdb_tools-4.1.1.tar", last modified: Mon Jan 22 16:04:27 2024, max compression
+gzip compressed data, was "biobb_pdb_tools-4.2.0.tar", last modified: Fri May 24 12:57:09 2024, max compression
```

## Comparing `biobb_pdb_tools-4.1.1.tar` & `biobb_pdb_tools-4.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)        0 2024-01-22 16:04:27.635857 biobb_pdb_tools-4.1.1/
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)    11358 2023-10-16 09:22:54.000000 biobb_pdb_tools-4.1.1/LICENSE
--rw-r--r--   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     6195 2024-01-22 16:04:27.635637 biobb_pdb_tools-4.1.1/PKG-INFO
--rw-r--r--   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     5228 2024-01-22 15:59:17.000000 biobb_pdb_tools-4.1.1/README.md
-drwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)        0 2024-01-22 16:04:27.631304 biobb_pdb_tools-4.1.1/biobb_pdb_tools/
--rw-r--r--   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)       71 2024-01-22 15:58:30.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/__init__.py
-drwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)        0 2024-01-22 16:04:27.635151 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)      279 2024-01-22 15:19:41.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/__init__.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     5120 2024-01-09 15:16:25.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_chain.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     4709 2024-01-09 15:16:35.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_chainxseg.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     4667 2024-01-09 15:22:06.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_delhetatm.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     4616 2024-01-09 15:14:09.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_fetch.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     5476 2024-01-19 14:27:28.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_merge.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     5594 2024-01-19 14:31:46.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_mkensemble.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     5157 2024-01-15 10:06:59.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_reres.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     5081 2024-01-09 15:24:23.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_seg.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     5865 2024-01-09 15:17:51.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_splitmodel.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     5866 2024-01-09 15:18:23.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_splitseg.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     5101 2024-01-09 15:21:26.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_tidy.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     5190 2024-01-09 15:26:01.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_tofasta.py
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     4690 2024-01-22 14:38:15.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_uniqname.py
-drwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)        0 2024-01-22 16:04:27.635410 biobb_pdb_tools-4.1.1/biobb_pdb_tools/test/
--rwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)        0 2024-01-22 12:06:35.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools/test/__init__.py
-drwxr-xr-x   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)        0 2024-01-22 16:04:27.632073 biobb_pdb_tools-4.1.1/biobb_pdb_tools.egg-info/
--rw-r--r--   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     6195 2024-01-22 16:04:27.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools.egg-info/PKG-INFO
--rw-r--r--   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)      969 2024-01-22 16:04:27.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools.egg-info/SOURCES.txt
--rw-r--r--   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)        1 2024-01-22 16:04:27.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools.egg-info/dependency_links.txt
--rw-r--r--   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)      909 2024-01-22 16:04:27.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools.egg-info/entry_points.txt
--rw-r--r--   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)       20 2024-01-22 16:04:27.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools.egg-info/requires.txt
--rw-r--r--   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)       16 2024-01-22 16:04:27.000000 biobb_pdb_tools-4.1.1/biobb_pdb_tools.egg-info/top_level.txt
--rw-r--r--   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)       38 2024-01-22 16:04:27.635905 biobb_pdb_tools-4.1.1/setup.cfg
--rw-r--r--   0 agarciad (995893168) IRBBARCELONA\Domain Users (1791188573)     2392 2024-01-22 15:58:15.000000 biobb_pdb_tools-4.1.1/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 12:57:09.842277 biobb_pdb_tools-4.2.0/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2023-11-16 15:06:50.000000 biobb_pdb_tools-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6734 2024-05-24 12:57:09.841974 biobb_pdb_tools-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5767 2024-05-24 11:48:51.000000 biobb_pdb_tools-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 12:57:09.838451 biobb_pdb_tools-4.2.0/biobb_pdb_tools/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       71 2024-05-24 11:48:38.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 12:57:09.841525 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573      279 2024-03-12 10:54:35.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5120 2024-01-19 12:01:26.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_chain.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4709 2024-01-19 12:01:26.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_chainxseg.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4667 2024-01-19 12:01:26.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_delhetatm.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4616 2024-01-19 12:01:26.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_fetch.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5476 2024-01-22 11:12:34.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_merge.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5594 2024-01-22 11:12:34.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_mkensemble.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5157 2024-01-19 12:01:26.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_reres.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5081 2024-01-19 12:01:26.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_seg.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5865 2024-01-19 12:01:26.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_splitmodel.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5866 2024-01-19 12:01:26.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_splitseg.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5101 2024-01-19 12:01:26.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_tidy.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5190 2024-01-19 12:01:26.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_tofasta.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4690 2024-03-12 10:54:35.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_uniqname.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 12:57:09.841659 biobb_pdb_tools-4.2.0/biobb_pdb_tools/test/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-11-16 15:06:50.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 12:57:09.839230 biobb_pdb_tools-4.2.0/biobb_pdb_tools.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6734 2024-05-24 12:57:09.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      969 2024-05-24 12:57:09.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2024-05-24 12:57:09.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      909 2024-05-24 12:57:09.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2024-05-24 12:57:09.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       16 2024-05-24 12:57:09.000000 biobb_pdb_tools-4.2.0/biobb_pdb_tools.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2024-05-24 12:57:09.842331 biobb_pdb_tools-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2392 2024-05-24 11:48:28.000000 biobb_pdb_tools-4.2.0/setup.py
```

### Comparing `biobb_pdb_tools-4.1.1/LICENSE` & `biobb_pdb_tools-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/PKG-INFO` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb_pdb_tools
-Version: 4.1.1
+Name: biobb-pdb-tools
+Version: 4.2.0
 Summary: Biobb_pdb_tools is a swiss army knife for manipulating and editing PDB files.
 Home-page: https://github.com/bioexcel/biobb_pdb_tools
 Author: Biobb developers
 Author-email: agustin.garcia@irbbarcelona.org
 Project-URL: Documentation, http://biobb-pdb-tools.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -15,22 +15,22 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: biobb_common==4.1.0
+Requires-Dist: biobb_common==4.2.0
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pdb_tools?label=Version)](https://GitHub.com/bioexcel/biobb_pdb_tools/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pdb-tools.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pdb-tools/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pdb_tools?label=Conda)](https://anaconda.org/bioconda/biobb_pdb_tools)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pdb_tools?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pdb_tools)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pdb_tools?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pdb_tools)
 [![](https://img.shields.io/pypi/pyversions/biobb-pdb-tools.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pdb-tools/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pdb_tools)
 
 [![](https://readthedocs.org/projects/biobb-pdb-tools/badge/?version=latest&label=Docs)](https://biobb-pdb-tools.readthedocs.io/en/latest/?badge=latest)
@@ -41,68 +41,75 @@
 
 [![](https://docs.bioexcel.eu/biobb_pdb_tools/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_pdb_tools/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_pdb_tools/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_pdb_tools/coverage/)
 [![](https://docs.bioexcel.eu/biobb_pdb_tools/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_pdb_tools/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_pdb_tools?label=Last%20Commit)](https://github.com/bioexcel/biobb_pdb_tools/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pdb_tools.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pdb_tools/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_pdb_tools
 
 ## Introduction
 biobb_pdb_tools is a swiss army knife for manipulating and editing PDB files. 
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pdb-tools.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pdb_tools>=4.1.1"
+        pip install "biobb_pdb_tools>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-pdb-tools.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pdb_tools>=4.1.1"
+        conda install -c bioconda "biobb_pdb_tools>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pdb-tools.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pdb-tools.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pdb_tools:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pdb_tools:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pdb_tools:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pdb_tools:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pdb_tools.sif https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_pdb_tools.sif https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pdb_tools.sif <command>
```

### Comparing `biobb_pdb_tools-4.1.1/README.md` & `biobb_pdb_tools-4.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pdb_tools?label=Version)](https://GitHub.com/bioexcel/biobb_pdb_tools/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pdb-tools.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pdb-tools/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pdb_tools?label=Conda)](https://anaconda.org/bioconda/biobb_pdb_tools)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pdb_tools?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pdb_tools)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pdb_tools?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pdb_tools)
 [![](https://img.shields.io/pypi/pyversions/biobb-pdb-tools.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pdb-tools/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pdb_tools)
 
 [![](https://readthedocs.org/projects/biobb-pdb-tools/badge/?version=latest&label=Docs)](https://biobb-pdb-tools.readthedocs.io/en/latest/?badge=latest)
@@ -18,68 +18,75 @@
 
 [![](https://docs.bioexcel.eu/biobb_pdb_tools/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_pdb_tools/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_pdb_tools/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_pdb_tools/coverage/)
 [![](https://docs.bioexcel.eu/biobb_pdb_tools/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_pdb_tools/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_pdb_tools?label=Last%20Commit)](https://github.com/bioexcel/biobb_pdb_tools/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pdb_tools.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pdb_tools/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_pdb_tools
 
 ## Introduction
 biobb_pdb_tools is a swiss army knife for manipulating and editing PDB files. 
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pdb-tools.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pdb_tools>=4.1.1"
+        pip install "biobb_pdb_tools>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-pdb-tools.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pdb_tools>=4.1.1"
+        conda install -c bioconda "biobb_pdb_tools>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pdb-tools.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pdb-tools.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pdb_tools:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pdb_tools:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pdb_tools:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pdb_tools:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pdb_tools.sif https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_pdb_tools.sif https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pdb_tools.sif <command>
```

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_chain.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_chain.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_chainxseg.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_chainxseg.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_delhetatm.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_delhetatm.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_fetch.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_fetch.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_merge.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_merge.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_mkensemble.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_mkensemble.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_reres.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_reres.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_seg.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_seg.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_splitmodel.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_splitmodel.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_splitseg.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_splitseg.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_tidy.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_tidy.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_tofasta.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_tofasta.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools/pdb_tools/biobb_pdb_uniqname.py` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools/pdb_tools/biobb_pdb_uniqname.py`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools.egg-info/PKG-INFO` & `biobb_pdb_tools-4.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb-pdb-tools
-Version: 4.1.1
+Name: biobb_pdb_tools
+Version: 4.2.0
 Summary: Biobb_pdb_tools is a swiss army knife for manipulating and editing PDB files.
 Home-page: https://github.com/bioexcel/biobb_pdb_tools
 Author: Biobb developers
 Author-email: agustin.garcia@irbbarcelona.org
 Project-URL: Documentation, http://biobb-pdb-tools.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -15,22 +15,22 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: biobb_common==4.1.0
+Requires-Dist: biobb_common==4.2.0
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pdb_tools?label=Version)](https://GitHub.com/bioexcel/biobb_pdb_tools/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pdb-tools.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pdb-tools/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pdb_tools?label=Conda)](https://anaconda.org/bioconda/biobb_pdb_tools)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pdb_tools?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pdb_tools)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pdb_tools?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pdb_tools)
 [![](https://img.shields.io/pypi/pyversions/biobb-pdb-tools.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pdb-tools/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pdb_tools)
 
 [![](https://readthedocs.org/projects/biobb-pdb-tools/badge/?version=latest&label=Docs)](https://biobb-pdb-tools.readthedocs.io/en/latest/?badge=latest)
@@ -41,68 +41,75 @@
 
 [![](https://docs.bioexcel.eu/biobb_pdb_tools/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_pdb_tools/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_pdb_tools/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_pdb_tools/coverage/)
 [![](https://docs.bioexcel.eu/biobb_pdb_tools/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_pdb_tools/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_pdb_tools?label=Last%20Commit)](https://github.com/bioexcel/biobb_pdb_tools/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pdb_tools.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pdb_tools/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_pdb_tools
 
 ## Introduction
 biobb_pdb_tools is a swiss army knife for manipulating and editing PDB files. 
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pdb-tools.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pdb_tools>=4.1.1"
+        pip install "biobb_pdb_tools>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-pdb-tools.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pdb_tools>=4.1.1"
+        conda install -c bioconda "biobb_pdb_tools>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pdb-tools.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pdb-tools.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pdb_tools:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_pdb_tools:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pdb_tools:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_pdb_tools:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pdb_tools.sif https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_pdb_tools.sif https://depot.galaxyproject.org/singularity/biobb_pdb_tools:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pdb_tools.sif <command>
```

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools.egg-info/SOURCES.txt` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/biobb_pdb_tools.egg-info/entry_points.txt` & `biobb_pdb_tools-4.2.0/biobb_pdb_tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_pdb_tools-4.1.1/setup.py` & `biobb_pdb_tools-4.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_pdb_tools",
-    version="4.1.1",
+    version="4.2.0",
     author="Biobb developers",
     author_email="agustin.garcia@irbbarcelona.org",
     description="Biobb_pdb_tools is a swiss army knife for manipulating and editing PDB files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_pdb_tools",
     project_urls={
         "Documentation": "http://biobb-pdb-tools.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==4.1.0'],
+    install_requires=['biobb_common==4.2.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "biobb_pdb_chain = biobb_pdb_tools.pdb_tools.biobb_pdb_chain:main",
             "biobb_pdb_chainxseg = biobb_pdb_tools.pdb_tools.biobb_pdb_chainxseg:main",
             "biobb_pdb_delhetatm = biobb_pdb_tools.pdb_tools.biobb_pdb_delhetatm:main",
             "biobb_pdb_fetch = biobb_pdb_tools.pdb_tools.biobb_pdb_fetch:main",
```

