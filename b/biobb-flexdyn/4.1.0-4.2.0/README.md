# Comparing `tmp/biobb_flexdyn-4.1.0.tar.gz` & `tmp/biobb_flexdyn-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_flexdyn-4.1.0.tar", last modified: Thu Sep  7 11:27:35 2023, max compression
+gzip compressed data, was "biobb_flexdyn-4.2.0.tar", last modified: Fri May 24 09:52:47 2024, max compression
```

## Comparing `biobb_flexdyn-4.1.0.tar` & `biobb_flexdyn-4.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 11:27:35.329168 biobb_flexdyn-4.1.0/
--rw-r--r--   0 gbayarri (1147421021) 1791188573    11357 2023-03-31 13:41:20.000000 biobb_flexdyn-4.1.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1099 2023-09-07 11:27:35.328997 biobb_flexdyn-4.1.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5623 2023-09-07 11:26:39.000000 biobb_flexdyn-4.1.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 11:27:35.326983 biobb_flexdyn-4.1.0/biobb_flexdyn/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       67 2023-09-07 11:26:20.000000 biobb_flexdyn-4.1.0/biobb_flexdyn/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 11:27:35.328820 biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      128 2023-04-12 15:32:08.000000 biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15447 2023-05-26 08:00:28.000000 biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/concoord_disco.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11996 2023-04-12 15:32:08.000000 biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/concoord_dist.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8421 2023-05-31 08:34:22.000000 biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/imod_imc.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6938 2023-05-31 08:34:22.000000 biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/imod_imode.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7724 2023-05-31 08:34:22.000000 biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/imod_imove.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6927 2023-04-12 15:32:08.000000 biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/nolb_nma.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6114 2023-04-12 15:32:08.000000 biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/prody_anm.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 11:27:35.327758 biobb_flexdyn-4.1.0/biobb_flexdyn.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1099 2023-09-07 11:27:35.000000 biobb_flexdyn-4.1.0/biobb_flexdyn.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573      564 2023-09-07 11:27:35.000000 biobb_flexdyn-4.1.0/biobb_flexdyn.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-09-07 11:27:35.000000 biobb_flexdyn-4.1.0/biobb_flexdyn.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      379 2023-09-07 11:27:35.000000 biobb_flexdyn-4.1.0/biobb_flexdyn.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2023-09-07 11:27:35.000000 biobb_flexdyn-4.1.0/biobb_flexdyn.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       14 2023-09-07 11:27:35.000000 biobb_flexdyn-4.1.0/biobb_flexdyn.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-09-07 11:27:35.329220 biobb_flexdyn-4.1.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1958 2023-09-07 11:26:08.000000 biobb_flexdyn-4.1.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 09:52:47.366241 biobb_flexdyn-4.2.0/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    11357 2023-03-31 13:41:20.000000 biobb_flexdyn-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1134 2024-05-24 09:52:47.366021 biobb_flexdyn-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6162 2024-05-24 09:51:53.000000 biobb_flexdyn-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 09:52:47.363866 biobb_flexdyn-4.2.0/biobb_flexdyn/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       67 2024-05-24 09:51:35.000000 biobb_flexdyn-4.2.0/biobb_flexdyn/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 09:52:47.365745 biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      128 2023-04-12 15:32:08.000000 biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15447 2023-05-26 08:00:28.000000 biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/concoord_disco.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11996 2023-04-12 15:32:08.000000 biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/concoord_dist.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     8421 2023-05-31 08:34:22.000000 biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/imod_imc.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6938 2023-05-31 08:34:22.000000 biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/imod_imode.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     7724 2023-05-31 08:34:22.000000 biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/imod_imove.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6927 2023-04-12 15:32:08.000000 biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/nolb_nma.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6114 2023-04-12 15:32:08.000000 biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/prody_anm.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 09:52:47.364646 biobb_flexdyn-4.2.0/biobb_flexdyn.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1134 2024-05-24 09:52:47.000000 biobb_flexdyn-4.2.0/biobb_flexdyn.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      564 2024-05-24 09:52:47.000000 biobb_flexdyn-4.2.0/biobb_flexdyn.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2024-05-24 09:52:47.000000 biobb_flexdyn-4.2.0/biobb_flexdyn.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      379 2024-05-24 09:52:47.000000 biobb_flexdyn-4.2.0/biobb_flexdyn.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2024-05-24 09:52:47.000000 biobb_flexdyn-4.2.0/biobb_flexdyn.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       14 2024-05-24 09:52:47.000000 biobb_flexdyn-4.2.0/biobb_flexdyn.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2024-05-24 09:52:47.366286 biobb_flexdyn-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1958 2024-05-24 09:51:25.000000 biobb_flexdyn-4.2.0/setup.py
```

### Comparing `biobb_flexdyn-4.1.0/LICENSE` & `biobb_flexdyn-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.1.0/PKG-INFO` & `biobb_flexdyn-4.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: biobb_flexdyn
-Version: 4.1.0
+Version: 4.2.0
 Summary: biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.
 Home-page: https://github.com/bioexcel/biobb_flexdyn
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
-Project-URL: Documentation, http://biobb_flexdyn.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-flexdyn.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: 3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.2.0
 
 biobb_flexdyn allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.
