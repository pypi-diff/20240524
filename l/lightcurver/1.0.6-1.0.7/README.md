# Comparing `tmp/lightcurver-1.0.6.tar.gz` & `tmp/lightcurver-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcurver-1.0.6.tar", last modified: Wed May  8 15:43:02 2024, max compression
+gzip compressed data, was "lightcurver-1.0.7.tar", last modified: Fri May 24 01:36:48 2024, max compression
```

## Comparing `lightcurver-1.0.6.tar` & `lightcurver-1.0.7.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.340828 lightcurver-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 15:42:52.000000 lightcurver-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-08 15:43:02.340828 lightcurver-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-08 15:42:52.000000 lightcurver-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.332827 lightcurver-1.0.6/lightcurver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.332827 lightcurver-1.0.6/lightcurver/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/pipeline/pipeline_dependency_graph.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/pipeline/state_checkers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/pipeline/task_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/pipeline/workflow_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.336827 lightcurver-1.0.6/lightcurver/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/footprint_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/image_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/normalization_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/psf_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/sources_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/plotting/star_photometry_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.336827 lightcurver-1.0.6/lightcurver/processes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/alternate_plate_solving_with_gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/background_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/cutout_making.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/frame_characterization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/frame_importation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/frame_star_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/normalization_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/plate_solving.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/psf_modelling.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/roi_deconv_file_preparation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/roi_modelling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/star_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    17623 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/star_photometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/processes/star_querying.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.336827 lightcurver-1.0.6/lightcurver/structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16714 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/structure/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/structure/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/structure/user_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/structure/user_header_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.340828 lightcurver-1.0.6/lightcurver/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/chi2_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/footprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/lightcurves_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/star_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/starred_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-08 15:42:52.000000 lightcurver-1.0.6/lightcurver/utilities/zeropoint_from_gaia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:43:02.340828 lightcurver-1.0.6/lightcurver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-08 15:43:02.000000 lightcurver-1.0.6/lightcurver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-08 15:43:02.000000 lightcurver-1.0.6/lightcurver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:43:02.000000 lightcurver-1.0.6/lightcurver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-08 15:43:02.000000 lightcurver-1.0.6/lightcurver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 15:43:02.000000 lightcurver-1.0.6/lightcurver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-08 15:42:52.000000 lightcurver-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:43:02.340828 lightcurver-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:48.102578 lightcurver-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-24 01:36:37.000000 lightcurver-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-24 01:36:48.102578 lightcurver-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-24 01:36:37.000000 lightcurver-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:48.090578 lightcurver-1.0.7/lightcurver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:48.094578 lightcurver-1.0.7/lightcurver/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/pipeline/pipeline_dependency_graph.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/pipeline/state_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/pipeline/task_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/pipeline/workflow_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:48.094578 lightcurver-1.0.7/lightcurver/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/plotting/footprint_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/plotting/image_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/plotting/normalization_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/plotting/psf_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/plotting/sources_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/plotting/star_photometry_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:48.098578 lightcurver-1.0.7/lightcurver/processes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/alternate_plate_solving_with_gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/background_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/cutout_making.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/frame_characterization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13579 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/frame_importation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/frame_star_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/normalization_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/plate_solving.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11077 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/psf_modelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/roi_deconv_file_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13687 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/roi_modelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/star_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18891 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/star_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/processes/star_querying.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:48.098578 lightcurver-1.0.7/lightcurver/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16714 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/structure/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/structure/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/structure/user_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/structure/user_header_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:48.098578 lightcurver-1.0.7/lightcurver/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/utilities/chi2_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/utilities/footprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/utilities/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/utilities/image_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/utilities/lightcurves_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/utilities/star_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/utilities/starred_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-24 01:36:37.000000 lightcurver-1.0.7/lightcurver/utilities/zeropoint_from_gaia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:36:48.098578 lightcurver-1.0.7/lightcurver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-24 01:36:48.000000 lightcurver-1.0.7/lightcurver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-24 01:36:48.000000 lightcurver-1.0.7/lightcurver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:36:48.000000 lightcurver-1.0.7/lightcurver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-24 01:36:48.000000 lightcurver-1.0.7/lightcurver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 01:36:48.000000 lightcurver-1.0.7/lightcurver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-24 01:36:37.000000 lightcurver-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:36:48.102578 lightcurver-1.0.7/setup.cfg
```

### Comparing `lightcurver-1.0.6/LICENSE` & `lightcurver-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/PKG-INFO` & `lightcurver-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurver
-Version: 1.0.6
+Version: 1.0.7
 Summary: A thorough structure for precise photometry and deconvolution of time series of wide field images.
 Author-email: Frédéric Dux <duxfrederic@gmail.com>
 Project-URL: homepage, https://duxfrederic.github.io/lightcurver/
 Project-URL: repository, https://github.com/duxfrederic/lightcurver
 Keywords: photometry,astronomy,deconvolution,PSF,pipeline
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,15 +16,15 @@
 Requires-Dist: scipy
 Requires-Dist: ephem
 Requires-Dist: pandas
 Requires-Dist: shapely
 Requires-Dist: astroquery
 Requires-Dist: h5py
 Requires-Dist: astroscrappy
