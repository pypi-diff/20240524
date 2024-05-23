# Comparing `tmp/mcemtools-0.9.2.tar.gz` & `tmp/mcemtools-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.9.2.tar", last modified: Mon Mar 18 02:29:19 2024, max compression
+gzip compressed data, was "mcemtools-0.9.3.tar", last modified: Thu May 23 23:38:22 2024, max compression
```

## Comparing `mcemtools-0.9.2.tar` & `mcemtools-0.9.3.tar`

### file list

```diff
@@ -1,57 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 02:29:19.808037 mcemtools-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-18 02:29:15.000000 mcemtools-0.9.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-03-18 02:29:15.000000 mcemtools-0.9.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-18 02:29:15.000000 mcemtools-0.9.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-18 02:29:15.000000 mcemtools-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-18 02:29:15.000000 mcemtools-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-03-18 02:29:19.808037 mcemtools-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-18 02:29:15.000000 mcemtools-0.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 02:29:19.804037 mcemtools-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-18 02:29:15.000000 mcemtools-0.9.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 02:29:19.804037 mcemtools-0.9.2/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20967 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 02:29:19.808037 mcemtools-0.9.2/mcemtools/denoise/
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/denoise/DATOS.py
--rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/denoise/LossFunc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/denoise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31188 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/denoise/cluster4net.py
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/denoise/denoise4_tsvd.py
--rw-r--r--   0 runner    (1001) docker     (127)    36697 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/denoise/denoise4net.py
--rw-r--r--   0 runner    (1001) docker     (127)    28970 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/denoise/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/denoise/nn_from_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    14024 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    10847 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-03-18 02:29:15.000000 mcemtools-0.9.2/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 02:29:19.808037 mcemtools-0.9.2/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-03-18 02:29:19.000000 mcemtools-0.9.2/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-18 02:29:19.000000 mcemtools-0.9.2/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 02:29:19.000000 mcemtools-0.9.2/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-18 02:29:19.000000 mcemtools-0.9.2/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 02:29:19.000000 mcemtools-0.9.2/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-18 02:29:19.000000 mcemtools-0.9.2/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-18 02:29:19.000000 mcemtools-0.9.2/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-18 02:29:15.000000 mcemtools-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-18 02:29:19.808037 mcemtools-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-18 02:29:15.000000 mcemtools-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 02:29:19.808037 mcemtools-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-18 02:29:15.000000 mcemtools-0.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-18 02:29:15.000000 mcemtools-0.9.2/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-18 02:29:15.000000 mcemtools-0.9.2/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-18 02:29:15.000000 mcemtools-0.9.2/tests/test_mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-03-18 02:29:15.000000 mcemtools-0.9.2/tests/test_tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-18 02:29:15.000000 mcemtools-0.9.2/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.418176 mcemtools-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 23:38:18.000000 mcemtools-0.9.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-23 23:38:18.000000 mcemtools-0.9.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-23 23:38:18.000000 mcemtools-0.9.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-23 23:38:18.000000 mcemtools-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-23 23:38:18.000000 mcemtools-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-23 23:38:22.418176 mcemtools-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-23 23:38:18.000000 mcemtools-0.9.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.410176 mcemtools-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-23 23:38:18.000000 mcemtools-0.9.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.410176 mcemtools-0.9.3/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.414176 mcemtools-0.9.3/mcemtools/classifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/classifier/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/classifier/capsnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.414176 mcemtools-0.9.3/mcemtools/denoise/
+-rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/DATOS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13131 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/LossFunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31188 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/cluster4net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/denoise4_tsvd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35985 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/denoise4net.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28947 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/denoise/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15574 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12907 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-05-23 23:38:18.000000 mcemtools-0.9.3/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.414176 mcemtools-0.9.3/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 23:38:22.000000 mcemtools-0.9.3/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-23 23:38:18.000000 mcemtools-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-23 23:38:22.418176 mcemtools-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-23 23:38:18.000000 mcemtools-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:38:22.414176 mcemtools-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/test_mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/test_tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-23 23:38:18.000000 mcemtools-0.9.3/tests/test_transforms.py
```

### Comparing `mcemtools-0.9.2/CONTRIBUTING.rst` & `mcemtools-0.9.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/HISTORY.rst` & `mcemtools-0.9.3/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -103,8 +103,12 @@
 -------------------
 * added denoise4_tsvd
 * faster bin_4D
 * torch handler does not update the model if the loss is inf or nan
 
 0.9.2 (2024-03-23)
 -------------------
-* annular mask can handle even sized image
+* annular mask can handle even sized image
+
+0.9.2 (2024-05-02)
+-------------------
+* viewer_4D takes second mask to subtract
```

### Comparing `mcemtools-0.9.2/LICENSE` & `mcemtools-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/PKG-INFO` & `mcemtools-0.9.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.9.2
+Version: 0.9.3
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -38,23 +38,15 @@
 .. image:: https://img.shields.io/travis/arsadri/mcemtools.svg
         :target: https://travis-ci.com/arsadri/mcemtools
 
 .. image:: https://readthedocs.org/projects/mcemtools/badge/?version=latest
         :target: https://mcemtools.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
-
-.. image:: https://pyup.io/repos/github/arsadri/mcemtools/shield.svg
-     :target: https://pyup.io/repos/github/arsadri/mcemtools/
-     :alt: Updates
-
-
-
-State of the art aalysis for electron microscopy
-
+Deep unsupervised analysis tools for Four-dimensional Scanning Transmission Electron Microscopy (4D-STEM) 
 
 * Free software: MIT license
 * Documentation: https://mcemtools.readthedocs.io.
 
 
 Features
 --------
@@ -176,7 +168,11 @@
 * added denoise4_tsvd
 * faster bin_4D
 * torch handler does not update the model if the loss is inf or nan
 
 0.9.2 (2024-03-23)
 -------------------
 * annular mask can handle even sized image
+
+0.9.2 (2024-05-02)
+-------------------
+* viewer_4D takes second mask to subtract
```

### Comparing `mcemtools-0.9.2/README.rst` & `mcemtools-0.9.3/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -9,23 +9,15 @@
 .. image:: https://img.shields.io/travis/arsadri/mcemtools.svg
         :target: https://travis-ci.com/arsadri/mcemtools
 
 .. image:: https://readthedocs.org/projects/mcemtools/badge/?version=latest
         :target: https://mcemtools.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
