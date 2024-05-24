# Comparing `tmp/tvb-widgets-2.0.1.tar.gz` & `tmp/tvb-widgets-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-widgets-2.0.1.tar", last modified: Fri Apr 26 19:52:30 2024, max compression
+gzip compressed data, was "tvb-widgets-2.0.2.tar", last modified: Thu May 23 14:07:22 2024, max compression
```

## Comparing `tvb-widgets-2.0.1.tar` & `tvb-widgets-2.0.2.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.053959 tvb-widgets-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35796 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-26 19:52:30.053959 tvb-widgets-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:52:30.053959 tvb-widgets-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.041959 tvb-widgets-2.0.1/tvb_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-26 19:52:30.000000 tvb-widgets-2.0.1/tvb_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-26 19:52:30.000000 tvb-widgets-2.0.1/tvb_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:52:30.000000 tvb-widgets-2.0.1/tvb_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-26 19:52:30.000000 tvb-widgets-2.0.1/tvb_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 19:52:30.000000 tvb-widgets-2.0.1/tvb_widgets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.041959 tvb-widgets-2.0.1/tvbwidgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.045960 tvb-widgets-2.0.1/tvbwidgets/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.045960 tvb-widgets-2.0.1/tvbwidgets/core/hpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/hpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/hpc/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/hpc/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/ini_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.045960 tvb-widgets-2.0.1/tvbwidgets/core/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/logger/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/logger/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.045960 tvb-widgets-2.0.1/tvbwidgets/core/pse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/pse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13775 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/pse/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/pse/pse_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/pse/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/pse/toml_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.045960 tvb-widgets-2.0.1/tvbwidgets/core/simulator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/simulator/model_exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/core/simulator/tvb_integrators.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/readers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.045960 tvb-widgets-2.0.1/tvbwidgets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/test_drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/test_exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/test_head_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/test_phase_plane_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/test_pse_stage_in.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/test_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/test_tvb_integrators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.049960 tvb-widgets-2.0.1/tvbwidgets/tests/ts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/ts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/ts/test_data_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/ts/test_mne_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/ts/test_plotly_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/tests/ts/ts_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.049960 tvb-widgets-2.0.1/tvbwidgets/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/base_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.049960 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/connectivity_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/global_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    13468 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/outputs_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.049960 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_react/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_react/Connectivity.css
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_react/Connectivity.tsx
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_react/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_react/connectivity_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_react/connectivity_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/dicom_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/drive_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/head_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    36757 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/phase_plane_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/pse_launcher_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/pse_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/storage_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.053959 tvb-widgets-2.0.1/tvbwidgets/ui/ts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/ts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/ts/base_ts_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:30.053959 tvb-widgets-2.0.1/tvbwidgets/ui/ts/data_wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/ts/data_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/ts/data_wrappers/base_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/ts/data_wrappers/numpy_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/ts/data_wrappers/tvb_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/ts/mne_ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/ts/plotly_ts_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/ts/ts_widget_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-26 19:52:24.000000 tvb-widgets-2.0.1/tvbwidgets/ui/widget_with_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.373426 tvb-widgets-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35796 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-23 14:07:22.369426 tvb-widgets-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:07:22.373426 tvb-widgets-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.361426 tvb-widgets-2.0.2/tvb_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-23 14:07:22.000000 tvb-widgets-2.0.2/tvb_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-23 14:07:22.000000 tvb-widgets-2.0.2/tvb_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:07:22.000000 tvb-widgets-2.0.2/tvb_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-23 14:07:22.000000 tvb-widgets-2.0.2/tvb_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 14:07:22.000000 tvb-widgets-2.0.2/tvb_widgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.361426 tvb-widgets-2.0.2/tvbwidgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.365426 tvb-widgets-2.0.2/tvbwidgets/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.365426 tvb-widgets-2.0.2/tvbwidgets/core/hpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/hpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/hpc/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/hpc/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/ini_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.365426 tvb-widgets-2.0.2/tvbwidgets/core/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/logger/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/logger/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.365426 tvb-widgets-2.0.2/tvbwidgets/core/pse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/pse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13775 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/pse/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/pse/pse_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/pse/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/pse/toml_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.365426 tvb-widgets-2.0.2/tvbwidgets/core/simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/simulator/model_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/core/simulator/tvb_integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/readers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.365426 tvb-widgets-2.0.2/tvbwidgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/test_drive_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/test_exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/test_head_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/test_phase_plane_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/test_pse_stage_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/test_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/test_tvb_integrators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.365426 tvb-widgets-2.0.2/tvbwidgets/tests/ts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/ts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/ts/test_data_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/ts/test_mne_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/ts/test_plotly_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/tests/ts/ts_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.369426 tvb-widgets-2.0.2/tvbwidgets/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/base_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.369426 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/connectivity_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/global_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13468 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/outputs_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.369426 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_react/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_react/Connectivity.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_react/Connectivity.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_react/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_react/connectivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_react/connectivity_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/dicom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/drive_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/head_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36757 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/phase_plane_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/pse_launcher_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/pse_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/storage_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.369426 tvb-widgets-2.0.2/tvbwidgets/ui/ts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/ts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/ts/base_ts_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:22.369426 tvb-widgets-2.0.2/tvbwidgets/ui/ts/data_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/ts/data_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/ts/data_wrappers/base_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/ts/data_wrappers/numpy_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/ts/data_wrappers/tvb_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14483 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/ts/mne_ts_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/ts/plotly_ts_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/ts/ts_widget_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-23 14:07:12.000000 tvb-widgets-2.0.2/tvbwidgets/ui/widget_with_browser.py
```

### Comparing `tvb-widgets-2.0.1/LICENSE` & `tvb-widgets-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/PKG-INFO` & `tvb-widgets-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 2.0.1
+Version: 2.0.2
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
```

### Comparing `tvb-widgets-2.0.1/README.md` & `tvb-widgets-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/setup.py` & `tvb-widgets-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvb_widgets.egg-info/PKG-INFO` & `tvb-widgets-2.0.2/tvb_widgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvb-widgets
-Version: 2.0.1
+Version: 2.0.2
 Summary: GUI widgets for EBRAINS showcases
 Home-page: https://github.com/the-virtual-brain/tvb-widgets
 Author: TVB Widgets Team (Juelich SDL Neuroscience, INS - Marseille, Codemart)
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb widgets jupyterlab ebrains showcases
 Platform: UNKNOWN