-Requires-Dist: starred-astro>=1.4.1
+Requires-Dist: starred-astro>=1.4.2
 Requires-Dist: pytest
 Requires-Dist: dill
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: jaxopt
 Requires-Dist: matplotlib
 Requires-Dist: numpy
```

### Comparing `lightcurver-1.0.6/README.md` & `lightcurver-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/pipeline/pipeline_dependency_graph.yaml` & `lightcurver-1.0.7/lightcurver/pipeline/pipeline_dependency_graph.yaml`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/pipeline/state_checkers.py` & `lightcurver-1.0.7/lightcurver/pipeline/state_checkers.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/pipeline/task_wrappers.py` & `lightcurver-1.0.7/lightcurver/pipeline/task_wrappers.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/pipeline/workflow_manager.py` & `lightcurver-1.0.7/lightcurver/pipeline/workflow_manager.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/plotting/footprint_plotting.py` & `lightcurver-1.0.7/lightcurver/plotting/footprint_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/plotting/image_plotting.py` & `lightcurver-1.0.7/lightcurver/plotting/image_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/plotting/normalization_plotting.py` & `lightcurver-1.0.7/lightcurver/plotting/normalization_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/plotting/psf_plotting.py` & `lightcurver-1.0.7/lightcurver/plotting/psf_plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,36 +41,36 @@
     fig, ax = plt.subplots(3, N+1, figsize=((N+1)*sub_size, 3*sub_size))
 
     for i in range(N):
         for j in range(3):
             ax[j, i].axis('off')
             ax[j, i].set_aspect('equal')
             if j == 0:
-                ax[j, i].imshow(datas[i], cmap=cmap)
+                ax[j, i].imshow(datas[i], cmap=cmap, origin='lower')
                 if names is not None:
                     ax[j, i].text(0.5, 0.02, names[i],
                                   horizontalalignment='center',
                                   verticalalignment='bottom',
                                   transform=ax[j, i].transAxes,
                                   color=text_color, fontsize=single_letter_text_size,
                                   weight='bold')
             elif j == 1:
-                ax[j, i].imshow(noisemaps[i], cmap=cmap)
+                ax[j, i].imshow(noisemaps[i], cmap=cmap, origin='lower')
                 ax[j, i].text(0.5, 0.02, 'noisemap, mask',
                               horizontalalignment='center',
                               verticalalignment='bottom',
                               transform=ax[j, i].transAxes,
                               color=text_color, fontsize=text_size,
                               weight='bold')
             elif j == 2:
                 res = np.array(residuals[i])  # explicit casting, jax stuff
                 if masks is not None:
                     mask = np.array(masks[i]).astype(bool)
                     res[np.where(~mask)] = np.nan
-                ax[j, i].imshow(res, cmap=cmap_residuals)
+                ax[j, i].imshow(res, cmap=cmap_residuals, origin='lower')
                 ax[j, i].text(0.5, 0.02, 'residuals',
                               horizontalalignment='center',
                               verticalalignment='bottom',
                               transform=ax[j, i].transAxes,
                               color=text_color, fontsize=text_size,
                               weight='bold')
 
@@ -90,15 +90,15 @@
                       verticalalignment='top',
                       transform=ax[1, N].transAxes,
                       color='white', fontsize=text_size,
                       weight='bold')
 
         ax[1, N].axis('off')
     # psf model plot
-    ax[2, N].imshow(full_psf, cmap=cmap, aspect='auto')
+    ax[2, N].imshow(full_psf, cmap=cmap, aspect='auto', origin='lower')
     ax[2, N].axis('off')
     ax[2, N].text(0.5, 0.01, 'Full PSF',
                   horizontalalignment='center',
                   verticalalignment='bottom',
                   transform=ax[2, N].transAxes,
                   color=text_color, fontsize=text_size,
                   weight='bold')
```