-
-.. image:: https://pyup.io/repos/github/arsadri/mcemtools/shield.svg
-     :target: https://pyup.io/repos/github/arsadri/mcemtools/
-     :alt: Updates
-
-
-
-State of the art aalysis for electron microscopy
-
+Deep unsupervised analysis tools for Four-dimensional Scanning Transmission Electron Microscopy (4D-STEM) 
 
 * Free software: MIT license
 * Documentation: https://mcemtools.readthedocs.io.
 
 
 Features
 --------
```

### Comparing `mcemtools-0.9.2/docs/Makefile` & `mcemtools-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/docs/conf.py` & `mcemtools-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/docs/installation.rst` & `mcemtools-0.9.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/docs/make.bat` & `mcemtools-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/mcemtools/__init__.py` & `mcemtools-0.9.3/mcemtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for mcemtools."""
 
 __author__ = """Alireza Sadri"""
 __email__ = 'alireza.sadri@monash.edu'
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 
 from .mcemtools import viewer_4D
 
 from .analysis   import (cross_correlation_4D,
                        SymmSTEM,
                        centre_of_mass_4D,
                        sum_4D,
```

### Comparing `mcemtools-0.9.2/mcemtools/analysis.py` & `mcemtools-0.9.3/mcemtools/analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from .masking import annular_mask, mask2D_to_4D, image_by_windows
 from lognflow import printprogress, lognflow
 from skimage.transform import warp_polar
+from itertools import product
 
 def normalize_4D(data4D, weights4D = None, method = 'loop'):
     """
         Note::
             make sure you have set weights4D[data4D == 0] = 0 when dealing with
             Poisson.
     """
@@ -51,15 +52,15 @@
         rot = np.roll(rot, 1, axis=0)
     return corr
 
 def calc_symm(CBED, inputs_to_share: tuple):
     mask_ang, nang, mflag = inputs_to_share
     
     polar = warp_polar(CBED)
-    kvec = np.tile(np.array([np.arange(_polar.shape[0])]).swapaxes(0, 1),
+    kvec = np.tile(np.array([np.arange(polar.shape[0])]).swapaxes(0, 1),
                 (1, nang))/(nang/2/np.pi)
     polar[mask_ang == 0] = 0
     
     """
         perform angular autocorrelation or autoconvolutiuon using Fourier
         correlation theorems.
         note: one difference between the above symmetry measures is the
@@ -166,15 +167,15 @@
     """
     if weight4D is not None:
         assert weight4D.shape == data4D.shape,\
             'weight4D should have the same shape as data4D'
     
     I4D_cpy = data4D.copy()
     if weight4D is not None:
-        I4D_cpy *= weight4D
+        I4D_cpy = I4D_cpy * weight4D
     PACBED = I4D_cpy.sum(1).sum(0).squeeze()
     totI = I4D_cpy.sum(3).sum(2).squeeze()
     return totI, PACBED
 
 def conv_4D_single(grc, sharables):
     imgbywin, data4D = sharables
     return data4D[grc[0]:grc[0] + imgbywin.win_shape[0], 
@@ -224,41 +225,32 @@
     :param logger:
         should have a __call__, it is print by default.
     """
     assert factor == int(factor), f'Binning factor must be integer, it is {factor}'
     data_shape = data.shape
     n_x, n_y = data_shape[0], data_shape[1]
     if len(data_shape) > 2:
