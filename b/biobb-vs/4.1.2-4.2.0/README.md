# Comparing `tmp/biobb_vs-4.1.2.tar.gz` & `tmp/biobb_vs-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_vs-4.1.2.tar", last modified: Wed May  8 08:10:00 2024, max compression
+gzip compressed data, was "biobb_vs-4.2.0.tar", last modified: Fri May 24 13:24:03 2024, max compression
```

## Comparing `biobb_vs-4.1.2.tar` & `biobb_vs-4.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.736750 biobb_vs-4.1.2/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:36:06.000000 biobb_vs-4.1.2/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6750 2024-05-08 08:10:00.736521 biobb_vs-4.1.2/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5855 2024-05-08 08:01:19.000000 biobb_vs-4.1.2/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.733464 biobb_vs-4.1.2/biobb_vs/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       79 2024-05-08 08:00:58.000000 biobb_vs-4.1.2/biobb_vs/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.734900 biobb_vs-4.1.2/biobb_vs/fpocket/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       79 2023-04-13 09:46:16.000000 biobb_vs-4.1.2/biobb_vs/fpocket/__init__.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6271 2024-05-08 08:07:28.000000 biobb_vs-4.1.2/biobb_vs/fpocket/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    10117 2023-04-13 09:43:47.000000 biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_filter.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9777 2024-05-07 13:49:44.000000 biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_run.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7531 2023-04-13 09:48:19.000000 biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_select.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.735021 biobb_vs-4.1.2/biobb_vs/test/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:36:06.000000 biobb_vs-4.1.2/biobb_vs/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.735884 biobb_vs-4.1.2/biobb_vs/utils/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       87 2023-04-13 09:46:25.000000 biobb_vs-4.1.2/biobb_vs/utils/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    18234 2024-05-08 07:48:18.000000 biobb_vs-4.1.2/biobb_vs/utils/bindingsite.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9027 2023-04-13 10:01:05.000000 biobb_vs-4.1.2/biobb_vs/utils/box.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11168 2023-09-14 09:21:33.000000 biobb_vs-4.1.2/biobb_vs/utils/box_residues.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    42086 2024-05-07 15:02:53.000000 biobb_vs-4.1.2/biobb_vs/utils/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7590 2023-09-14 09:21:44.000000 biobb_vs-4.1.2/biobb_vs/utils/extract_model_pdbqt.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.736262 biobb_vs-4.1.2/biobb_vs/vina/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       46 2023-04-13 09:46:34.000000 biobb_vs-4.1.2/biobb_vs/vina/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11684 2024-04-02 08:03:45.000000 biobb_vs-4.1.2/biobb_vs/vina/autodock_vina_run.py
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2882 2023-04-13 10:20:42.000000 biobb_vs-4.1.2/biobb_vs/vina/common.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-08 08:10:00.734241 biobb_vs-4.1.2/biobb_vs.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6750 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      683 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      417 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        9 2024-05-08 08:10:00.000000 biobb_vs-4.1.2/biobb_vs.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2024-05-08 08:10:00.736797 biobb_vs-4.1.2/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1756 2024-05-08 08:00:29.000000 biobb_vs-4.1.2/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:24:03.081163 biobb_vs-4.2.0/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:36:06.000000 biobb_vs-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6750 2024-05-24 13:24:03.080889 biobb_vs-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5855 2024-05-24 13:23:02.000000 biobb_vs-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:24:03.077985 biobb_vs-4.2.0/biobb_vs/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       79 2024-05-24 13:22:50.000000 biobb_vs-4.2.0/biobb_vs/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:24:03.079368 biobb_vs-4.2.0/biobb_vs/fpocket/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       79 2023-04-13 09:46:16.000000 biobb_vs-4.2.0/biobb_vs/fpocket/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6271 2024-05-08 08:07:28.000000 biobb_vs-4.2.0/biobb_vs/fpocket/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    10117 2023-04-13 09:43:47.000000 biobb_vs-4.2.0/biobb_vs/fpocket/fpocket_filter.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9777 2024-05-07 13:49:44.000000 biobb_vs-4.2.0/biobb_vs/fpocket/fpocket_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7531 2023-04-13 09:48:19.000000 biobb_vs-4.2.0/biobb_vs/fpocket/fpocket_select.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:24:03.079490 biobb_vs-4.2.0/biobb_vs/test/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:36:06.000000 biobb_vs-4.2.0/biobb_vs/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:24:03.080265 biobb_vs-4.2.0/biobb_vs/utils/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       87 2023-04-13 09:46:25.000000 biobb_vs-4.2.0/biobb_vs/utils/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18234 2024-05-08 07:48:18.000000 biobb_vs-4.2.0/biobb_vs/utils/bindingsite.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9027 2023-04-13 10:01:05.000000 biobb_vs-4.2.0/biobb_vs/utils/box.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11168 2023-09-14 09:21:33.000000 biobb_vs-4.2.0/biobb_vs/utils/box_residues.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    42086 2024-05-07 15:02:53.000000 biobb_vs-4.2.0/biobb_vs/utils/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7704 2024-05-24 13:14:04.000000 biobb_vs-4.2.0/biobb_vs/utils/extract_model_pdbqt.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:24:03.080642 biobb_vs-4.2.0/biobb_vs/vina/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       46 2023-04-13 09:46:34.000000 biobb_vs-4.2.0/biobb_vs/vina/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11684 2024-04-02 08:03:45.000000 biobb_vs-4.2.0/biobb_vs/vina/autodock_vina_run.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2882 2023-04-13 10:20:42.000000 biobb_vs-4.2.0/biobb_vs/vina/common.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 13:24:03.078746 biobb_vs-4.2.0/biobb_vs.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6750 2024-05-24 13:24:03.000000 biobb_vs-4.2.0/biobb_vs.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      683 2024-05-24 13:24:03.000000 biobb_vs-4.2.0/biobb_vs.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2024-05-24 13:24:03.000000 biobb_vs-4.2.0/biobb_vs.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      417 2024-05-24 13:24:03.000000 biobb_vs-4.2.0/biobb_vs.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2024-05-24 13:24:03.000000 biobb_vs-4.2.0/biobb_vs.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        9 2024-05-24 13:24:03.000000 biobb_vs-4.2.0/biobb_vs.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2024-05-24 13:24:03.081216 biobb_vs-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1756 2024-05-24 13:22:40.000000 biobb_vs-4.2.0/setup.py
```

### Comparing `biobb_vs-4.1.2/LICENSE` & `biobb_vs-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/PKG-INFO` & `biobb_vs-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb_vs
-Version: 4.1.2
+Version: 4.2.0
 Summary: Biobb_vs is the Biobb module collection to perform virtual screening studies.
 Home-page: https://github.com/bioexcel/biobb_vs
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
 Project-URL: Documentation, http://biobb-vs.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -14,22 +14,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: biobb_common==4.1.0
