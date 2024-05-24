# Comparing `tmp/rf-1.0.3.tar.gz` & `tmp/rf-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rf-1.0.3.tar", last modified: Thu Jan  4 21:47:57 2024, max compression
+gzip compressed data, was "rf-1.1.0.tar", last modified: Fri May 24 20:51:07 2024, max compression
```

## Comparing `rf-1.0.3.tar` & `rf-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,54 @@
-drwxr-xr-x   0 gi48zar  (15276) bioinf3   (2904)        0 2024-01-04 21:47:57.722887 rf-1.0.3/
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     4320 2024-01-04 16:39:00.000000 rf-1.0.3/CHANGELOG
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     1084 2024-01-04 15:35:33.000000 rf-1.0.3/LICENSE
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)      180 2024-01-04 15:35:33.000000 rf-1.0.3/MANIFEST.in
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     1388 2024-01-04 21:47:57.714887 rf-1.0.3/PKG-INFO
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     2451 2024-01-04 15:35:33.000000 rf-1.0.3/README.md
-drwxr-xr-x   0 gi48zar  (15276) bioinf3   (2904)        0 2024-01-04 21:47:57.386887 rf-1.0.3/rf/
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     9907 2024-01-04 16:38:16.000000 rf-1.0.3/rf/__init__.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)    16058 2024-01-04 15:35:33.000000 rf-1.0.3/rf/batch.py
-drwxr-xr-x   0 gi48zar  (15276) bioinf3   (2904)        0 2024-01-04 21:47:57.486887 rf-1.0.3/rf/data/
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     2429 2024-01-04 15:35:33.000000 rf-1.0.3/rf/data/iasp91.dat
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)    27623 2024-01-04 15:35:33.000000 rf-1.0.3/rf/deconvolve.py
-drwxr-xr-x   0 gi48zar  (15276) bioinf3   (2904)        0 2024-01-04 21:47:57.570887 rf-1.0.3/rf/example/
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     3661 2024-01-04 15:35:33.000000 rf-1.0.3/rf/example/conf.json
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)   145408 2024-01-04 15:35:33.000000 rf-1.0.3/rf/example/example_data.mseed
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)    17203 2024-01-04 15:35:33.000000 rf-1.0.3/rf/example/example_events.xml
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     6101 2024-01-04 15:35:33.000000 rf-1.0.3/rf/example/example_inventory.xml
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)    12210 2024-01-04 15:35:33.000000 rf-1.0.3/rf/example/minimal_example.tar.gz
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)    11590 2024-01-04 15:35:33.000000 rf-1.0.3/rf/example/minimal_example_S.tar.gz
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)    13817 2024-01-04 15:59:33.000000 rf-1.0.3/rf/imaging.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     4900 2024-01-04 15:35:33.000000 rf-1.0.3/rf/profile.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)    28059 2024-01-04 15:35:33.000000 rf-1.0.3/rf/rfstream.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     8849 2024-01-04 15:35:33.000000 rf-1.0.3/rf/simple_model.py
-drwxr-xr-x   0 gi48zar  (15276) bioinf3   (2904)        0 2024-01-04 21:47:57.682887 rf-1.0.3/rf/tests/
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)      393 2024-01-04 15:35:33.000000 rf-1.0.3/rf/tests/__init__.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)       32 2024-01-04 15:35:33.000000 rf-1.0.3/rf/tests/__main__.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     3782 2024-01-04 15:35:33.000000 rf-1.0.3/rf/tests/test_batch.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     7210 2024-01-04 15:35:33.000000 rf-1.0.3/rf/tests/test_deconvolve.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     1112 2024-01-04 15:35:33.000000 rf-1.0.3/rf/tests/test_imaging.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     1334 2024-01-04 15:35:33.000000 rf-1.0.3/rf/tests/test_profile.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     8576 2024-01-04 15:35:33.000000 rf-1.0.3/rf/tests/test_rfstream.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)    30895 2024-01-04 15:35:33.000000 rf-1.0.3/rf/tests/test_simple_model.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)      891 2024-01-04 15:35:33.000000 rf-1.0.3/rf/tests/util.py
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     8993 2024-01-04 15:35:33.000000 rf-1.0.3/rf/util.py
-drwxr-xr-x   0 gi48zar  (15276) bioinf3   (2904)        0 2024-01-04 21:47:57.694887 rf-1.0.3/rf.egg-info/
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     1388 2024-01-04 21:47:57.000000 rf-1.0.3/rf.egg-info/PKG-INFO
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)      767 2024-01-04 21:47:57.000000 rf-1.0.3/rf.egg-info/SOURCES.txt
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)        1 2024-01-04 21:47:57.000000 rf-1.0.3/rf.egg-info/dependency_links.txt
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)       67 2024-01-04 21:47:57.000000 rf-1.0.3/rf.egg-info/entry_points.txt
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)        1 2024-01-04 16:00:34.000000 rf-1.0.3/rf.egg-info/not-zip-safe
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)      196 2024-01-04 21:47:57.000000 rf-1.0.3/rf.egg-info/requires.txt
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)        3 2024-01-04 21:47:57.000000 rf-1.0.3/rf.egg-info/top_level.txt
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)       38 2024-01-04 21:47:57.726887 rf-1.0.3/setup.cfg
--rw-r--r--   0 gi48zar  (15276) bioinf3   (2904)     2083 2024-01-04 15:35:33.000000 rf-1.0.3/setup.py
+drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2024-05-24 20:51:07.547014 rf-1.1.0/
+-rw-rw-r--   0 eule      (1000) eule      (1000)     4574 2024-05-24 20:47:34.000000 rf-1.1.0/CHANGELOG
+-rw-rw-r--   0 eule      (1000) eule      (1000)     1098 2024-05-24 20:39:56.000000 rf-1.1.0/LICENSE
+-rw-rw-r--   0 eule      (1000) eule      (1000)      180 2016-06-18 00:15:31.000000 rf-1.1.0/MANIFEST.in
+-rw-r--r--   0 eule      (1000) eule      (1000)     1191 2024-05-24 20:51:07.543014 rf-1.1.0/PKG-INFO
+-rw-rw-r--   0 eule      (1000) eule      (1000)     2544 2024-05-24 20:39:56.000000 rf-1.1.0/README.md
+drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2024-05-24 20:51:07.539014 rf-1.1.0/rf/
+-rw-rw-r--   0 eule      (1000) eule      (1000)    10037 2024-05-24 20:48:35.000000 rf-1.1.0/rf/__init__.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)    16058 2019-10-17 07:25:24.000000 rf-1.1.0/rf/batch.py
+drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2024-05-24 20:51:07.539014 rf-1.1.0/rf/data/
+-rw-rw-r--   0 eule      (1000) eule      (1000)     2429 2015-06-22 16:30:18.000000 rf-1.1.0/rf/data/iasp91.dat
+-rw-rw-r--   0 eule      (1000) eule      (1000)    27682 2024-05-22 21:31:41.000000 rf-1.1.0/rf/deconvolve.py
+drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2024-05-24 20:51:07.543014 rf-1.1.0/rf/example/
+-rw-rw-r--   0 eule      (1000) eule      (1000)     3661 2016-07-12 15:27:36.000000 rf-1.1.0/rf/example/conf.json
+-rw-rw-r--   0 eule      (1000) eule      (1000)   145408 2016-06-22 09:42:26.000000 rf-1.1.0/rf/example/example_data.mseed
+-rw-rw-r--   0 eule      (1000) eule      (1000)   145408 2016-05-27 19:35:04.000000 rf-1.1.0/rf/example/example_data_old.mseed
+-rw-rw-r--   0 eule      (1000) eule      (1000)    17203 2016-06-22 09:42:26.000000 rf-1.1.0/rf/example/example_events.xml
+-rw-rw-r--   0 eule      (1000) eule      (1000)    17203 2016-05-27 19:35:04.000000 rf-1.1.0/rf/example/example_events_old.xml
+-rw-rw-r--   0 eule      (1000) eule      (1000)     6101 2014-03-22 19:44:45.000000 rf-1.1.0/rf/example/example_inventory.xml
+-rw-rw-r--   0 eule      (1000) eule      (1000)    12210 2016-06-22 09:42:27.000000 rf-1.1.0/rf/example/minimal_example.tar.gz
+-rw-rw-r--   0 eule      (1000) eule      (1000)    11590 2016-06-22 09:42:27.000000 rf-1.1.0/rf/example/minimal_example_S.tar.gz
+-rw-rw-r--   0 eule      (1000) eule      (1000)     7880 2024-05-24 20:39:56.000000 rf-1.1.0/rf/harmonics.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)    18538 2024-05-24 20:39:56.000000 rf-1.1.0/rf/imaging.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     4900 2019-10-17 07:25:24.000000 rf-1.1.0/rf/profile.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)    28368 2024-05-24 20:39:56.000000 rf-1.1.0/rf/rfstream.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     8849 2019-12-09 16:23:28.000000 rf-1.1.0/rf/simple_model.py
+drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2024-05-24 20:51:07.543014 rf-1.1.0/rf/syn/
+-rw-rw-r--   0 eule      (1000) eule      (1000)        0 2019-10-08 13:17:18.000000 rf-1.1.0/rf/syn/__init__.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)      195 2020-05-11 15:28:23.000000 rf-1.1.0/rf/syn/core.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     2938 2020-04-22 11:17:44.000000 rf-1.1.0/rf/syn/tws.py
+drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2024-05-24 20:51:07.543014 rf-1.1.0/rf/tests/
+-rw-rw-r--   0 eule      (1000) eule      (1000)      393 2019-12-11 09:55:38.000000 rf-1.1.0/rf/tests/__init__.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)       32 2016-07-08 23:04:34.000000 rf-1.1.0/rf/tests/__main__.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     3782 2019-10-17 07:25:25.000000 rf-1.1.0/rf/tests/test_batch.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     7210 2021-01-21 09:31:32.000000 rf-1.1.0/rf/tests/test_deconvolve.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     2023 2024-05-24 20:39:56.000000 rf-1.1.0/rf/tests/test_harmonics.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     1455 2024-05-24 20:39:56.000000 rf-1.1.0/rf/tests/test_imaging.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     1334 2017-04-10 15:47:47.000000 rf-1.1.0/rf/tests/test_profile.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     8576 2019-10-17 07:25:25.000000 rf-1.1.0/rf/tests/test_rfstream.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)    30895 2017-04-10 15:47:47.000000 rf-1.1.0/rf/tests/test_simple_model.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     2359 2019-07-01 07:54:55.000000 rf-1.1.0/rf/tests/test_util.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)      891 2017-04-10 15:47:47.000000 rf-1.1.0/rf/tests/util.py
+-rw-rw-r--   0 eule      (1000) eule      (1000)     8993 2019-10-17 07:25:25.000000 rf-1.1.0/rf/util.py
+drwxrwxr-x   0 eule      (1000) eule      (1000)        0 2024-05-24 20:51:07.543014 rf-1.1.0/rf.egg-info/
+-rw-r--r--   0 eule      (1000) eule      (1000)     1191 2024-05-24 20:51:07.000000 rf-1.1.0/rf.egg-info/PKG-INFO
+-rw-rw-r--   0 eule      (1000) eule      (1000)      969 2024-05-24 20:51:07.000000 rf-1.1.0/rf.egg-info/SOURCES.txt
+-rw-rw-r--   0 eule      (1000) eule      (1000)        1 2024-05-24 20:51:07.000000 rf-1.1.0/rf.egg-info/dependency_links.txt
+-rw-rw-r--   0 eule      (1000) eule      (1000)       67 2024-05-24 20:51:07.000000 rf-1.1.0/rf.egg-info/entry_points.txt
+-rw-rw-r--   0 eule      (1000) eule      (1000)        1 2016-05-31 21:08:33.000000 rf-1.1.0/rf.egg-info/not-zip-safe
+-rw-rw-r--   0 eule      (1000) eule      (1000)       47 2016-09-12 12:04:02.000000 rf-1.1.0/rf.egg-info/pbr.json
+-rw-rw-r--   0 eule      (1000) eule      (1000)      200 2024-05-24 20:51:07.000000 rf-1.1.0/rf.egg-info/requires.txt
+-rw-rw-r--   0 eule      (1000) eule      (1000)        3 2024-05-24 20:51:07.000000 rf-1.1.0/rf.egg-info/top_level.txt
+-rw-rw-r--   0 eule      (1000) eule      (1000)       38 2024-05-24 20:51:07.547014 rf-1.1.0/setup.cfg
+-rw-rw-r--   0 eule      (1000) eule      (1000)     1906 2024-05-22 21:31:41.000000 rf-1.1.0/setup.py
```

### Comparing `rf-1.0.3/CHANGELOG` & `rf-1.1.0/CHANGELOG`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+1.1.0:
+  * add calculation of harmonic decomposition and corresponding plot (see #48)
+  * update multitaper deconvolution to use the multitaper package instead of outdated mtspec (see #49)
+  * add option to only plot stacked receiver function (see #48)
 1.0.3:
-  * fix: use ax.sharey instead of join method which is unsupported in recent mpl verions
+  * fix: use ax.sharey instead of join method which is unsupported in recent mpl versions
 1.0.2:
   * enhance compatibility with SeismicHandler (see #37, #38)
   * fix: replace np.asscalar
 1.0.1:
   * improvements for iterative deconvolution (see #33)
 1.0.0:
   * add iterative deconvolution and multitaper deconvolution (see #30, #31)
```

