# Comparing `tmp/biobb_godmd-4.1.0.tar.gz` & `tmp/biobb_godmd-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_godmd-4.1.0.tar", last modified: Thu Sep  7 13:37:56 2023, max compression
+gzip compressed data, was "biobb_godmd-4.2.0.tar", last modified: Fri May 24 10:32:55 2024, max compression
```

## Comparing `biobb_godmd-4.1.0.tar` & `biobb_godmd-4.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 13:37:56.526190 biobb_godmd-4.1.0/
--rw-r--r--   0 gbayarri (1147421021) 1791188573    11357 2023-04-11 11:37:10.000000 biobb_godmd-4.1.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1006 2023-09-07 13:37:56.526014 biobb_godmd-4.1.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5295 2023-09-07 13:37:10.000000 biobb_godmd-4.1.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 13:37:56.524491 biobb_godmd-4.1.0/biobb_godmd/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       63 2023-09-07 13:36:50.000000 biobb_godmd-4.1.0/biobb_godmd/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 13:37:56.525823 biobb_godmd-4.1.0/biobb_godmd/godmd/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       53 2023-04-11 11:37:10.000000 biobb_godmd-4.1.0/biobb_godmd/godmd/__init__.py
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2281 2023-07-27 10:53:24.000000 biobb_godmd-4.1.0/biobb_godmd/godmd/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16841 2023-07-31 11:32:52.000000 biobb_godmd-4.1.0/biobb_godmd/godmd/godmd_prep.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16003 2023-07-31 11:32:52.000000 biobb_godmd-4.1.0/biobb_godmd/godmd/godmd_run.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 13:37:56.525287 biobb_godmd-4.1.0/biobb_godmd.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1006 2023-09-07 13:37:56.000000 biobb_godmd-4.1.0/biobb_godmd.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573      383 2023-09-07 13:37:56.000000 biobb_godmd-4.1.0/biobb_godmd.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-09-07 13:37:56.000000 biobb_godmd-4.1.0/biobb_godmd.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      110 2023-09-07 13:37:56.000000 biobb_godmd-4.1.0/biobb_godmd.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2023-09-07 13:37:56.000000 biobb_godmd-4.1.0/biobb_godmd.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       12 2023-09-07 13:37:56.000000 biobb_godmd-4.1.0/biobb_godmd.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-09-07 13:37:56.526237 biobb_godmd-4.1.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1490 2023-09-07 13:36:32.000000 biobb_godmd-4.1.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 10:32:55.049298 biobb_godmd-4.2.0/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573    11357 2023-04-11 11:37:10.000000 biobb_godmd-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1041 2024-05-24 10:32:55.049043 biobb_godmd-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5834 2024-05-24 10:32:12.000000 biobb_godmd-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 10:32:55.047326 biobb_godmd-4.2.0/biobb_godmd/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       63 2024-05-24 10:31:59.000000 biobb_godmd-4.2.0/biobb_godmd/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 10:32:55.048747 biobb_godmd-4.2.0/biobb_godmd/godmd/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       53 2023-04-11 11:37:10.000000 biobb_godmd-4.2.0/biobb_godmd/godmd/__init__.py
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2281 2023-07-27 10:53:24.000000 biobb_godmd-4.2.0/biobb_godmd/godmd/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16841 2023-07-31 11:32:52.000000 biobb_godmd-4.2.0/biobb_godmd/godmd/godmd_prep.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    16003 2024-05-24 10:31:37.000000 biobb_godmd-4.2.0/biobb_godmd/godmd/godmd_run.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 10:32:55.048169 biobb_godmd-4.2.0/biobb_godmd.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1041 2024-05-24 10:32:55.000000 biobb_godmd-4.2.0/biobb_godmd.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      383 2024-05-24 10:32:55.000000 biobb_godmd-4.2.0/biobb_godmd.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2024-05-24 10:32:55.000000 biobb_godmd-4.2.0/biobb_godmd.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573      110 2024-05-24 10:32:55.000000 biobb_godmd-4.2.0/biobb_godmd.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2024-05-24 10:32:55.000000 biobb_godmd-4.2.0/biobb_godmd.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       12 2024-05-24 10:32:55.000000 biobb_godmd-4.2.0/biobb_godmd.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2024-05-24 10:32:55.049352 biobb_godmd-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1490 2024-05-24 10:31:51.000000 biobb_godmd-4.2.0/setup.py
```

### Comparing `biobb_godmd-4.1.0/LICENSE` & `biobb_godmd-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_godmd-4.1.0/PKG-INFO` & `biobb_godmd-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: biobb_godmd
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).
 Home-page: https://github.com/bioexcel/biobb_godmd
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
-Project-URL: Documentation, http://biobb_godmd.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-godmd.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD
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
 
 Biobb_godmd allows the calculation of protein conformational transitions using the GOdMD tool.