### Comparing `lightcurver-1.0.6/lightcurver/plotting/sources_plotting.py` & `lightcurver-1.0.7/lightcurver/plotting/sources_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/plotting/star_photometry_plotting.py` & `lightcurver-1.0.7/lightcurver/plotting/star_photometry_plotting.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/processes/alternate_plate_solving_with_gaia.py` & `lightcurver-1.0.7/lightcurver/processes/alternate_plate_solving_with_gaia.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/processes/background_estimation.py` & `lightcurver-1.0.7/lightcurver/processes/background_estimation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/processes/cutout_making.py` & `lightcurver-1.0.7/lightcurver/processes/cutout_making.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,31 +22,33 @@
 def extract_stamp(data, header, exptime, sky_coord, cutout_size, background_rms_electron_per_second):
     """
     :param data: 2d numpy array containing the full image
     :param header: fits header for WCS info
     :param exptime: float, exposure time to convert from e-/s to e- and back.
     :param sky_coord: astropy SkyCoord: center of cutout
     :param cutout_size: int, pixels
-    :return: 2d cutout array, 2d cutout noisemap array, wcs string of cutout
+    :return: 2d cutout array, 2d cutout noisemap array, wcs string of cutout, center of cutout in original image (x,y)
     """
 
     wcs = WCS(header)
     data_cutout = Cutout2D(data, sky_coord, cutout_size, wcs=wcs, mode='partial')
     # let's also carry the WCS of the cutouts
     wcs_header = data_cutout.wcs.to_header()
     wcs_header_string = wcs_header.tostring()
+    # in case we need to refer back to the original position of the cutout in the fits file:
+    original_center_position = data_cutout.center_original
 
     # now just take the numpy array
     data_cutout_electrons = exptime * data_cutout.data
 
     noisemap_electrons = ((exptime * background_rms_electron_per_second)**2 + np.abs(data_cutout_electrons))**0.5
     # remove zeros if there are any ...
     noisemap_electrons[noisemap_electrons < 1e-7] = 1e-7
 
