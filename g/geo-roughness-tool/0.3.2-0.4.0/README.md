# Comparing `tmp/geo_roughness_tool-0.3.2.tar.gz` & `tmp/geo_roughness_tool-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_roughness_tool-0.3.2.tar", last modified: Wed May 22 10:01:49 2024, max compression
+gzip compressed data, was "geo_roughness_tool-0.4.0.tar", last modified: Thu May 23 19:30:21 2024, max compression
```

## Comparing `geo_roughness_tool-0.3.2.tar` & `geo_roughness_tool-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:49.546649 geo_roughness_tool-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-22 10:01:49.546649 geo_roughness_tool-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:01:49.546649 geo_roughness_tool-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:49.534649 geo_roughness_tool-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:49.538649 geo_roughness_tool-0.3.2/src/geo_roughness_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:49.538649 geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/threshold_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:49.542649 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/analyze_and_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/header_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/preview_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:49.542649 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   131080 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png
--rw-r--r--   0 runner    (1001) docker     (127)   122497 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)   114372 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/resources/app_icon_dark.ico
--rw-r--r--   0 runner    (1001) docker     (127)   371098 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/resources/app_icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)   400936 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/resources/app_icon_light.png
--rw-r--r--   0 runner    (1001) docker     (127)    12366 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:49.542649 geo_roughness_tool-0.3.2/src/geo_roughness_tool/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-22 10:01:37.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool/tests/test_application_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:01:49.542649 geo_roughness_tool-0.3.2/src/geo_roughness_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-22 10:01:49.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-22 10:01:49.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:01:49.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-22 10:01:49.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 10:01:49.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 10:01:49.000000 geo_roughness_tool-0.3.2/src/geo_roughness_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.719605 geo_roughness_tool-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-23 19:30:21.719605 geo_roughness_tool-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:30:21.719605 geo_roughness_tool-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.711605 geo_roughness_tool-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.711605 geo_roughness_tool-0.4.0/src/geo_roughness_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.715605 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.715605 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/preview_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.715605 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   114372 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_dark.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   371098 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   400936 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13724 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.719605 geo_roughness_tool-0.4.0/src/geo_roughness_tool/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.719605 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/top_level.txt
```

### Comparing `geo_roughness_tool-0.3.2/LICENSE` & `geo_roughness_tool-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/PKG-INFO` & `geo_roughness_tool-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.3.2
+Version: 0.4.0
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
@@ -28,37 +28,42 @@
 Requires-Dist: setuptools==69.5.1
 
 ![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
 ![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
 
 # GeoRoughness Tool
 
-The GeoRoughness Tool is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
+This is a spatial analysis tool for calculating surface roughness from Digital Elevation Models (DEMs). The tool 
+provides a comprehensive solution for geospatial analysis, allowing users to compute roughness values based on the
+standard deviation of height within a specified window size. The tool allows for easy classification of roughness values
+and generation of roughness maps for visualizing the terrain's variability.
 
 ## Features
 
-- **GeoTIFF Support**: Load and process DEM data directly from GeoTIFF files.
-- **Flexible Window Sizes**: Specify the window size in meters for roughness calculations.
-- **Advanced Thresholding**: Configure high value and categorical thresholds to refine processing.
-- **Dual Interface**: Operate through a user-friendly GUI or a powerful CLI.
-- **Dynamic Previews**: Generate and view pseudo-colored previews of the processed DEM within the GUI.
-- **Selective Saving**: Choose when to save processed outputs after reviewing results.
+- **Surface Roughness Calculation**: Compute roughness values based on the standard deviation of height.
+- **Surface Roughness Mapping**: Generate roughness maps for visualizing the terrain's variability.
+- **Surface Roughness Classification**: Categorize roughness values into different classes.
+- **Classification Quality Metrics**: Evaluate the quality of the classification using accuracy metrics.
+- **Classification Optimization**: Optimize the classification thresholds for better results.
+
+---
 
 ## Documentation
 
 For more detailed information about the tool's capabilities and additional configurations, 
 please refer to the [Project's Wiki](../../wiki).
 
 ## Installation Guide for GeoRoughness Tool
 
 Follow these steps to install the GeoRoughness Tool on your system. The program is available
 as a Python package and can therefore be installed on any major operating system.
 
 > [!TIP]
-> If you are not that experienced using command line tools or experience any problems during installation, please refer to the [Getting Started Wiki Page](../../wiki/Getting-Started) for a more detailed and OS specific installation guide.
+> If you are not that experienced using command line tools or experience any problems during installation, please refer 
+> to the [Getting Started Wiki Page](../../wiki/Getting-Started) for a more detailed and OS specific installation guide.
 
 ### Prerequisites
 
 Before you begin, ensure that your system meets the following requirements:
 - **Python 3.12 or later**: The software is built to run with Python 3.12 and above.
 - **pip**: Python's package installer, used to install the GeoRoughness Tool.
 
@@ -79,54 +84,44 @@
 
 #### 3. Install GeoRoughness Tool
 Install the package via pip:
 ```bash
 pip3 install geo-roughness-tool
 ```
 
-## Usage
+---
 
-### GUI Application
+## Usage
 
-To launch the GUI, simply run the following command in your terminal:
+To launch the Application, simply run the following command in your terminal after installation:
 
 ```bash
 georough
 ```
 
-The graphical interface allows you to browse for input files, set processing parameters, and view the roughness map interactively before deciding to save the output.
+---
 
 ### CLI Application
 
-For those who prefer working in a command-line environment, the CLI provides a robust solution. Here’s how to use it:
+This package also provides a basic command line interface (CLI) for batch processing of DEM files. For more information 
+on how to use the CLI, please refer to the [CLI Documentation](../../wiki/Getting-Started#CLI-Application).
 
-```bash
-georough --input_path "path/to/input.tif" --output_dir "path/to/output" --window_size 1.0 --band_number 1 --high_value_threshold 1.0 --categorical_thresholds 0.1, 0.2, 0.3
-```
+---
 
-### Parameters
-
-- **`--input_path`**: Path to the input GeoTIFF file.
-- **`--output_dir`**: Directory where the output files will be saved.
-- **`--window_size`** (optional): The size of the window in meters for calculating roughness.
-- **`--band_number`** (optional): The specific band of the DEM to process.
-- **`--high_value_threshold`** (optional): Threshold to filter out high elevation values.
-- **`--categorical_thresholds`** (optional): Set of thresholds to categorize the elevation data.
-
-## Disclaimer
+## AI-Assisted Development
 
 > [!NOTE]
-> **AI-Assisted Development**
-> 
-> This project leverages artificial intelligence, including OpenAI's GPT-4 and GitHub Copilot, to assist in generating parts of the code and documentation. These tools provide suggestions that enhance the development process and help in crafting more robust and comprehensive materials. While AI tools have been instrumental in accelerating development and improving productivity, the final decisions on the inclusion and modification of the generated content rest solely with the human developers. This ensures that each aspect of the project aligns with our quality standards and functional requirements. 
+> This project leverages artificial intelligence, including OpenAI's GPT-4, GPT-4o and GitHub Copilot, to assist in generating parts of the code and documentation. These tools provide suggestions that enhance the development process and help in crafting more robust and comprehensive materials. While AI tools have been instrumental in accelerating development and improving productivity, the final decisions on the inclusion and modification of the generated content rest solely with the human developers. This ensures that each aspect of the project aligns with our quality standards and functional requirements. 
 > 
 > Please note that while AI has contributed to the project, it may not capture the full complexity or context of the development practices. As such, any anomalies or errors introduced by AI-generated content have been reviewed and rectified to the best of our capabilities. However, users should exercise their judgment and discretion when using or modifying this software. 
 > 
 > For any concerns or questions about the AI-generated content within this project, please feel free to contact us through the repository's issues section.
 
+---
+
 ## Contributing
 
 We welcome contributions! If you have suggestions or want to report bugs, please use the [Issues](../../issues) section of this repository.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `geo_roughness_tool-0.3.2/README.md` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,69 @@
+Metadata-Version: 2.1
+Name: geo-roughness-tool
+Version: 0.4.0
+Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
+Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
+Author: Lukas Batschelet
+License: MIT
+Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
+Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
+Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
+Keywords: GIS,GeoTIFF,DEM,surface roughness,geographic information systems
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: GIS
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: customtkinter==5.2.2
+Requires-Dist: matplotlib==3.8.4
+Requires-Dist: numpy==1.26.4
+Requires-Dist: Pillow==10.3.0
+Requires-Dist: rasterio==1.3.10
+Requires-Dist: screeninfo==0.8.1
+Requires-Dist: setuptools==69.5.1
+
 ![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
 ![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
 
 # GeoRoughness Tool
 
-The GeoRoughness Tool is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
+This is a spatial analysis tool for calculating surface roughness from Digital Elevation Models (DEMs). The tool 
+provides a comprehensive solution for geospatial analysis, allowing users to compute roughness values based on the
+standard deviation of height within a specified window size. The tool allows for easy classification of roughness values
+and generation of roughness maps for visualizing the terrain's variability.
 
 ## Features
 
-- **GeoTIFF Support**: Load and process DEM data directly from GeoTIFF files.
-- **Flexible Window Sizes**: Specify the window size in meters for roughness calculations.
-- **Advanced Thresholding**: Configure high value and categorical thresholds to refine processing.
-- **Dual Interface**: Operate through a user-friendly GUI or a powerful CLI.
-- **Dynamic Previews**: Generate and view pseudo-colored previews of the processed DEM within the GUI.
-- **Selective Saving**: Choose when to save processed outputs after reviewing results.
+- **Surface Roughness Calculation**: Compute roughness values based on the standard deviation of height.
+- **Surface Roughness Mapping**: Generate roughness maps for visualizing the terrain's variability.
+- **Surface Roughness Classification**: Categorize roughness values into different classes.
+- **Classification Quality Metrics**: Evaluate the quality of the classification using accuracy metrics.
+- **Classification Optimization**: Optimize the classification thresholds for better results.
+
+---
 
 ## Documentation
 
 For more detailed information about the tool's capabilities and additional configurations, 
 please refer to the [Project's Wiki](../../wiki).
 
 ## Installation Guide for GeoRoughness Tool
 
 Follow these steps to install the GeoRoughness Tool on your system. The program is available
 as a Python package and can therefore be installed on any major operating system.
 
 > [!TIP]
-> If you are not that experienced using command line tools or experience any problems during installation, please refer to the [Getting Started Wiki Page](../../wiki/Getting-Started) for a more detailed and OS specific installation guide.
+> If you are not that experienced using command line tools or experience any problems during installation, please refer 
+> to the [Getting Started Wiki Page](../../wiki/Getting-Started) for a more detailed and OS specific installation guide.
 
 ### Prerequisites
 
 Before you begin, ensure that your system meets the following requirements:
 - **Python 3.12 or later**: The software is built to run with Python 3.12 and above.
 - **pip**: Python's package installer, used to install the GeoRoughness Tool.
 
@@ -50,54 +84,44 @@
 
 #### 3. Install GeoRoughness Tool
 Install the package via pip:
 ```bash
 pip3 install geo-roughness-tool
 ```
 
-## Usage
+---
 
-### GUI Application
+## Usage
 
-To launch the GUI, simply run the following command in your terminal:
+To launch the Application, simply run the following command in your terminal after installation:
 
 ```bash
 georough
 ```
 
-The graphical interface allows you to browse for input files, set processing parameters, and view the roughness map interactively before deciding to save the output.
+---
 
 ### CLI Application
 
-For those who prefer working in a command-line environment, the CLI provides a robust solution. Here’s how to use it:
-
-```bash
-georough --input_path "path/to/input.tif" --output_dir "path/to/output" --window_size 1.0 --band_number 1 --high_value_threshold 1.0 --categorical_thresholds 0.1, 0.2, 0.3
-```
-
-### Parameters
+This package also provides a basic command line interface (CLI) for batch processing of DEM files. For more information 
+on how to use the CLI, please refer to the [CLI Documentation](../../wiki/Getting-Started#CLI-Application).
 
-- **`--input_path`**: Path to the input GeoTIFF file.
-- **`--output_dir`**: Directory where the output files will be saved.
-- **`--window_size`** (optional): The size of the window in meters for calculating roughness.
-- **`--band_number`** (optional): The specific band of the DEM to process.
-- **`--high_value_threshold`** (optional): Threshold to filter out high elevation values.
-- **`--categorical_thresholds`** (optional): Set of thresholds to categorize the elevation data.
+---
 
-## Disclaimer
+## AI-Assisted Development
 
 > [!NOTE]
-> **AI-Assisted Development**
-> 
-> This project leverages artificial intelligence, including OpenAI's GPT-4 and GitHub Copilot, to assist in generating parts of the code and documentation. These tools provide suggestions that enhance the development process and help in crafting more robust and comprehensive materials. While AI tools have been instrumental in accelerating development and improving productivity, the final decisions on the inclusion and modification of the generated content rest solely with the human developers. This ensures that each aspect of the project aligns with our quality standards and functional requirements. 
+> This project leverages artificial intelligence, including OpenAI's GPT-4, GPT-4o and GitHub Copilot, to assist in generating parts of the code and documentation. These tools provide suggestions that enhance the development process and help in crafting more robust and comprehensive materials. While AI tools have been instrumental in accelerating development and improving productivity, the final decisions on the inclusion and modification of the generated content rest solely with the human developers. This ensures that each aspect of the project aligns with our quality standards and functional requirements. 
 > 
 > Please note that while AI has contributed to the project, it may not capture the full complexity or context of the development practices. As such, any anomalies or errors introduced by AI-generated content have been reviewed and rectified to the best of our capabilities. However, users should exercise their judgment and discretion when using or modifying this software. 
 > 
 > For any concerns or questions about the AI-generated content within this project, please feel free to contact us through the repository's issues section.
 
+---
+
 ## Contributing
 
 We welcome contributions! If you have suggestions or want to report bugs, please use the [Issues](../../issues) section of this repository.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `geo_roughness_tool-0.3.2/setup.py` & `geo_roughness_tool-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Read the contents of your requirements file
 def read_requirements(file_name):
     with open(file_name, 'r', encoding='utf-8') as f:
         return f.read().splitlines()
 
 setup(
     name='geo-roughness-tool',
-    version='0.3.2',
+    version='0.4.0',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/lbatschelet/GeoRoughness-Tool',
     license='MIT',
     author='Lukas Batschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     long_description=read('README.md'),  # Use the README.md as the long description
```

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/application_driver.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/application_driver.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/defaults.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/defaults.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/geo_tiff_processor.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/geo_tiff_processor.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/processing_parameters.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/processing_parameters.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/classes/threshold_optimizer.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/threshold_optimizer.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/cli_main.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/cli_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/footer_frame.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/footer_frame.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
-import logging.handlers
+import os
 import webbrowser
 from typing import Any
 import tkinter as tk
 import tkinter.scrolledtext as st
+from PIL import Image, ImageTk
 
 import customtkinter as ctk
 
-
 from .defaults import DEFAULTS
 from geo_roughness_tool.log_config import Defaults
 
 # Set up logging
 logger = logging.getLogger(__name__)
 
 
@@ -44,43 +44,59 @@
         """
         super().__init__(parent, **kwargs)
         logger.info("Initializing FooterFrame")
         self.main_gui = main_gui
 
         # Configure the grid
         self.grid_rowconfigure([0, 1], weight=1)
-        self.grid_columnconfigure([0, 1, 2, 3], weight=1)
+        self.grid_columnconfigure([0, 1, 2], weight=1)
 
         # Create the help button
         self.help_button = WebsiteButton(self,
                                          "https://github.com/lbatschelet/GeoRoughness-Tool",
                                          text="Documentation")
         self.help_button.grid(row=0,
                               column=0,
                               padx=(DEFAULTS.PADX, DEFAULTS.PADX * 0.5),
                               pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5),
-                              sticky="nsew")
+                              sticky="new")
+
+        # Load the original images
+        script_dir = os.path.dirname(__file__)
+        self.original_light_image = Image.open(
+            os.path.join(script_dir, "resources", "GeoRoughness_Banner_long_light.png"))
+        self.original_dark_image = Image.open(
+            os.path.join(script_dir, "resources", "GeoRoughness_Banner_long_dark.png"))
+
+        # Create the CTkImage
+        self.banner_image = ctk.CTkImage(light_image=self.original_light_image, dark_image=self.original_dark_image,
+                                         size=(200, 40))
+
+        # Create the banner label
+        self.banner_label = ctk.CTkLabel(self, image=self.banner_image, text="")
+        self.banner_label.grid(row=0, column=1, pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5), sticky="nsew")
+        logger.info("Banner label created")
 
         # Create the log button
         self.log_button = ctk.CTkButton(self, text="Show Logs", command=self.open_log_window)
         self.log_button.grid(row=0,
-                             column=3,
+                             column=2,
                              padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX),
                              pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5),
-                             sticky="nsew")
+                             sticky="new")
 
         # Create the info label
         self.info_label = (
             ctk.CTkLabel(self,
                          text="GeoRoughness Tool - © 2024 L. Batschelet, F. Mohaupt, S. Röthlisberger. "
                               "Licensed under the MIT License.",
                          font=self.main_gui.fonts['small']))
         self.info_label.grid(row=1,
                              column=0,
-                             columnspan=4,
+                             columnspan=3,
                              padx=DEFAULTS.PADX,
                              pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY),
                              sticky="nsew")
 
     def open_log_window(self):
         """
         Opens the log window.
@@ -202,8 +218,7 @@
 
                 # Restore the scroll position
                 self.text_area.yview_moveto(vert_scroll_position[0])
                 self.text_area.xview_moveto(horiz_scroll_position[0])
 
         # Schedule the next update
         self.after(Defaults.LOG_UPDATE_INTERVAL, self.update_logs)
-
```

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/parameter_input.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/parameter_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .defaults import DEFAULTS
 
 class ParameterFrame(ctk.CTkFrame):
     def __init__(self, parent, main_gui, **kwargs):
         super().__init__(parent, **kwargs)
 
         self.main_gui = main_gui
+        self.advanced_options_visible = False
 
         # Make the GUI responsive
         self.grid_columnconfigure([0, 1], weight=1)
         self.grid_rowconfigure([0, 1], weight=1)
 
         self.window_size_field = (
             ParameterInput(self,
@@ -61,71 +62,78 @@
 
         # Create a new frame for the buttons
         self.button_frame = ctk.CTkFrame(self)
         self.button_frame.grid(row=2,
                                column=0,
                                columnspan=2,
                                padx=DEFAULTS.PADX,
-                               pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5),
+                               pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY),
                                sticky="ew")
         # Set equal weights for each column in the button frame
         self.button_frame.grid_columnconfigure([0, 1, 2], weight=1)
 
         self.start_processing_button = (
             ctk.CTkButton(self.button_frame, text="Start Processing", command=self.main_gui.start_processing))
         self.start_processing_button.grid(row=0,
                                           column=0,
-                                          padx=(DEFAULTS.PADX, DEFAULTS.PADX * 0.5),
-                                          pady=DEFAULTS.PADY,
+                                          padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX * 0.5),
+                                          pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5),
                                           sticky="ew")
 
         self.analyze_and_optimize_button = ctk.CTkButton(self.button_frame,
                                                          text="Analyze and optimize...",
                                                          command=self.toggle_frame, state=tk.DISABLED)
         self.analyze_and_optimize_button.grid(row=0,
                                               column=1,
                                               padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX * 0.5),
-                                              pady=DEFAULTS.PADY,
+                                              pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5),
                                               sticky="ew")
 
         self.save_file_button = (
             ctk.CTkButton(self.button_frame, text="Save File", command=self.main_gui.save_image, state=tk.DISABLED))
         self.save_file_button.grid(row=0,
                                    column=2,
                                    padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX * 0.5),
-                                   pady=DEFAULTS.PADY,
+                                   pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5),
                                    sticky="ew")
 
-        # Initially hide advanced options
-        self.band_number_field.grid_remove()
-        self.high_value_threshold_field.grid_remove()
-
         # Create a new frame and initially hide it
         self.analyze_and_optimize_frame = AnalyzeAndOptimizeFrame(self, main_gui)
         self.analyze_and_optimize_frame.grid(row=3,
                                              column=0,
-                                             columnspan=3,
+                                             columnspan=2,
                                              padx=DEFAULTS.PADX,
                                              pady=(0, DEFAULTS.PADY),
                                              sticky="ew")
+
+        # Initially hide advanced options
+        self.band_number_field.grid_remove()
+        self.high_value_threshold_field.grid_remove()
         self.analyze_and_optimize_frame.grid_remove()
 
     def toggle_advanced_options(self, show):
+        self.advanced_options_visible = show
         if show:
             self.band_number_field.grid()
             self.high_value_threshold_field.grid()
+            self.analyze_and_optimize_frame.toggle_calculate_quality(show)
         else:
             self.band_number_field.grid_remove()
             self.high_value_threshold_field.grid_remove()
+            self.analyze_and_optimize_frame.toggle_calculate_quality(show)
 
     def toggle_frame(self):
         if self.analyze_and_optimize_frame.winfo_viewable():
             self.analyze_and_optimize_frame.grid_remove()
         else:
             self.analyze_and_optimize_frame.grid()
+            if self.advanced_options_visible:
+                self.analyze_and_optimize_frame.toggle_calculate_quality(True)
+            else:
+                self.analyze_and_optimize_frame.toggle_calculate_quality(False)
 
     def get_parameters(self):
         return {
             "window_size": self.window_size_field.get() or None,
             "category_thresholds": self.category_thresholds_field.get() or None,
             "band_number": self.band_number_field.get() or None,
             "high_value_threshold": self.high_value_threshold_field.get() or None,
@@ -139,31 +147,31 @@
         self.main_gui = main_gui
         self.url = url
         self.grid_columnconfigure([0, 1], weight=1)
 
         self.name_label = ctk.CTkLabel(self, text=name, font=self.main_gui.fonts['h3'])
         self.name_label.grid(row=0,
                              column=0,
-                             padx=(DEFAULTS.PADX, DEFAULTS.PADX * 0.25),
-                             pady=DEFAULTS.PADY,
+                             padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX * 0.25),
+                             pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.25),
                              sticky="w")
 
         self.description_button = ctk.CTkButton(self, text="Description", command=self.open_url)
         self.description_button.grid(row=0,
                                      column=1,
-                                     padx=(DEFAULTS.PADX * 0.25, DEFAULTS.PADX),
-                                     pady=DEFAULTS.PADY,
+                                     padx=(DEFAULTS.PADX * 0.25, DEFAULTS.PADX * 0.5),
+                                     pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.25),
                                      sticky="e")
 
         self.entry = ctk.CTkEntry(self)
         self.entry.grid(row=1,
                         column=0,
                         columnspan=2,
-                        padx=(DEFAULTS.PADX, DEFAULTS.PADX),
-                        pady=(0, DEFAULTS.PADY),
+                        padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX * 0.5),
+                        pady=(DEFAULTS.PADY * 0.25, DEFAULTS.PADY * 0.5),
                         sticky="ew")
 
     def open_url(self):
         webbrowser.open(self.url)
 
     def get(self):
-        return self.entry.get()
+        return self.entry.get()
```

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/path_frame.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/path_frame.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,30 +53,31 @@
         super().__init__(parent, **kwargs)
         self.main_gui = main_gui
         self.grid_columnconfigure(0, weight=1)
 
         self.name_label = ctk.CTkLabel(self, text=name, font=self.main_gui.fonts['h3'])
         self.name_label.grid(row=0,
                              column=0,
-                             padx=DEFAULTS.PADX,
-                             pady=(DEFAULTS.PADY, DEFAULTS.PADY * 0.5),
+                             padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX * 0.5),
+                             pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.25),
                              sticky="w")
 
         self.entry = ctk.CTkEntry(self)
         self.entry.grid(row=1,
                         column=0,
-                        padx=(DEFAULTS.PADX, DEFAULTS.PADX * 0.5),
-                        pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY),
+                        padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX * 0.5),
+                        pady=(DEFAULTS.PADY * 0.25, DEFAULTS.PADY * 0.5),
+                        columnspan=2,
                         sticky="ew")
 
         self.browse_button = ctk.CTkButton(self, text="Browse", command=self.browse)
-        self.browse_button.grid(row=1,
+        self.browse_button.grid(row=0,
                                 column=1,
-                                padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX),
-                                pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY))
+                                padx=(DEFAULTS.PADX * 0.5, DEFAULTS.PADX * 0.5),
+                                pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.25))
 
     @abc.abstractmethod
     def browse(self):
         pass
 
     def get(self):
         return self.entry.get()
```

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/preview_image.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/resources/app_icon_dark.ico` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_dark.ico`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/resources/app_icon_dark.png` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_dark.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui/resources/app_icon_light.png` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_light.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/gui_main.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,33 @@
-"""
-gui_main.py
------------
-Version: 1.3.0
-Author: Lukas Batschelet
-Date: 14.05.2024
------------
-This module contains the main GUI class for the Surface Roughness Calculator application.
-"""
-
 import logging
 import os
 import tkinter as tk
 import platform
-from tkinter import messagebox, filedialog
+from tkinter import messagebox, filedialog, Menu
+import webbrowser
 
 import customtkinter as ctk
 import rasterio
 from PIL import Image, ImageTk
 from customtkinter import CTkScrollableFrame
 from screeninfo import get_monitors
 
-
 from .classes.application_driver import ApplicationDriver
 from .classes.processing_parameters import ProcessingParameters
 from .classes.threshold_optimizer import ThresholdOptimizer
 from .gui.defaults import DEFAULTS
 from .gui.footer_frame import FooterFrame
-from .gui.header_frame import HeaderFrame
 from .gui.parameter_input import ParameterFrame
 from .gui.path_frame import PathFrame
 from .gui.preview_image import PreviewImage
 
 logger = logging.getLogger(__name__)
 
 
+
 class GUIMain(ctk.CTk):
     def __init__(self):
         super().__init__()
 
         self.driver = None
         self.title("GeoRoughness Tool")
         self.show_advanced_options = False
@@ -60,14 +50,24 @@
         if platform.system() == "Windows":
             self.iconbitmap(os.path.join(script_dir, "gui/resources", "app_icon_dark.ico"))
         else:
             light_icon_path = os.path.join(script_dir, "gui/resources", "app_icon_light.png")
             dark_icon_path = os.path.join(script_dir, "gui/resources", "app_icon_dark.png")
             self.set_icon(light_icon_path, dark_icon_path)
 
+        # Set the application name on macOS
+        if platform.system() == "Darwin":
+            try:
+                from Foundation import NSBundle
+                bundle = NSBundle.mainBundle()
+                info = bundle.localizedInfoDictionary() or bundle.infoDictionary()
+                info['CFBundleName'] = "GeoRoughness Tool"
+            except ImportError:
+                pass
+
         # Get screen information
         monitors = get_monitors()
         primary_monitor = monitors[0]  # Assuming the primary monitor is the first one
 
         screen_width = int(0.65 * primary_monitor.width)
         screen_height = int(0.7 * primary_monitor.height)
 
@@ -78,49 +78,85 @@
         # Adjust the window size within the defined limits
         screen_width = min(max(screen_width, min_width), max_width)
         screen_height = min(max(screen_height, min_height), max_height)
 
         # Set window size
         self.geometry(f"{screen_width}x{screen_height}")
 
+        # Create the menu
+        self.create_menu()
+
         # Create a ScrolledFrame
         self.scrolled_frame = CTkScrollableFrame(self)
         self.scrolled_frame.pack(fill="both", expand=True)
 
         # Make the GUI responsive
         self.scrolled_frame.grid_columnconfigure(0, weight=1)
-        self.scrolled_frame.grid_rowconfigure([0, 1, 2, 3, 4, 5], weight=1)
-
-        self.header_frame = HeaderFrame(self.scrolled_frame, self)
-        self.header_frame.grid(row=0,
-                               column=0,
-                               sticky="nsew")
+        self.scrolled_frame.grid_rowconfigure([0, 1, 2, 3, 4], weight=1)
 
         self.path_frame = PathFrame(self.scrolled_frame, self)
-        self.path_frame.grid(row=1,
+        self.path_frame.grid(row=0,
                              column=0,
                              sticky="nsew")
 
         self.parameter_frame = ParameterFrame(self.scrolled_frame, self)
-        self.parameter_frame.grid(row=2,
+        self.parameter_frame.grid(row=1,
                                   column=0,
                                   sticky="nsew")
 
         self.preview_frame = PreviewImage(self.scrolled_frame, self, self.preview_image)
-        self.preview_frame.grid(row=3,
+        self.preview_frame.grid(row=2,
                                 column=0,
                                 padx=DEFAULTS.PADX,
                                 pady=(DEFAULTS.PADY * 0.5, DEFAULTS.PADY * 0.5),
                                 sticky="nsew")
 
         self.footer_frame = FooterFrame(self.scrolled_frame, self)
-        self.footer_frame.grid(row=4,
+        self.footer_frame.grid(row=3,
                                column=0,
                                sticky="nsew")
 
+    def create_menu(self):
+        # Create a menu bar
+        self.menubar = Menu(self)
+
+        # Options menu
+        self.options_menu = Menu(self.menubar, tearoff=0)
+        self.advanced_options_label = "Show Advanced Options"
+        self.options_menu.add_command(label=self.advanced_options_label, command=self.toggle_advanced_options)
+        self.menubar.add_cascade(label="Options", menu=self.options_menu)
+
+        # Help menu
+        help_menu = Menu(self.menubar, tearoff=0)
+        help_menu.add_command(label="Wiki", command=self.open_wiki)
+        help_menu.add_command(label="Documentation", command=self.open_documentation)
+        self.menubar.add_cascade(label="Help", menu=help_menu)
+
+        # Set the menu bar
+        self.config(menu=self.menubar)
+
+    def toggle_advanced_options(self):
+        self.show_advanced_options = not self.show_advanced_options
+        self.parameter_frame.toggle_advanced_options(self.show_advanced_options)
+        self.path_frame.toggle_advanced_options(self.show_advanced_options)
+        new_label = "Hide Advanced Options" if self.show_advanced_options else "Show Advanced Options"
+        self.update_menu_label(new_label)
+
+    def update_menu_label(self, new_label):
+        self.advanced_options_label = new_label
+        self.options_menu.entryconfig(0, label=new_label)
+
+    @staticmethod
+    def open_documentation():
+        webbrowser.open("https://github.com/lbatschelet/GeoRoughness-Tool")
+
+    @staticmethod
+    def open_wiki():
+        webbrowser.open("https://github.com/lbatschelet/GeoRoughness-Tool/wiki")
+
     def set_icon(self, light_icon_path, dark_icon_path):
         if self.get_appearance_mode() == "Dark":
             icon_image = Image.open(dark_icon_path)
         else:
             icon_image = Image.open(light_icon_path)
 
         icon_photo = ImageTk.PhotoImage(icon_image)
@@ -135,19 +171,14 @@
                 )
 
         self.bind('<<ThemeChanged>>', on_theme_change)
 
     def get_appearance_mode(self):
         return ctk.get_appearance_mode()
 
-    def toggle_advanced_options(self):
-        self.show_advanced_options = not self.show_advanced_options
-        self.parameter_frame.toggle_advanced_options(self.show_advanced_options)
-        self.path_frame.toggle_advanced_options(self.show_advanced_options)
-
     def start_processing(self) -> None:
         """
         Starts the processing of the GeoTIFF file with the provided parameters.
 
         This method gathers the parameters from the GUI, creates an instance of the ProcessingParameters class,
         initializes the ApplicationDriver with these parameters, and manages the processing flow,
         including displaying results and handling errors.
```

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/log_config.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/log_config.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool/main.py` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool/main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.3.2/src/geo_roughness_tool.egg-info/SOURCES.txt` & `geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,18 +19,17 @@
 src/geo_roughness_tool/classes/geo_tiff_processor.py
 src/geo_roughness_tool/classes/processing_parameters.py
 src/geo_roughness_tool/classes/threshold_optimizer.py
 src/geo_roughness_tool/gui/__init__.py
 src/geo_roughness_tool/gui/analyze_and_optimize.py
 src/geo_roughness_tool/gui/defaults.py
 src/geo_roughness_tool/gui/footer_frame.py
-src/geo_roughness_tool/gui/header_frame.py
 src/geo_roughness_tool/gui/parameter_input.py
 src/geo_roughness_tool/gui/path_frame.py
 src/geo_roughness_tool/gui/preview_image.py
-src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-Light.png
-src/geo_roughness_tool/gui/resources/GeoRoughness-Banner-lang-dark.png
+src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_dark.png
+src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_light.png
 src/geo_roughness_tool/gui/resources/app_icon_dark.ico
 src/geo_roughness_tool/gui/resources/app_icon_dark.png
 src/geo_roughness_tool/gui/resources/app_icon_light.png
 src/geo_roughness_tool/tests/__init__.py
 src/geo_roughness_tool/tests/test_application_driver.py
```