### Comparing `rf-1.0.3/LICENSE` & `rf-1.1.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2013-2019 Tom Eulenfeld
+Copyright (c) 2013-2024 Tom Eulenfeld, Hannah Mark
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
@@ -13,8 +13,8 @@
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `rf-1.0.3/README.md` & `rf-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # rf
 ## Receiver function calculation in seismology
 [![build status](https://github.com/trichter/rf/workflows/tests/badge.svg)](https://github.com/trichter/rf/actions)
+[![docs status](https://readthedocs.org/projects/rf/badge/?version=latest)](https://rf.readthedocs.io)
 [![codecov](https://codecov.io/gh/trichter/rf/branch/master/graph/badge.svg)](https://codecov.io/gh/trichter/rf)
 [![pypi version](https://img.shields.io/pypi/v/rf.svg)](https://pypi.python.org/pypi/rf)
 [![python version](https://img.shields.io/pypi/pyversions/rf.svg)](https://python.org)
 [![JOSS](http://joss.theoj.org/papers/10.21105/joss.01808/status.svg)](https://doi.org/10.21105/joss.01808)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4455036.svg)](https://doi.org/10.5281/zenodo.4455036)
 
 ##### Documentation: https://rf.readthedocs.io/
 ##### Tutorials:
   1. Calculate receiver functions - minimal example ([notebook][nb1])
   2. Calculate receiver functions and stack them by common conversion points to create a profile ([notebook][nb2])
   3. Compare different deconvolution methods ([notebook][nb3])
+  4. Harmonic deconvolution with synthetics - minimal example ([notebook][nb4])
 
 [nb1]: https://nbviewer.jupyter.org/github/trichter/notebooks/blob/master/receiver_function_minimal_example.ipynb
 [nb2]: https://nbviewer.jupyter.org/github/trichter/notebooks/blob/master/receiver_function_profile_chile.ipynb
 [nb3]: https://nbviewer.jupyter.org/github/hfmark/notebooks/blob/main/rf_comparison.ipynb
+[nb4]: https://nbviewer.jupyter.org/github/hfmark/notebooks/blob/main/rf_harmonics.ipynb
 
 ##### Get help and discuss: [ObsPy Related Projects category](https://discourse.obspy.org/c/obspy-related-projects/rf/14) in the ObsPy forum
 
 ##### Contribute:
 
 All contributions are welcome ... e.g. report bugs, discuss or add new features.
-For example, the package could profit from more advanced deconvolution techniques.
-New deconvolution functions can be tested by just passing them to deconvolve method (see docs).
 
 ##### Citation:
 
 If you found this package useful, please consider citing it.
 
 Tom Eulenfeld (2020), rf: Receiver function calculation in seismology, *Journal of Open Source Software*, 5(48), 1808, doi: [10.21105/joss.01808](https://doi.org/10.21105/joss.01808) [[pdf]](https://www.theoj.org/joss-papers/joss.01808/10.21105.joss.01808.pdf)
```