-        data_binned = np.zeros((int(n_x/factor), int(n_y/factor), *data_shape[2:]),
+        data_summed = np.zeros((n_x - factor + 1, n_y - factor + 1, *data_shape[2:]),
                                dtype = data.dtype)
     else:
-        data_binned = np.zeros((int(n_x/factor), int(n_y/factor)), 
+        data_summed = np.zeros((n_x - factor + 1, n_y - factor + 1), 
                                dtype = data.dtype)
-    inds_i, inds_j = np.where(np.ones((n_x, n_y)) > 0)
     logger(f'bin_image start for dataset of shape {data_shape}...')
-    logger('top left')
-    data_binned[
-        (inds_i[::factor]/factor).astype('int'), 
-        (inds_j[::factor]/factor).astype('int')] += \
-            data[inds_i[::factor], inds_j[::factor]]
-    logger('top right')
-    data_binned[
-        (inds_i[1::factor]/factor).astype('int'), 
-        (inds_j[::factor]/factor).astype('int')] += \
-            data[inds_i[1::factor], inds_j[::factor]]
-    logger('bot left')
-    data_binned[
-        (inds_i[::factor]/factor).astype('int'), 
-        (inds_j[1::factor]/factor).astype('int')] += \
-            data[inds_i[::factor], inds_j[1::factor]]
-    logger('bot right')
-    data_binned[
-        (inds_i[1::factor]/factor).astype('int'), 
-        (inds_j[1::factor]/factor).astype('int')] += \
-            data[inds_i[1::factor], inds_j[1::factor]]
+    
+    fh = int(factor/2)
+    
+    for indi, indj in product(list(range(factor)), list(range(factor))):
+        rend = -fh + indi
+        cend = -fh + indj
+        if rend == 0: rend = n_x
+        if cend == 0: cend = n_y
+        data_summed += data[fh - 1 + indi:rend, fh - 1 + indj:cend].copy()
+
+    data_binned = data_summed[::factor, ::factor]
+        
     logger(f'... bin_image done with shape {data_binned.shape}')
     return data_binned
 
 def bin_4D(data4D, 
            n_pos_in_bin: int = 1, n_pix_in_bin: int = 1,
            method_pos: str = 'skip', method_pix: str = 'linear',
            conv_function = sum_4D, skip = (1, 1), logger = print):
```

### Comparing `mcemtools-0.9.2/mcemtools/data.py` & `mcemtools-0.9.3/mcemtools/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,26 +193,27 @@
         self.noisy_mu = self.reconstruct2D(
             self.Y_label.sum(3).sum(2).sum(1).squeeze())
         self.noisy_PACBED = self.Y_label.sum(1).sum(0).squeeze()
         self.cropped_shape = (grid_x.shape[0], grid_y.shape[0], n_r, n_c)
         
         self.trainable_inds = np.arange(self.n_pts, dtype='int')
     
-    def update(self, inimg):
+    def update(self, inimg, update_label = True):
         for gpt_cnt in range(self.n_pts):
             a_tile = inimg[
                 self.xx[gpt_cnt] - self.len_side // 2 : 
                     self.xx[gpt_cnt] + self.len_side // 2 + 1,
                 self.yy[gpt_cnt] - self.len_side // 2 : 
                     self.yy[gpt_cnt] + self.len_side // 2 + 1].copy()
             a_tile = a_tile.reshape(
                 self.len_side*self.len_side, self.n_r, self.n_c)
             self.X_in[gpt_cnt] = a_tile[self.mask_range == 1].copy()
-            self.Y_label[gpt_cnt] = a_tile[self.mask_range == 0].copy()
-    
+            if update_label:
+                self.Y_label[gpt_cnt] = a_tile[self.mask_range == 0].copy()
+
     def reconstruct1D(self, out1D_viewed):
         n_pts = self.xx.shape[0]
         out1D_viewed = out1D_viewed.squeeze()
         output = np.zeros((self.inimg_shape[0],
                            self.inimg_shape[1], 2), dtype='float32')
         for gpt_cnt in range(n_pts):
             output[self.xx[gpt_cnt], self.yy[gpt_cnt]] = \
```

### Comparing `mcemtools-0.9.2/mcemtools/denoise/LossFunc.py` & `mcemtools-0.9.3/mcemtools/denoise/LossFunc.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
     def forward(self, y_out, x_in, inds):
         with torch.no_grad():
             n_images = x_in.shape[0]
             log_factorial_x_in = self.log_factorial[x_in.long()]
         
         err_p = x_in * torch.log(y_out + self.output_stabilizer
-                                 ) - y_out + log_factorial_x_in
+                                 ) - y_out - log_factorial_x_in
         err_p[:, :, self.mask_backprop == 0] = 0
         res_p = - err_p.sum() / self.mask_backprop_sum / n_images
         
         err_f = (x_in - y_out)**2 
         err_f[:, :, self.mask_backprop == 0] = 0
         res_f = (err_f.sum() / self.mask_backprop_sum / n_images)**0.5
         
@@ -325,14 +325,15 @@
 class mseLoss(nn.Module):
     def __init__(self):
         super(mseLoss, self).__init__()
 
     def forward(self, inputs, targets, inds = None):
         return (((targets - inputs)**2).mean())**0.5
 
+
 class justLoss(nn.Module):
     def __init__(self):
         super(justLoss, self).__init__()
 
     def forward(self, inputs, targets):
         return((targets - inputs).mean())
```

### Comparing `mcemtools-0.9.2/mcemtools/denoise/cluster4net.py` & `mcemtools-0.9.3/mcemtools/denoise/cluster4net.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/mcemtools/denoise/denoise4_tsvd.py` & `mcemtools-0.9.3/mcemtools/denoise/denoise4_tsvd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/mcemtools/denoise/denoise4net.py` & `mcemtools-0.9.3/mcemtools/denoise/denoise4net.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import scipy.ndimage
 import matplotlib.pyplot as plt
 from sklearn.cluster import KMeans
 from lognflow import lognflow, logviewer, printprogress, plt_colorbar
 
 import mcemtools
 
-from .DATOS         import DATOS
-from .nn_from_torch import nn_from_torch
+from .DATOS         import DATOS, nn_from_torch
+# from .nn_from_torch import nn_from_torch
 from .networks      import U_Net as network4D
 from .networks      import U_Net_fieldImage as network2D
 # from .networks_3 import DcUnet as network4D
 from .LossFunc      import mseLoss, STEM4D_PoissonLoss_FnormLoss 
 
 # torch.autograd.set_detect_anomaly(True)
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
@@ -308,22 +308,15 @@
         if(not log_exist_ok):
             logger = lognflow(logs_root)
         else:
             logger = lognflow(log_dir = pretrained_fpath_I4D.parent.parent)    
 
     logged_ref            = logviewer(ref_dir)
     data4D_noisy          = logged_ref.get_single('noisy.npy')
-    data4D_noisy_diffused = logged_ref.get_single('data4D_noisy_diffused.npy')
     data4D_nonoise        = logged_ref.get_single('nonoise.npy')
-    if data4D_noisy_diffused is None:
-        data4D_noisy_diffused = data4D_noisy
-        
-    if(True):
-        data4D_noisy = data4D_noisy_diffused.copy()
-    
     if use_pre_denoised_STEM:
         denoised_STEM  = logged_ref.get_single('denoised_STEM.npy')
         assert denoised_STEM is not None, 'set use_pre_denoised_STEM = False'
     
     data4D_shape = data4D_noisy.shape
     n_x, n_y, n_r, n_c = data4D_shape
     
@@ -338,14 +331,16 @@
     
     mch = mcemtools.data4D_to_frame(data4D_noisy[
             hyps_I4D['n_prob']//2:n_canvas_patterns - hyps_I4D['n_prob']//2,
             hyps_I4D['n_prob']//2:n_canvas_patterns - hyps_I4D['n_prob']//2])
     im = plt.imshow(mch); plt_colorbar(im)
     print(logger.log_plt('I4D_denoiser/canvas_noisy/noisy', dpi = 4000))        
 
+    logger.log_single('n_kernels', np.array([hyps_I4D['n_kernels']]))
+
     logger(f'hyps_STEM:')
     logger(hyps_STEM)
     logger(f'hyps_I4D:')
     logger(hyps_I4D)
     logger(f'Orginal data4D shape: {data4D_shape}')
     noisy_STEM, noisy_PACBED = mcemtools.sum_4D(data4D_noisy)
     logger(f'noisy_STEM.shape: {noisy_STEM.shape}')
@@ -421,46 +416,51 @@
                     nn_from_torch(
                         data_generator = data_gen_STEM,
                         torchModel = torchModel_STEM,
                         lossFunc = criterion_STEM,
                         device = device,
                         logger = logger,
                         learning_rate = hyps_STEM['learning_rate'],
-                        momentum = hyps_STEM['momentum'],
+                        momentum = hyps_STEM['learning_momentum'],
                         pass_indices_to_model = False) 
                 
                 _, denoised_STEM = infer_STEM(torch_handler_STEM,  data_gen_STEM, 
                                               logger,hyps_STEM['infer_size_STEM'])
                 torchModel_STEM.Ne_output = Ne_estimated/denoised_STEM.mean()
                 if(FLAG_train_STEM):
-                    DATOS_sampler_STEM = DATOS(trainable_inds.shape[0], 
-                                             n_segments = hyps_STEM['n_segments'],
-                                             mbatch_size = hyps_STEM['mbatch_size'],
-                                             n_epochs = hyps_STEM['n_epochs'])
-                    model_path = train_STEM(hyps_STEM['n_kSweeps'], 
-                                          torch_handler_STEM, 
-                                          data_gen_STEM,
-                                          logger, 
-                                          DATOS_sampler_STEM,
-                                          trainable_inds,
-                                          hyps_STEM['infer_size_STEM'],
-                                          hyps_STEM['mask_rate'])
+                    DATOS_sampler_STEM = DATOS(
+                        trainable_inds.shape[0], 
+                        n_segments = hyps_STEM['n_segments'],
+                        mbatch_size = hyps_STEM['mbatch_size'],
+                        n_epochs = hyps_STEM['n_epochs'])
+                    model_path = train_STEM(
+                        hyps_STEM['n_kSweeps'], 
+                        torch_handler_STEM, 
+                        data_gen_STEM,
+                        logger, 
+                        DATOS_sampler_STEM,
+                        trainable_inds,
+                        hyps_STEM['infer_size_STEM'],
+                        hyps_STEM['mask_rate'])
                     logger(f'Training STEM image denoising is finished.')
                     logger(f'Model is at: {model_path.absolute()}')
         
                 _, denoised_STEM = infer_STEM(torch_handler_STEM, 
                                           data_gen_STEM, logger, 
                                           hyps_STEM['infer_size_STEM'])
-                logger.log_single('STEM_denoiser/denoised_STEM.npy', denoised_STEM)
-                logger.log_imshow('STEM_denoiser/denoised_STEM.jpg', denoised_STEM)
+                logger.log_single('STEM_denoiser/denoised_STEM.npy', 
+                                  denoised_STEM)
+                logger.log_imshow('STEM_denoiser/denoised_STEM.jpg',
+                                  denoised_STEM)
                 denoised_STEM_mean = denoised_STEM.mean()
                 if ( (denoised_STEM_mean < Ne_estimated / 2) |
                      (denoised_STEM_mean > Ne_estimated * 2) ):
                     logger('The STEM denoiser was unsuccessful'
-                           f'The estimated Ne was {Ne_estimated}, but the STEM denoiser '
+                           f'The estimated Ne was {Ne_estimated},'
+                           f' but the STEM denoiser '
                            f'came up with {denoised_STEM_mean}')
                     raise ValueError
             elif STEM_denoiser_model_type == 'TSVD':
                 denoised_STEM = mcemtools.tensor_svd.tensor_svd_denoise(
                     data4D_noisy, rank = (
                         rank_info.n_x, rank_info.n_y, rank_info.n_pix))
                 denoised_STEM = denoised_STEM.reshape(*data4D_noisy_shape)
@@ -518,19 +518,21 @@
         logger('Making a training dataset using noisy')
         data_gen_I4D = mcemtools.data_maker_4D(
             data4D_noisy_new, data4D_nonoise, len_side = hyps_I4D['n_prob'],
             trainable_area_I4D = trainable_area_I4D)
     elif(False):
         logger('Making a diffused input dataset')
         data_gen_I4D_diffused = mcemtools.data_maker_4D(
-            data4D_noisy_diffused, data4D_nonoise, len_side = hyps_I4D['n_prob'],
+            data4D_noisy_diffused, data4D_nonoise, 
+            len_side = hyps_I4D['n_prob'],
             trainable_area_I4D = trainable_area_I4D)
         logger('Generating original noisy dataset')
         data_gen_I4D_X_in = data_gen_I4D_diffused.X_in.copy()
-        pvalue = data_gen_I4D_diffused.reconstruct4D(data_gen_I4D_diffused.Y_label)
+        pvalue = data_gen_I4D_diffused.reconstruct4D(
+            data_gen_I4D_diffused.Y_label)
         pvalue = pvalue[hyps_I4D['n_prob']//2:5+hyps_I4D['n_prob']//2,
                         hyps_I4D['n_prob']//2:5+hyps_I4D['n_prob']//2
                         ].reshape(25, n_r, n_c)
         logger.log_imshow_by_subplots(
             'I4D_denoiser/sample_100/data4D_noisy_diffused', pvalue)
         
         del data_gen_I4D_diffused
@@ -628,53 +630,70 @@
     noisy_PACBED_loss = noisy_PACBED_in / data_gen_I4D.n_pts
     noisy_STEM_loss = noisy_STEM_in / PACBED_mask.sum()
     criterion_I4D = STEM4D_PoissonLoss_FnormLoss(
         mask_backprop = torch.from_numpy(PACBED_mask).float().to(device),
         x_in_max = 1000, device = 'cuda',
         output_stabilizer = 1e-6,
         noisy_PACBED = torch.from_numpy(noisy_PACBED_loss).float().to(device),
-        noisy_mSTEM = torch.from_numpy(noisy_STEM_loss.ravel()).float().to(device),
+        noisy_mSTEM = torch.from_numpy(
+            noisy_STEM_loss.ravel()).float().to(device),
         PAC_loss_factor = hyps_I4D['PAC_loss_factor'],
         mSTEM_loss_factor = hyps_I4D['mSTME_loss_factor'],
         )
 
     torch_handler_I4D = nn_from_torch(
         data_generator = data_gen_I4D,
         torchModel = torchModel_I4D,
         lossFunc = criterion_I4D,
         device = device,
         logger = logger,
         learning_rate = 1e-7,
-        momentum = hyps_I4D['momentum'],
+        momentum = 1e-8,
         pass_indices_to_model = True,
         fix_during_infer = True) 
     
     perv_loss = np.nan
     Elapsed_time = 0
-    for refine_step in range(1, 20):
-        for kcnt in range(hyps_I4D['n_ksweeps']):
-            ETA_base = Elapsed_time * (hyps_I4D['n_ksweeps'] - kcnt)
-            # init_I4D(None, noisy_PACBED_in,
-            #         logger, data_gen_I4D, torch_handler_I4D, hyps_I4D['infer_size_I4D'])
+
+    n_refine_steps = hyps_I4D['n_refine_steps']
+
+    refine_step_list = np.arange(1, n_refine_steps)
+    for refine_step in refine_step_list:
+
+        if refine_step > 1:
+            torch_handler_I4D.update_learning_rate(hyps_I4D['learning_rate'])
+            torch_handler_I4D.update_momentum(hyps_I4D['learning_momentum'])
+
+        n_ksweeps = hyps_I4D['n_ksweeps']
+        if refine_step == n_refine_steps - 1:
+            n_ksweeps = hyps_I4D['n_ksweeps_last']
+
+        for kcnt in range(n_ksweeps):
+            ETA_base = Elapsed_time * ((n_ksweeps - kcnt) + 
+                              n_ksweeps * (len(refine_step_list) - refine_step))
+
             if refine_step == 1:
                 if kcnt == 0:
                     n_epochs = 1
                 else:
-                    torch_handler_I4D.update_learning_rate(hyps_I4D['learning_rate'])
+                    torch_handler_I4D.update_learning_rate(
+                        hyps_I4D['learning_rate'])
+                    torch_handler_I4D.update_momentum(
+                        hyps_I4D['learning_momentum'])
                     n_epochs = hyps_I4D['n_epochs']
         
-                if kcnt < 2:#hyps_I4D['n_ksweeps'] / 2:
+                if kcnt < 2:
                     init_I4D(noisy_STEM_in, None,
                              logger, data_gen_I4D, torch_handler_I4D, 
                              hyps_I4D['infer_size_I4D'])
-        
+
                 if(not FLAG_train_I4D):
-                    kcnt = hyps_I4D['n_ksweeps']
+                    kcnt = n_ksweeps
                 
-                criterion_I4D.LAGMUL = criterion_I4D_LAGMUL(kcnt, hyps_I4D['n_ksweeps'])
+                criterion_I4D.LAGMUL = criterion_I4D_LAGMUL(kcnt, n_ksweeps)
             logger(f'criterion_I4D.LAGMUL: {criterion_I4D.LAGMUL}')
             if(FLAG_train_I4D):
                 DATOS_sampler_I4D = DATOS(
                     trainable_inds.shape[0], 
                     classes = classes,
                     n_segments = hyps_I4D['n_segments'],
                     mbatch_size = hyps_I4D['mbatch_size'],
@@ -705,84 +724,73 @@
                 hyps_I4D['n_prob']//2:hyps_I4D['n_prob']//2 + 5, 
                 hyps_I4D['n_prob']//2:hyps_I4D['n_prob']//2 + 5
                     ].reshape(25, n_r, n_c)
             logger.log_imshow_by_subplots(
                 'I4D_denoiser/samples/data4D_denoised', 
                 pvalue)
             
-            ####################################################################
             data4D_noisy_new[hyps_I4D['n_prob']//2 : -(hyps_I4D['n_prob']//2),
                              hyps_I4D['n_prob']//2 : -(hyps_I4D['n_prob']//2)] \
                 = data4D_denoised.copy().astype('float32')
-            # if(log_denoised_every_sweep):
-            #     logger.log_single('I4D_denoiser/I4D_denoised_inter/denoised', 
-            #                       data4D_noisy_new)
-            
-            # ratio = 1 / hyps_I4D['n_ksweeps']
-            # data4D_noisy_new[hyps_I4D['n_prob']//2 : -(hyps_I4D['n_prob']//2),
-            #                  hyps_I4D['n_prob']//2 : -(hyps_I4D['n_prob']//2)] \
-            #     *=(1 - ratio)
-            # data4D_noisy_new[hyps_I4D['n_prob']//2 : -(hyps_I4D['n_prob']//2),
-            #                  hyps_I4D['n_prob']//2 : -(hyps_I4D['n_prob']//2)] \
-            #     += ratio * np.random.poisson(data4D_denoised).astype('float32')
-            ####################################################################
             
             noisy_STEM, noisy_PACBED  = mcemtools.sum_4D(data4D_noisy_new)
             Ne_estimated = noisy_STEM.mean()
             logger(f'estimated Ne per probe position: {Ne_estimated}')
             logger.log_imshow(
                 'I4D_denoiser/I4D_denoised_STEM/final_STEM_noisy', 
                 noisy_STEM[hyps_I4D['n_prob']//2:-hyps_I4D['n_prob']//2,
                         hyps_I4D['n_prob']//2:-hyps_I4D['n_prob']//2])
             logger.log_imshow(
-                'I4D_denoiser/I4D_denoised_PACBED/final_noisy_PACBED',  noisy_PACBED)
+                'I4D_denoiser/I4D_denoised_PACBED/final_noisy_PACBED',
+                noisy_PACBED)
             
             mch = mcemtools.data4D_to_frame(data4D_noisy_new[
                 hyps_I4D['n_prob']//2:n_canvas_patterns - hyps_I4D['n_prob']//2,
                 hyps_I4D['n_prob']//2:n_canvas_patterns - hyps_I4D['n_prob']//2])
             im = plt.imshow(mch); plt_colorbar(im)
             print(logger.log_plt('I4D_denoiser/canvas_denoised/denoised', 
                                  dpi = 4000))
             
             if not FLAG_train_I4D:
                 break
         
         logger('Making a diffused input dataset')
-        data4D_noisy_diffused = data4D_noisy.copy() * (
-                1 - refine_step/20) + data4D_noisy_new * refine_step/20
-        data_gen_I4D_diffused = mcemtools.data_maker_4D(
-            data4D_noisy_diffused, data4D_nonoise, len_side = hyps_I4D['n_prob'],
-            trainable_area_I4D = trainable_area_I4D)
-        logger('Generating original noisy dataset')
-        data_gen_I4D_X_in = data_gen_I4D_diffused.X_in.copy()
-        data_gen_I4D_Y_label = data_gen_I4D_diffused.Y_label.copy()
-        pvalue = data_gen_I4D_diffused.reconstruct4D(data_gen_I4D_diffused.Y_label)
+        beta = refine_step/(len(refine_step_list) + 1)
+        logger(f'The combination weight is: {beta}')
+        
+        data4D_noisy_diffused = \
+            data4D_noisy * (1 - beta) + data4D_noisy_new * beta
+        data4D_noisy_diffused = data4D_noisy_diffused.astype('float32')
+        logger('labels are diffused too.')
+        data_gen_I4D.update(data4D_noisy_diffused)
+        
+        pvalue = data_gen_I4D.reconstruct4D(data_gen_I4D.Y_label)
         pvalue = pvalue[hyps_I4D['n_prob']//2:5+hyps_I4D['n_prob']//2,
                         hyps_I4D['n_prob']//2:5+hyps_I4D['n_prob']//2
                         ].reshape(25, n_r, n_c)
         logger.log_imshow_by_subplots(
             'I4D_denoiser/sample_100/data4D_noisy_diffused', pvalue)
-        del data_gen_I4D_diffused
-        logger('Making a training dataset using noisy')
-        data_gen_I4D.X_in = data_gen_I4D_X_in.copy()
-        data_gen_I4D.Y_label = data_gen_I4D_Y_label.copy()
-        del data_gen_I4D_X_in, data_gen_I4D_Y_label
+        del data4D_noisy_diffused
         logger('training dataset is modified with diffused input')
         if(log_denoised_every_sweep):
-            logger.log_single('I4D_denoiser/I4D_denoised_inter/denoised', 
-                data4D_noisy_new)
-        
+            logger.log_single(
+                'I4D_denoiser/I4D_denoised_inter/denoised', data4D_noisy_new)
+            
+        hyps_I4D['learning_rate'] *= hyps_I4D['learning_rate_decay']
+        hyps_I4D['learning_momentum'] *= hyps_I4D['learning_momentum_decay']
+    
     logger.log_single('I4D_denoiser/I4D_denoised/denoised', data4D_noisy_new)
     
     frame_denoised = mcemtools.data4D_to_frame(data4D_noisy_new)
     frame_nonoise = mcemtools.data4D_to_frame(data4D_nonoise)
     frame_noisy = mcemtools.data4D_to_frame(data4D_noisy)
     logger.log_single('I4D_denoiser/canvases/denoised', frame_denoised)
     logger.log_single('I4D_denoiser/canvases/nonoise', frame_nonoise)
     logger.log_single('I4D_denoiser/canvases/noisy', frame_noisy)
     
-    logger('--\|/'*16)
     logger_dir = logger.log_dir
-    
+    logger(f'Check in: {logger_dir}')
+    logger('__`T*'*16)
+        
     del logger
     
-    return logger_dir
+    return logger_dir
```

### Comparing `mcemtools-0.9.2/mcemtools/denoise/networks.py` & `mcemtools-0.9.3/mcemtools/denoise/networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -601,15 +601,15 @@
                  num_classes = 1,
                  mid_channels = 32):
         super(ResNet18, self).__init__()
         self.mid_channels = mid_channels
         
         self.conv1 = nn.Conv2d(
             image_channels, self.mid_channels, kernel_size=3, stride=1)
-        #self.bn = nn.BatchNorm2d(self.mid_channels)
+        self.bn = nn.BatchNorm2d(self.mid_channels)
         self.relu = nn.ReLU()
         self.maxpool = nn.MaxPool2d(kernel_size = 3, stride = 2, padding = 1)
         
         #ResNet18 layers
         self.layer1 = self._make_layer(
             layers[0], layer_out_channels = 1*self.mid_channels, stride=1) 
         self.layer2 = self._make_layer(
@@ -628,15 +628,15 @@
         for i in range(num_residual_blocks - 1 ):
             layers.append(ResNetBlock(self.mid_channels, 
                                       layer_out_channels, stride=stride))
         return nn.Sequential(*layers)
     
     def forward(self, x):
         x = self.conv1(x)
-        #x = self.bn(x) ##############################################################
+        x = self.bn(x)
         x = self.relu(x)
         x = self.maxpool(x)
         x = self.layer1(x) 
         x = self.layer2(x) 
         x = self.layer3(x) 
         x = self.avgpool(x)
         x = x.reshape(x.shape[0], -1)
@@ -847,14 +847,15 @@
         x8 = 0*x7[:, :1, :, :]
         x8[:, 0] = x7.mean(1)
         if(self.mask is not None):
             x8[:, :, self.mask[9:-9, 9:-9]==0] = 0
         return(x8)
 
 def test_denoise4DSTEM_resNet():
+    torch.cuda.empty_cache()
     denoiser_model = denoise4DSTEM_resNet().to('cuda')
-    x = torch.randn(2, 1, 7*128, 7*128).to('cuda')
-    y = denoiser_model(x)
-    print(f'{x.shape} --> NN --> {y.shape} ')
+    x = torch.randn(7000, 1, 1024, 1024).float().to('cuda')
+    # y = denoiser_model(x)
+    # print(f'{x.shape} --> NN --> {y.shape} ')
     
 if __name__ == '__main__':
     test_denoise4DSTEM_resNet()
```

### Comparing `mcemtools-0.9.2/mcemtools/masking.py` & `mcemtools-0.9.3/mcemtools/masking.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """
     n_r, n_c = image_shape
     if centre is None: # use the middle of the image
         # centre = (int(n_r/2), int(n_c/2))
         centre = (n_r/2, n_c/2)
     if radius is None: 
         # use the smallest distance between the centre and image walls
-        radius = np.minimum(centre[0], centre[1])
+        radius = np.inf
 
     Y, X = np.ogrid[:n_r, :n_c]
     
     if n_r/2 == n_r//2:
         Y = Y + 0.49
     if n_c/2 == n_c//2:
         X = X + 0.49
@@ -58,14 +58,52 @@
     mask = dist_from_centre <= radius
     
     if(in_radius is not None):
         mask *= in_radius <= dist_from_centre
 
     return mask.astype('uint8') 
 
+def crop_or_pad(data, new_shape, padding_value = 0):
+    """shape data to have the new shape new_shape
+    Parameters
+    ----------
+        :param data
+        :param new_shape
+        :param padding_value
+            the padded areas fill value
+    Returns
+    -------
+        : np.ndarray of type data.dtype of shape new_shape
+            If a dimension of new_shape is smaller than a, a will be cut, 
+            if bigger, a will be put in the middle of padded zeros.
+    """
+    data_shape = data.shape
+    
+    assert len(data_shape) == len(new_shape), \
+        'put np.ndarray a in b, the length of their shapes should be the same.'
+    
+    for dim in range(len(data_shape)):
+        if data_shape[dim] != new_shape[dim]:
+            data = data.swapaxes(0, dim)
+            start = int((data_shape[dim] - new_shape[dim])/2)
+            finish = int((data_shape[dim] + new_shape[dim])/2)
+            pad_left = -int((data_shape[dim] - new_shape[dim])/2)
+            pad_right = int(np.ceil((new_shape[dim] - data_shape[dim])/2))
+            if data_shape[dim] > new_shape[dim]:
+                data = data[start : finish]
+            elif data_shape[dim] < new_shape[dim]:
+                data = np.vstack(
+                    (padding_value + np.zeros(((pad_left, ) + data.shape[1:]),
+                                      dtype=data.dtype),
+                     data,
+                     padding_value + np.zeros(((pad_right, ) + data.shape[1:]),
+                                      dtype=data.dtype)))
+            data = data.swapaxes(0, dim)
+    return data
+
 class image_by_windows:
     def __init__(self, 
                  img_shape: tuple[int, int], 
                  win_shape: tuple[int, int],
                  skip: tuple[int, int] = (1, 1),
                  method = 'linear'):
         """image by windows
```

### Comparing `mcemtools-0.9.2/mcemtools/mcemtools.py` & `mcemtools-0.9.3/mcemtools/mcemtools.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,52 +24,59 @@
         self.statistics_4D = statistics_4D
         self.logger = logger
         self.sleep_between_moves = sleep_between_moves
         self.min_shape_edge_width = min_shape_edge_width
         
         self.data4D_shape = self.data4D.shape
         self.data4D_shape_list = np.array(self.data4D_shape)
-        self.viewers_list = [napari.Viewer(title = title + '_STEM'), 
-                             napari.Viewer(title = title + '_PACBED')]
+        self.viewers_list = [napari.Viewer(title = title + '_PACBED'), 
+                             napari.Viewer(title = title + '_STEM')]
         STEM_img, PACBED = self.statistics_4D(self.data4D)
         self.viewers_list[0].add_image(PACBED)
         self.viewers_list[1].add_image(STEM_img)
         
         for viewer in self.viewers_list:
             viewer.bind_key(key = 'Up'   , func = self.move_up)
             viewer.bind_key(key = 'Down' , func = self.move_down)
             viewer.bind_key(key = 'Left' , func = self.move_left)
             viewer.bind_key(key = 'Right', func = self.move_right)
             viewer.bind_key(key = 'i'    , func = self.print_shape_info)
             viewer.bind_key(key = 'm'    , func = self.show_mask)
-            viewer.bind_key(key = 'f'    , func = self.show_frame4D)
             viewer.bind_key(key = 'F5'   , func = self.update_by_masked_sum_4D)
+
+        self.viewers_list[1].bind_key(key = 'g', func = self.show_frame4D)
         
         self.viewers_list[0].mouse_drag_callbacks.append(self.mouse_drag_event)
         self.viewers_list[1].mouse_drag_callbacks.append(self.mouse_drag_event)
         
         self.mask2D_list = []
         self.mask2D_list.append(np.ones(
             (self.data4D_shape[2], self.data4D_shape[3]), dtype='int8'))
         self.mask2D_list.append(np.ones(
             (self.data4D_shape[0], self.data4D_shape[1]), dtype='int8'))
+        self.mask2D_neg_list = []
+        self.mask2D_neg_list.append(np.zeros(
+            (self.data4D_shape[2], self.data4D_shape[3]), dtype='int8'))
+        self.mask2D_neg_list.append(np.zeros(
+            (self.data4D_shape[0], self.data4D_shape[1]), dtype='int8'))
         self.move_perv_time_time = 0
         napari.run()
     
     def show_mask(self, viewer):
         self.update_by_masked_sum_4D(viewer)
         viewer_index = self.viewers_list.index(viewer)
         self.logger(f'showing mask for viewer {viewer_index}')
+        mask2D = self.mask2D_list[viewer_index] - self.mask2D_neg_list[viewer_index]
         try:
             self.logger.log_single(
-                'mask', self.mask2D_list[viewer_index],time_tag = False)
+                'mask', mask2D,time_tag = False)
         except:
             pass
         plt.figure()
-        plt.imshow(self.mask2D_list[viewer_index])
+        plt.imshow(mask2D)
         plt.title(f'mask for viewer {viewer_index}')
         plt.show()
     
     def get_mask2D(self, shape_layer, mask_shape):
         from skimage.draw import polygon2mask
         from scipy.ndimage import binary_dilation, binary_fill_holes
         
@@ -126,34 +133,64 @@
     def update_by_masked_sum_4D(self, viewer, *args, **kwargs):
         viewer_index = self.viewers_list.index(viewer)
         
         data4D_shape_select = viewer.layers[0].data.shape
         mask2D = np.ones(data4D_shape_select, dtype='int8')
         if(len(viewer.layers) > 1):
             mask2D = self.get_mask2D(viewer.layers[1], data4D_shape_select)
+        mask2D_neg = np.zeros(data4D_shape_select, dtype='int8')
+        if(len(viewer.layers) > 2):
+            mask2D_neg = self.get_mask2D(viewer.layers[2], data4D_shape_select)
         
-        if( (self.mask2D_list[viewer_index] != mask2D).sum()>0):
+        if( ((self.mask2D_list[viewer_index] != mask2D).sum()>0) |
+            ( (self.mask2D_neg_list[viewer_index] != mask2D_neg).sum()>0) ):
             self.mask2D_list.__setitem__(viewer_index, mask2D.copy())
-            mask4D = np.zeros(self.data4D_shape, dtype='int8')
+            self.mask2D_neg_list.__setitem__(viewer_index, mask2D_neg.copy())
             if(viewer_index == 0):
-                if (self.mask2D_list[viewer_index]==1).sum() == 1:
-                    ind_r, ind_c = np.where(self.mask2D_list[viewer_index]==1)
+                if (mask2D==1).sum() == 1:
+                    ind_r, ind_c = np.where(mask2D==1)
                     STEM_img = self.data4D[..., ind_r, ind_c].squeeze().copy()
                 else:
-                    mask4D[:, :, self.mask2D_list[viewer_index]==1] = 1
+                    mask4D = np.zeros(self.data4D_shape, dtype='int8')
+                    mask4D[:, :, mask2D==1] = 1
                     STEM_img, _ = self.statistics_4D(self.data4D, mask4D)
+                if(mask2D_neg.sum() > 0):
+                    if (mask2D_neg==1).sum() == 1:
+                        ind_r, ind_c = np.where(mask2D_neg==1)
+                        STEM_img -= self.data4D[..., ind_r, ind_c].squeeze().copy()
+                    else:
+                        mask4D = np.zeros(self.data4D_shape, dtype='int8')
+                        mask4D[:, :, mask2D_neg==1] = 1
+                        _STEM_img, _ = self.statistics_4D(self.data4D, mask4D)
+                        STEM_img -= _STEM_img/mask2D_neg.sum()*(
+                            mask2D==1).sum()
+                
                 self.viewers_list[1].layers[0].data = STEM_img
                 self.logger('STEM image updated')
             if(viewer_index == 1):
-                if (self.mask2D_list[viewer_index]==1).sum() == 1:
-                    ind_x, ind_y = np.where(self.mask2D_list[viewer_index]==1)
+                if (mask2D==1).sum() == 1:
+                    ind_x, ind_y = np.where(mask2D==1)
                     PACBED = self.data4D[ind_x, ind_y].copy()
                 else:
-                    mask4D[self.mask2D_list[viewer_index]==1, :, :] = 1
+                    mask4D = np.zeros(self.data4D_shape, dtype='int8')
+                    mask4D[mask2D==1, :, :] = 1
                     _, PACBED = self.statistics_4D(self.data4D, mask4D)
+                    
+                if(mask2D_neg.sum() > 0):
+                    print('-+'*40)
+                    if (mask2D_neg==1).sum() == 1:
+                        ind_r, ind_c = np.where(mask2D_neg==1)
+                        PACBED -= self.data4D[ind_r, ind_c].squeeze().copy()
+                    else:
+                        mask4D = np.zeros(self.data4D_shape, dtype='int8')
+                        mask4D[mask2D_neg==1] = 1
+                        _, _PACBED = self.statistics_4D(self.data4D, mask4D)
+                        PACBED -= _PACBED/mask2D_neg.sum()*(
+                            mask2D==1).mean()
+                        
                 self.viewers_list[0].layers[0].data = PACBED
                 self.logger('PACBED image updated')
             
     def mouse_drag_event(self, viewer, event):
         dragged = False
         yield
         while event.type == 'mouse_move':
@@ -164,14 +201,15 @@
             
     def print_shape_info(self, viewer):
         self.logger(f'shape_type:{viewer.layers[1].shape_type}')
         self.logger(f'data:{viewer.layers[1].data}')
         self.logger(f'edge_width:{viewer.layers[1].edge_width}')
     
     def show_frame4D(self, viewer):
+        print('f pressed', flush = True)
         viewer_index = self.viewers_list.index(viewer)
         self.logger(f'showing frame for viewer {viewer_index}')
         data4D_shape_select = viewer.layers[0].data.shape
         mask2D = np.ones(data4D_shape_select, dtype='int8')
         if(len(viewer.layers) > 1):
             mask2D = self.get_mask2D(viewer.layers[1], data4D_shape_select)
         
@@ -200,29 +238,36 @@
             self.logger('No mask is selected, and I am surely not turning ' + \
                         'the whole datset into a frame')
         
     def move(self, viewer, axis, sign):
         viewer_index = self.viewers_list.index(viewer)
         if(len(viewer.layers) <= 1):
             return
+        layer = viewer.layers[1]
+        try:
+            layer_1 = int(str(viewer.layers.selection).split('[')[1].split(']')[0])
+            if layer_1 == 1:
+                layer = viewer.layers[2]
+        except:
+            pass
         time_since_last_move = time.time() - self.move_perv_time_time
-        n_shapes = len(viewer.layers[1].data)
-        selected_shape_cnt_list = list(viewer.layers[1].selected_data)
+        n_shapes = len(layer.data)
+        selected_shape_cnt_list = list(layer.selected_data)
         if selected_shape_cnt_list:
             cdata = []
             for shape_cnt in range(n_shapes):
-                _cdata = viewer.layers[1].data[int(shape_cnt)]
+                _cdata = layer.data[int(shape_cnt)]
                 if shape_cnt in selected_shape_cnt_list:
                     _cdata[:, axis] += sign
                 cdata.append(_cdata)
-            viewer.layers[1].data = cdata
+            layer.data = cdata
             selected_data = set()
             for shape_cnt in selected_shape_cnt_list:
                 selected_data.add(shape_cnt)
-            viewer.layers[1].selected_data = selected_data
+            layer.selected_data = selected_data
         sleep_between_moves = self.sleep_between_moves
         if (self.mask2D_list[viewer_index]==1).sum() == 1:
             sleep_between_moves = 0
         if time_since_last_move > sleep_between_moves:
             self.update_by_masked_sum_4D(viewer)
         self.move_perv_time_time = time.time()
```

### Comparing `mcemtools-0.9.2/mcemtools/tensor_svd.py` & `mcemtools-0.9.3/mcemtools/tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/mcemtools/transforms.py` & `mcemtools-0.9.3/mcemtools/transforms.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.9.3/mcemtools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.9.2
+Version: 0.9.3
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -38,23 +38,15 @@
 .. image:: https://img.shields.io/travis/arsadri/mcemtools.svg
         :target: https://travis-ci.com/arsadri/mcemtools
 
 .. image:: https://readthedocs.org/projects/mcemtools/badge/?version=latest
         :target: https://mcemtools.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
-
-.. image:: https://pyup.io/repos/github/arsadri/mcemtools/shield.svg
-     :target: https://pyup.io/repos/github/arsadri/mcemtools/
-     :alt: Updates
-
-
-
-State of the art aalysis for electron microscopy
-
+Deep unsupervised analysis tools for Four-dimensional Scanning Transmission Electron Microscopy (4D-STEM) 
 
 * Free software: MIT license
 * Documentation: https://mcemtools.readthedocs.io.
 
 
 Features
 --------
@@ -176,7 +168,11 @@
 * added denoise4_tsvd
 * faster bin_4D
 * torch handler does not update the model if the loss is inf or nan
 
 0.9.2 (2024-03-23)
 -------------------
 * annular mask can handle even sized image
+
+0.9.2 (2024-05-02)
+-------------------
+* viewer_4D takes second mask to subtract
```

### Comparing `mcemtools-0.9.2/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.9.3/mcemtools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,21 +30,23 @@
 mcemtools.egg-info/PKG-INFO
 mcemtools.egg-info/SOURCES.txt
 mcemtools.egg-info/dependency_links.txt
 mcemtools.egg-info/entry_points.txt
 mcemtools.egg-info/not-zip-safe
 mcemtools.egg-info/requires.txt
 mcemtools.egg-info/top_level.txt
+mcemtools/classifier/ResNet.py
+mcemtools/classifier/__init__.py
+mcemtools/classifier/capsnet.py
 mcemtools/denoise/DATOS.py
 mcemtools/denoise/LossFunc.py
 mcemtools/denoise/__init__.py
 mcemtools/denoise/cluster4net.py
 mcemtools/denoise/denoise4_tsvd.py
 mcemtools/denoise/denoise4net.py
 mcemtools/denoise/networks.py
-mcemtools/denoise/nn_from_torch.py
 tests/__init__.py
 tests/test_analysis.py
 tests/test_masking.py
 tests/test_mcemtools.py
 tests/test_tensor_svd.py
 tests/test_transforms.py
```

### Comparing `mcemtools-0.9.2/setup.py` & `mcemtools-0.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
```

### Comparing `mcemtools-0.9.2/tests/test_analysis.py` & `mcemtools-0.9.3/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/tests/test_mcemtools.py` & `mcemtools-0.9.3/tests/test_mcemtools.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/tests/test_tensor_svd.py` & `mcemtools-0.9.3/tests/test_tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.9.2/tests/test_transforms.py` & `mcemtools-0.9.3/tests/test_transforms.py`

 * *Files identical despite different names*