-    return data_cutout.data, noisemap_electrons / exptime, wcs_header_string
+    return data_cutout.data, noisemap_electrons / exptime, wcs_header_string, np.array(original_center_position)
 
 
 def extract_all_stamps():
     """
     This is the routine that the workflow manager will call.
     It interfaces with the user config and the database to locate the
     files and objects to extract, then extracts to a hdf5 file.
@@ -103,38 +105,47 @@
             data, header = fits.getdata(image_file), fits.getheader(image_file)
             global_rms = frame['background_rms_electron_per_second']
             # organize hdf5 file
             if frame['image_relpath'] not in reg_f.keys():
                 frame_set = reg_f.create_group(frame['image_relpath'])
             else:
                 frame_set = reg_f[frame['image_relpath']]
+            # keep track of the total shape of the image, so we can rescale image coordinates later,
+            # useful for distortion.
+            if 'frame_shape' not in frame_set:
+                frame_set['frame_shape'] = data.shape
+            # now the "object dependent" parts: needs groups as there will be one entry per extracted object.
             if 'data' not in frame_set.keys():
                 data_set = frame_set.create_group('data')
             else:
                 data_set = frame_set['data']
             if 'noisemap' not in frame_set.keys():
                 noise_set = frame_set.create_group('noisemap')
             else:
                 noise_set = frame_set['noisemap']
             if 'wcs' not in frame_set.keys():
                 wcs_set = frame_set.create_group('wcs')
             else:
                 wcs_set = frame_set['wcs']
+            if 'image_pixel_coordinates' not in frame_set.keys():
+                pixel_coord_set = frame_set.create_group('image_pixel_coordinates')
+            else:
+                pixel_coord_set = frame_set['image_pixel_coordinates']
             if 'cosmicsmask' not in frame_set.keys():
                 cosmic_mask = frame_set.create_group('cosmicsmask')
             else:
                 cosmic_mask = frame_set['cosmicsmask']
 
             if user_config['redo_stamp_extraction'] or ('ROI' not in cosmic_mask.keys()):
                 # extract the ROI -- assuming no proper motion.
-                cutout, noisemap, wcs_str = extract_stamp(data=data, header=header,
-                                                          exptime=frame['exptime'],
-                                                          sky_coord=user_config['ROI_SkyCoord'],
-                                                          cutout_size=user_config['stamp_size_ROI'],
-                                                          background_rms_electron_per_second=global_rms)
+                cutout, noisemap, wcs_str, cutout_center = extract_stamp(data=data, header=header,
+                                                                         exptime=frame['exptime'],
+                                                                         sky_coord=user_config['ROI_SkyCoord'],
+                                                                         cutout_size=user_config['stamp_size_ROI'],
+                                                                         background_rms_electron_per_second=global_rms)
                 # clean the cosmics
                 if user_config['clean_cosmics']:
                     mask, cleaned = detect_cosmics(cutout, invar=noisemap**2)
                 else:
                     mask = np.zeros_like(cutout, dtype=bool)
                     cleaned = cutout
                 if 'ROI' in data_set:
@@ -145,14 +156,17 @@
                 noise_set['ROI'] = noisemap
                 if 'ROI' in wcs_set:
                     del wcs_set['ROI']
                 wcs_set['ROI'] = wcs_str
                 if 'ROI' in cosmic_mask:
                     del cosmic_mask['ROI']
                 cosmic_mask['ROI'] = mask
+                if 'ROI' in pixel_coord_set:
+                    del pixel_coord_set['ROI']
+                pixel_coord_set['ROI'] = cutout_center
 
             # set proper motion to 0 when not available
             if len(stars) > 0:  # if 0 stars, then frame will not be queried downstream.
                 stars.loc[np.isnan(stars['pmra']), 'pmra'] = 0.0
                 stars.loc[np.isnan(stars['pmdec']), 'pmdec'] = 0.0
             elif len(stars) == 0:
                 logger.warning(
@@ -169,19 +183,21 @@
                                           pm_ra_cosdec=star['pmra'] * u.mas / u.yr,
                                           pm_dec=star['pmdec'] * u.mas / u.yr,
                                           frame='icrs',
                                           obstime=Time(star['ref_epoch'], format='decimalyear'))
                     # then correct the proper motion
                     obs_epoch = Time(frame['mjd'], format='mjd')
                     corrected_coord = star_coord.apply_space_motion(new_obstime=obs_epoch)
-                    cutout, noisemap, wcs_str = extract_stamp(data=data, header=header,
-                                                              exptime=frame['exptime'],
-                                                              sky_coord=corrected_coord,
-                                                              cutout_size=user_config['stamp_size_stars'],
-                                                              background_rms_electron_per_second=global_rms)
+                    cutout, noisemap, wcs_str, cutout_center = extract_stamp(
+                        data=data, header=header,
+                        exptime=frame['exptime'],
+                        sky_coord=corrected_coord,
+                        cutout_size=user_config['stamp_size_stars'],
+                        background_rms_electron_per_second=global_rms
+                    )
 
                     # again, clean the cosmics.
                     if user_config['clean_cosmics']:
                         mask, cleaned = detect_cosmics(cutout, invar=noisemap**2)
                     else:
                         mask = np.zeros_like(cutout, dtype=bool)
                         cleaned = cutout
@@ -193,9 +209,12 @@
                     noise_set[star_name] = noisemap
                     if star_name in wcs_set:
                         del wcs_set[star_name]
                     wcs_set[star_name] = wcs_str
                     if star_name in cosmic_mask:
                         del cosmic_mask[star_name]
                     cosmic_mask[star_name] = mask
+                    if star_name in pixel_coord_set:
+                        del pixel_coord_set['ROI']
+                    pixel_coord_set[star_name] = cutout_center
 
             logger.info(f"Frame with id {frame['id']}: completed making of cutouts.")
```

### Comparing `lightcurver-1.0.6/lightcurver/processes/frame_characterization.py` & `lightcurver-1.0.7/lightcurver/processes/frame_characterization.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/processes/frame_importation.py` & `lightcurver-1.0.7/lightcurver/processes/frame_importation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/processes/frame_star_assignment.py` & `lightcurver-1.0.7/lightcurver/processes/frame_star_assignment.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/processes/normalization_calculation.py` & `lightcurver-1.0.7/lightcurver/processes/normalization_calculation.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/processes/plate_solving.py` & `lightcurver-1.0.7/lightcurver/processes/plate_solving.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/processes/psf_modelling.py` & `lightcurver-1.0.7/lightcurver/processes/psf_modelling.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from time import time
 from starred.procedures.psf_routines import build_psf
 
 from ..structure.database import select_stars_for_a_frame, execute_sqlite_query, get_pandas
 from ..structure.user_config import get_user_config
 from ..plotting.psf_plotting import plot_psf_diagnostic
 from ..utilities.footprint import get_combined_footprint_hash
+from ..utilities.image_coordinates import rescale_image_coordinates
 
 
 def check_psf_exists(frame_id, psf_ref, combined_footprint_hash):
     """
     just checks if the PSF in question has already been modelled. (for same frame ID, of the specific combined footprint
     and same name constructed from the stars used in the model).
     Args:
