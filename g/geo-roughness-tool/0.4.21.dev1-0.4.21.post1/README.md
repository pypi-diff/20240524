# Comparing `tmp/geo_roughness_tool-0.4.21.dev1.tar.gz` & `tmp/geo_roughness_tool-0.4.21.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_roughness_tool-0.4.21.dev1.tar", last modified: Fri May 24 09:50:54 2024, max compression
+gzip compressed data, was "geo_roughness_tool-0.4.21.post1.tar", last modified: Fri May 24 09:57:11 2024, max compression
```

## Comparing `geo_roughness_tool-0.4.21.dev1.tar` & `geo_roughness_tool-0.4.21.post1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.395396 geo_roughness_tool-0.4.21.dev1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.383396 geo_roughness_tool-0.4.21.dev1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.387396 geo_roughness_tool-0.4.21.dev1/.github/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   212970 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.github/resources/GeoRoughness_Banner_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)   226976 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.github/resources/GeoRoughness_Banner_light.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.387396 geo_roughness_tool-0.4.21.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.387396 geo_roughness_tool-0.4.21.dev1/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.idea/dem-roughness-calculator.iml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.387396 geo_roughness_tool-0.4.21.dev1/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.idea/other.xml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-24 09:50:53.000000 geo_roughness_tool-0.4.21.dev1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-24 09:50:54.395396 geo_roughness_tool-0.4.21.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 09:50:54.395396 geo_roughness_tool-0.4.21.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.383396 geo_roughness_tool-0.4.21.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.387396 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.391396 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/processing_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/threshold_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/cli_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.391396 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/analyze_and_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/footer_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/parameter_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/path_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/preview_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.395396 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_light.png
--rw-r--r--   0 runner    (1001) docker     (127)   114372 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/resources/app_icon_dark.ico
--rw-r--r--   0 runner    (1001) docker     (127)   371098 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/resources/app_icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)   400936 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/resources/app_icon_light.png
--rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-24 09:50:44.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:50:54.395396 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-24 09:50:54.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-24 09:50:54.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:50:54.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-24 09:50:54.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-24 09:50:54.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 09:50:54.000000 geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.336271 geo_roughness_tool-0.4.21.post1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.324271 geo_roughness_tool-0.4.21.post1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.324271 geo_roughness_tool-0.4.21.post1/.github/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   212970 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.github/resources/GeoRoughness_Banner_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   226976 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.github/resources/GeoRoughness_Banner_light.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.324271 geo_roughness_tool-0.4.21.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.328271 geo_roughness_tool-0.4.21.post1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.idea/dem-roughness-calculator.iml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.328271 geo_roughness_tool-0.4.21.post1/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.idea/other.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-24 09:57:10.000000 geo_roughness_tool-0.4.21.post1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-24 09:57:11.332271 geo_roughness_tool-0.4.21.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 09:57:11.336271 geo_roughness_tool-0.4.21.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.324271 geo_roughness_tool-0.4.21.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.328271 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.332271 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10503 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/threshold_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/cli_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.332271 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/analyze_and_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/footer_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/parameter_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/path_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/preview_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.332271 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   114372 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/resources/app_icon_dark.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   371098 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/resources/app_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   400936 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/resources/app_icon_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13712 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-24 09:57:00.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:57:11.332271 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-24 09:57:11.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-24 09:57:11.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:57:11.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-24 09:57:11.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-24 09:57:11.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 09:57:11.000000 geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool.egg-info/top_level.txt
```

### Comparing `geo_roughness_tool-0.4.21.dev1/.github/FUNDING.yml` & `geo_roughness_tool-0.4.21.post1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/.github/resources/GeoRoughness_Banner_dark.png` & `geo_roughness_tool-0.4.21.post1/.github/resources/GeoRoughness_Banner_dark.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/.github/resources/GeoRoughness_Banner_light.png` & `geo_roughness_tool-0.4.21.post1/.github/resources/GeoRoughness_Banner_light.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/.github/workflows/publish.yml` & `geo_roughness_tool-0.4.21.post1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/.gitignore` & `geo_roughness_tool-0.4.21.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/.idea/dem-roughness-calculator.iml` & `geo_roughness_tool-0.4.21.post1/.idea/dem-roughness-calculator.iml`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/CITATION.cff` & `geo_roughness_tool-0.4.21.post1/CITATION.cff`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 cff-version: 1.2.0
 message: "If you use this software in your work, please cite it using the following metadata."
 title: "GeoRoughness Tool"
-version: 0.4.20
+version: 0.4.21
 date-released: 2024-05-24
 
 authors:
   - family-names: "Batschelet"
     given-names: "Lukas"
     orcid: "0009-0005-0696-0285"
     affiliation: "Institute of Geography, University of Bern, Switzerland"
```

### Comparing `geo_roughness_tool-0.4.21.dev1/LICENSE` & `geo_roughness_tool-0.4.21.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/PKG-INFO` & `geo_roughness_tool-0.4.21.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.4.21.dev1
+Version: 0.4.21.post1
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
```

### Comparing `geo_roughness_tool-0.4.21.dev1/README.md` & `geo_roughness_tool-0.4.21.post1/README.md`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/setup.py` & `geo_roughness_tool-0.4.21.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 def read_requirements(file_name):
     with open(file_name, 'r', encoding='utf-8') as f:
         return f.read().splitlines()
 
 setup(
     name='geo-roughness-tool',
     use_scm_version={
-        "local_scheme": "no-local-version",  # Exclude local version identifier
-        "version_scheme": "guess-next-dev",  # Optional, choose a version scheme
+        "version_scheme": "post-release",
+        "local_scheme": "no-local-version"
     },
-    setup_requires=['setuptools-scm'],
+    setup_requires=["setuptools-scm"],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     url='https://github.com/lbatschelet/GeoRoughness-Tool',
     license='MIT',
     author='Lukas Batschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     long_description=read('README.md'),  # Use the README.md as the long description
```

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/application_driver.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/application_driver.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/defaults.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/defaults.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/geo_tiff_processor.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/geo_tiff_processor.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/processing_parameters.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/processing_parameters.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/classes/threshold_optimizer.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/classes/threshold_optimizer.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/cli_main.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/cli_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/analyze_and_optimize.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/analyze_and_optimize.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/footer_frame.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/footer_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/parameter_input.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/parameter_input.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/path_frame.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/path_frame.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/preview_image.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/preview_image.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_dark.png` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_dark.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_light.png` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/resources/GeoRoughness_Banner_long_light.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/resources/app_icon_dark.ico` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/resources/app_icon_dark.ico`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/resources/app_icon_dark.png` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/resources/app_icon_dark.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui/resources/app_icon_light.png` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui/resources/app_icon_light.png`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/gui_main.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/gui_main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/log_config.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/log_config.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool/main.py` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool/main.py`

 * *Files identical despite different names*

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool.egg-info/PKG-INFO` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-roughness-tool
-Version: 0.4.21.dev1
+Version: 0.4.21.post1
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/GeoRoughness-Tool
 Author: Lukas Batschelet
 License: MIT
 Project-URL: Documentation, https://github.com/lbatschelet/GeoRoughness-Tool/wiki
 Project-URL: Source, https://github.com/lbatschelet/GeoRoughness-Tool
 Project-URL: Tracker, https://github.com/lbatschelet/GeoRoughness-Tool/issues
```

### Comparing `geo_roughness_tool-0.4.21.dev1/src/geo_roughness_tool.egg-info/SOURCES.txt` & `geo_roughness_tool-0.4.21.post1/src/geo_roughness_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