### Comparing `rf-1.0.3/rf/__init__.py` & `rf-1.1.0/rf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 Installation
 ------------
 
 Dependencies of rf are
 
     * ObsPy_ and some of its dependencies,
     * cartopy, geographiclib, shapely,
-    * mtspec_ for multitaper deconvolution,
+    * multitaper_ for multitaper deconvolution,
     * toeplitz_ for faster time domain deconvolution (optional),
     * obspyh5_ for hdf5 file support (optional),
     * tqdm for progress bar in batch processing (optional).
 
 rf can be installed with ::
 
     pip install rf
@@ -71,15 +71,15 @@
 To install the development version of rf download the source code and run ::
 
     pip install .
 
 Here are some instructions to install rf into a fresh conda environment::
 
     conda config --add channels conda-forge
-    conda create -n rfenv obspy cartopy geographiclib shapely h5py mtspec tqdm fortran-compiler
+    conda create -n rfenv obspy cartopy geographiclib shapely h5py multitaper tqdm fortran-compiler
     conda activate rfenv
     pip install obspyh5 toeplitz rf
     rf-runtests
 
 The ``fortran-compiler`` metapackage helps finding the right fortran compiler
 and its dependencies for any OS. Often, problems with the compilation of Fortran
 codes (toeplitz package) can be solved by setting
