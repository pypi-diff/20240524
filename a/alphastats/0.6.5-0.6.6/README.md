# Comparing `tmp/alphastats-0.6.5.tar.gz` & `tmp/alphastats-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphastats-0.6.5.tar", last modified: Mon Aug 21 14:05:35 2023, max compression
+gzip compressed data, was "alphastats-0.6.6.tar", last modified: Fri May 24 13:15:46 2024, max compression
```

## Comparing `alphastats-0.6.5.tar` & `alphastats-0.6.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.721802 alphastats-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-08-21 14:05:04.000000 alphastats-0.6.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-21 14:05:04.000000 alphastats-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-08-21 14:05:35.721802 alphastats-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-08-21 14:05:04.000000 alphastats-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.705802 alphastats-0.6.5/alphastats/
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/DataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (123)    13960 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/DataSet_Plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12583 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/DataSet_Preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/DataSet_Statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.705802 alphastats-0.6.5/alphastats/data/
--rw-r--r--   0 runner    (1001) docker     (123)    70534 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/data/contaminations.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.705802 alphastats-0.6.5/alphastats/gui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.705802 alphastats-0.6.5/alphastats/gui/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/AlphaPeptStats.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/alphapeptstats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30529 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/alphastats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    20433 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/alphastats_logo_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.705802 alphastats-0.6.5/alphastats/gui/pages/
--rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/pages/02_Import Data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/pages/03_Data Overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/pages/03_Preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/pages/04_Analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/pages/06_Results.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.709802 alphastats-0.6.5/alphastats/gui/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/sample_data/metadata.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)  9509624 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/sample_data/proteinGroups.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.717802 alphastats-0.6.5/alphastats/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/utils/analysis_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/utils/software_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/gui/utils/ui_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/load_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.721802 alphastats-0.6.5/alphastats/loader/
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/loader/AlphaPeptLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/loader/BaseLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/loader/DIANNLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/loader/FragPipeLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/loader/GenericLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/loader/MaxQuantLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/loader/SpectronautLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/loader/mzTabLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.721802 alphastats-0.6.5/alphastats/multicova/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/multicova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29725 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/multicova/multicova.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.721802 alphastats-0.6.5/alphastats/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/plots/ClusterMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/plots/DimensionalityReduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/plots/IntensityPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/plots/PlotUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/plots/SampleHistogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/plots/VolcanoPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.721802 alphastats-0.6.5/alphastats/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/statistics/Anova.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/statistics/DifferentialExpressionAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/statistics/MultiCovaAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/statistics/StatisticUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-08-21 14:05:04.000000 alphastats-0.6.5/alphastats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.705802 alphastats-0.6.5/alphastats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-08-21 14:05:35.000000 alphastats-0.6.5/alphastats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-08-21 14:05:35.000000 alphastats-0.6.5/alphastats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-21 14:05:35.000000 alphastats-0.6.5/alphastats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-21 14:05:35.000000 alphastats-0.6.5/alphastats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-21 14:05:35.000000 alphastats-0.6.5/alphastats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-21 14:05:35.000000 alphastats-0.6.5/alphastats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-21 14:05:35.721802 alphastats-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-08-21 14:05:04.000000 alphastats-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-21 14:05:35.721802 alphastats-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    37339 2023-08-21 14:05:04.000000 alphastats-0.6.5/tests/test_DataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-08-21 14:05:04.000000 alphastats-0.6.5/tests/test_DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-08-21 14:05:04.000000 alphastats-0.6.5/tests/test_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.665721 alphastats-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-24 13:15:20.000000 alphastats-0.6.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-24 13:15:20.000000 alphastats-0.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-24 13:15:46.665721 alphastats-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-05-24 13:15:20.000000 alphastats-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.645721 alphastats-0.6.6/alphastats/
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19551 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/DataSet_Plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13426 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/DataSet_Preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/DataSet_Statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.645721 alphastats-0.6.6/alphastats/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    70534 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/data/contaminations.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.649721 alphastats-0.6.6/alphastats/gui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.649721 alphastats-0.6.6/alphastats/gui/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/AlphaPeptStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31042 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/alphapeptstats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30529 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/alphastats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20433 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/alphastats_logo_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.649721 alphastats-0.6.6/alphastats/gui/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    14532 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/pages/02_Import Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/pages/03_Data Overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/pages/03_Preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/pages/04_Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/pages/06_Results.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.649721 alphastats-0.6.6/alphastats/gui/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    26661 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/sample_data/metadata.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)  9509624 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/sample_data/proteinGroups.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.661721 alphastats-0.6.6/alphastats/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/utils/analysis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/utils/software_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/gui/utils/ui_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.661721 alphastats-0.6.6/alphastats/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/AlphaPeptLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/BaseLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/DIANNLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/FragPipeLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/GenericLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/MaxQuantLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/SpectronautLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/loader/mzTabLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.661721 alphastats-0.6.6/alphastats/multicova/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/multicova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29725 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/multicova/multicova.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.665721 alphastats-0.6.6/alphastats/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/ClusterMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/DimensionalityReduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/IntensityPlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/PlotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/SampleHistogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13581 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/VolcanoPlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.665721 alphastats-0.6.6/alphastats/statistics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/statistics/Anova.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/statistics/DifferentialExpressionAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/statistics/MultiCovaAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/statistics/StatisticUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-24 13:15:20.000000 alphastats-0.6.6/alphastats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.665721 alphastats-0.6.6/alphastats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 13:15:46.000000 alphastats-0.6.6/alphastats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:15:46.665721 alphastats-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-24 13:15:20.000000 alphastats-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:15:46.665721 alphastats-0.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    37650 2024-05-24 13:15:20.000000 alphastats-0.6.6/tests/test_DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-24 13:15:20.000000 alphastats-0.6.6/tests/test_DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-05-24 13:15:20.000000 alphastats-0.6.6/tests/test_loaders.py
```

### Comparing `alphastats-0.6.5/LICENSE.txt` & `alphastats-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/PKG-INFO` & `alphastats-0.6.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.6.5
+Version: 0.6.6
 Summary: An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