+Requires-Dist: biobb_common==4.2.0
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_vs?label=Version)](https://GitHub.com/bioexcel/biobb_vs/tags/)
 [![](https://img.shields.io/pypi/v/biobb-vs.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-vs/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_vs?label=Conda)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_vs?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_vs?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_vs)
 [![](https://img.shields.io/pypi/pyversions/biobb-vs.svg?label=Python%20Versions)](https://pypi.org/project/biobb-vs/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_vs)
 
 [![](https://readthedocs.org/projects/biobb-vs/badge/?version=latest&label=Docs)](https://biobb-vs.readthedocs.io/en/latest/?badge=latest)
@@ -60,60 +60,60 @@
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-vs.readthedocs.io/en/latest/).
 
 > At the time of publishing the current version, **autodock_vina has not been compiled for the new ARM mac M1/M2 chips**. So the vina.autodock_vina_run only work in these computers through docker containers.
 
 ### Version
-v4.1.2 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_vs>=4.1.2"
+        pip install "biobb_vs>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_vs>=4.1.2"
+        conda install -c bioconda "biobb_vs>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-vs.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_vs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_vs:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0
+        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_vs.sif <command>
```

### Comparing `biobb_vs-4.1.2/README.md` & `biobb_vs-4.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_vs?label=Version)](https://GitHub.com/bioexcel/biobb_vs/tags/)
 [![](https://img.shields.io/pypi/v/biobb-vs.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-vs/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_vs?label=Conda)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_vs?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_vs?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_vs)
 [![](https://img.shields.io/pypi/pyversions/biobb-vs.svg?label=Python%20Versions)](https://pypi.org/project/biobb-vs/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_vs)
 
 [![](https://readthedocs.org/projects/biobb-vs/badge/?version=latest&label=Docs)](https://biobb-vs.readthedocs.io/en/latest/?badge=latest)
@@ -38,60 +38,60 @@
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-vs.readthedocs.io/en/latest/).
 
 > At the time of publishing the current version, **autodock_vina has not been compiled for the new ARM mac M1/M2 chips**. So the vina.autodock_vina_run only work in these computers through docker containers.
 
 ### Version
-v4.1.2 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_vs>=4.1.2"
+        pip install "biobb_vs>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_vs>=4.1.2"
+        conda install -c bioconda "biobb_vs>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-vs.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_vs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_vs:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0
+        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_vs.sif <command>
```

### Comparing `biobb_vs-4.1.2/biobb_vs/fpocket/common.py` & `biobb_vs-4.2.0/biobb_vs/fpocket/common.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_filter.py` & `biobb_vs-4.2.0/biobb_vs/fpocket/fpocket_filter.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_run.py` & `biobb_vs-4.2.0/biobb_vs/fpocket/fpocket_run.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/biobb_vs/fpocket/fpocket_select.py` & `biobb_vs-4.2.0/biobb_vs/fpocket/fpocket_select.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/biobb_vs/utils/bindingsite.py` & `biobb_vs-4.2.0/biobb_vs/utils/bindingsite.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/biobb_vs/utils/box.py` & `biobb_vs-4.2.0/biobb_vs/utils/box.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/biobb_vs/utils/box_residues.py` & `biobb_vs-4.2.0/biobb_vs/utils/box_residues.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/biobb_vs/utils/common.py` & `biobb_vs-4.2.0/biobb_vs/utils/common.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/biobb_vs/utils/extract_model_pdbqt.py` & `biobb_vs-4.2.0/biobb_vs/utils/extract_model_pdbqt.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     import Bio.Align.substitution_matrices
 
 
 class ExtractModelPDBQT(BiobbObject):
     """
     | biobb_vs ExtractModelPDBQT
     | Extracts a model from a PDBQT file with several models.
+    | Extracts a model from a PDBQT file with several models. The model number to extract is defined by the user.
 
     Args:
         input_pdbqt_path (str): Input PDBQT file. File type: input. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/data/utils/models.pdbqt>`_. Accepted formats: pdbqt (edam:format_1476).
         output_pdbqt_path (str): Output PDBQT file. File type: output. `Sample file <https://github.com/bioexcel/biobb_vs/raw/master/biobb_vs/test/reference/utils/ref_extract_model.pdbqt>`_. Accepted formats: pdbqt (edam:format_1476).
         properties (dic - Python dictionary object containing the tool parameters, not input/output files):
             * **model** (*int*) - (1) [0~1000|1] Model number to extract from input_pdbqt_path.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
```

### Comparing `biobb_vs-4.1.2/biobb_vs/vina/autodock_vina_run.py` & `biobb_vs-4.2.0/biobb_vs/vina/autodock_vina_run.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/biobb_vs/vina/common.py` & `biobb_vs-4.2.0/biobb_vs/vina/common.py`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/biobb_vs.egg-info/PKG-INFO` & `biobb_vs-4.2.0/biobb_vs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb-vs
-Version: 4.1.2
+Version: 4.2.0
 Summary: Biobb_vs is the Biobb module collection to perform virtual screening studies.
 Home-page: https://github.com/bioexcel/biobb_vs
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
 Project-URL: Documentation, http://biobb-vs.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -14,22 +14,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: biobb_common==4.1.0
+Requires-Dist: biobb_common==4.2.0
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_vs?label=Version)](https://GitHub.com/bioexcel/biobb_vs/tags/)
 [![](https://img.shields.io/pypi/v/biobb-vs.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-vs/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_vs?label=Conda)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_vs?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_vs)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_vs?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_vs:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_vs)
 [![](https://img.shields.io/pypi/pyversions/biobb-vs.svg?label=Python%20Versions)](https://pypi.org/project/biobb-vs/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_vs)
 
 [![](https://readthedocs.org/projects/biobb-vs/badge/?version=latest&label=Docs)](https://biobb-vs.readthedocs.io/en/latest/?badge=latest)
@@ -60,60 +60,60 @@
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-vs.readthedocs.io/en/latest/).
 
 > At the time of publishing the current version, **autodock_vina has not been compiled for the new ARM mac M1/M2 chips**. So the vina.autodock_vina_run only work in these computers through docker containers.
 
 ### Version
-v4.1.2 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_vs>=4.1.2"
+        pip install "biobb_vs>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_vs>=4.1.2"
+        conda install -c bioconda "biobb_vs>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-vs.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-vs.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_vs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_vs:4.1.2--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_vs:4.2.0--pyhdfd78af_0 <command>
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.1.2--pyhdfd78af_0
+        singularity pull --name biobb_vs.sif https://depot.galaxyproject.org/singularity/biobb_vs:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_vs.sif <command>
```

### Comparing `biobb_vs-4.1.2/biobb_vs.egg-info/SOURCES.txt` & `biobb_vs-4.2.0/biobb_vs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_vs-4.1.2/setup.py` & `biobb_vs-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_vs",
-    version="4.1.2",
+    version="4.2.0",
     author="Biobb developers",
     author_email="genis.bayarri@irbbarcelona.org",
     description="Biobb_vs is the Biobb module collection to perform virtual screening studies.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_vs",
     project_urls={
         "Documentation": "http://biobb-vs.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==4.1.0'],
+    install_requires=['biobb_common==4.2.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "fpocket_filter = biobb_vs.fpocket.fpocket_filter:main",
             "fpocket_run = biobb_vs.fpocket.fpocket_run:main",
             "fpocket_select = biobb_vs.fpocket.fpocket_select:main",
             "bindingsite = biobb_vs.utils.bindingsite:main",
```

