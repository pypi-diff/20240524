# Comparing `tmp/deepslice-1.2.tar.gz` & `tmp/deepslice-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepslice-1.2.tar", last modified: Fri May 24 15:36:32 2024, max compression
+gzip compressed data, was "deepslice-1.2.1.tar", last modified: Fri May 24 15:45:01 2024, max compression
```

## Comparing `deepslice-1.2.tar` & `deepslice-1.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.093908 deepslice-1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/coord_post_processing/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/angle_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/depth_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/coord_post_processing/plane_alignment_functions/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/coord_post_processing/spacing_and_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/metadata/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/metadata/metadata_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/metadata/volumes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/metadata/volumes/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.089908 deepslice-1.2/DeepSlice/metadata/weights/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/metadata/weights/placeholder.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.093908 deepslice-1.2/DeepSlice/neural_network/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/neural_network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/neural_network/network_architecture.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/neural_network/neural_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.093908 deepslice-1.2/DeepSlice/read_and_write/
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/read_and_write/QuickNII_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:36:25.000000 deepslice-1.2/DeepSlice/read_and_write/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:36:32.093908 deepslice-1.2/DeepSlice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-05-24 15:36:32.000000 deepslice-1.2/DeepSlice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-24 15:36:32.000000 deepslice-1.2/DeepSlice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:36:32.000000 deepslice-1.2/DeepSlice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-24 15:36:32.000000 deepslice-1.2/DeepSlice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 15:36:32.000000 deepslice-1.2/DeepSlice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-24 15:36:25.000000 deepslice-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-05-24 15:36:32.093908 deepslice-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-24 15:36:25.000000 deepslice-1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 15:36:32.093908 deepslice-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-24 15:36:25.000000 deepslice-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:45:01.104104 deepslice-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:45:01.104104 deepslice-1.2.1/DeepSlice/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:45:01.104104 deepslice-1.2.1/DeepSlice/coord_post_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/coord_post_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/coord_post_processing/angle_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/coord_post_processing/depth_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:45:01.104104 deepslice-1.2.1/DeepSlice/coord_post_processing/plane_alignment_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/coord_post_processing/plane_alignment_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11657 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/coord_post_processing/spacing_and_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9299 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:45:01.104104 deepslice-1.2.1/DeepSlice/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/metadata/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/metadata/metadata_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:45:01.104104 deepslice-1.2.1/DeepSlice/metadata/volumes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/metadata/volumes/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:45:01.104104 deepslice-1.2.1/DeepSlice/metadata/weights/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/metadata/weights/placeholder.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:45:01.104104 deepslice-1.2.1/DeepSlice/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/neural_network/network_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/neural_network/neural_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:45:01.104104 deepslice-1.2.1/DeepSlice/read_and_write/
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/read_and_write/QuickNII_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 15:44:56.000000 deepslice-1.2.1/DeepSlice/read_and_write/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:45:01.104104 deepslice-1.2.1/DeepSlice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-05-24 15:45:01.000000 deepslice-1.2.1/DeepSlice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-24 15:45:01.000000 deepslice-1.2.1/DeepSlice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:45:01.000000 deepslice-1.2.1/DeepSlice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-24 15:45:01.000000 deepslice-1.2.1/DeepSlice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 15:45:01.000000 deepslice-1.2.1/DeepSlice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-24 15:44:56.000000 deepslice-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-05-24 15:45:01.104104 deepslice-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-24 15:44:56.000000 deepslice-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 15:45:01.108104 deepslice-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-24 15:44:57.000000 deepslice-1.2.1/setup.py
```

### Comparing `deepslice-1.2/DeepSlice/coord_post_processing/angle_methods.py` & `deepslice-1.2.1/DeepSlice/coord_post_processing/angle_methods.py`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/DeepSlice/coord_post_processing/depth_estimation.py` & `deepslice-1.2.1/DeepSlice/coord_post_processing/depth_estimation.py`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py` & `deepslice-1.2.1/DeepSlice/coord_post_processing/plane_alignment_functions/plane_alignment.py`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/DeepSlice/coord_post_processing/spacing_and_indexing.py` & `deepslice-1.2.1/DeepSlice/coord_post_processing/spacing_and_indexing.py`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/DeepSlice/main.py` & `deepslice-1.2.1/DeepSlice/main.py`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/DeepSlice/metadata/config.json` & `deepslice-1.2.1/DeepSlice/metadata/config.json`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/DeepSlice/metadata/metadata_loader.py` & `deepslice-1.2.1/DeepSlice/metadata/metadata_loader.py`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/DeepSlice/neural_network/neural_network.py` & `deepslice-1.2.1/DeepSlice/neural_network/neural_network.py`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/DeepSlice/read_and_write/QuickNII_functions.py` & `deepslice-1.2.1/DeepSlice/read_and_write/QuickNII_functions.py`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/DeepSlice.egg-info/PKG-INFO` & `deepslice-1.2.1/DeepSlice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.2
+Version: 1.2.1
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.2.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.2.1.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

#### html2text {}

```diff
@@ -1,44 +1,45 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.2 Summary: A package to align
-histology to 3D brain atlases Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/
-1.2.tar.gz Author: DeepSlice Team Author-email: harry.carey@medisin.uio.no
-License: GPL-3.0 Keywords: histology,brain,atlas,alignment Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Science/Research Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: scikit-learn
-Requires-Dist: scikit-image Requires-Dist: tensorflow<=2.15.0 Requires-Dist:
-h5py Requires-Dist: typing Requires-Dist: pandas Requires-Dist: requests
-Requires-Dist: protobuf==3.20 Requires-Dist: lxml Requires-Dist:
-urllib3==1.26.6 [![DOI](https://zenodo.org/badge/274122364.svg)](https://
-zenodo.org/badge/latestdoi/274122364) ![Alt](docs/images/
-DeepSlice_github_banner.png "DeepSlice Banner") DeepSlice is a python library
-which automatically aligns mouse histology with the allen brain atlas common
-coordinate framework (and now rat brain histology to the Waxholm rat brain
-atlas, though this is in beta). The alignments are viewable, and refinable,
-using the [QuickNII](https://www.nitrc.org/projects/quicknii "QuickNII")
-software package. DeepSlice requires no preprocessing and works on any stain,
-however we have found it performs best on brightfield images. At present one
-limitation is that it only works on Coronally cut sections, we will release an
-update in the future for sagittal and horizontally cut histology. ![Alt](docs/
-images/process.PNG) DeepSlice automates the process of identifying exactly
-where in the brain a section lies, it can accomodate non-orthogonal cutting
-planes and will produce an image specific annotation for each section in your
-brain. ## Workflow DeepSlice is fully integrated with the _Q_U_I_N_T_ _w_o_r_k_f_l_o_w_. Quint
-helps you register, segment and quantify brain wide datasets!  
-ð­ð§ ð¬ð»ð¤ ## Web Application If you would like to use DeepSlice but
-don't need your own personal installation, check out [**DeepSlice Flask**]
-(https://www.DeepSlice.com.au), a fully functional web application which will
-allow you to upload your dataset and download the aligned results. The web
-interface was developed by [Michael Pegios](https://github.com/ThermoDev/). ##
-[Installation: How to install DeepSlice](#installation) ## [Usage: How to align
-using DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
-(examples/example_notebooks/DeepSlice_example.ipynb) **Happy Aligning :)**
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.2.1 Summary: A package to
+align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
+DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
+tags/1.2.1.tar.gz Author: DeepSlice Team Author-email:
+harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
+histology,brain,atlas,alignment Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
+Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
+Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
+Language :: Python Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: numpy Requires-Dist: scikit-learn Requires-Dist: scikit-
+image Requires-Dist: tensorflow<=2.15.0 Requires-Dist: h5py Requires-Dist:
+typing Requires-Dist: pandas Requires-Dist: requests Requires-Dist:
+protobuf==3.20 Requires-Dist: lxml Requires-Dist: urllib3==1.26.6 [![DOI]
+(https://zenodo.org/badge/274122364.svg)](https://zenodo.org/badge/latestdoi/
+274122364) ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
+DeepSlice is a python library which automatically aligns mouse histology with
+the allen brain atlas common coordinate framework (and now rat brain histology
+to the Waxholm rat brain atlas, though this is in beta). The alignments are
+viewable, and refinable, using the [QuickNII](https://www.nitrc.org/projects/
+quicknii "QuickNII") software package. DeepSlice requires no preprocessing and
+works on any stain, however we have found it performs best on brightfield
+images. At present one limitation is that it only works on Coronally cut
+sections, we will release an update in the future for sagittal and horizontally
+cut histology. ![Alt](docs/images/process.PNG) DeepSlice automates the process
+of identifying exactly where in the brain a section lies, it can accomodate
+non-orthogonal cutting planes and will produce an image specific annotation for
+each section in your brain. ## Workflow DeepSlice is fully integrated with the
+_Q_U_I_N_T_ _w_o_r_k_f_l_o_w_. Quint helps you register, segment and quantify brain wide
+datasets!   ð­ð§ ð¬ð»ð¤ ## Web Application If you would like to use
+DeepSlice but don't need your own personal installation, check out [**DeepSlice
+Flask**](https://www.DeepSlice.com.au), a fully functional web application
+which will allow you to upload your dataset and download the aligned results.
+The web interface was developed by [Michael Pegios](https://github.com/
+ThermoDev/). ## [Installation: How to install DeepSlice](#installation) ##
+[Usage: How to align using DeepSlice](#basic-usage) ## [For a jupyter notebook
+example check out](examples/example_notebooks/DeepSlice_example.ipynb) **Happy
+Aligning :)**
 ************ IInnssttaallllaattiioonn ************
 ********** FFrroomm PPIIPP **********
 This is the easy and recommended way to install DeepSlice, simply: ```bash pip
 install DeepSlice ``` And you're ready to go! ð Check out the PyPi package
 [here](https://pypi.org/project/DeepSlice/)
 ********** FFrroomm SSoouurrccee **********
 **First** In order to easily install all the dependancies we recommend using
```

### Comparing `deepslice-1.2/DeepSlice.egg-info/SOURCES.txt` & `deepslice-1.2.1/DeepSlice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/LICENSE` & `deepslice-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/PKG-INFO` & `deepslice-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DeepSlice
-Version: 1.2
+Version: 1.2.1
 Summary: A package to align histology to 3D brain atlases
 Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.2.tar.gz
+Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.2.1.tar.gz
 Author: DeepSlice Team
 Author-email: harry.carey@medisin.uio.no
 License: GPL-3.0
 Keywords: histology,brain,atlas,alignment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

#### html2text {}

```diff
@@ -1,44 +1,45 @@
-Metadata-Version: 2.1 Name: DeepSlice Version: 1.2 Summary: A package to align
-histology to 3D brain atlases Home-page: https://github.com/PolarBean/DeepSlice
-Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/tags/
-1.2.tar.gz Author: DeepSlice Team Author-email: harry.carey@medisin.uio.no
-License: GPL-3.0 Keywords: histology,brain,atlas,alignment Classifier:
-Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
-Science/Research Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: scikit-learn
-Requires-Dist: scikit-image Requires-Dist: tensorflow<=2.15.0 Requires-Dist:
-h5py Requires-Dist: typing Requires-Dist: pandas Requires-Dist: requests
-Requires-Dist: protobuf==3.20 Requires-Dist: lxml Requires-Dist:
-urllib3==1.26.6 [![DOI](https://zenodo.org/badge/274122364.svg)](https://
-zenodo.org/badge/latestdoi/274122364) ![Alt](docs/images/
-DeepSlice_github_banner.png "DeepSlice Banner") DeepSlice is a python library
-which automatically aligns mouse histology with the allen brain atlas common
-coordinate framework (and now rat brain histology to the Waxholm rat brain
-atlas, though this is in beta). The alignments are viewable, and refinable,
-using the [QuickNII](https://www.nitrc.org/projects/quicknii "QuickNII")
-software package. DeepSlice requires no preprocessing and works on any stain,
-however we have found it performs best on brightfield images. At present one
-limitation is that it only works on Coronally cut sections, we will release an
-update in the future for sagittal and horizontally cut histology. ![Alt](docs/
-images/process.PNG) DeepSlice automates the process of identifying exactly
-where in the brain a section lies, it can accomodate non-orthogonal cutting
-planes and will produce an image specific annotation for each section in your
-brain. ## Workflow DeepSlice is fully integrated with the _Q_U_I_N_T_ _w_o_r_k_f_l_o_w_. Quint
-helps you register, segment and quantify brain wide datasets!  
-ð­ð§ ð¬ð»ð¤ ## Web Application If you would like to use DeepSlice but
-don't need your own personal installation, check out [**DeepSlice Flask**]
-(https://www.DeepSlice.com.au), a fully functional web application which will
-allow you to upload your dataset and download the aligned results. The web
-interface was developed by [Michael Pegios](https://github.com/ThermoDev/). ##
-[Installation: How to install DeepSlice](#installation) ## [Usage: How to align
-using DeepSlice](#basic-usage) ## [For a jupyter notebook example check out]
-(examples/example_notebooks/DeepSlice_example.ipynb) **Happy Aligning :)**
+Metadata-Version: 2.1 Name: DeepSlice Version: 1.2.1 Summary: A package to
+align histology to 3D brain atlases Home-page: https://github.com/PolarBean/
+DeepSlice Download-URL: https://github.com/PolarBean/DeepSlice/archive/refs/
+tags/1.2.1.tar.gz Author: DeepSlice Team Author-email:
+harry.carey@medisin.uio.no License: GPL-3.0 Keywords:
+histology,brain,atlas,alignment Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Science/Research Classifier:
+Topic :: Scientific/Engineering :: Bio-Informatics Classifier: License :: OSI
+Approved :: GNU General Public License v3 (GPLv3) Classifier: Programming
+Language :: Python Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: numpy Requires-Dist: scikit-learn Requires-Dist: scikit-
+image Requires-Dist: tensorflow<=2.15.0 Requires-Dist: h5py Requires-Dist:
+typing Requires-Dist: pandas Requires-Dist: requests Requires-Dist:
+protobuf==3.20 Requires-Dist: lxml Requires-Dist: urllib3==1.26.6 [![DOI]
+(https://zenodo.org/badge/274122364.svg)](https://zenodo.org/badge/latestdoi/
+274122364) ![Alt](docs/images/DeepSlice_github_banner.png "DeepSlice Banner")
+DeepSlice is a python library which automatically aligns mouse histology with
+the allen brain atlas common coordinate framework (and now rat brain histology
+to the Waxholm rat brain atlas, though this is in beta). The alignments are
+viewable, and refinable, using the [QuickNII](https://www.nitrc.org/projects/
+quicknii "QuickNII") software package. DeepSlice requires no preprocessing and
+works on any stain, however we have found it performs best on brightfield
+images. At present one limitation is that it only works on Coronally cut
+sections, we will release an update in the future for sagittal and horizontally
+cut histology. ![Alt](docs/images/process.PNG) DeepSlice automates the process
+of identifying exactly where in the brain a section lies, it can accomodate
+non-orthogonal cutting planes and will produce an image specific annotation for
+each section in your brain. ## Workflow DeepSlice is fully integrated with the
+_Q_U_I_N_T_ _w_o_r_k_f_l_o_w_. Quint helps you register, segment and quantify brain wide
+datasets!   ð­ð§ ð¬ð»ð¤ ## Web Application If you would like to use
+DeepSlice but don't need your own personal installation, check out [**DeepSlice
+Flask**](https://www.DeepSlice.com.au), a fully functional web application
+which will allow you to upload your dataset and download the aligned results.
+The web interface was developed by [Michael Pegios](https://github.com/
+ThermoDev/). ## [Installation: How to install DeepSlice](#installation) ##
+[Usage: How to align using DeepSlice](#basic-usage) ## [For a jupyter notebook
+example check out](examples/example_notebooks/DeepSlice_example.ipynb) **Happy
+Aligning :)**
 ************ IInnssttaallllaattiioonn ************
 ********** FFrroomm PPIIPP **********
 This is the easy and recommended way to install DeepSlice, simply: ```bash pip
 install DeepSlice ``` And you're ready to go! ð Check out the PyPi package
 [here](https://pypi.org/project/DeepSlice/)
 ********** FFrroomm SSoouurrccee **********
 **First** In order to easily install all the dependancies we recommend using
```

### Comparing `deepslice-1.2/README.md` & `deepslice-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `deepslice-1.2/setup.py` & `deepslice-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='DeepSlice',
     packages=find_packages(),
-    version='1.2',
+    version='1.2.1',
     license='GPL-3.0',
     description='A package to align histology to 3D brain atlases',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='DeepSlice Team',
     package_data={'DeepSlice': ['metadata/volumes/placeholder.txt', 'metadata/config.json','metadata/weights/*.txt']},
     include_package_data=True,
     author_email='harry.carey@medisin.uio.no',
     url='https://github.com/PolarBean/DeepSlice',
-    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.2.tar.gz',
+    download_url='https://github.com/PolarBean/DeepSlice/archive/refs/tags/1.2.1.tar.gz',
     keywords=['histology', 'brain', 'atlas', 'alignment'],
     install_requires=[
         'numpy',
         'scikit-learn',
         'scikit-image',
         'tensorflow<=2.15.0',
         'h5py',
```

