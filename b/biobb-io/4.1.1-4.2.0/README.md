# Comparing `tmp/biobb_io-4.1.1.tar.gz` & `tmp/biobb_io-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_io-4.1.1.tar", last modified: Tue May  7 14:30:48 2024, max compression
+gzip compressed data, was "biobb_io-4.2.0.tar", last modified: Fri May 24 10:50:13 2024, max compression
```

## Comparing `biobb_io-4.1.1.tar` & `biobb_io-4.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-07 14:30:48.786547 biobb_io-4.1.1/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11358 2022-05-26 11:34:05.000000 biobb_io-4.1.1/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6760 2024-05-07 14:30:48.786285 biobb_io-4.1.1/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5845 2024-05-07 14:27:42.000000 biobb_io-4.1.1/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-07 14:30:48.780159 biobb_io-4.1.1/biobb_io/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       58 2024-05-07 14:26:59.000000 biobb_io-4.1.1/biobb_io/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-07 14:30:48.785711 biobb_io-4.1.1/biobb_io/api/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      243 2023-04-12 15:24:32.000000 biobb_io-4.1.1/biobb_io/api/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5082 2023-04-12 15:36:10.000000 biobb_io-4.1.1/biobb_io/api/alphafold.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5527 2023-04-12 15:38:00.000000 biobb_io-4.1.1/biobb_io/api/api_binding_site.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5474 2023-04-12 15:39:47.000000 biobb_io-4.1.1/biobb_io/api/canonical_fasta.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    13075 2024-05-07 14:16:21.000000 biobb_io-4.1.1/biobb_io/api/common.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     4942 2023-04-12 15:44:12.000000 biobb_io-4.1.1/biobb_io/api/drugbank.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5282 2023-04-12 15:52:03.000000 biobb_io-4.1.1/biobb_io/api/ideal_sdf.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5332 2023-05-03 08:22:17.000000 biobb_io-4.1.1/biobb_io/api/ligand.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     4856 2023-04-12 15:57:32.000000 biobb_io-4.1.1/biobb_io/api/memprotmd_sim.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     4821 2023-04-12 15:54:50.000000 biobb_io-4.1.1/biobb_io/api/memprotmd_sim_list.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7179 2023-04-12 15:56:06.000000 biobb_io-4.1.1/biobb_io/api/memprotmd_sim_search.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5366 2023-04-12 15:59:29.000000 biobb_io-4.1.1/biobb_io/api/mmcif.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5674 2023-04-12 16:04:54.000000 biobb_io-4.1.1/biobb_io/api/pdb.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7345 2023-04-12 16:01:22.000000 biobb_io-4.1.1/biobb_io/api/pdb_cluster_zip.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6948 2023-04-12 16:02:37.000000 biobb_io-4.1.1/biobb_io/api/pdb_variants.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5190 2023-04-12 16:06:10.000000 biobb_io-4.1.1/biobb_io/api/structure_info.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-07 14:30:48.786002 biobb_io-4.1.1/biobb_io/test/
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2022-05-26 11:34:05.000000 biobb_io-4.1.1/biobb_io/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2024-05-07 14:30:48.780968 biobb_io-4.1.1/biobb_io.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6760 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      716 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      652 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        9 2024-05-07 14:30:48.000000 biobb_io-4.1.1/biobb_io.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2024-05-07 14:30:48.786599 biobb_io-4.1.1/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2101 2024-05-07 14:26:46.000000 biobb_io-4.1.1/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 10:50:13.160741 biobb_io-4.2.0/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:34:05.000000 biobb_io-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6760 2024-05-24 10:50:13.160456 biobb_io-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5845 2024-05-24 10:49:13.000000 biobb_io-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 10:50:13.156633 biobb_io-4.2.0/biobb_io/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573       58 2024-05-24 10:49:00.000000 biobb_io-4.2.0/biobb_io/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 10:50:13.159913 biobb_io-4.2.0/biobb_io/api/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573      243 2023-04-12 15:24:32.000000 biobb_io-4.2.0/biobb_io/api/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5082 2023-04-12 15:36:10.000000 biobb_io-4.2.0/biobb_io/api/alphafold.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5527 2023-04-12 15:38:00.000000 biobb_io-4.2.0/biobb_io/api/api_binding_site.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5474 2023-04-12 15:39:47.000000 biobb_io-4.2.0/biobb_io/api/canonical_fasta.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13075 2024-05-07 14:16:21.000000 biobb_io-4.2.0/biobb_io/api/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4942 2023-04-12 15:44:12.000000 biobb_io-4.2.0/biobb_io/api/drugbank.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5282 2023-04-12 15:52:03.000000 biobb_io-4.2.0/biobb_io/api/ideal_sdf.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5332 2023-05-03 08:22:17.000000 biobb_io-4.2.0/biobb_io/api/ligand.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4856 2023-04-12 15:57:32.000000 biobb_io-4.2.0/biobb_io/api/memprotmd_sim.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     4821 2023-04-12 15:54:50.000000 biobb_io-4.2.0/biobb_io/api/memprotmd_sim_list.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7179 2023-04-12 15:56:06.000000 biobb_io-4.2.0/biobb_io/api/memprotmd_sim_search.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5366 2023-04-12 15:59:29.000000 biobb_io-4.2.0/biobb_io/api/mmcif.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5674 2023-04-12 16:04:54.000000 biobb_io-4.2.0/biobb_io/api/pdb.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7345 2023-04-12 16:01:22.000000 biobb_io-4.2.0/biobb_io/api/pdb_cluster_zip.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6948 2023-04-12 16:02:37.000000 biobb_io-4.2.0/biobb_io/api/pdb_variants.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5190 2023-04-12 16:06:10.000000 biobb_io-4.2.0/biobb_io/api/structure_info.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 10:50:13.160144 biobb_io-4.2.0/biobb_io/test/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:34:05.000000 biobb_io-4.2.0/biobb_io/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 10:50:13.157390 biobb_io-4.2.0/biobb_io.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6760 2024-05-24 10:50:13.000000 biobb_io-4.2.0/biobb_io.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      716 2024-05-24 10:50:13.000000 biobb_io-4.2.0/biobb_io.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2024-05-24 10:50:13.000000 biobb_io-4.2.0/biobb_io.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      652 2024-05-24 10:50:13.000000 biobb_io-4.2.0/biobb_io.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2024-05-24 10:50:13.000000 biobb_io-4.2.0/biobb_io.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        9 2024-05-24 10:50:13.000000 biobb_io-4.2.0/biobb_io.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2024-05-24 10:50:13.160794 biobb_io-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2101 2024-05-24 10:48:53.000000 biobb_io-4.2.0/setup.py
```

### Comparing `biobb_io-4.1.1/LICENSE` & `biobb_io-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/PKG-INFO` & `biobb_io-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb_io
-Version: 4.1.1
+Version: 4.2.0
 Summary: Biobb_io is the Biobb module collection to fetch data to be consumed by the rest of the Biobb building blocks.
 Home-page: https://github.com/bioexcel/biobb_io
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-io.readthedocs.io/en/latest/
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
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_io?label=Version)](https://GitHub.com/bioexcel/biobb_io/tags/)
 [![](https://img.shields.io/pypi/v/biobb-io.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-io/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_io?label=Conda)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_io?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_io?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_io)
 [![](https://img.shields.io/pypi/pyversions/biobb-io.svg?label=Python%20Versions)](https://pypi.org/project/biobb-io/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_io)
 
 [![](https://readthedocs.org/projects/biobb-io/badge/?version=latest&label=Docs)](https://biobb-io.readthedocs.io/en/latest/?badge=latest)
@@ -59,58 +59,58 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-io.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
-        pip install "biobb_io==4.1.1"
+        pip install "biobb_io==4.2.0"
         
 * Usage: [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 * Installation:
 
 
-        conda install -c bioconda "biobb_io==4.1.1"
+        conda install -c bioconda "biobb_io==4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_io:4.2.0--pyhdfd78af_0
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_io:4.2.0--pyhdfd78af_0 <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html).
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_io.sif <command>
```

### Comparing `biobb_io-4.1.1/README.md` & `biobb_io-4.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_io?label=Version)](https://GitHub.com/bioexcel/biobb_io/tags/)
 [![](https://img.shields.io/pypi/v/biobb-io.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-io/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_io?label=Conda)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_io?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_io?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_io)
 [![](https://img.shields.io/pypi/pyversions/biobb-io.svg?label=Python%20Versions)](https://pypi.org/project/biobb-io/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_io)
 
 [![](https://readthedocs.org/projects/biobb-io/badge/?version=latest&label=Docs)](https://biobb-io.readthedocs.io/en/latest/?badge=latest)
@@ -37,58 +37,58 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-io.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
-        pip install "biobb_io==4.1.1"
+        pip install "biobb_io==4.2.0"
         
 * Usage: [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 * Installation:
 
 
-        conda install -c bioconda "biobb_io==4.1.1"
+        conda install -c bioconda "biobb_io==4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_io:4.2.0--pyhdfd78af_0
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_io:4.2.0--pyhdfd78af_0 <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html).
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_io.sif <command>
```

### Comparing `biobb_io-4.1.1/biobb_io/api/alphafold.py` & `biobb_io-4.2.0/biobb_io/api/alphafold.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/api_binding_site.py` & `biobb_io-4.2.0/biobb_io/api/api_binding_site.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/canonical_fasta.py` & `biobb_io-4.2.0/biobb_io/api/canonical_fasta.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/common.py` & `biobb_io-4.2.0/biobb_io/api/common.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/drugbank.py` & `biobb_io-4.2.0/biobb_io/api/drugbank.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/ideal_sdf.py` & `biobb_io-4.2.0/biobb_io/api/ideal_sdf.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/ligand.py` & `biobb_io-4.2.0/biobb_io/api/ligand.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/memprotmd_sim.py` & `biobb_io-4.2.0/biobb_io/api/memprotmd_sim.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/memprotmd_sim_list.py` & `biobb_io-4.2.0/biobb_io/api/memprotmd_sim_list.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/memprotmd_sim_search.py` & `biobb_io-4.2.0/biobb_io/api/memprotmd_sim_search.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/mmcif.py` & `biobb_io-4.2.0/biobb_io/api/mmcif.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/pdb.py` & `biobb_io-4.2.0/biobb_io/api/pdb.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/pdb_cluster_zip.py` & `biobb_io-4.2.0/biobb_io/api/pdb_cluster_zip.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/pdb_variants.py` & `biobb_io-4.2.0/biobb_io/api/pdb_variants.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io/api/structure_info.py` & `biobb_io-4.2.0/biobb_io/api/structure_info.py`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io.egg-info/PKG-INFO` & `biobb_io-4.2.0/biobb_io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb-io
-Version: 4.1.1
+Version: 4.2.0
 Summary: Biobb_io is the Biobb module collection to fetch data to be consumed by the rest of the Biobb building blocks.
 Home-page: https://github.com/bioexcel/biobb_io
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-io.readthedocs.io/en/latest/
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
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_io?label=Version)](https://GitHub.com/bioexcel/biobb_io/tags/)
 [![](https://img.shields.io/pypi/v/biobb-io.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-io/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_io?label=Conda)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_io?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_io)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_io?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_io:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_io)
 [![](https://img.shields.io/pypi/pyversions/biobb-io.svg?label=Python%20Versions)](https://pypi.org/project/biobb-io/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_io)
 
 [![](https://readthedocs.org/projects/biobb-io/badge/?version=latest&label=Docs)](https://biobb-io.readthedocs.io/en/latest/?badge=latest)
@@ -59,58 +59,58 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-io.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.1 2024.1
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
-        pip install "biobb_io==4.1.1"
+        pip install "biobb_io==4.2.0"
         
 * Usage: [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 * Installation:
 
 
-        conda install -c bioconda "biobb_io==4.1.1"
+        conda install -c bioconda "biobb_io==4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-io.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_io:4.2.0--pyhdfd78af_0
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_io:4.1.1--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_io:4.2.0--pyhdfd78af_0 <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-io.readthedocs.io/en/latest/command_line.html).
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.1.1--pyhdfd78af_0
+        singularity pull --name biobb_io.sif https://depot.galaxyproject.org/singularity/biobb_io:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_io.sif <command>
```

### Comparing `biobb_io-4.1.1/biobb_io.egg-info/SOURCES.txt` & `biobb_io-4.2.0/biobb_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/biobb_io.egg-info/entry_points.txt` & `biobb_io-4.2.0/biobb_io.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_io-4.1.1/setup.py` & `biobb_io-4.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_io",
-    version="4.1.1",
+    version="4.2.0",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="Biobb_io is the Biobb module collection to fetch data to be consumed by the rest of the Biobb building blocks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_io",
     project_urls={
         "Documentation": "http://biobb-io.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==4.1.0'],
+    install_requires=['biobb_common==4.2.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "alphafold = biobb_io.api.alphafold:main",
             "api_binding_site = biobb_io.api.api_binding_site:main",
             "canonical_fasta = biobb_io.api.canonical_fasta:main",
             "drugbank = biobb_io.api.drugbank:main",
```