@@ -107,17 +108,23 @@
             continue
 
         # get the cutouts
         with h5py.File(regions_file, 'r') as f:
             data_group = f[f"{frame['image_relpath']}/data"]
             noisemap_group = f[f"{frame['image_relpath']}/noisemap"]
             mask_group = f[f"{frame['image_relpath']}/cosmicsmask"]
+            positions_group = f[f"{frame['image_relpath']}/image_pixel_coordinates"]
             datas = np.array([data_group[gaia_id][...] for gaia_id in list(stars['gaia_id'])])
             noisemaps = np.array([noisemap_group[name][...] for name in list(stars['gaia_id'])])
             cosmics_masks = np.array([mask_group[name][...] for name in list(stars['gaia_id'])]).astype(bool)
+            # stuff related to positions of the cutouts in the frame, for distortion
+            frame_shape = f[f"{frame['image_relpath']}/frame_shape"][...]
+            image_positions = np.array([positions_group[gaia_id][...] for gaia_id in list(stars['gaia_id'])])
+            rescaled_image_positions = rescale_image_coordinates(xy_coordinates_array=image_positions,
+                                                                 image_shape=frame_shape)
             # invert because the cosmics are marked as True, but we want the healthy pixels to be marked as True:
             cosmics_masks = ~cosmics_masks
         # now we'll prepare automatic masks (masking other objects in the field)
         automatic_masks = []
         for data, noisemap in zip(datas, noisemaps):
             mask = mask_surrounding_stars(data, noisemap)
             automatic_masks.append(mask)
@@ -148,20 +155,22 @@
                 f"The frame with id {frame['id']} had {n_stars_before} reference stars, "
                 "but none could be used due to too many masked pixels. Skipping."
             )
             continue
 
         # we set the initial guess for the position of the star to the center (guess_method thing)
         # because we are confident that is where the star will be (plate solving + gaia proper motions)