@@ -16,14 +16,39 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pandas==2.0.2
+Requires-Dist: scikit-learn==1.2.2
+Requires-Dist: data_cache>=0.1.6
+Requires-Dist: plotly==5.15.0
+Requires-Dist: statsmodels==0.14.0
+Requires-Dist: sklearn_pandas==2.2.0
+Requires-Dist: pingouin==0.5.3
+Requires-Dist: scipy==1.10.1
+Requires-Dist: tqdm>=4.64.0
+Requires-Dist: diffxpy==0.7.4
+Requires-Dist: anndata==0.9.1
+Requires-Dist: umap-learn==0.5.3
+Requires-Dist: streamlit==1.22.0
+Requires-Dist: tables==3.7.0
+Requires-Dist: numpy==1.23.5
+Requires-Dist: numba==0.56.4
+Requires-Dist: numba-stats==0.5.0
+Requires-Dist: swifter==1.2.0
+Requires-Dist: click==8.0.1
+Requires-Dist: kaleido==0.2.1
+Requires-Dist: combat==0.3.3
+Requires-Dist: xlsxwriter==3.1.0
+Requires-Dist: pyteomics==4.6.0
+Requires-Dist: openpyxl>=3.0.10
+Requires-Dist: nbformat>=5.0
 
 [![PyPI version](https://badge.fury.io/py/alphastats.svg)](https://badge.fury.io/py/alphastats)
 [![codecov](https://codecov.io/gh/MannLabs/alphastats/branch/main/graph/badge.svg?token=HY4A0KKLRI)](https://codecov.io/gh/MannLabs/alphastats)
 [![Downloads](https://static.pepy.tech/badge/alphastats)](https://pepy.tech/project/alphastats)
 [![Downloads](https://static.pepy.tech/badge/alphastats/week)](https://pepy.tech/project/alphastats)
 [![CI](https://github.com/MannLabs/alphapeptstats/actions/workflows/python-package.yml/badge.svg)](https://github.com/MannLabs/alphapeptstats/actions/workflows/python-package.yml)
 [![Documentation Status](https://readthedocs.org/projects/alphapeptstats/badge/?version=latest)](https://alphapeptstats.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `alphastats-0.6.5/README.md` & `alphastats-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/DataSet.py` & `alphastats-0.6.6/alphastats/DataSet.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/DataSet_Pathway.py` & `alphastats-0.6.6/alphastats/DataSet_Pathway.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/DataSet_Plot.py` & `alphastats-0.6.6/alphastats/DataSet_Plot.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/DataSet_Preprocess.py` & `alphastats-0.6.6/alphastats/DataSet_Preprocess.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from random import random
-import pandas as pd
-import sklearn
+import itertools
 import logging
+
 import numpy as np
+import pandas as pd
+import sklearn
 import sklearn.ensemble
 import sklearn.impute
-from alphastats.utils import ignore_warning
-from sklearn.experimental import enable_iterative_imputer
-import itertools
+import streamlit as st
 
+from sklearn.experimental import enable_iterative_imputer #noqa
+from alphastats.utils import ignore_warning
 
 
 class Preprocess:
     def _remove_sampels(self, sample_list: list):
         # exclude samples for analysis
         self.mat = self.mat.drop(sample_list)
         self.metadata = self.metadata[~self.metadata[self.sample].isin(sample_list)]
@@ -26,53 +27,66 @@
         return self.mat[self.mat.index.isin(self.metadata[self.sample].tolist())]
 
     def preprocess_print_info(self):
         """Print summary of preprocessing steps"""
         print(pd.DataFrame(self.preprocessing_info.items()))
 
     def _remove_na_values(self, cut_off):
+        if (
+            self.preprocessing_info.get("Missing values were removed")
+            and self.preprocessing_info.get("Data completeness cut-off") == cut_off
+        ):
+            logging.info("Missing values have already been filtered.")
+            st.warning(
+                "Missing values have already been filtered. To apply another cutoff, reset preprocessing."
+            )
+            return
         cut = 1 - cut_off
-        limit = self.mat.shape[0] * cut
-        
+
+        num_samples, num_proteins = self.mat.shape
+        limit = num_samples * cut
+
+        self.mat.replace(0, np.nan, inplace=True)
         keep_list = list()
         invalid = 0
         for column_name in self.mat.columns:
             column = self.mat[column_name]
-            # Get the count of Zeros in column 
-            count = (column == 0).sum()
+            count = column.isna().sum()
             try:
                 count = count.item()
                 if isinstance(count, int):
                     if count < limit:
                         keep_list += [column_name]
-                    
+
             except ValueError:
-                invalid +=1
+                invalid += 1
                 continue
-        
-        self.mat= self.mat[keep_list]
+        self.mat = self.mat[keep_list]
+
         self.preprocessing_info.update(
-            {"Data completeness cut-off": cut_off}
+            {
+                "Number of removed ProteinGroups due to data completeness cutoff": num_proteins
+                - self.mat.shape[1],
+                "Missing values were removed": True,
+                "Data completeness cut-off": cut_off,
+            }
         )
-        percentage = cut_off * 100
-        print(f"Proteins with a data completeness across all samples of less than {percentage} % have been removed.")
-
 
     def _filter(self):
         if len(self.filter_columns) == 0:
             logging.info("No columns to filter.")
             return
 
-        if self.preprocessing_info.get("Contaminations have been removed") == True:
+        if self.preprocessing_info.get("Contaminations have been removed"):
             logging.info("Contaminatons have already been filtered.")
             return
 
         #  print column names with contamination
         protein_groups_to_remove = self.rawinput[
-            (self.rawinput[self.filter_columns] == True).any(axis=1)
+            self.rawinput[self.filter_columns].any(axis=1)
         ][self.index_column].tolist()
 
         protein_groups_to_remove = list(
             set(protein_groups_to_remove) & set(self.mat.columns.to_list())
         )
 
         # remove columns with protein groups
@@ -101,164 +115,173 @@
         protein_group_na = self.mat.columns[self.mat.isna().all()].tolist()
 
         if len(protein_group_na) > 0:
             self.mat = self.mat.drop(protein_group_na, axis=1)
             logging.info(
                 f" {len(protein_group_na)} Protein Groups were removed due to missing values."
             )
-
         logging.info("Imputing data...")
 
         if method == "mean":
-            imp = sklearn.impute.SimpleImputer(missing_values=np.nan, strategy="mean", keep_empty_features=True)
+            imp = sklearn.impute.SimpleImputer(
+                missing_values=np.nan, strategy="mean", keep_empty_features=True
+            )
             imputation_array = imp.fit_transform(self.mat.values)
 
         elif method == "median":
-            imp = sklearn.impute.SimpleImputer(missing_values=np.nan, strategy="median", keep_empty_features=True)
+            imp = sklearn.impute.SimpleImputer(
+                missing_values=np.nan, strategy="median", keep_empty_features=True
+            )
             imputation_array = imp.fit_transform(self.mat.values)
 
         elif method == "knn":
             # change for text
             method = "k-Nearest Neighbor"
             imp = sklearn.impute.KNNImputer(n_neighbors=2, weights="uniform")
             imputation_array = imp.fit_transform(self.mat.values)
 
         elif method == "randomforest":
-            randomforest = sklearn.ensemble.RandomForestRegressor(
-                max_depth=10,
-                bootstrap=True,
-                max_samples=0.5,
-                n_jobs=2,
-                random_state=0,
-                verbose=0,  #  random forest takes a while print progress
+            imp = sklearn.ensemble.HistGradientBoostingRegressor(
+                max_depth=10, max_iter=100, random_state=0
             )
-            imp = sklearn.impute.IterativeImputer(
-                random_state=0, estimator=randomforest
-            )
-
-            # the random forest imputer doesnt work with float32/float16..
-            #  so the values are multiplied and converted to integers
-            array_multi_mio = self.mat.values * 1000000
-            array_int = array_multi_mio.astype("int")
-
-            imputation_array = imp.fit_transform(array_int)
-            imputation_array = imputation_array / 1000000
+            imp = sklearn.impute.IterativeImputer(random_state=0, estimator=imp)
+            imputation_array = imp.fit_transform(self.mat.values)
 
         else:
             raise ValueError(
                 "Imputation method: {method} is invalid."
                 "Choose 'mean'. 'median', 'knn' (for k-nearest Neighbors) or "
                 "'randomforest' for random forest imputation."
             )
 
         self.mat = pd.DataFrame(
             imputation_array, index=self.mat.index, columns=self.mat.columns
         )
         self.preprocessing_info.update({"Imputation": method})
 
+    def _linear_normalization(self, dataframe: pd.DataFrame):
+        """Normalize data using l2 norm without breaking when encoutering nones
+        l2 = sqrt(sum(x**2))
+
+        Args:
+            dataframe (pd.DataFrame): dataframe to normalize
+
+        Returns:
+            np.array: normalized np.array
+        """
+        square_sum_per_row = dataframe.pow(2).sum(axis=1, skipna=True)
+
+        l2_norms = np.sqrt(square_sum_per_row)
+        normalized_vals = dataframe.div(l2_norms.replace(0, 1), axis=0)
+        return normalized_vals.values
+
     @ignore_warning(UserWarning)
     @ignore_warning(RuntimeWarning)
     def _normalization(self, method: str):
-
         if method == "zscore":
             scaler = sklearn.preprocessing.StandardScaler()
-            normalized_array = scaler.fit_transform(self.mat.values)
+            normalized_array = scaler.fit_transform(
+                self.mat.values.transpose()
+            ).transpose()
 
         elif method == "quantile":
             qt = sklearn.preprocessing.QuantileTransformer(random_state=0)
-            normalized_array = qt.fit_transform(self.mat.values)
+            normalized_array = qt.fit_transform(self.mat.values.transpose()).transpose()
 
         elif method == "linear":
-            normalized_array = sklearn.preprocessing.normalize(
-                self.mat.values, norm="l2"
-            )
+            normalized_array = self._linear_normalization(self.mat)
 
         elif method == "vst":
-            scaler = sklearn.preprocessing.PowerTransformer(standardize=False)
-            normalized_array = scaler.fit_transform(self.mat.values)
+            minmax = sklearn.preprocessing.MinMaxScaler()
+            scaler = sklearn.preprocessing.PowerTransformer()
+            minmaxed_array = minmax.fit_transform(self.mat.values.transpose())
+            normalized_array = scaler.fit_transform(minmaxed_array).transpose()
 
         else:
             raise ValueError(
                 "Normalization method: {method} is invalid"
                 "Choose from 'zscore', 'quantile', 'linear' normalization. or 'vst' for variance stabilization transformation"
             )
 
         self.mat = pd.DataFrame(
             normalized_array, index=self.mat.index, columns=self.mat.columns
         )
 
         self.preprocessing_info.update({"Normalization": method})
 
     def reset_preprocessing(self):
-        """ Reset all preprocessing steps
-        """
-        #  reset all preprocessing steps
+        """Reset all preprocessing steps"""
         self.create_matrix()
         print("All preprocessing steps are reset.")
-    
+
     @ignore_warning(RuntimeWarning)
     def _compare_preprocessing_modes(self, func, params_for_func) -> list:
         dataset = self
         imputation_methods = ["mean", "median", "knn", "randomforest"]
-        normalization_methods = ["vst","zscore", "quantile" ]
-        
-        preprocessing_modes = list(itertools.product(normalization_methods, imputation_methods))
+        normalization_methods = ["vst", "zscore", "quantile"]
 
+        preprocessing_modes = list(
+            itertools.product(normalization_methods, imputation_methods)
+        )
 
         results_list = []
 
         del params_for_func["compare_preprocessing_modes"]
         params_for_func["dataset"] = params_for_func.pop("self")
 
         for preprocessing_mode in preprocessing_modes:
             # reset preprocessing
             dataset.reset_preprocessing()
-            print(f"Normalization {preprocessing_mode[0]}, Imputation {str(preprocessing_mode[1])}")
+            print(
+                f"Normalization {preprocessing_mode[0]}, Imputation {str(preprocessing_mode[1])}"
+            )
             dataset.mat.replace([np.inf, -np.inf], np.nan, inplace=True)
 
             dataset.preprocess(
                 subset=True,
                 normalization=preprocessing_mode[0],
                 imputation=preprocessing_mode[1],
             )
 
             res = func(**params_for_func)
             results_list.append(res)
-        
+
             print("\t")
 
         return results_list
 
     def _log2_transform(self):
         self.mat = np.log2(self.mat + 0.1)
         self.preprocessing_info.update({"Log2-transformed": True})
         print("Data has been log2-transformed.")
-    
-    def batch_correction(self, batch:str):
+
+    def batch_correction(self, batch: str):
         """Correct for technical bias/batch effects
         Behdenna A, Haziza J, Azencot CA and Nordor A. (2020) pyComBat, a Python tool for batch effects correction in high-throughput molecular data using empirical Bayes methods. bioRxiv doi: 10.1101/2020.03.17.995431
         Args:
             batch (str): column name in the metadata describing the different batches
         """
-        import combat
         from combat.pycombat import pycombat
+
         data = self.mat.transpose()
-        series_of_batches = self.metadata.set_index(self.sample).reindex(data.columns.to_list())[batch]
+        series_of_batches = self.metadata.set_index(self.sample).reindex(
+            data.columns.to_list()
+        )[batch]
         self.mat = pycombat(data=data, batch=series_of_batches).transpose()
 
     @ignore_warning(RuntimeWarning)
     def preprocess(
         self,
-        log2_transform: bool=True,
-        remove_contaminations: bool=False,
-        subset: bool=False,
-        data_completeness: float=0,
-        normalization: str=None,
-        imputation: str=None,
-        remove_samples: list=None,
+        log2_transform: bool = True,
+        remove_contaminations: bool = False,
+        subset: bool = False,
+        data_completeness: float = 0,
+        normalization: str = None,
+        imputation: str = None,
+        remove_samples: list = None,
     ):
         """Preprocess Protein data
 
         Removal of contaminations:
 
         Removes all observations, that were identified as contaminations.
 
@@ -296,30 +319,34 @@
             data_completeness (float, optional): data completeness across all samples between 0-1. Defaults to 0.
             remove_samples (list, optional): list with sample ids to remove. Defaults to None.
             imputation (str, optional):  method to impute data: either "mean", "median", "knn" or "randomforest". Defaults to None.
             subset (bool, optional): filter matrix so only samples that are described in metadata found in matrix. Defaults to False.
         """
         if remove_contaminations:
             self._filter()
-        
+
         if remove_samples is not None:
             self._remove_sampels(sample_list=remove_samples)
 
         if subset:
             self.mat = self._subset()
-        
 
-        if data_completeness> 0:
+        if data_completeness > 0:
             self._remove_na_values(cut_off=data_completeness)
 
         if log2_transform and self.preprocessing_info.get("Log2-transformed") is False:
             self._log2_transform()
 
         if normalization is not None:
             self._normalization(method=normalization)
             self.mat = self.mat.replace([np.inf, -np.inf], np.nan)
-            
+
         if imputation is not None:
             self._imputation(method=imputation)
 
         self.mat = self.mat.loc[:, (self.mat != 0).any(axis=0)]
+        self.preprocessing_info.update(
+            {
+                "Matrix: Number of ProteinIDs/ProteinGroups": self.mat.shape[1],
+            }
+        )
         self.preprocessed = True
```

### Comparing `alphastats-0.6.5/alphastats/DataSet_Statistics.py` & `alphastats-0.6.6/alphastats/DataSet_Statistics.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/__init__.py` & `alphastats-0.6.6/alphastats/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __project__ = "alphastats"
-__version__ = "0.6.5"
+__version__ = "0.6.6"
 __license__ = "Apache"
 __description__ = "An open-source Python package for Mass Spectrometry Analysis"
 __author__ = "Mann Labs"
 __author_email__ = "elena.krismer@hotmail.com"
 __github__ = "https://github.com/MannLabs/alphapeptstats"
 __keywords__ = [
     "bioinformatics",
```

### Comparing `alphastats-0.6.5/alphastats/data/contaminations.txt` & `alphastats-0.6.6/alphastats/data/contaminations.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/.streamlit/config.toml` & `alphastats-0.6.6/alphastats/gui/.streamlit/config.toml`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/AlphaPeptStats.py` & `alphastats-0.6.6/alphastats/gui/AlphaPeptStats.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/alphapeptstats_logo.png` & `alphastats-0.6.6/alphastats/gui/alphapeptstats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/alphastats_logo.png` & `alphastats-0.6.6/alphastats/gui/alphastats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/alphastats_logo_2.png` & `alphastats-0.6.6/alphastats/gui/alphastats_logo_2.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/gui.py` & `alphastats-0.6.6/alphastats/gui/gui.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/pages/02_Import Data.py` & `alphastats-0.6.6/alphastats/gui/pages/02_Import Data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,119 +1,128 @@
-import streamlit as st
-import sys
-import os
 import io
+import os
+
+import streamlit as st
 
 try:
-    from alphastats.gui.utils.ui_helper import sidebar_info
-    from alphastats.gui.utils.analysis_helper import *
+    from alphastats.DataSet import DataSet
+    from alphastats.gui.utils.analysis_helper import (
+        get_sample_names_from_software_file,
+        read_uploaded_file_into_df,
+    )
     from alphastats.gui.utils.software_options import software_options
+    from alphastats.gui.utils.ui_helper import sidebar_info
     from alphastats.loader.MaxQuantLoader import MaxQuantLoader
-    from alphastats.DataSet import DataSet
 
 except ModuleNotFoundError:
     from utils.ui_helper import sidebar_info
-    from utils.analysis_helper import *
+    from utils.analysis_helper import (
+        get_sample_names_from_software_file,
+        read_uploaded_file_into_df,
+    )
     from utils.software_options import software_options
     from alphastats import MaxQuantLoader
     from alphastats import DataSet
 
-
 import pandas as pd
 import plotly.express as px
-
 from streamlit.runtime import get_instance
 from streamlit.runtime.scriptrunner.script_run_context import get_script_run_ctx
 
 runtime = get_instance()
 session_id = get_script_run_ctx().session_id
 session_info = runtime._session_mgr.get_session_info(session_id)
 
 user_session_id = session_id
 st.session_state["user_session_id"] = user_session_id
 
 if "loader" not in st.session_state:
     st.session_state["loader"] = None
 
+if "gene_to_prot_id" not in st.session_state:
+    st.session_state["gene_to_prot_id"] = {}
 
-def load_options():
+if "organism" not in st.session_state:
+    st.session_state["organism"] = 9606 # human
 
+
+def load_options():
     from alphastats.gui.utils.options import plotting_options, statistic_options
 
     st.session_state["plotting_options"] = plotting_options
     st.session_state["statistic_options"] = statistic_options
 
 
 def check_software_file(df, software):
     """
     check if software files are in right format
     can be fragile when different settings are used or software is updated
     """
 
     if software == "MaxQuant":
         expected_columns = ["Protein IDs", "Reverse", "Potential contaminant"]
-        if (set(expected_columns).issubset(set(df.columns.to_list()))) == False:
+        if not set(expected_columns).issubset(set(df.columns.to_list())):
             st.error(
                 "This is not a valid MaxQuant file. Please check:"
                 "http://www.coxdocs.org/doku.php?id=maxquant:table:proteingrouptable"
             )
 
     elif software == "AlphaPept":
         if "object" in df.iloc[:, 1:].dtypes.to_list():
             st.error("This is not a valid AlphaPept file.")
 
     elif software == "DIANN":
         expected_columns = [
             "Protein.Group",
         ]
 
-        if (set(expected_columns).issubset(set(df.columns.to_list()))) == False:
+        if not set(expected_columns).issubset(set(df.columns.to_list())):
             st.error("This is not a valid DIA-NN file.")
 
     elif software == "Spectronaut":
         expected_columns = [
             "PG.ProteinGroups",
         ]
 
-        if (set(expected_columns).issubset(set(df.columns.to_list()))) == False:
+        if not set(expected_columns).issubset(set(df.columns.to_list())):
             st.error("This is not a valid Spectronaut file.")
 
     elif software == "FragPipe":
         expected_columns = ["Protein"]
-        if (set(expected_columns).issubset(set(df.columns.to_list()))) == False:
+        if not set(expected_columns).issubset(set(df.columns.to_list())):
             st.error(
                 "This is not a valid FragPipe file. Please check:"
                 "https://fragpipe.nesvilab.org/docs/tutorial_fragpipe_outputs.html#combined_proteintsv"
             )
 
-def select_columns_for_loaders(software, software_df:None):
+
+def select_columns_for_loaders(software, software_df: None):
     """
     select intensity and index column depending on software
     will be saved in session state
     """
     st.write("\n\n")
     st.markdown("### 2. Select columns used for further analysis.")
     st.markdown("Select intensity columns for further analysis")
 
     if software != "Other":
-
         st.selectbox(
             "Intensity Column",
             options=software_options.get(software).get("intensity_column"),
             key="intensity_column",
         )
 
         st.markdown("Select index column (with ProteinGroups) for further analysis")
 
         st.selectbox(
             "Index Column",
             options=software_options.get(software).get("index_column"),
             key="index_column",
         )
-        
+
     else:
         st.multiselect(
             "Intensity Columns",
             options=software_df.columns.to_list(),
             key="intensity_column",
         )
 
@@ -145,35 +154,38 @@
     if len(valid_sample_columns) == 0:
         st.error(
             f"Metadata does not match Proteomics data."
             f"Information for the samples: {samples_proteomics_data} is required."
         )
 
     st.write(
-        f"Select column that contains sample IDs matching the sample names described "
+        "Select column that contains sample IDs matching the sample names described "
         + f"in {software_options.get(software).get('import_file')}"
     )
 
     with st.form("sample_column"):
         st.selectbox("Sample Column", options=valid_sample_columns, key="sample_column")
         submitted = st.form_submit_button("Create DataSet")
 
     if submitted:
+        if len(df[st.session_state.sample_column].to_list()) != len(
+            df[st.session_state.sample_column].unique()
+        ):
+            st.error("Sample names have to be unique.")
+            st.stop()
         return True
 
 
 def upload_softwarefile(software):
-
     softwarefile = st.file_uploader(
         software_options.get(software).get("import_file"),
         type=["csv", "tsv", "txt", "hdf"],
     )
 
     if softwarefile is not None:
-
         softwarefile_df = read_uploaded_file_into_df(softwarefile)
         # display head a protein data
 
         check_software_file(softwarefile_df, software)
 
         st.write(
             f"File successfully uploaded. Number of rows: {softwarefile_df.shape[0]}"
@@ -198,37 +210,35 @@
 
 def create_metadata_file():
     dataset = DataSet(loader=st.session_state.loader)
     st.session_state["metadata_columns"] = ["sample"]
     metadata = dataset.metadata
     buffer = io.BytesIO()
 
-    with pd.ExcelWriter(buffer, engine='xlsxwriter') as writer:
+    with pd.ExcelWriter(buffer, engine="xlsxwriter") as writer:
         # Write each dataframe to a different worksheet.
-        metadata.to_excel(writer, sheet_name='Sheet1', index=False)
-        # Close the Pandas Excel writer and output the Excel file to the buffer
-        writer.close()
+        metadata.to_excel(writer, sheet_name="Sheet1", index=False)
 
         st.download_button(
             label="Download metadata template as Excel",
             data=buffer,
-            file_name='metadata.xlsx',
-            mime='application/vnd.ms-excel'
+            file_name="metadata.xlsx",
+            mime="application/vnd.ms-excel",
         )
 
-def upload_metadatafile(software):
 
+def upload_metadatafile(software):
     st.write("\n\n")
     st.markdown("### 3. Prepare Metadata.")
     metadatafile_upload = st.file_uploader(
-        "Upload metadata file. with information about your samples", key="metadatafile",
+        "Upload metadata file. with information about your samples",
+        key="metadatafile",
     )
 
-    if metadatafile_upload is not None and  st.session_state.loader is not None:
-
+    if metadatafile_upload is not None and st.session_state.loader is not None:
         metadatafile_df = read_uploaded_file_into_df(st.session_state.metadatafile)
         # display metadata
         st.write(
             f"File successfully uploaded. Number of rows: {metadatafile_df.shape[0]}"
             f", Number of columns: {metadatafile_df.shape[1]}. \nPreview:"
         )
         st.dataframe(metadatafile_df.head(5))
@@ -238,50 +248,47 @@
             # create dataset
             st.session_state["dataset"] = DataSet(
                 loader=st.session_state.loader,
                 metadata_path=metadatafile_df,
                 sample_column=st.session_state.sample_column,
             )
             st.session_state["metadata_columns"] = metadatafile_df.columns.to_list()
-
             load_options()
 
-            display_loaded_dataset()
-
     if st.session_state.loader is not None:
         create_metadata_file()
-        st.write("Download the template file and add additional information as "
-                 + "columns to your samples such as disease group. "
-                 + "Upload the updated metadata file.")
-    
+        st.write(
+            "Download the template file and add additional information as "
+            + "columns to your samples such as disease group. "
+            + "Upload the updated metadata file."
+        )
+
     if st.session_state.loader is not None:
         if st.button("Create a DataSet without metadata"):
             st.session_state["dataset"] = DataSet(loader=st.session_state.loader)
             st.session_state["metadata_columns"] = ["sample"]
 
             load_options()
 
-            display_loaded_dataset()
-
 
 def load_sample_data():
     _this_file = os.path.abspath(__file__)
     _this_directory = os.path.dirname(_this_file)
-    _parent_directory = os.path.dirname(_this_directory)     
-    folder_to_load = os.path.join(_parent_directory, 'sample_data')
-    
-    filepath= os.path.join(folder_to_load, "proteinGroups.txt")
-    metadatapath= os.path.join(folder_to_load, "metadata.xlsx")
+    _parent_directory = os.path.dirname(_this_directory)
+    folder_to_load = os.path.join(_parent_directory, "sample_data")
+
+    filepath = os.path.join(folder_to_load, "proteinGroups.txt")
+    metadatapath = os.path.join(folder_to_load, "metadata.xlsx")
 
     loader = MaxQuantLoader(file=filepath)
-    ds = DataSet(
-        loader=loader, metadata_path=metadatapath, sample_column="sample"
-    )
-    metadatapath = os.path.join(_this_directory, "sample_data/metadata.xlsx").replace(
-        "pages/", ""
+    ds = DataSet(loader=loader, metadata_path=metadatapath, sample_column="sample")
+    metadatapath = (
+        os.path.join(_this_directory, "sample_data", "metadata.xlsx")
+        .replace("pages/", "")
+        .replace("pages\\", "")
     )
 
     loader = MaxQuantLoader(file=filepath)
     ds = DataSet(loader=loader, metadata_path=metadatapath, sample_column="sample")
 
     ds.metadata = ds.metadata[
         [
@@ -298,39 +305,39 @@
 
     load_options()
 
 
 def import_data():
     options = ["<select>"] + list(software_options.keys())
 
-    software = st.selectbox(
+    st.selectbox(
         "Select your Proteomics Software",
         options=options,
+        key="software",
     )
-    session_state_empty = False
-
-    if software != "<select>":
-        upload_softwarefile(software=software)
 
+    if st.session_state.software != "<select>":
+        upload_softwarefile(software=st.session_state.software)
+    if "loader" not in st.session_state:
+        st.session_state["loader"] = None
     if st.session_state.loader is not None:
-        upload_metadatafile(software)
+        upload_metadatafile(st.session_state.software)
 
 
 def display_loaded_dataset():
-
     st.info("Data was successfully imported")
     st.info("DataSet has been created")
 
     st.markdown(f"*Preview:* Raw data from {st.session_state.dataset.software}")
     st.dataframe(st.session_state.dataset.rawinput.head(5))
 
-    st.markdown(f"*Preview:* Metadata")
+    st.markdown("*Preview:* Metadata")
     st.dataframe(st.session_state.dataset.metadata.head(5))
 
-    st.markdown(f"*Preview:* Matrix")
+    st.markdown("*Preview:* Matrix")
 
     df = pd.DataFrame(
         st.session_state.dataset.mat.values,
         index=st.session_state.dataset.mat.index.to_list(),
     ).head(5)
 
     st.dataframe(df)
@@ -351,16 +358,16 @@
 def empty_session_state():
     """
     remove all variables to avoid conflicts
     """
     for key in st.session_state.keys():
         del st.session_state[key]
     st.empty()
+    st.session_state["software"] = "<select>"
 
-    from streamlit.runtime import get_instance
     from streamlit.runtime.scriptrunner.script_run_context import get_script_run_ctx
 
     user_session_id = get_script_run_ctx().session_id
     st.session_state["user_session_id"] = user_session_id
 
 
 sidebar_info()
@@ -369,19 +376,27 @@
 if "dataset" not in st.session_state:
     st.markdown("### Import Proteomics Data")
 
     st.markdown(
         "Create a DataSet with the output of your proteomics software package and the corresponding metadata (optional). "
     )
 
-    import_data()
-    st.markdown("### Or Load sample Dataset")
+import_data()
 
-if st.button("Load sample DataSet - PXD011839"):
+if "dataset" in st.session_state:
+    st.info("DataSet has been imported")
+
+    if "distribution_plot" not in st.session_state:
+        save_plot_sampledistribution_rawdata()
+
+    display_loaded_dataset()
+
+st.markdown("### Or Load sample Dataset")
 
+if st.button("Load sample DataSet - PXD011839"):
     st.write(
         """
 
     ### Plasma proteome profiling discovers novel proteins associated with non-alcoholic fatty liver disease
 
     **Description**
 
@@ -402,22 +417,13 @@
     Sachs S, Stemmer K, Müller TD, Tschöp MH, Hofmann SM, Mann M, Plasma proteome profiling discovers novel proteins 
     associated with non-alcoholic fatty liver disease. Mol Syst Biol, 15(3):e8793(2019)
     """
     )
 
     load_sample_data()
 
-if "dataset" in st.session_state:
-    st.info("DataSet has been imported")
-
-    if "distribution_plot" not in st.session_state:
-        save_plot_sampledistribution_rawdata()
-
-    if st.button("New Session: Import new dataset"):
-
-        empty_session_state()
-
-        import_data()
 
-    if "dataset" in st.session_state:
+st.markdown("### To start a new session:")
 
-        display_loaded_dataset()
+if st.button("New Session: Import new dataset"):
+    empty_session_state()
+    st.rerun()
```

### Comparing `alphastats-0.6.5/alphastats/gui/pages/03_Data Overview.py` & `alphastats-0.6.6/alphastats/gui/pages/03_Data Overview.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/pages/03_Preprocessing.py` & `alphastats-0.6.6/alphastats/gui/pages/03_Preprocessing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -141,8 +141,8 @@
 
 main_preprocessing()
 
 
 def plot_intensity_distribution():
     st.selectbox(
         "Sample", options=st.session_state.dataset.metadata["sample"].to_list()
-    )
+    )
```

### Comparing `alphastats-0.6.5/alphastats/gui/pages/04_Analysis.py` & `alphastats-0.6.6/alphastats/gui/pages/04_Analysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/pages/06_Results.py` & `alphastats-0.6.6/alphastats/gui/pages/06_Results.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/sample_data/metadata.xlsx` & `alphastats-0.6.6/alphastats/gui/sample_data/metadata.xlsx`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/sample_data/proteinGroups.txt` & `alphastats-0.6.6/alphastats/gui/sample_data/proteinGroups.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/utils/analysis_helper.py` & `alphastats-0.6.6/alphastats/gui/utils/analysis_helper.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/utils/options.py` & `alphastats-0.6.6/alphastats/gui/utils/options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/utils/software_options.py` & `alphastats-0.6.6/alphastats/gui/utils/software_options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/gui/utils/ui_helper.py` & `alphastats-0.6.6/alphastats/gui/utils/ui_helper.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/load_data.py` & `alphastats-0.6.6/alphastats/load_data.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/loader/AlphaPeptLoader.py` & `alphastats-0.6.6/alphastats/loader/AlphaPeptLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/loader/BaseLoader.py` & `alphastats-0.6.6/alphastats/loader/BaseLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/loader/DIANNLoader.py` & `alphastats-0.6.6/alphastats/loader/DIANNLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/loader/FragPipeLoader.py` & `alphastats-0.6.6/alphastats/loader/FragPipeLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/loader/GenericLoader.py` & `alphastats-0.6.6/alphastats/loader/GenericLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/loader/MaxQuantLoader.py` & `alphastats-0.6.6/alphastats/loader/MaxQuantLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/loader/SpectronautLoader.py` & `alphastats-0.6.6/alphastats/loader/SpectronautLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/loader/mzTabLoader.py` & `alphastats-0.6.6/alphastats/loader/mzTabLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/multicova/multicova.py` & `alphastats-0.6.6/alphastats/multicova/multicova.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/plots/ClusterMap.py` & `alphastats-0.6.6/alphastats/plots/ClusterMap.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/plots/DimensionalityReduction.py` & `alphastats-0.6.6/alphastats/plots/DimensionalityReduction.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/plots/IntensityPlot.py` & `alphastats-0.6.6/alphastats/plots/IntensityPlot.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/plots/PlotUtils.py` & `alphastats-0.6.6/alphastats/plots/PlotUtils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/plots/SampleHistogram.py` & `alphastats-0.6.6/alphastats/plots/SampleHistogram.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/plots/VolcanoPlot.py` & `alphastats-0.6.6/alphastats/plots/VolcanoPlot.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/statistics/Anova.py` & `alphastats-0.6.6/alphastats/statistics/Anova.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/statistics/DifferentialExpressionAnalysis.py` & `alphastats-0.6.6/alphastats/statistics/DifferentialExpressionAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/statistics/MultiCovaAnalysis.py` & `alphastats-0.6.6/alphastats/statistics/MultiCovaAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/statistics/StatisticUtils.py` & `alphastats-0.6.6/alphastats/statistics/StatisticUtils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats/utils.py` & `alphastats-0.6.6/alphastats/utils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/alphastats.egg-info/PKG-INFO` & `alphastats-0.6.6/alphastats.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.6.5
+Version: 0.6.6
 Summary: An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
 Author-email: elena.krismer@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
@@ -16,14 +16,39 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pandas==2.0.2
+Requires-Dist: scikit-learn==1.2.2
+Requires-Dist: data_cache>=0.1.6
+Requires-Dist: plotly==5.15.0
+Requires-Dist: statsmodels==0.14.0
+Requires-Dist: sklearn_pandas==2.2.0
+Requires-Dist: pingouin==0.5.3
+Requires-Dist: scipy==1.10.1
+Requires-Dist: tqdm>=4.64.0
+Requires-Dist: diffxpy==0.7.4
+Requires-Dist: anndata==0.9.1
+Requires-Dist: umap-learn==0.5.3
+Requires-Dist: streamlit==1.22.0
+Requires-Dist: tables==3.7.0
+Requires-Dist: numpy==1.23.5
+Requires-Dist: numba==0.56.4
+Requires-Dist: numba-stats==0.5.0
+Requires-Dist: swifter==1.2.0
+Requires-Dist: click==8.0.1
+Requires-Dist: kaleido==0.2.1
+Requires-Dist: combat==0.3.3
+Requires-Dist: xlsxwriter==3.1.0
+Requires-Dist: pyteomics==4.6.0
+Requires-Dist: openpyxl>=3.0.10
+Requires-Dist: nbformat>=5.0
 
 [![PyPI version](https://badge.fury.io/py/alphastats.svg)](https://badge.fury.io/py/alphastats)
 [![codecov](https://codecov.io/gh/MannLabs/alphastats/branch/main/graph/badge.svg?token=HY4A0KKLRI)](https://codecov.io/gh/MannLabs/alphastats)
 [![Downloads](https://static.pepy.tech/badge/alphastats)](https://pepy.tech/project/alphastats)
 [![Downloads](https://static.pepy.tech/badge/alphastats/week)](https://pepy.tech/project/alphastats)
 [![CI](https://github.com/MannLabs/alphapeptstats/actions/workflows/python-package.yml/badge.svg)](https://github.com/MannLabs/alphapeptstats/actions/workflows/python-package.yml)
 [![Documentation Status](https://readthedocs.org/projects/alphapeptstats/badge/?version=latest)](https://alphapeptstats.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `alphastats-0.6.5/alphastats.egg-info/SOURCES.txt` & `alphastats-0.6.6/alphastats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/setup.py` & `alphastats-0.6.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     return required
 
 
 def create_pip_wheel():
     requirements = get_requirements()
     setuptools.setup(
         name="alphastats",
-        version="0.6.5",
+        version="0.6.6",
         license="Apache",
         description="An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics",
         long_description=get_long_description(),
         long_description_content_type="text/markdown",
         author="Mann Labs",
         author_email="elena.krismer@gmail.com",
         url="https://github.com/MannLabs/alphastats",
```

### Comparing `alphastats-0.6.5/tests/test_DataSet.py` & `alphastats-0.6.6/tests/test_DataSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,56 +233,67 @@
         self.assertEqual(self.obj.metadata.shape, (2, 2))
 
     @patch("logging.Logger.warning")
     def test_remove_misc_samples_in_metadata(self, mock):
         df = pd.DataFrame(
             {"sample": ["A", "B", "C"], "b": ["disease", "health", "disease"]}
         )
-        obj = DataSet(loader=self.loader, metadata_path=df, sample_column="sample",)
+        obj = DataSet(
+            loader=self.loader,
+            metadata_path=df,
+            sample_column="sample",
+        )
         #  is sample C removed
         self.assertEqual(self.obj.metadata.shape, (2, 2))
         mock.assert_called_once()
 
     def test_load_metadata_df(self):
         if self.metadata_path.endswith(".csv"):
             df = pd.read_csv(self.metadata_path)
         else:
             df = pd.read_excel(self.metadata_path)
-        obj = DataSet(loader=self.loader, metadata_path=df, sample_column="sample",)
+        obj = DataSet(
+            loader=self.loader,
+            metadata_path=df,
+            sample_column="sample",
+        )
         self.assertIsInstance(obj.metadata, pd.DataFrame)
         self.assertFalse(obj.metadata.empty)
 
     def test_preprocess_remove_samples(self):
         sample_list = ["A"]
         self.obj.preprocess(remove_samples=sample_list)
         self.assertEqual(self.obj.mat.shape, (1, 3781))
 
     def test_preprocess_normalize_zscore(self):
         self.obj.mat = pd.DataFrame({"a": [2, 5, 4], "b": [5, 4, 4], "c": [0, 10, 8]})
         # zscore Normalization
         self.obj.preprocess(log2_transform=False, normalization="zscore")
         expected_mat = pd.DataFrame(
             {
-                "a": [-1.33630621, 1.06904497, 0.26726124],
-                "b": [1.41421356, -0.70710678, -0.70710678],
-                "c": [-1.38873015, 0.9258201, 0.46291005],
+                "a": [-0.162221, -0.508001, -0.707107],
+                "b": [1.297771, -0.889001, -0.707107],
+                "c": [-1.135550, 1.397001, 1.414214],
             }
         )
         pd._testing.assert_frame_equal(self.obj.mat, expected_mat)
 
     def test_preprocess_normalize_quantile(self):
         self.obj.mat = pd.DataFrame({"a": [2, 5, 4], "b": [5, 4, 4], "c": [0, 10, 8]})
         # Quantile Normalization
         self.obj.preprocess(log2_transform=False, normalization="quantile")
         expected_mat = pd.DataFrame(
-            {"a": [0.0, 1.0, 0.5], "b": [1.0, 0.0, 0.0], "c": [0.0, 1.0, 0.5]}
+            {"a": [0.5, 0.5, 0.0], 
+             "b": [1.0, 0.0, 0.0], 
+             "c": [0.0, 1.0, 1.0]}
         )
         pd._testing.assert_frame_equal(self.obj.mat, expected_mat)
 
     def test_preprocess_normalize_linear(self):
+        # !!! normalizes by row and not by feature
         self.obj.mat = pd.DataFrame({"a": [2, 5, 4], "b": [5, 4, 4], "c": [0, 10, 8]})
         # Linear Normalization
         self.obj.preprocess(log2_transform=False, normalization="linear")
         expected_mat = pd.DataFrame(
             {
                 "a": [0.37139068, 0.42107596, 0.40824829],
                 "b": [0.92847669, 0.33686077, 0.40824829],
@@ -293,17 +304,17 @@
 
     def test_preprocess_normalize_vst(self):
         self.obj.mat = pd.DataFrame({"a": [2, 5, 4], "b": [5, 4, 4], "c": [0, 10, 8]})
         # Linear Normalization
         self.obj.preprocess(log2_transform=False, normalization="vst")
         expected_mat = pd.DataFrame(
             {
-                "a": [ 3.19059101,  11.591763, 8.365096],
-                "b": [0.084829, 0.084829, 0.084829],
-                "c": [0.000000, 7.850074, 6.435102],
+                "a": [-0.009526, -0.236399, -0.707107],
+                "b": [	1.229480, -1.089313, -0.707107],
+                "c": [-1.219954, 1.325712, 1.414214],
             }
         )
         pd._testing.assert_frame_equal(self.obj.mat.round(2), expected_mat.round(2))
 
     def test_preprocess_imputation_mean_values(self):
         self.obj.mat = pd.DataFrame(
             {"a": [2, np.nan, 4], "b": [5, 4, 4], "c": [np.nan, 10, np.nan]}
@@ -337,17 +348,17 @@
     def test_preprocess_imputation_randomforest_values(self):
         self.obj.mat = pd.DataFrame(
             {"a": [2, np.nan, 4], "b": [5, 4, 4], "c": [np.nan, 10, np.nan]}
         )
         self.obj.preprocess(log2_transform=False, imputation="randomforest")
         expected_mat = pd.DataFrame(
             {
-                "a": [2.00000000e00, -9.22337204e12, 4.00000000e00],
-                "b": [5.00000000e00, 4.00000000e00, 4.0],
-                "c": [-9.22337204e12, 1.00000000e01, -9.22337204e12],
+                "a": [2.0, 3.0, 4.0],
+                "b": [5.0, 4.0, 4.0],
+                "c": [10.0, 10.0, 10.0],
             }
         )
         pd._testing.assert_frame_equal(self.obj.mat, expected_mat)
 
     def test_plot_sampledistribution_group(self):
         plot = self.obj.plot_sampledistribution(
             method="box", color="disease", log_scale=False
@@ -405,29 +416,31 @@
     def test_load_evidence_wrong_sample_names(self):
         with self.assertRaises(ValueError):
             loader = MaxQuantLoader(
                 file="testfiles/maxquant/proteinGroups.txt",
                 evidence_file="testfiles/maxquant_go/evidence.txt",
             )
             DataSet(
-                loader=loader, metadata_path=self.metadata_path, sample_column="sample",
+                loader=loader,
+                metadata_path=self.metadata_path,
+                sample_column="sample",
             )
 
     def test_plot_pca_group(self):
         pca_plot = self.obj.plot_pca(group=self.comparison_column)
         # 5 different disease
         self.assertEqual(len(pca_plot.to_plotly_json().get("data")), 5)
-    
+
     def test_data_completeness(self):
         self.obj.preprocess(log2_transform=False, data_completeness=0.7)
-        self.assertEqual(self.obj.mat.shape[1], 517)
+        self.assertEqual(self.obj.mat.shape[1], 159)
 
     def test_plot_pca_circles(self):
         pca_plot = self.obj.plot_pca(group=self.comparison_column, circle=True)
-        # are there 5 circles drawn - for each group
+        # are there 5 circles test_preprocess_imputation_randomforest_values - for each group
         number_of_groups = len(pca_plot.to_plotly_json().get("layout").get("shapes"))
         self.assertEqual(number_of_groups, 5)
 
     def test_plot_umap_group(self):
         umap_plot = self.obj.plot_umap(group=self.comparison_column)
         # 5 different disease
         self.assertEqual(len(umap_plot.to_plotly_json().get("data")), 5)
@@ -456,17 +469,15 @@
     def test_plot_volcano_compare_preprocessing_modes(self):
         result_list = self.obj.plot_volcano(
             method="ttest",
             group1=["1_31_C6", "1_32_C7", "1_57_E8"],
             group2=["1_71_F10", "1_73_F12"],
             compare_preprocessing_modes=True,
         )
-
-        self.assertEqual(len(result_list), 12)               
-
+        self.assertEqual(len(result_list), 12)
 
     def test_preprocess_subset(self):
         self.obj.preprocess(subset=True, log2_transform=False)
         self.assertEqual(self.obj.mat.shape, (48, 1364))
 
     @patch.object(Statistics, "tukey_test")
     def test_anova_without_tukey(self, mock):
@@ -484,22 +495,25 @@
             add_significance=True,
         )
         plot_dict = plot.to_plotly_json()
         self.assertEqual(len(plot_dict.get("data")), 3)
 
     @patch("logging.Logger.warning")
     def test_plot_intenstity_subgroup_significance_warning(self, mock):
+        import streamlit as st
+
+        st.session_state["gene_to_prot_id"] = {}
         plot = self.obj.plot_intensity(
             protein_id="K7ERI9;A0A024R0T8;P02654;K7EJI9;K7ELM9;K7EPF9;K7EKP1",
             group="disease",
             add_significance=True,
         )
         plot_dict = plot.to_plotly_json()
         self.assertEqual(len(plot_dict.get("data")), 5)
-        mock.assert_called_once()
+        self.assertEqual(mock.call_count, 2)
 
     def test_anova_with_tukey(self):
         # with first 100 protein ids
         self.obj.preprocess(imputation="mean")
         id_list = self.obj.mat.columns.tolist()[0:100]
         results = self.obj.anova(column="disease", protein_ids=id_list, tukey=True)
         self.assertEqual(results.shape, (100, 10))
@@ -531,15 +545,15 @@
             group1="healthy",
             group2="liver cirrhosis",
             method="ttest",
             labels=True,
             draw_line=False,
         )
         n_labels = len(plot.to_plotly_json().get("layout").get("annotations"))
-        #self.assertTrue(n_labels > 20)
+        # self.assertTrue(n_labels > 20)
 
     def test_plot_volcano_wald(self):
         """
         Volcano Plot with wald test and list of samples
         """
         self.obj.preprocess(imputation="knn")
         self.obj.plot_volcano(
@@ -561,26 +575,28 @@
             group2="type 2 diabetes mellitus|non-alcoholic fatty liver disease",
             method="sam",
             draw_line=True,
             perm=10,
         )
 
         # fdr lines get drawn
-        line_1 = plot.to_plotly_json()["data"][3].get("line").get("shape")
-        line_2 = plot.to_plotly_json()["data"][4].get("line").get("shape")
+        line_1 = plot.to_plotly_json()["data"][-2].get("line").get("shape")
+        line_2 = plot.to_plotly_json()["data"][-1].get("line").get("shape")
 
         self.assertEqual(line_1, "spline")
         self.assertEqual(line_2, "spline")
-    
+
     def test_plot_volcano_list(self):
         self.obj.preprocess(imputation="mean")
-        plot = self.obj.plot_volcano( method="ttest",
+        plot = self.obj.plot_volcano(
+            method="ttest",
             group1=["1_31_C6", "1_32_C7", "1_57_E8"],
             group2=["1_71_F10", "1_73_F12"],
-            color_list=self.obj.mat.columns.to_list()[0:20])
+            color_list=self.obj.mat.columns.to_list()[0:20],
+        )
         self.assertEqual(len(plot.to_plotly_json()["data"][0]["x"]), 20)
 
     def test_plot_clustermap_significant(self):
         import sys
 
         sys.setrecursionlimit(100000)
         self.obj.preprocess(imputation="knn")
@@ -598,27 +614,27 @@
             column="disease",
             group1="healthy",
             group2="liver cirrhosis",
             method="ttest",
             labels=True,
         )
         n_labels = len(plot.to_plotly_json().get("layout").get("annotations"))
-    
+
     def test_plot_volcano_with_labels_proteins_welch_ttest(self):
         # remove gene names
         self.obj.gene_names = None
         plot = self.obj.plot_volcano(
             column="disease",
             group1="healthy",
             group2="liver cirrhosis",
             method="welch-ttest",
             labels=True,
         )
         n_labels = len(plot.to_plotly_json().get("layout").get("annotations"))
-        #self.assertTrue(n_labels > 20)
+        # self.assertTrue(n_labels > 20)
 
     def test_calculate_diff_exp_wrong(self):
         # get groups from comparison column
         with self.assertRaises(ValueError):
             self.obj.preprocess(imputation="knn")
             groups = list(set(self.obj.metadata[self.comparison_column].to_list()))
             group1, group2 = groups[0], groups[1]
@@ -707,47 +723,53 @@
 
         annotation = (
             plot.to_plotly_json().get("layout").get("annotations")[1].get("text")
         )
         self.assertEqual(annotation, "***")
 
     def test_plot_intensity_all(self):
-        plot = self.obj.plot_intensity(protein_id="Q9BWP8", 
-            group="disease", 
+        plot = self.obj.plot_intensity(
+            protein_id="Q9BWP8",
+            group="disease",
             subgroups=["liver cirrhosis", "healthy"],
             method="all",
-            add_significance=True)
+            add_significance=True,
+        )
         self.assertEqual(plot.to_plotly_json()["data"][0]["points"], "all")
 
-    
     def test_plot_samplehistograms(self):
         fig = self.obj.plot_samplehistograms().to_plotly_json()
         self.assertEqual(312, len(fig["data"]))
-    
+
     def test_batch_correction(self):
-        self.obj.preprocess(subset=True, imputation="knn", normalization="quantile")
+        self.obj.preprocess(subset=True, imputation="knn", normalization="linear")
         self.obj.batch_correction(batch="batch_artifical_added")
-        first_value = self.obj.mat.values[0,0]
-        self.assertAlmostEqual(0.0111, first_value, places=2)   
+        first_value = self.obj.mat.values[0, 0]
+        self.assertAlmostEqual(-0.00555, first_value, places=3)
 
     def test_multicova_analysis_invalid_covariates(self):
         self.obj.preprocess(imputation="knn", normalization="zscore", subset=True)
         res, _ = self.obj.multicova_analysis(
-            covariates=["disease", "Alkaline phosphatase measurement", "Body mass index ", "not here"],
+            covariates=[
+                "disease",
+                "Alkaline phosphatase measurement",
+                "Body mass index ",
+                "not here",
+            ],
             subset={"disease": ["healthy", "liver cirrhosis"]},
         )
         self.assertEqual(res.shape[1], 45)
 
     # def test_perform_gsea(self):
     #     df = self.obj.perform_gsea(column="disease",
     #                             group1="healthy",
     #                                     group2="liver cirrhosis",
     #                                     gene_sets= 'KEGG_2019_Human')
 
-    #     cholesterol_enhanced = 'Cholesterol metabolism' in df.index.to_list()
+    #     cholersterol_enhanced = 'Cholesterol metabolism' in df.index.to_list()
     #     self.assertTrue(cholersterol_enhanced)
 
 
 class TestDIANNDataSet(BaseTestDataSet.BaseTest):
     def setUp(self):
         self.loader = DIANNLoader(file="testfiles/diann/report_final.pg_matrix.tsv")
         self.metadata_path = "testfiles/diann/metadata.xlsx"
@@ -906,50 +928,49 @@
 
     @classmethod
     def tearDownClass(cls):
         if os.path.isdir("testfiles/spectronaut/__MACOSX"):
             shutil.rmtree("testfiles/spectronaut/__MACOSX")
 
         os.remove("testfiles/spectronaut/results.tsv")
-    
+
 class TestGenericDataSet(BaseTestDataSet.BaseTest):
     @classmethod
     def setUpClass(cls):
         if os.path.isfile("testfiles/fragpipe/combined_proteins.tsv") == False:
             shutil.unpack_archive(
                 "testfiles/fragpipe/combined_proteins.tsv.zip", "testfiles/fragpipe"
             )
 
         cls.cls_loader = GenericLoader(
             file="testfiles/fragpipe/combined_proteins.tsv",
             intensity_column=[
                 "S1 Razor Intensity",	"S2 Razor Intensity", "S3 Razor Intensity",
-                "S4 Razor Intensity",	"S5 Razor Intensity",	"S6 Razor Intensity", 
+                "S4 Razor Intensity",	"S5 Razor Intensity",	"S6 Razor Intensity",
                 "S7 Razor Intensity", "S8 Razor Intensity"
             ],
             index_column="Protein",
             sep="\t"
         )
         cls.cls_metadata_path = "testfiles/fragpipe/metadata2.xlsx"
         cls.cls_obj = DataSet(
             loader=cls.cls_loader,
             metadata_path=cls.cls_metadata_path,
             sample_column="analytical_sample external_id",
         )
-      
+
     def setUp(self):
         self.loader = copy.deepcopy(self.cls_loader)
         self.metadata_path = copy.deepcopy(self.cls_metadata_path)
         self.obj = copy.deepcopy(self.cls_obj)
         self.matrix_dim = (8, 5)
         self.matrix_dim_filtered = (8, 5)
         self.comparison_column = "grouping1"
 
     @classmethod
     def tearDownClass(cls):
         if os.path.isdir("testfiles/fragpipe/__MACOSX"):
             shutil.rmtree("testfiles/fragpipe/__MACOSX")
 
-       
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `alphastats-0.6.5/tests/test_DataSet_Pathway.py` & `alphastats-0.6.6/tests/test_DataSet_Pathway.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.5/tests/test_loaders.py` & `alphastats-0.6.6/tests/test_loaders.py`

 * *Files identical despite different names*

