# Comparing `tmp/biobb_analysis-4.1.0.tar.gz` & `tmp/biobb_analysis-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_analysis-4.1.0.tar", last modified: Thu Sep  7 07:54:40 2023, max compression
+gzip compressed data, was "biobb_analysis-4.2.0.tar", last modified: Fri May 24 06:51:17 2024, max compression
```

## Comparing `biobb_analysis-4.1.0.tar` & `biobb_analysis-4.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 07:54:40.221920 biobb_analysis-4.1.0/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:32:48.000000 biobb_analysis-4.1.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     6330 2023-09-07 07:54:40.221747 biobb_analysis-4.1.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5380 2023-09-07 07:53:18.000000 biobb_analysis-4.1.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 07:54:40.215671 biobb_analysis-4.1.0/biobb_analysis/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       82 2023-09-07 07:52:58.000000 biobb_analysis-4.1.0/biobb_analysis/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 07:54:40.218373 biobb_analysis-4.1.0/biobb_analysis/ambertools/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573      237 2023-04-12 10:13:13.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18276 2023-04-12 10:24:35.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13377 2023-04-12 11:15:00.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_average.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13184 2023-04-12 12:46:16.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_bfactor.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13291 2023-04-12 12:53:31.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_convert.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13387 2023-04-12 12:56:42.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_dry.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13403 2023-04-12 12:59:34.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_image.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5718 2023-04-12 13:01:18.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_input.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13387 2023-04-12 13:03:30.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_mask.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11475 2023-04-12 13:28:38.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_rgyr.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15009 2023-04-12 13:32:27.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_rms.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13109 2023-04-12 13:34:45.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_rmsf.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13179 2023-04-12 13:36:26.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_slice.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12946 2023-04-12 13:38:14.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_snapshot.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13411 2023-04-12 13:40:26.000000 biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_strip.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 07:54:40.221279 biobb_analysis-4.1.0/biobb_analysis/gromacs/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573      154 2023-04-12 10:13:19.000000 biobb_analysis-4.1.0/biobb_analysis/gromacs/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    19167 2023-04-12 13:42:07.000000 biobb_analysis-4.1.0/biobb_analysis/gromacs/common.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17757 2023-07-25 10:08:55.000000 biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_cluster.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9092 2023-04-12 13:51:32.000000 biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_energy.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    19456 2023-04-12 13:57:45.000000 biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_image.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11312 2023-04-12 14:00:12.000000 biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_rgyr.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11164 2023-04-12 14:07:47.000000 biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_rms.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12853 2023-04-12 14:23:24.000000 biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_trjconv_str.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    14293 2023-07-25 10:07:11.000000 biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_trjconv_str_ens.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13379 2023-04-12 14:24:04.000000 biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_trjconv_trj.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 07:54:40.221582 biobb_analysis-4.1.0/biobb_analysis/test/
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:32:48.000000 biobb_analysis-4.1.0/biobb_analysis/test/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-09-07 07:54:40.216428 biobb_analysis-4.1.0/biobb_analysis.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     6330 2023-09-07 07:54:40.000000 biobb_analysis-4.1.0/biobb_analysis.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1328 2023-09-07 07:54:40.000000 biobb_analysis-4.1.0/biobb_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-09-07 07:54:40.000000 biobb_analysis-4.1.0/biobb_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1198 2023-09-07 07:54:40.000000 biobb_analysis-4.1.0/biobb_analysis.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2023-09-07 07:54:40.000000 biobb_analysis-4.1.0/biobb_analysis.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       15 2023-09-07 07:54:40.000000 biobb_analysis-4.1.0/biobb_analysis.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-09-07 07:54:40.221965 biobb_analysis-4.1.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     2805 2023-09-07 07:52:43.000000 biobb_analysis-4.1.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 06:51:17.457915 biobb_analysis-4.2.0/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11358 2022-05-26 11:32:48.000000 biobb_analysis-4.2.0/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6904 2024-05-24 06:51:17.457662 biobb_analysis-4.2.0/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     5919 2024-05-24 06:49:38.000000 biobb_analysis-4.2.0/README.md
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 06:51:17.452987 biobb_analysis-4.2.0/biobb_analysis/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       82 2024-05-24 06:49:06.000000 biobb_analysis-4.2.0/biobb_analysis/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 06:51:17.455883 biobb_analysis-4.2.0/biobb_analysis/ambertools/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573      237 2023-04-12 10:13:13.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    18276 2023-04-12 10:24:35.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13377 2023-04-12 11:15:00.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_average.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13184 2023-04-12 12:46:16.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_bfactor.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13291 2023-04-12 12:53:31.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_convert.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13387 2023-04-12 12:56:42.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_dry.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13403 2023-04-12 12:59:34.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_image.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5718 2023-04-12 13:01:18.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_input.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13387 2023-04-12 13:03:30.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_mask.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11475 2023-04-12 13:28:38.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_rgyr.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15009 2023-04-12 13:32:27.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_rms.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13109 2023-04-12 13:34:45.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_rmsf.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13179 2023-04-12 13:36:26.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_slice.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12946 2023-04-12 13:38:14.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_snapshot.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13411 2023-04-12 13:40:26.000000 biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_strip.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 06:51:17.457278 biobb_analysis-4.2.0/biobb_analysis/gromacs/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573      154 2023-04-12 10:13:19.000000 biobb_analysis-4.2.0/biobb_analysis/gromacs/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    19167 2023-04-12 13:42:07.000000 biobb_analysis-4.2.0/biobb_analysis/gromacs/common.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    17757 2024-05-02 09:30:54.000000 biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_cluster.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573     9092 2023-04-12 13:51:32.000000 biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_energy.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    19456 2023-04-12 13:57:45.000000 biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_image.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11312 2023-04-12 14:00:12.000000 biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_rgyr.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11164 2023-04-12 14:07:47.000000 biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_rms.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    12853 2023-04-12 14:23:24.000000 biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_trjconv_str.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    14293 2023-07-25 10:07:11.000000 biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_trjconv_str_ens.py
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573    13379 2023-04-12 14:24:04.000000 biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_trjconv_trj.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 06:51:17.457406 biobb_analysis-4.2.0/biobb_analysis/test/
+-rwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2022-05-26 11:32:48.000000 biobb_analysis-4.2.0/biobb_analysis/test/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2024-05-24 06:51:17.453736 biobb_analysis-4.2.0/biobb_analysis.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     6904 2024-05-24 06:51:17.000000 biobb_analysis-4.2.0/biobb_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1328 2024-05-24 06:51:17.000000 biobb_analysis-4.2.0/biobb_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2024-05-24 06:51:17.000000 biobb_analysis-4.2.0/biobb_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     1198 2024-05-24 06:51:17.000000 biobb_analysis-4.2.0/biobb_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2024-05-24 06:51:17.000000 biobb_analysis-4.2.0/biobb_analysis.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       15 2024-05-24 06:51:17.000000 biobb_analysis-4.2.0/biobb_analysis.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2024-05-24 06:51:17.457961 biobb_analysis-4.2.0/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) 1791188573     2805 2024-05-24 06:48:53.000000 biobb_analysis-4.2.0/setup.py
```

### Comparing `biobb_analysis-4.1.0/LICENSE` & `biobb_analysis-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/PKG-INFO` & `biobb_analysis-4.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: biobb_analysis
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.
 Home-page: https://github.com/bioexcel/biobb_analysis
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
-Project-URL: Documentation, http://biobb_analysis.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-analysis.readthedocs.io/en/latest/
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
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_analysis?label=Version)](https://GitHub.com/bioexcel/biobb_analysis/tags/)
 [![](https://img.shields.io/pypi/v/biobb-analysis.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-analysis/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_analysis?label=Conda)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_analysis?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_analysis?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_analysis)
 [![](https://img.shields.io/pypi/pyversions/biobb-analysis.svg?label=Python%20Versions)](https://pypi.org/project/biobb-analysis/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_analysis)
 
 [![](https://readthedocs.org/projects/biobb-analysis/badge/?version=latest&label=Docs)](https://biobb-analysis.readthedocs.io/en/latest/?badge=latest)
@@ -40,86 +41,93 @@
 
 [![](https://docs.bioexcel.eu/biobb_analysis/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_analysis/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_analysis/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_analysis/coverage/)
 [![](https://docs.bioexcel.eu/biobb_analysis/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_analysis/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_analysis?label=Last%20Commit)](https://github.com/bioexcel/biobb_analysis/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_analysis.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_analysis/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 
 # biobb_analysis
 
 ### Introduction
 Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_analysis.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-analysis.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_analysis>=4.1.0"
+        pip install "biobb_analysis>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_analysis>=4.1.0"
+        conda install -c bioconda "biobb_analysis>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_analysis:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_analysis:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_analysis:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_analysis:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_analysis.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html).
 
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

### Comparing `biobb_analysis-4.1.0/README.md` & `biobb_analysis-4.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_analysis?label=Version)](https://GitHub.com/bioexcel/biobb_analysis/tags/)
 [![](https://img.shields.io/pypi/v/biobb-analysis.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-analysis/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_analysis?label=Conda)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_analysis?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_analysis?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_analysis)
 [![](https://img.shields.io/pypi/pyversions/biobb-analysis.svg?label=Python%20Versions)](https://pypi.org/project/biobb-analysis/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_analysis)
 
 [![](https://readthedocs.org/projects/biobb-analysis/badge/?version=latest&label=Docs)](https://biobb-analysis.readthedocs.io/en/latest/?badge=latest)
@@ -18,86 +18,93 @@
 
 [![](https://docs.bioexcel.eu/biobb_analysis/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_analysis/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_analysis/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_analysis/coverage/)
 [![](https://docs.bioexcel.eu/biobb_analysis/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_analysis/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_analysis?label=Last%20Commit)](https://github.com/bioexcel/biobb_analysis/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_analysis.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_analysis/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 
 # biobb_analysis
 
 ### Introduction
 Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_analysis.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-analysis.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_analysis>=4.1.0"
+        pip install "biobb_analysis>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_analysis>=4.1.0"
+        conda install -c bioconda "biobb_analysis>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_analysis:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_analysis:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_analysis:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_analysis:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_analysis.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html).
 
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

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/common.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/common.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_average.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_average.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_bfactor.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_bfactor.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_convert.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_convert.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_dry.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_dry.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_image.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_image.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_input.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_input.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_mask.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_mask.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_rgyr.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_rgyr.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_rms.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_rms.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_rmsf.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_rmsf.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_slice.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_slice.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_snapshot.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_snapshot.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/ambertools/cpptraj_strip.py` & `biobb_analysis-4.2.0/biobb_analysis/ambertools/cpptraj_strip.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/gromacs/common.py` & `biobb_analysis-4.2.0/biobb_analysis/gromacs/common.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_cluster.py` & `biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_cluster.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_energy.py` & `biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_energy.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_image.py` & `biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_image.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_rgyr.py` & `biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_rgyr.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_rms.py` & `biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_rms.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_trjconv_str.py` & `biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_trjconv_str.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_trjconv_str_ens.py` & `biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_trjconv_str_ens.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis/gromacs/gmx_trjconv_trj.py` & `biobb_analysis-4.2.0/biobb_analysis/gromacs/gmx_trjconv_trj.py`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis.egg-info/PKG-INFO` & `biobb_analysis-4.2.0/biobb_analysis.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: biobb-analysis
-Version: 4.1.0
+Version: 4.2.0
 Summary: Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.
 Home-page: https://github.com/bioexcel/biobb_analysis
 Author: Biobb developers
 Author-email: genis.bayarri@irbbarcelona.org
-Project-URL: Documentation, http://biobb_analysis.readthedocs.io/en/latest/
+Project-URL: Documentation, http://biobb-analysis.readthedocs.io/en/latest/
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
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_analysis?label=Version)](https://GitHub.com/bioexcel/biobb_analysis/tags/)
 [![](https://img.shields.io/pypi/v/biobb-analysis.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-analysis/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_analysis?label=Conda)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_analysis?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_analysis)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_analysis?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.1.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_analysis:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_analysis)
 [![](https://img.shields.io/pypi/pyversions/biobb-analysis.svg?label=Python%20Versions)](https://pypi.org/project/biobb-analysis/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_analysis)
 
 [![](https://readthedocs.org/projects/biobb-analysis/badge/?version=latest&label=Docs)](https://biobb-analysis.readthedocs.io/en/latest/?badge=latest)
@@ -40,86 +41,93 @@
 
 [![](https://docs.bioexcel.eu/biobb_analysis/junit/testsbadge.svg)](https://docs.bioexcel.eu/biobb_analysis/junit/report.html)
 [![](https://docs.bioexcel.eu/biobb_analysis/coverage/coveragebadge.svg)](https://docs.bioexcel.eu/biobb_analysis/coverage/)
 [![](https://docs.bioexcel.eu/biobb_analysis/flake8/flake8badge.svg)](https://docs.bioexcel.eu/biobb_analysis/flake8/)
 [![](https://img.shields.io/github/last-commit/bioexcel/biobb_analysis?label=Last%20Commit)](https://github.com/bioexcel/biobb_analysis/commits/master)
 [![](https://img.shields.io/github/issues/bioexcel/biobb_analysis.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_analysis/issues/)
 
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
+[![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
+
+[](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
+
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
+
 
 # biobb_analysis
 
 ### Introduction
 Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
-[latest API documentation](http://biobb_analysis.readthedocs.io/en/latest/).
+[latest API documentation](http://biobb-analysis.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.0 2023.3
+v4.2.0 2024.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_analysis>=4.1.0"
+        pip install "biobb_analysis>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_analysis>=4.1.0"
+        conda install -c bioconda "biobb_analysis>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-analysis.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_analysis:4.1.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_analysis:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_analysis:4.1.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_analysis:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.1.0--pyhdfd78af_0
+        singularity pull --name biobb_analysis.sif https://depot.galaxyproject.org/singularity/biobb_analysis:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_analysis.sif <command>
 
 
 The command list and specification can be found at the [Command Line documentation](https://biobb-analysis.readthedocs.io/en/latest/command_line.html).
 
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

### Comparing `biobb_analysis-4.1.0/biobb_analysis.egg-info/SOURCES.txt` & `biobb_analysis-4.2.0/biobb_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/biobb_analysis.egg-info/entry_points.txt` & `biobb_analysis-4.2.0/biobb_analysis.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_analysis-4.1.0/setup.py` & `biobb_analysis-4.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_analysis",
-    version="4.1.0",
+    version="4.2.0",
     author="Biobb developers",
     author_email="genis.bayarri@irbbarcelona.org",
     description="Biobb_analysis is the Biobb module collection to perform analysis of molecular dynamics simulations.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_analysis",
     project_urls={
-        "Documentation": "http://biobb_analysis.readthedocs.io/en/latest/",
+        "Documentation": "http://biobb-analysis.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==4.1.0'],
+    install_requires=['biobb_common==4.2.0'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "cpptraj_average = biobb_analysis.ambertools.cpptraj_average:main",
             "cpptraj_bfactor = biobb_analysis.ambertools.cpptraj_bfactor:main",
             "cpptraj_convert = biobb_analysis.ambertools.cpptraj_convert:main",
             "cpptraj_dry = biobb_analysis.ambertools.cpptraj_dry:main",
```