@@ -187,26 +187,29 @@
     * rotation
     * deconvolution
 
 Please see `.RFStream.rf()`
 for a more detailed description.
 RFStream provides the possibility to perform moveout correction,
 piercing point calculation and profile stacking.
+There are also functions included for calculating back-azimuthal harmonics
+from an RFStream.
 
 Tutorials
 ---------
 
 The following Jupyter notebooks can be viewed online or downloaded
 to be locally reproduced.
 
     1. Calculate receiver functions - minimal example (notebook1_)
     2. Calculate receiver functions and stack them by common conversion points
        to create a profile (notebook2_)
     3. Calculate and compare receiver functions calculated with different
        deconvolution methods (notebook3_)
+    4. Harmonic deconvolution with synthetics - minimal example (notebook4_)
 
 Command line tool for batch processing
 --------------------------------------
 
 The rf package provides a command line utility 'rf' which runs all the
 necessary steps to perform receiver function calculation.
 Use
@@ -255,24 +258,22 @@
 .. __: https://doi.org/10.21105/joss.01808
 
 .. _this: https://doi.org/10.17169/refubium-14424
 .. _ObsPy: http://www.obspy.org/
 .. _pip: http://www.pip-installer.org/
 .. _obspyh5: https://github.com/trichter/obspyh5/
 .. _toeplitz: https://github.com/trichter/toeplitz/
-.. _mtspec: https://github.com/krischer/mtspec
+.. _multitaper: https://github.com/gaprieto/multitaper
 
 .. _notebook1: http://nbviewer.jupyter.org/github/trichter/notebooks/blob/master/receiver_function_minimal_example.ipynb
 .. _notebook2: http://nbviewer.jupyter.org/github/trichter/notebooks/blob/master/receiver_function_profile_chile.ipynb
 .. _notebook3: https://nbviewer.jupyter.org/github/hfmark/notebooks/blob/main/rf_comparison.ipynb
+.. _notebook4: https://nbviewer.jupyter.org/github/hfmark/notebooks/blob/main/rf_harmonics.ipynb
 
 .. _GitHub: https://github.com/trichter/rf/
 """
 
-__version__ = '1.0.3'
+__version__ = '1.1.0'
 
 from rf.profile import get_profile_boxes
 from rf.rfstream import read_rf, RFStream, rfstats
 from rf.util import iter_event_data, IterMultipleComponents
-
-if 'dev' not in __version__:  # get image for correct version from travis-ci
-    __doc__ = __doc__.replace('branch=master', 'branch=v%s' % __version__)
```

### Comparing `rf-1.0.3/rf/batch.py` & `rf-1.1.0/rf/batch.py`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/data/iasp91.dat` & `rf-1.1.0/rf/data/iasp91.dat`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/deconvolve.py` & `rf-1.1.0/rf/deconvolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,15 +455,15 @@
         corresponds to cut-off frequency in Hz for a response value of
         exp(-0.5)=0.607.
     :param itmax: limit on number of iterations/spikes to add
     :param minderr: stop iteration when the change in error from adding another
         spike drops below this threshold
     :param mute_shift: Mutes all samples at beginning of trace
         (lenght given by time shift).
-        For `len(src)==len(rsp)` this mutes all samples before the onset.
+        For ``len(src)==len(rsp)`` this mutes all samples before the onset.
     :param normalize: normalize all results so that the maximum of the trace
         with the supplied index is 1. Set normalize to None for no normalization.
 
     :return: (list of) array(s) with deconvolution(s)
     """
 
     ncomp = len(rsp)    # number of components we're looping over here