```

### Comparing `biobb_godmd-4.1.0/README.md` & `biobb_godmd-4.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_godmd?label=Version)](https://GitHub.com/bioexcel/biobb_godmd/tags/)
 [![](https://img.shields.io/pypi/v/biobb-godmd.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-godmd/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_godmd?label=Conda)](https://anaconda.org/bioconda/biobb_godmd)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_godmd?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_godmd)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_godmd?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_godmd:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_godmd:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_godmd)
 [![](https://img.shields.io/pypi/pyversions/biobb-godmd.svg?label=Python%20Versions)](https://pypi.org/project/biobb-godmd/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_godmd)
 
 [![](https://readthedocs.org/projects/biobb-godmd/badge/?version=latest&label=Docs)](https://biobb-godmd.readthedocs.io/en/latest/?badge=latest)
@@ -18,86 +18,93 @@
 
 [![](https://docs.bioexcel.eu/biobb_godmd/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_godmd/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_godmd/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_godmd/coverage/)
 [![](https://docs.bioexcel.eu/biobb_godmd/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_godmd/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_godmd?label=Last%20Commit)](https://github.com/bioexcel/biobb_godmd/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_godmd.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_godmd/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 # biobb_godmd
 
 ### Introduction
 biobb_godmd is a BioBB category for the GOdMD tool.
 biobb_godmd allows the calculation of protein conformational transitions using the GOdMD tool.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_godmd.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-godmd.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_godmd>=4.1.0"
+        pip install "biobb_godmd>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-godmd.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_godmd>=4.1.0"
+        conda install -c bioconda "biobb_godmd>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-godmd.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-godmd.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_godmd:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_godmd:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_godmd:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_godmd:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_godmd.sif https://depot.galaxyproject.org/singularity/biobb_godmd:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_godmd.sif https://depot.galaxyproject.org/singularity/biobb_godmd:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_godmd.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-godmd.readthedocs.io/en/latest/command_line.html).
 
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

### Comparing `biobb_godmd-4.1.0/biobb_godmd/godmd/common.py` & `biobb_godmd-4.2.0/biobb_godmd/godmd/common.py`

 * *Files identical despite different names*

### Comparing `biobb_godmd-4.1.0/biobb_godmd/godmd/godmd_prep.py` & `biobb_godmd-4.2.0/biobb_godmd/godmd/godmd_prep.py`

 * *Files identical despite different names*

### Comparing `biobb_godmd-4.1.0/biobb_godmd/godmd/godmd_run.py` & `biobb_godmd-4.2.0/biobb_godmd/godmd/godmd_run.py`

 * *Files identical despite different names*

### Comparing `biobb_godmd-4.1.0/biobb_godmd.egg-info/PKG-INFO` & `biobb_godmd-4.2.0/biobb_godmd.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: biobb-godmd
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).
 Home-page: https://github.com/bioexcel/biobb_godmd
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
-Project-URL: Documentation, http://biobb_godmd.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-godmd.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD
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
 
 Biobb_godmd allows the calculation of protein conformational transitions using the GOdMD tool.
```

### Comparing `biobb_godmd-4.1.0/setup.py` & `biobb_godmd-4.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_godmd",
-    version="4.1.0",
+    version="4.2.0",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="Biobb_godmd is a BioBB category for GOdMD tool (protein conformational transitions).",
     long_description="Biobb_godmd allows the calculation of protein conformational transitions using the GOdMD tool.",
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility Ensemble Protein Transitions GOdMD",
     url="https://github.com/bioexcel/biobb_godmd",
     project_urls={
-        "Documentation": "http://biobb_godmd.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-godmd.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==4.1.0'],
+    install_requires=['biobb_common==4.2.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "godmd_prep = biobb_godmd.godmd.godmd_prep:main",
             "godmd_run = biobb_godmd.godmd.godmd_run:main"
         ]
     },
```