```

### Comparing `tvb-widgets-2.0.1/tvb_widgets.egg-info/SOURCES.txt` & `tvb-widgets-2.0.2/tvb_widgets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 tvb_widgets.egg-info/PKG-INFO
 tvb_widgets.egg-info/SOURCES.txt
 tvb_widgets.egg-info/dependency_links.txt
 tvb_widgets.egg-info/requires.txt
 tvb_widgets.egg-info/top_level.txt
 tvbwidgets/__init__.py
```

### Comparing `tvb-widgets-2.0.1/tvbwidgets/__init__.py` & `tvb-widgets-2.0.2/tvbwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/api.py` & `tvb-widgets-2.0.2/tvbwidgets/api.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/auth.py` & `tvb-widgets-2.0.2/tvbwidgets/core/auth.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/exceptions.py` & `tvb-widgets-2.0.2/tvbwidgets/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/hpc/config.py` & `tvb-widgets-2.0.2/tvbwidgets/core/hpc/config.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/hpc/launcher.py` & `tvb-widgets-2.0.2/tvbwidgets/core/hpc/launcher.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/ini_parser.py` & `tvb-widgets-2.0.2/tvbwidgets/core/ini_parser.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/logger/builder.py` & `tvb-widgets-2.0.2/tvbwidgets/core/logger/builder.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/logger/logging.conf` & `tvb-widgets-2.0.2/tvbwidgets/core/logger/logging.conf`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/pse/parameters.py` & `tvb-widgets-2.0.2/tvbwidgets/core/pse/parameters.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/pse/pse_data.py` & `tvb-widgets-2.0.2/tvbwidgets/core/pse/pse_data.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/pse/toml_storage.py` & `tvb-widgets-2.0.2/tvbwidgets/core/pse/toml_storage.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/simulator/model_exporters.py` & `tvb-widgets-2.0.2/tvbwidgets/core/simulator/model_exporters.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/core/simulator/tvb_integrators.py` & `tvb-widgets-2.0.2/tvbwidgets/core/simulator/tvb_integrators.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/readers.py` & `tvb-widgets-2.0.2/tvbwidgets/readers.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/tests/test_base.py` & `tvb-widgets-2.0.2/tvbwidgets/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/tests/test_drive_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/tests/test_drive_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/tests/test_exporters.py` & `tvb-widgets-2.0.2/tvbwidgets/tests/test_exporters.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/tests/test_head_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/tests/test_head_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/tests/test_phase_plane_export.py` & `tvb-widgets-2.0.2/tvbwidgets/tests/test_phase_plane_export.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/tests/test_pse_stage_in.py` & `tvb-widgets-2.0.2/tvbwidgets/tests/test_pse_stage_in.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/tests/test_readers.py` & `tvb-widgets-2.0.2/tvbwidgets/tests/test_readers.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/tests/ts/test_data_wrappers.py` & `tvb-widgets-2.0.2/tvbwidgets/tests/ts/test_data_wrappers.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/tests/ts/test_mne_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/tests/ts/test_mne_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/tests/ts/test_plotly_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/tests/ts/test_plotly_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/tests/ts/ts_generator.py` & `tvb-widgets-2.0.2/tvbwidgets/tests/ts/ts_generator.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/base_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/base_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/connectivity_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/connectivity_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/global_context.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/global_context.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/operations.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/operations.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_ipy/outputs_3d.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_ipy/outputs_3d.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_react/Connectivity.tsx` & `tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_react/Connectivity.tsx`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_react/connectivity_model.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_react/connectivity_model.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/connectivity_react/connectivity_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/connectivity_react/connectivity_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/dicom_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/dicom_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/drive_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/drive_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/head_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/head_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/phase_plane_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/phase_plane_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/pse_launcher_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/pse_launcher_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/pse_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/pse_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/storage_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/storage_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/ts/base_ts_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/ts/base_ts_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/ts/data_wrappers/base_data_wrapper.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/ts/data_wrappers/base_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/ts/data_wrappers/numpy_data_wrapper.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/ts/data_wrappers/numpy_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/ts/data_wrappers/tvb_data_wrapper.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/ts/data_wrappers/tvb_data_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
     def __init__(self, data):
         # type: (TimeSeries) -> None
         if data is None or not isinstance(data, TimeSeries):
             raise InvalidInputException("Not a valid TVB TS " + str(data))
         self.data = data
         self.ch_names = []
-        variables_labels = data.variables_labels
-        if variables_labels is not None and variables_labels != []:
+        variables_labels = data.variables_labels    # this give a numpy.ndarray
+        if variables_labels is not None and variables_labels.size != 0:
             sv_options = [(variables_labels[idx], idx) for idx in range(len(variables_labels))]
             self.extra_dimensions = ABCDataWrapper.extra_dimensions.copy()
             self.extra_dimensions[1] = ("State var.", sv_options)
 
     @property
     def data_shape(self):
         # type: () -> tuple
```

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/ts/mne_ts_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/ts/mne_ts_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/ts/plotly_ts_widget.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/ts/plotly_ts_widget.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/ts/ts_widget_browser.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/ts/ts_widget_browser.py`

 * *Files identical despite different names*

### Comparing `tvb-widgets-2.0.1/tvbwidgets/ui/widget_with_browser.py` & `tvb-widgets-2.0.2/tvbwidgets/ui/widget_with_browser.py`

 * *Files identical despite different names*