@@ -554,40 +554,40 @@
     :param olap: window overlap between 0 and 1 (default: 0.75)
     :param normalize: normalize all results so that the maximum of the trace
         with supplied index is 1. Set normalize to None for no normalization.
 
     :return: (list of) array(s) with deconvolution(s)
     """
     try:
-        import mtspec as mt
+        import multitaper as mt
     except ImportError as ex:
-        msg = 'mtspec package is needed for multitaper deconvolution'
+        msg = 'multitaper package is needed for multitaper deconvolution'
         raise ImportError(msg) from ex
 
     # check src trace length < rsp trace length:
     assert len(src) < len(rsp[0]), 'source wavelet must be shorter than response'
     assert len(nse[0]) <= len(rsp[0]), 'noise should not be longer than response'
 
     nft = len(rsp[0])  # length of final arrays
     dt = 1./sampling_rate  # sample spacing
 
-    # calculate multitapers with mtspec
+    # calculate multitapers with German's multitaper package
     ntap = int(round(T/dt))  # #points in each taper
-
-    tap, el, _ = mt.multitaper.dpss(ntap, tband, K); tap = tap.T
+    slepians = mt.MTSpec(np.arange(ntap),nw=tband,kspec=K)
+    tap = slepians.vn.T; el = slepians.lamb
     if K >= 2:
         tap[1] = -tap[1]  # adjust to match sign convention
     if K >= 3:
         tap[2] = -tap[2]
     if K > 3:
         print('Warning: taper signs may need adjustment for K>3')
 
     ofac = 1 / (1 - olap)  # calculate overlap factor
 
-    sfft = np.zeros((K,nft), dtype=np.complex)  # array for holding freq-domain source estimate
+    sfft = np.zeros((K,nft), dtype=complex)  # array for holding freq-domain source estimate
     src = detrend(src, type='constant')  # demean and detrend source
     src = detrend(src, type='linear')
 
     # window and taper the source
     nwav = len(src)   # number of nonzero points for the source
     nwin = int(ofac*nwav/ntap)  # number of windows needed to cover the source
 
@@ -608,16 +608,16 @@
     sfft = fac*sfft
 
     # loop response components and do a similar window/taper/transform thing
     ncomp = len(rsp)
     RF_out = np.zeros((ncomp, nft))
     for c in range(ncomp):
         dat = rsp[c]; nos = nse[c]  # pick out component
-        dfft = np.zeros((K,nft), dtype=np.complex)  # arrays for storing freq-domain estimates
-        nfft = np.zeros((K,nft), dtype=np.complex)
+        dfft = np.zeros((K,nft), dtype=complex)  # arrays for storing freq-domain estimates
+        nfft = np.zeros((K,nft), dtype=complex)
 
         # window, taper, and transform the noise
         nos = detrend(nos, type='constant')
         nos = detrend(nos, type='linear')
         nos_pad = np.zeros(nft)
         nos_pad[:len(nos)] = nos
         nwin = int(ofac*len(nos)/ntap)
```

### Comparing `rf-1.0.3/rf/example/conf.json` & `rf-1.1.0/rf/example/conf.json`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/example/example_data.mseed` & `rf-1.1.0/rf/example/example_data.mseed`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/example/example_events.xml` & `rf-1.1.0/rf/example/example_events.xml`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/example/example_inventory.xml` & `rf-1.1.0/rf/example/example_inventory.xml`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/example/minimal_example.tar.gz` & `rf-1.1.0/rf/example/minimal_example.tar.gz`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/example/minimal_example_S.tar.gz` & `rf-1.1.0/rf/example/minimal_example_S.tar.gz`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/imaging.py` & `rf-1.1.0/rf/imaging.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,46 +21,57 @@
         if len(labelset) == 1:
             return labelset.pop()
     return ''
 
 
 def plot_rf(stream, fname=None, fig_width=7., trace_height=0.5,
             stack_height=0.5, dpi=None,
-            scale=1, fillcolors=(None, None), trim=None,
+            trace_scale=False, scale_factor=1, fillcolors=(None, None), trim=None,
             info=(('back_azimuth', u'baz (°)', 'C0'),
                   ('distance', u'dist (°)', 'C3')),
+            show_traces=True,
             show_vlines=False):
     """
     Plot receiver functions.
 
     :param stream: stream to plot
     :param fname: filename to save plot to. Can be None. In this case
         the figure is left open.
     :param fig_width: width of figure in inches
     :param trace_height: height of one trace in inches
     :param stack_height: height of stack axes in inches
     :param dpi: dots per inch for the created figure
-    :param scale: scale for individual traces
+    :param trace_scale: if True, scale each trace individually; if false,
+        scale traces by global max amplitude
+    :param scale_factor: factor for scaling traces, either individually
+        or globally. A value of 1 generally works well.
     :param fillcolors: fill colors for positive and negative wiggles
     :param trim: trim stream relative to onset before plotting using
          `~.rfstream.RFStream.slice2()`
     :param info: Plot one additional axes showing maximal two entries of
         the stats object. Each entry in this list is a list consisting of
         three entries: key, label and color.
         info can be None. In this case no additional axes is plotted.
     :param show_vlines: If True, show vertical alignment grid lines on plot
         at positions of the major x-tick marks.