```

### Comparing `biobb_flexdyn-4.1.0/README.md` & `biobb_flexdyn-4.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_flexdyn?label=Version)](https://GitHub.com/bioexcel/biobb_flexdyn/tags/)
 [![](https://img.shields.io/pypi/v/biobb-flexdyn.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-flexdyn/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_flexdyn?label=Conda)](https://anaconda.org/bioconda/biobb_flexdyn)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_flexdyn?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_flexdyn)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_flexdyn?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_flexdyn)
 [![](https://img.shields.io/pypi/pyversions/biobb-flexdyn.svg?label=Python%20Versions)](https://pypi.org/project/biobb-flexdyn/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_flexdyn)
 
 [![](https://readthedocs.org/projects/biobb-flexdyn/badge/?version=latest&label=Docs)](https://biobb-flexdyn.readthedocs.io/en/latest/?badge=latest)
@@ -18,84 +18,91 @@
 
 [![](https://docs.bioexcel.eu/biobb_flexdyn/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_flexdyn/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_flexdyn/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_flexdyn/coverage/)
 [![](https://docs.bioexcel.eu/biobb_flexdyn/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_flexdyn/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_flexdyn?label=Last%20Commit)](https://github.com/bioexcel/biobb_flexdyn/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_flexdyn.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_flexdyn/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_flexdyn
 
 ### Introduction
 biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.
 biobb_flexdyn allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility. It is based on the work done in the **flexdyn implementation study** from the **3D-Bioinfo ELIXIR structural community** (https://elixir-europe.org/communities/3d-bioinfo).
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_flexdyn.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-flexdyn.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_flexdyn>=4.1.0"
+        pip install "biobb_flexdyn>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-flexdyn.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_flexdyn>=4.1.0"
+        conda install -c bioconda "biobb_flexdyn>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-flexdyn.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-flexdyn.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_flexdyn:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_flexdyn:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_flexdyn:4.1.0--pyhdfd78af_0
+        docker run quay.io/biocontainers/biobb_flexdyn:4.2.0--pyhdfd78af_0
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_flexdyn.sif https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_flexdyn.sif https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_flexdyn.sif <command>
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-flexdyn.readthedocs.io/en/latest/command_line.html).
 
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

### Comparing `biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/concoord_disco.py` & `biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/concoord_disco.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/concoord_dist.py` & `biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/concoord_dist.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/imod_imc.py` & `biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/imod_imc.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/imod_imode.py` & `biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/imod_imode.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/imod_imove.py` & `biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/imod_imove.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/nolb_nma.py` & `biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/nolb_nma.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.1.0/biobb_flexdyn/flexdyn/prody_anm.py` & `biobb_flexdyn-4.2.0/biobb_flexdyn/flexdyn/prody_anm.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.1.0/biobb_flexdyn.egg-info/PKG-INFO` & `biobb_flexdyn-4.2.0/biobb_flexdyn.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: biobb-flexdyn
-Version: 4.1.0
+Version: 4.2.0
 Summary: biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.
 Home-page: https://github.com/bioexcel/biobb_flexdyn
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
-Project-URL: Documentation, http://biobb_flexdyn.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-flexdyn.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: 3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: biobb_common==4.2.0
 
 biobb_flexdyn allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.
```

### Comparing `biobb_flexdyn-4.1.0/biobb_flexdyn.egg-info/SOURCES.txt` & `biobb_flexdyn-4.2.0/biobb_flexdyn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.1.0/setup.py` & `biobb_flexdyn-4.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_flexdyn",
-    version="4.1.0",
+    version="4.2.0",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.",
     long_description="biobb_flexdyn allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.",
     long_description_content_type="text/markdown",
     keywords="3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure",
     url="https://github.com/bioexcel/biobb_flexdyn",
     project_urls={
-        "Documentation": "http://biobb_flexdyn.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-flexdyn.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
     include_package_data=True,
-    install_requires=['biobb_common==4.1.0'],
+    install_requires=['biobb_common==4.2.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "concoord_dist = biobb_flexdyn.flexdyn.concoord_dist:main",
             "concoord_disco = biobb_flexdyn.flexdyn.concoord_disco:main",
             "imod_imode = biobb_flexdyn.flexdyn.imod_imode:main",
             "imod_imove = biobb_flexdyn.flexdyn.imod_imove:main",
```