-        result = build_psf(datas, noisemaps, subsampling_factor=user_config['subsampling_factor'],
+        result = build_psf(image=datas, noisemap=noisemaps, subsampling_factor=user_config['subsampling_factor'],
                            n_iter_analytic=user_config['psf_n_iter_analytic'],
                            n_iter_adabelief=user_config['psf_n_iter_pixels'],
                            masks=masks,
                            guess_method_star_position='center', 
-                           guess_fwhm_pixels=frame['seeing_pixels'])
+                           guess_fwhm_pixels=frame['seeing_pixels'],
+                           field_distortion=user_config['field_distortion'],
+                           stamp_coordinates=rescaled_image_positions)
         psf_plots_dir = user_config['plots_dir'] / 'PSFs' / str(combined_footprint_hash)
         psf_plots_dir.mkdir(exist_ok=True, parents=True)
         frame_name = Path(frame['image_relpath']).stem
         seeing = frame['seeing_pixels'] * frame['pixel_scale']
         loss_history = result['adabelief_extra_fields']['loss_history']
         plot_psf_diagnostic(datas=datas, noisemaps=noisemaps, residuals=result['residuals'],
                             full_psf=result['full_psf'],
@@ -176,30 +185,35 @@
             frame_group = f[frame['image_relpath']]
             if psf_ref in frame_group.keys():
                 del frame_group[psf_ref]
             psf_group = frame_group.create_group(psf_ref)
             psf_group['narrow_psf'] = np.array(result['narrow_psf'])
             psf_group['full_psf'] = np.array(result['full_psf'])
             psf_group['subsampling_factor'] = np.array([user_config['subsampling_factor']])
+            # for distortion, we have kwargs_distortion ~ {'dilation_x': array, 'dilation_y': array, ....}
+            distortion_group = psf_group.create_group('distortion')
+            for key, value in result['kwargs_psf']['kwargs_distortion'].items():
+                distortion_group[key] = value
 
         # and update the database.
         loss_index = int(0.9 * np.array(loss_history).size)
         initial_change = np.nanmax(loss_history[:loss_index]) - np.nanmin(loss_history[:loss_index])
         end_change = np.nanmax(loss_history[loss_index:]) - np.nanmin(loss_history[loss_index:])
         relative_loss_differential = float(end_change / initial_change)
         insert_params = (frame['id'], float(result['chi2']), relative_loss_differential, psf_ref,
                          combined_footprint_hash, user_config['subsampling_factor'])
-        insert_query = "REPLACE INTO PSFs "
-        insert_query += "(frame_id, chi2, relative_loss_differential, psf_ref, combined_footprint_hash, subsampling_factor) "
-        insert_query += f"VALUES ({','.join(['?'] * len(insert_params))})"
-
+        insert_query = f"""
+        REPLACE INTO PSFs 
+        (frame_id, chi2, relative_loss_differential, psf_ref, combined_footprint_hash, subsampling_factor)
+        VALUES ({','.join(['?'] * len(insert_params))})
+        """
         execute_sqlite_query(insert_query, insert_params, is_select=False)
 
         time_taken = time() - t0
         logger.info(
             f"PSF built for frame with id {frame['id']}. "
             f"The reference is {psf_ref}, that is {n_stars_before} stars available, and {n_stars_after} actually used "
             "after filtering of masked pixels. "
-            f"The reduced chi2 is {result['chi2']:.02f}, and it took us {time_taken:.01f} seconds to complete everything. "
+            f"The reduced chi2 is {result['chi2']:.02f}, and it took us {time_taken:.01f} seconds to do everything. "
         )
```

### Comparing `lightcurver-1.0.6/lightcurver/processes/roi_deconv_file_preparation.py` & `lightcurver-1.0.7/lightcurver/processes/roi_deconv_file_preparation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import h5py
 import numpy as np
 import logging
 
+from starred.psf.psf import apply_distortion
+
 from ..structure.database import get_pandas, execute_sqlite_query
 from ..utilities.footprint import get_combined_footprint_hash
 from ..utilities.chi2_selector import get_chi2_bounds
 from ..structure.user_config import get_user_config
+from ..utilities.image_coordinates import rescale_image_coordinates
 
 
 def get_frames_for_roi(combined_footprint_hash, psf_fit_chi2_min, psf_fit_chi2_max,
                        constraints_on_frame_columns_dict, constraints_on_normalization_coeff_dict):
     """
     Retrieves frames and associated PSFs (built with stars of the given footprint)
     provided that those frames have a PSF with a chi2 between psf_fit_chi2_min and psf_fit_chi2_max.
@@ -152,15 +155,29 @@
         normalization_uncertainty = []
         for j, frame in frames.iterrows():
             coefficient = frame['coefficient']
             data.append(h5f[f"{frame['image_relpath']}/data/ROI"][...] / coefficient)
             noisemap.append(h5f[f"{frame['image_relpath']}/noisemap/ROI"][...] / coefficient)
             mask.append(h5f[f"{frame['image_relpath']}/cosmicsmask/ROI"][...])
             psf_ref = frame['psf_ref']
-            psf.append(h5f[f"{frame['image_relpath']}/{psf_ref}/narrow_psf"][...])
+            narrow_psf = h5f[f"{frame['image_relpath']}/{psf_ref}/narrow_psf"][...]
+            # if distortion of the psf ...
+            if user_config['field_distortion']:
+                kwargs_distortion = {}
+                distortion_group = h5f[f"{frame['image_relpath']}/{psf_ref}/distortion"]
+                for key in distortion_group.keys():
+                    kwargs_distortion[key] = distortion_group[key][...]
+                # 2. collect the position of the star in the frame
+                position = h5f[f"{frame['image_relpath']}/image_pixel_coordinates/ROI"][...]
+                frame_shape = h5f[f"{frame['image_relpath']}/frame_shape"]
+                position = rescale_image_coordinates(xy_coordinates_array=position, image_shape=frame_shape)
+                # 3. get the psf at this position
+                narrow_psf = apply_distortion(narrow_psf=narrow_psf, kwargs_distortion=kwargs_distortion,
+                                              star_xy_coordinates=position)
+            psf.append(narrow_psf)
             subsampling_factors.append(h5f[f"{frame['image_relpath']}/{psf_ref}/subsampling_factor"][...])
             seeing.append(frame['seeing_arcseconds'])
             pixel_scale.append(frame['pixel_scale'])
             wcs.append(h5f[f"{frame['image_relpath']}/wcs/ROI"][()])
             exptime.append(frame['exptime'])
             sky_level_electron_per_second.append(frame['sky_level_electron_per_second'])
             mjd.append(frame['mjd'])
```

### Comparing `lightcurver-1.0.6/lightcurver/processes/roi_modelling.py` & `lightcurver-1.0.7/lightcurver/processes/roi_modelling.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/processes/star_extraction.py` & `lightcurver-1.0.7/lightcurver/processes/star_extraction.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/processes/star_photometry.py` & `lightcurver-1.0.7/lightcurver/processes/star_photometry.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 import logging
 from time import time
 from starred.deconvolution.deconvolution import setup_model
 from starred.deconvolution.loss import Loss
 from starred.deconvolution.parameters import ParametersDeconv
 from starred.optim.optimization import Optimizer
 from starred.utils.noise_utils import propagate_noise
+from starred.psf.psf import apply_distortion
 
 from ..structure.database import execute_sqlite_query, select_stars, select_stars_for_a_frame, get_pandas
 from ..structure.user_config import get_user_config
 from ..utilities.chi2_selector import get_chi2_bounds
 from ..utilities.footprint import get_combined_footprint_hash
 from ..utilities.starred_utilities import get_flux_uncertainties
+from ..utilities.image_coordinates import rescale_image_coordinates
 from ..plotting.star_photometry_plotting import plot_joint_deconv_diagnostic
 
 
 def do_one_deconvolution(data, noisemap, psf, subsampling_factor,
                          n_iter=2000, uniform_background_per_epoch=False, starlet_global_background=True):
     """
     Joint 'deconvolution' of N stamps of a star (in data), with noisemap, and associated PSF at each slice.
@@ -276,15 +278,32 @@
                 # we need to reconstruct which stars were used in the psf given our
                 # accepted stars in 'stars_to_use_psf'.
                 stars_psf = select_stars_for_a_frame(frame_id=frame['id'],
                                                      stars_to_use=user_config['stars_to_use_psf'],
                                                      combined_footprint_hash=combined_footprint_hash)
                 psf_ref = 'psf_' + ''.join(sorted(stars_psf['name']))
                 mask.append(h5f[f"{frame['image_relpath']}/cosmicsmask/{star['gaia_id']}"][...])
-                psf.append(h5f[f"{frame['image_relpath']}/{psf_ref}/narrow_psf"][...])
+                narrow_psf = h5f[f"{frame['image_relpath']}/{psf_ref}/narrow_psf"][...]
+
+                # if we wish to account for distortion, then ...more steps!
+                # 1. collect the distortion keywords
+                if user_config['field_distortion']:
+                    kwargs_distortion = {}
+                    distortion_group = h5f[f"{frame['image_relpath']}/{psf_ref}/distortion"]
+                    for key in distortion_group.keys():
+                        kwargs_distortion[key] = distortion_group[key][...]
+                    # 2. collect the position of the star in the frame
+                    position = h5f[f"{frame['image_relpath']}/image_pixel_coordinates/{star['gaia_id']}"][...]
+                    frame_shape = h5f[f"{frame['image_relpath']}/frame_shape"]
+                    position = rescale_image_coordinates(xy_coordinates_array=position, image_shape=frame_shape)
+                    # 3. get the psf at this position
+                    narrow_psf = apply_distortion(narrow_psf=narrow_psf, kwargs_distortion=kwargs_distortion,
+                                                  star_xy_coordinates=position)
+                # psf ready, distortion or not
+                psf.append(narrow_psf)
             data, noisemap, mask, psf = np.array(data), np.array(noisemap), np.array(mask), np.array(psf)
             # just like for the PSF, we need to remove the NaNs ...
             isnan = np.where(np.isnan(data) * np.isnan(noisemap))
             data[isnan] = 0.
             noisemap[isnan] = 1e7
             # cosmics: masks are 'true' where cosmic, and we typically want it to "true" for good pixels
             mask = ~(np.array(mask).astype(bool))  # so we invert it.
```

### Comparing `lightcurver-1.0.6/lightcurver/processes/star_querying.py` & `lightcurver-1.0.7/lightcurver/processes/star_querying.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/structure/database.py` & `lightcurver-1.0.7/lightcurver/structure/database.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/structure/user_config.py` & `lightcurver-1.0.7/lightcurver/structure/user_config.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/structure/user_header_parser.py` & `lightcurver-1.0.7/lightcurver/structure/user_header_parser.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/utilities/chi2_selector.py` & `lightcurver-1.0.7/lightcurver/utilities/chi2_selector.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/utilities/footprint.py` & `lightcurver-1.0.7/lightcurver/utilities/footprint.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/utilities/gaia.py` & `lightcurver-1.0.7/lightcurver/utilities/gaia.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/utilities/lightcurves_postprocessing.py` & `lightcurver-1.0.7/lightcurver/utilities/lightcurves_postprocessing.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/utilities/star_naming.py` & `lightcurver-1.0.7/lightcurver/utilities/star_naming.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/utilities/starred_utilities.py` & `lightcurver-1.0.7/lightcurver/utilities/starred_utilities.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver/utilities/zeropoint_from_gaia.py` & `lightcurver-1.0.7/lightcurver/utilities/zeropoint_from_gaia.py`

 * *Files identical despite different names*

### Comparing `lightcurver-1.0.6/lightcurver.egg-info/PKG-INFO` & `lightcurver-1.0.7/lightcurver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightcurver
-Version: 1.0.6
+Version: 1.0.7
 Summary: A thorough structure for precise photometry and deconvolution of time series of wide field images.
 Author-email: Frédéric Dux <duxfrederic@gmail.com>
 Project-URL: homepage, https://duxfrederic.github.io/lightcurver/
 Project-URL: repository, https://github.com/duxfrederic/lightcurver
 Keywords: photometry,astronomy,deconvolution,PSF,pipeline
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,15 +16,15 @@
 Requires-Dist: scipy
 Requires-Dist: ephem
 Requires-Dist: pandas
 Requires-Dist: shapely
 Requires-Dist: astroquery
 Requires-Dist: h5py
 Requires-Dist: astroscrappy
-Requires-Dist: starred-astro>=1.4.1
+Requires-Dist: starred-astro>=1.4.2
 Requires-Dist: pytest
 Requires-Dist: dill
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: jaxopt
 Requires-Dist: matplotlib
 Requires-Dist: numpy
```

### Comparing `lightcurver-1.0.6/lightcurver.egg-info/SOURCES.txt` & `lightcurver-1.0.7/lightcurver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 ./lightcurver/structure/exceptions.py
 ./lightcurver/structure/user_config.py
 ./lightcurver/structure/user_header_parser.py
 ./lightcurver/utilities/__init__.py
 ./lightcurver/utilities/chi2_selector.py
 ./lightcurver/utilities/footprint.py
 ./lightcurver/utilities/gaia.py
+./lightcurver/utilities/image_coordinates.py
 ./lightcurver/utilities/lightcurves_postprocessing.py
 ./lightcurver/utilities/star_naming.py
 ./lightcurver/utilities/starred_utilities.py
 ./lightcurver/utilities/zeropoint_from_gaia.py
 lightcurver.egg-info/PKG-INFO
 lightcurver.egg-info/SOURCES.txt
 lightcurver.egg-info/dependency_links.txt
```

### Comparing `lightcurver-1.0.6/pyproject.toml` & `lightcurver-1.0.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.6.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lightcurver"
-version = "1.0.6"
+version = "1.0.7"
 authors = [{ name = "Frédéric Dux", email = "duxfrederic@gmail.com" }]
 description = "A thorough structure for precise photometry and deconvolution of time series of wide field images."
 readme = "README.md"
 keywords = ["photometry", "astronomy", "deconvolution", "PSF", "pipeline"]  
 classifiers = [] 
 dependencies = [
     "pyyaml",
@@ -19,15 +19,15 @@
     "scipy",
     "ephem",
     "pandas",
     "shapely",
     "astroquery",
     "h5py",
     "astroscrappy",
-    "starred-astro >= 1.4.1", 
+    "starred-astro >= 1.4.2", 
     "pytest",
     "dill",
     "jax",
     "jaxlib",
     "jaxopt",
     "matplotlib",
     "numpy",
```