+    :param show_traces: If True, plot the individual traces in the stream
+        in an additional set of axes below the plot of the stacked trace. If
+        False, info will also be set to None and the only thing plotted
+        is the stacked trace.
     """
 
     if len(stream) == 0:
         return
     if trim:
         stream = stream.slice2(*trim, reftime='onset')
     if info is None:
         info = ()
+    if not show_traces:
+        info = None
+        trace_height = 0
     N = len(stream)
     # calculate axes and figure dimensions
     # big letters: inches, small letters: figure fraction
     H = trace_height
     HS = stack_height
     FB = 0.5
     FT = 0.2
@@ -77,15 +88,16 @@
     FW2 = FW - FL - FR - (DW + FW3) * bool(info)
     fl = FL / FW
     fr = FR / FW
     fw2 = FW2 / FW
     fw3 = FW3 / FW
     # init figure and axes
     fig = plt.figure(figsize=(FW, FH), dpi=dpi)
-    ax1 = fig.add_axes([fl, fb, fw2, h * (N + 2)])
+    if show_traces:
+        ax1 = fig.add_axes([fl, fb, fw2, h * (N + 2)])
     if info:
         ax3 = fig.add_axes(
             [1 - fr - fw3, fb, fw3, h * (N + 2)], sharey=ax1)
         info = list(info)
         info[0] = [ax3] + list(info[0])
         if len(info) > 1:
             ax4 = ax3.twiny()
@@ -96,68 +108,81 @@
         c1, c2 = fillcolors
         if c1:
             ax.fill_between(t, d + i, i, where=d >= 0, lw=0., facecolor=c1)
         if c2:
             ax.fill_between(t, d + i, i, where=d < 0, lw=0., facecolor=c2)
         ax.plot(t, d + i, 'k')
     xlim = (0, 0)
-    max_ = max(np.max(np.abs(tr.data)) for tr in stream)
+    max_ = max(np.max(np.abs(tr.data))
+               for tr in stream)  # for scaling, if not trace_scale
     for i, tr in enumerate(stream):
         times = tr.times(reftime=tr.stats.onset)
         xlim = (min(xlim[0], times[0]), max(xlim[1], times[-1]))
-        _plot(ax1, times, tr.data / max_ * scale, i + 1)
+        if show_traces:
+            # scale trace by trace (otherwise, we scale by global trace max)
+            if trace_scale:
+                max_ = max(np.abs(tr.data))
+            _plot(ax1, times, tr.data / max_ * scale_factor, i + 1)
     # plot right axes with header information
-    for ax, header, label, color in info:
-        data = [tr.stats[header] for tr in stream]
-        ax.plot(data, 1 + np.arange(len(stream)), '.' + color, mec=color)
-        ax.set_xlabel(label, color=color, size='small')
-        if header == 'back_azimuth':
-            ax.set_xticks(np.arange(5) * 90)
-            ax.set_xticklabels(['0', '', '180', '', '360'], size='small')
-        else:
-            ax.xaxis.set_major_locator(MaxNLocator(4))
-            for l in ax.get_xticklabels():
-                l.set_fontsize('small')
-        ax.xaxis.set_minor_locator(AutoMinorLocator())
-    # set x and y limits
-    ax1.set_xlim(*xlim)
-    ax1.set_ylim(-0.5, N + 1.5)
-    ax1.set_yticklabels('')
-    ax1.set_xlabel('time (s)')
-    ax1.xaxis.set_minor_locator(AutoMinorLocator())
-    aligner_color = "#a0a0a080"
-    if show_vlines:
-        ax1.xaxis.grid(True, color=aligner_color, linestyle=':')
+    if info:
+        for ax, header, label, color in info:
+            data = [tr.stats[header] for tr in stream]
+            ax.plot(data, 1 + np.arange(len(stream)), '.' + color, mec=color)
+            ax.set_xlabel(label, color=color, size='small')
+            if header == 'back_azimuth':
+                ax.set_xticks(np.arange(5) * 90)
+                ax.set_xticklabels(['0', '', '180', '', '360'], size='small')
+            else:
+                ax.xaxis.set_major_locator(MaxNLocator(4))
+                for l in ax.get_xticklabels():
+                    l.set_fontsize('small')
+            ax.xaxis.set_minor_locator(AutoMinorLocator())
+    if show_traces:
+        # set x and y limits
+        ax1.set_xlim(*xlim)
+        ax1.set_ylim(-0.5, N + 1.5)
+        ax1.set_yticklabels('')
+        ax1.set_xlabel('time (s)')
+        ax1.xaxis.set_minor_locator(AutoMinorLocator())
+        aligner_color = "#a0a0a080"
+        if show_vlines:
+            ax1.xaxis.grid(True, color=aligner_color, linestyle=':')
 
     # plot stack
     try:
         stack = stream.stack()
     except ValueError:
         msg = 'Different npts for traces in one RF plot. Do not plot stack.'
         warnings.warn(msg)
     else:
         if len(stack) > 1:
             warnings.warn('Different stations or channels in one RF plot. ' +
                           'Do not plot stack.')
         elif len(stack) == 1:
-            ax2 = fig.add_axes([fl, 1 - ft - hs, fw2, hs], sharex=ax1)
+            if show_traces:
+                ax2 = fig.add_axes([fl, 1 - ft - hs, fw2, hs], sharex=ax1)
+            elif not show_traces:
+                ax2 = fig.add_axes([fl, 1 - ft - hs, fw2, hs])
             _plot(ax2, times, stack[0].data, 0)
+            if not show_traces:
+                ax2.set_xlim(*xlim)
             for l in ax2.get_xticklabels():
                 l.set_visible(False)
             ax2.yaxis.set_major_locator(MaxNLocator(4))
             for l in ax2.get_yticklabels():
                 l.set_fontsize('small')
             if show_vlines:
                 ax2.xaxis.grid(True, color=aligner_color, linestyle=':')
     # annotate plot with seed id
     bbox = dict(boxstyle='round', facecolor='white', alpha=0.8, lw=0)
     title = '%s traces  %s' % (len(stream), _label(stream))
-    ax1.annotate(title, (1 - 0.5 * fr, 1 - 0.5 * ft),
-                 xycoords='figure fraction', va='top', ha='right',
-                 bbox=bbox, clip_on=False)
+    if show_traces:
+        ax1.annotate(title, (1 - 0.5 * fr, 1 - 0.5 * ft),
+                     xycoords='figure fraction', va='top', ha='right',
+                     bbox=bbox, clip_on=False)
     # save plot
     if fname:
         fig.savefig(fname, dpi=dpi)
         plt.close(fig)
     else:
         return fig
 
@@ -348,7 +373,99 @@
         raise NotImplementedError("'%s' not supported for top parameter" % top)
     ax.set_xlim(*xlim)
     if fname:
         fig.savefig(fname, dpi=dpi)
         plt.close(fig)
     else:
         return fig
+
+
+def plot_harmonics(hd, hd2=None, fillcolors=('b', 'r'), trim=None):
+    """
+    Plot components from harmonic decomposition.
+
+    The plot will have two panels. In all cases the left panel will show
+    the modeled components of hd.
+    If hd2 is supplied, the right panel will show the modeled components of hd2.
+    If hd2 is None and hd has unmodeled components, those will be on the right.
+    If hd2 is None and hd does not have unmodeled components, the right panel will
+    be empty.
+
+    :param hd: RFStream of harmonics, returned from `rf.harmonics.harmonics()`
+        or the corresponding `~rf.rfstream.RFStream.harmonics()` method.
+        The stream should contain modeled components, and may also include
+        unmodeled components
+    :param hd2: Optional second RFStream of harmonics. If used, it should
+        contain modeled components
+    :param fillcolors: fill colors for positive and negative wiggles
+    :param trim: trim stream relative to onset before plotting using
+        `~rf.rfstream.RFStream.slice2()`
+
+    """
+    if trim:
+        try:
+            hd = hd.slice2(*trim, reftime='onset')
+            if hd2:
+                hd2 = hd2.slice2(*trim, reftime='onset')
+        except AttributeError:  # if it's obspy.Stream() instead of RFStream(), might still work
+            warnings.warn(
+                'Warning: onset is not in trace stats, so this may not work as expected')
+    ref0 = max(abs(hd.select(channel='0', location='mod')[0].data))
+    for tr in hd:
+        if max(abs(tr.data)) > ref0:
+            ref0 = max(abs(tr.data))
+    mod = hd.select(location='mod')
+    if hd2:
+        ref1 = max(abs(hd2.select(channel='0', location='mod')[0].data))
+        for tr in hd2.select(location='mod'):
+            if max(abs(tr.data)) > ref0:
+                ref1 = max(abs(tr.data))
+        unmod = hd2.select(location='mod')
+    else:
+        ref1 = ref0
+        unmod = hd.select(location='unmod')
+
+    fig = plt.figure(constrained_layout=True)
+    gs = fig.add_gridspec(1, 2)
+    ax_mod = fig.add_subplot(gs[:, 0])
+    ax_unmod = fig.add_subplot(gs[:, 1], sharey=ax_mod, sharex=ax_mod)
+
+    def _plot(ax, t, d, i):
+        c1, c2 = fillcolors
+        if c1:
+            ax.fill_between(t, d + i, i, where=d >= 0, lw=0., facecolor=c1)
+        if c2:
+            ax.fill_between(t, d + i, i, where=d < 0, lw=0., facecolor=c2)
+        ax.plot(t, d + i, 'k')
+
+    for i in range(5):
+        tr = mod[i]
+        t = tr.times(reftime=tr.stats.onset)
+        j = 4 - int(tr.stats['channel'])
+        wiggle = tr.data/ref0
+        _plot(ax_mod, t, wiggle, j)
+        if len(unmod) > 0:
+            tr = unmod[i]
+            t = tr.times(reftime=tr.stats.onset)
+            j = 4 - int(tr.stats['channel'])
+            wiggle = tr.data/ref1
+            _plot(ax_unmod, t, wiggle, j)
+
+    ax_mod.set_title('anisotropy/dip %s' % mod[0].stats.components)
+    if not hd2 and len(unmod) > 0:
+        ax_unmod.set_title('unmodeled %s' % mod[0].stats.components)
+    if hd2:
+        ax_unmod.set_title('anisotropy/dip %s' % unmod[0].stats.components)
+
+    ax_mod.set_xlabel('Delay time [s]')
+    ax_unmod.set_xlabel('Delay time [s]')
+
+    ax_mod.yaxis.set_ticks(np.arange(5))
+    ax_mod.set_yticklabels(['sin($2\\theta$)', 'cos($2\\theta$)',
+                            'sin($\\theta$)', 'cos($\\theta$)', 'constant'])
+    ax_unmod.yaxis.tick_right()
+    if trim:
+        ax_mod.set_xlim(trim)  # fallback if not trimmed as requested
+
+    fig.suptitle('Harmonics: %s' % (mod[0].stats.station))
+
+    return fig
```

### Comparing `rf-1.0.3/rf/profile.py` & `rf-1.1.0/rf/profile.py`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/rfstream.py` & `rf-1.1.0/rf/rfstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import numpy as np
 from obspy import read, Stream, Trace
 from obspy.core import AttribDict
 from obspy.geodetics import gps2dist_azimuth
 from obspy.taup import TauPyModel
 from rf.deconvolve import deconvolve
+from rf.harmonics import harmonics
 from rf.simple_model import load_model
 from rf.util import DEG2KM, IterMultipleComponents, _add_processing_info
 
 
 def __get_event_origin_prop(h):
     def wrapper(event):
         try:
@@ -424,14 +425,24 @@
             tr2 = RFTrace(data=data, header=header)
             if 'onset' in tr.stats:
                 onset = tr.stats.onset - tr.stats.starttime
                 tr2.stats.onset = tr2.stats.starttime + onset
             traces.append(tr2)
         return self.__class__(traces)
 
+    def harmonics(self, *args, **kwargs):
+        """
+        Perform harmonic decomposition on stream.
+
+        All args and kwargs are passed to the function
+        `~rf.harmonics.harmonics()`.
+        """
+        hd = harmonics(self, *args, **kwargs)
+        return hd
+
     def profile(self, *args, **kwargs):
         """
         Return profile of receiver functions in the stream.
 
         See `.profile.profile()` for help on arguments.
         """
         from rf.profile import profile
```

### Comparing `rf-1.0.3/rf/simple_model.py` & `rf-1.1.0/rf/simple_model.py`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/tests/test_batch.py` & `rf-1.1.0/rf/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/tests/test_deconvolve.py` & `rf-1.1.0/rf/tests/test_deconvolve.py`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/tests/test_imaging.py` & `rf-1.1.0/rf/tests/test_imaging.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,14 +31,23 @@
 
     @unittest.skipIf(cartopy is None, 'cartopy not installed')
     def test_plot_ppoints(self):
         from rf.imaging import plot_ppoints
         stream = minimal_example_rf()
         plot_ppoints(stream.ppoints(50), inventory=stream)
 
+    def test_plot_harmonics(self):
+        from rf.imaging import plot_harmonics
+        from rf.harmonics import harmonics
+        stream = minimal_example_rf()
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            harm = harmonics(stream,components='QT',scalars=(1,1))
+        plot_harmonics(harm)
+
 
 def suite():
     return unittest.makeSuite(ImagingTestCase, 'test')
 
 
 if __name__ == '__main__':
     unittest.main(defaultTest='suite')
```

### Comparing `rf-1.0.3/rf/tests/test_profile.py` & `rf-1.1.0/rf/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/tests/test_rfstream.py` & `rf-1.1.0/rf/tests/test_rfstream.py`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/tests/test_simple_model.py` & `rf-1.1.0/rf/tests/test_simple_model.py`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/tests/util.py` & `rf-1.1.0/rf/tests/util.py`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf/util.py` & `rf-1.1.0/rf/util.py`

 * *Files identical despite different names*

### Comparing `rf-1.0.3/rf.egg-info/SOURCES.txt` & `rf-1.1.0/rf.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,44 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 rf/__init__.py
 rf/batch.py
 rf/deconvolve.py
+rf/harmonics.py
 rf/imaging.py
 rf/profile.py
 rf/rfstream.py
 rf/simple_model.py
 rf/util.py
 rf.egg-info/PKG-INFO
 rf.egg-info/SOURCES.txt
 rf.egg-info/dependency_links.txt
 rf.egg-info/entry_points.txt
 rf.egg-info/not-zip-safe
+rf.egg-info/pbr.json
 rf.egg-info/requires.txt
 rf.egg-info/top_level.txt
 rf/data/iasp91.dat
 rf/example/conf.json
 rf/example/example_data.mseed
+rf/example/example_data_old.mseed
 rf/example/example_events.xml
+rf/example/example_events_old.xml
 rf/example/example_inventory.xml
 rf/example/minimal_example.tar.gz
 rf/example/minimal_example_S.tar.gz
+rf/syn/__init__.py
+rf/syn/core.py
+rf/syn/tws.py
 rf/tests/__init__.py
 rf/tests/__main__.py
 rf/tests/test_batch.py
 rf/tests/test_deconvolve.py
+rf/tests/test_harmonics.py
 rf/tests/test_imaging.py
 rf/tests/test_profile.py
 rf/tests/test_rfstream.py
 rf/tests/test_simple_model.py
+rf/tests/test_util.py
 rf/tests/util.py
```

### Comparing `rf-1.0.3/setup.py` & `rf-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,30 +26,26 @@
 
 REQUIRES = ['decorator', 'matplotlib>=2', 'numpy', 'scipy',
             'setuptools', 'obspy>=1.0.3',
             'cartopy', 'geographiclib', 'shapely']
 
 EXTRAS_REQUIRE = {
     'doc': ['sphinx', 'alabaster'],  # and decorator, obspy
-    'deconv_multitaper': ['mtspec'],
+    'deconv_multitaper': ['multitaper'],
     'h5': ['obspyh5>=0.3'],
     'toeplitz': ['toeplitz'],
     'batch': ['tqdm']
     }
 
 CLASSIFIERS = [
     'Environment :: Console',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
     'Topic :: Scientific/Engineering :: Physics'
     ]
 
 
 setup(name='rf',
       version=VERSION,
       description=DESCRIPTION,
```

