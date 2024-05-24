# Comparing `tmp/geo_roughness_tool-0.4.0.tar.gz` & `tmp/geo_roughness_tool-0.4.10.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_roughness_tool-0.4.0.tar", last modified: Thu May 23 19:30:21 2024, max compression
+gzip compressed data, was "geo_roughness_tool-0.4.10.dev0.tar", last modified: Fri May 24 09:04:06 2024, max compression
```

## Comparing `geo_roughness_tool-0.4.0.tar` & `geo_roughness_tool-0.4.10.dev0.tar`

### file list

```diff
@@ -1,45 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.719605 geo_roughness_tool-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-23 19:30:21.719605 geo_roughness_tool-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:30:21.719605 geo_roughness_tool-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.711605 geo_roughness_tool-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.711605 geo_roughness_tool-0.4.0/src/geo_roughness_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.715605 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/threshold_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.715605 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/analyze_and_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/preview_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.715605 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_light.png
--rw-r--r--   0 runner    (1001) docker     (127)   114372 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_dark.ico
--rw-r--r--   0 runner    (1001) docker     (127)   371098 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)   400936 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_light.png
--rw-r--r--   0 runner    (1001) docker     (127)    13724 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.719605 geo_roughness_tool-0.4.0/src/geo_roughness_tool/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-23 19:30:12.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool/tests/test_application_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:30:21.719605 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 19:30:21.000000 geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.616978 geo_roughness_tool-0.4.10.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.608978 geo_roughness_tool-0.4.10.dev0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.608978 geo_roughness_tool-0.4.10.dev0/.github/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   212970 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.github/resources/GeoRoughness_Banner_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   226976 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.github/resources/GeoRoughness_Banner_light.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.608978 geo_roughness_tool-0.4.10.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.608978 geo_roughness_tool-0.4.10.dev0/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.idea/dem-roughness-calculator.iml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.608978 geo_roughness_tool-0.4.10.dev0/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.idea/other.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-24 09:04:05.000000 geo_roughness_tool-0.4.10.dev0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-24 09:04:06.616978 geo_roughness_tool-0.4.10.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 09:04:06.616978 geo_roughness_tool-0.4.10.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.604978 geo_roughness_tool-0.4.10.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.612978 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.612978 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.612978 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/preview_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.616978 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   114372 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/resources/app_icon_dark.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   371098 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/resources/app_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   400936 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/resources/app_icon_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13723 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-24 09:03:51.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:04:06.616978 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-24 09:04:06.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-24 09:04:06.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:04:06.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-24 09:04:06.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-24 09:04:06.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 09:04:06.000000 geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool.egg-info/top_level.txt
```

### Comparing `geo_roughness_tool-0.4.0/LICENSE` & `geo_roughness_tool-0.4.10.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/PKG-INFO` & `geo_roughness_tool-0.4.10.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.4.0
+Version: 0.4.10.dev0
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
@@ -22,14 +22,19 @@
 Requires-Dist: customtkinter==5.2.2
 Requires-Dist: matplotlib==3.8.4
 Requires-Dist: numpy==1.26.4
 Requires-Dist: Pillow==10.3.0
 Requires-Dist: rasterio==1.3.10
 Requires-Dist: screeninfo==0.8.1
 Requires-Dist: setuptools==69.5.1
+Requires-Dist: requests==2.32.2
+Requires-Dist: packaging==24.0
+Requires-Dist: wheel==0.43.0
+Requires-Dist: twine==5.1.0
+Requires-Dist: setuptools-scm==8.1.0
 
 ![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
 ![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
 
 # GeoRoughness Tool
 
 This is a spatial analysis tool for calculating surface roughness from Digital Elevation Models (DEMs). The tool
```

### Comparing `geo_roughness_tool-0.4.0/README.md` & `geo_roughness_tool-0.4.10.dev0/README.md`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/setup.py` & `geo_roughness_tool-0.4.10.dev0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 # Read the contents of your requirements file
 def read_requirements(file_name):
     with open(file_name, 'r', encoding='utf-8') as f:
         return f.read().splitlines()
 
 setup(
     name='geo-roughness-tool',
-    version='0.4.0',
+    use_scm_version={
+        "local_scheme": "no-local-version",  # Exclude local version identifier
+        "version_scheme": "guess-next-dev",  # Optional, choose a version scheme
+    },
+    setup_requires=['setuptools-scm'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/lbatschelet/GeoRoughness-Tool',
     license='MIT',
     author='Lukas Batschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     long_description=read('README.md'),  # Use the README.md as the long description
```

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/application_driver.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/application_driver.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/defaults.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/defaults.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/geo_tiff_processor.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/geo_tiff_processor.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/processing_parameters.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/processing_parameters.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/classes/threshold_optimizer.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/classes/threshold_optimizer.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/cli_main.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/cli_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/analyze_and_optimize.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/analyze_and_optimize.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/footer_frame.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/footer_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/parameter_input.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/parameter_input.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/path_frame.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/path_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/preview_image.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_dark.png` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_dark.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_light.png` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_light.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_dark.ico` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/resources/app_icon_dark.ico`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_dark.png` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/resources/app_icon_dark.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui/resources/app_icon_light.png` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui/resources/app_icon_light.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/gui_main.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/gui_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from .gui.parameter_input import ParameterFrame
 from .gui.path_frame import PathFrame
 from .gui.preview_image import PreviewImage
 
 logger = logging.getLogger(__name__)
 
 
-
 class GUIMain(ctk.CTk):
     def __init__(self):
         super().__init__()
 
         self.driver = None
         self.title("GeoRoughness Tool")
         self.show_advanced_options = False
```

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool/log_config.py` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool/log_config.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.0/src/geo_roughness_tool.egg-info/PKG-INFO` & `geo_roughness_tool-0.4.10.dev0/src/geo_roughness_tool.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.4.0
+Version: 0.4.10.dev0
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
@@ -22,14 +22,19 @@
 Requires-Dist: customtkinter==5.2.2
 Requires-Dist: matplotlib==3.8.4
 Requires-Dist: numpy==1.26.4
 Requires-Dist: Pillow==10.3.0
 Requires-Dist: rasterio==1.3.10
 Requires-Dist: screeninfo==0.8.1
 Requires-Dist: setuptools==69.5.1
+Requires-Dist: requests==2.32.2
+Requires-Dist: packaging==24.0
+Requires-Dist: wheel==0.43.0
+Requires-Dist: twine==5.1.0
+Requires-Dist: setuptools-scm==8.1.0
 
 ![GeoRoughness_Banner_dark.png](.github%2Fresources%2FGeoRoughness_Banner_dark.png#gh-dark-mode-only)
 ![GeoRoughness_Banner_light.png](.github%2Fresources%2FGeoRoughness_Banner_light.png#gh-light-mode-only)
 
 # GeoRoughness Tool
 
 This is a spatial analysis tool for calculating surface roughness from Digital Elevation Models (DEMs). The tool
```

