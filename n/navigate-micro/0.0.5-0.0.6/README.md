# Comparing `tmp/navigate-micro-0.0.5.tar.gz` & `tmp/navigate_micro-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "navigate-micro-0.0.5.tar", last modified: Wed Apr 10 12:01:58 2024, max compression
+gzip compressed data, was "navigate_micro-0.0.6.tar", last modified: Fri May 24 15:37:59 2024, max compression
```

## Comparing `navigate-micro-0.0.5.tar` & `navigate_micro-0.0.6.tar`

### file list

```diff
@@ -1,291 +1,305 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/
--rw-rw-rw-   0        0        0     2114 2024-04-10 12:01:23.000000 navigate-micro-0.0.5/LICENSE.md
--rw-rw-rw-   0        0        0      132 2024-04-10 12:01:23.000000 navigate-micro-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6595 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1878 2024-04-10 12:01:23.000000 navigate-micro-0.0.5/README.md
--rw-rw-rw-   0        0        0     1995 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.912177 navigate-micro-0.0.5/src/
--rw-rw-rw-   0        0        0        0 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.912177 navigate-micro-0.0.5/src/navigate/
--rw-rw-rw-   0        0        0        7 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/VERSION
--rw-rw-rw-   0        0        0      225 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/__init__.py
--rw-rw-rw-   0        0        0     3993 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/_commit.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.912177 navigate-micro-0.0.5/src/navigate/config/
--rw-rw-rw-   0        0        0       98 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/__init__.py
--rw-rw-rw-   0        0        0    37570 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/config.py
--rw-rw-rw-   0        0        0    11736 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/configuration.yaml
--rw-rw-rw-   0        0        0     2385 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/experiment.yml
--rw-rw-rw-   0        0        0       66 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/rest_api_config.yml
--rw-rw-rw-   0        0        0     6914 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/synthetic_configuration.yaml
--rw-rw-rw-   0        0        0     7197 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/waveform_constants.yml
--rw-rw-rw-   0        0        0      218 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/config/waveform_templates.yml
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.912177 navigate-micro-0.0.5/src/navigate/controller/
--rw-rw-rw-   0        0        0       62 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/__init__.py
--rw-rw-rw-   0        0        0    12782 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/configuration_controller.py
--rw-rw-rw-   0        0        0    49646 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/controller.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.927802 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/
--rw-rw-rw-   0        0        0     1427 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/__init__.py
--rw-rw-rw-   0        0        0    17550 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/acquire_bar_controller.py
--rw-rw-rw-   0        0        0    15957 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/adaptiveoptics_popup_controller.py
--rw-rw-rw-   0        0        0    10817 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/autofocus_popup_controller.py
--rw-rw-rw-   0        0        0     6105 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_map_setting_popup_controller.py
--rw-rw-rw-   0        0        0    22294 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_setting_controller.py
--rw-rw-rw-   0        0        0    44619 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_view_controller.py
--rw-rw-rw-   0        0        0    17711 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/channel_setting_controller.py
--rw-rw-rw-   0        0        0    35208 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/channels_tab_controller.py
--rw-rw-rw-   0        0        0     9611 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/feature_advanced_setting_controller.py
--rw-rw-rw-   0        0        0    29415 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/features_popup_controller.py
--rw-rw-rw-   0        0        0     3894 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/gui_controller.py
--rw-rw-rw-   0        0        0     9430 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/ilastik_popup_controller.py
--rw-rw-rw-   0        0        0     8431 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/keystroke_controller.py
--rw-rw-rw-   0        0        0    42034 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/menu_controller.py
--rw-rw-rw-   0        0        0     9733 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/microscope_popup_controller.py
--rw-rw-rw-   0        0        0    11435 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/multi_position_controller.py
--rw-rw-rw-   0        0        0    12864 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/plugins_controller.py
--rw-rw-rw-   0        0        0    22523 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/stage_controller.py
--rw-rw-rw-   0        0        0    16629 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/tiling_wizard_controller.py
--rw-rw-rw-   0        0        0    21786 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/tiling_wizard_controller2.py
--rw-rw-rw-   0        0        0    31409 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/waveform_popup_controller.py
--rw-rw-rw-   0        0        0    12872 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/sub_controllers/waveform_tab_controller.py
--rw-rw-rw-   0        0        0    16135 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/controller/thread_pool.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.927802 navigate-micro-0.0.5/src/navigate/log_files/
--rw-rw-rw-   0        0        0       58 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/log_files/__init__.py
--rw-rw-rw-   0        0        0     3721 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/log_files/filters.py
--rw-rw-rw-   0        0        0     7471 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/log_files/log_functions.py
--rw-rw-rw-   0        0        0     1305 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/log_files/logging.yml
--rw-rw-rw-   0        0        0     1315 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/log_files/model_logging.yml
--rw-rw-rw-   0        0        0     4445 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/main.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/
--rw-rw-rw-   0        0        0       76 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/analysis/
--rw-rw-rw-   0        0        0       82 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/analysis/__init__.py
--rw-rw-rw-   0        0        0    14091 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/analysis/boundary_detect.py
--rw-rw-rw-   0        0        0     5547 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/analysis/camera.py
--rw-rw-rw-   0        0        0     2858 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/analysis/image_contrast.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/concurrency/
--rw-rw-rw-   0        0        0       67 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/concurrency/__init__.py
--rw-rw-rw-   0        0        0    26823 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/concurrency/concurrency_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/data_sources/
--rw-rw-rw-   0        0        0      922 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/data_sources/__init__.py
--rw-rw-rw-   0        0        0    20357 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/data_sources/bdv_data_source.py
--rw-rw-rw-   0        0        0    12940 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/data_sources/data_source.py
--rw-rw-rw-   0        0        0    10817 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/data_sources/tiff_data_source.py
--rw-rw-rw-   0        0        0    42546 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/device_startup_functions.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/
--rw-rw-rw-   0        0        0       34 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/asi/
--rw-rw-rw-   0        0        0       69 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/asi/__init__.py
--rw-rw-rw-   0        0        0    25001 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/asi/asi_tiger_controller.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/coherent/
--rw-rw-rw-   0        0        0     6497 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/coherent/ObisLaser.py
--rw-rw-rw-   0        0        0       38 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/coherent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/dynamixel/
--rw-rw-rw-   0        0        0       40 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/dynamixel/__init__.py
--rw-rw-rw-   0        0        0    10609 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/dynamixel/dynamixel_functions.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/hamamatsu/
--rw-rw-rw-   0        0        0    41704 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/hamamatsu/HamamatsuAPI.py
--rw-rw-rw-   0        0        0       36 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/hamamatsu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/imagineoptics/
--rw-rw-rw-   0        0        0       51 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/imagineoptics/__init__.py
--rw-rw-rw-   0        0        0      481 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/imagineoptics/enums.py
--rw-rw-rw-   0        0        0    32812 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/imagineoptics/imop.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.943424 navigate-micro-0.0.5/src/navigate/model/devices/APIs/mcl/
--rw-rw-rw-   0        0        0       55 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/mcl/__init__.py
--rw-rw-rw-   0        0        0     5681 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/mcl/madlib.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/omicron/
--rw-rw-rw-   0        0        0    12303 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/omicron/LuxxLaser.py
--rw-rw-rw-   0        0        0       39 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/omicron/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/
--rw-rw-rw-   0        0        0     4461 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/
--rw-rw-rw-   0        0        0    10711 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/constants_generator.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/
--rw-rw-rw-   0        0        0        0 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/__init__.py
--rw-rw-rw-   0        0        0    43400 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/camera.py
--rw-rw-rw-   0        0        0    29219 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/
--rw-rw-rw-   0        0        0      413 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/camera_settings.py
--rw-rw-rw-   0        0        0     1239 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/change_settings_test.py
--rw-rw-rw-   0        0        0     2525 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/check_frame_status.py
--rw-rw-rw-   0        0        0     2692 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/live_mode.py
--rw-rw-rw-   0        0        0      940 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/meta_data.py
--rw-rw-rw-   0        0        0     2288 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_camera.py
--rw-rw-rw-   0        0        0     1927 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_rois.py
--rw-rw-rw-   0        0        0     1319 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/newest_frame.py
--rw-rw-rw-   0        0        0     1595 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/seq_mode.py
--rw-rw-rw-   0        0        0      494 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/single_image_polling.py
--rw-rw-rw-   0        0        0      395 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/single_image_polling_show.py
--rw-rw-rw-   0        0        0     3654 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/stream_to_disk.py
--rw-rw-rw-   0        0        0     1873 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/sw_trigger.py
--rw-rw-rw-   0        0        0    15288 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/test_camera.py
--rw-rw-rw-   0        0        0       39 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/sutter/
--rw-rw-rw-   0        0        0    20712 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/sutter/MP285.py
--rw-rw-rw-   0        0        0       48 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/sutter/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.959048 navigate-micro-0.0.5/src/navigate/model/devices/APIs/thorlabs/
--rw-rw-rw-   0        0        0       45 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/thorlabs/__init__.py
--rw-rw-rw-   0        0        0    18113 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/APIs/thorlabs/kcube_inertial.py
--rw-rw-rw-   0        0        0      671 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/camera/
--rw-rw-rw-   0        0        0       25 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/camera/__init__.py
--rw-rw-rw-   0        0        0     8334 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_base.py
--rw-rw-rw-   0        0        0    23489 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_hamamatsu.py
--rw-rw-rw-   0        0        0    23173 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_photometrics.py
--rw-rw-rw-   0        0        0    11490 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/daq/
--rw-rw-rw-   0        0        0       40 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/daq/__init__.py
--rw-rw-rw-   0        0        0     6238 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_base.py
--rw-rw-rw-   0        0        0    20126 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_ni.py
--rw-rw-rw-   0        0        0     6165 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/
--rw-rw-rw-   0        0        0       31 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/__init__.py
--rw-rw-rw-   0        0        0     7169 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_asi.py
--rw-rw-rw-   0        0        0     3650 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_base.py
--rw-rw-rw-   0        0        0    11305 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_sutter.py
--rw-rw-rw-   0        0        0     4140 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/galvo/
--rw-rw-rw-   0        0        0       31 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/galvo/__init__.py
--rw-rw-rw-   0        0        0     8952 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_base.py
--rw-rw-rw-   0        0        0     4389 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_ni.py
--rw-rw-rw-   0        0        0     2704 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/lasers/
--rw-rw-rw-   0        0        0       24 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/lasers/__init__.py
--rw-rw-rw-   0        0        0     3321 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_base.py
--rw-rw-rw-   0        0        0     7294 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_ni.py
--rw-rw-rw-   0        0        0     2786 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/mirrors/
--rw-rw-rw-   0        0        0       36 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/mirrors/__init__.py
--rw-rw-rw-   0        0        0     3141 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_base.py
--rw-rw-rw-   0        0        0     5128 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_imop.py
--rw-rw-rw-   0        0        0     2840 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_synthetic.py
--rw-rw-rw-   0        0        0     5222 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/objectives.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.974674 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/
--rw-rw-rw-   0        0        0       31 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/__init__.py
--rw-rw-rw-   0        0        0     9992 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_base.py
--rw-rw-rw-   0        0        0    10671 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_equipment_solutions.py
--rw-rw-rw-   0        0        0     4592 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_ni.py
--rw-rw-rw-   0        0        0     3052 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.990299 navigate-micro-0.0.5/src/navigate/model/devices/shutter/
--rw-rw-rw-   0        0        0       26 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/shutter/__init__.py
--rw-rw-rw-   0        0        0     3074 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_base.py
--rw-rw-rw-   0        0        0     2729 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_synthetic.py
--rw-rw-rw-   0        0        0     4183 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_ttl.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.990299 navigate-micro-0.0.5/src/navigate/model/devices/stages/
--rw-rw-rw-   0        0        0       24 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/__init__.py
--rw-rw-rw-   0        0        0    18031 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_asi.py
--rw-rw-rw-   0        0        0     8375 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_base.py
--rw-rw-rw-   0        0        0    11617 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_galvo.py
--rw-rw-rw-   0        0        0     6855 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_mcl.py
--rw-rw-rw-   0        0        0     9756 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_pi.py
--rw-rw-rw-   0        0        0    10457 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_sutter.py
--rw-rw-rw-   0        0        0     7634 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_synthetic.py
--rw-rw-rw-   0        0        0     8657 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_tl_kcube_inertial.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:57.990299 navigate-micro-0.0.5/src/navigate/model/devices/zoom/
--rw-rw-rw-   0        0        0       23 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/zoom/__init__.py
--rw-rw-rw-   0        0        0     5967 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_base.py
--rw-rw-rw-   0        0        0     9014 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_dynamixel.py
--rw-rw-rw-   0        0        0     2894 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_synthetic.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.005920 navigate-micro-0.0.5/src/navigate/model/features/
--rw-rw-rw-   0        0        0       62 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/__init__.py
--rw-rw-rw-   0        0        0    21608 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/adaptive_optics.py
--rw-rw-rw-   0        0        0     8529 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/auto_tile_scan.py
--rw-rw-rw-   0        0        0    20037 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/autofocus.py
--rw-rw-rw-   0        0        0    55561 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/common_features.py
--rw-rw-rw-   0        0        0    22979 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/cva_conpro.py
--rw-rw-rw-   0        0        0    42808 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/feature_container.py
--rw-rw-rw-   0        0        0    14931 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/feature_related_functions.py
--rw-rw-rw-   0        0        0    13532 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/image_writer.py
--rw-rw-rw-   0        0        0    19751 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/remove_empty_tiles.py
--rw-rw-rw-   0        0        0     9274 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/restful_features.py
--rw-rw-rw-   0        0        0    16368 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/features/volume_search.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.005920 navigate-micro-0.0.5/src/navigate/model/metadata_sources/
--rw-rw-rw-   0        0        0       43 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/metadata_sources/__init__.py
--rw-rw-rw-   0        0        0    20659 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/metadata_sources/bdv_metadata.py
--rw-rw-rw-   0        0        0    12574 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/metadata_sources/metadata.py
--rw-rw-rw-   0        0        0    10605 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/metadata_sources/ome_tiff_metadata.py
--rw-rw-rw-   0        0        0    35870 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/microscope.py
--rw-rw-rw-   0        0        0    57127 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/model.py
--rw-rw-rw-   0        0        0    10117 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/plugins_model.py
--rw-rw-rw-   0        0        0    14067 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/model/waveforms.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.005920 navigate-micro-0.0.5/src/navigate/plugins/
--rw-rw-rw-   0        0        0       25 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.005920 navigate-micro-0.0.5/src/navigate/tools/
--rw-rw-rw-   0        0        0       66 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/__init__.py
--rw-rw-rw-   0        0        0     3332 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/common_dict_tools.py
--rw-rw-rw-   0        0        0     4277 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/common_functions.py
--rw-rw-rw-   0        0        0     2887 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/decorators.py
--rw-rw-rw-   0        0        0     6897 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/file_functions.py
--rw-rw-rw-   0        0        0     4135 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/image.py
--rw-rw-rw-   0        0        0     5696 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/linear_algebra.py
--rw-rw-rw-   0        0        0     7854 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/main_functions.py
--rw-rw-rw-   0        0        0     8376 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/multipos_table_tools.py
--rw-rw-rw-   0        0        0     4004 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/sdf.py
--rw-rw-rw-   0        0        0     3268 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/waveform_template_funcs.py
--rw-rw-rw-   0        0        0     4254 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/tools/xml_tools.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.005920 navigate-micro-0.0.5/src/navigate/view/
--rw-rw-rw-   0        0        0       46 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.021545 navigate-micro-0.0.5/src/navigate/view/custom_widgets/
--rw-rw-rw-   0        0        0     3286 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/ArrowLabel.py
--rw-rw-rw-   0        0        0     7028 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/DockableNotebook.py
--rw-rw-rw-   0        0        0    11451 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/LabelInputWidgetFactory.py
--rw-rw-rw-   0        0        0       67 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/hover.py
--rw-rw-rw-   0        0        0     8768 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/hoverbar.py
--rw-rw-rw-   0        0        0     4905 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/hovermixin.py
--rw-rw-rw-   0        0        0     6301 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/popup.py
--rw-rw-rw-   0        0        0     5675 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/scrollbars.py
--rw-rw-rw-   0        0        0    39055 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/custom_widgets/validation.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.021545 navigate-micro-0.0.5/src/navigate/view/icon/
--rw-rw-rw-   0        0        0    67646 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/icon/mic.ico
--rw-rw-rw-   0        0        0   127742 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/icon/mic.png
--rw-rw-rw-   0        0        0   256647 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/icon/mic_orig.png
--rw-rw-rw-   0        0        0   364584 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/icon/splash_screen_image.png
--rw-rw-rw-   0        0        0     7364 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_application_window.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.021545 navigate-micro-0.0.5/src/navigate/view/main_window_content/
--rw-rw-rw-   0        0        0       46 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/__init__.py
--rw-rw-rw-   0        0        0     5490 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/acquire_notebook.py
--rw-rw-rw-   0        0        0    20237 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/camera_tab.py
--rw-rw-rw-   0        0        0    31198 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/channels_tab.py
--rw-rw-rw-   0        0        0    20004 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/display_notebook.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.021545 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/
--rw-rw-rw-   0        0        0    11248 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greydown.png
--rw-rw-rw-   0        0        0     5729 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greydown_disabled.png
--rw-rw-rw-   0        0        0    11254 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyleft.png
--rw-rw-rw-   0        0        0     5882 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyleft_disabled.png
--rw-rw-rw-   0        0        0    11078 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyright.png
--rw-rw-rw-   0        0        0     5883 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyright_disabled.png
--rw-rw-rw-   0        0        0    10935 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyup.png
--rw-rw-rw-   0        0        0     5636 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyup_disabled.png
--rw-rw-rw-   0        0        0     8912 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/images/wa_right.png
--rw-rw-rw-   0        0        0     3874 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/menus.py
--rw-rw-rw-   0        0        0    15198 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/multiposition_tab.py
--rw-rw-rw-   0        0        0     4246 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/settings_notebook.py
--rw-rw-rw-   0        0        0    30950 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/main_window_content/stage_tab.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/src/navigate/view/popups/
--rw-rw-rw-   0        0        0       59 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/__init__.py
--rw-rw-rw-   0        0        0     8160 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/acquire_popup.py
--rw-rw-rw-   0        0        0    14713 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/adaptiveoptics_popup.py
--rw-rw-rw-   0        0        0     8164 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/autofocus_setting_popup.py
--rw-rw-rw-   0        0        0     4976 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/camera_map_setting_popup.py
--rw-rw-rw-   0        0        0     5352 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/camera_view_popup_window.py
--rw-rw-rw-   0        0        0    18655 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/feature_list_popup.py
--rw-rw-rw-   0        0        0     6068 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/ilastik_setting_popup.py
--rw-rw-rw-   0        0        0     8312 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/microscope_setting_popup_window.py
--rw-rw-rw-   0        0        0     4554 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/plugins_popup.py
--rw-rw-rw-   0        0        0     8481 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/tiling_wizard_popup.py
--rw-rw-rw-   0        0        0    10122 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/tiling_wizard_popup2.py
--rw-rw-rw-   0        0        0    11807 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/popups/waveform_parameter_popup_window.py
--rw-rw-rw-   0        0        0     3667 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/src/navigate/view/splash_screen.py
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/src/navigate_micro.egg-info/
--rw-rw-rw-   0        0        0     6595 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12235 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      623 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-10 12:01:57.000000 navigate-micro-0.0.5/src/navigate_micro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 12:01:58.037174 navigate-micro-0.0.5/test/
--rw-rw-rw-   0        0        0     2198 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/test/test_commit.py
--rw-rw-rw-   0        0        0     2834 2024-04-10 12:01:24.000000 navigate-micro-0.0.5/test/test_main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.689031 navigate_micro-0.0.6/
+-rw-rw-rw-   0        0        0     2114 2024-05-24 15:37:29.000000 navigate_micro-0.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0      132 2024-05-24 15:37:29.000000 navigate_micro-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6645 2024-05-24 15:37:59.689031 navigate_micro-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1878 2024-05-24 15:37:29.000000 navigate_micro-0.0.6/README.md
+-rw-rw-rw-   0        0        0     2020 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 15:37:59.689031 navigate_micro-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.548295 navigate_micro-0.0.6/src/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.563918 navigate_micro-0.0.6/src/navigate/
+-rw-rw-rw-   0        0        0        7 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/VERSION
+-rw-rw-rw-   0        0        0      225 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/__init__.py
+-rw-rw-rw-   0        0        0     3993 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/_commit.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.563918 navigate_micro-0.0.6/src/navigate/config/
+-rw-rw-rw-   0        0        0       98 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/config/__init__.py
+-rw-rw-rw-   0        0        0    39595 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/config/config.py
+-rw-rw-rw-   0        0        0     9551 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/config/configuration.yaml
+-rw-rw-rw-   0        0        0    17358 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/config/configuration_database.py
+-rw-rw-rw-   0        0        0     2319 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/config/experiment.yml
+-rw-rw-rw-   0        0        0       66 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/config/rest_api_config.yml
+-rw-rw-rw-   0        0        0     6914 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/config/synthetic_configuration.yaml
+-rw-rw-rw-   0        0        0     7197 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/config/waveform_constants.yml
+-rw-rw-rw-   0        0        0      218 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/config/waveform_templates.yml
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.563918 navigate_micro-0.0.6/src/navigate/controller/
+-rw-rw-rw-   0        0        0       62 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/__init__.py
+-rw-rw-rw-   0        0        0    12782 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/configuration_controller.py
+-rw-rw-rw-   0        0        0    19030 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/configurator.py
+-rw-rw-rw-   0        0        0    50277 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/controller.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.580211 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/
+-rw-rw-rw-   0        0        0     1427 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/__init__.py
+-rw-rw-rw-   0        0        0    17550 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/acquire_bar_controller.py
+-rw-rw-rw-   0        0        0    15957 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/adaptiveoptics_popup_controller.py
+-rw-rw-rw-   0        0        0    10817 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/autofocus_popup_controller.py
+-rw-rw-rw-   0        0        0     6105 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/camera_map_setting_popup_controller.py
+-rw-rw-rw-   0        0        0    22306 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/camera_setting_controller.py
+-rw-rw-rw-   0        0        0    44619 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/camera_view_controller.py
+-rw-rw-rw-   0        0        0    17684 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/channel_setting_controller.py
+-rw-rw-rw-   0        0        0    35016 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/channels_tab_controller.py
+-rw-rw-rw-   0        0        0     9611 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/feature_advanced_setting_controller.py
+-rw-rw-rw-   0        0        0    29415 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/features_popup_controller.py
+-rw-rw-rw-   0        0        0     3894 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/gui_controller.py
+-rw-rw-rw-   0        0        0     9430 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/ilastik_popup_controller.py
+-rw-rw-rw-   0        0        0     8431 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/keystroke_controller.py
+-rw-rw-rw-   0        0        0    42223 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/menu_controller.py
+-rw-rw-rw-   0        0        0     9733 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/microscope_popup_controller.py
+-rw-rw-rw-   0        0        0    11131 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/multi_position_controller.py
+-rw-rw-rw-   0        0        0    15472 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/plugins_controller.py
+-rw-rw-rw-   0        0        0    23128 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/stage_controller.py
+-rw-rw-rw-   0        0        0    16629 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/tiling_wizard_controller.py
+-rw-rw-rw-   0        0        0    21786 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/tiling_wizard_controller2.py
+-rw-rw-rw-   0        0        0    31409 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/waveform_popup_controller.py
+-rw-rw-rw-   0        0        0    13415 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/sub_controllers/waveform_tab_controller.py
+-rw-rw-rw-   0        0        0    16135 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/controller/thread_pool.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.580211 navigate_micro-0.0.6/src/navigate/log_files/
+-rw-rw-rw-   0        0        0       58 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/log_files/__init__.py
+-rw-rw-rw-   0        0        0     3721 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/log_files/filters.py
+-rw-rw-rw-   0        0        0     7471 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/log_files/log_functions.py
+-rw-rw-rw-   0        0        0     1305 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/log_files/logging.yml
+-rw-rw-rw-   0        0        0     1315 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/log_files/model_logging.yml
+-rw-rw-rw-   0        0        0     4648 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.580211 navigate_micro-0.0.6/src/navigate/model/
+-rw-rw-rw-   0        0        0       76 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.580211 navigate_micro-0.0.6/src/navigate/model/analysis/
+-rw-rw-rw-   0        0        0       82 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/analysis/__init__.py
+-rw-rw-rw-   0        0        0    14091 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/analysis/boundary_detect.py
+-rw-rw-rw-   0        0        0     5547 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/analysis/camera.py
+-rw-rw-rw-   0        0        0     2858 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/analysis/image_contrast.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.580211 navigate_micro-0.0.6/src/navigate/model/concurrency/
+-rw-rw-rw-   0        0        0       67 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/concurrency/__init__.py
+-rw-rw-rw-   0        0        0    26823 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/concurrency/concurrency_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/data_sources/
+-rw-rw-rw-   0        0        0     1064 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/data_sources/__init__.py
+-rw-rw-rw-   0        0        0    12914 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/data_sources/bdv_data_source.py
+-rw-rw-rw-   0        0        0    13402 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/data_sources/data_source.py
+-rw-rw-rw-   0        0        0     9028 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/data_sources/pyramidal_data_source.py
+-rw-rw-rw-   0        0        0    10424 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/data_sources/tiff_data_source.py
+-rw-rw-rw-   0        0        0     6655 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/data_sources/zarr_data_source.py
+-rw-rw-rw-   0        0        0    48124 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/device_startup_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/APIs/
+-rw-rw-rw-   0        0        0       34 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/APIs/asi/
+-rw-rw-rw-   0        0        0       69 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/asi/__init__.py
+-rw-rw-rw-   0        0        0     1562 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/asi/asi_MFC_controller.py
+-rw-rw-rw-   0        0        0    23436 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/asi/asi_MS2000_controller.py
+-rw-rw-rw-   0        0        0    25046 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/asi/asi_tiger_controller.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/APIs/coherent/
+-rw-rw-rw-   0        0        0     6497 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/coherent/ObisLaser.py
+-rw-rw-rw-   0        0        0       38 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/coherent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/APIs/dynamixel/
+-rw-rw-rw-   0        0        0       40 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/dynamixel/__init__.py
+-rw-rw-rw-   0        0        0    10609 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/dynamixel/dynamixel_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/APIs/hamamatsu/
+-rw-rw-rw-   0        0        0    41704 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/hamamatsu/HamamatsuAPI.py
+-rw-rw-rw-   0        0        0       36 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/hamamatsu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/APIs/imagineoptics/
+-rw-rw-rw-   0        0        0       51 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/imagineoptics/__init__.py
+-rw-rw-rw-   0        0        0      481 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/imagineoptics/enums.py
+-rw-rw-rw-   0        0        0    32812 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/imagineoptics/imop.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/APIs/mcl/
+-rw-rw-rw-   0        0        0       55 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/mcl/__init__.py
+-rw-rw-rw-   0        0        0     5681 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/mcl/madlib.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/APIs/omicron/
+-rw-rw-rw-   0        0        0    12303 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/omicron/LuxxLaser.py
+-rw-rw-rw-   0        0        0       39 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/omicron/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/
+-rw-rw-rw-   0        0        0     4461 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.595241 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/
+-rw-rw-rw-   0        0        0    10711 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/constants_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.610902 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/__init__.py
+-rw-rw-rw-   0        0        0    43400 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/camera.py
+-rw-rw-rw-   0        0        0    29219 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.610902 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/
+-rw-rw-rw-   0        0        0      413 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/camera_settings.py
+-rw-rw-rw-   0        0        0     1239 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/change_settings_test.py
+-rw-rw-rw-   0        0        0     2525 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/check_frame_status.py
+-rw-rw-rw-   0        0        0     2692 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/live_mode.py
+-rw-rw-rw-   0        0        0      940 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/meta_data.py
+-rw-rw-rw-   0        0        0     2288 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_camera.py
+-rw-rw-rw-   0        0        0     1927 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_rois.py
+-rw-rw-rw-   0        0        0     1319 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/newest_frame.py
+-rw-rw-rw-   0        0        0     1595 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/seq_mode.py
+-rw-rw-rw-   0        0        0      494 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/single_image_polling.py
+-rw-rw-rw-   0        0        0      395 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/single_image_polling_show.py
+-rw-rw-rw-   0        0        0     3654 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/stream_to_disk.py
+-rw-rw-rw-   0        0        0     1873 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/sw_trigger.py
+-rw-rw-rw-   0        0        0    15288 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/test_camera.py
+-rw-rw-rw-   0        0        0       39 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.610902 navigate_micro-0.0.6/src/navigate/model/devices/APIs/sutter/
+-rw-rw-rw-   0        0        0    20712 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/sutter/MP285.py
+-rw-rw-rw-   0        0        0       48 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/sutter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.610902 navigate_micro-0.0.6/src/navigate/model/devices/APIs/thorlabs/
+-rw-rw-rw-   0        0        0       45 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/thorlabs/__init__.py
+-rw-rw-rw-   0        0        0    18113 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/thorlabs/kcube_inertial.py
+-rw-rw-rw-   0        0        0    19802 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/APIs/thorlabs/kcube_steppermotor.py
+-rw-rw-rw-   0        0        0      671 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.610902 navigate_micro-0.0.6/src/navigate/model/devices/camera/
+-rw-rw-rw-   0        0        0      280 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/camera/__init__.py
+-rw-rw-rw-   0        0        0     8334 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/camera/camera_base.py
+-rw-rw-rw-   0        0        0    24310 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/camera/camera_hamamatsu.py
+-rw-rw-rw-   0        0        0    18162 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/camera/camera_photometrics.py
+-rw-rw-rw-   0        0        0    11269 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/camera/camera_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.626531 navigate_micro-0.0.6/src/navigate/model/devices/daq/
+-rw-rw-rw-   0        0        0      122 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/daq/__init__.py
+-rw-rw-rw-   0        0        0     6238 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/daq/daq_base.py
+-rw-rw-rw-   0        0        0    20126 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/daq/daq_ni.py
+-rw-rw-rw-   0        0        0     6165 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/daq/daq_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.626531 navigate_micro-0.0.6/src/navigate/model/devices/filter_wheel/
+-rw-rw-rw-   0        0        0      179 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/filter_wheel/__init__.py
+-rw-rw-rw-   0        0        0     7169 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/filter_wheel/filter_wheel_asi.py
+-rw-rw-rw-   0        0        0     3650 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/filter_wheel/filter_wheel_base.py
+-rw-rw-rw-   0        0        0    11305 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/filter_wheel/filter_wheel_sutter.py
+-rw-rw-rw-   0        0        0     4140 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/filter_wheel/filter_wheel_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.626531 navigate_micro-0.0.6/src/navigate/model/devices/galvo/
+-rw-rw-rw-   0        0        0      106 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/galvo/__init__.py
+-rw-rw-rw-   0        0        0     8846 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/galvo/galvo_base.py
+-rw-rw-rw-   0        0        0     4389 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/galvo/galvo_ni.py
+-rw-rw-rw-   0        0        0     2704 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/galvo/galvo_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.626531 navigate_micro-0.0.6/src/navigate/model/devices/lasers/
+-rw-rw-rw-   0        0        0       99 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/lasers/__init__.py
+-rw-rw-rw-   0        0        0     3321 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/lasers/laser_base.py
+-rw-rw-rw-   0        0        0     7294 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/lasers/laser_ni.py
+-rw-rw-rw-   0        0        0     2786 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/lasers/laser_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.626531 navigate_micro-0.0.6/src/navigate/model/devices/mirrors/
+-rw-rw-rw-   0        0        0      114 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/mirrors/__init__.py
+-rw-rw-rw-   0        0        0     3141 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/mirrors/mirror_base.py
+-rw-rw-rw-   0        0        0     5128 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/mirrors/mirror_imop.py
+-rw-rw-rw-   0        0        0     2840 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/mirrors/mirror_synthetic.py
+-rw-rw-rw-   0        0        0     5222 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/objectives.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.626531 navigate_micro-0.0.6/src/navigate/model/devices/remote_focus/
+-rw-rw-rw-   0        0        0      171 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/remote_focus/__init__.py
+-rw-rw-rw-   0        0        0     9886 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/remote_focus/remote_focus_base.py
+-rw-rw-rw-   0        0        0    10668 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/remote_focus/remote_focus_equipment_solutions.py
+-rw-rw-rw-   0        0        0     4592 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/remote_focus/remote_focus_ni.py
+-rw-rw-rw-   0        0        0     3052 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/remote_focus/remote_focus_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.626531 navigate_micro-0.0.6/src/navigate/model/devices/shutter/
+-rw-rw-rw-   0        0        0      110 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/shutter/__init__.py
+-rw-rw-rw-   0        0        0     3074 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/shutter/laser_shutter_base.py
+-rw-rw-rw-   0        0        0     2729 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/shutter/laser_shutter_synthetic.py
+-rw-rw-rw-   0        0        0     4183 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/shutter/laser_shutter_ttl.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.642158 navigate_micro-0.0.6/src/navigate/model/devices/stages/
+-rw-rw-rw-   0        0        0      333 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/__init__.py
+-rw-rw-rw-   0        0        0    18031 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_asi.py
+-rw-rw-rw-   0        0        0     2717 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_asi_MFCTwoThousand.py
+-rw-rw-rw-   0        0        0    20160 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_asi_MSTwoThousand.py
+-rw-rw-rw-   0        0        0     8375 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_base.py
+-rw-rw-rw-   0        0        0    11906 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_galvo.py
+-rw-rw-rw-   0        0        0     6855 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_mcl.py
+-rw-rw-rw-   0        0        0     9756 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_pi.py
+-rw-rw-rw-   0        0        0    10457 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_sutter.py
+-rw-rw-rw-   0        0        0     7634 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_synthetic.py
+-rw-rw-rw-   0        0        0     8657 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_tl_kcube_inertial.py
+-rw-rw-rw-   0        0        0     9882 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_tl_kcube_steppermotor.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.642158 navigate_micro-0.0.6/src/navigate/model/devices/zoom/
+-rw-rw-rw-   0        0        0      115 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/zoom/__init__.py
+-rw-rw-rw-   0        0        0     5967 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/zoom/zoom_base.py
+-rw-rw-rw-   0        0        0     9014 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/zoom/zoom_dynamixel.py
+-rw-rw-rw-   0        0        0     2894 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/devices/zoom/zoom_synthetic.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.642158 navigate_micro-0.0.6/src/navigate/model/features/
+-rw-rw-rw-   0        0        0       62 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/__init__.py
+-rw-rw-rw-   0        0        0    21608 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/adaptive_optics.py
+-rw-rw-rw-   0        0        0     8529 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/auto_tile_scan.py
+-rw-rw-rw-   0        0        0    20037 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/autofocus.py
+-rw-rw-rw-   0        0        0    55644 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/common_features.py
+-rw-rw-rw-   0        0        0    22979 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/cva_conpro.py
+-rw-rw-rw-   0        0        0    42808 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/feature_container.py
+-rw-rw-rw-   0        0        0    14931 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/feature_related_functions.py
+-rw-rw-rw-   0        0        0    13706 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/image_writer.py
+-rw-rw-rw-   0        0        0    19751 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/remove_empty_tiles.py
+-rw-rw-rw-   0        0        0     9534 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/restful_features.py
+-rw-rw-rw-   0        0        0    16368 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/features/volume_search.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.657783 navigate_micro-0.0.6/src/navigate/model/metadata_sources/
+-rw-rw-rw-   0        0        0       43 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/metadata_sources/__init__.py
+-rw-rw-rw-   0        0        0    20873 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/metadata_sources/bdv_metadata.py
+-rw-rw-rw-   0        0        0    12651 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/metadata_sources/metadata.py
+-rw-rw-rw-   0        0        0    10605 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/metadata_sources/ome_tiff_metadata.py
+-rw-rw-rw-   0        0        0     7684 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/metadata_sources/zarr_metadata.py
+-rw-rw-rw-   0        0        0    36011 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/microscope.py
+-rw-rw-rw-   0        0        0    57233 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/model.py
+-rw-rw-rw-   0        0        0    11634 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/plugins_model.py
+-rw-rw-rw-   0        0        0    14067 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/model/waveforms.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.657783 navigate_micro-0.0.6/src/navigate/plugins/
+-rw-rw-rw-   0        0        0       25 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.657783 navigate_micro-0.0.6/src/navigate/tools/
+-rw-rw-rw-   0        0        0       66 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/__init__.py
+-rw-rw-rw-   0        0        0     3332 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/common_dict_tools.py
+-rw-rw-rw-   0        0        0     4277 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/common_functions.py
+-rw-rw-rw-   0        0        0     2887 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/decorators.py
+-rw-rw-rw-   0        0        0     6897 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/file_functions.py
+-rw-rw-rw-   0        0        0     4135 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/image.py
+-rw-rw-rw-   0        0        0     5696 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/linear_algebra.py
+-rw-rw-rw-   0        0        0     8285 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/main_functions.py
+-rw-rw-rw-   0        0        0     8376 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/multipos_table_tools.py
+-rw-rw-rw-   0        0        0     4387 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/sdf.py
+-rw-rw-rw-   0        0        0     4625 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/slicing.py
+-rw-rw-rw-   0        0        0     3268 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/waveform_template_funcs.py
+-rw-rw-rw-   0        0        0     4254 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/tools/xml_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.657783 navigate_micro-0.0.6/src/navigate/view/
+-rw-rw-rw-   0        0        0       46 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/__init__.py
+-rw-rw-rw-   0        0        0    20588 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/configurator_application_window.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.673408 navigate_micro-0.0.6/src/navigate/view/custom_widgets/
+-rw-rw-rw-   0        0        0     3286 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/custom_widgets/ArrowLabel.py
+-rw-rw-rw-   0        0        0     1234 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/custom_widgets/CollapsibleFrame.py
+-rw-rw-rw-   0        0        0     7028 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/custom_widgets/DockableNotebook.py
+-rw-rw-rw-   0        0        0    11451 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/custom_widgets/LabelInputWidgetFactory.py
+-rw-rw-rw-   0        0        0       67 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/custom_widgets/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/custom_widgets/hover.py
+-rw-rw-rw-   0        0        0     8768 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/custom_widgets/hoverbar.py
+-rw-rw-rw-   0        0        0     4905 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/custom_widgets/hovermixin.py
+-rw-rw-rw-   0        0        0     6301 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/custom_widgets/popup.py
+-rw-rw-rw-   0        0        0     5675 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/custom_widgets/scrollbars.py
+-rw-rw-rw-   0        0        0    39055 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/custom_widgets/validation.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.673408 navigate_micro-0.0.6/src/navigate/view/icon/
+-rw-rw-rw-   0        0        0    67646 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/icon/mic.ico
+-rw-rw-rw-   0        0        0   127742 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/icon/mic.png
+-rw-rw-rw-   0        0        0   256647 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/icon/mic_orig.png
+-rw-rw-rw-   0        0        0   364584 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/icon/splash_screen_image.png
+-rw-rw-rw-   0        0        0     7116 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_application_window.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.673408 navigate_micro-0.0.6/src/navigate/view/main_window_content/
+-rw-rw-rw-   0        0        0       46 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/__init__.py
+-rw-rw-rw-   0        0        0     5490 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/acquire_notebook.py
+-rw-rw-rw-   0        0        0    20237 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/camera_tab.py
+-rw-rw-rw-   0        0        0    31265 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/channels_tab.py
+-rw-rw-rw-   0        0        0    20004 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/display_notebook.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.673408 navigate_micro-0.0.6/src/navigate/view/main_window_content/images/
+-rw-rw-rw-   0        0        0    11248 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greydown.png
+-rw-rw-rw-   0        0        0     5729 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greydown_disabled.png
+-rw-rw-rw-   0        0        0    11254 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyleft.png
+-rw-rw-rw-   0        0        0     5882 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyleft_disabled.png
+-rw-rw-rw-   0        0        0    11078 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyright.png
+-rw-rw-rw-   0        0        0     5883 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyright_disabled.png
+-rw-rw-rw-   0        0        0    10935 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyup.png
+-rw-rw-rw-   0        0        0     5636 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyup_disabled.png
+-rw-rw-rw-   0        0        0     8912 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/images/wa_right.png
+-rw-rw-rw-   0        0        0     3874 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/menus.py
+-rw-rw-rw-   0        0        0    15198 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/multiposition_tab.py
+-rw-rw-rw-   0        0        0     4246 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/settings_notebook.py
+-rw-rw-rw-   0        0        0    30950 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/main_window_content/stage_tab.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.689031 navigate_micro-0.0.6/src/navigate/view/popups/
+-rw-rw-rw-   0        0        0       59 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/__init__.py
+-rw-rw-rw-   0        0        0     8160 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/acquire_popup.py
+-rw-rw-rw-   0        0        0    14713 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/adaptiveoptics_popup.py
+-rw-rw-rw-   0        0        0     8164 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/autofocus_setting_popup.py
+-rw-rw-rw-   0        0        0     4976 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/camera_map_setting_popup.py
+-rw-rw-rw-   0        0        0     5352 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/camera_view_popup_window.py
+-rw-rw-rw-   0        0        0    18655 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/feature_list_popup.py
+-rw-rw-rw-   0        0        0     6068 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/ilastik_setting_popup.py
+-rw-rw-rw-   0        0        0     8312 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/microscope_setting_popup_window.py
+-rw-rw-rw-   0        0        0     4554 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/plugins_popup.py
+-rw-rw-rw-   0        0        0     8481 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/tiling_wizard_popup.py
+-rw-rw-rw-   0        0        0    10122 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/tiling_wizard_popup2.py
+-rw-rw-rw-   0        0        0    11807 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/popups/waveform_parameter_popup_window.py
+-rw-rw-rw-   0        0        0     3667 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/src/navigate/view/splash_screen.py
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.689031 navigate_micro-0.0.6/src/navigate_micro.egg-info/
+-rw-rw-rw-   0        0        0     6645 2024-05-24 15:37:59.000000 navigate_micro-0.0.6/src/navigate_micro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12989 2024-05-24 15:37:59.000000 navigate_micro-0.0.6/src/navigate_micro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 15:37:59.000000 navigate_micro-0.0.6/src/navigate_micro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-24 15:37:59.000000 navigate_micro-0.0.6/src/navigate_micro.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      641 2024-05-24 15:37:59.000000 navigate_micro-0.0.6/src/navigate_micro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-24 15:37:59.000000 navigate_micro-0.0.6/src/navigate_micro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 15:37:59.689031 navigate_micro-0.0.6/test/
+-rw-rw-rw-   0        0        0     2198 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/test/test_commit.py
+-rw-rw-rw-   0        0        0     2834 2024-05-24 15:37:30.000000 navigate_micro-0.0.6/test/test_main.py
```

### Comparing `navigate-micro-0.0.5/LICENSE.md` & `navigate_micro-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/PKG-INFO` & `navigate_micro-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navigate-micro
-Version: 0.0.5
+Version: 0.0.6
 Summary: Open source, smart, light-sheet microscopy control software.
 Author: The Dean Lab, UT Southwestern Medical Center
 License: Copyright (c) 2021-2023 The University of Texas Southwestern Medical Center.
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are
@@ -73,14 +73,15 @@
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xvfb; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: jupyterlab; extra == "dev"
+Requires-Dist: pydantic-ome-ngff; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: nbconvert; extra == "docs"
 Requires-Dist: sphinx<6.0.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-issues; extra == "docs"
```

### Comparing `navigate-micro-0.0.5/README.md` & `navigate_micro-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/pyproject.toml` & `navigate_micro-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -92,34 +92,36 @@
 000005b0: 5b0d 0a20 2020 2022 7079 7465 7374 222c  [..    "pytest",
 000005c0: 0d0a 2020 2020 2270 7974 6573 742d 7876  ..    "pytest-xv
 000005d0: 6662 222c 0d0a 2020 2020 2270 7974 6573  fb",..    "pytes
 000005e0: 742d 636f 7622 2c0d 0a20 2020 2022 7072  t-cov",..    "pr
 000005f0: 652d 636f 6d6d 6974 222c 0d0a 2020 2020  e-commit",..    
 00000600: 2269 7079 6b65 726e 656c 222c 0d0a 2020  "ipykernel",..  
 00000610: 2020 226a 7570 7974 6572 6c61 6222 2c0d    "jupyterlab",.
-00000620: 0a20 2020 205d 0d0a 0d0a 646f 6373 203d  .    ]....docs =
-00000630: 205b 0d0a 2020 2020 226e 756d 7079 646f   [..    "numpydo
-00000640: 6322 2c0d 0a20 2020 2022 6e62 636f 6e76  c",..    "nbconv
-00000650: 6572 7422 2c0d 0a20 2020 2022 7370 6869  ert",..    "sphi
-00000660: 6e78 3c36 2e30 2e30 222c 0d0a 2020 2020  nx<6.0.0",..    
-00000670: 2273 7068 696e 785f 7274 645f 7468 656d  "sphinx_rtd_them
-00000680: 6522 2c0d 0a20 2020 2022 7370 6869 6e78  e",..    "sphinx
-00000690: 2d63 6f70 7962 7574 746f 6e22 2c0d 0a20  -copybutton",.. 
-000006a0: 2020 2022 7370 6869 6e78 2d69 7373 7565     "sphinx-issue
-000006b0: 7322 2c0d 0a20 2020 2022 7370 6869 6e78  s",..    "sphinx
-000006c0: 2d64 6573 6967 6e22 2c0d 0a20 2020 2022  -design",..    "
-000006d0: 7079 7961 6d6c 222c 0d0a 2020 2020 2270  pyyaml",..    "p
-000006e0: 7964 6174 615f 7370 6869 6e78 5f74 6865  ydata_sphinx_the
-000006f0: 6d65 3d3d 302e 3130 2e30 7263 3222 2c0d  me==0.10.0rc2",.
-00000700: 0a20 2020 2022 7370 6869 6e78 2d74 6f6f  .    "sphinx-too
-00000710: 6c62 6f78 220d 0a5d 0d0a 0d0a 726f 626f  lbox"..]....robo
-00000720: 7420 3d20 5b0d 0a20 2020 2022 6d65 6361  t = [..    "meca
-00000730: 6465 6d69 6370 7922 2c0d 0a5d 0d0a 0d0a  demicpy",..]....
-00000740: 5b70 726f 6a65 6374 2e75 726c 735d 0d0a  [project.urls]..
-00000750: 536f 7572 6365 203d 2022 6874 7470 733a  Source = "https:
-00000760: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6865  //github.com/The
-00000770: 4465 616e 4c61 622f 6e61 7669 6761 7465  DeanLab/navigate
-00000780: 220d 0a0d 0a5b 746f 6f6c 2e73 6574 7570  "....[tool.setup
-00000790: 746f 6f6c 732e 6479 6e61 6d69 635d 0d0a  tools.dynamic]..
-000007a0: 7665 7273 696f 6e20 3d20 7b66 696c 6520  version = {file 
-000007b0: 3d20 2273 7263 2f6e 6176 6967 6174 652f  = "src/navigate/
-000007c0: 5645 5253 494f 4e22 7d0d 0a              VERSION"}..
+00000620: 0a20 2020 2022 7079 6461 6e74 6963 2d6f  .    "pydantic-o
+00000630: 6d65 2d6e 6766 6622 0d0a 2020 2020 5d0d  me-ngff"..    ].
+00000640: 0a0d 0a64 6f63 7320 3d20 5b0d 0a20 2020  ...docs = [..   
+00000650: 2022 6e75 6d70 7964 6f63 222c 0d0a 2020   "numpydoc",..  
+00000660: 2020 226e 6263 6f6e 7665 7274 222c 0d0a    "nbconvert",..
+00000670: 2020 2020 2273 7068 696e 783c 362e 302e      "sphinx<6.0.
+00000680: 3022 2c0d 0a20 2020 2022 7370 6869 6e78  0",..    "sphinx
+00000690: 5f72 7464 5f74 6865 6d65 222c 0d0a 2020  _rtd_theme",..  
+000006a0: 2020 2273 7068 696e 782d 636f 7079 6275    "sphinx-copybu
+000006b0: 7474 6f6e 222c 0d0a 2020 2020 2273 7068  tton",..    "sph
+000006c0: 696e 782d 6973 7375 6573 222c 0d0a 2020  inx-issues",..  
+000006d0: 2020 2273 7068 696e 782d 6465 7369 676e    "sphinx-design
+000006e0: 222c 0d0a 2020 2020 2270 7979 616d 6c22  ",..    "pyyaml"
+000006f0: 2c0d 0a20 2020 2022 7079 6461 7461 5f73  ,..    "pydata_s
+00000700: 7068 696e 785f 7468 656d 653d 3d30 2e31  phinx_theme==0.1
+00000710: 302e 3072 6332 222c 0d0a 2020 2020 2273  0.0rc2",..    "s
+00000720: 7068 696e 782d 746f 6f6c 626f 7822 0d0a  phinx-toolbox"..
+00000730: 5d0d 0a0d 0a72 6f62 6f74 203d 205b 0d0a  ]....robot = [..
+00000740: 2020 2020 226d 6563 6164 656d 6963 7079      "mecademicpy
+00000750: 222c 0d0a 5d0d 0a0d 0a5b 7072 6f6a 6563  ",..]....[projec
+00000760: 742e 7572 6c73 5d0d 0a53 6f75 7263 6520  t.urls]..Source 
+00000770: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
+00000780: 622e 636f 6d2f 5468 6544 6561 6e4c 6162  b.com/TheDeanLab
+00000790: 2f6e 6176 6967 6174 6522 0d0a 0d0a 5b74  /navigate"....[t
+000007a0: 6f6f 6c2e 7365 7475 7074 6f6f 6c73 2e64  ool.setuptools.d
+000007b0: 796e 616d 6963 5d0d 0a76 6572 7369 6f6e  ynamic]..version
+000007c0: 203d 207b 6669 6c65 203d 2022 7372 632f   = {file = "src/
+000007d0: 6e61 7669 6761 7465 2f56 4552 5349 4f4e  navigate/VERSION
+000007e0: 227d 0d0a                                "}..
```

### Comparing `navigate-micro-0.0.5/src/navigate/_commit.py` & `navigate_micro-0.0.6/src/navigate/_commit.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/config/config.py` & `navigate_micro-0.0.6/src/navigate/config/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 from os.path import isfile
 from multiprocessing.managers import ListProxy, DictProxy
 
 # Third Party Imports
 import yaml
 
 # Local Imports
-
+from navigate.tools.common_functions import build_ref_name
 
 def get_navigate_path():
     """Establish a program home directory in AppData/Local/.navigate for Windows
     or ~/.navigate for Mac and Linux.
 
     Returns
     -------
@@ -669,30 +669,25 @@
         "MultiPositions" not in configuration["experiment"]
         or type(configuration["experiment"]["MultiPositions"]) is not ListProxy
     ):
         update_config_dict(manager, configuration["experiment"], "MultiPositions", [])
     position_ids = []
     multipositions = configuration["experiment"]["MultiPositions"]
     for i, position in enumerate(multipositions):
-        for axis in ["x", "y", "z", "theta", "f"]:
             try:
-                position[axis] = float(position[axis])
-            except ValueError:
+                for j in range(5):
+                    float(position[j])
+            except (ValueError, KeyError):
                 position_ids.append(i)
-                break
+                
     for idx in position_ids[::-1]:
         del multipositions[idx]
     if len(multipositions) < 1:
-        multipositions.append(None)
-        update_config_dict(
-            manager,
-            multipositions,
-            0,
-            {"x": 10.0, "y": 10.0, "z": 10.0, "f": 10.0, "theta": 10.0},
-        )
+        multipositions.append([10.0, 10.0, 10.0, 10.0, 10.0])
+
     microscope_setting_dict["multiposition_count"] = len(multipositions)
 
 
 def verify_waveform_constants(manager, configuration):
     """Verifies and updates the waveform constants in the configuration dictionary.
 
     This function checks and ensures that the waveform constants in the given
@@ -760,18 +755,16 @@
                     is not DictProxy
                 ):
                     update_config_dict(
                         manager,
                         waveform_dict[microscope_name][zoom],
                         laser,
                         {
-                            "amplitude": config_dict["remote_focus_device"][
-                                "amplitude"
-                            ],
-                            "offset": config_dict["remote_focus_device"]["offset"],
+                            "amplitude": 0,
+                            "offset": 0,
                             # "percent_smoothing": "0",
                             # "delay": config_dict["remote_focus_device"][
                             #     "delay"
                             # ],
                         },
                     )
                 else:
@@ -860,17 +853,17 @@
                     or type(waveform_dict[microscope_name][zoom]) is not DictProxy
                 ):
                     update_config_dict(
                         manager,
                         waveform_dict[microscope_name],
                         zoom,
                         {
-                            "amplitude": "0.11",
-                            "offset": config_dict["galvo"][i]["offset"],
-                            "frequency": config_dict["galvo"][i]["frequency"],
+                            "amplitude": "0",
+                            "offset": 0,
+                            "frequency": 10,
                         },
                     )
                 else:
                     for k in ["amplitude", "offset", "frequency"]:
                         if k not in waveform_dict[microscope_name][zoom].keys():
                             waveform_dict[microscope_name][zoom][k] = config_dict[
                                 "galvo"
@@ -892,20 +885,16 @@
                 waveform_dict.pop(k)
 
     # other_constants
     waveform_dict = configuration["waveform_constants"]
     other_constants_dict = {
         "remote_focus_settle_duration": "0",
         "percent_smoothing": "0",
-        "remote_focus_delay": config_dict["remote_focus_device"][
-            "delay"
-        ],
-        "remote_focus_ramp_falling": config_dict["remote_focus_device"][
-            "ramp_falling"
-        ]
+        "remote_focus_delay": "0",
+        "remote_focus_ramp_falling": "5"
     }
     if (
         "other_constants" not in waveform_dict.keys()
         or type(waveform_dict["other_constants"]) is not DictProxy
     ):
         update_config_dict(
             manager,
@@ -920,21 +909,81 @@
             waveform_dict["other_constants"][k] = "0"
 
 def verify_configuration(manager, configuration):
     """Verify configuration files.
     
     Supports old version of configurations.
     """
+    channel_count = 5
+    # generate hardware header section
     device_config = configuration["configuration"]["microscopes"]
+    hardware_dict = {}
+    ref_list = {
+        "camera": [],
+        "stage": [],
+        "zoom": None,
+        "mirror": None,
+    }
     for microscope_name in device_config.keys():
         # camera
         # delay_percent -> delay
         camera_config = device_config[microscope_name]["camera"]
         if "delay" not in camera_config.keys():
             camera_config["delay"] = camera_config.get("delay_percent", 2)
         # remote focus
         # ramp_falling_percent -> ramp_falling
         remote_focus_config = device_config[microscope_name]["remote_focus_device"]
         if "ramp_falling" not in remote_focus_config.keys():
             remote_focus_config["ramp_falling"] = remote_focus_config.get("ramp_falling_percent", 5)
         if "delay" not in remote_focus_config.keys():
             remote_focus_config["delay"] = remote_focus_config.get("delay_percent", 0)
+        
+        # daq
+        daq_type = device_config[microscope_name]["daq"]["hardware"]["type"]
+        if not daq_type.lower().startswith("synthetic"):
+            hardware_dict["daq"] = {"type": daq_type}
+
+        # camera
+        if "camera" not in hardware_dict:  
+            hardware_dict["camera"] = []
+        camera_idx = build_ref_name("-", camera_config["hardware"]["type"], camera_config["hardware"]["serial_number"])
+        if camera_idx not in ref_list["camera"]:
+            ref_list["camera"].append(camera_idx)
+            hardware_dict["camera"].append(camera_config["hardware"])
+
+        try:
+            channel_count = max(channel_count, camera_config.get("count", 5))
+        except TypeError:
+            channel_count = 5
+
+        # zoom (one zoom)
+        if "zoom" not in hardware_dict:
+            zoom_config = device_config[microscope_name]["zoom"]["hardware"]
+            # zoom_idx = build_ref_name("-", zoom_config["type"], zoom_config["servo_id"])
+            hardware_dict["zoom"] = zoom_config
+
+        # filter wheel
+        if "filter_wheel" not in hardware_dict:
+            filter_wheel_config = device_config[microscope_name]["filter_wheel"]["hardware"]
+            hardware_dict["filter_wheel"] = filter_wheel_config
+        # stage
+        if "stage" not in hardware_dict:
+            hardware_dict["stage"] = []
+        stages = device_config[microscope_name]["stage"]["hardware"]
+        if type(stages) != ListProxy:
+            stages = [stages]
+        for i, stage in enumerate(stages):
+            stage_idx = build_ref_name("-", stage["type"], stage["serial_number"])
+            if stage_idx not in ref_list["stage"]:
+                hardware_dict["stage"].append(stage)
+
+        # mirror
+        if "mirror" in device_config[microscope_name].keys() and "mirror" not in hardware_dict:
+            hardware_dict["mirror"] = device_config[microscope_name]["mirror"]["hardware"]
+
+    if "daq" not in hardware_dict:
+        hardware_dict["daq"] = {
+            "type": "synthetic"
+        }
+    update_config_dict(manager, configuration["configuration"], "hardware", hardware_dict)
+
+    update_config_dict(manager, configuration["configuration"], "gui", {"channels": {"count": channel_count}})
```

### Comparing `navigate-micro-0.0.5/src/navigate/config/experiment.yml` & `navigate_micro-0.0.6/src/navigate/config/experiment.yml`

 * *Files 4% similar despite different names*

```diff
@@ -66,8 +66,8 @@
   scanrange: 500.0
   n_plane: 1
   offset_start: 0.0
   offset_end: 10.0
   conpro_cycling_mode: Per Stack
   waveform_template: Default
 MultiPositions:
-  [{'x': 15000.0, 'y': 12000.0, 'z': 15500.0, 'theta': 0.0, 'f': 70000.0}, {'x': 35000.0, 'y': 42000.0, 'z': 15500.0, 'theta': 0.0, 'f': 70000.0}]
+  [[15000.0,12000.0,15500.0,0.0,70000.0], [35000.0,42000.0,15500.0,0.0,70000.0]]
```

### Comparing `navigate-micro-0.0.5/src/navigate/config/synthetic_configuration.yaml` & `navigate_micro-0.0.6/src/navigate/config/synthetic_configuration.yaml`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/config/waveform_constants.yml` & `navigate_micro-0.0.6/src/navigate/config/waveform_constants.yml`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/configuration_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/configuration_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/controller.py` & `navigate_micro-0.0.6/src/navigate/controller/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,14 +411,17 @@
         self.acquire_bar_controller.populate_experiment_values()
         # self.stage_controller.populate_experiment_values()
         self.multiposition_tab_controller.set_positions(
             self.configuration["experiment"]["MultiPositions"]
         )
         self.channels_tab_controller.populate_experiment_values()
         self.camera_setting_controller.populate_experiment_values()
+        self.waveform_tab_controller.set_waveform_template(
+            self.configuration["experiment"]["MicroscopeState"]["waveform_template"]
+        )
 
         # autofocus popup
         if hasattr(self, "af_popup_controller"):
             self.af_popup_controller.populate_experiment_values()
 
         if file_name:
             self.plugin_controller.populate_experiment_setting()
@@ -436,22 +439,28 @@
         Returns
         -------
         string
             Warning info if any
 
         """
         self.camera_setting_controller.update_experiment_values()
+
+        # set waveform template
+        if self.acquire_bar_controller.mode in ["live", "single", "z-stack"]:
+            camera_setting = self.configuration["experiment"]["CameraParameters"]
+            if camera_setting["sensor_mode"] == "Light-Sheet" and camera_setting[
+                "readout_direction"
+            ] in ["Bidirectional", "Rev. Bidirectional"]:
+                self.waveform_tab_controller.set_waveform_template("Bidirectional")
+            else:
+                self.waveform_tab_controller.set_waveform_template("Default")
+
         # update multi-positions
         positions = self.multiposition_tab_controller.get_positions()
-        update_config_dict(
-            self.manager,
-            self.configuration["experiment"],
-            "MultiPositions",
-            positions,
-        )
+        self.configuration["experiment"]["MultiPositions"] = positions
         self.configuration["experiment"]["MicroscopeState"][
             "multiposition_count"
         ] = len(positions)
 
         # TODO: validate experiment dict
 
         channel_warning = self.channels_tab_controller.verify_experiment_values()
@@ -748,17 +757,19 @@
             save_yaml_file(
                 file_directory=file_directory,
                 content_dict=self.configuration["experiment"],
                 filename="experiment.yml",
             )
 
             # Save the waveform_constants.yaml file.
-            save_yaml_file(file_directory=file_directory,
-                           content_dict=self.configuration['waveform_constants'],
-                           filename="waveform_constants.yml")
+            save_yaml_file(
+                file_directory=file_directory,
+                content_dict=self.configuration["waveform_constants"],
+                filename="waveform_constants.yml",
+            )
 
             self.camera_setting_controller.solvent = self.configuration["experiment"][
                 "Saving"
             ]["solvent"]
             self.camera_setting_controller.calculate_physical_dimensions()
             self.execute("acquire")
 
@@ -981,15 +992,14 @@
             if not isinstance(image_id, int):
                 logger.debug(
                     f"Navigate Controller - Something wrong happened, stop the model!, "
                     f"{image_id}"
                 )
                 self.execute("stop_acquire")
 
-
             # Display the Image in the View
             self.camera_view_controller.try_to_display_image(image_id=image_id)
             images_received += 1
 
             # Update progress bar.
             self.acquire_bar_controller.progress_bar(
                 images_received=images_received,
```

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/__init__.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/acquire_bar_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/acquire_bar_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/adaptiveoptics_popup_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/adaptiveoptics_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/autofocus_popup_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/autofocus_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_map_setting_popup_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/camera_map_setting_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_setting_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/camera_setting_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -536,20 +536,20 @@
             self.default_width,
             self.default_height,
         ) = self.parent_controller.configuration_controller.camera_pixels
         self.trigger_source = camera_config_dict["trigger_source"]
         self.trigger_active = camera_config_dict["trigger_active"]
         self.readout_speed = camera_config_dict["readout_speed"]
         # framerate_widgets
-        self.framerate_widgets["exposure_time"].widget.min = camera_config_dict[
-            "exposure_time_range"
-        ]["min"]
-        self.framerate_widgets["exposure_time"].widget.max = camera_config_dict[
-            "exposure_time_range"
-        ]["max"]
+        # self.framerate_widgets["exposure_time"].widget.min = camera_config_dict[
+        #     "exposure_time_range"
+        # ]["min"]
+        # self.framerate_widgets["exposure_time"].widget.max = camera_config_dict[
+        #     "exposure_time_range"
+        # ]["max"]
 
         # roi max width and height
         self.roi_widgets["Width"].widget.config(to=self.default_width)
         self.roi_widgets["Height"].widget.config(to=self.default_height)
         if self.roi_widgets["Width"].get() > self.default_width:
             self.roi_widgets["Width"].set(self.default_width)
         if self.roi_widgets["Height"].get() > self.default_height:
```

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/camera_view_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/camera_view_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/channel_setting_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/channel_setting_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -282,27 +282,27 @@
                 "interval_time",
             ]:
                 try:
                     setting_dict[widget_name] = float(channel_vals[widget_name].get())
                 except Exception:
                     setting_dict[widget_name] = 0
                     return False
-                ref_name = (
-                    "exposure_time"
-                    if widget_name == "camera_exposure_time"
-                    else widget_name
-                )
-                setting_range = self.parent_controller.parent_controller.configuration[
-                    "configuration"
-                ]["gui"]["channels"][ref_name]
-                if (
-                    setting_dict[widget_name] < setting_range["min"]
-                    or setting_dict[widget_name] > setting_range["max"]
-                ):
-                    return False
+                # ref_name = (
+                #     "exposure_time"
+                #     if widget_name == "camera_exposure_time"
+                #     else widget_name
+                # )
+                # setting_range = self.parent_controller.parent_controller.configuration[
+                #     "configuration"
+                # ]["gui"]["channels"][ref_name]
+                # if (
+                #     setting_dict[widget_name] < setting_range["min"]
+                #     or setting_dict[widget_name] > setting_range["max"]
+                # ):
+                #     return False
             else:
                 setting_dict[widget_name] = channel_vals[widget_name].get()
 
             if widget_name == "camera_exposure_time" or widget_name == "is_selected":
                 self.parent_controller.execute("recalculate_timepoint")
             return True
 
@@ -408,15 +408,14 @@
         int
             The index of the value in the dropdown list.
 
         Examples
         --------
         >>> self.get_index("laser", "488")
         """
-        print("get index", dropdown_name, value)
         if not value:
             return -1
         if dropdown_name == "laser":
             return self.view.laser_pulldowns[0]["values"].index(value)
         elif dropdown_name == "filter":
             return self.view.filterwheel_pulldowns[0]["values"].index(value)
         return -1
@@ -426,26 +425,26 @@
 
         Returns
         -------
         string
             Warning info
         """
         selected_channel_num = 0
-        setting_range = self.configuration_controller.gui_setting["channels"]
         for channel_key in self.channel_setting_dict.keys():
             setting_dict = self.channel_setting_dict[channel_key]
+            idx = int(channel_key[len("channel_"):]) - 1
             if setting_dict["is_selected"]:
                 selected_channel_num += 1
                 # laser power
-                if setting_dict["laser_power"] < setting_range["laser_power"]["min"]:
+                if setting_dict["laser_power"] < self.view.laserpower_pulldowns[idx]["from"]:
                     return f"Laser power below configured threshold. Please adjust to meet or exceed the specified minimum in the configuration.yaml({setting_range['laser_power']['min']})."
-                elif setting_dict["laser_power"] > setting_range["laser_power"]["max"]:
+                elif setting_dict["laser_power"] > self.view.laserpower_pulldowns[idx]["to"]:
                     return f"Laser power exceeds configured maximum. Please adjust to meet or be below the specified maximum in the configuration.yaml({setting_range['laser_power']['max']})."
                 # exposure time
-                if setting_dict["camera_exposure_time"] < setting_range["exposure_time"]["min"]:
+                if setting_dict["camera_exposure_time"] < self.view.exptime_pulldowns[idx]["from"]:
                     return f"Exposure time below configured threshold.Please adjust to meet or exceed the specified minimum in the configuration.yaml({setting_range['exposure_time']['min']})."
-                elif setting_dict["camera_exposure_time"] > setting_range["exposure_time"]["max"]:
+                elif setting_dict["camera_exposure_time"] > self.view.exptime_pulldowns[idx]["to"]:
                     return f"Exposure time exceeds configured maximum. Please adjust to meet or be below the specified maximum in the configuration.yaml({setting_range['exposure_time']['max']})"
 
         if selected_channel_num == 0:
             return "No selected channel!"
         return None
```

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/channels_tab_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/channels_tab_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,16 +109,14 @@
         self.stack_acq_buttons["set_end"].configure(command=self.update_end_position)
 
         # stack acquisition_variables
         #: float: The z origin of the stack.
         self.z_origin = 0
         #: float: The focus origin of the stack.
         self.focus_origin = 0
-        #: float: The stage velocity.
-        self.stage_velocity = None
         #: float: The filter wheel delay.
         self.filter_wheel_delay = None
         #: dict: The microscope state dictionary.
         self.microscope_state_dict = None
 
         # laser/stack cycling event binds
         self.stack_acq_vals["cycling"].trace_add("write", self.update_cycling_setting)
@@ -177,18 +175,17 @@
         Examples
         --------
         >>> self.initialize()
         """
         config = self.parent_controller.configuration_controller
 
         self.stack_acq_widgets["cycling"].widget["values"] = ["Per Z", "Per Stack"]
-        self.stage_velocity = config.stage_setting_dict["velocity"]
         self.filter_wheel_delay = config.filter_wheel_setting_dict["filter_wheel_delay"]
         self.channel_setting_controller.initialize()
-        self.set_spinbox_range_limits(config.configuration["configuration"]["gui"])
+        # self.set_spinbox_range_limits(config.configuration["configuration"]["gui"])
         self.show_verbose_info("channels tab has been initialized")
 
     def populate_experiment_values(self):
         """Distribute initial MicroscopeState values to this and sub-controllers and
         associated views.
 
         Examples
@@ -644,15 +641,15 @@
             # distance = [x2-x1, y2-y1, z2-z1, theta2-theta1, f2-f1]
             # max_distance_idx = np.argmax(distance)
             # Now if we are going to do this properly, we would need to do this for
             # all of the positions so that we can calculate the total experiment
             # time. Probably assemble a matrix of all the positions and then do
             # the calculations.
 
-            stage_delay = 0  # distance[max_distance_idx]/self.stage_velocity
+            stage_delay = 0
             # TODO False value.
 
             # If we were actually acquiring the data, we would call the function to
             # move the stage here.
             experiment_duration = experiment_duration + stage_delay
 
             for channel_idx in range(len(channel_exposure_time)):
```

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/feature_advanced_setting_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/feature_advanced_setting_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/features_popup_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/features_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/gui_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/gui_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/ilastik_popup_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/ilastik_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/keystroke_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/keystroke_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/menu_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/menu_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,43 +179,43 @@
             Camera view sub-controller.
 
         """
 
         # File Menu
         file_menu = {
             self.view.menubar.menu_file: {
-                "New Experiment": [
+                "Load Default Configuration": [
                     "standard",
                     self.new_experiment,
                     "Ctrl+Shift+N",
                     "<Control-N>",
                     "<Control_L-N>",
                 ],
-                "Load Experiment": [
+                "Load Experiment File": [
                     "standard",
                     self.load_experiment,
                     "Ctrl+Shift+O",
                     "<Control-O>",
                     "<Control_L-O>",
                 ],
-                "Save Experiment": [
+                "Save Experiment File": [
                     "standard",
                     self.save_experiment,
                     "Ctrl+Shift+S",
                     "<Control-S>",
                     "<Control_L-S>",
                 ],
-                "Load Waveform Constants": [
+                "Load Waveform Constants File": [
                     "standard",
                     self.load_waveform_constants,
                     None,
                     None,
                     None,
                 ],
-                "Save Waveform Constants": [
+                "Save Waveform Constants File": [
                     "standard",
                     self.save_waveform_constants,
                     None,
                     None,
                     None,
                 ],
                 "add_separator": [None],
@@ -374,44 +374,44 @@
         self.populate_menu(autofocus_menu)
 
         # Window menu
         windows_menu = {
             self.view.menubar.menu_window: {
                 "Channel Settings": [
                     "standard",
-                    lambda event: self.switch_tabs(1),
+                    lambda *args: self.switch_tabs(1),
                     "Ctrl+1",
                     "<Control-Key-1>",
                     "<Control_L-Key-1",
                 ],
                 "Camera Settings": [
                     "standard",
-                    lambda event: self.switch_tabs(2),
+                    lambda *args: self.switch_tabs(2),
                     "Ctrl+2",
                     "<Control-Key-2>",
                     "<Control_L-Key-2",
                 ],
                 "Stage Control": [
                     "standard",
-                    lambda event: self.switch_tabs(3),
+                    lambda *args: self.switch_tabs(3),
                     "Ctrl+3",
                     "<Control-Key-3>",
                     "<Control_L-Key-3",
                 ],
                 "Multiposition Table": [
                     "standard",
-                    lambda event: self.switch_tabs(4),
+                    lambda *args: self.switch_tabs(4),
                     "Ctrl+4",
                     "<Control-Key-4>",
                     "<Control_L-Key-4",
                 ],
                 "add_separator": ["standard", None, None, None, None],
                 "Popout Camera Display": [
                     "standard",
-                    self.not_implemented,
+                    lambda: self.popout_camera_display(),
                     None,
                     None,
                     None,
                 ],
                 "Help": ["standard", self.popup_help, None, None, None],
             }
         }
@@ -891,14 +891,18 @@
             # Avoids KeyError if the user is in a popdown menu.
             pass
 
     def switch_tabs(self, tab):
         """Switch tabs."""
         self.parent_controller.view.settings.select(tab - 1)
 
+    def popout_camera_display(self):
+        """Pop out camera display."""
+        self.parent_controller.view.camera_waveform.popout()
+
     def popup_feature_list_setting(self):
         """Show feature list popup window"""
         feature_list_popup = FeatureListPopup(self.view, title="Add New Feature List")
         self.parent_controller.features_popup_controller = FeaturePopupController(
             feature_list_popup, self.parent_controller
         )
```

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/microscope_popup_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/microscope_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/multi_position_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/multi_position_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,61 +92,57 @@
         self.parent_controller.execute("eliminate_tiles")
 
     def set_positions(self, positions):
         """Set positions to multi-position's table
 
         Parameters
         ----------
-        positions : dict
+        positions : [[]]
             positions to be set
 
         Example
         -------
-        >>>    positions = {
-        >>>    0: {'x': 0, 'y': 0, 'z': 0, 'theta': 0, 'f': 0},
-        >>>    1: {'x': 1, 'y': 1, 'z': 1, 'theta': 1, 'f': 1},
-        >>>    2: {'x': 2, 'y': 2, 'z': 2, 'theta': 2, 'f': 2}}
+        >>>    positions = [
+        >>>    [0, 0, 0, 0, 0],
+        >>>    [1, 1, 1, 1, 1],
+        >>>    [2, 2, 2, 2, 2]]
         >>>    set_positions(positions)
         """
         axis_dict = {"x": "X", "y": "Y", "z": "Z", "theta": "R", "f": "F"}
         data = {}
 
-        for name in axis_dict:
-            data[axis_dict[name]] = list(pos[name] for pos in positions)
+        for i, name in enumerate(axis_dict.keys()):
+            data[axis_dict[name]] = list(pos[i] for pos in positions)
         self.table.model.df = pd.DataFrame(data)
         self.table.redraw()
         self.show_verbose_info("loaded new positions")
 
     def get_positions(self):
         """Return all positions from the Multi-Position Acquisition Interface.
 
         Returns
         -------
-        dict
-            positions in the format of {index: {axis: value}}
+        list
+            positions in the format of [[x, y, z, theta, f], ]
 
         Example
         -------
         >>> get_positions()
         """
-        axis_dict = {"X": "x", "Y": "y", "Z": "z", "R": "theta", "F": "f"}
         positions = []
         rows = self.table.model.df.shape[0]
         for i in range(rows):
             temp = list(self.table.model.df.iloc[i])
             if (
                 len(
                     list(filter(lambda v: type(v) == float and not math.isnan(v), temp))
                 )
                 == 5
             ):
-                temp = dict(self.table.model.df.iloc[i])
-                positions.append({})
-                for k in axis_dict:
-                    positions[i][axis_dict[k]] = temp[k]
+                positions.append(temp)
         return positions
 
     def handle_double_click(self, event):
         """Move to a position within the Multi-Position Acquisition Interface.
 
         When double-clicked the row head, it will call the parent/central controller
         to move stage and update stage view
```

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/plugins_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/plugins_controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,67 +26,84 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 # IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 #
 
+# Standard library imports
 from pathlib import Path
 import os
 import inspect
 import tkinter as tk
+from tkinter import messagebox
 
+# Third-party imports
+
+# Local application imports
 from navigate.config.config import get_navigate_path
 from navigate.view.custom_widgets.popup import PopUp
 from navigate.tools.file_functions import load_yaml_file, save_yaml_file
 from navigate.tools.common_functions import combine_funcs, load_module_from_file
 from navigate.tools.decorators import AcquisitionMode
 from navigate.model.features import feature_related_functions
 from navigate.controller.sub_controllers.gui_controller import GUIController
 from navigate.view.popups.plugins_popup import PluginsPopup
 
 
 class PluginsController:
-    """Plugins manaager in the controller side"""
+    """Plugins manager in the controller side"""
 
     def __init__(self, view, parent_controller):
-        """Initialize plugins manager class"""
+        """Initialize plugins manager class.
+
+        Parameters
+        ----------
+        view: object
+            tkinter frame object.
+        parent_controller: object
+            navigate controller.
+        """
         #: object: tkinter frame object.
         self.view = view
+
         #: object: navigate controller.
         self.parent_controller = parent_controller
+
         #: str: plugins default path.
         self.plugins_path = os.path.join(
             Path(__file__).resolve().parent.parent.parent, "plugins"
         )
+
         #: dict: installed plugins with GUI
         self.plugins_dict = {}
 
     def populate_experiment_setting(self):
         """populate experiment values to plugin GUI"""
         for plugin_name in self.plugins_dict:
             try:
                 self.plugins_dict[plugin_name].populate_experiment_setting()
-            except:
+            except Exception:
                 pass
 
     def load_plugins(self):
         """Load plugins"""
         plugins = os.listdir(self.plugins_path)
         installed_plugins = dict(
             [(f, os.path.join(self.plugins_path, f)) for f in plugins]
         )
         # load plugins from plugins_config
         plugins_config_path = os.path.join(
             get_navigate_path(), "config", "plugins_config.yml"
         )
-        if not os.path.exists(plugins_config_path):
+        plugins_config = load_yaml_file(plugins_config_path)
+        if plugins_config is None:
+            plugins_config = {}
             save_yaml_file(get_navigate_path(), {}, "plugins_config.yml")
         else:
-            plugins_config = load_yaml_file(plugins_config_path)
             for plugin_name, plugin_path in plugins_config.items():
                 if plugin_path and os.path.exists(plugin_path):
                     installed_plugins[plugin_name] = plugin_path
         for _, plugin_path in installed_plugins.items():
             if not os.path.isdir(plugin_path):
                 continue
 
@@ -114,20 +131,31 @@
                     and os.path.isfile(view_file)
                     and os.path.exists(controller_file)
                     and os.path.isfile(controller_file)
                 ):
                     plugin_frame_module = load_module_from_file(
                         f"{plugin_class_name}Frame", view_file
                     )
+                    if plugin_frame_module is None:
+                        print(
+                            f"Make sure that the plugin frame name {plugin_class_name} is correct! "
+                            f"Plugin {plugin_name} needs to be uninstalled from navigate or reinstalled!"
+                        )
+                        continue
                     plugin_frame = getattr(
                         plugin_frame_module, f"{plugin_class_name}Frame"
                     )
                     plugin_controller_module = load_module_from_file(
                         f"{plugin_class_name}Controller", controller_file
                     )
+                    if plugin_controller_module is None:
+                        print(
+                            f"Make sure that the plugin controller {plugin_class_name} is correct! "
+                            f"Plugin {plugin_name} needs to be uninstalled from navigate or reinstalled!"
+                        )
                     plugin_controller = getattr(
                         plugin_controller_module, f"{plugin_class_name}Controller"
                     )
 
                     if plugin_config["view"] == "Popup":
                         # menu
                         self.parent_controller.view.menubar.menu_plugins.add_command(
@@ -183,24 +211,33 @@
         plugin_name : str
             plugin name.
         frame: object
             navigate frame object
         controller: object
             navigate controller
         """
-        plugin_frame = frame(self.view.settings)
-        self.view.settings.add(plugin_frame, text=plugin_name, sticky=tk.NSEW)
-        plugin_controller = controller(plugin_frame, self.parent_controller)
-        controller_name = (
-            "__plugin" + "_".join(plugin_name.lower().split()) + "_controller"
-        )
-        self.plugins_dict[controller_name] = plugin_controller
+        try:
+            plugin_frame = frame(self.view.settings)
+            self.view.settings.add(plugin_frame, text=plugin_name, sticky=tk.NSEW)
+            plugin_controller = controller(plugin_frame, self.parent_controller)
+            controller_name = (
+                "__plugin" + "_".join(plugin_name.lower().split()) + "_controller"
+            )
+            self.plugins_dict[controller_name] = plugin_controller
+        except:
+            messagebox.showwarning(
+                title="Warning",
+                message=(
+                    f"Plugin {plugin_name} has something went wrong."
+                    f"Please make sure the plugin works correctly or uninstall it!"
+                )
+            )
 
     def build_popup_window(self, plugin_name, frame, controller):
-        """Build popup window for plugins
+        """Build popup window for a plugin
 
         Parameters
         ----------
         plugin_name : str
             plugin name.
         frame: object
             navigate frame object
@@ -208,14 +245,23 @@
             navigate controller
         """
         controller_name = (
             "__plugin" + "_".join(plugin_name.lower().split()) + "_controller"
         )
 
         def func(*args, **kwargs):
+            """Function to build popup window for a plugin
+
+            Parameters
+            ----------
+            args: list
+                arguments.
+            kwargs: dict
+                keyword arguments.
+            """
             if controller_name in self.plugins_dict:
                 self.plugins_dict[controller_name].popup.deiconify()
                 return
             popup = PopUp(self.view, plugin_name, "+320+180", transient=False)
             popup.configure(bg="white")
             content_frame = popup.get_frame()
             plugin_frame = frame(content_frame)
@@ -230,23 +276,48 @@
             popup.protocol(
                 "WM_DELETE_WINDOW",
                 combine_funcs(
                     popup.dismiss, lambda: self.plugins_dict.pop(controller_name)
                 ),
             )
 
-        return func
+        def func_with_wrapper(*args, **kwargs):
+            try:
+                func(*args, **kwargs)
+            except:
+                messagebox.showwarning(
+                    title="Warning",
+                    message=(
+                        f"Plugin {plugin_name} has something went wrong."
+                        f"Please make sure the plugin works correctly or uninstall it from navigate!"
+                    )
+                )
+
+        return func_with_wrapper
 
 
 class UninstallPluginController(GUIController):
+    """Uninstall plugin controller"""
+
     def __init__(self, view, parent_controller):
+        """Initialize uninstall plugin controller class.
+
+        Parameters
+        ----------
+        view: object
+            tkinter frame object.
+        parent_controller: object
+            navigate controller.
+        """
         super().__init__(view, parent_controller)
 
+        #: str: plugin config path.
         self.plugin_config_path = os.path.join(get_navigate_path(), "config")
 
+        #: PluginsPopup: popup window object.
         self.popup = PluginsPopup(view)
         self.popup.uninstall_btn.config(command=self.uninstall_plugins)
         self.popup.popup.protocol("WM_DELETE_WINDOW", self.exit_func)
         self.refresh_plugins()
 
     def showup(self):
         """Show up the popup window"""
@@ -263,34 +334,44 @@
         self.plugin_config = load_yaml_file(
             os.path.join(self.plugin_config_path, "plugins_config.yml")
         )
 
         self.popup.build_widgets(self.plugin_config)
 
     def uninstall_plugins(self, *args):
-        """Uninstall plugins"""
+        """Uninstall plugins.
+
+        Parameters
+        ----------
+        args: list
+            arguments.
+        """
         feature_lists_path = get_navigate_path() + "/feature_lists"
         features = os.listdir(feature_lists_path)
         feature_config = {}
         for feature_name in features:
             if feature_name.endswith(".yml") and feature_name != "__sequence.yml":
-                feature_content = load_yaml_file(os.path.join(feature_lists_path, feature_name))
+                feature_content = load_yaml_file(
+                    os.path.join(feature_lists_path, feature_name)
+                )
                 if feature_content and feature_content.get("filename", None):
                     feature_config[feature_name] = feature_content["filename"]
         flag = False
         for var in self.popup.variables:
             if var.get():
                 # remove the feature list if a deleted plugin has any.
                 for feature_name in feature_config:
-                    if feature_config[feature_name].startswith(self.plugin_config[var.get()]):
+                    if feature_config[feature_name].startswith(
+                        self.plugin_config[var.get()]
+                    ):
                         os.remove(f"{feature_lists_path}/{feature_name}")
                 self.plugin_config.pop(var.get())
                 flag = True
         if flag:
             save_yaml_file(
                 self.plugin_config_path, self.plugin_config, "plugins_config.yml"
             )
-            tk.messagebox.showwarning(
+            messagebox.showwarning(
                 title="Navigate",
                 message="Plugins are uninstalled! Please restart Navigate!",
             )
             self.showup()
```

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/stage_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/stage_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,21 +280,23 @@
                     logger.info(f"Focus axis buttons set to {state}")
             else:
                 pass
 
     def bind_position_callbacks(self):
         """Binds position_callback() to each axis, records the trace name so we can
         unbind later."""
+        widgets = self.view.get_widgets()
         if not self.position_callbacks_bound:
             for axis in ["x", "y", "z", "theta", "f"]:
                 # add event bind to position entry variables
-                cbname = self.widget_vals[axis].trace_add(
-                    "write", self.position_callback(axis)
-                )
-                self.position_callback_traces[axis] = cbname
+                widgets[axis].widget.bind("<FocusOut>", self.position_callback(axis))
+                # cbname = self.widget_vals[axis].trace_add(
+                #     "write", self.position_callback(axis)
+                # )
+                # self.position_callback_traces[axis] = cbname
             self.position_callbacks_bound = True
 
     def unbind_position_callbacks(self):
         """Unbinds position callbacks."""
         if self.position_callbacks_bound:
             for axis, cbname in self.position_callback_traces.items():
                 self.widget_vals[axis].trace_remove("write", cbname)
@@ -314,36 +316,40 @@
         """This function is to populate(set) position in the View
 
         Parameters
         ----------
         position : dict
             {'x': value, 'y': value, 'z': value, 'theta': value, 'f': value}
         """
-        widgets = self.view.get_widgets()
         for axis in ["x", "y", "z", "theta", "f"]:
-            self.widget_vals[axis].set(position.get(axis, 0))
-            # validate position value if set through variable
-            if self.stage_limits:
-                widgets[axis].widget.trigger_focusout_validation()
-            self.stage_setting_dict[axis] = position.get(axis, 0)
+            if axis not in position:
+                continue
+            self.widget_vals[axis].set(position[axis])
+            self.position_callback(axis)()
         self.show_verbose_info("Set stage position")
 
     def set_position_silent(self, position):
         """This function is to populate(set) position in the View without a trace.
 
         Parameters
         ----------
         position : dict
             {'x': value, 'y': value, 'z': value, 'theta': value, 'f': value}
         """
-        self.unbind_position_callbacks()
-
-        self.set_position(position)
+        widgets = self.view.get_widgets()
+        for axis in ["x", "y", "z", "theta", "f"]:
+            if axis not in position:
+                continue
+            self.widget_vals[axis].set(position[axis])
+            # validate position value if set through variable
+            if self.stage_limits:
+                widgets[axis].widget.trigger_focusout_validation()
+            self.stage_setting_dict[axis] = position.get(axis, 0)
+        self.show_verbose_info("Set stage position")
 
-        self.bind_position_callbacks()
 
     def get_position(self):
         """This function returns current position from the view.
 
         Returns
         -------
         position : dict
@@ -388,25 +394,26 @@
             step_val = self.widget_vals[axis + "_step"]
 
         def handler():
             """This function generates command functions according to the desired axis
             to move."""
             stage_direction = -1 if self.flip_flags[axis] else 1
             try:
-                temp = position_val.get() + step_val.get() * stage_direction
+                temp = float(position_val.get()) + step_val.get() * stage_direction
             except tk._tkinter.TclError:
                 return
             if self.stage_limits is True:
                 if temp > self.position_max[axis]:
                     temp = self.position_max[axis]
                 elif temp < self.position_min[axis]:
                     temp = self.position_min[axis]
             # guarantee stage won't move out of limits
-            if position_val.get() != temp:
+            if float(position_val.get()) != temp:
                 position_val.set(temp)
+                self.position_callback(axis)()
 
         return handler
 
     def down_btn_handler(self, axis):
         """This function generates command functions according to the desired axis
         to move.
 
@@ -428,25 +435,26 @@
             step_val = self.widget_vals[axis + "_step"]
 
         def handler():
             """This function generates command functions according to the desired axis
             to move."""
             stage_direction = -1 if self.flip_flags[axis] else 1
             try:
-                temp = position_val.get() - step_val.get() * stage_direction
+                temp = float(position_val.get()) - step_val.get() * stage_direction
             except tk._tkinter.TclError:
                 return
             if self.stage_limits is True:
                 if temp < self.position_min[axis]:
                     temp = self.position_min[axis]
                 elif temp > self.position_max[axis]:
                     temp = self.position_max[axis]
             # guarantee stage won't move out of limits
-            if position_val.get() != temp:
+            if float(position_val.get()) != temp:
                 position_val.set(temp)
+                self.position_callback(axis)()
 
         return handler
 
     def zero_btn_handler(self, axis):
         """This function generates command functions according to the desired axis
         to move.
 
@@ -461,14 +469,15 @@
         handler : object
             Function for setting desired stage positions in the View.
         """
         position_val = self.widget_vals[axis]
 
         def handler():
             position_val.set(0)
+            self.position_callback(axis)()
 
         return handler
 
     def xy_zero_btn_handler(self):
         """This function generates command functions to set xy position to zero
 
         Returns
@@ -478,14 +487,16 @@
         """
         x_val = self.widget_vals["x"]
         y_val = self.widget_vals["y"]
 
         def handler():
             x_val.set(0)
             y_val.set(0)
+            self.position_callback("x")()
+            self.position_callback("y")()
 
         return handler
 
     def stop_button_handler(self, *args):
         """This function stops the stage after a 250 ms debouncing period of time."""
         self.view.after(250, lambda *args: self.parent_controller.execute("stop_stage"))
 
@@ -543,15 +554,15 @@
 
         def handler(*args):
             """Callback functions bind to position variables."""
             if self.event_id[axis]:
                 self.view.after_cancel(self.event_id[axis])
             # if position is not a number, then do not move stage
             try:
-                position = position_var.get()
+                position = float(position_var.get())
                 if self.stage_limits:
                     widget.trigger_focusout_validation()
                     # if position is not inside limits do not move stage
                     if (
                         position < float(self.position_min[axis])
                         or position > float(self.position_max[axis])
                     ):
```

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/tiling_wizard_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/tiling_wizard_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/tiling_wizard_controller2.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/tiling_wizard_controller2.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/waveform_popup_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/waveform_popup_controller.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/controller/sub_controllers/waveform_tab_controller.py` & `navigate_micro-0.0.6/src/navigate/controller/sub_controllers/waveform_tab_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -324,7 +324,24 @@
 
         Examples
         --------
         >>> self.set_mode(mode)
         """
         state = "normal" if mode == "stop" else "disabled"
         self.view.waveform_settings.inputs["waveform_template"].widget["state"] = state
+
+    def set_waveform_template(self, template_name):
+        """Set the waveform template name
+
+        Parameters
+        ----------
+        template_name : str
+            Set the waveform template name
+
+        Examples
+        --------
+        >>> self.set_waveform_template(template_name)
+        """
+        self.view.waveform_settings.inputs["waveform_template"].set(template_name)
+        self.parent_controller.configuration["experiment"]["MicroscopeState"][
+            "waveform_template"
+        ] = template_name
```

### Comparing `navigate-micro-0.0.5/src/navigate/controller/thread_pool.py` & `navigate_micro-0.0.6/src/navigate/controller/thread_pool.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/log_files/filters.py` & `navigate_micro-0.0.6/src/navigate/log_files/filters.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/log_files/log_functions.py` & `navigate_micro-0.0.6/src/navigate/log_files/log_functions.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/log_files/logging.yml` & `navigate_micro-0.0.6/src/navigate/log_files/logging.yml`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/log_files/model_logging.yml` & `navigate_micro-0.0.6/src/navigate/log_files/model_logging.yml`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/main.py` & `navigate_micro-0.0.6/src/navigate/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 # Standard Library Imports
 import tkinter as tk
 import platform
 import os
-import warnings
 
 # Third Party Imports
 
 # Local Imports
 from navigate.controller.controller import Controller
+from navigate.controller.configurator import Configurator
 from navigate.log_files.log_functions import log_setup
 from navigate.view.splash_screen import SplashScreen
 from navigate.tools.main_functions import (
     evaluate_parser_input_arguments,
     create_parser,
 )
 
@@ -64,30 +64,32 @@
         --synthetic-hardware
         --sh
         --config-file
         --experiment-file
         --waveform_constants-path
         --rest-api-file
         --waveform-templates-file
-        --logging-config
+        --logging-confi
 
     Returns
     -------
     None
 
     Examples
     --------
     >>> python main.py --synthetic-hardware
     """
-    if platform.system() != 'Windows':
-        print("WARNING: navigate was built to operate on a Windows platform. "
-              "While much of the software will work for evaluation purposes, some "
-              "unanticipated behaviors may occur. For example, it is known that the "
-              "Tkinter-based GUI does not grid symmetrically, nor resize properly "
-              "on MacOS. Testing on Linux operating systems has not been performed.")
+    if platform.system() != "Windows":
+        print(
+            "WARNING: navigate was built to operate on a Windows platform. "
+            "While much of the software will work for evaluation purposes, some "
+            "unanticipated behaviors may occur. For example, it is known that the "
+            "Tkinter-based GUI does not grid symmetrically, nor resize properly "
+            "on MacOS. Testing on Linux operating systems has not been performed."
+        )
 
     # Start the GUI, withdraw main screen, and show splash screen.
     root = tk.Tk()
     root.withdraw()
 
     # Splash Screen
     current_directory = os.path.dirname(os.path.realpath(__file__))
@@ -102,26 +104,31 @@
     (
         configuration_path,
         experiment_path,
         waveform_constants_path,
         rest_api_path,
         waveform_templates_path,
         logging_path,
+        configurator,
     ) = evaluate_parser_input_arguments(args)
 
     log_setup("logging.yml", logging_path)
 
-    Controller(
-        root,
-        splash_screen,
-        configuration_path,
-        experiment_path,
-        waveform_constants_path,
-        rest_api_path,
-        waveform_templates_path,
-        args,
-    )
+    if args.configurator:
+        Configurator(root, splash_screen)
+    else:
+        Controller(
+            root,
+            splash_screen,
+            configuration_path,
+            experiment_path,
+            waveform_constants_path,
+            rest_api_path,
+            waveform_templates_path,
+            args,
+        )
+
     root.mainloop()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/analysis/boundary_detect.py` & `navigate_micro-0.0.6/src/navigate/model/analysis/boundary_detect.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/analysis/camera.py` & `navigate_micro-0.0.6/src/navigate/model/analysis/camera.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/analysis/image_contrast.py` & `navigate_micro-0.0.6/src/navigate/model/analysis/image_contrast.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/concurrency/concurrency_tools.py` & `navigate_micro-0.0.6/src/navigate/model/concurrency/concurrency_tools.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/data_sources/__init__.py` & `navigate_micro-0.0.6/src/navigate/model/data_sources/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ File type specific data sources. """
 
-FILE_TYPES = ["TIFF", "OME-TIFF", "H5", "N5"]
+FILE_TYPES = ["TIFF", "OME-TIFF", "H5", "N5", "OME-Zarr"]
 
 
 def get_data_source(file_type):
     """Get the data source class for the given file type.
 
     Parameters
     ----------
@@ -28,9 +28,14 @@
         return TiffDataSource
 
     elif (file_type == "H5") or file_type == ("N5"):
         from .bdv_data_source import BigDataViewerDataSource
 
         return BigDataViewerDataSource
 
+    elif file_type == "OME-Zarr":
+        from .zarr_data_source import OMEZarrDataSource
+
+        return OMEZarrDataSource
+
     else:
         raise NotImplementedError(f"Unknown file type {file_type}. Cannot open.")
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/data_sources/bdv_data_source.py` & `navigate_micro-0.0.6/src/navigate/model/metadata_sources/bdv_metadata.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,561 +27,511 @@
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 # IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 #  Standard Imports
 import os
+from typing import Optional, Union
+import xml.etree.ElementTree as ET
 
 # Third Party Imports
-import h5py
-import zarr  # for n5
 import numpy as np
 import numpy.typing as npt
 
 # Local imports
-from .data_source import DataSource
-from ..metadata_sources.bdv_metadata import BigDataViewerMetadata
-from multiprocessing.managers import DictProxy
+from .metadata import XMLMetadata
+from navigate.tools.linear_algebra import affine_rotation, affine_shear
 
 
-class BigDataViewerDataSource(DataSource):
-    """BigDataViewer data source.
-
-    This class is used to write data to a BigDataViewer-compatible file. It
-    supports both HDF5 and N5 file formats. The file is written in a
-    multi-resolution pyramid format, with each resolution level subdivided into
-    32x32x1 blocks. The number of blocks in each dimension is determined by the
-    shape of the data and the resolution level.
+class BigDataViewerMetadata(XMLMetadata):
+    """Metadata for BigDataViewer files.
+
+    Note
+    ----
+        XML spec in section 2.3 of https://arxiv.org/abs/1412.0488.
+
     """
 
-    def __init__(self, file_name: str = None, mode: str = "w") -> None:
-        """Initializes the BigDataViewerDataSource.
+    def __init__(self) -> None:
+        """Initialize the BigDataViewer metadata object."""
+        super().__init__()
+
+        # Affine Transform Parameters
+        #: bool: Shear the data.
+        self.shear_data = False
+        #: str: Dimension to shear the data.
+        self.shear_dimension = "YZ"
+        #: float: Angle in degrees to shear the data.
+        self.shear_angle = 0
+        #: npt.NDArray: Shear transform matrix.
+        self.shear_transform = np.eye(3, 4)
+
+        # Rotation Transform Parameters
+        #: bool: Rotate the data.
+        self.rotate_data = False
+        #: float: Angle in degrees to rotate the data in X.
+        self.rotate_angle_x = 0
+        #: float: Angle in degrees to rotate the data in Y.
+        self.rotate_angle_y = 0
+        #: float: Angle in degrees to rotate the data in Z.
+        self.rotate_angle_z = 0
+        #: npt.NDArray: Rotation transform matrix.
+        self.rotate_transform = np.eye(3, 4)
+
+    def get_affine_parameters(self, configuration):
+        """Get the affine transform parameters from the configuration file.
 
         Parameters
         ----------
-        file_name : str
-            The name of the file to write to.
-        mode : str
-            The mode to open the file in. Must be "w" for write or "r" for read.
+        configuration : dict
+            Configuration dictionary.
         """
-        #: np.array: The resolution of each down-sampled pyramid level.
-        self._resolutions = np.array(
-            [[1, 1, 1], [2, 2, 1], [4, 4, 1], [8, 8, 1]], dtype=int
-        )
-        #: np.array: The number of subdivisions in each dimension.
-        self._subdivisions = None
-        #: np.array: The shape of the image.
-        self._shapes = None
-        #: np.array: The image.
-        self.image = None
-        #: list: The views.
-        self._views = []
-        #: zarr.N5Store: The N5 store.
-        self.__store = None
-        #: str: The file type.
-        self.__file_type = os.path.splitext(os.path.basename(file_name))[-1][1:].lower()
-        if self.__file_type not in ["h5", "n5"]:
-            raise ValueError(f"Unknown file type {self.__file_type}.")
-        if self.__file_type == "h5":
-            self.setup = self._setup_h5
-            self.ds_name = self._h5_ds_name
-        elif self.__file_type == "n5":
-            self.setup = self._setup_n5
-            self.ds_name = self._n5_ds_name
-
-        # self._current_frame = 0
-        #: BigDataViewerMetadata: The metadata.
-        self.metadata = BigDataViewerMetadata()
-
-        super().__init__(file_name, mode)
-
-    def __getitem__(self, keys):
-        """Magic method to get slice requests passed by, e.g., ds[:,2:3,...].
-        Allows arbitrary slicing of dataset via calls to get_slice().
+        bdv_configuration = configuration["configuration"].get("BDVParameters")
 
-        Order is xycztps where x, y, z are Cartesian indices, c is channel,
-        t is timepoints, p is positions and s is subdivisions to index along.
+        if bdv_configuration is not None:
 
-        TODO: Add subdivisions.
+            # Shear Parameters
+            self.shear_data = bdv_configuration["shear"].get("shear_data", False)
+            self.shear_dimension = (
+                bdv_configuration["shear"].get("shear_dimension", "YZ").upper()
+            )
+            self.shear_angle = bdv_configuration["shear"].get("shear_angle", 0)
+
+            # Rotate Parameters
+            self.rotate_data = bdv_configuration["rotate"].get("rotate_data", False)
+            self.rotate_angle_x = bdv_configuration["rotate"].get("X", 0)
+            self.rotate_angle_y = bdv_configuration["rotate"].get("Y", 0)
+            self.rotate_angle_z = bdv_configuration["rotate"].get("Z", 0)
+
+    def bdv_xml_dict(
+        self, file_name: Union[str, list, None], views: list, **kw
+    ) -> dict:
+        """Create a BigDataViewer XML dictionary from a list of views.
 
         Parameters
         ----------
-        keys : tuple
-            Tuple of indices.
+        file_name : str
+            The file name of the file to be written.
+        views : list
+            A list of dictionaries containing metadata for each view.
+        **kw
+            Additional keyword arguments.
 
         Returns
         -------
-        npt.ArrayLike
-            Array of shape (p, t, z, c, y, x)
+        dict
+            A dictionary containing the XML metadata.
+
         """
+        # Header
+        bdv_dict = {"version": 0.2}
 
-        # Check lengths
-        if isinstance(keys, slice) or isinstance(keys, int):
-            length = 1
-        else:
-            length = len(keys)
-        if length < 1:
-            raise IndexError(
-                "Too few indices. Indices may be (x, y, c, z, t, p, subdiv)."
-            )
-        elif length > 7:
-            raise IndexError(
-                "Too many indices. Indices may be (x, y, c, z, t, p, subdiv)."
-            )
+        # File path
+        bdv_dict["BasePath"] = {"type": "relative", "text": "."}
+        bdv_dict["SequenceDescription"] = {}
 
-        # Handle "slice the rest"
-        if length > 1 and keys[-1] == Ellipsis:
-            keys = keys[:-2]
-            length -= 1
-
-        def ensure_iter(pos):
-            """Ensure the input is iterable.
-
-            Parameters
-            ----------
-            pos : int
-                The position.
-
-            Returns
-            -------
-            range
-                The range.
+        ext = os.path.basename(file_name).split(".")[-1]
+        if ext == "h5":
             """
-            if length > pos:
-                try:
-                    val = keys[pos]
-                except TypeError:
-                    # Only one key
-                    val = keys
-                if isinstance(val, slice):
-                    if val.start is None and val.stop is None and val.step is None:
-                        return range(self.shape[pos])
-                    return range(10**10)[val]
-                elif isinstance(val, int):
-                    return range(val, val + 1)
-            else:
-                return range(self.shape[pos])
-
-        def ensure_slice(pos):
-            """Ensure the input is a slice or a single integer.
-
-            Parameters
-            ----------
-            pos : int
-                The position.
-
-            Returns
-            -------
-            slice
-                The slice.
+            <ImageLoader format="bdv.hdf5">
+                <hdf5 type="relative">dataset.h5</hdf5>
+            </ImageLoader>
             """
-            # TODO: Handle list as input
-            if length > pos:
-                try:
-                    val = keys[pos]
-                except TypeError:
-                    # Only one key
-                    val = keys
-                assert isinstance(val, slice) or isinstance(val, int)
-                return val
-            else:
-                # Default to all values
-                return slice(None, None, None)
-
-        # Get legal indices
-        xs = ensure_slice(0)
-        ys = ensure_slice(1)
-        cs = ensure_iter(2)
-        zs = ensure_slice(3)
-        ts = ensure_iter(4)
-        if length > 5:
-            val = keys[5]
-            if isinstance(val, slice):
-                if val.start is None and val.stop is None and val.step is None:
-                    ps = range(self.positions)
-                else:
-                    ps = range(10**10)[val]
-            elif isinstance(val, int):
-                ps = range(val, val + 1)
-        else:
-            ps = range(self.positions)
-
-        if length > 6 and isinstance(keys[6], int):
-            subdiv = keys[6]
-        else:
-            subdiv = 0
-
-        if len(cs) == 1 and len(ts) == 1 and len(ps) == 1:
-            return self.get_slice(xs, ys, cs[0], zs, ts[0], ps[0], subdiv)
-
-        def slice_len(sl, n):
-            """Calculate the length of the slice over an array of size n.
+            bdv_dict["SequenceDescription"]["ImageLoader"] = {"format": "bdv.hdf5"}
+            bdv_dict["SequenceDescription"]["ImageLoader"]["hdf5"] = {
+                "type": "relative",
+                "text": file_name,
+            }
+
+        # TODO: Consider adding support for tiff/tif files. Needs evaluation.
+        # elif ext == "tiff" or ext == "tif":
+        #     """
+        #     Need to iterate through the time points, etc.
+        #     <ImageLoader format="spimreconstruction.filelist">
+        #         <imglib2container>ArrayImgFactory</imglib2container>
+        #         <ZGrouped>false</ZGrouped>
+        #         <files>
+        #             <FileMapping view_setup="0" timepoint="0" series="0" channel="0">
+        #                 <file type="relative">1_CH00_000000.tif</file>
+        #             </FileMapping>
+        #             <FileMapping view_setup="1" timepoint="0" series="0" channel="0">
+        #                 <file type="relative">1_CH01_000000.tif</file>
+        #             </FileMapping>
+        #         </files>
+        #     </ImageLoader>
+        #     """
+        #     pass
 
-            Parameters
-            ----------
-            sl : slice
-                The slice.
-            n : int
-                The size of the array.
-
-            Returns
-            -------
-            int
-                The length of the slice.
+        elif ext == "n5":
             """
-            sx = sl.indices(n)
-            return (sx[1] - sx[0]) // sx[2]
-
-        sliced_ds = np.empty(
-            (
-                len(ps),
-                len(ts),
-                slice_len(zs, self.shape_z) // self.resolutions[subdiv][2],
-                len(cs),
-                slice_len(ys, self.shape_y) // self.resolutions[subdiv][1],
-                slice_len(xs, self.shape_x) // self.resolutions[subdiv][0],
-            ),
-            dtype=np.uint16,
-        )
-
-        for c in cs:
-            for t in ts:
-                for p in ps:
-                    sliced_ds[p, t, :, c, :, :] = self.get_slice(
-                        xs, ys, c, zs, t, p, subdiv
-                    )
+            <ImageLoader format="bdv.n5" version="1.0">
+                <n5 type="relative">dataset.n5</n5>
+            </ImageLoader>
+            """
+            bdv_dict["SequenceDescription"]["ImageLoader"] = {"format": "bdv.n5"}
+            bdv_dict["SequenceDescription"]["ImageLoader"]["n5"] = {
+                "type": "relative",
+                "text": file_name,
+            }
+
+        # Calculate shear and rotation transforms
+        self.bdv_shear_transform()
+        self.bdv_rotate_transform()
+
+        # Populate ViewSetups
+        bdv_dict["SequenceDescription"]["ViewSetups"] = {}
+        bdv_dict["SequenceDescription"]["ViewSetups"]["ViewSetup"] = []
+        # Attributes are necessary for BigStitcher
+        bdv_dict["SequenceDescription"]["ViewSetups"]["Attributes"] = [
+            {
+                "name": "illumination",
+                "Illumination": {"id": {"text": 0}, "name": {"text": 0}},
+            },
+            {"name": "channel", "Channel": []},
+            {"name": "tile", "Tile": []},
+            {"name": "angle", "Angle": {"id": {"text": 0}, "name": {"text": 0}}},
+        ]
+        # The actual loop that populates ViewSetup
+        view_id = 0
+        for c in range(self.shape_c):
+            # We also take care of the Channel attributes here
+            ch = {"id": {"text": str(c)}, "name": {"text": str(c)}}
+            bdv_dict["SequenceDescription"]["ViewSetups"]["Attributes"][1][
+                "Channel"
+            ].append(ch)
+            for p in range(self.positions):
+                d = {"id": {"text": view_id}, "name": {"text": view_id}}
+                d["size"] = {"text": f"{self.shape_x} {self.shape_y} {self.shape_z}"}
+                d["voxelSize"] = {"unit": {"text": "um"}}
+                d["voxelSize"]["size"] = {"text": f"{self.dx} {self.dy} {self.dz}"}
+                # These attributes are necessary for BigStitcher
+                d["attributes"] = {
+                    "illumination": {"text": "0"},
+                    "channel": {"text": str(c)},
+                    "tile": {"text": str(p)},
+                    "angle": {"text": "0"},
+                }
+                bdv_dict["SequenceDescription"]["ViewSetups"]["ViewSetup"].append(d)
+                view_id += 1
+        # Finish up the Tile Attributes outside of the channels loop so we have
+        # one per tile
+        for p in range(self.positions):
+            tile = {"id": {"text": str(p)}, "name": {"text": str(p)}}
+            bdv_dict["SequenceDescription"]["ViewSetups"]["Attributes"][2][
+                "Tile"
+            ].append(tile)
+
+        # Time
+        bdv_dict["SequenceDescription"]["Timepoints"] = {"type": "range"}
+        bdv_dict["SequenceDescription"]["Timepoints"]["first"] = {"text": 0}
+        bdv_dict["SequenceDescription"]["Timepoints"]["last"] = {
+            "text": self.shape_t - 1
+        }
 
-        return sliced_ds
+        # View registrations
+        bdv_dict["ViewRegistrations"] = {"ViewRegistration": []}
+        for t in range(self.shape_t):
+            for p in range(self.positions):
+                for c in range(self.shape_c):
+                    view_id = c * self.positions + p
+                    mat = np.zeros((3, 4), dtype=float)
+                    for z in range(self.shape_z):
+                        matrix_id = (
+                            z
+                            + self.shape_z * c
+                            + p * self.shape_c * self.shape_z
+                            + t * self.shape_c * self.shape_z * self.positions
+                        )
+
+                        # Construct centroid of volume matrix
+                        # print(matrix_id, views[matrix_id])
+                        try:
+                            mat += (
+                                self.stage_positions_to_affine_matrix(
+                                    **views[matrix_id]
+                                )
+                                / self.shape_z
+                            )
+                        except IndexError:
+                            # We have most likely canceled in the middle of
+                            # an acquisition.
+                            pass
+
+                    view_transforms = [
+                        {
+                            "type": "affine",
+                            "Name": "Translation to Regular Grid",
+                            "affine": {
+                                "text": " ".join([f"{x:.6f}" for x in mat.ravel()])
+                            },
+                        }
+                    ]
+
+                    if self.shear_data:
+                        view_transforms.append(
+                            {
+                                "type": "affine",
+                                "Name": "Shearing Transform",
+                                "affine": {
+                                    "text": " ".join(
+                                        [
+                                            f"{x:.6f}"
+                                            for x in self.shear_transform.ravel()
+                                        ]
+                                    )
+                                },
+                            }
+                        )
+
+                    if self.rotate_data:
+                        view_transforms.append(
+                            {
+                                "type": "affine",
+                                "Name": "Rotation Transform",
+                                "affine": {
+                                    "text": " ".join(
+                                        [
+                                            f"{x:.6f}"
+                                            for x in self.rotate_transform.ravel()
+                                        ]
+                                    )
+                                },
+                            }
+                        )
+
+                    d = dict(timepoint=t, setup=view_id, ViewTransform=view_transforms)
+
+                    bdv_dict["ViewRegistrations"]["ViewRegistration"].append(d)
+
+        return bdv_dict
+
+    def stage_positions_to_affine_matrix(
+        self, x: float, y: float, z: float, theta: float, f: Optional[float] = None
+    ) -> npt.ArrayLike:
+        """Convert stage positions to an affine matrix.
 
-    def get_slice(self, x, y, c, z=0, t=0, p=0, subdiv=0):
-        """Get a single slice of the dataset.
+        Ignore theta, focus for now.
 
         Parameters
         ----------
-        x : int or slice
-            x indices to grab
-        y : int or slice
-            y indices to grab
-        c : int
-            Single channel
-        z : int or slice
-            z indices to grab
-        t : int
-            Single timepoint
-        p : int
-            Single position
-        subdiv : int
-            Subdivision of the dataset to index along
+        x : float
+            The x position of the stage.
+        y : float
+            The y position of the stage.
+        z : float
+            The z position of the stage.
+        theta : float
+            The theta position of the stage.
+        f : Optional[float], optional
+            The focus position of the stage, by default None
 
         Returns
         -------
         npt.ArrayLike
-            3D (z, y, x) slice of data set
+            An affine matrix.
         """
-        setup = self.ds_name(t, c, p).replace("???", str(subdiv))
-        return self.image[setup][z, y, x]
-
-    @property
-    def resolutions(self) -> npt.ArrayLike:
-        """Getter for resolutions.
+        arr = np.eye(3, 4)
 
-        Store as XYZ per BDV spec.
-
-        Returns
-        -------
-        resolutions : npt.ArrayLike
-            The resolutions.
-        """
-        return self._resolutions
+        # Set the transform positions
+        xp, yp, zp = x / self.dx, y / self.dy, z / self.dz
 
-    @property
-    def subdivisions(self) -> npt.ArrayLike:
-        """Getter for subdivisions.
+        # Allow additional axes (e.g. f) to couple onto existing axes (e.g. z)
+        # if they are both moving along the same physical dimension
+        if self._coupled_axes is not None:
+            for leader, follower in self._coupled_axes.items():
+                if leader.lower() not in "xyz":
+                    print(
+                        f"Unrecognized coupled axis {leader}. "
+                        "Not gonna do anything with this."
+                    )
+                    continue
+                elif leader.lower() == "x":
+                    xp += float(locals()[f"{follower.lower()}"]) / self.dx
+                elif leader.lower() == "y":
+                    yp += float(locals()[f"{follower.lower()}"]) / self.dy
+                elif leader.lower() == "z":
+                    zp += float(locals()[f"{follower.lower()}"]) / self.dz
 
-        Store as XYZ per BDV spec.
+        # Translation into pixels
+        arr[:, 3] = [yp, xp, zp]
 
-        Returns
-        -------
-        subdivisions : npt.ArrayLike
-            The subdivisions.
-        """
-        if self._subdivisions is None:
-            self._subdivisions = np.zeros((4, 3), dtype=int)
-            self._subdivisions[:, 0] = np.gcd(32, self.shapes[:, 0])
-            self._subdivisions[:, 1] = np.gcd(32, self.shapes[:, 1])
-            self._subdivisions[:, 2] = np.gcd(32, self.shapes[:, 2])
-
-            # Safety
-            self._subdivisions = np.maximum(self._subdivisions, 1)
-
-            # Reverse to XYZ
-            self._subdivisions = self._subdivisions[:, ::-1]
-        return self._subdivisions
-
-    @property
-    def shapes(self) -> npt.ArrayLike:
-        """Getter for image shape.
+        # Rotation (theta pivots in the xz plane, about the y axis)
+        # sin_theta, cos_theta = np.sin(theta), np.cos(theta)
+        # arr[0,0], arr[2,2] = cos_theta, cos_theta
+        # arr[0,2], arr[2,0] = sin_theta, -sin_theta
 
-        Store as ZYX rather than XYZ, per BDV spec.
+        return arr
 
-        Returns
-        -------
-        shapes : npt.ArrayLike
-            The shapes.
+    def affine_matrix_to_stage_positions(self, mat: npt.ArrayLike) -> tuple:
         """
-        if self._shapes is None:
-            self._shapes = np.maximum(
-                np.ceil(
-                    np.array([self.shape_z, self.shape_y, self.shape_x])[None, :]
-                    / self.resolutions[:, ::-1]
-                ).astype(int),
-                1,
-            )
-        return self._shapes
+        Convert affine matrix back into stage positions.
 
-    @property
-    def nbytes(self) -> int:
-        """Getter for image size.
+        Ignore theta, focus for now.
 
-        Size in bytes. Overrides base class. Accounts for subdivisions.
+        Parameters
+        ----------
+        mat : npt.ArrayLike
+            An affine matrix.
 
         Returns
         -------
-        size : int
-            The size of the image in bytes.
+        tuple
+            A tuple of stage positions.
         """
-        return (
-            np.prod(self.shapes, axis=1)
-            * self.shape_t
-            * self.shape_c
-            * self.positions
-            * self.bits
-            // 8
-        ).sum()
-
-    def set_metadata_from_configuration_experiment(
-        self, configuration: DictProxy
-    ) -> None:
-        """Sets the metadata from according to the microscope configuration.
+        y, x, z = mat[:, 3] * np.array([self.dy, self.dx, self.dz])
+        theta, f = None, None
 
-        Parameters
-        ----------
-        configuration : DictProxy
-            The configuration experiment.
-        """
-        self._subdivisions = None
-        self._shapes = None
+        return x, y, z, theta, f
 
-        # Set rotation and affine transform information in metadata.
-        self.metadata.get_affine_parameters(configuration=configuration)
-        return super().set_metadata_from_configuration_experiment(configuration)
+    def bdv_shear_transform(self):
+        """Calculate the shear transform matrix.
+
+        BDV-specific. Matrix provided is not (4,4), but (3,4).
+        """
+        if self.shear_data:
+            self.shear_transform = affine_shear(
+                dz=self.dz,
+                dx=self.dx,
+                dy=self.dy,
+                dimension=self.shear_dimension,
+                angle=self.shear_angle,
+            )[:3]
+        else:
+            self.shear_transform = np.eye(3, 4)
 
-    def write(self, data: npt.ArrayLike, **kw) -> None:
-        """Writes data to the image file.
+    def bdv_rotate_transform(self):
+        """Calculate the BDV rotation transform matrix.
 
-        Parameters
-        ----------
-        data : npt.ArrayLike
-            The data to write.
-        kw : dict
-            The keyword arguments to write.
+        BDV-specific. Matrix provided is not (4,4), but (3,4).
         """
-        self.mode = "w"
-
-        is_kw = len(kw) > 0
-
-        c, z, t, p = self._cztp_indices(
-            self._current_frame, self.metadata.per_stack
-        )  # find current channel
-
-        if not (z or c or t or p):
-            self.setup()
-
-        ds_name = self.ds_name(t, c, p)
-        for i in range(self.subdivisions.shape[0]):
-            dx, dy, dz = self.resolutions[i, ...]
-            if z % dz == 0:
-                dataset_name = ds_name.replace("???", str(i))
-                # print(z, dz, dataset_name, self.image[dataset_name].shape,
-                #       data[::dx, ::dy].shape)
-                zs = min(z // dz, self.shapes[i, 0] - 1)  # TODO: Is this necessary?
-                self.image[dataset_name][zs, ...] = data[::dy, ::dx].astype(np.int16)
-                if is_kw and (i == 0):
-                    self._views.append(kw)
-        self._current_frame += 1
-
-        # Check if this was the last frame to write
-        c, z, t, p = self._cztp_indices(self._current_frame, self.metadata.per_stack)
-        if (z == 0) and (c == 0) and ((t >= self.shape_t) or (p >= self.positions)):
-            self.setup(
-                self.shape_c * self.positions, self.shape_c * (p + 1), create_flag=False
-            )
-            self.positions = p + 1
+        if self.rotate_data:
+            self.rotate_transform = affine_rotation(
+                x=self.rotate_angle_x, y=self.rotate_angle_y, z=self.rotate_angle_z
+            )[:3]
+        else:
+            self.rotate_transform = np.eye(3, 4)
 
-    def _h5_ds_name(self, t, c, p):
-        """Get the HDF5 dataset name for the given timepoint, channel, and position.
+    def parse_xml(self, root: Union[str, ET.Element]) -> tuple:
+        """Parse a BigDataViewer XML file into our metadata format.
 
         Parameters
         ----------
-        t : int
-            The timepoint.
-        c : int
-            The channel.
-        p : int
-            The position.
+        root : Union[str, ET.Element]
+            The root of the XML tree.
 
         Returns
         -------
-        ds_name : str
-            The dataset name.
+        tuple
+            A tuple containing the file path, setups, and transforms.
         """
-        time_group_name = f"t{t:05}"
-        setup_group_name = f"s{(c*self.positions+p):02}"
-        ds_name = "/".join([time_group_name, setup_group_name, "???", "cells"])
-        return ds_name
 
-    def _n5_ds_name(self, t, c, p):
-        """Get the N5 dataset name for the given timepoint, channel, and position.
-
-        Parameters
-        ----------
-        t : int
-            The timepoint.
-        c : int
-            The channel.
-        p : int
-            The position.
-
-        Returns
-        -------
-        ds_name : str
-            The dataset name.
-        """
-        time_group_name = f"timepoint{t}"
-        setup_group_name = f"setup{(c*self.positions+p)}"
-        ds_name = "/".join([setup_group_name, time_group_name, "s???"])
-        return ds_name
-
-    def read(self) -> None:
-        """Reads data from the image file."""
-        self.mode = "r"
-        if self.__file_type == "h5":
-            self.image = h5py.File(self.file_name, "r")
-        elif self.__file_type == "n5":
-            self.image = zarr.N5Store(self.file_name)
-        xml_fn = os.path.splitext(self.file_name)[0] + ".xml"
-        self.metadata.parse_xml(xml_fn)
-        self.get_shape_from_metadata()
+        # Open the file, if present
+        if isinstance(root, str) and os.path.isfile(root):
+            with open(root, "r") as fp:
+                example = fp.read()
+                root = ET.fromstring(example)
+
+        if root.tag != "SpimData":
+            raise NotImplementedError(f"Unknown format {root.tag} failed to load.")
+
+        # Check if we are loading a BigDataViewer hdf5
+        image_loader = root.find("SequenceDescription/ImageLoader")
+        if image_loader.attrib["format"] not in ["bdv.hdf5", "bdv.n5"]:
+            raise NotImplementedError(
+                f"Unknown format {image_loader.attrib['format']} failed to load."
+            )
 
-    def _setup_h5(self, *args, create_flag=True):
-        """Set up the HDF5 file.
+        # Parse the file path
+        base_path = root.find("BasePath")
+        file = root.find("SequenceDescription/ImageLoader/hdf5")
+        file_path = os.path.join(base_path.text, file.text)
+
+        # Get setups. Each setup represents a visualisation data source in the viewer
+        # that provides one image volume per timepoint
+        setups = [
+            x.text for x in root.findall("SequenceDescription/ViewSetups/ViewSetup/id")
+        ]
+
+        # Get channels, one per setup
+        channels = list(
+            set(
+                [
+                    x.text
+                    for x in root.findall(
+                        "SequenceDescription/ViewSetups/ViewSetup/attributes/channel"
+                    )
+                ]
+            )
+        )
 
-        This function creates the file and the datasets to populate.
-        """
-        if create_flag:
-            self.image = h5py.File(self.file_name, "a")
+        # Get number of positions, one per setup/channel
+        self.positions = len(
+            root.findall("SequenceDescription/ViewSetups/ViewSetup/attributes/tile")
+        ) // len(channels)
+
+        # Get image sizes in (x, y, z), one per setup
+        sizes = [
+            [int(y) for y in x.text.split()]
+            for x in root.findall("SequenceDescription/ViewSetups/ViewSetup/size")
+        ]
+
+        # Get image voxel sizes (dx, dy, dz), one per setup
+        voxel_sizes = [
+            [float(y) for y in x.text.split()]
+            for x in root.findall(
+                "SequenceDescription/ViewSetups/ViewSetup/voxelSize/size"
+            )
+        ]
 
-        setup_start, setup_end = 0, self.shape_c * self.positions
-        if len(args) >= 2:
-            setup_start, setup_end = args[0], args[1]
-
-        # Create setups
-        for i in range(setup_start, setup_end):
-            setup_group_name = f"s{i:02}"
-            if setup_group_name in self.image:
-                del self.image[setup_group_name]
-            self.image.create_dataset(
-                f"{setup_group_name}/resolutions",
-                data=self.resolutions,
-                dtype="float64",
+        # Get timepoints
+        timepoint_type = root.find("SequenceDescription/Timepoints").attrib["type"]
+        if timepoint_type != "range":
+            raise NotImplementedError(
+                f"Unknown format {timepoint_type} failed to load."
             )
-            self.image.create_dataset(
-                f"{setup_group_name}/subdivisions",
-                data=self.subdivisions,
-                dtype="int32",
+        t_start = int(root.find("SequenceDescription/Timepoints/first").text)
+        t_stop = int(root.find("SequenceDescription/Timepoints/last").text)
+        timepoints = (t_start, t_stop + 1)
+
+        # Get affine transformations, one per setup
+        tt, ts = np.array(
+            [
+                [int(x.attrib["timepoint"]), int(x.attrib["setup"])]
+                for x in root.findall("ViewRegistrations/ViewRegistration")
+            ]
+        ).T
+        transforms = [
+            np.array(x.text.split(), dtype=float).reshape(-1, 4)
+            for x in root.findall(
+                "ViewRegistrations/ViewRegistration/ViewTransform/affine"
             )
+        ]
 
-        # Create the datasets to populate
-        for t in range(self.shape_t):
-            time_group_name = f"t{t:05}"
-            for i in range(setup_start, setup_end):
-                setup_group_name = f"s{i:02}"
-                for j in range(self.subdivisions.shape[0]):
-                    dataset_name = "/".join(
-                        [time_group_name, setup_group_name, f"{j}", "cells"]
-                    )
-                    if dataset_name in self.image:
-                        del self.image[dataset_name]
-                    # print(f"Creating {dataset_name} with shape {self.shapes[j,...]}")
-                    self.image.create_dataset(
-                        dataset_name,
-                        chunks=tuple(self.subdivisions[j, ...][::-1]),
-                        shape=self.shapes[j, ...],
-                        dtype="int16",
-                    )
+        # Set up metadata parameters
+        self.dx, self.dy, self.dz = np.array(voxel_sizes).min(
+            0
+        )  # default to finest sampling
+        self._multiposition = self.positions > 1
+        self.shape_x, self.shape_y, self.shape_z = np.array(sizes).max(
+            0
+        )  # default to largest size captured
+        self.shape_c = len(channels)
+        self.shape_t = timepoints[1] - timepoints[0]
+
+        return file_path, setups, transforms
 
-    def _setup_n5(self, *args, create_flag=True):
-        """Set up the N5 file.
+    def write_xml(self, file_name: str, views: list) -> None:
+        """Write BigDataViewer XML metadata.
 
-        This function creates the file and the datasets to populate. By default,
-        it appears to implement blosc compression. Consequently, the anticipated file
-        size, and the actual file size, do not match. This is not the case for HDF5.
-
-        Note
-        ----
-            Setups and timepoints are flipped in N5 vs. HDF5, see
-            https://github.com/bigdataviewer/bigdataviewer-core/blob/master/BDV%20N5%20format.md
+        Parameters
+        ----------
+        file_name : str
+            The file name of the file to be written.
+        views : list
+            A list of dictionaries containing metadata for each view.
 
         """
-        if create_flag:
-            self.__store = zarr.N5Store(self.file_name)
-            self.image = zarr.group(store=self.__store, overwrite=True)
-
-        setup_start, setup_end = 0, self.shape_c * self.positions
-        if len(args) >= 2:
-            setup_start, setup_end = args[0], args[1]
-
-        for i in range(setup_start, setup_end):
-            setup_group_name = f"setup{i}"
-            setup = self.image.create_group(setup_group_name)
-            setup.attrs["downsamplingFactors"] = self.resolutions.tolist()
-            setup.attrs["dataType"] = "int16"
-            for t in range(self.shape_t):
-                time_group_name = f"timepoint{t}"
-                timepoint = setup.create_group(time_group_name)
-                for j in range(self.subdivisions.shape[0]):
-                    s_group_name = f"s{j}"
-                    shape = [int(x) for x in self.shapes[j, ...][::-1]]
-                    # chunks = self.subdivisions[j, ...]
-                    sx = timepoint.zeros(
-                        s_group_name, shape=tuple(shape), chunks=(shape[0], shape[1], 1)
-                    )
-                    sx.attrs["dataType"] = "int16"
-                    sx.attrs["blockSize"] = [shape[0], shape[1], 1]
-                    sx.attrs["dimensions"] = list(shape)
-        # print(self.image.tree())
-
-    def _mode_checks(self) -> None:
-        """Checks that the mode is valid."""
-        self._write_mode = self._mode == "w"
-        self.close()  # if anything was already open, close it
-        if self._write_mode:
-            self._current_frame = 0
-            self._views = []
-            self.setup()
-        else:
-            self.read()
-        self._closed = False
 
-    def close(self) -> None:
-        """Close the image file."""
-        if self._closed:
-            return
-        self._check_shape(self._current_frame - 1, self.metadata.per_stack)
-        if self.__file_type == "n5":
-            self.__store.close()
-        else:
-            self.image.close()
-        if self.mode != "r":
-            self.metadata.write_xml(self.file_name, views=self._views)
-        self._closed = True
+        return super().write_xml(
+            file_name, file_type="bdv", root="SpimData", views=views
+        )
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/data_sources/data_source.py` & `navigate_micro-0.0.6/src/navigate/model/data_sources/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
             self.metadata = None  # Expect a metadata object
         #: str: Mode to open the file in. Can be 'r' or 'w'.
         self._mode = None
         #: bool: Has the data source been closed?
         self._closed = True
         #: int: Number of bits per pixel.
         self.bits = 16
+        if not hasattr(self, "dtype"):
+            self.dtype = "uint16"
 
         #: float: Pixel size in x dimension (microns).
         #: float: Pixel size in y dimension (microns).
         #: float: Pixel size in z dimension (microns).
         self.dx, self.dy, self.dz = 1, 1, 1  # pixel sizes (um)
 
         #: float: The time interval between frames (seconds).
@@ -97,15 +99,15 @@
             1,
             1,
             1,
         )
         #: int: Number of positions in the data source.
         self.positions = 1
 
-        #: str: Mode to open the file in. Can be 'r' or 'w'.
+        # Set the mode using the getters/setters below
         self.mode = mode
 
         #: int: Current frame number.
         self._current_frame = 0
 
     @property
     def nbytes(self) -> int:
@@ -194,14 +196,18 @@
         Returns
         -------
         tuple
             Shape of the data source in XYCZT format.
         """
         return (self.shape_x, self.shape_y, self.shape_c, self.shape_z, self.shape_t)
 
+    def setup(self):
+        """Additional steps for establishing the initial file setup."""
+        pass
+
     def set_metadata_from_configuration_experiment(
         self, configuration: DictProxy
     ) -> None:
         """Sets the metadata from according to the microscope configuration.
 
         Parameters
         ----------
@@ -210,15 +216,15 @@
         """
 
         self.metadata.configuration = configuration
         self.get_shape_from_metadata()
 
     def set_metadata(self, metadata_config: dict) -> None:
         """Sets the metadata
-        
+
         Parameters
         ----------
         metadata_config : dict
             shape configuration: "c", "z", "t", "p", "is_dynamic", "per_stack"
         """
         self.metadata.set_from_dict(metadata_config)
         self.get_shape_from_metadata()
@@ -323,19 +329,27 @@
                 self.metadata.shape_t, self.metadata.positions = maxt + 1, maxp + 1
         # print(
         #     f"result c: {self.shape_c} z: {self.shape_z} "
         #     f"t: {self.shape_t} p: {self.positions}"
         # )
 
     def _mode_checks(self) -> None:
-        """Run additional checks after setting the mode."""
-        pass
+        """Checks that the mode is valid."""
+        self._write_mode = self._mode == "w"
+        self.close()  # if anything was already open, close it
+        if self._write_mode:
+            self._current_frame = 0
+            self._views = []
+            self.setup()
+        else:
+            self.read()
+        self._closed = False
 
     def write(self, data: npt.ArrayLike, **kw) -> None:
-        """Write data to file.
+        """Writes 2D image to the data source.
 
         Parameters
         ----------
         data : npt.ArrayLike
             Data to write to file.
         **kw : dict
             Additional keyword arguments.
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/data_sources/tiff_data_source.py` & `navigate_micro-0.0.6/src/navigate/model/data_sources/tiff_data_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         for i, ax in enumerate(list(self.image.series[0].axes)):
             if ax == "Q":
                 # TODO: This is a hack for tifffile. Find a way to remove this.
                 ax = "Z"
             setattr(self, f"shape_{ax.lower()}", self.data.shape[i])
 
     def write(self, data: npt.ArrayLike, **kw) -> None:
-        """Write data to a tiff file.
+        """Writes 2D image to the data source.
 
         One channel, all z-position, one timepoint = one stack.
         N channels are opened simultaneously for writing.
         At each time point, a new file is opened for each channel.
 
         Parameters
         ----------
@@ -264,26 +264,14 @@
                 tifffile.TiffWriter(
                     file_name, bigtiff=self.is_bigtiff, ome=False, byteorder="<"
                 )
             )
             self.file_name.append(file_name)
             self.uid.append(str(uuid.uuid4()))
 
-    def _mode_checks(self) -> None:
-        """Check that the mode is valid."""
-        self._write_mode = self._mode == "w"
-        self.close()  # if anything was already open, close it
-        if self._write_mode:
-            self._current_frame = 0
-            self._views = []
-            # self._setup_write_image()
-        else:
-            self.read()
-        self._closed = False
-
     def close(self, internal=False) -> None:
         """Close the file.
 
         Parameters
         ----------
         internal : bool
             Internal flag. Do not close if True.
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/device_startup_functions.py` & `navigate_micro-0.0.6/src/navigate/model/device_startup_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,65 +132,45 @@
     if is_synthetic:
         cam_type = "SyntheticCamera"
     else:
         cam_type = configuration["configuration"]["hardware"]["camera"][camera_id][
             "type"
         ]
 
-    if cam_type in ["HamamatsuOrca", "HamamatsuOrcaLightning", "HamamatsuOrcaFire"]:
+    if cam_type in [
+        "HamamatsuOrca",
+        "HamamatsuOrcaLightning",
+        "HamamatsuOrcaFire",
+        "HamamatsuOrcaFusion",
+    ]:
         # Locally Import Hamamatsu API and Initialize Camera Controller
         HamamatsuController = importlib.import_module(
             "navigate.model.devices.APIs.hamamatsu.HamamatsuAPI"
         )
         return auto_redial(HamamatsuController.DCAM, (camera_id,), exception=Exception)
 
     elif cam_type.lower() == "syntheticcamera" or cam_type.lower() == "synthetic":
         from navigate.model.devices.camera.camera_synthetic import (
             SyntheticCameraController,
         )
 
         return SyntheticCameraController()
-    elif cam_type == "Photometrics":
-
-        def import_photometrics(camera_connection):
-            """Import Photometrics API and Initialize Camera Controller.
-
-            Parameters
-            ----------
-            camera_connection : str
-                Camera connection string
-
-            Returns
-            -------
-            camera_toopen : object
-                Camera object.
-
-            Note
-            ----
-                To make this work, please install the SDK at
-                https://www.photometrics.com/support/download/pvcam-sdk
-                and go to APIs/photometrics/PyVCAM-master and run python setup.py
-                install
-            """
-            from pyvcam import pvc
-            from pyvcam.camera import Camera
 
-            pvc.init_pvcam()
-            # camera_names = Camera.get_available_camera_names()
-            camera_toopen = Camera.select_camera(camera_connection)
-            camera_toopen.open()
-            return camera_toopen
+    elif cam_type == "Photometrics":
+        from navigate.model.devices.camera.camera_photometrics import (
+            build_photometrics_connection,
+        )
 
         camera_connection = configuration["configuration"]["hardware"]["camera"][
             camera_id
         ]["camera_connection"]
 
         # return camera object in the auto_redial function.
         return auto_redial(
-            import_photometrics, (camera_connection,), exception=Exception
+            build_photometrics_connection, (camera_connection,), exception=Exception
         )
     else:
         device_not_found("camera", camera_id, cam_type)
 
 
 def start_camera(
     microscope_name,
@@ -248,32 +228,45 @@
 
     elif cam_type == "HamamatsuOrcaFire":
         from navigate.model.devices.camera.camera_hamamatsu import (
             HamamatsuOrcaFire,
         )
 
         return HamamatsuOrcaFire(microscope_name, device_connection, configuration)
-    
+
+    elif cam_type == "HamamatsuOrcaFusion":
+        from navigate.model.devices.camera.camera_hamamatsu import (
+            HamamatsuOrcaFusion,
+        )
+
+        return HamamatsuOrcaFusion(microscope_name, device_connection, configuration)
+
     elif cam_type == "Photometrics":
         from navigate.model.devices.camera.camera_photometrics import (
-            PhotometricsKinetix,
+            PhotometricsBase,
         )
 
-        return PhotometricsKinetix(microscope_name, device_connection, configuration)
+        return PhotometricsBase(microscope_name, device_connection, configuration)
 
     elif cam_type.lower() == "syntheticcamera" or cam_type.lower() == "synthetic":
         from navigate.model.devices.camera.camera_synthetic import SyntheticCamera
 
         return SyntheticCamera(microscope_name, device_connection, configuration)
 
     elif "camera" in plugin_devices:
 
-        return plugin_devices["camera"]["start_device"](
-            microscope_name, device_connection, configuration
-        )
+        for start_function in plugin_devices["camera"]["start_device"]:
+            try:
+                return start_function(
+                    microscope_name, device_connection, configuration, is_synthetic,
+                    device_type="camera"
+                )
+            except RuntimeError:
+                continue
+        device_not_found(microscope_name, "camera", cam_type)
     else:
         device_not_found(microscope_name, "camera", cam_type)
 
 
 def load_mirror(configuration, is_synthetic=False):
     """Initializes the deformable mirror class on a dedicated thread.
 
@@ -457,14 +450,18 @@
                     build_MCLStage_connection,
                     (stage_config["serial_number"],),
                     exception=MadlibError,
                 )
             )
 
         elif stage_type == "ASI" and platform.system() == "Windows":
+            """Filter wheel can be controlled from the same Tiger Controller. If
+            so, then we will load this as a shared device. If not, we will create the
+            connection to the Tiger Controller.
+            """
             filter_wheel = configuration["configuration"]["hardware"]["filter_wheel"][
                 "type"
             ]
             if filter_wheel == "ASI":
                 stage_devices.append("shared device")
             else:
                 from navigate.model.devices.stages.stage_asi import (
@@ -481,30 +478,99 @@
                             stage_config["port"],
                             stage_config["baudrate"],
                         ),
                         exception=TigerException,
                     )
                 )
 
+        elif stage_type == "MS2000" and platform.system() == "Windows":
+            """Filter wheel can be controlled from the same Controller. If
+            so, then we will load this as a shared device. If not, we will create the
+            connection to the Controller.
+
+            TODO: Evaluate whether MS2000 should be able to operate as a shared device.
+            """
+            filter_wheel = configuration["configuration"]["hardware"]["filter_wheel"][
+                "type"
+            ]
+
+            if filter_wheel == "MS2000":
+                stage_devices.append("shared device")
+            else:
+                from navigate.model.devices.stages.stage_asi_MSTwoThousand import (
+                    build_ASI_Stage_connection,
+                )
+                from navigate.model.devices.APIs.asi.asi_MS2000_controller import (
+                    MS2000Exception,
+                )
+
+                stage_devices.append(
+                    auto_redial(
+                        build_ASI_Stage_connection,
+                        (
+                            stage_config["port"],
+                            stage_config["baudrate"],
+                        ),
+                        exception=MS2000Exception,
+                    )
+                )
+
+        elif stage_type == "MFC2000" and platform.system() == "Windows":
+            """Filter wheel can be controlled from the same Tiger Controller. If
+            so, then we will load this as a shared device. If not, we will create the
+            connection to the Tiger Controller.
+
+            TODO: Evaluate whether MFC2000 should be able to operate as a shared device.
+            """
+            filter_wheel = configuration["configuration"]["hardware"]["filter_wheel"][
+                "type"
+            ]
+            if filter_wheel == "MFC2000":
+                stage_devices.append("shared device")
+            else:
+                from navigate.model.devices.stages.stage_asi_MFCTwoThousand import (
+                    build_ASI_Stage_connection,
+                )
+                from navigate.model.devices.APIs.asi.asi_tiger_controller import (
+                    TigerException,
+                )
+
+                stage_devices.append(
+                    auto_redial(
+                        build_ASI_Stage_connection,
+                        (
+                            stage_config["port"],
+                            stage_config["baudrate"],
+                        ),
+                        exception=TigerException,
+                    )
+                )
+
         elif stage_type == "GalvoNIStage" and platform.system() == "Windows":
             stage_devices.append(DummyDeviceConnection())
 
         elif (
             stage_type.lower() == "syntheticstage" or stage_type.lower() == "synthetic"
         ):
             stage_devices.append(DummyDeviceConnection())
 
         elif "stage" in plugin_devices:
-            try:
-                device_connection = plugin_devices["stage"]["load_device"](
-                    configuration, is_synthetic
-                )
-                stage_devices.append(device_connection)
-            except RuntimeError as e:
-                raise e
+            is_found = False
+            for load_function in plugin_devices["stage"]["load_device"]:
+                try:
+                    device_connection = load_function(
+                        stage_config, is_synthetic, device_type="stage"
+                    )
+                    stage_devices.append(device_connection)
+                    is_found = True
+                    break
+                except RuntimeError:
+                    continue
+            if not is_found:
+                device_not_found(stage_type)
         else:
             device_not_found(stage_type)
 
     return stage_devices
 
 
 def start_stage(
@@ -563,40 +629,61 @@
 
         return SutterStage(microscope_name, device_connection, configuration, id)
 
     elif device_type == "Thorlabs":
         from navigate.model.devices.stages.stage_tl_kcube_inertial import TLKIMStage
 
         return TLKIMStage(microscope_name, device_connection, configuration, id)
+    
+    elif device_type == "KST101":
+        from navigate.model.devices.stages.stage_tl_kcube_steppermotor import TLKSTStage
 
+        return TLKSTStage(microscope_name, device_connection, configuration, id)
+    
     elif device_type == "MCL":
         from navigate.model.devices.stages.stage_mcl import MCLStage
 
         return MCLStage(microscope_name, device_connection, configuration, id)
 
     elif device_type == "ASI":
         from navigate.model.devices.stages.stage_asi import ASIStage
 
         return ASIStage(microscope_name, device_connection, configuration, id)
 
+    elif device_type == "MS2000":
+        from navigate.model.devices.stages.stage_asi_MSTwoThousand import ASIStage
+
+        return ASIStage(microscope_name, device_connection, configuration, id)
+
+    elif device_type == "MFC2000":
+        from navigate.model.devices.stages.stage_asi import ASIStage
+
+        return ASIStage(microscope_name, device_connection, configuration, id)
+
     elif device_type == "GalvoNIStage":
         from navigate.model.devices.stages.stage_galvo import GalvoNIStage
 
         return GalvoNIStage(microscope_name, device_connection, configuration, id)
 
     elif device_type.lower() == "syntheticstage" or device_type.lower() == "synthetic":
         from navigate.model.devices.stages.stage_synthetic import SyntheticStage
 
         return SyntheticStage(microscope_name, device_connection, configuration, id)
 
     elif "stage" in plugin_devices:
 
-        return plugin_devices["stage"]["start_device"](
-            microscope_name, device_connection, configuration, id
-        )
+        for start_function in plugin_devices["stage"]["start_device"]:
+            try:
+                return start_function(
+                    microscope_name, device_connection, configuration, is_synthetic,
+                    device_type="stage", id=id
+                )
+            except RuntimeError:
+                continue
+        device_not_found(microscope_name, "stage", device_type, id)
     else:
         device_not_found(microscope_name, "stage", device_type, id)
 
 
 def load_zoom_connection(configuration, is_synthetic=False, plugin_devices={}):
     """Initializes the Zoom class on a dedicated thread.
 
@@ -637,15 +724,20 @@
             build_dynamixel_zoom_connection, (configuration,), exception=Exception
         )
     elif device_type.lower() == "syntheticzoom" or device_type.lower() == "synthetic":
         return DummyDeviceConnection()
 
     elif "zoom" in plugin_devices:
 
-        return plugin_devices["zoom"]["load_device"](configuration)
+        for load_function in plugin_devices["zoom"]["load_device"]:
+            try:
+                return load_function(device_info, is_synthetic, device_type="zoom")
+            except RuntimeError:
+                continue
+        device_not_found("Zoom", device_type)
     else:
         device_not_found("Zoom", device_type)
 
 
 def start_zoom(
     microscope_name,
     device_connection,
@@ -702,19 +794,25 @@
         return SyntheticZoom(microscope_name, device_connection, configuration)
     elif device_type == "NoDevice" or "None":
         from navigate.model.devices.zoom.zoom_base import ZoomBase
 
         return ZoomBase(microscope_name, device_connection, configuration)
     elif "zoom" in plugin_devices:
 
-        return plugin_devices["zoom"]["start_device"](
-            microscope_name, device_connection, configuration
-        )
+        for start_zoom in plugin_devices["zoom"]["start_device"]:
+            try:
+                return start_zoom(
+                    microscope_name, device_connection, configuration, is_synthetic,
+                    device_type="zoom"
+                )
+            except RuntimeError:
+                continue
+        device_not_found("Zoom", device_type)
     else:
-        device_not_found(configuration["configuration"]["hardware"]["zoom"]["type"])
+        device_not_found("Zoom", device_type)
 
 
 def load_filter_wheel_connection(configuration, is_synthetic=False, plugin_devices={}):
     """Initializes the Filter Wheel class on a dedicated thread.
 
     Load filter wheel information from the configuration file. Proper filter wheel types
     include SutterFilterWheel, ASI, and SyntheticFilterWheel.
@@ -767,15 +865,22 @@
         device_type.lower() == "syntheticfilterwheel"
         or device_type.lower() == "synthetic"
     ):
         return DummyDeviceConnection()
 
     elif "filter_wheel" in plugin_devices:
 
-        return plugin_devices["filter_wheel"]["load_device"](device_info)
+        for load_function in plugin_devices["filter_wheel"]["load_device"]:
+            try:
+                return load_function(
+                    device_info, is_synthetic, device_type="filter_wheel"
+                )
+            except RuntimeError:
+                continue
+        device_not_found("filter_wheel", device_type)
     else:
         device_not_found("filter_wheel", device_type)
 
 
 def start_filter_wheel(
     microscope_name,
     device_connection,
@@ -841,17 +946,23 @@
             SyntheticFilterWheel,
         )
 
         return SyntheticFilterWheel(microscope_name, device_connection, configuration)
 
     elif "filter_wheel" in plugin_devices:
 
-        return plugin_devices["filter_wheel"]["start_device"](
-            microscope_name, device_connection, configuration
-        )
+        for start_function in plugin_devices["filter_wheel"]["start_device"]:
+            try:
+                return start_function(
+                    microscope_name, device_connection, configuration, is_synthetic,
+                    device_type="filter_wheel"
+                )
+            except RuntimeError:
+                continue
+        device_not_found(microscope_name, "filter_wheel", device_type)
     else:
         device_not_found(microscope_name, "filter_wheel", device_type)
 
 
 def start_daq(configuration, is_synthetic=False):
     """Initializes the data acquisition (DAQ) class on a dedicated thread.
 
@@ -952,17 +1063,24 @@
         from navigate.model.devices.shutter.laser_shutter_synthetic import (
             SyntheticShutter,
         )
 
         return SyntheticShutter(microscope_name, None, configuration)
 
     elif "shutter" in plugin_devices:
-        return plugin_devices["shutter"]["start_device"](
-            microscope_name, None, configuration
-        )
+
+        for start_function in plugin_devices["shutter"]["start_device"]:
+            try:
+                return start_function(
+                    microscope_name, None, configuration, is_synthetic,
+                    device_type="shutter"
+                )
+            except RuntimeError:
+                continue
+        device_not_found(microscope_name, "shutter", device_type)
 
     else:
         device_not_found(microscope_name, "shutter", device_type)
 
 
 def start_lasers(
     microscope_name,
@@ -1019,17 +1137,22 @@
     elif device_type.lower() == "syntheticlaser" or device_type.lower() == "synthetic":
         if device_connection is not None:
             return device_connection
         from navigate.model.devices.lasers.laser_synthetic import SyntheticLaser
 
         return SyntheticLaser(microscope_name, device_connection, configuration, id)
     elif "lasers" in plugin_devices:
-        return plugin_devices["lasers"]["start_device"](
-            microscope_name, device_connection, configuration, id
-        )
+        for start_function in plugin_devices["lasers"]["start_device"]:
+            try:
+                return start_function(
+                    microscope_name, device_connection, configuration, is_synthetic, device_type="lasers", id=id
+                )
+            except RuntimeError:
+                continue
+        device_not_found(microscope_name, "laser", device_type, id)
     else:
         device_not_found(microscope_name, "laser", device_type, id)
 
 
 def start_remote_focus_device(
     microscope_name,
     device_connection,
@@ -1094,17 +1217,24 @@
         from navigate.model.devices.remote_focus.remote_focus_synthetic import (
             SyntheticRemoteFocus,
         )
 
         return SyntheticRemoteFocus(microscope_name, device_connection, configuration)
 
     elif "remote_focus_device" in plugin_devices:
-        return plugin_devices["remote_focus_device"]["start_device"](
-            microscope_name, device_connection, configuration
-        )
+
+        for start_function in plugin_devices["remote_focus_device"]["start_device"]:
+            try:
+                return start_function(
+                    microscope_name, device_connection, configuration, is_synthetic,
+                    device_type="remote_focus_device"
+                )
+            except RuntimeError:
+                continue
+        device_not_found(microscope_name, "remote_focus", device_type)
 
     else:
         device_not_found(microscope_name, "remote_focus", device_type)
 
 
 def start_galvo(
     microscope_name,
@@ -1156,17 +1286,23 @@
 
         return GalvoNI(microscope_name, device_connection, configuration, id)
     elif device_type.lower() == "syntheticgalvo" or device_type.lower() == "synthetic":
         from navigate.model.devices.galvo.galvo_synthetic import SyntheticGalvo
 
         return SyntheticGalvo(microscope_name, device_connection, configuration, id)
     elif "galvo" in plugin_devices:
-        return plugin_devices["galvo"]["start_device"](
-            microscope_name, device_connection, configuration, id
-        )
+        for start_function in plugin_devices["galvo"]["start_device"]:
+            try:
+                return start_function(
+                    microscope_name, device_connection, configuration, is_synthetic,
+                    device_type="galvo", id=id
+                )
+            except RuntimeError:
+                continue
+        device_not_found(microscope_name, "galvo", id, device_type)
 
     else:
         device_not_found(microscope_name, "galvo", id, device_type)
 
 
 def device_not_found(*args):
     """Display error message if device not found.
@@ -1223,41 +1359,35 @@
     if "camera" in configuration["configuration"]["hardware"].keys():
         devices["camera"] = {}
         for id, device in enumerate(
             configuration["configuration"]["hardware"]["camera"]
         ):
             try:
                 camera = load_camera_connection(configuration, id, is_synthetic)
-            except RuntimeError as e:
+            except RuntimeError as e:  # noqa
                 if "camera" in plugin_devices:
                     camera = plugin_devices["camera"]["load_device"](
                         configuration, id, is_synthetic
                     )
+                else:
+                    raise e
 
             if (not is_synthetic) and device["type"].startswith("Hamamatsu"):
                 camera_serial_number = str(camera._serial_number)
-                device_ref_name = build_ref_name(
-                    "_", device["type"], camera_serial_number
-                )
+                device_ref_name = camera_serial_number
                 # if the serial number has leading zeros,
                 # the yaml reader will convert it to an octal number
                 if camera_serial_number.startswith("0"):
                     try:
                         oct_num = int(camera_serial_number, 8)
-                        devices["camera"][build_ref_name(
-                            "_",
-                            device["type"],
-                            oct_num
-                        )] = camera
+                        device_ref_name = str(oct_num)
                     except ValueError:
                         pass
             else:
-                device_ref_name = build_ref_name(
-                    "_", device["type"], device["serial_number"]
-                )
+                device_ref_name = str(device["serial_number"])
             devices["camera"][device_ref_name] = camera
 
     # load mirror
     if "mirror" in configuration["configuration"]["hardware"].keys():
         devices["mirror"] = {}
         device = configuration["configuration"]["hardware"]["mirror"]
         device_ref_name = build_ref_name("_", device["type"])
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/asi/asi_tiger_controller.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/asi/asi_tiger_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# serialport.py
+# Standard Imports
+import threading
+import time
+
+# Third Party Imports
 from serial import Serial
 from serial import SerialException
 from serial import SerialTimeoutException
 from serial import EIGHTBITS
 from serial import PARITY_NONE
 from serial import STOPBITS_ONE
 from serial.tools import list_ports
-import threading
 
-import time
+# Local Imports
 
 
 class TigerException(Exception):
     """
     Exception raised when error code from Tiger Console is received.
 
     Attributes:
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/coherent/ObisLaser.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/coherent/ObisLaser.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/dynamixel/dynamixel_functions.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/dynamixel/dynamixel_functions.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/hamamatsu/HamamatsuAPI.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/hamamatsu/HamamatsuAPI.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/imagineoptics/imop.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/imagineoptics/imop.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/mcl/madlib.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/mcl/madlib.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/omicron/LuxxLaser.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/omicron/LuxxLaser.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/setup.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/setup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/constants_generator.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/constants_generator.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/camera.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/camera.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/constants.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/src/pyvcam/constants.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/change_settings_test.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/change_settings_test.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/check_frame_status.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/check_frame_status.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/live_mode.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/live_mode.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/meta_data.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/meta_data.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_camera.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_camera.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_rois.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/multi_rois.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/newest_frame.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/newest_frame.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/seq_mode.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/seq_mode.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/stream_to_disk.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/stream_to_disk.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/sw_trigger.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/sw_trigger.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/test_camera.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/sutter/MP285.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/sutter/MP285.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/APIs/thorlabs/kcube_inertial.py` & `navigate_micro-0.0.6/src/navigate/model/devices/APIs/thorlabs/kcube_inertial.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/__init__.py` & `navigate_micro-0.0.6/src/navigate/model/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_base.py` & `navigate_micro-0.0.6/src/navigate/model/devices/camera/camera_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_hamamatsu.py` & `navigate_micro-0.0.6/src/navigate/model/devices/camera/camera_hamamatsu.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,48 +44,14 @@
 
 
 class HamamatsuBase(CameraBase):
     """HamamatsuOrca camera class.
 
     This is the default parent class for Hamamatsu Cameras.
     This includes the ORCA Flash 4.0, Fusion, Lightning, and Fire.
-
-    **Configuration**::
-
-        hardware:
-          camera:
-            -
-                type: HamamatsuOrca
-                serial_number: 302158
-            -
-                type: HamamatsuOrca
-                serial_number: 302159
-        ...
-
-        microscopes:
-          microscope_name:
-            camera:
-              hardware:
-                name: camera
-                type: HamamatsuOrca
-                serial_number: 302352
-              lightsheet_rolling_shutter_width: 608
-              defect_correct_mode: 2.0 # Off: 1.0, On: 2.0
-              delay_percent: 10
-              pulse_percent: 1
-              x_pixels_step: 4
-              y_pixels_step: 4
-              x_pixels_min: 4
-              y_pixels_min: 4
-              exposure_time_range:
-                min: 1
-                max: 1000
-                step: 1
-              flip_x: False
-              flip_y: False
     """
 
     def __init__(self, microscope_name, device_connection, configuration):
         """Initialize HamamatsuOrca class.
 
         Parameters
         ----------
@@ -99,23 +65,31 @@
         super().__init__(microscope_name, device_connection, configuration)
 
         #: dict: Camera parameters
         self.camera_parameters["x_pixels"] = self.camera_controller.max_image_width
         self.camera_parameters["y_pixels"] = self.camera_controller.max_image_height
         self.camera_parameters["x_pixels_min"] = self.camera_controller.min_image_width
         self.camera_parameters["y_pixels_min"] = self.camera_controller.min_image_height
-        self.camera_parameters["x_pixels_step"] = self.camera_controller.step_image_width
-        self.camera_parameters["y_pixels_step"] = self.camera_controller.step_image_height
-        self.minimum_exposure_time, _, _ = self.camera_controller.get_property_range("exposure_time")
+        self.camera_parameters[
+            "x_pixels_step"
+        ] = self.camera_controller.step_image_width
+        self.camera_parameters[
+            "y_pixels_step"
+        ] = self.camera_controller.step_image_height
+        self.minimum_exposure_time, _, _ = self.camera_controller.get_property_range(
+            "exposure_time"
+        )
 
         #: object: Camera controller
         if self.camera_controller.get_property_value("readout_speed"):
             _, speed_max, _ = self.camera_controller.get_property_range("readout_speed")
             if speed_max is not None:
-                self.camera_controller.set_property_value("readout_speed", int(speed_max))
+                self.camera_controller.set_property_value(
+                    "readout_speed", int(speed_max)
+                )
                 self.camera_parameters["readout_speed"] = int(speed_max)
             else:
                 self.camera_controller.set_property_value("readout_speed", 1)
                 self.camera_parameters["readout_speed"] = 1
 
         self.camera_parameters[
             "pixel_size_in_microns"
@@ -174,21 +148,24 @@
             "trigger_polarity",
             "trigger_source",
             "internal_line_interval",
             "internal_line_speed",
             "image_height",
             "image_width",
             "exposure_time",
-            "readout_time"
+            "readout_time",
         ]
         for param in params:
             print(param, self.camera_controller.get_property_value(param))
             logger.info(f"{param}, {self.camera_controller.get_property_value(param)}")
 
-        print("*** exposure time range:", self.camera_controller.get_property_range("exposure_time"))
+        print(
+            "*** exposure time range:",
+            self.camera_controller.get_property_range("exposure_time"),
+        )
 
     def close_camera(self):
         """Close HamamatsuOrca Camera"""
         self.camera_controller.dev_close()
 
     def set_sensor_mode(self, mode):
         """Set HamamatsuOrca sensor mode.
@@ -210,18 +187,26 @@
             ) = self.camera_controller.get_property_range("subarray_hsize")
             (
                 self.camera_controller.min_image_height,
                 _,
                 self.camera_controller.step_image_height,
             ) = self.camera_controller.get_property_range("subarray_vsize")
             # update configuration dict
-            self.camera_parameters["x_pixels_min"] = self.camera_controller.min_image_width
-            self.camera_parameters["y_pixels_min"] = self.camera_controller.min_image_height
-            self.camera_parameters["x_pixels_step"] = self.camera_controller.step_image_width
-            self.camera_parameters["y_pixels_step"] = self.camera_controller.step_image_height
+            self.camera_parameters[
+                "x_pixels_min"
+            ] = self.camera_controller.min_image_width
+            self.camera_parameters[
+                "y_pixels_min"
+            ] = self.camera_controller.min_image_height
+            self.camera_parameters[
+                "x_pixels_step"
+            ] = self.camera_controller.step_image_width
+            self.camera_parameters[
+                "y_pixels_step"
+            ] = self.camera_controller.step_image_height
         else:
             print("Camera mode not supported")
             logger.info("Camera mode not supported")
 
     def set_readout_direction(self, mode):
         """Set HamamatsuOrca readout direction.
 
@@ -236,15 +221,17 @@
             "bytrigger": 3.0,
             "diverge": 5.0,
             "Bidirectional": 6.0,
             "Rev. Bidirectional": 7.0,
         }
 
         if mode in readout_direction_dict:
-            self.camera_controller.set_property_value("readout_direction", readout_direction_dict[mode])
+            self.camera_controller.set_property_value(
+                "readout_direction", readout_direction_dict[mode]
+            )
         else:
             print("Camera readout direction not supported")
             logger.info("Camera readout direction not supported")
 
     def calculate_readout_time(self):
         """Calculate duration of time needed to readout an image.
 
@@ -258,30 +245,28 @@
         readout_time : float
             Duration of time needed to readout an image.
 
         """
         readout_time = self.camera_controller.get_property_value("readout_time")
 
         # with camera internal delay
-        return readout_time + 4 * self.minimum_exposure_time
+        return readout_time  # + 4 * self.minimum_exposure_time
 
     def set_exposure_time(self, exposure_time):
         """Set HamamatsuOrca exposure time.
 
         Note
         ----
             Units of the Hamamatsu API are in seconds.
-            Units for the software are in milliseconds. Conversion is done here.
 
         Parameters
         ----------
         exposure_time : float
             Exposure time in seconds.
         """
-        exposure_time = exposure_time
         return self.camera_controller.set_property_value("exposure_time", exposure_time)
 
     def set_line_interval(self, line_interval_time):
         """Set HamamatsuOrca line interval.
 
         Parameters
         ----------
@@ -395,16 +380,17 @@
         return self.x_pixels == roi_width and self.y_pixels == roi_height
 
     def initialize_image_series(self, data_buffer=None, number_of_frames=100):
         """Initialize HamamatsuOrca image series.
 
         Parameters
         ----------
-        data_buffer : int
-            Size of the data to buffer.  Default is None.
+        data_buffer :
+            List of SharedNDArrays of shape=(self.img_height, self.img_width) and dtype="uint16" # noqa
+            Default is None.
         number_of_frames : int
             Number of frames.  Default is 100.
         """
         self.camera_controller.start_acquisition(data_buffer, number_of_frames)
         self.is_acquiring = True
 
     def close_image_series(self):
@@ -417,42 +403,18 @@
 
     def get_new_frame(self):
         """Get frame from HamamatsuOrca camera.
 
         Returns
         -------
         frame : numpy.ndarray
-            Frame from HamamatsuOrca camera.
+            Frame ids from HamamatsuOrca camera.
         """
         return self.camera_controller.get_frames()
 
-    def get_minimum_waiting_time(self):
-        """Get minimum waiting time for HamamatsuOrca.
-
-        This function gets the timing information from the camera device
-        cyclic_trigger_period, minimum_trigger_blank, minimum_trigger_interval
-        'cyclic_trigger_period' if current device is 0.
-
-        According to the documentation, trigger_blank should be bigger than
-        trigger_interval.
-
-        Returns
-        -------
-        trigger_blank : float
-            Minimum waiting time.
-        """
-        # cyclic_trigger =
-        #   self.camera_controller.get_property_value('cyclic_trigger_period')
-        trigger_blank = self.camera_controller.get_property_value(
-            "minimum_trigger_blank"
-        )
-        # trigger_interval =
-        #   self.camera_controller.get_property_value('minimum_trigger_interval')
-        return trigger_blank
-
 
 class HamamatsuOrcaLightning(HamamatsuBase):
     """HamamatsuOrcaLightning camera class."""
 
     def __init__(self, microscope_name, device_connection, configuration):
         """Initialize HamamatsuOrcaLightning class.
 
@@ -496,19 +458,21 @@
         """
 
         camera_line_interval = full_chip_exposure_time / (
             6 + (shutter_width + self.y_pixels) / 4
         )
         self.camera_parameters["line_interval"] = camera_line_interval
 
-        maximum_internal_line_interval = 0.0002 # 200.0 us
+        maximum_internal_line_interval = 0.0002  # 200.0 us
         if camera_line_interval > maximum_internal_line_interval:
             camera_line_interval = maximum_internal_line_interval
-            full_chip_exposure_time = camera_line_interval * (6 + (shutter_width + self.y_pixels) / 4)
-        
+            full_chip_exposure_time = camera_line_interval * (
+                6 + (shutter_width + self.y_pixels) / 4
+            )
+
         exposure_time = camera_line_interval * ((shutter_width + 3) // 4)
         return exposure_time, camera_line_interval, full_chip_exposure_time
 
 
 class HamamatsuOrcaFire(HamamatsuBase):
     def __init__(self, microscope_name, device_connection, configuration):
         """Initialize HamamatsuOrcaFire class.
@@ -520,27 +484,32 @@
         device_connection : object
             Hardware device to connect to
         configuration : multiprocessing.managers.DictProxy
             Global configuration of the microscope
         """
         HamamatsuBase.__init__(self, microscope_name, device_connection, configuration)
         self.camera_parameters["supported_readout_directions"] = [
-            "Top-to-Bottom", "Bottom-to-Top", "Bidirectional", "Rev. Bidirectional"]
+            "Top-to-Bottom",
+            "Bottom-to-Top",
+            "Bidirectional",
+            "Rev. Bidirectional",
+        ]
 
         # self.minimum_exposure_time = 7.309 * 10 ** -6  # 7.309 us
 
         self.camera_parameters["x_pixels"] = self.camera_controller.get_property_value(
-            "image_width")
+            "image_width"
+        )
 
         self.camera_parameters["y_pixels"] = self.camera_controller.get_property_value(
-            "image_height")
+            "image_height"
+        )
 
         logger.info("HamamatsuOrcaFire Initialized")
 
-
     def calculate_light_sheet_exposure_time(
         self, full_chip_exposure_time, shutter_width
     ):
         """Convert normal mode exposure time to light-sheet mode exposure time.
         Calculate the parameters for an acquisition
 
         Parameters
@@ -559,24 +528,26 @@
         full_chip_exposure_time : float
             Updated full chip exposure time (s).
         """
         # 4H delay, (Vn/2+5)H readout
         camera_line_interval = full_chip_exposure_time / (
             9 + (shutter_width + self.y_pixels) / 2
         )
-        
-        maximum_internal_line_interval = 0.0002339 # 233.9 us
+
+        maximum_internal_line_interval = 0.0002339  # 233.9 us
         if camera_line_interval > maximum_internal_line_interval:
             camera_line_interval = maximum_internal_line_interval
-            full_chip_exposure_time = camera_line_interval * (9 + (shutter_width + self.y_pixels) / 2)
+            full_chip_exposure_time = camera_line_interval * (
+                9 + (shutter_width + self.y_pixels) / 2
+            )
 
         self.camera_parameters["line_interval"] = camera_line_interval
 
         # round up exposure time
-        exposure_time = camera_line_interval * ((shutter_width+1) // 2)
+        exposure_time = camera_line_interval * ((shutter_width + 1) // 2)
         return exposure_time, camera_line_interval, full_chip_exposure_time
 
 
 class HamamatsuOrca(HamamatsuBase):
     def __init__(self, microscope_name, device_connection, configuration):
         """Initialize HamamatsuOrca class.
 
@@ -590,15 +561,17 @@
             Hardware device to connect to
         configuration : multiprocessing.managers.DictProxy
             Global configuration of the microscope
         """
         HamamatsuBase.__init__(self, microscope_name, device_connection, configuration)
 
         self.camera_parameters["supported_readout_directions"] = [
-            "Top-to-Bottom", "Bottom-to-Top"]
+            "Top-to-Bottom",
+            "Bottom-to-Top",
+        ]
 
         # self.minimum_exposure_time = 9.74436 * 10 ** -6
 
         logger.info("HamamatsuOrca Initialized")
 
     def calculate_light_sheet_exposure_time(
         self, full_chip_exposure_time, shutter_width
@@ -618,19 +591,87 @@
         exposure_time : float
             Light-sheet mode exposure time (s).
         camera_line_interval : float
             HamamatsuOrca line interval duration (s).
         full_chip_exposure_time : float
             Updated full chip exposure time (s).
         """
-        camera_line_interval = full_chip_exposure_time / (4 + shutter_width + self.y_pixels)
-        
-        maximum_internal_line_interval = 963.8e-6 # 963.8 us
+        camera_line_interval = full_chip_exposure_time / (
+            10 + shutter_width + self.y_pixels
+        )
+
+        maximum_internal_line_interval = 0.1  # 100ms
         if camera_line_interval > maximum_internal_line_interval:
             camera_line_interval = maximum_internal_line_interval
-            full_chip_exposure_time = camera_line_interval * (4 + shutter_width + self.y_pixels)
+            full_chip_exposure_time = camera_line_interval * (
+                10 + shutter_width + self.y_pixels
+            )
 
-        self.camera_parameters["line_interval"] = camera_line_interval
+        self.camera_parameters["line_interval"] = camera_line_interval * shutter_width
+
+        # round up exposure time
+        exposure_time = camera_line_interval * shutter_width
+        return exposure_time, camera_line_interval, full_chip_exposure_time
+
+
+class HamamatsuOrcaFusion(HamamatsuBase):
+    """HamamatsuOrcaFusion camera class."""
+
+    def __init__(self, microscope_name, device_connection, configuration):
+        """Initialize HamamatsuOrcaFusion class.
+
+        Parameters
+        ----------
+        microscope_name : str
+            Name of microscope in configuration
+        device_connection : object
+            Hardware device to connect to
+        configuration : multiprocessing.managers.DictProxy
+            Global configuration of the microscope
+        """
+        HamamatsuBase.__init__(self, microscope_name, device_connection, configuration)
+
+        self.camera_parameters["supported_readout_directions"] = [
+            "Top-to-Bottom",
+            "Bottom-to-Top",
+        ]
+
+        logger.info("HamamatsuOrcaFusion Initialized")
+
+    def calculate_light_sheet_exposure_time(
+        self, full_chip_exposure_time, shutter_width
+    ):
+        """Calculate light sheet exposure time.
+
+        Parameters
+        ----------
+        full_chip_exposure_time : float
+            Full chip exposure time in seconds.
+        shutter_width : int
+            Shutter width.
+
+        Returns
+        -------
+        exposure_time : float
+            Exposure time in seconds.
+        camera_line_interval : float
+            Camera line interval in seconds.
+        full_chip_exposure_time : float
+            Full chip exposure time in seconds.
+        """
+
+        camera_line_interval = full_chip_exposure_time / (
+            4 + shutter_width + self.y_pixels
+        )
+
+        maximum_internal_line_interval = 963.8e-6  # 963.8 us
+        if camera_line_interval > maximum_internal_line_interval:
+            camera_line_interval = maximum_internal_line_interval
+            full_chip_exposure_time = camera_line_interval * (
+                4 + shutter_width + self.y_pixels
+            )
+
+        self.camera_parameters["line_interval"] = camera_line_interval * shutter_width
 
         # round up exposure time
         exposure_time = camera_line_interval * shutter_width
         return exposure_time, camera_line_interval, full_chip_exposure_time
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_photometrics.py` & `navigate_micro-0.0.6/src/navigate/model/devices/camera/camera_photometrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,32 +30,67 @@
 # POSSIBILITY OF SUCH DAMAGE.
 #
 
 # Standard Library Imports
 import logging
 
 # Third Party Imports
-# you shouldn't need to call this as self.controller is the camera object
-# and should have everything needed
 from ctypes import *  # noqa
 import numpy as np
+from pyvcam import pvc
+from pyvcam.camera import Camera
 
 # Local Imports
 from navigate.model.devices.camera.camera_base import CameraBase
 
 # Logger Setup
 p = __name__.split(".")[1]
 logger = logging.getLogger(p)
 
 
-class PhotometricsKinetix(CameraBase):
-    """Photometrics Kinetix camera class.
+def build_photometrics_connection(camera_connection):
+    """Build Sutter Stage Serial Port connection
+
+    Import Photometrics API and Initialize Camera Controller.
+
+    Parameters
+    ----------
+    camera_connection : str
+        Camera connection string
+
+    Returns
+    -------
+    camera_to_open : object
+        Camera object.
+    """
+    try:
+        pvc.init_pvcam()
+        # camera_names = Camera.get_available_camera_names()
+        camera_to_open = Camera.select_camera(camera_connection)
+        camera_to_open.open()
+        return camera_to_open
+    except Exception as e:
+        logger.debug(f"Could not establish connection with camera: {e}")
+        raise UserWarning(
+            "Could not establish connection with camera", camera_connection
+        )
+
+
+class PhotometricsBase(CameraBase):
+    """Photometrics Base camera class.
 
     This class is the interface between the rest of the microscope code and the
-    Photometrics API.
+    Photometrics API. It has been tested with the Photometrics Iris 15
+
+
+    Note
+    ----
+        If you want to use a photometrics camera, please go first to the
+        PyVCAM-master folder in APIs and run:
+        python setup.py install
     """
 
     def __init__(self, microscope_name, device_connection, configuration):
         """Initialize the Photometrics class.
 
         Parameters
         ---------
@@ -68,118 +103,97 @@
         -------
 
         """
         super().__init__(microscope_name, device_connection, configuration)
 
         #: int: Exposure Time in milliseconds
         self._exposuretime = 20
+
         #: int: Scan Mode (0 = Normal, 1 = ASLM)
         self._scanmode = 0
+
         #: int: Scan Delay
         self._scandelay = 1
+
         #: int: Number of frames
         self._numberofframes = 100
+
         #: obj: Data Buffer
         self._databuffer = None
+
         #: int: Number of frames received
         self._frames_received = 0
-        #: float: Unit for line delay
-        self._unitforlinedelay = 0.00375  # 3.75  us for dynamic mode kinetix
+
         #: list: Frame IDs
         self._frame_ids = []
+
         #: dict: Camera parameters
         self.camera_parameters["x_pixels"] = self.camera_controller.sensor_size[0]
         self.camera_parameters["y_pixels"] = self.camera_controller.sensor_size[1]
 
-        # todo: complete first init of parameters to default values
-
-        # Values are pulled from the CameraParameters section of the
-        # configuration.yml file.
-        # Exposure time converted here from milliseconds to seconds.
         self.set_sensor_mode("Normal")
         self.camera_controller.binning = 1
-        # not implemented: readout_speed, defect_correct_mode
+        # TODO: Implement readout_speed, defect_correct_mode
         self.camera_controller.exp_mode = "Edge Trigger"
         self.camera_controller.prog_scan_dir = 0
-        # self.camera_controller.speed_table_index = 1 # 1 for 100 MHz
-        self.camera_controller.readout_port = 0
-        self.camera_controller.gain = 1
-        #
-        # self.camera_controller.set_property_value("trigger_active",
-        #                                           self.camera_parameters[
-        #                                           'trigger_active'])
-        # self.camera_controller.set_property_value("trigger_mode",
-        #                                           self.camera_parameters[
-        #                                           'trigger_mode'])
-        # self.camera_controller.set_property_value("trigger_polarity",
-        #                                           self.camera_parameters[
-        #                                           \'trigger_polarity'])
-        # self.camera_controller.set_property_value("trigger_source",
-        #                                           self.camera_parameters[
-        #                                           'trigger_source'])
-        # # DCAM_IDPROP_IMAGE_WIDTH/HEIGHT is readonly
-        # self.camera_controller.set_property_value("image_height",
-        #                                            self.camera_parameters[
-        #                                            'y_pixels'])
-        # self.camera_controller.set_property_value("image_width",
-        #                                            self.camera_parameters[
-        #                                            'x_pixels'])
+
+        # Photometrics camera settings from config file
+        self.camera_controller.readout_port = self.camera_parameters["readout_port"]
+        self.camera_controller.speed_table_index = self.camera_parameters[
+            "speed_table_index"
+        ]
+        self.camera_controller.gain = self.camera_parameters["gain"]
 
         logger.info("Photometrics Initialized")
 
     def __del__(self):
-        """Delete PhotometricsKinetix object."""
+        """Delete PhotometricsBase object."""
         if hasattr(self, "camera_controller"):
             self.camera_controller.close()
-            # pvc.uninit_pvcam()
-            print("camera closed")
-        logger.info("PhotometricsKinetix Shutdown")
+        logger.info("PhotometricsBase Shutdown")
 
     @property
     def serial_number(self):
         """Get Camera Serial Number
 
         Returns
         -------
         serial_number : str
             Serial number for the camera.
         """
-        # return self.camera_controller._serial_number
-        ser_no = self.camera_controller.serial_no
-        return ser_no
+        return self.camera_controller.serial_no
 
     def report_settings(self):
         """Print Camera Settings."""
-        # todo: complete param recording
+        # TODO: complete param recording
         print("sensor_mode: " + str(self.camera_controller.prog_scan_mode))
         print("binning: " + str(self.camera_controller.binning))
         print("readout_speed" + str(self.camera_controller.readout_time))
         print("trigger_active")
         print("trigger_mode")
         print("trigger_polarity")
         print("trigger_source")
         print("internal_line_interval")
         print("sensor size" + str(self.camera_controller.sensor_size))
         print("image_height and width" + str(self.x_pixels) + ", " + str(self.y_pixels))
-
         print("exposure_time" + str(self._exposuretime))
 
     def close_camera(self):
-        """Close Photometrics Kinetix Camera"""
+        """Close Photometrics Camera"""
         self.camera_controller.close()
 
     def set_sensor_mode(self, mode):
         """Set Photometrics sensor mode
 
         Can be normal or programmable scan mode (e.g., ASLM).
 
         Parameters
         ----------
         mode : str
-            'Normal (static)' or 'Light-Sheet (ASLM)'
+            'Normal' (static) or 'Light-Sheet' (ASLM)
         """
         modes_dict = {"Normal": 0, "Light-Sheet": 1}
         if mode in modes_dict:
             self.camera_controller.prog_scan_mode = modes_dict[mode]
             self._scanmode = modes_dict[mode]
         else:
             print("Camera mode not supported" + str(modes_dict[mode]))
@@ -191,104 +205,67 @@
         Parameters
         ----------
         mode : str
             'Top-to-Bottom', 'Bottom-to-Top', 'Alternate'
             Scan direction options: {'Down': 0, 'Up': 1, 'Down/Up Alternate': 2}
 
         """
-        print("available scan directions on camera are:")
-        print(str(self.camera_controller.prog_scan_dirs))
+        # print("available scan directions on camera are:")
+        # print(str(self.camera_controller.prog_scan_dirs))
 
         if mode == "Top-to-Bottom":
             #  'Down' readout direction
             self.camera_controller.prog_scan_dir = 0
         elif mode == "Bottom-to-Top":
             #  'Up' readout direction
             self.camera_controller.prog_scan_dir = 1
         elif mode == "Alternate":
             self.camera_controller.prog_scan_dir = 2
         else:
-            print("Camera readout direction not supported")
             logger.info("Camera readout direction not supported")
 
     def calculate_readout_time(self):
         """Calculate duration of time needed to readout an image.
 
         Calculates the readout time and maximum frame rate according to the camera
         configuration settings.
 
-        Warn
+        Note
         ----
-            Not implemented. Currently hard-coded for Hamamatsu Orca Flash 4.0.
+            Function only called for normal acquisition mode.
 
         Returns
         -------
         readout_time : float
-            Duration of time needed to readout an image.
+            Duration of time needed to readout an image in seconds.
         """
 
-        # todo
-        h = 3.75 * 10**-6  # Readout timing constant
-        # h = self.camera_controller.get_property_value("readout_time")
-        vn = self.y_pixels
-        exposure_time = self._exposuretime
-        # trigger_source = self.camera_controller.get_property_value('trigger_source')
-        # trigger_active = self.camera_controller.get_property_value('trigger_active')
-        #
-        if self._scanmode == 0:  # normal/static light-sheet
-            readout_time = exposure_time - ((vn + 10) * h + exposure_time)
-        else:
-            # todo: not sure if these equations are correct
-            readout_time = exposure_time - (
-                (vn + 10) * h * self._scandelay + exposure_time
-            )
+        # get the readout time from the Photometrics camera in us
+        readout_time_ms = self.camera_controller.readout_time / 1000
 
-            #
-        #     #  Area sensor mode operation
-        #     if trigger_source == 1:
-        #         # Internal Trigger Source
-        #         max_frame_rate = 1 / ((vn / 2) * h)
-        #         readout_time = exposure_time - ((vn / 2) * h)
-        #
-        #     if trigger_active == 1 or 2:
-        #         #  External Trigger Source
-        #         #  Edge == 1, Level == 2
-        #         max_frame_rate = 1 / ((vn / 2) * h + exposure_time + 10 * h)
-        #         readout_time = exposure_time - ((vn / 2) * h + exposure_time + 10 * h)
-        #
-        #     if trigger_active == 3:
-        #         #  External Trigger Source
-        #         #  Synchronous Readout == 3
-        #         max_frame_rate = 1 / ((vn / 2) * h + 5 * h)
-        #         readout_time = exposure_time - ((vn / 2) * h + 5 * h)
-        #
-        # if sensor_mode == 12:
-        #     #  Progressive sensor mode operation
-        #     max_frame_rate = 1 / (exposure_time + (vn + 10) * h)
-        #     readout_time = exposure_time - 1 / (exposure_time + (vn + 10) * h)
-        #
-        return readout_time
+        return readout_time_ms / 1000
 
     def set_exposure_time(self, exposure_time):
         """Set Photometrics exposure time.
 
-        Units of the Photometrics API are in seconds.
-        All of our units are in milliseconds.
+        Note: Units of the Photometrics API are in milliseconds
 
         Parameters
         ----------
         exposure_time : float
-            Exposure time in milliseconds.
+            Exposure time in seconds.
 
         Returns
         -------
         exposure_time : float
-            Exposure time in seconds.
+            Exposure time in milliseconds.
         """
-        self._exposuretime = exposure_time
+        self._exposuretime = int(exposure_time * 1000)
+        self.camera_controller.exp_time = self._exposuretime
+        self.camera_controller.start_live(self._exposuretime)
         return exposure_time
 
     def set_line_interval(self, line_interval_time):
         """Set Photometrics line interval.
 
         Parameters
         ----------
@@ -303,85 +280,62 @@
     ):
         """Convert normal mode exposure time to light-sheet mode exposure time.
         Calculate the parameters for an ASLM acquisition
 
         Parameters
         ----------
         full_chip_exposure_time : float
-            Normal mode exposure time.
+            Normal mode exposure time in seconds
         shutter_width : int
+            Shutter width in pixels
 
         Returns
         -------
         exposure_time : float
-            Light-sheet mode exposure time.
+            Light-sheet mode exposure time in seconds
         camera_line_interval : float
             HamamatsuOrca line interval duration.
         full_chip_exposure_time : float
             Full chip exposure time (s)
         """
-        # TODO: what's the units of the input full_chip_exposure_time? miliseconds or seconds?
 
-        linedelay = self._unitforlinedelay  # 10.16us
+        # size of ROI
         nbrows = self.y_pixels
-        ASLM_scanWidth = 70
 
+        # transform exposure time to milliseconds for Photometrics API.
+        full_chip_exposure_time = full_chip_exposure_time * 1000
+
+        # equations to calculate ASLM parameters
+        linedelay = self.camera_parameters["unitforlinedelay"] / 1000
         ASLM_lineExposure = int(
-            np.ceil(full_chip_exposure_time / (1 + nbrows / ASLM_scanWidth))
+            np.ceil(full_chip_exposure_time / (1 + (1 + nbrows) / shutter_width))
         )
         ASLM_line_delay = (
             int(
                 np.ceil(
-                    (full_chip_exposure_time - ASLM_lineExposure) / (nbrows * linedelay)
+                    (full_chip_exposure_time - ASLM_lineExposure)
+                    / ((nbrows + 1) * linedelay)
                 )
             )
             - 1
         )
+
         ASLM_acquisition_time = (
             (ASLM_line_delay + 1) * nbrows * linedelay
             + ASLM_lineExposure
             + (ASLM_line_delay + 1) * linedelay
         )
 
         self.camera_parameters["line_interval"] = ASLM_lineExposure
-
         self._exposuretime = ASLM_lineExposure
         self._scandelay = ASLM_line_delay
-        print(
-            "ASLM parameters are: {} exposure time, and {} line delay factor, {} "
-            "total acquisition time for {} scan width".format(
-                ASLM_lineExposure,
-                ASLM_line_delay,
-                ASLM_acquisition_time,
-                ASLM_scanWidth,
-            )
-        )
-
-        return ASLM_lineExposure, ASLM_line_delay, full_chip_exposure_time
-
-    def _calculate_ASLMparameters(self, desired_exposuretime):
-        """Calculate the parameters for an ASLM acquisition
-
-        Parameters
-        ----------
-        desired_exposuretime : float
-            Exposure time in milliseconds.
-
-        Returns
-        -------
-        exposure_time : float
-            Light-sheet mode exposure time.
-
-        Warn
-        ----
-            Not implemented. No code in this function.
-        """
+        return ASLM_lineExposure / 1000, ASLM_line_delay, ASLM_acquisition_time / 1000
 
     def set_binning(self, binning_string):
-        """Set HamamatsuOrca binning mode.
+        """Set Photometrics binning mode.
 
         Parameters
         ----------
         binning_string : str
             Desired binning properties (e.g., '1x1', '2x2',
             '4x4', '8x8', '16x16', '1x2', '2x4')
 
@@ -391,49 +345,61 @@
             True if binning was set successfully, False otherwise.
 
         """
         binning_dict = {
             "1x1": 1,
             "2x2": 2,
             "4x4": 4,
+            "8x8": 8,
         }
         if binning_string not in binning_dict.keys():
             logger.debug(f"can't set binning to {binning_string}")
-            print(f"can't set binning to {binning_string}")
+            print(f"Can't set binning to {binning_string}")
             return False
         self.camera_controller.binning = binning_dict[binning_string]
         idx = binning_string.index("x")
+
         #: int: Binning in x direction
         self.x_binning = int(binning_string[:idx])
+
         #: int: Binning in y direction
         self.y_binning = int(binning_string[idx + 1 :])
+
+        #: int: Number of pixels in x direction
         self.x_pixels = int(self.x_pixels / self.x_binning)
+
+        #: int: Number of pixels in y direction
         self.y_pixels = int(self.y_pixels / self.y_binning)
-        # should update experiment in controller side
-        # self.configuration['experiment']['CameraParameters']['camera_binning'] = str(
-        # self.x_binning) + 'x' + str(self.y_binning)
         return True
 
     def set_ROI(self, roi_height=3200, roi_width=3200):
         """Change the size of the active region on the camera.
 
         Parameters
         ----------
         roi_height : int
-            Height of active camera region.
+            Height of active camera region. Default is 3200.
         roi_width : int
-            Width of active camera region.
+            Width of active camera region. Default is 3200.
+
+        Returns
+        -------
+        result: bool
+            True if successful, False otherwise.
         """
+
         # Get the Maximum Number of Pixels from the Configuration File
         camera_height = self.camera_parameters["y_pixels"]
         camera_width = self.camera_parameters["x_pixels"]
 
         if (
             roi_height > camera_height
             or roi_width > camera_width
+            or roi_height < 1
+            or roi_width < 1
             or roi_height % 2 == 1
             or roi_width % 2 == 1
         ):
             logger.debug(f"can't set roi to {roi_width} and {roi_height}")
             return False
 
         # Calculate Location of Image Edges
@@ -443,164 +409,112 @@
 
         if roi_top % 2 != 0 or roi_bottom % 2 == 0:
             logger.debug(f"can't set ROI to {roi_width} and {roi_height}")
             return False
 
         # Set ROI
         self.camera_controller.set_roi(roi_left, roi_top, roi_width, roi_height)
-        # self.x_pixels, self.y_pixels = self.camera_controller.shape()
-
         logger.info(f"Photometrics ROI shape, {self.camera_controller.shape()}")
-
         return self.x_pixels == roi_width and self.y_pixels == roi_height
 
     def initialize_image_series(self, data_buffer=None, number_of_frames=100):
         """Initialize Photometrics image series. This is for starting stacks etc.
 
         Parameters
         ----------
-        data_buffer : int
-            Size of the data to buffer.  Default is None.
+        data_buffer :
+            List of SharedNDArrays of shape=(self.img_height,
+            self.img_width) and dtype="uint16"
+            Default is None.
         number_of_frames : int
             Number of frames.  Default is 100.
         """
-        print(self._exposuretime)
-        self.camera_controller.readout_port = 0
-        self.camera_controller.speed_table_index = 0
-        self.camera_controller.gain = 1
-        self._exposuretime = 20
 
-        # set following parameters if in programmable scan mode (ASLM)
+        # set camera parameters depending on acquisition mode
         self._scanmode = self.camera_controller.prog_scan_mode
         if self._scanmode == 1:
+            # Programmable scan mode (ASLM)
             self.camera_controller.exp_mode = "Edge Trigger"
             self.camera_controller.prog_scan_line_delay = self._scandelay
             self.camera_controller.exp_out_mode = 4
-            print("camera ready to acquire programmable scan mode")
-
+            print(
+                "camera ready to acquire programmable scan mode "
+                "with scandelay {}".format(self._scandelay)
+            )
         else:
+            # Normal mode
             self.camera_controller.exp_out_mode = "Any Row"
             self.camera_controller.exp_mode = "Edge Trigger"
             print("camera ready to acquire static light sheet mode")
 
-        # prepare buffer pointer array
-        # ptr_array = c_void_p * number_of_frames
-        # data_ptr = ptr_array()
-        # for i in range(number_of_frames):
-        #     np_array = data_buffer[i]
-        #     data_ptr[i] = np_array.ctypes.data
-
+        # Prepare for buffered acquisition
+        #: int: Number of frames
         self._numberofframes = number_of_frames
+
+        #: obj: Data Buffer
         self._data_buffer = data_buffer
+
+        #: int: Number of frames received
         self._frames_received = 0
+
+        #: list: Frame IDs
         self._frame_ids = []
 
+        #: bool: Acquisition flag
         self.is_acquiring = True
-        self.camera_controller.start_live(exp_time=self._exposuretime)
-
-    def _receive_images(self):
 
-        # wait_for_camera = True
+        # Start camera - call it here as there are some error messages showing up
+        # a call to the camera here.
+        # Start live will be called a second time from the exposure time function,
+        # with the current exposure time.
+        self.camera_controller.start_live()
 
-        # while self.is_acquiring == True:
+    def _receive_images(self):
+        """
+        Update image in the data buffer if the Photometrics camera acquired a new
+        image and return frame ids.
 
-        # time.sleep(0.002)
+        Returns
+        -------
+        frame : numpy.ndarray
+            Frame ids from Photometrics camera that point to newly acquired data in
+            data buffer
+        """
+        # Try to grap the next frame from camera
         try:
             frame, fps, frame_count = self.camera_controller.poll_frame(
                 timeout_ms=10000
             )
-            # self._frame_ids.append(self._frames_received)
-
             self._data_buffer[self._frames_received][:, :] = np.copy(
                 frame["pixel_data"][:]
             )
+            # Delete copied frame for memory management
             frame = None
             del frame
             self._frames_received += 1
             if self._frames_received >= self._numberofframes:
                 self._frames_received = 0
             return [self._frames_received - 1]
         except Exception as e:
             print(str(e))
-        #     break
-
-        # print("excited loop")
 
         return []
 
-    # def _receive_imagesV1(self):
-    #
-    #     frame_ids = []
-    #     wait_for_camera=True
-    #     print("wait to receive frames")
-    #
-    #
-    #     while wait_for_camera ==True:
-    #         time.sleep(0.002)
-    #         print(self.camera_controller.check_frame_status())
-    #         if self.camera_controller.check_frame_status()=='FRAME_AVAILABLE':
-    #             # framesReceived < number_of_frames:
-    #
-    #             if self.is_acquiring==False: #exit if acquisition is done
-    #                 break
-    #
-    #             print(self._frames_received)
-    #             try:
-    #                 frame, fps, frame_count = self.camera_controller.poll_frame(
-    #                 timeout_ms=10000)
-    #                 print("received frame")
-    #                 frame_ids.append(self._frames_received)
-    #                 self.data_buffer[self._frames_received][:,:] = np.copy(frame[
-    #                 'pixel_data'][:])
-    #                 frame = None
-    #                 del frame
-    #                 self._frames_received += 1
-    #                 if self._frames_received >= self._numberofframes:
-    #                     self._frames_received = 0
-    #
-    #
-    #
-    #
-    #             except Exception as e:
-    #                 print(str(e))
-    #                 break
-    #     return frame_ids
+    def get_new_frame(self):
+        """
+        Call update function for data buffer and get frame ids from Photometrics camera.
+
+        Returns
+        -------
+        frame : numpy.ndarray
+            Frame ids from Photometrics camera that point to newly acquired
+            data in data buffer
+        """
+        return self._receive_images()
 
     def close_image_series(self):
-        """Close image series.
+        """Close Photometrics image series.
 
         Stops the acquisition and sets is_acquiring flag to False.
         """
-        print("Calling finish")
         self.camera_controller.finish()
         self.is_acquiring = False
-
-    def get_new_frame(self):
-        """Get frame ids from Photometrics camera."""
-        # return self.camera_controller.get_frame(exp_time=self._exposuretime)
-        # self.camera_controller.start_live(exp_time=self._exposuretime)
-
-        # self._receive_images()
-        # return self._frame_ids[]
-
-        return self._receive_images()
-
-    def get_minimum_waiting_time(self):
-        """Get minimum waiting time for HamamatsuOrca.
-
-        This function get timing information from the camera device
-        cyclic_trigger_period, minimum_trigger_blank, minimum_trigger_interval
-        'cyclic_trigger_period' of current device is 0
-        according to the document, trigger_blank should be bigger than trigger_interval.
-        """
-        # # cyclic_trigger = self.camera_controller.get_property_value(
-        # 'cyclic_trigger_period')
-        # trigger_blank = self.camera_controller.get_property_value(
-        # 'minimum_trigger_blank')
-        # # trigger_interval = self.camera_controller.get_property_value(
-        # 'minimum_trigger_interval')
-        # return trigger_blank
-        # readout_time = (self.y_pixels + 1) * Camera_parameters.highres_
-        # line_digitization_time  # +1 for the reset time at the first row
-        # before the start
-        # minimal_trigger_timeinterval = self._exposuretime + readout_time
-        return 2
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/camera/camera_synthetic.py` & `navigate_micro-0.0.6/src/navigate/model/devices/camera/camera_synthetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,24 +303,14 @@
             Height of active camera region.
         roi_width : int
             Width of active camera region.
         """
         self.x_pixels = roi_width
         self.y_pixels = roi_height
 
-    def get_minimum_waiting_time(self):
-        """Get minimum waiting time for SyntheticCamera.
-
-        Returns
-        -------
-        float
-            Minimum waiting time.
-        """
-        return 0.01
-
     def calculate_readout_time(self):
         """Calculate duration of time needed to readout an image. Calculates the readout
         time and maximum frame rate according to the camera configuration settings.
 
         Returns
         -------
         readout_time : float
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_base.py` & `navigate_micro-0.0.6/src/navigate/model/devices/daq/daq_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_ni.py` & `navigate_micro-0.0.6/src/navigate/model/devices/daq/daq_ni.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/daq/daq_synthetic.py` & `navigate_micro-0.0.6/src/navigate/model/devices/daq/daq_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_asi.py` & `navigate_micro-0.0.6/src/navigate/model/devices/filter_wheel/filter_wheel_asi.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_base.py` & `navigate_micro-0.0.6/src/navigate/model/devices/filter_wheel/filter_wheel_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_sutter.py` & `navigate_micro-0.0.6/src/navigate/model/devices/filter_wheel/filter_wheel_sutter.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/filter_wheel/filter_wheel_synthetic.py` & `navigate_micro-0.0.6/src/navigate/model/devices/filter_wheel/filter_wheel_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_base.py` & `navigate_micro-0.0.6/src/navigate/model/devices/galvo/galvo_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,17 +77,15 @@
 
         #: int: Sample rate.
         self.sample_rate = configuration["configuration"]["microscopes"][
             microscope_name
         ]["daq"]["sample_rate"]
 
         #: float: Sweep time.
-        self.sweep_time = configuration["configuration"]["microscopes"][
-            microscope_name
-        ]["daq"]["sweep_time"]
+        self.sweep_time = 0
 
         #: float: Camera delay
         self.camera_delay = configuration["configuration"]["microscopes"][
             microscope_name
         ]["camera"]["delay"] / 1000
 
         #: float: Galvo max voltage.
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_ni.py` & `navigate_micro-0.0.6/src/navigate/model/devices/galvo/galvo_ni.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/galvo/galvo_synthetic.py` & `navigate_micro-0.0.6/src/navigate/model/devices/galvo/galvo_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_base.py` & `navigate_micro-0.0.6/src/navigate/model/devices/lasers/laser_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_ni.py` & `navigate_micro-0.0.6/src/navigate/model/devices/lasers/laser_ni.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/lasers/laser_synthetic.py` & `navigate_micro-0.0.6/src/navigate/model/devices/lasers/laser_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_base.py` & `navigate_micro-0.0.6/src/navigate/model/devices/mirrors/mirror_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_imop.py` & `navigate_micro-0.0.6/src/navigate/model/devices/mirrors/mirror_imop.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/mirrors/mirror_synthetic.py` & `navigate_micro-0.0.6/src/navigate/model/devices/mirrors/mirror_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/objectives.py` & `navigate_micro-0.0.6/src/navigate/model/devices/objectives.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_base.py` & `navigate_micro-0.0.6/src/navigate/model/devices/remote_focus/remote_focus_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,15 @@
 
         #: int: Sample rate of the DAQ.
         self.sample_rate = configuration["configuration"]["microscopes"][
             microscope_name
         ]["daq"]["sample_rate"]
 
         #: float: Sweep time of the DAQ.
-        self.sweep_time = configuration["configuration"]["microscopes"][
-            microscope_name
-        ]["daq"]["sweep_time"]
+        self.sweep_time = 0
 
         #: float: Camera delay percent.
         self.camera_delay = configuration["configuration"]["microscopes"][
             microscope_name
         ]["camera"]["delay"] / 1000
 
         # Waveform Parameters
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_equipment_solutions.py` & `navigate_micro-0.0.6/src/navigate/model/devices/remote_focus/remote_focus_equipment_solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             Configuration dictionary
         """
         super().__init__(microscope_name, device_connection, configuration)
 
         #: str: Name of the RS232 communication port.
         self.comport = configuration["configuration"]["microscopes"][microscope_name][
             "remote_focus_device"
-        ]["hardware"].get("comport", "COM1")
+        ]["hardware"].get("port", "COM1")
 
         #: int: Baud rate of the RS232 communication port.
         self.baud_rate = 115200
 
         #: int: Number of data bits.
         self.byte_size = serial.EIGHTBITS
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_ni.py` & `navigate_micro-0.0.6/src/navigate/model/devices/remote_focus/remote_focus_ni.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/remote_focus/remote_focus_synthetic.py` & `navigate_micro-0.0.6/src/navigate/model/devices/remote_focus/remote_focus_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_base.py` & `navigate_micro-0.0.6/src/navigate/model/devices/shutter/laser_shutter_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_synthetic.py` & `navigate_micro-0.0.6/src/navigate/model/devices/shutter/laser_shutter_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/shutter/laser_shutter_ttl.py` & `navigate_micro-0.0.6/src/navigate/model/devices/shutter/laser_shutter_ttl.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_asi.py` & `navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_asi.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_base.py` & `navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_galvo.py` & `navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_galvo.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,17 +123,20 @@
 
         #: str: Trigger source for the DAQ.
         self.trigger_source = configuration["configuration"]["microscopes"][
             microscope_name
         ]["daq"]["trigger_source"]
 
         #: float: Percent of the camera delay.
-        self.camera_delay = configuration["configuration"]["microscopes"][
-            microscope_name
-        ]["camera"]["delay"] / 1000
+        self.camera_delay = (
+            configuration["configuration"]["microscopes"][microscope_name]["camera"][
+                "delay"
+            ]
+            / 1000
+        )
 
         #: float: Sample rate of the DAQ.
         self.sample_rate = self.configuration["configuration"]["microscopes"][
             self.microscope_name
         ]["daq"]["sample_rate"]
 
         #: dict: Dictionary of exposure times for each channel.
@@ -156,15 +159,15 @@
 
         Returns
         -------
         dict
             Dictionary of positions for each axis.
         """
         return self.get_position_dict()
-    
+
     def update_waveform(self, waveform_dict):
         """Update the waveform for the stage.
 
         Parameters
         ----------
         waveform_dict : dict
             Dictionary of waveforms for each channel
@@ -172,15 +175,15 @@
         Returns
         -------
         result : bool
             success or failed
         """
         self.switch_mode("waveform")
         microscope_state = self.configuration["experiment"]["MicroscopeState"]
-        
+
         for channel_key in microscope_state["channels"].keys():
             # channel includes 'is_selected', 'laser', 'filter', 'camera_exposure'...
             channel = microscope_state["channels"][channel_key]
 
             # Only proceed if it is enabled in the GUI
             if channel["is_selected"] is True:
 
@@ -232,15 +235,19 @@
 
         volts = eval(self.volts_per_micron, {"x": axis_abs})
         if volts > self.galvo_max_voltage:
             volts = self.galvo_max_voltage
         if volts < self.galvo_min_voltage:
             volts = self.galvo_min_voltage
 
-        self.ao_task.write(volts, auto_start=True)
+        try:
+            self.ao_task.write(volts, auto_start=True)
+        except Exception as e:
+            logger.debug(f"Error moving {axis} to {axis_abs} volts: {volts}")
+            logger.exception(e)
         # Stage Settle Duration in Milliseconds
         if (
             wait_until_done
             and (self.distance_threshold is not None)
             and (delta_position >= self.distance_threshold)
         ):
             time.sleep(self.stage_settle_duration)
@@ -291,12 +298,17 @@
         """
         self.exposure_times = exposure_times
         self.sweep_times = sweep_times
         if mode == "normal":
             if self.ao_task is None:
                 self.ao_task = nidaqmx.Task()
                 self.ao_task.ao_channels.add_ao_voltage_chan(self.axes_channels[0])
-            self.move_axis_absolute(self.axes[0], float(self.configuration["experiment"]["StageParameters"][self.axes[0]]))
+            self.move_axis_absolute(
+                self.axes[0],
+                float(
+                    self.configuration["experiment"]["StageParameters"][self.axes[0]]
+                ),
+            )
         elif self.ao_task:
             self.ao_task.stop()
             self.ao_task.close()
-            self.ao_task = None
+            self.ao_task = None
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_mcl.py` & `navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_mcl.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_pi.py` & `navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_pi.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_sutter.py` & `navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_sutter.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_synthetic.py` & `navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/stages/stage_tl_kcube_inertial.py` & `navigate_micro-0.0.6/src/navigate/model/devices/stages/stage_tl_kcube_inertial.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_base.py` & `navigate_micro-0.0.6/src/navigate/model/devices/zoom/zoom_base.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_dynamixel.py` & `navigate_micro-0.0.6/src/navigate/model/devices/zoom/zoom_dynamixel.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/devices/zoom/zoom_synthetic.py` & `navigate_micro-0.0.6/src/navigate/model/devices/zoom/zoom_synthetic.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/features/adaptive_optics.py` & `navigate_micro-0.0.6/src/navigate/model/features/adaptive_optics.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/features/auto_tile_scan.py` & `navigate_micro-0.0.6/src/navigate/model/features/auto_tile_scan.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/features/autofocus.py` & `navigate_micro-0.0.6/src/navigate/model/features/autofocus.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/features/common_features.py` & `navigate_micro-0.0.6/src/navigate/model/features/common_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -591,26 +591,26 @@
             A boolean value indicating whether to continue the position control process.
         """
         self.model.logger.debug(
             f"multi-position current idx: {self.current_idx}, {self.position_count}"
         )
         if self.current_idx >= self.position_count:
             return False
-        pos_dict = self.multiposition_table[self.current_idx]
+        pos_dict = dict(zip(["x", "y", "z", "theta", "f"], self.multiposition_table[self.current_idx]))
         # pause data thread if necessary
         if self.current_idx == 0:
             temp = self.model.get_stage_position()
             pre_stage_pos = dict(
                 map(
                     lambda k: (k, temp[f"{k}_pos"]),
                     ["x", "y", "z", "f", "theta"],
                 )
             )
         else:
-            pre_stage_pos = self.multiposition_table[self.current_idx - 1]
+            pre_stage_pos = dict(zip(["x", "y", "z", "theta", "f"], self.multiposition_table[self.current_idx - 1]))
         delta_x = abs(pos_dict["x"] - pre_stage_pos["x"])
         delta_y = abs(pos_dict["y"] - pre_stage_pos["y"])
         delta_z = abs(pos_dict["z"] - pre_stage_pos["z"])
         delta_f = abs(pos_dict["f"] - pre_stage_pos["f"])
         should_pause_data_thread = any(
             distance > self.stage_distance_threshold
             for distance in [delta_x, delta_y, delta_z, delta_f]
@@ -868,52 +868,54 @@
         pos_dict = self.model.get_stage_position()
         self.model.logger.debug(f"**** ZStack get stage position: {pos_dict}")
         #: float: The z position of the channel being acquired in the z-stack
         self.restore_z = pos_dict["z_pos"]
         #: float: The f position of the channel being acquired in the z-stack
         self.restore_f = pos_dict["f_pos"]
 
+        # position: x, y, z, theta, f
         if bool(microscope_state["is_multiposition"]):
             self.positions = self.model.configuration["experiment"]["MultiPositions"]
         else:
             self.positions = [
-                {
-                    "x": float(pos_dict["x_pos"]),
-                    "y": float(pos_dict["y_pos"]),
-                    "z": float(
+                [
+                    float(pos_dict["x_pos"]),
+                    float(pos_dict["y_pos"]),
+                    float(
                         microscope_state.get(
                             "stack_z_origin",
                             pos_dict["z_pos"],
                         )
                         if not self.get_origin
                         else pos_dict["z_pos"]
                     ),
-                    "theta": float(pos_dict["theta_pos"]),
-                    "f": float(
+                    float(pos_dict["theta_pos"]),
+                    float(
                         microscope_state.get(
                             "stack_focus_origin",
                             pos_dict["f_pos"],
                         )
                         if not self.get_origin
                         else pos_dict["f_pos"]
                     ),
-                }
+                ]
             ]
 
         # Setup next channel down here, to ensure defocus isn't merged into
         # restore f_pos, positions
         self.model.active_microscope.central_focus = None
         self.model.active_microscope.current_channel = 0
         self.model.active_microscope.prepare_next_channel()
 
         self.model.logger.debug(
             f"*** ZStack pre_signal_func: {self.positions}, {self.start_focus}, "
             f"{self.start_z_position}"
         )
         self.current_position_idx = 0
+        self.current_position = dict(zip(["x", "y", "z", "theta", "f"], self.positions[0]))
         self.z_position_moved_time = 0
         self.need_to_move_new_position = True
         self.need_to_move_z_position = True
         #: bool: Flag to determine whether to pause the data thread.
         self.should_pause_data_thread = False
         # TODO: distance > 1000 should not be hardcoded and somehow related to
         #  different kinds of stage devices.
@@ -937,59 +939,63 @@
         bool
             A boolean value indicating whether to continue the z-stack acquisition
             process.
         """
         if self.model.stop_acquisition:
             return False
         data_thread_is_paused = False
+        
         # move stage X, Y, Theta
         if self.need_to_move_new_position:
             self.need_to_move_new_position = False
 
+            self.pre_position = self.current_position
+            self.current_position = dict(zip(["x", "y", "z", "theta", "f"], self.positions[self.current_position_idx]))
+
             # calculate first z, f position
             self.current_z_position = (
-                self.start_z_position + self.positions[self.current_position_idx]["z"]
+                self.start_z_position + self.current_position["z"]
             )
             self.current_focus_position = (
-                self.start_focus + self.positions[self.current_position_idx]["f"]
+                self.start_focus + self.current_position["f"]
             )
             if self.defocus is not None:
                 self.current_focus_position += self.defocus[
                     self.current_channel_in_list
                 ]
 
             # calculate delta_x, delta_y
             # TODO: Here.
             pos_dict = dict(
                 map(
                     lambda ax: (
                         f"{ax}_abs",
-                        self.positions[self.current_position_idx][ax],
+                        self.current_position[ax],
                     ),
                     ["x", "y", "theta"],
                 )
             )
 
             if self.current_position_idx > 0:
                 delta_x = (
-                    self.positions[self.current_position_idx]["x"]
-                    - self.positions[self.current_position_idx - 1]["x"]
+                    self.current_position["x"]
+                    - self.pre_position["x"]
                 )
                 delta_y = (
-                    self.positions[self.current_position_idx]["y"]
-                    - self.positions[self.current_position_idx - 1]["y"]
+                    self.current_position["y"]
+                    - self.pre_position["y"]
                 )
                 delta_z = (
-                    self.positions[self.current_position_idx]["z"]
-                    - self.positions[self.current_position_idx - 1]["z"]
+                    self.current_position["z"]
+                    - self.pre_position["z"]
                     + self.z_stack_distance
                 )
                 delta_f = (
-                    self.positions[self.current_position_idx]["f"]
-                    - self.positions[self.current_position_idx - 1]["f"]
+                    self.current_position["f"]
+                    - self.pre_position["f"]
                     + self.f_stack_distance
                 )
             else:
                 delta_x = 0
                 delta_y = 0
                 delta_z = 0
                 delta_f = 0
@@ -1072,18 +1078,18 @@
             self.z_position_moved_time += 1
 
         # decide whether to move X,Y,Theta
         if self.z_position_moved_time >= self.number_z_steps:
             self.z_position_moved_time = 0
             # calculate first z, f position
             self.current_z_position = (
-                self.start_z_position + self.positions[self.current_position_idx]["z"]
+                self.start_z_position + self.current_position["z"]
             )
             self.current_focus_position = (
-                self.start_focus + self.positions[self.current_position_idx]["f"]
+                self.start_focus + self.current_position["f"]
             )
             if (
                 self.z_stack_distance > self.stage_distance_threshold
                 or self.f_stack_distance > self.stage_distance_threshold
             ):
                 self.should_pause_data_thread = True
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/features/cva_conpro.py` & `navigate_micro-0.0.6/src/navigate/model/features/cva_conpro.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/features/feature_container.py` & `navigate_micro-0.0.6/src/navigate/model/features/feature_container.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/features/feature_related_functions.py` & `navigate_micro-0.0.6/src/navigate/model/features/feature_related_functions.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/features/image_writer.py` & `navigate_micro-0.0.6/src/navigate/model/features/image_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,23 @@
 p = __name__.split(".")[1]
 logger = logging.getLogger(p)
 
 
 class ImageWriter:
     """Class for saving acquired data to disk."""
 
-    def __init__(self, model, data_buffer=None, sub_dir="", image_name=None, saving_flags=None, saving_config={}):
+    def __init__(
+        self,
+        model,
+        data_buffer=None,
+        sub_dir="",
+        image_name=None,
+        saving_flags=None,
+        saving_config={},
+    ):
         """Class for saving acquired data to disk.
 
         Parameters
         ----------
         model : navigate.model.model.Model
             Navigate Model class for controlling hardware/acquisition.
         data_buffer: [SharedNDArray]
@@ -261,18 +269,22 @@
                             + ".tif"
                         )
                         imsave(
                             os.path.join(self.mip_directory, mip_name),
                             self.mip[c_save_idx, :, :],
                         )
             except Exception as e:
+                from traceback import format_exc
+
                 # Close the image, stop the acquisition, log error, and notify user.
                 self.close()
                 self.model.stop_acquisition = True
-                self.model.event_queue.put(("warning", "Insufficient Disk Space. "))
+                self.model.event_queue.put(
+                    ("warning", f"Error - ImageWriter: {format_exc()}")
+                )
                 logger.debug(f"Error - ImageWriter: {e}")
                 return
 
     def generate_image_name(self, current_channel, ext=".tif"):
         """Generates a string for the filename, e.g., CH00_000000.tif.
 
         Parameters
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/features/remove_empty_tiles.py` & `navigate_micro-0.0.6/src/navigate/model/features/remove_empty_tiles.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/features/restful_features.py` & `navigate_micro-0.0.6/src/navigate/model/features/restful_features.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 class IlastikSegmentation:
     """Ilastik segmentation class.
 
     Uses Ilastik REST API to perform segmentation in a separate process.
     """
 
-    def __init__(self, model):
+    def __init__(self, model, microscope_name="Nanoscale", zoom_value="N/A"):
         """Initialize Ilastik segmentation class.
 
         Parameters
         ----------
         model : Model
             Model object
         """
@@ -101,14 +101,20 @@
 
         #: int: number of pieces
         self.pieces_num = 1
 
         #: int: size of pieces
         self.pieces_size = 1
 
+        #: str: high resolution microscope name
+        self.high_res_microscope_name = microscope_name
+
+        #: str: zoom value
+        self.high_res_zoom_value = zoom_value
+
         #: dict: configuration table
         self.config_table = {"data": {"init": self.init_func, "main": self.data_func}}
 
     def init_func(self, *args):
         """Initialize Ilastik segmentation.
 
         Parameters
@@ -160,33 +166,34 @@
                 if self.model.mark_ilastik_position:
                     self.mark_position(segmentation_mask[segmentation_id])
         else:
             print("There is something wrong!")
 
     def update_setting(self):
         """Update Ilastik segmentation settings."""
+        try:
+            pixel_size = float(
+                self.model.configuration["configuration"]["microscopes"][
+                    self.high_res_microscope_name
+                ]["zoom"]["pixel_size"][self.high_res_zoom_value]
+            )
+        except (KeyError, AttributeError):
+            return
+        
         self.resolution = self.model.configuration["experiment"]["MicroscopeState"][
             "microscope_name"
         ]
         self.zoom = self.model.configuration["experiment"]["MicroscopeState"]["zoom"]
         # Get current mag
         current_microscope_name = self.resolution
         curr_pixel_size = float(
             self.model.configuration["configuration"]["microscopes"][
                 current_microscope_name
             ]["zoom"]["pixel_size"][self.zoom]
         )
-        # target resolution is 'high'
-        # TODO:
-        high_res_microscope_name = "Nanoscale"
-        pixel_size = float(
-            self.model.configuration["configuration"]["microscopes"][
-                high_res_microscope_name
-            ]["zoom"]["pixel_size"]["N/A"]
-        )
         # calculate pieces
         self.pieces_num = int(curr_pixel_size / pixel_size)
         self.pieces_size = ceil(
             float(
                 self.model.configuration["experiment"]["CameraParameters"]["x_pixels"]
             )
             / self.pieces_num
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/features/volume_search.py` & `navigate_micro-0.0.6/src/navigate/model/features/volume_search.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/metadata_sources/bdv_metadata.py` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/display_notebook.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) 2021-2022  The University of Texas Southwestern Medical Center.
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
-# modification, are permitted for academic and research use only (subject to the
-# limitations in the disclaimer below) provided that the following conditions are met:
+# modification, are permitted for academic and research use only
+# (subject to the limitations in the disclaimer below)
+# provided that the following conditions are met:
 
 #      * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 
 #      * Redistributions in binary form must reproduce the above copyright
 #      notice, this list of conditions and the following disclaimer in the
 #      documentation and/or other materials provided with the distribution.
@@ -25,510 +26,555 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 # IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-#  Standard Imports
-import os
-from typing import Optional, Union
-import xml.etree.ElementTree as ET
+# Standard Library Imports
+import tkinter as tk
+from tkinter import ttk, Grid
+import logging
 
 # Third Party Imports
-import numpy as np
-import numpy.typing as npt
+from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
+from matplotlib.figure import Figure
 
-# Local imports
-from .metadata import XMLMetadata
-from navigate.tools.linear_algebra import affine_rotation, affine_shear
-
-
-class BigDataViewerMetadata(XMLMetadata):
-    """Metadata for BigDataViewer files.
-
-    Note
-    ----
-        XML spec in section 2.3 of https://arxiv.org/abs/1412.0488.
-
-    """
-
-    def __init__(self) -> None:
-        """Initialize the BigDataViewer metadata object."""
-        super().__init__()
-
-        # Affine Transform Parameters
-        #: bool: Shear the data.
-        self.shear_data = False
-        #: str: Dimension to shear the data.
-        self.shear_dimension = "YZ"
-        #: float: Angle in degrees to shear the data.
-        self.shear_angle = 0
-        #: npt.NDArray: Shear transform matrix.
-        self.shear_transform = np.eye(3, 4)
-
-        # Rotation Transform Parameters
-        #: bool: Rotate the data.
-        self.rotate_data = False
-        #: float: Angle in degrees to rotate the data in X.
-        self.rotate_angle_x = 0
-        #: float: Angle in degrees to rotate the data in Y.
-        self.rotate_angle_y = 0
-        #: float: Angle in degrees to rotate the data in Z.
-        self.rotate_angle_z = 0
-        #: npt.NDArray: Rotation transform matrix.
-        self.rotate_transform = np.eye(3, 4)
+# Local Imports
+from navigate.view.custom_widgets.DockableNotebook import DockableNotebook
+from navigate.view.custom_widgets.LabelInputWidgetFactory import LabelInput
+
+
+# Logger Setup
+p = __name__.split(".")[1]
+logger = logging.getLogger(p)
+
+
+class CameraNotebook(DockableNotebook):
+    """This class is the notebook that holds the camera view and waveform settings
+    tabs."""
+
+    def __init__(self, frame_top_right, *args, **kwargs):
+        """Init function for the CameraNotebook class.
 
-    def get_affine_parameters(self, configuration):
-        """Get the affine transform parameters from the configuration file.
 
         Parameters
         ----------
-        configuration : dict
-            Configuration dictionary.
+        frame_top_right : tk.Frame
+            The frame that will hold the notebook.
+        *args : tuple
+            Variable length argument list.
+        **kwargs : dict
+            Arbitrary keyword arguments.
         """
-        bdv_configuration = configuration["configuration"].get("BDVParameters")
+        # Init notebook
+        DockableNotebook.__init__(self, frame_top_right, *args, **kwargs)
 
-        if bdv_configuration is not None:
+        # Putting notebook 2 into top right frame
+        self.grid(row=0, column=0)
 
-            # Shear Parameters
-            self.shear_data = bdv_configuration["shear"].get("shear_data", False)
-            self.shear_dimension = (
-                bdv_configuration["shear"].get("shear_dimension", "YZ").upper()
-            )
-            self.shear_angle = bdv_configuration["shear"].get("shear_angle", 0)
+        #: CameraTab: The camera tab.
+        self.camera_tab = CameraTab(self)
+
+        #: WaveformTab: The waveform settings tab.
+        self.waveform_tab = WaveformTab(self)
 
-            # Rotate Parameters
-            self.rotate_data = bdv_configuration["rotate"].get("rotate_data", False)
-            self.rotate_angle_x = bdv_configuration["rotate"].get("X", 0)
-            self.rotate_angle_y = bdv_configuration["rotate"].get("Y", 0)
-            self.rotate_angle_z = bdv_configuration["rotate"].get("Z", 0)
-
-    def bdv_xml_dict(
-        self, file_name: Union[str, list, None], views: list, **kw
-    ) -> dict:
-        """Create a BigDataViewer XML dictionary from a list of views.
+        # Tab list
+        tab_list = [self.camera_tab, self.waveform_tab]
+        self.set_tablist(tab_list)
+
+        # Adding tabs to self notebook
+        self.add(self.camera_tab, text="Camera View", sticky=tk.NSEW)
+        self.add(self.waveform_tab, text="Waveform Settings", sticky=tk.NSEW)
+
+
+class CameraTab(tk.Frame):
+    """CameraTab class."""
+
+    def __init__(self, cam_wave, *args, **kwargs):
+        """Initialize the CameraTab class.
 
         Parameters
         ----------
-        file_name : str
-            The file name of the file to be written.
-        views : list
-            A list of dictionaries containing metadata for each view.
-        **kw
-            Additional keyword arguments.
+        cam_wave : tk.Frame
+            The frame that will hold the camera tab.
+        *args : tuple
+            Variable length argument list.
+        **kwargs : dict
+            Arbitrary keyword arguments.
+        """
+        #  Init Frame
+        tk.Frame.__init__(self, cam_wave, *args, **kwargs)
 
-        Returns
-        -------
-        dict
-            A dictionary containing the XML metadata.
+        #: int: The index of the tab.
+        self.index = 0
 
-        """
-        # Header
-        bdv_dict = {"version": 0.2}
+        # Formatting
+        tk.Grid.columnconfigure(self, "all", weight=1)
+        tk.Grid.rowconfigure(self, "all", weight=1)
 
-        # File path
-        bdv_dict["BasePath"] = {"type": "relative", "text": "."}
-        bdv_dict["SequenceDescription"] = {}
-
-        ext = os.path.basename(file_name).split(".")[-1]
-        if ext == "h5":
-            """
-            <ImageLoader format="bdv.hdf5">
-                <hdf5 type="relative">dataset.h5</hdf5>
-            </ImageLoader>
-            """
-            bdv_dict["SequenceDescription"]["ImageLoader"] = {"format": "bdv.hdf5"}
-            bdv_dict["SequenceDescription"]["ImageLoader"]["hdf5"] = {
-                "type": "relative",
-                "text": file_name,
-            }
-
-        elif ext == "tiff" or ext == "tif":
-            """
-            Need to iterate through the time points, etc.
-            <ImageLoader format="spimreconstruction.filelist">
-                <imglib2container>ArrayImgFactory</imglib2container>
-                <ZGrouped>false</ZGrouped>
-                <files>
-                    <FileMapping view_setup="0" timepoint="0" series="0" channel="0">
-                        <file type="relative">1_CH00_000000.tif</file>
-                    </FileMapping>
-                    <FileMapping view_setup="1" timepoint="0" series="0" channel="0">
-                        <file type="relative">1_CH01_000000.tif</file>
-                    </FileMapping>
-                </files>
-            </ImageLoader>
-            """
-            pass
-
-        elif ext == "n5":
-            """
-            <ImageLoader format="bdv.n5" version="1.0">
-                <n5 type="relative">dataset.n5</n5>
-            </ImageLoader>
-            """
-            bdv_dict["SequenceDescription"]["ImageLoader"] = {"format": "bdv.n5"}
-            bdv_dict["SequenceDescription"]["ImageLoader"]["n5"] = {
-                "type": "relative",
-                "text": file_name,
-            }
-
-        # Calculate shear and rotation transforms
-        self.bdv_shear_transform()
-        self.bdv_rotate_transform()
-
-        # Populate ViewSetups
-        bdv_dict["SequenceDescription"]["ViewSetups"] = {}
-        bdv_dict["SequenceDescription"]["ViewSetups"]["ViewSetup"] = []
-        # Attributes are necessary for BigStitcher
-        bdv_dict["SequenceDescription"]["ViewSetups"]["Attributes"] = [
-            {
-                "name": "illumination",
-                "Illumination": {"id": {"text": 0}, "name": {"text": 0}},
-            },
-            {"name": "channel", "Channel": []},
-            {"name": "tile", "Tile": []},
-            {"name": "angle", "Angle": {"id": {"text": 0}, "name": {"text": 0}}},
-        ]
-        # The actual loop that populates ViewSetup
-        view_id = 0
-        for c in range(self.shape_c):
-            # We also take care of the Channel attributes here
-            ch = {"id": {"text": str(c)}, "name": {"text": str(c)}}
-            bdv_dict["SequenceDescription"]["ViewSetups"]["Attributes"][1][
-                "Channel"
-            ].append(ch)
-            for p in range(self.positions):
-                d = {"id": {"text": view_id}, "name": {"text": view_id}}
-                d["size"] = {"text": f"{self.shape_x} {self.shape_y} {self.shape_z}"}
-                d["voxelSize"] = {"unit": {"text": "um"}}
-                d["voxelSize"]["size"] = {"text": f"{self.dx} {self.dy} {self.dz}"}
-                # These attributes are necessary for BigStitcher
-                d["attributes"] = {
-                    "illumination": {"text": "0"},
-                    "channel": {"text": str(c)},
-                    "tile": {"text": str(p)},
-                    "angle": {"text": "0"},
-                }
-                bdv_dict["SequenceDescription"]["ViewSetups"]["ViewSetup"].append(d)
-                view_id += 1
-        # Finish up the Tile Attributes outside of the channels loop so we have
-        # one per tile
-        for p in range(self.positions):
-            tile = {"id": {"text": str(p)}, "name": {"text": str(p)}}
-            bdv_dict["SequenceDescription"]["ViewSetups"]["Attributes"][2][
-                "Tile"
-            ].append(tile)
-
-        # Time
-        bdv_dict["SequenceDescription"]["Timepoints"] = {"type": "range"}
-        bdv_dict["SequenceDescription"]["Timepoints"]["first"] = {"text": 0}
-        bdv_dict["SequenceDescription"]["Timepoints"]["last"] = {
-            "text": self.shape_t - 1
-        }
-
-        # View registrations
-        bdv_dict["ViewRegistrations"] = {"ViewRegistration": []}
-        for t in range(self.shape_t):
-            for p in range(self.positions):
-                for c in range(self.shape_c):
-                    view_id = c * self.positions + p
-                    mat = np.zeros((3, 4), dtype=float)
-                    for z in range(self.shape_z):
-                        matrix_id = (
-                            z
-                            + self.shape_z * c
-                            + p * self.shape_c * self.shape_z
-                            + t * self.shape_c * self.shape_z * self.positions
-                        )
-
-                        # Construct centroid of volume matrix
-                        # print(matrix_id, views[matrix_id])
-                        try:
-                            mat += (
-                                self.stage_positions_to_affine_matrix(
-                                    **views[matrix_id]
-                                )
-                                / self.shape_z
-                            )
-                        except IndexError:
-                            # We have most likely canceled in the middle of
-                            # an acquisition.
-                            pass
-
-                    view_transforms = [
-                        {
-                            "type": "affine",
-                            "Name": "Translation to Regular Grid",
-                            "affine": {
-                                "text": " ".join([f"{x:.6f}" for x in mat.ravel()])
-                            },
-                        }
-                    ]
-
-                    if self.shear_data:
-                        view_transforms.append(
-                            {
-                                "type": "affine",
-                                "Name": "Shearing Transform",
-                                "affine": {
-                                    "text": " ".join(
-                                        [
-                                            f"{x:.6f}"
-                                            for x in self.shear_transform.ravel()
-                                        ]
-                                    )
-                                },
-                            }
-                        )
-
-                    if self.rotate_data:
-                        view_transforms.append(
-                            {
-                                "type": "affine",
-                                "Name": "Rotation Transform",
-                                "affine": {
-                                    "text": " ".join(
-                                        [
-                                            f"{x:.6f}"
-                                            for x in self.rotate_transform.ravel()
-                                        ]
-                                    )
-                                },
-                            }
-                        )
-
-                    d = dict(timepoint=t, setup=view_id, ViewTransform=view_transforms)
-
-                    bdv_dict["ViewRegistrations"]["ViewRegistration"].append(d)
-
-        return bdv_dict
-
-    def stage_positions_to_affine_matrix(
-        self, x: float, y: float, z: float, theta: float, f: Optional[float] = None
-    ) -> npt.ArrayLike:
-        """Convert stage positions to an affine matrix.
+        #: tk.Frame: The frame that will hold the camera image.
+        self.cam_image = ttk.Frame(self)
+        self.cam_image.grid(row=0, column=0, rowspan=3, sticky=tk.NSEW)
+
+        #: Bool: The popup flag.
+        self.is_popup = False
+
+        #: Bool: The docked flag.
+        self.is_docked = True
+
+        #: int: The width of the canvas.
+        #: int: The height of the canvas.
+        self.canvas_width, self.canvas_height = 512, 512
+
+        #: tk.Canvas: The canvas that will hold the camera image.
+        self.canvas = tk.Canvas(
+            self.cam_image, width=self.canvas_width, height=self.canvas_height
+        )
+        self.canvas.grid(row=0, column=0, sticky=tk.NSEW, padx=5, pady=5)
+
+        #: matplotlib.figure.Figure: The figure that will hold the camera image.
+        self.matplotlib_figure = Figure(figsize=[6, 6], tight_layout=True)
+
+        #: matplotlib.backends.backend_tkagg.FigureCanvasTkAgg: The canvas that will
+        # hold the camera image.
+        self.matplotlib_canvas = FigureCanvasTkAgg(self.matplotlib_figure, self.canvas)
+
+        #: IntensityFrame: The frame that will hold the scale settings/palette color.
+        self.scale_palette = IntensityFrame(self)
+        self.scale_palette.grid(row=0, column=1, sticky=tk.NSEW, padx=5, pady=5)
+
+        #: tk.Scale: The slider that will hold the slice index.
+        self.slider = tk.Scale(
+            self,
+            from_=0,
+            to=200,
+            tickinterval=20,
+            orient=tk.HORIZONTAL,
+            showvalue=0,
+            label="Slice Index",
+        )
+        self.slider.configure(state="disabled")  # 'normal'
+        self.slider.grid(row=3, column=0, sticky=tk.NSEW, padx=5, pady=5)
+
+        #: MetricsFrame: The frame that will hold the camera selection and counts.
+        self.image_metrics = MetricsFrame(self)
+        self.image_metrics.grid(row=1, column=1, sticky=tk.NSEW, padx=5, pady=5)
 
-        Ignore theta, focus for now.
+        #: RenderFrame: The frame that will hold the live display functionality.
+        self.live_frame = RenderFrame(self)
+        self.live_frame.grid(row=2, column=1, sticky=tk.NSEW, padx=5, pady=5)
+
+
+class RenderFrame(ttk.Labelframe):
+    """This class is the frame that holds the live display functionality."""
+
+    def __init__(self, cam_view, *args, **kwargs):
+        """Initialize the RenderFrame class.
 
         Parameters
         ----------
-        x : float
-            The x position of the stage.
-        y : float
-            The y position of the stage.
-        z : float
-            The z position of the stage.
-        theta : float
-            The theta position of the stage.
+        cam_view : tk.Frame
+            The frame that will hold the live display functionality.
+        *args : tuple
+            Variable length argument list.
+        **kwargs : dict
+            Arbitrary keyword arguments.
+        """
+        # Init Frame
+        text_label = "Image Display"
+        ttk.Labelframe.__init__(self, cam_view, text=text_label, *args, **kwargs)
+
+        # Formatting
+        Grid.columnconfigure(self, "all", weight=1)
+        Grid.rowconfigure(self, "all", weight=1)
+
+        #: tk.StringVar: The variable that holds the live display functionality.
+        self.live_var = tk.StringVar()
+
+        #: ttk.Combobox: The combobox that holds the live display functionality.
+        self.live = ttk.Combobox(
+            self, textvariable=self.live_var, state="readonly", width=6
+        )
+        self.live["values"] = (
+            "Live",
+            "XY Slice",
+            "YZ Slice",
+            "ZY Slice",
+            "XY MIP",
+            "YZ MIP",
+            "ZY MIP",
+        )
+        self.live.set("Live")
+        self.live.grid(row=0, column=0)
+        self.live.state = "readonly"
+
+    def get_variables(self):
+        """Function to get the variables.
+
+        The key is the widget name, value is the variable associated.
 
         Returns
         -------
-        npt.ArrayLike
-            An affine matrix.
+        variables : dict
+            The dictionary that holds the variables.
         """
-        arr = np.eye(3, 4)
+        variables = {}
+        for key, widget in self.inputs.items():
+            variables[key] = widget.get()
+        return variables
+
+    def get_widgets(self):
+        """Function to get the widgets.
+
+        The key is the widget name, value is the LabelInput class that has all the data.
 
-        # Set the transform positions
-        xp, yp, zp = x / self.dx, y / self.dy, z / self.dz
+        Returns
+        -------
+        self.inputs : dict
+            The dictionary that holds the widgets.
+        """
+        return self.inputs
 
-        # Allow additional axes (e.g. f) to couple onto existing axes (e.g. z)
-        # if they are both moving along the same physical dimension
-        if self._coupled_axes is not None:
-            for leader, follower in self._coupled_axes.items():
-                if leader.lower() not in "xyz":
-                    print(
-                        f"Unrecognized coupled axis {leader}. "
-                        "Not gonna do anything with this."
-                    )
-                    continue
-                elif leader.lower() == "x":
-                    xp += float(locals()[f"{follower.lower()}"]) / self.dx
-                elif leader.lower() == "y":
-                    yp += float(locals()[f"{follower.lower()}"]) / self.dy
-                elif leader.lower() == "z":
-                    zp += float(locals()[f"{follower.lower()}"]) / self.dz
-
-        # Translation into pixels
-        arr[:, 3] = [yp, xp, zp]
-
-        # Rotation (theta pivots in the xz plane, about the y axis)
-        # sin_theta, cos_theta = np.sin(theta), np.cos(theta)
-        # arr[0,0], arr[2,2] = cos_theta, cos_theta
-        # arr[0,2], arr[2,0] = sin_theta, -sin_theta
 
-        return arr
+class WaveformTab(tk.Frame):
+    """This class is the frame that holds the waveform tab."""
+
+    def __init__(self, cam_wave, *args, **kwargs):
+        """Initialize the WaveformTab class.
+
+        Parameters
+        ----------
+        cam_wave : tk.Frame
+            The frame that will hold the waveform tab.
+        *args : tuple
+            Variable length argument list.
+        **kwargs : dict
+            Arbitrary keyword arguments.
 
-    def affine_matrix_to_stage_positions(self, mat: npt.ArrayLike) -> tuple:
         """
-        Convert affine matrix back into stage positions.
+        # Init Frame
+        tk.Frame.__init__(self, cam_wave, *args, **kwargs)
+
+        #: int: The index of the tab.
+        self.index = 1
+
+        #: bool: The popup flag.
+        self.is_docked = True
+
+        # Formatting
+        tk.Grid.columnconfigure(self, "all", weight=1)
+        tk.Grid.rowconfigure(self, "all", weight=1)
+
+        #: tk.Frame: The frame that will hold the waveform plots.
+        self.waveform_plots = ttk.Frame(self)
+        self.waveform_plots.grid(row=0, column=0, sticky=tk.NSEW)
+
+        #: matplotlib.figure.Figure: The figure that will hold the waveform plots.
+        self.fig = Figure(figsize=(6, 6), dpi=100)
+
+        #: matplotlib.backends.backend_tkagg.FigureCanvasTkAgg: The canvas that will
+        # hold the waveform plots.
+        self.canvas = FigureCanvasTkAgg(self.fig, master=self.waveform_plots)
+        self.canvas.draw()
+
+        #: tk.Frame: The frame that will hold the waveform settings.
+        self.waveform_settings = WaveformSettingsFrame(self)
+        self.waveform_settings.grid(row=1, column=0, sticky=tk.NSEW, padx=5, pady=5)
+
 
-        Ignore theta, focus for now.
+class WaveformSettingsFrame(ttk.Labelframe):
+    """This class is the frame that holds the waveform settings."""
+
+    def __init__(self, wav_view, *args, **kwargs):
+        """Initialize the WaveformSettingsFrame class.
 
         Parameters
         ----------
-        mat : npt.ArrayLike
-            An affine matrix.
+        wav_view : tk.Frame
+            The frame that will hold the waveform settings.
+        *args : tuple
+            Variable length argument list.
+        **kwargs : dict
+            Arbitrary keyword arguments.
+        """
+        # Init Frame
+        text_label = "Settings"
+        ttk.Labelframe.__init__(self, wav_view, text=text_label, *args, **kwargs)
+
+        # Formatting
+        tk.Grid.columnconfigure(self, "all", weight=1)
+        tk.Grid.rowconfigure(self, "all", weight=1)
+
+        #: dict: The dictionary that holds the widgets.
+        self.inputs = {}
+
+        self.inputs["sample_rate"] = LabelInput(
+            parent=self,
+            label="Sample rate",
+            input_class=ttk.Spinbox,
+            input_var=tk.IntVar(),
+            input_args={"from_": 1, "to": 2**16 - 1, "increment": 1, "width": 5},
+        )
+        self.inputs["sample_rate"].grid(row=0, column=0, sticky=tk.NSEW, padx=3, pady=3)
+
+        self.inputs["waveform_template"] = LabelInput(
+            parent=self,
+            label="Waveform Template",
+            input_class=ttk.Combobox,
+            input_var=tk.StringVar(),
+            input_args={"width": 20},
+        )
+        self.inputs["waveform_template"].grid(
+            row=0, column=1, sticky=tk.NSEW, padx=3, pady=3
+        )
+
+    def get_variables(self):
+        """Function to get the variables.
 
         Returns
         -------
-        tuple
-            A tuple of stage positions.
+        variables : dict
+            The dictionary that holds the variables.
         """
-        y, x, z = mat[:, 3] * np.array([self.dy, self.dx, self.dz])
-        theta, f = None, None
+        variables = {}
+        for key, widget in self.inputs.items():
+            variables[key] = widget.get()
+        return variables
 
-        return x, y, z, theta, f
+    def get_widgets(self):
+        """Function to get the widgets.
 
-    def bdv_shear_transform(self):
-        """Calculate the shear transform matrix.
-
-        BDV-specific. Matrix provided is not (4,4), but (3,4).
-        """
-        if self.shear_data:
-            self.shear_transform = affine_shear(
-                dz=self.dz,
-                dx=self.dx,
-                dy=self.dy,
-                dimension=self.shear_dimension,
-                angle=self.shear_angle,
-            )[:3]
-        else:
-            self.shear_transform = np.eye(3, 4)
-
-    def bdv_rotate_transform(self):
-        """Calculate the BDV rotation transform matrix.
-
-        BDV-specific. Matrix provided is not (4,4), but (3,4).
-        """
-        if self.rotate_data:
-            self.rotate_transform = affine_rotation(
-                x=self.rotate_angle_x, y=self.rotate_angle_y, z=self.rotate_angle_z
-            )[:3]
-        else:
-            self.rotate_transform = np.eye(3, 4)
+        Returns
+        -------
+        self.inputs : dict
+            The dictionary that holds the widgets.
+        """
+        return self.inputs
 
-    def parse_xml(self, root: Union[str, ET.Element]) -> tuple:
-        """Parse a BigDataViewer XML file into our metadata format.
+
+class MetricsFrame(ttk.Labelframe):
+    """This class is the frame that holds the image metrics."""
+
+    def __init__(self, cam_view, *args, **kwargs):
+        """Initialize the MetricsFrame class.
 
         Parameters
         ----------
-        root : Union[str, ET.Element]
-            The root of the XML tree.
+        cam_view : tk.Frame
+            The frame that will hold the image metrics.
+        *args : tuple
+            Variable length argument list.
+        **kwargs : dict
+            Arbitrary keyword arguments.
+        """
+        # Init Labelframe
+        text_label = "Image Metrics"
+        ttk.Labelframe.__init__(self, cam_view, text=text_label, *args, **kwargs)
+
+        # Formatting
+        tk.Grid.columnconfigure(self, "all", weight=1)
+        tk.Grid.rowconfigure(self, "all", weight=1)
+
+        # Dictionary for widgets
+        #: dict: The dictionary that holds the widgets.
+        self.inputs = {}
+
+        # Labels and names
+        #: list: The list of labels for the widgets.
+        self.labels = ["Frames to Avg", "Image Max Counts", "Channel"]
+        #: list: The list of names for the widgets.
+        self.names = ["Frames", "Image", "Channel"]
+
+        # Loop for widgets
+        for i in range(len(self.labels)):
+            if i == 0:
+                self.inputs[self.names[i]] = LabelInput(
+                    parent=self,
+                    label=self.labels[i],
+                    input_class=ttk.Spinbox,
+                    input_var=tk.IntVar(),
+                    input_args={"from_": 1, "to": 32, "increment": 1, "width": 5},
+                    label_pos="top",
+                )
+                self.inputs[self.names[i]].grid(
+                    row=i, column=0, sticky=tk.NSEW, padx=5, pady=3
+                )
+            if i > 0:
+                self.inputs[self.names[i]] = LabelInput(
+                    parent=self,
+                    label=self.labels[i],
+                    input_class=ttk.Entry,
+                    input_var=tk.IntVar(),
+                    input_args={"width": 5, "state": "disabled"},
+                    label_pos="top",
+                )
+                self.inputs[self.names[i]].grid(
+                    row=i, column=0, sticky=(tk.NSEW), padx=5, pady=3
+                )
+                self.inputs[self.names[i]].configure(width=5)
+
+    def get_variables(self):
+        """This function returns a dictionary of all the variables that are tied to
+        each  widget name.
+
+        The key is the widget name, value is the variable associated.
 
         Returns
         -------
-        tuple
-            A tuple containing the file path, setups, and transforms.
+        variables : dict
+            The dictionary that holds the variables.
         """
+        variables = {}
+        for key, widget in self.inputs.items():
+            variables[key] = widget.get()
+        return variables
 
-        # Open the file, if present
-        if isinstance(root, str) and os.path.isfile(root):
-            with open(root, "r") as fp:
-                example = fp.read()
-                root = ET.fromstring(example)
-
-        if root.tag != "SpimData":
-            raise NotImplementedError(f"Unknown format {root.tag} failed to load.")
-
-        # Check if we are loading a BigDataViewer hdf5
-        image_loader = root.find("SequenceDescription/ImageLoader")
-        if image_loader.attrib["format"] not in ["bdv.hdf5", "bdv.n5"]:
-            raise NotImplementedError(
-                f"Unknown format {image_loader.attrib['format']} failed to load."
-            )
+    def get_widgets(self):
+        """This function returns the dictionary that holds the widgets.
 
-        # Parse the file path
-        base_path = root.find("BasePath")
-        file = root.find("SequenceDescription/ImageLoader/hdf5")
-        file_path = os.path.join(base_path.text, file.text)
-
-        # Get setups. Each setup represents a visualisation data source in the viewer
-        # that provides one image volume per timepoint
-        setups = [
-            x.text for x in root.findall("SequenceDescription/ViewSetups/ViewSetup/id")
-        ]
+        The key is the widget name, value is the LabelInput class that has all the data.
+
+        Returns
+        -------
+        self.inputs : dict
+            The dictionary that holds the widgets.
+        """
+        return self.inputs
 
-        # Get channels, one per setup
-        channels = list(
-            set(
-                [
-                    x.text
-                    for x in root.findall(
-                        "SequenceDescription/ViewSetups/ViewSetup/attributes/channel"
-                    )
-                ]
-            )
-        )
 
-        # Get number of positions, one per setup/channel
-        self.positions = len(
-            root.findall("SequenceDescription/ViewSetups/ViewSetup/attributes/tile")
-        ) // len(channels)
-
-        # Get image sizes in (x, y, z), one per setup
-        sizes = [
-            [int(y) for y in x.text.split()]
-            for x in root.findall("SequenceDescription/ViewSetups/ViewSetup/size")
+class IntensityFrame(ttk.Labelframe):
+    """This class is the frame that holds the intensity controls."""
+
+    def __init__(self, cam_view, *args, **kwargs):
+        """Initialize the IntensityFrame class.
+
+         Parameters
+        ----------
+        cam_view : tk.Frame
+            The frame that will hold the intensity controls.
+        *args : tuple
+            Variable length argument list.
+        **kwargs : dict
+            Arbitrary keyword arguments.
+        """
+        # Init Frame
+        text_label = "LUT"
+        ttk.Labelframe.__init__(self, cam_view, text=text_label, *args, **kwargs)
+
+        # Formatting
+        tk.Grid.columnconfigure(self, "all", weight=1)
+        tk.Grid.rowconfigure(self, "all", weight=1)
+
+        #: dict: The dictionary that holds the widgets.
+        self.inputs = {}
+
+        #: list: The list of LUTs for the image display.
+        self.color_labels = [
+            "Gray",
+            "Gradient",
+            "Rainbow",
+            "SNR",
         ]
 
-        # Get image voxel sizes (dx, dy, dz), one per setup
-        voxel_sizes = [
-            [float(y) for y in x.text.split()]
-            for x in root.findall(
-                "SequenceDescription/ViewSetups/ViewSetup/voxelSize/size"
-            )
+        #: list: The list of maplotlib LUT names.
+        self.color_values = [
+            "gist_gray",
+            "plasma",
+            "afmhot",
+            "RdBu_r",
         ]
 
-        # Get timepoints
-        timepoint_type = root.find("SequenceDescription/Timepoints").attrib["type"]
-        if timepoint_type != "range":
-            raise NotImplementedError(
-                f"Unknown format {timepoint_type} failed to load."
+        #: tk.StringVar: The variable that holds the LUT.
+        self.color = tk.StringVar()
+        for i in range(len(self.color_labels)):
+            self.inputs[self.color_labels[i]] = LabelInput(
+                parent=self,
+                label=self.color_labels[i],
+                input_class=ttk.Radiobutton,
+                input_var=self.color,
+                input_args={"value": self.color_values[i]},
             )
-        t_start = int(root.find("SequenceDescription/Timepoints/first").text)
-        t_stop = int(root.find("SequenceDescription/Timepoints/last").text)
-        timepoints = (t_start, t_stop + 1)
-
-        # Get affine transformations, one per setup
-        tt, ts = np.array(
-            [
-                [int(x.attrib["timepoint"]), int(x.attrib["setup"])]
-                for x in root.findall("ViewRegistrations/ViewRegistration")
-            ]
-        ).T
-        transforms = [
-            np.array(x.text.split(), dtype=float).reshape(-1, 4)
-            for x in root.findall(
-                "ViewRegistrations/ViewRegistration/ViewTransform/affine"
+            self.inputs[self.color_labels[i]].grid(
+                row=i, column=0, sticky=tk.NSEW, pady=3
             )
-        ]
 
-        # Set up metadata parameters
-        self.dx, self.dy, self.dz = np.array(voxel_sizes).min(
-            0
-        )  # default to finest sampling
-        self._multiposition = self.positions > 1
-        self.shape_x, self.shape_y, self.shape_z = np.array(sizes).max(
-            0
-        )  # default to largest size captured
-        self.shape_c = len(channels)
-        self.shape_t = timepoints[1] - timepoints[0]
+        #: tk.BooleanVar: The variable that holds the flip xy flag.
+        self.transpose = tk.BooleanVar()
 
-        return file_path, setups, transforms
+        #: str: The name of the flip xy flag.
+        self.trans = "Flip XY"
+        self.inputs[self.trans] = LabelInput(
+            parent=self,
+            label=self.trans,
+            input_class=ttk.Checkbutton,
+            input_var=self.transpose,
+        )
+        self.inputs[self.trans].grid(
+            row=len(self.color_labels), column=0, sticky=tk.NSEW, pady=3
+        )
 
-    def write_xml(self, file_name: str, views: list) -> None:
-        """Write BigDataViewer XML metadata.
+        #: tk.BooleanVar: The variable that holds the autoscale flag.
+        self.autoscale = tk.BooleanVar()
 
-        Parameters
-        ----------
-        file_name : str
-            The file name of the file to be written.
-        views : list
-            A list of dictionaries containing metadata for each view.
+        #: str: The name of the autoscale flag.
+        self.auto = "Autoscale"
 
-        """
+        #: list: The list of min and max counts.
+        self.minmax = ["Min Counts", "Max Counts"]
 
-        return super().write_xml(
-            file_name, file_type="bdv", root="SpimData", views=views
+        #: list: The list of min and max names.
+        self.minmax_names = ["Min", "Max"]
+        self.inputs[self.auto] = LabelInput(
+            parent=self,
+            label=self.auto,
+            input_class=ttk.Checkbutton,
+            input_var=self.autoscale,
+        )
+        self.inputs[self.auto].grid(
+            row=len(self.color_labels) + 1, column=0, sticky=tk.NSEW, pady=3
         )
+
+        # Max and Min Counts
+        for i in range(len(self.minmax)):
+            self.inputs[self.minmax_names[i]] = LabelInput(
+                parent=self,
+                label=self.minmax[i],
+                input_class=ttk.Spinbox,
+                input_var=tk.IntVar(),
+                input_args={"from_": 1, "to": 2**16 - 1, "increment": 1, "width": 5},
+            )
+            self.inputs[self.minmax_names[i]].grid(
+                row=i + len(self.color_labels) + 2,
+                column=0,
+                sticky=tk.NSEW,
+                padx=3,
+                pady=3,
+            )
+
+    def get_variables(self):
+        """This function returns a dictionary of all the variables that are tied to
+        each  widget name.
+
+        The key is the widget name, value is the variable associated.
+
+        Returns
+        -------
+        variables : dict
+            The dictionary that holds the variables.
+        """
+        variables = {}
+        for key, widget in self.inputs.items():
+            variables[key] = widget.get()
+        return variables
+
+    def get_widgets(self):
+        """This function returns the dictionary that holds the widgets.
+
+        The key is the widget name, value is the LabelInput class that has all the data.
+
+        Returns
+        -------
+        self.inputs : dict
+            The dictionary that holds the widgets.
+        """
+        return self.inputs
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/metadata_sources/metadata.py` & `navigate_micro-0.0.6/src/navigate/model/metadata_sources/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,19 +165,20 @@
         ]
         zoom = state["zoom"]
         pixel_size = float(scope["zoom"]["pixel_size"][zoom])
         self.dx, self.dy = pixel_size, pixel_size
         self.dz = float(abs(state["step_size"]))
         self.dt = float(state["timepoint_interval"])
 
+        # TODO: do we need to update the XML meta data accordingly?
         self.shape_x = int(
-            self.configuration["experiment"]["CameraParameters"]["x_pixels"]
+            self.configuration["experiment"]["CameraParameters"]["img_x_pixels"]
         )
         self.shape_y = int(
-            self.configuration["experiment"]["CameraParameters"]["y_pixels"]
+            self.configuration["experiment"]["CameraParameters"]["img_y_pixels"]
         )
         if (
             (state["image_mode"] == "z-stack")
             or (state["image_mode"] == "customized")
             or (state["image_mode"] == "ConstantVelocityAcquisition")
         ):
             self.shape_z = int(state["number_z_steps"])
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/metadata_sources/ome_tiff_metadata.py` & `navigate_micro-0.0.6/src/navigate/model/metadata_sources/ome_tiff_metadata.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/model/microscope.py` & `navigate_micro-0.0.6/src/navigate/model/microscope.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         #: dict: Dictionary of plugin devices
         self.plugin_devices = {}
 
         if is_virtual:
             return
 
         device_ref_dict = {
-            "camera": ["type", "serial_number"],
+            "camera": ["serial_number"],
             "filter_wheel": ["type"],
             "zoom": ["type", "servo_id"],
             "shutter": ["type", "channel"],
             "remote_focus_device": ["type", "channel"],
             "galvo": ["type", "channel"],
             "lasers": ["wavelength"],
             "mirror": ["type"],
@@ -190,20 +190,22 @@
                 ):
                     device_connection = devices_dict[device_name][device_ref_name]
 
                 elif is_plugin:
                     device_plugin_dict = devices_dict.get(device_name, {})
                     try:
                         exec(
-                            f"device_plugin_dict['{device_ref_name}'] = devices_dict['__plugins__']['{device_name}']['load_device'](configuration, is_synthetic)"
+                            f"device_plugin_dict['{device_ref_name}'] = devices_dict['__plugins__']['{device_name}']['load_device']"
+                            f"(configuration['configuration']['microscopes'][self.microscope_name]['{device_name}']['hardware'], is_synthetic)"
                         )
                         devices_dict[device_name] = device_plugin_dict
                         device_connection = device_plugin_dict[device_ref_name]
                         exec(
-                            f"self.plugin_devices['{device_name}'] = devices_dict['__plugins__']['{device_name}']['start_device'](self.microscope_name, device_connection, configuration, is_synthetic)"
+                            f"self.plugin_devices['{device_name}'] = devices_dict['__plugins__']['{device_name}']['start_device']"
+                            f"(self.microscope_name, device_connection, configuration, is_synthetic)"
                         )
                     except RuntimeError:
                         print(
                             f"Device {device_name} isn't loaded correctly! Please check the spelling and the plugin!"
                         )
                         continue
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/model.py` & `navigate_micro-0.0.6/src/navigate/model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,15 +499,15 @@
             "Navigate Model - Received command from controller:", command, args
         )
         if not self.data_buffer:
             logging.debug("Navigate Model - Shared Memory Buffer Not Set Up.")
             return
 
         if command == "acquire":
-            """ Begin an acquisition."""
+            """Begin an acquisition."""
             self.is_acquiring = True
             self.imaging_mode = self.configuration["experiment"]["MicroscopeState"][
                 "image_mode"
             ]
             self.is_save = self.configuration["experiment"]["MicroscopeState"][
                 "is_save"
             ]
@@ -747,15 +747,16 @@
             self.stop_stage()
 
         elif command == "terminate":
             self.terminate()
 
         # elif command == "change_camera":
         #     new_camera = list(self.active_microscope.cameras.values())[args[0]]
-        #     print(f"Using new camera >> {new_camera.camera_controller._serial_number}")
+        #     print(f"Using new camera >> {
+        #     new_camera.camera_controller._serial_number}")
         #     self.active_microscope.camera = new_camera
 
         elif command == "exit":
             for camera in self.active_microscope.cameras.values():
                 camera.camera_controller.dev_close()
         else:
             self.active_microscope.run_command(command, *args)
@@ -1061,15 +1062,15 @@
         except:  # noqa
             self.active_microscope.daq.stop_acquisition()
             if self.active_microscope.current_channel == 0:
                 self.stop_acquisition = True
                 self.event_queue.put(
                     (
                         "warning",
-                        "There is an error happened. Please read the log files for details!",
+                        "An error happened. Please read the log files for details!",
                     )
                 )
                 return
             self.active_microscope.daq.prepare_acquisition(
                 f"channel_{self.active_microscope.current_channel}"
             )
             self.active_microscope.daq.run_acquisition()
@@ -1085,20 +1086,21 @@
     def run_live_acquisition(self):
         """Stream live image to the GUI.
 
         Recalculates the waveforms for each image, thereby allowing people to adjust
         acquisition parameters in real-time.
         """
         self.stop_acquisition = False
-        while self.stop_acquisition is False and self.stop_send_signal is False:
+        while not self.stop_acquisition and not self.stop_send_signal:
             self.run_acquisition()
-            if not self.injected_flag.value:
-                self.signal_container.reset()
-            else:
+            if self.injected_flag.value:
                 self.reset_feature_list()
+            elif hasattr(self, "signal_container"):
+                self.signal_container.reset()
+
         # Update the stage position.
         # Allows the user to externally move the stage in the continuous mode.
         self.get_stage_position()
 
     def run_acquisition(self):
         """Run acquisition along with a feature list one time."""
         if not hasattr(self, "signal_container"):
@@ -1148,15 +1150,14 @@
                             "args": ("experiment.MicroscopeState.selected_channels",),
                         },
                     )
                 ],
             )
             injected_flag.value = False
 
-
     def change_resolution(self, resolution_value):
         """Switch resolution mode of the microscope.
 
         Parameters
         ----------
         resolution_value : str
             Resolution mode.
@@ -1419,30 +1420,30 @@
             System folcer can be found at '..../.navigate/feature_lists'
         """
         feature_lists_path = get_navigate_path() + "/feature_lists"
         if not os.path.exists(feature_lists_path):
             os.makedirs(feature_lists_path)
             return
         # get __sequence.yml
-        if not os.path.exists(f"{feature_lists_path}/__sequence.yml"):
+        feature_records = load_yaml_file(f"{feature_lists_path}/__sequence.yml")
+        if feature_records is None:
             feature_records = []
-        else:
-            feature_records = load_yaml_file(f"{feature_lists_path}/__sequence.yml")
-
         # add non added feature lists
         feature_list_files = [
             temp
             for temp in os.listdir(feature_lists_path)
             if (temp.endswith(".yml") or temp.endswith(".yaml"))
             and os.path.isfile(os.path.join(feature_lists_path, temp))
         ]
         for item in feature_list_files:
             if item == "__sequence.yml":
                 continue
             temp = load_yaml_file(f"{feature_lists_path}/{item}")
+            if temp is None:
+                continue
             add_flag = True
             for feature in feature_records:
                 if feature["feature_list_name"] == temp["feature_list_name"]:
                     add_flag = False
                     break
             if add_flag:
                 feature_records.append(
@@ -1455,14 +1456,17 @@
         i = 0
         while i < len(feature_records):
             temp = feature_records[i]
             if not os.path.exists(f"{feature_lists_path}/{temp['yaml_file_name']}"):
                 del feature_records[i]
                 continue
             item = load_yaml_file(f"{feature_lists_path}/{temp['yaml_file_name']}")
+            if item is None:
+                i += 1
+                continue
 
             if item["module_name"]:
                 try:
                     module = load_module_from_file(
                         item["module_name"], item["filename"]
                     )
                     feature = getattr(module, item["module_name"])
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/plugins_model.py` & `navigate_micro-0.0.6/src/navigate/model/plugins_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,20 +77,21 @@
                     self.plugins_path, f
                 )
 
         # load plugins from plugins_config
         plugins_config_path = os.path.join(
             get_navigate_path(), "config", "plugins_config.yml"
         )
-        if not os.path.exists(plugins_config_path):
+        plugins_config = load_yaml_file(plugins_config_path)
+        if plugins_config is None:
+            plugins_config = {}
             save_yaml_file(
                 os.path.join(get_navigate_path(), "config"), {}, "plugins_config.yml"
             )
         else:
-            plugins_config = load_yaml_file(plugins_config_path)
             verified_plugins_config = {}
             for plugin_name, plugin_path in plugins_config.items():
                 if not plugin_path:
                     print(
                         f"Plugin '{plugin_name}' is not installed correctly. "
                         f"Please reinstall it if necessary."
                     )
@@ -203,18 +204,37 @@
                             device_type_name = module.DEVICE_TYPE_NAME
                         except AttributeError:
                             print(
                                 f"Plugin device: {device} is not set correctly!"
                                 "Please make sure the DEVICE_TYPE_NAME is given right!"
                             )
                             continue
-                        devices_dict[device_type_name] = {}
-                        devices_dict[device_type_name][
-                            "ref_list"
-                        ] = module.DEVICE_REF_LIST
-                        devices_dict[device_type_name][
-                            "load_device"
-                        ] = module.load_device
-                        devices_dict[device_type_name][
-                            "start_device"
-                        ] = module.start_device
+                        # core devices
+                        core_devices = ["camera", "remote_focus_device", "galvo",
+                                        "filter_wheel", "stage", "zoom", "shutter", "lasers"]
+                        if device_type_name in core_devices:
+                            if device_type_name not in devices_dict:
+                                devices_dict[device_type_name] = {}
+                                devices_dict[device_type_name]["load_device"] = []
+                                devices_dict[device_type_name]["start_device"] = []
+                            devices_dict[device_type_name]["load_device"].append(module.load_device)
+                            devices_dict[device_type_name]["start_device"].append(module.start_device)
+                        elif device_type_name == "multiple_devices":
+                            for device_name in core_devices:
+                                if device_name not in devices_dict:
+                                    devices_dict[device_name] = {}
+                                    devices_dict[device_name]["load_device"] = []
+                                    devices_dict[device_name]["start_device"] = []
+                                devices_dict[device_name]["load_device"].append(module.load_device)
+                                devices_dict[device_name]["start_device"].append(module.start_device)
+                        else:
+                            devices_dict[device_type_name] = {}
+                            devices_dict[device_type_name][
+                                "ref_list"
+                            ] = module.DEVICE_REF_LIST
+                            devices_dict[device_type_name][
+                                "load_device"
+                            ] = module.load_device
+                            devices_dict[device_type_name][
+                                "start_device"
+                            ] = module.start_device
         return devices_dict, plugin_acquisition_modes
```

### Comparing `navigate-micro-0.0.5/src/navigate/model/waveforms.py` & `navigate_micro-0.0.6/src/navigate/model/waveforms.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/tools/common_dict_tools.py` & `navigate_micro-0.0.6/src/navigate/tools/common_dict_tools.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/tools/common_functions.py` & `navigate_micro-0.0.6/src/navigate/tools/common_functions.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/tools/decorators.py` & `navigate_micro-0.0.6/src/navigate/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/tools/file_functions.py` & `navigate_micro-0.0.6/src/navigate/tools/file_functions.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/tools/image.py` & `navigate_micro-0.0.6/src/navigate/tools/image.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/tools/linear_algebra.py` & `navigate_micro-0.0.6/src/navigate/tools/linear_algebra.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/tools/main_functions.py` & `navigate_micro-0.0.6/src/navigate/tools/main_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,25 +64,32 @@
         Path to remote focusing and galvo waveform constants file
     rest_api_path
         Path to REST API file
     waveform_templates_path
         Path to waveform templates file
     logging_path
         Path to non-default logging location
+    configurator
+        Boolean, True if configurator is enabled
     """
     # Retrieve the Default Configuration paths
     (
         configuration_path,
         experiment_path,
         waveform_constants_path,
         rest_api_path,
         waveform_templates_path,
     ) = get_configuration_paths()
 
     # Evaluate Input Arguments
+    if args.configurator:
+        configurator = True
+    else:
+        configurator = False
+
     if args.config_file:
         assert args.config_file.exists(), "Configuration file Path {} not valid".format(
             args.config_file
         )
         configuration_path = args.config_file
 
     if args.experiment_file:
@@ -123,14 +130,15 @@
     return (
         configuration_path,
         experiment_path,
         waveform_constants_path,
         rest_api_path,
         waveform_templates_path,
         logging_path,
+        configurator,
     )
 
 
 def create_parser():
     """Add Parser Input Arguments to ArgumentParser Object.
 
     Parameters
@@ -143,14 +151,23 @@
         ArgumentParserObject with Added Input Arguments"""
 
     parser = argparse.ArgumentParser(description="navigate Command Line Arguments")
 
     input_args = parser.add_argument_group("Input Arguments")
 
     input_args.add_argument(
+        "-c",
+        "--configurator",
+        required=False,
+        default=False,
+        action="store_true",
+        help="Configurator - " "GUI for preparing a configuration.yaml file..",
+    )
+
+    input_args.add_argument(
         "-sh",
         "--synthetic-hardware",
         required=False,
         default=False,
         action="store_true",
         help="Synthetic Hardware - "
         "Allows launching of the software without the physical devices attached.",
```

### Comparing `navigate-micro-0.0.5/src/navigate/tools/multipos_table_tools.py` & `navigate_micro-0.0.6/src/navigate/tools/multipos_table_tools.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/tools/sdf.py` & `navigate_micro-0.0.6/src/navigate/tools/sdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,7 +104,23 @@
     """
     w = np.array(w)  # Ensure w is an array
 
     q = np.abs(p) - w[:, None]
     return np.linalg.norm(np.maximum(q, 0.0), axis=0) + np.minimum(
         np.maximum(q[0, :], np.maximum(q[1, :], q[2, :])), 0.0
     )
+
+def ellipsoid(p, r):
+    """Signed distance function for an ellipsoid.
+    
+    p : npt.ArrayLike
+        (3, N) array of points on which to evaluate the sdf.
+    w : tuple
+        (3,) tuple of ellipsoid radii
+    """
+
+    r = np.array(r)
+
+    k0 = np.linalg.norm(p/(r[:,None]), axis=0)
+    k1 = np.linalg.norm(p/((r*r)[:,None]), axis=0)
+
+    return k0*(k0-1.0)/k1
```

### Comparing `navigate-micro-0.0.5/src/navigate/tools/waveform_template_funcs.py` & `navigate_micro-0.0.6/src/navigate/tools/waveform_template_funcs.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/tools/xml_tools.py` & `navigate_micro-0.0.6/src/navigate/tools/xml_tools.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/custom_widgets/ArrowLabel.py` & `navigate_micro-0.0.6/src/navigate/view/custom_widgets/ArrowLabel.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/custom_widgets/DockableNotebook.py` & `navigate_micro-0.0.6/src/navigate/view/custom_widgets/DockableNotebook.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/custom_widgets/LabelInputWidgetFactory.py` & `navigate_micro-0.0.6/src/navigate/view/custom_widgets/LabelInputWidgetFactory.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/custom_widgets/hover.py` & `navigate_micro-0.0.6/src/navigate/view/custom_widgets/hover.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/custom_widgets/hoverbar.py` & `navigate_micro-0.0.6/src/navigate/view/custom_widgets/hoverbar.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/custom_widgets/hovermixin.py` & `navigate_micro-0.0.6/src/navigate/view/custom_widgets/hovermixin.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/custom_widgets/popup.py` & `navigate_micro-0.0.6/src/navigate/view/custom_widgets/popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/custom_widgets/scrollbars.py` & `navigate_micro-0.0.6/src/navigate/view/custom_widgets/scrollbars.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/custom_widgets/validation.py` & `navigate_micro-0.0.6/src/navigate/view/custom_widgets/validation.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/icon/mic.ico` & `navigate_micro-0.0.6/src/navigate/view/icon/mic.ico`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/icon/mic.png` & `navigate_micro-0.0.6/src/navigate/view/icon/mic.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/icon/mic_orig.png` & `navigate_micro-0.0.6/src/navigate/view/icon/mic_orig.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/icon/splash_screen_image.png` & `navigate_micro-0.0.6/src/navigate/view/icon/splash_screen_image.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_application_window.py` & `navigate_micro-0.0.6/src/navigate/view/main_application_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     A main window is created and passed to the mainapp class. This class will init as a
     frame then config the main window. It then creates a menubar using the menubar
     class.
 
     Adds the options for each file menu. It then sets up the frames, then grids the
     frames.
 
-    Finally it uses the notebook classes to put them into the respective frames on the
+    Finally, it uses the notebook classes to put them into the respective frames on the
     tk.Grid. Each of the notebook classes includes tab classes and inits those etc.
 
     The second parameter in each classes __init__ function is the parent.
 
     I used the name of the parent so that it would be easier to keep track of
     inheritances.
 
@@ -104,33 +104,32 @@
         # Inits this class as a frame subclass with the root as its parent
         #: ScrolledFrame: The scrollable version of the main frame for the application
         self.scroll_frame = ScrolledFrame(root)
         self.scroll_frame.grid(row=0, column=0, sticky=tk.NSEW)
 
         ttk.Frame.__init__(self, self.scroll_frame.interior, *args, **kwargs)
 
-        # Initialize Logger
         #: logging.Logger: The logger for this class
         self.logger = logging.getLogger(p)
 
-        # This starts the main window config, and makes sure that any child
-        # widgets can be resized with the window
         #: tk.Tk: The main window of the application
         self.root = root
         self.root.title("navigate")
 
         # keep icons relative to view directory structure
         view_directory = Path(__file__).resolve().parent
         try:
             photo_image = view_directory.joinpath("icon", "mic.png")
             self.root.iconphoto(True, tk.PhotoImage(file=photo_image))
         except tk.TclError:
             pass
+
         self.root.resizable(True, True)
         self.root.geometry("")
+
         tk.Grid.columnconfigure(root, "all", weight=1)
         tk.Grid.rowconfigure(root, "all", weight=1)
 
         # Creating and linking menu to main window/app
         #: Menubar: The menu bar for the application
         self.menubar = Menubar(root)
 
@@ -155,15 +154,15 @@
         self.top_frame.grid(
             row=0, column=0, columnspan=2, sticky=tk.NSEW, padx=3, pady=3
         )
         self.frame_left.grid(row=1, column=0, rowspan=2, sticky=tk.NSEW, padx=3, pady=3)
         self.frame_top_right.grid(row=1, column=1, sticky=tk.NSEW, padx=3, pady=3)
         self.frame_bottom_right.grid(row=2, column=1, sticky=tk.NSEW, padx=3, pady=3)
 
-        # Putting Notebooks into frames, tabs are held within the class of each
-        # notebook
         #: SettingsNotebook: The settings notebook for the application
         self.settings = SettingsNotebook(self.frame_left, self.root)
+
         #: CameraNotebook: The camera notebook for the application
         self.camera_waveform = CameraNotebook(self.frame_top_right, self.root)
+
         #: AcquireBar: The acquire bar for the application
         self.acqbar = AcquireBar(self.top_frame, self.root)
```

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/acquire_notebook.py` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/acquire_notebook.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/camera_tab.py` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/camera_tab.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/channels_tab.py` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/channels_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,34 +285,34 @@
 
             #  Exposure Time Spin boxes
             self.exptime_variables.append(tk.StringVar())
             self.exptime_pulldowns.append(
                 ValidatedSpinbox(
                     self.frame_columns[4],
                     from_=0,
-                    to=5000.0,
+                    to=1000.0,
                     textvariable=self.exptime_variables[num],
-                    increment=25,
+                    increment=5,
                     width=5,
                     font=tk.font.Font(size=11),
                 )
             )
             self.exptime_pulldowns[num].grid(
                 row=num + 1, column=0, sticky=tk.NSEW, padx=1, pady=1
             )
 
             #  Time Interval Spin boxes
             self.interval_variables.append(tk.StringVar())
             self.interval_spins.append(
                 ValidatedSpinbox(
                     self.frame_columns[5],
                     from_=0,
-                    to=5000.0,
+                    to=1000.0,
                     textvariable=self.interval_variables[num],
-                    increment=1,
+                    increment=5,
                     width=3,
                     font=tk.font.Font(size=11),
                 )
             )
             self.interval_spins[num].grid(
                 row=num + 1, column=0, sticky=tk.NSEW, padx=1, pady=1
             )
@@ -390,15 +390,15 @@
         self.start_label.grid(row=0, column=0, sticky="S")
         for i in range(len(start_names)):
             self.inputs[start_names[i]] = LabelInput(
                 parent=self.pos_slice,
                 label=start_labels[i],
                 input_class=ValidatedSpinbox,
                 input_var=tk.DoubleVar(),
-                input_args={"from_": 0.0, "to": 10000, "increment": 0.5, "width": 6},
+                input_args={"from_": -5000, "to": 10000, "increment": 1, "width": 6},
             )
             self.inputs[start_names[i]].grid(
                 row=i + 1, column=0, sticky="N", pady=2, padx=(6, 0)
             )
             self.inputs[start_names[i]].label.grid(sticky="N")
 
         # Start button
@@ -416,15 +416,15 @@
         self.end_label.grid(row=0, column=1, sticky="S")
         for i in range(len(end_names)):
             self.inputs[end_names[i]] = LabelInput(
                 parent=self.pos_slice,
                 label=end_labels[i],
                 input_class=ValidatedSpinbox,
                 input_var=tk.DoubleVar(),
-                input_args={"from_": 0.0, "to": 10000, "increment": 0.5, "width": 6},
+                input_args={"from_": -5000, "to": 10000, "increment": 1, "width": 6},
             )
             self.inputs[end_names[i]].grid(
                 row=i + 1, column=1, sticky="N", pady=2, padx=(6, 0)
             )
             self.inputs[end_names[i]].label.grid(sticky="N")
 
         # End Button
@@ -435,15 +435,15 @@
         #: tkinter.Label: The label for the step size
         self.step_size_label = ttk.Label(self.pos_slice, text="Step Size")
         self.step_size_label.grid(row=0, column=2, sticky="S")
         self.inputs["step_size"] = LabelInput(
             parent=self.pos_slice,
             input_class=ValidatedSpinbox,
             input_var=tk.DoubleVar(),
-            input_args={"width": 6},
+            input_args={"from_": 0.1, "to": 1000, "increment": 0.1, "width": 6},
         )
         self.inputs["step_size"].grid(row=1, column=2, sticky="N", padx=6)
 
         # Slice Frame (Vertically oriented)
         #: tkinter.Label: The label to add empty space to the slice frame
         self.empty_label = ttk.Label(self.pos_slice, text=" ")
         self.empty_label.grid(row=0, column=3, sticky="N")
@@ -451,15 +451,15 @@
         slice_labels = ["# slices      ", "Abs Z Start", "Abs Z Stop"]
         for i in range(len(slice_names)):
             self.inputs[slice_names[i]] = LabelInput(
                 parent=self.pos_slice,
                 label=slice_labels[i],
                 input_class=ttk.Spinbox,
                 input_var=tk.DoubleVar(),
-                input_args={"increment": 0.5, "width": 6},
+                input_args={"from_": 0.1, "to": 1000, "increment": 0.1, "width": 6},
             )
             self.inputs[slice_names[i]].widget.configure(state="disabled")
             self.inputs[slice_names[i]].grid(
                 row=i + 1, column=3, sticky="NSEW", pady=2, padx=(6, 0)
             )
 
         # Laser Cycling Settings
@@ -599,15 +599,15 @@
         self.stack_acq_spinval = tk.StringVar()
         #: ttk.Spinbox: The stack acquisition time spinbox
         self.stack_acq_spinbox = ttk.Spinbox(
             self,
             from_=0,
             to=5000.0,
             textvariable=self.stack_acq_spinval,  # this holds the data in the entry
-            increment=25,
+            increment=1,
             width=6,
         )
         self.stack_acq_spinbox.grid(row=2, column=1, sticky=tk.NSEW, pady=2)
         self.stack_acq_spinbox.state(["disabled"])  # Starts it disabled
 
         # Stack Pause Label
         #: tkinter.Label: The label for the stack pause spinbox
@@ -619,15 +619,15 @@
         self.stack_pause_spinval = tk.StringVar()
         #: ttk.Spinbox: The stack pause spinbox
         self.stack_pause_spinbox = ValidatedSpinbox(
             self,
             from_=0,
             to=5000.0,
             textvariable=self.stack_pause_spinval,
-            increment=25,
+            increment=1,
             width=6,
         )
         self.stack_pause_spinbox.grid(row=0, column=3, sticky=tk.NSEW, pady=2)
         self.inputs["stack_pause"] = self.stack_pause_spinbox
 
         # Timepoint Interval Label
         #: tkinter.Label: The label for the timepoint interval spinbox
```

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/display_notebook.py` & `navigate_micro-0.0.6/src/navigate/view/popups/feature_list_popup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (c) 2021-2022  The University of Texas Southwestern Medical Center.
 # All rights reserved.
 
 # Redistribution and use in source and binary forms, with or without
-# modification, are permitted for academic and research use only
-# (subject to the limitations in the disclaimer below)
-# provided that the following conditions are met:
+# modification, are permitted for academic and research use only (subject to the
+# limitations in the disclaimer below) provided that the following conditions are met:
 
 #      * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 
 #      * Redistributions in binary form must reproduce the above copyright
 #      notice, this list of conditions and the following disclaimer in the
 #      documentation and/or other materials provided with the distribution.
@@ -25,556 +24,478 @@
 # CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 # IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
+#
 
 # Standard Library Imports
 import tkinter as tk
-from tkinter import ttk, Grid
-import logging
-
-# Third Party Imports
-from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
-from matplotlib.figure import Figure
+from tkinter import ttk
 
 # Local Imports
-from navigate.view.custom_widgets.DockableNotebook import DockableNotebook
+from navigate.view.custom_widgets.popup import PopUp
 from navigate.view.custom_widgets.LabelInputWidgetFactory import LabelInput
 
 
-# Logger Setup
-p = __name__.split(".")[1]
-logger = logging.getLogger(p)
-
-
-class CameraNotebook(DockableNotebook):
-    """This class is the notebook that holds the camera view and waveform settings
-    tabs."""
-
-    def __init__(self, frame_top_right, *args, **kwargs):
-        """Init function for the CameraNotebook class.
+class FeatureIcon(ttk.Button):
+    """Feature Icon Widget"""
 
+    def __init__(self, parent, feature_name="", set_bg=False):
+        """Initialize the Feature Icon Widget
 
         Parameters
         ----------
-        frame_top_right : tk.Frame
-            The frame that will hold the notebook.
-        *args : tuple
-            Variable length argument list.
-        **kwargs : dict
-            Arbitrary keyword arguments.
-        """
-        # Init notebook
-        DockableNotebook.__init__(self, frame_top_right, *args, **kwargs)
-
-        # Putting notebook 2 into top right frame
-        self.grid(row=0, column=0)
-
-        #: CameraTab: The camera tab.
-        self.camera_tab = CameraTab(self)
-
-        #: WaveformTab: The waveform settings tab.
-        self.waveform_tab = WaveformTab(self)
-
-        # Tab list
-        tab_list = [self.camera_tab, self.waveform_tab]
-        self.set_tablist(tab_list)
-
-        # Adding tabs to self notebook
-        self.add(self.camera_tab, text="Camera View", sticky=tk.NSEW)
-        self.add(self.waveform_tab, text="Waveform Settings", sticky=tk.NSEW)
-
-
-class CameraTab(tk.Frame):
-    """CameraTab class."""
-
-    def __init__(self, cam_wave, *args, **kwargs):
-        """Initialize the CameraTab class.
+        parent : tk.Frame
+            Parent frame of the widget
+        feature_name : str
+            Name of the feature
+        """
+        ttk.Button.__init__(self, parent, text=feature_name)
+
+        # Create a style
+        style = ttk.Style()
+        style.configure("Custom.TButton", background="red")
+        if set_bg:
+            self.configure(style="Custom.TButton")
+        
+        self.configure(padding=(10, 20))
+
+
+class FeatureConfigPopup:
+    """Feature Config Popup Widget"""
+
+    def __init__(
+        self,
+        root,
+        *args,
+        features=[],
+        feature_name="",
+        args_name=[],
+        args_value=[],
+        **kwargs
+    ):
+        """Initialize the Feature Config Popup Widget
 
         Parameters
         ----------
-        cam_wave : tk.Frame
-            The frame that will hold the camera tab.
-        *args : tuple
-            Variable length argument list.
-        **kwargs : dict
-            Arbitrary keyword arguments.
-        """
-        #  Init Frame
-        tk.Frame.__init__(self, cam_wave, *args, **kwargs)
-
-        #: int: The index of the tab.
-        self.index = 0
-
-        # Formatting
-        tk.Grid.columnconfigure(self, "all", weight=1)
-        tk.Grid.rowconfigure(self, "all", weight=1)
-
-        #: tk.Frame: The frame that will hold the camera image.
-        self.cam_image = ttk.Frame(self)
-        self.cam_image.grid(row=0, column=0, rowspan=3, sticky=tk.NSEW)
-
-        #: Bool: The popup flag.
-        self.is_popup = False
-
-        #: Bool: The docked flag.
-        self.is_docked = True
-
-        #: int: The width of the canvas.
-        #: int: The height of the canvas.
-        self.canvas_width, self.canvas_height = 512, 512
-
-        #: tk.Canvas: The canvas that will hold the camera image.
-        self.canvas = tk.Canvas(
-            self.cam_image, width=self.canvas_width, height=self.canvas_height
-        )
-        self.canvas.grid(row=0, column=0, sticky=tk.NSEW, padx=5, pady=5)
-
-        #: matplotlib.figure.Figure: The figure that will hold the camera image.
-        self.matplotlib_figure = Figure(figsize=[6, 6], tight_layout=True)
-
-        #: matplotlib.backends.backend_tkagg.FigureCanvasTkAgg: The canvas that will
-        # hold the camera image.
-        self.matplotlib_canvas = FigureCanvasTkAgg(self.matplotlib_figure, self.canvas)
-
-        #: IntensityFrame: The frame that will hold the scale settings/palette color.
-        self.scale_palette = IntensityFrame(self)
-        self.scale_palette.grid(row=0, column=1, sticky=tk.NSEW, padx=5, pady=5)
-
-        #: tk.Scale: The slider that will hold the slice index.
-        self.slider = tk.Scale(
-            self,
-            from_=0,
-            to=200,
-            tickinterval=20,
-            orient=tk.HORIZONTAL,
-            showvalue=0,
-            label="Slice Index",
+        root : tk.Tk
+            Root window of the application
+        *args : list
+            List of arguments
+        features : list
+            List of features
+        feature_name : str
+            Name of the feature
+        args_name : list
+            List of arguments name
+        args_value : list
+            List of arguments value
+        """
+        # Creating popup window with this name and size/placement,
+
+        #: PopUp: Popup window
+        self.popup = PopUp(
+            root, kwargs["title"], "+320+180", top=False, transient=False
+        )
+
+        # Change background of popup window to white
+        self.popup.configure(bg="white")
+
+        # Creating content frame
+        content_frame = self.popup.get_frame()
+
+        #: list: List of input widgets
+        self.inputs = []
+
+        #: LabelInput: Feature name widget
+        self.feature_name_widget = LabelInput(
+            parent=content_frame,
+            label="Feature Name",
+            label_args={"width": 20},
+            input_class=ttk.Combobox,
+            input_var=tk.StringVar(),
+            input_args={"width": 30, "state": "readonly"},
         )
-        self.slider.configure(state="disabled")  # 'normal'
-        self.slider.grid(row=3, column=0, sticky=tk.NSEW, padx=5, pady=5)
-
-        #: MetricsFrame: The frame that will hold the camera selection and counts.
-        self.image_metrics = MetricsFrame(self)
-        self.image_metrics.grid(row=1, column=1, sticky=tk.NSEW, padx=5, pady=5)
-
-        #: RenderFrame: The frame that will hold the live display functionality.
-        self.live_frame = RenderFrame(self)
-        self.live_frame.grid(row=2, column=1, sticky=tk.NSEW, padx=5, pady=5)
-
+        self.feature_name_widget.grid(row=0, column=0, sticky=tk.NSEW, padx=3, pady=3)
+        self.feature_name_widget.set(feature_name)
+        self.feature_name_widget.set_values(features)
+
+        separator = ttk.Separator(content_frame)
+        separator.grid(row=1, column=0, sticky=tk.NSEW, pady=10)
+
+        #: ttk.Frame: Parameter frame
+        self.parameter_frame = ttk.Frame(content_frame)
+        self.parameter_frame.grid(row=2, column=0, sticky=tk.NSEW, padx=30, pady=30)
+
+        row = 3
+        if "true" in kwargs:
+            self.preview_btn_true = ttk.Button(content_frame, text="Preview (True)")
+            self.preview_btn_true.grid(row=row, column=0, sticky=tk.NSEW)
+            separator = ttk.Separator(content_frame)
+            separator.grid(row=row+1, column=0, sticky=tk.NSEW, pady=(0,10))
+            self.feature_list_true_frame = FeatureListFrame(content_frame)
+            self.feature_list_true_frame.grid(row=row+2, column=0, sticky=tk.NSEW)
+            row += 3
+
+        if "false" in kwargs:
+            self.preview_btn_false = ttk.Button(content_frame, text="Preview (False)")
+            self.preview_btn_false.grid(row=row, column=0, sticky=tk.NSEW)
+            separator = ttk.Separator(content_frame)
+            separator.grid(row=row+1, column=0, sticky=tk.NSEW, pady=(0,10))
+            self.feature_list_false_frame = FeatureListFrame(content_frame)
+            self.feature_list_false_frame.grid(row=row+2, column=0, sticky=tk.NSEW)
 
-class RenderFrame(ttk.Labelframe):
-    """This class is the frame that holds the live display functionality."""
+        self.build_widgets(args_name, args_value, kwargs.get("parameter_config", {}))
 
-    def __init__(self, cam_view, *args, **kwargs):
-        """Initialize the RenderFrame class.
+    def build_widgets(self, args_name, args_value, parameter_config=None):
+        """Build widgets for the popup
 
         Parameters
         ----------
-        cam_view : tk.Frame
-            The frame that will hold the live display functionality.
-        *args : tuple
-            Variable length argument list.
-        **kwargs : dict
-            Arbitrary keyword arguments.
-        """
-        # Init Frame
-        text_label = "Image Display"
-        ttk.Labelframe.__init__(self, cam_view, text=text_label, *args, **kwargs)
-
-        # Formatting
-        Grid.columnconfigure(self, "all", weight=1)
-        Grid.rowconfigure(self, "all", weight=1)
-
-        #: tk.StringVar: The variable that holds the live display functionality.
-        self.live_var = tk.StringVar()
-
-        #: ttk.Combobox: The combobox that holds the live display functionality.
-        self.live = ttk.Combobox(
-            self, textvariable=self.live_var, state="readonly", width=6
-        )
-        self.live["values"] = (
-            "Live",
-            "XY Slice",
-            "YZ Slice",
-            "ZY Slice",
-            "XY MIP",
-            "YZ MIP",
-            "ZY MIP",
-        )
-        self.live.set("Live")
-        self.live.grid(row=0, column=0)
-        self.live.state = "readonly"
-
-    def get_variables(self):
-        """Function to get the variables.
-
-        The key is the widget name, value is the variable associated.
+        args_name : list
+            List of arguments name
+        args_value : list
+            List of arguments value
+        parameter_config : dict
+            Dictionary of parameter configuration
+        """
+        #: list: List of input widgets
+        self.inputs = []
+        #: list: List of input widgets type
+        self.inputs_type = []
+
+        for child in self.parameter_frame.winfo_children():
+            child.destroy()
+
+        for i, arg_name in enumerate(args_name):
+            arg_input_class = ttk.Entry
+            arg_input_var = tk.StringVar
+            if type(args_value[i]) is bool:
+                arg_input_class = ttk.Combobox
+                values = ["True", "False"]
+            elif parameter_config is not None and arg_name in parameter_config:
+                arg_input_class = ttk.Combobox
+                values = list(parameter_config[arg_name].keys())
+
+            temp = LabelInput(
+                parent=self.parameter_frame,
+                label=arg_name + ":",
+                label_args={"padding": (2, 5, 5, 0), "width": 20},
+                input_class=arg_input_class,
+                input_var=arg_input_var(),
+                input_args={"width": 30},
+            )
 
-        Returns
-        -------
-        variables : dict
-            The dictionary that holds the variables.
-        """
-        variables = {}
-        for key, widget in self.inputs.items():
-            variables[key] = widget.get()
-        return variables
+            self.inputs.append(temp)
+            self.inputs_type.append(type(args_value[i]))
+            temp.grid(row=i + 2, column=0, sticky=tk.NSEW, padx=30, pady=10)
+            if arg_input_class is ttk.Combobox:
+                temp.set_values(values)
+                temp.widget.config(state="readonly")
+            temp.set(str(args_value[i]))
 
     def get_widgets(self):
-        """Function to get the widgets.
-
-        The key is the widget name, value is the LabelInput class that has all the data.
+        """Get widgets
 
         Returns
         -------
-        self.inputs : dict
-            The dictionary that holds the widgets.
+        list
+            List of input widgets
         """
         return self.inputs
 
 
-class WaveformTab(tk.Frame):
-    """This class is the frame that holds the waveform tab."""
+class FeatureListPopup:
+    """Feature List Popup Widget"""
 
-    def __init__(self, cam_wave, *args, **kwargs):
-        """Initialize the WaveformTab class.
+    def __init__(self, root, *args, **kwargs):
+        """Initialize the Feature List Popup Widget
 
         Parameters
         ----------
-        cam_wave : tk.Frame
-            The frame that will hold the waveform tab.
-        *args : tuple
-            Variable length argument list.
+        root : tk.Tk
+            Root window of the application
+        *args : list
+            List of arguments
         **kwargs : dict
-            Arbitrary keyword arguments.
-
+            Dictionary of keyword arguments
         """
-        # Init Frame
-        tk.Frame.__init__(self, cam_wave, *args, **kwargs)
+        # Creating popup window with this name and size/placement,
+        # PopUp is a Toplevel window
+        #: PopUp: Popup window
+        self.popup = PopUp(
+            root, kwargs["title"], "+320+180", top=False, transient=False
+        )
+        # Change background of popup window to white
+        self.popup.configure(bg="white")
+        #: bool: Flag to indicate if the popup is for adding new list
+        self.add_new_list_flag = False
+        if kwargs["title"].startswith("Add"):
+            self.add_new_list_flag = True
 
-        #: int: The index of the tab.
-        self.index = 1
+        # Creating content frame
+        content_frame = self.popup.get_frame()
 
-        #: bool: The popup flag.
-        self.is_docked = True
+        #: dict: Dictionary of input widgets
+        self.inputs = {}
+        self.inputs["feature_list_name"] = LabelInput(
+            parent=content_frame,
+            label="Feature List Name",
+            input_class=ttk.Entry,
+            input_var=tk.StringVar(),
+            input_args={"width": 50},
+        )
 
-        # Formatting
-        tk.Grid.columnconfigure(self, "all", weight=1)
-        tk.Grid.rowconfigure(self, "all", weight=1)
+        self.inputs["feature_list_name"].grid(
+            row=0, column=0, sticky=tk.NSEW, padx=3, pady=3
+        )
 
-        #: tk.Frame: The frame that will hold the waveform plots.
-        self.waveform_plots = ttk.Frame(self)
-        self.waveform_plots.grid(row=0, column=0, sticky=tk.NSEW)
+        separator = ttk.Separator(content_frame)
+        separator.grid(row=2, column=0, sticky=tk.NSEW, padx=3, pady=3)
 
-        #: matplotlib.figure.Figure: The figure that will hold the waveform plots.
-        self.fig = Figure(figsize=(6, 6), dpi=100)
+        scroll_frame = ttk.Frame(content_frame)
+        scroll_frame.grid(row=3, column=0, sticky=tk.NSEW)
+        canvas = tk.Canvas(scroll_frame, width=800, height=350)
+        scrollbar = ttk.Scrollbar(scroll_frame, orient="horizon", command=canvas.xview)
+        self.feature_view_frame = ttk.Frame(canvas)
 
-        #: matplotlib.backends.backend_tkagg.FigureCanvasTkAgg: The canvas that will
-        # hold the waveform plots.
-        self.canvas = FigureCanvasTkAgg(self.fig, master=self.waveform_plots)
-        self.canvas.draw()
+        self.feature_view_frame.bind(
+            "<Configure>", lambda e: canvas.configure(scrollregion=canvas.bbox("all"))
+        )
 
-        #: tk.Frame: The frame that will hold the waveform settings.
-        self.waveform_settings = WaveformSettingsFrame(self)
-        self.waveform_settings.grid(row=1, column=0, sticky=tk.NSEW, padx=5, pady=5)
+        canvas.create_window((0, 0), window=self.feature_view_frame, anchor="nw")
 
+        canvas.configure(xscrollcommand=scrollbar.set)
 
-class WaveformSettingsFrame(ttk.Labelframe):
-    """This class is the frame that holds the waveform settings."""
+        canvas.pack(side="top", fill="both", expand=True)
+        scrollbar.pack(side="bottom", fill="x")
 
-    def __init__(self, wav_view, *args, **kwargs):
-        """Initialize the WaveformSettingsFrame class.
+        separator = ttk.Separator(content_frame)
+        separator.grid(row=4, column=0, sticky=tk.NSEW, padx=3, pady=3)
+        self.inputs["content"] = tk.Text(content_frame, width=100, height=10)
+        self.inputs["content"].grid(row=5, column=0, sticky=tk.NSEW, padx=10, pady=3)
 
-        Parameters
-        ----------
-        wav_view : tk.Frame
-            The frame that will hold the waveform settings.
-        *args : tuple
-            Variable length argument list.
-        **kwargs : dict
-            Arbitrary keyword arguments.
-        """
-        # Init Frame
-        text_label = "Settings"
-        ttk.Labelframe.__init__(self, wav_view, text=text_label, *args, **kwargs)
-
-        # Formatting
-        tk.Grid.columnconfigure(self, "all", weight=1)
-        tk.Grid.rowconfigure(self, "all", weight=1)
+        #: dict: Dictionary of buttons
+        self.buttons = {}
+        button_frame = ttk.Frame(content_frame)
+        button_frame.grid(row=6, column=0, sticky=tk.NSEW)
+        self.buttons["preview"] = ttk.Button(button_frame, text="Preview")
+        self.buttons["preview"].grid(row=0, column=0, padx=3, pady=3)
+        if self.add_new_list_flag:
+            self.buttons["add"] = ttk.Button(button_frame, text="Add")
+            self.buttons["add"].grid(row=0, column=1, padx=3, pady=3)
+        else:
+            self.buttons["confirm"] = ttk.Button(button_frame, text="Confirm")
+            self.buttons["confirm"].grid(row=0, column=1, padx=3, pady=3)
+        self.buttons["cancel"] = ttk.Button(button_frame, text="Cancel")
+        self.buttons["cancel"].grid(row=0, column=2, sticky=tk.SE, padx=3, pady=3)
 
-        #: dict: The dictionary that holds the widgets.
-        self.inputs = {}
+class FeatureListFrame(ttk.Frame):
+    """Feature list graph frame"""
+    def __init__(self, root, *args, width=800, height=200, **kwargs):
+        super().__init__(root)
 
-        self.inputs["sample_rate"] = LabelInput(
-            parent=self,
-            label="Sample rate",
-            input_class=ttk.Spinbox,
-            input_var=tk.IntVar(),
-            input_args={"from_": 1, "to": 2**16 - 1, "increment": 1, "width": 5},
-        )
-        self.inputs["sample_rate"].grid(row=0, column=0, sticky=tk.NSEW, padx=3, pady=3)
-
-        self.inputs["waveform_template"] = LabelInput(
-            parent=self,
-            label="Waveform Template",
-            input_class=ttk.Combobox,
-            input_var=tk.StringVar(),
-            input_args={"width": 20},
-        )
-        self.inputs["waveform_template"].grid(
-            row=0, column=1, sticky=tk.NSEW, padx=3, pady=3
+        scroll_frame = ttk.Frame(self)
+        scroll_frame.grid(row=0, column=0, sticky=tk.NSEW)
+        canvas = tk.Canvas(scroll_frame, width=width, height=height)
+        scrollbar = ttk.Scrollbar(scroll_frame, orient="horizon", command=canvas.xview)
+        self.feature_view_frame = ttk.Frame(canvas)
+
+        self.feature_view_frame.bind(
+            "<Configure>", lambda e: canvas.configure(scrollregion=canvas.bbox("all"))
         )
 
-    def get_variables(self):
-        """Function to get the variables.
+        canvas.create_window((0, 0), window=self.feature_view_frame, anchor="nw")
 
-        Returns
-        -------
-        variables : dict
-            The dictionary that holds the variables.
-        """
-        variables = {}
-        for key, widget in self.inputs.items():
-            variables[key] = widget.get()
-        return variables
+        canvas.configure(xscrollcommand=scrollbar.set)
 
-    def get_widgets(self):
-        """Function to get the widgets.
+        canvas.pack(side="top", fill="both", expand=True)
+        scrollbar.pack(side="bottom", fill="x")
+
+        self.content = tk.Text(self, width=100, height=5)
+        self.content.grid(row=2, column=0, sticky=tk.NSEW, padx=10, pady=3)
 
-        Returns
-        -------
-        self.inputs : dict
-            The dictionary that holds the widgets.
-        """
-        return self.inputs
 
 
-class MetricsFrame(ttk.Labelframe):
-    """This class is the frame that holds the image metrics."""
+class FeatureAdvancedSettingPopup:
+    """Feature Advanced Setting Popup Widget"""
 
-    def __init__(self, cam_view, *args, **kwargs):
-        """Initialize the MetricsFrame class.
+    def __init__(
+        self,
+        root,
+        *args,
+        features=[],
+        feature_name="",
+        args_name=[],
+        args_default_value=[],
+        **kwargs
+    ):
+        """Initialize the Feature Advanced Setting Popup Widget
 
         Parameters
         ----------
-        cam_view : tk.Frame
-            The frame that will hold the image metrics.
-        *args : tuple
-            Variable length argument list.
-        **kwargs : dict
-            Arbitrary keyword arguments.
-        """
-        # Init Labelframe
-        text_label = "Image Metrics"
-        ttk.Labelframe.__init__(self, cam_view, text=text_label, *args, **kwargs)
-
-        # Formatting
-        tk.Grid.columnconfigure(self, "all", weight=1)
-        tk.Grid.rowconfigure(self, "all", weight=1)
-
-        # Dictionary for widgets
-        #: dict: The dictionary that holds the widgets.
-        self.inputs = {}
-
-        # Labels and names
-        #: list: The list of labels for the widgets.
-        self.labels = ["Frames to Avg", "Image Max Counts", "Channel"]
-        #: list: The list of names for the widgets.
-        self.names = ["Frames", "Image", "Channel"]
-
-        # Loop for widgets
-        for i in range(len(self.labels)):
-            if i == 0:
-                self.inputs[self.names[i]] = LabelInput(
-                    parent=self,
-                    label=self.labels[i],
-                    input_class=ttk.Spinbox,
-                    input_var=tk.IntVar(),
-                    input_args={"from_": 1, "to": 32, "increment": 1, "width": 5},
-                    label_pos="top",
-                )
-                self.inputs[self.names[i]].grid(
-                    row=i, column=0, sticky=tk.NSEW, padx=5, pady=3
-                )
-            if i > 0:
-                self.inputs[self.names[i]] = LabelInput(
-                    parent=self,
-                    label=self.labels[i],
-                    input_class=ttk.Entry,
-                    input_var=tk.IntVar(),
-                    input_args={"width": 5, "state": "disabled"},
-                    label_pos="top",
-                )
-                self.inputs[self.names[i]].grid(
-                    row=i, column=0, sticky=(tk.NSEW), padx=5, pady=3
-                )
-                self.inputs[self.names[i]].configure(width=5)
-
-    def get_variables(self):
-        """This function returns a dictionary of all the variables that are tied to
-        each  widget name.
-
-        The key is the widget name, value is the variable associated.
-
-        Returns
-        -------
-        variables : dict
-            The dictionary that holds the variables.
-        """
-        variables = {}
-        for key, widget in self.inputs.items():
-            variables[key] = widget.get()
-        return variables
-
-    def get_widgets(self):
-        """This function returns the dictionary that holds the widgets.
-
-        The key is the widget name, value is the LabelInput class that has all the data.
+        root : tk.Tk
+            Root window of the application
+        features : list
+            List of features
+        feature_name : str
+            Name of the feature
+        args_name : list
+            List of arguments name
+        args_default_value : list
+            List of arguments default value
+        """
+        # Creating popup window with this name and size/placement,
+        # PopUp is a Toplevel window
+        #: PopUp: Popup window
+        self.popup = PopUp(
+            root, kwargs["title"], "+320+180", top=False, transient=False
+        )
+        # Change background of popup window to white
+        self.popup.configure(bg="white")
 
-        Returns
-        -------
-        self.inputs : dict
-            The dictionary that holds the widgets.
-        """
-        return self.inputs
+        # Creating content frame
+        content_frame = self.popup.get_frame()
 
+        #: dict: Dictionary of input widgets
+        self.inputs = {}
+        #: dict: Dictionary of buttons
+        self.buttons = {}
 
-class IntensityFrame(ttk.Labelframe):
-    """This class is the frame that holds the intensity controls."""
+        self.feature_name_widget = LabelInput(
+            parent=content_frame,
+            label="Feature Name",
+            label_args={"width": 20},
+            input_class=ttk.Combobox,
+            input_var=tk.StringVar(),
+            input_args={"width": 30, "state": "readonly"},
+        )
+        self.feature_name_widget.grid(row=0, column=0, sticky=tk.NSEW, padx=3, pady=3)
+        self.feature_name_widget.set(feature_name)
+        self.feature_name_widget.set_values(features)
+
+        separator = ttk.Separator(content_frame)
+        separator.grid(row=1, column=0, sticky=tk.NSEW, pady=10)
+
+        #: ttk.Frame: Parameter frame
+        self.parameter_frame = ttk.Frame(content_frame)
+        self.parameter_frame.grid(row=2, column=0, sticky=tk.NSEW, padx=30, pady=30)
+        #: dict: Dictionary of argument frames
+        self.arg_frames = {}
 
-    def __init__(self, cam_view, *args, **kwargs):
-        """Initialize the IntensityFrame class.
+    def build_widgets(self, args_name, parameter_config=None):
+        """Build widgets for the popup
 
-         Parameters
+        Parameters
         ----------
-        cam_view : tk.Frame
-            The frame that will hold the intensity controls.
-        *args : tuple
-            Variable length argument list.
-        **kwargs : dict
-            Arbitrary keyword arguments.
+        args_name : list
+            List of arguments name
+        parameter_config : dict
+            Dictionary of parameter configuration
         """
-        # Init Frame
-        text_label = "LUT"
-        ttk.Labelframe.__init__(self, cam_view, text=text_label, *args, **kwargs)
-
-        # Formatting
-        tk.Grid.columnconfigure(self, "all", weight=1)
-        tk.Grid.rowconfigure(self, "all", weight=1)
-
-        #: dict: The dictionary that holds the widgets.
+        #: dict: Dictionary of input widgets
         self.inputs = {}
+        #: dict: Dictionary of buttons
+        self.buttons = {}
+        #: dict: Dictionary of argument frames
+        self.arg_frames = {}
+
+        for child in self.parameter_frame.winfo_children():
+            child.destroy()
+        self.save_button = None
+
+        row_id = 0
+        for _, arg_name in enumerate(args_name):
+            # ref_value, value, delete button, load button
+            self.inputs[arg_name] = []
+            arg_label = ttk.Label(self.parameter_frame, text=arg_name + ":")
+            arg_label.grid(row=row_id, column=0, sticky=tk.NW)
+            row_id += 1
+            arg_frame = ttk.Frame(self.parameter_frame)
+            arg_frame.grid(row=row_id, column=0, sticky=tk.NSEW)
+            row_id += 1
+            self.arg_frames[arg_name] = arg_frame
+            if parameter_config is not None and arg_name in parameter_config:
+                for k, v in parameter_config[arg_name].items():
+                    self.add_new_row(arg_name, k, v)
+            add_button = ttk.Button(self.parameter_frame, text="Add")
+            add_button.grid(row=row_id, column=0, sticky=tk.NW, padx=3, pady=3)
+            self.buttons[arg_name] = add_button
+            row_id += 1
+            separator = ttk.Separator(self.parameter_frame)
+            separator.grid(row=row_id, column=0, sticky=tk.NSEW, pady=10)
+            row_id += 1
+
+        if len(args_name) > 1:
+            save_button = ttk.Button(self.parameter_frame, text="Save")
+            save_button.grid(row=row_id, column=0, sticky=tk.NE, padx=3, pady=3)
+            #: ttk.Button: Save button
+            self.save_button = save_button
 
-        #: list: The list of LUTs for the image display.
-        self.color_labels = [
-            "Gray",
-            "Gradient",
-            "Rainbow",
-            "SNR",
-        ]
-
-        #: list: The list of maplotlib LUT names.
-        self.color_values = [
-            "gist_gray",
-            "plasma",
-            "afmhot",
-            "RdBu_r",
-        ]
-
-        #: tk.StringVar: The variable that holds the LUT.
-        self.color = tk.StringVar()
-        for i in range(len(self.color_labels)):
-            self.inputs[self.color_labels[i]] = LabelInput(
-                parent=self,
-                label=self.color_labels[i],
-                input_class=ttk.Radiobutton,
-                input_var=self.color,
-                input_args={"value": self.color_values[i]},
-            )
-            self.inputs[self.color_labels[i]].grid(
-                row=i, column=0, sticky=tk.NSEW, pady=3
-            )
+    def add_new_row(self, arg_name, k="", v=""):
+        """Add new row to the popup
 
-        #: tk.BooleanVar: The variable that holds the flip xy flag.
-        self.transpose = tk.BooleanVar()
-
-        #: str: The name of the flip xy flag.
-        self.trans = "Flip XY"
-        self.inputs[self.trans] = LabelInput(
-            parent=self,
-            label=self.trans,
-            input_class=ttk.Checkbutton,
-            input_var=self.transpose,
-        )
-        self.inputs[self.trans].grid(
-            row=len(self.color_labels), column=0, sticky=tk.NSEW, pady=3
-        )
-
-        #: tk.BooleanVar: The variable that holds the autoscale flag.
-        self.autoscale = tk.BooleanVar()
-
-        #: str: The name of the autoscale flag.
-        self.auto = "Autoscale"
-
-        #: list: The list of min and max counts.
-        self.minmax = ["Min Counts", "Max Counts"]
-
-        #: list: The list of min and max names.
-        self.minmax_names = ["Min", "Max"]
-        self.inputs[self.auto] = LabelInput(
-            parent=self,
-            label=self.auto,
-            input_class=ttk.Checkbutton,
-            input_var=self.autoscale,
-        )
-        self.inputs[self.auto].grid(
-            row=len(self.color_labels) + 1, column=0, sticky=tk.NSEW, pady=3
-        )
-
-        # Max and Min Counts
-        for i in range(len(self.minmax)):
-            self.inputs[self.minmax_names[i]] = LabelInput(
-                parent=self,
-                label=self.minmax[i],
-                input_class=ttk.Spinbox,
-                input_var=tk.IntVar(),
-                input_args={"from_": 1, "to": 2**16 - 1, "increment": 1, "width": 5},
-            )
-            self.inputs[self.minmax_names[i]].grid(
-                row=i + len(self.color_labels) + 2,
-                column=0,
-                sticky=tk.NSEW,
-                padx=3,
-                pady=3,
-            )
-
-    def get_variables(self):
-        """This function returns a dictionary of all the variables that are tied to
-        each  widget name.
-
-        The key is the widget name, value is the variable associated.
-
-        Returns
-        -------
-        variables : dict
-            The dictionary that holds the variables.
-        """
-        variables = {}
-        for key, widget in self.inputs.items():
-            variables[key] = widget.get()
-        return variables
+        Parameters
+        ----------
+        arg_name : str
+            Name of the argument
+        k : str
+            Name of the function
+        v : str
+            Value of the function
+        """
+        r = len(self.inputs[arg_name])
+        arg_frame = self.arg_frames[arg_name]
+        ref_value_entry = LabelInput(
+            parent=arg_frame,
+            label="Function Name",
+            input_class=ttk.Entry,
+            input_var=tk.StringVar(),
+            input_args={"width": 50},
+        )
+        ref_value_entry.grid(row=r, column=1, sticky=tk.NSEW, padx=3, pady=3)
+        ref_value_entry.set(k)
+        value_entry = LabelInput(
+            parent=arg_frame,
+            label="Value",
+            input_class=ttk.Entry,
+            input_var=tk.StringVar(),
+            input_args={"width": 50},
+        )
+        value_entry.grid(row=r, column=2, sticky=tk.NSEW, padx=3, pady=3)
+        value_entry.set(v)
+        load_button = ttk.Button(arg_frame, text="Load")
+        load_button.grid(row=r, column=3, sticky=tk.NSEW, padx=3, pady=3)
+        delete_button = ttk.Button(arg_frame, text="Delete")
+        delete_button.grid(row=r, column=4, sticky=tk.NSEW, padx=3, pady=3)
+        delete_button.config(command=self.delete_row(arg_name, r))
+        self.inputs[arg_name].append(
+            (ref_value_entry, value_entry, load_button, delete_button)
+        )
 
-    def get_widgets(self):
-        """This function returns the dictionary that holds the widgets.
+    def delete_row(self, arg_name, r):
+        """Delete row from the popup
 
-        The key is the widget name, value is the LabelInput class that has all the data.
+        Parameters
+        ----------
+        arg_name : str
+            Name of the argument
+        r : int
+            Row number
+        """
+
+        def func():
+            """Function to delete row from the popup
+
+            Returns
+            -------
+            func
+                Function to delete row from the popup
+            """
+            for w in self.inputs[arg_name][r]:
+                w.grid_remove()
+            self.inputs[arg_name][r] = None
 
-        Returns
-        -------
-        self.inputs : dict
-            The dictionary that holds the widgets.
-        """
-        return self.inputs
+        return func
```

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greydown.png` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greydown.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greydown_disabled.png` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greydown_disabled.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyleft.png` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyleft.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyleft_disabled.png` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyleft_disabled.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyright.png` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyright.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyright_disabled.png` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyright_disabled.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyup.png` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyup.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/greyup_disabled.png` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/images/greyup_disabled.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/images/wa_right.png` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/images/wa_right.png`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/menus.py` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/menus.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/multiposition_tab.py` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/multiposition_tab.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/settings_notebook.py` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/settings_notebook.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/main_window_content/stage_tab.py` & `navigate_micro-0.0.6/src/navigate/view/main_window_content/stage_tab.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
         #: list: List of frames for the position entries.
         self.frame_back_list = []
         for i in range(len(entry_names)):
             self.inputs[entry_names[i]] = LabelInput(
                 parent=self,
                 label=entry_labels[i],
                 input_class=ValidatedEntry,
-                input_var=tk.DoubleVar(),
+                input_var=tk.StringVar(),
                 input_args={
                     "required": True,
                     "precision": 0.1,
                     "width": 6,
                     "takefocus": False,
                 },
             )
```

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/acquire_popup.py` & `navigate_micro-0.0.6/src/navigate/view/popups/acquire_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/adaptiveoptics_popup.py` & `navigate_micro-0.0.6/src/navigate/view/popups/adaptiveoptics_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/autofocus_setting_popup.py` & `navigate_micro-0.0.6/src/navigate/view/popups/autofocus_setting_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/camera_map_setting_popup.py` & `navigate_micro-0.0.6/src/navigate/view/popups/camera_map_setting_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/camera_view_popup_window.py` & `navigate_micro-0.0.6/src/navigate/view/popups/camera_view_popup_window.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/feature_list_popup.py` & `navigate_micro-0.0.6/src/navigate/controller/configurator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2021-2022  The University of Texas Southwestern Medical Center.
 # All rights reserved.
-
 # Redistribution and use in source and binary forms, with or without
-# modification, are permitted for academic and research use only (subject to the
-# limitations in the disclaimer below) provided that the following conditions are met:
+# modification, are permitted for academic and research use only
+# (subject to the limitations in the disclaimer below)
+# provided that the following conditions are met:
 
 #      * Redistributions of source code must retain the above copyright notice,
 #      this list of conditions and the following disclaimer.
 
 #      * Redistributions in binary form must reproduce the above copyright
 #      notice, this list of conditions and the following disclaimer in the
 #      documentation and/or other materials provided with the distribution.
@@ -24,478 +24,421 @@
 # CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 # BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 # IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
-#
 
 # Standard Library Imports
 import tkinter as tk
-from tkinter import ttk
-
-# Local Imports
-from navigate.view.custom_widgets.popup import PopUp
-from navigate.view.custom_widgets.LabelInputWidgetFactory import LabelInput
+from time import sleep
+from tkinter import filedialog, messagebox
 
+# Third Party Imports
 
-class FeatureIcon(ttk.Button):
-    """Feature Icon Widget"""
-
-    def __init__(self, parent, feature_name="", set_bg=False):
-        """Initialize the Feature Icon Widget
-
-        Parameters
-        ----------
-        parent : tk.Frame
-            Parent frame of the widget
-        feature_name : str
-            Name of the feature
-        """
-        ttk.Button.__init__(self, parent, text=feature_name)
-
-        # Create a style
-        style = ttk.Style()
-        style.configure("Custom.TButton", background="red")
-        if set_bg:
-            self.configure(style="Custom.TButton")
-        
-        self.configure(padding=(10, 20))
+# Local Imports
+from navigate.view.configurator_application_window import ConfigurationAssistantWindow
+from navigate.view.configurator_application_window import (
+    MicroscopeTab,
+    MicroscopeWindow,
+)
+from navigate.config.configuration_database import (
+    hardwares_dict,
+    hardwares_config_name_dict,
+)
+from navigate.tools.file_functions import load_yaml_file
+
+# Logger Setup
+import logging
+
+p = __name__.split(".")[1]
+logger = logging.getLogger(p)
 
 
-class FeatureConfigPopup:
-    """Feature Config Popup Widget"""
+class Configurator:
+    """Navigate Configurator"""
 
-    def __init__(
-        self,
-        root,
-        *args,
-        features=[],
-        feature_name="",
-        args_name=[],
-        args_value=[],
-        **kwargs
-    ):
-        """Initialize the Feature Config Popup Widget
+    def __init__(self, root, splash_screen):
+        """Initiates the configurator application window.
 
         Parameters
         ----------
         root : tk.Tk
-            Root window of the application
-        *args : list
-            List of arguments
-        features : list
-            List of features
-        feature_name : str
-            Name of the feature
-        args_name : list
-            List of arguments name
-        args_value : list
-            List of arguments value
+            The main window of the application
+        splash_screen : SplashScreen
+            The splash screen of the application
         """
-        # Creating popup window with this name and size/placement,
+        self.root = root
 
-        #: PopUp: Popup window
-        self.popup = PopUp(
-            root, kwargs["title"], "+320+180", top=False, transient=False
-        )
-
-        # Change background of popup window to white
-        self.popup.configure(bg="white")
-
-        # Creating content frame
-        content_frame = self.popup.get_frame()
-
-        #: list: List of input widgets
-        self.inputs = []
-
-        #: LabelInput: Feature name widget
-        self.feature_name_widget = LabelInput(
-            parent=content_frame,
-            label="Feature Name",
-            label_args={"width": 20},
-            input_class=ttk.Combobox,
-            input_var=tk.StringVar(),
-            input_args={"width": 30, "state": "readonly"},
-        )
-        self.feature_name_widget.grid(row=0, column=0, sticky=tk.NSEW, padx=3, pady=3)
-        self.feature_name_widget.set(feature_name)
-        self.feature_name_widget.set_values(features)
-
-        separator = ttk.Separator(content_frame)
-        separator.grid(row=1, column=0, sticky=tk.NSEW, pady=10)
-
-        #: ttk.Frame: Parameter frame
-        self.parameter_frame = ttk.Frame(content_frame)
-        self.parameter_frame.grid(row=2, column=0, sticky=tk.NSEW, padx=30, pady=30)
-
-        row = 3
-        if "true" in kwargs:
-            self.preview_btn_true = ttk.Button(content_frame, text="Preview (True)")
-            self.preview_btn_true.grid(row=row, column=0, sticky=tk.NSEW)
-            separator = ttk.Separator(content_frame)
-            separator.grid(row=row+1, column=0, sticky=tk.NSEW, pady=(0,10))
-            self.feature_list_true_frame = FeatureListFrame(content_frame)
-            self.feature_list_true_frame.grid(row=row+2, column=0, sticky=tk.NSEW)
-            row += 3
-
-        if "false" in kwargs:
-            self.preview_btn_false = ttk.Button(content_frame, text="Preview (False)")
-            self.preview_btn_false.grid(row=row, column=0, sticky=tk.NSEW)
-            separator = ttk.Separator(content_frame)
-            separator.grid(row=row+1, column=0, sticky=tk.NSEW, pady=(0,10))
-            self.feature_list_false_frame = FeatureListFrame(content_frame)
-            self.feature_list_false_frame.grid(row=row+2, column=0, sticky=tk.NSEW)
-
-        self.build_widgets(args_name, args_value, kwargs.get("parameter_config", {}))
-
-    def build_widgets(self, args_name, args_value, parameter_config=None):
-        """Build widgets for the popup
-
-        Parameters
-        ----------
-        args_name : list
-            List of arguments name
-        args_value : list
-            List of arguments value
-        parameter_config : dict
-            Dictionary of parameter configuration
-        """
-        #: list: List of input widgets
-        self.inputs = []
-        #: list: List of input widgets type
-        self.inputs_type = []
-
-        for child in self.parameter_frame.winfo_children():
-            child.destroy()
-
-        for i, arg_name in enumerate(args_name):
-            arg_input_class = ttk.Entry
-            arg_input_var = tk.StringVar
-            if type(args_value[i]) is bool:
-                arg_input_class = ttk.Combobox
-                values = ["True", "False"]
-            elif parameter_config is not None and arg_name in parameter_config:
-                arg_input_class = ttk.Combobox
-                values = list(parameter_config[arg_name].keys())
-
-            temp = LabelInput(
-                parent=self.parameter_frame,
-                label=arg_name + ":",
-                label_args={"padding": (2, 5, 5, 0), "width": 20},
-                input_class=arg_input_class,
-                input_var=arg_input_var(),
-                input_args={"width": 30},
+        # Show the splash screen for 1 second and then destroy it.
+        sleep(1)
+        splash_screen.destroy()
+        self.root.deiconify()
+        self.view = ConfigurationAssistantWindow(root)
+        self.view.microscope_window = MicroscopeWindow(
+            self.view.microscope_frame, self.view.root
+        )
+
+        self.view.top_window.add_button.config(command=self.add_microscope)
+        self.view.top_window.new_button.config(command=self.new_configuration)
+        self.view.top_window.load_button.config(command=self.load_configuration)
+        self.view.top_window.save_button.config(command=self.save)
+        self.view.top_window.cancel_button.config(command=self.on_cancel)
+        self.microscope_id = 0
+        self.create_config_window(0)
+
+        print(
+            "WARNING: The Configuration Assistant is not fully implemented. "
+            "Users are still required to manually configure their system."
+        )
+
+    def on_cancel(self):
+        """Closes the window and exits the program"""
+        self.root.destroy()
+        exit()
+
+    def add_microscope(self):
+        """Add a new microscope tab"""
+        self.microscope_id += 1
+        self.create_config_window(self.microscope_id)
+
+    def delete_microscopes(self):
+        """Delete all microscopes"""
+        # delete microscopes
+        for tab_id in self.view.microscope_window.tabs():
+            self.view.microscope_window.forget(tab_id)
+        self.view.microscope_window.tab_list = []
+        self.microscope_id = 0
+
+    def new_configuration(self):
+        """Create new configurations"""
+        self.delete_microscopes()
+        self.create_config_window(self.microscope_id)
+
+    def save(self):
+        """Save configuration file"""
+
+        def set_value(temp_dict, key_list, value):
+            """Set value
+
+            Parameters
+            ----------
+            temp_dict: dict
+                Target dictionary
+            key_list: list
+                keyword list
+            value: any
+                value of the item
+            """
+            if type(key_list) is list:
+                for i in range(len(key_list) - 1):
+                    k = key_list[i]
+                    temp_dict[k] = temp_dict.get(k, {})
+                    temp_dict = temp_dict[k]
+            temp_dict[key_list[-1]] = value
+
+        filename = filedialog.asksaveasfilename(
+            defaultextension=".yml", filetypes=[("Yaml file", "*.yml *.yaml")]
+        )
+        if not filename:
+            return
+        # warning_info
+        warning_info = {}
+        config_dict = {}
+        for tab_index in self.view.microscope_window.tabs():
+            microscope_name = self.view.microscope_window.tab(tab_index, "text")
+            microscope_tab = self.view.microscope_window.nametowidget(tab_index)
+            microscope_dict = {}
+            config_dict[microscope_name] = microscope_dict
+            for hardware_tab_index in microscope_tab.tabs():
+                hardware_name = microscope_tab.tab(hardware_tab_index, "text")
+                hardware_tab = microscope_tab.nametowidget(hardware_tab_index)
+                hardware_dict = {}
+                microscope_dict[
+                    hardwares_config_name_dict.get(hardware_name, hardware_name)
+                ] = hardware_dict
+                for variable_list in hardware_tab.variables_list:
+                    if variable_list is None:
+                        continue
+                    variables, value_dict, ref, format = variable_list
+                    if format is None:
+                        format = ""
+                    temp_dict = hardware_dict
+                    if ref is not None:
+                        if format.startswith("list"):
+                            hardware_dict[ref] = hardware_dict.get(ref, [])
+                            temp_dict = {}
+                            hardware_dict[ref].append(temp_dict)
+                        elif format.startswith("item"):
+                            format_list = format.split(";")
+                            ref_list = ref.split(";")
+                            for i, format in enumerate(format_list):
+                                ref = ref_list[i]
+                                hardware_dict[ref] = hardware_dict.get(ref, {})
+                                temp_dict = hardware_dict[ref]
+                                k_idx = format[
+                                    format.index("(") + 1 : format.index(",")
+                                ].strip()
+                                v_idx = format[
+                                    format.index(",") + 1 : format.index(")")
+                                ].strip()
+                                k = variables[k_idx].get()
+                                if k.strip() == "":
+                                    warning_info[hardware_name] = True
+                                    print(
+                                        f"Notice: {hardware_name} has an empty value {ref}! Please double check if it's okay!"
+                                    )
+                                    
+                                if k_idx in value_dict:
+                                    k = value_dict[k_idx][v]
+                                v = variables[v_idx].get()
+                                if v_idx in value_dict:
+                                    v = value_dict[v_idx][v]
+                                temp_dict[k] = v
+                            continue
+                        else:
+                            temp_dict = {}
+                            hardware_dict[ref] = hardware_dict.get("ref", temp_dict)
+                    for k, var in variables.items():
+                        try:
+                            if k in value_dict:
+                                v = value_dict[k][var.get()]
+                            else:
+                                v = var.get()
+                        except tk._tkinter.TclError:
+                            v = ""
+                            print(
+                                f"Notice: {hardware_name} has an empty value {k}! Please double check!"
+                            )
+                            warning_info[hardware_name] = True
+                        set_value(temp_dict, k.split("/"), v)
+
+        self.write_to_yaml(config_dict, filename)
+        # display warning
+        if warning_info:
+            messagebox.showwarning(
+                title="Configuration",
+                message=f"There are empty value(s) with {', '.join(warning_info.keys())}. Please double check!"
             )
 
-            self.inputs.append(temp)
-            self.inputs_type.append(type(args_value[i]))
-            temp.grid(row=i + 2, column=0, sticky=tk.NSEW, padx=30, pady=10)
-            if arg_input_class is ttk.Combobox:
-                temp.set_values(values)
-                temp.widget.config(state="readonly")
-            temp.set(str(args_value[i]))
-
-    def get_widgets(self):
-        """Get widgets
-
-        Returns
-        -------
-        list
-            List of input widgets
-        """
-        return self.inputs
-
-
-class FeatureListPopup:
-    """Feature List Popup Widget"""
-
-    def __init__(self, root, *args, **kwargs):
-        """Initialize the Feature List Popup Widget
-
-        Parameters
-        ----------
-        root : tk.Tk
-            Root window of the application
-        *args : list
-            List of arguments
-        **kwargs : dict
-            Dictionary of keyword arguments
-        """
-        # Creating popup window with this name and size/placement,
-        # PopUp is a Toplevel window
-        #: PopUp: Popup window
-        self.popup = PopUp(
-            root, kwargs["title"], "+320+180", top=False, transient=False
-        )
-        # Change background of popup window to white
-        self.popup.configure(bg="white")
-        #: bool: Flag to indicate if the popup is for adding new list
-        self.add_new_list_flag = False
-        if kwargs["title"].startswith("Add"):
-            self.add_new_list_flag = True
-
-        # Creating content frame
-        content_frame = self.popup.get_frame()
-
-        #: dict: Dictionary of input widgets
-        self.inputs = {}
-        self.inputs["feature_list_name"] = LabelInput(
-            parent=content_frame,
-            label="Feature List Name",
-            input_class=ttk.Entry,
-            input_var=tk.StringVar(),
-            input_args={"width": 50},
-        )
-
-        self.inputs["feature_list_name"].grid(
-            row=0, column=0, sticky=tk.NSEW, padx=3, pady=3
-        )
-
-        separator = ttk.Separator(content_frame)
-        separator.grid(row=2, column=0, sticky=tk.NSEW, padx=3, pady=3)
-
-        scroll_frame = ttk.Frame(content_frame)
-        scroll_frame.grid(row=3, column=0, sticky=tk.NSEW)
-        canvas = tk.Canvas(scroll_frame, width=800, height=350)
-        scrollbar = ttk.Scrollbar(scroll_frame, orient="horizon", command=canvas.xview)
-        self.feature_view_frame = ttk.Frame(canvas)
-
-        self.feature_view_frame.bind(
-            "<Configure>", lambda e: canvas.configure(scrollregion=canvas.bbox("all"))
-        )
-
-        canvas.create_window((0, 0), window=self.feature_view_frame, anchor="nw")
-
-        canvas.configure(xscrollcommand=scrollbar.set)
-
-        canvas.pack(side="top", fill="both", expand=True)
-        scrollbar.pack(side="bottom", fill="x")
-
-        separator = ttk.Separator(content_frame)
-        separator.grid(row=4, column=0, sticky=tk.NSEW, padx=3, pady=3)
-        self.inputs["content"] = tk.Text(content_frame, width=100, height=10)
-        self.inputs["content"].grid(row=5, column=0, sticky=tk.NSEW, padx=10, pady=3)
-
-        #: dict: Dictionary of buttons
-        self.buttons = {}
-        button_frame = ttk.Frame(content_frame)
-        button_frame.grid(row=6, column=0, sticky=tk.NSEW)
-        self.buttons["preview"] = ttk.Button(button_frame, text="Preview")
-        self.buttons["preview"].grid(row=0, column=0, padx=3, pady=3)
-        if self.add_new_list_flag:
-            self.buttons["add"] = ttk.Button(button_frame, text="Add")
-            self.buttons["add"].grid(row=0, column=1, padx=3, pady=3)
-        else:
-            self.buttons["confirm"] = ttk.Button(button_frame, text="Confirm")
-            self.buttons["confirm"].grid(row=0, column=1, padx=3, pady=3)
-        self.buttons["cancel"] = ttk.Button(button_frame, text="Cancel")
-        self.buttons["cancel"].grid(row=0, column=2, sticky=tk.SE, padx=3, pady=3)
-
-class FeatureListFrame(ttk.Frame):
-    """Feature list graph frame"""
-    def __init__(self, root, *args, width=800, height=200, **kwargs):
-        super().__init__(root)
-
-        scroll_frame = ttk.Frame(self)
-        scroll_frame.grid(row=0, column=0, sticky=tk.NSEW)
-        canvas = tk.Canvas(scroll_frame, width=width, height=height)
-        scrollbar = ttk.Scrollbar(scroll_frame, orient="horizon", command=canvas.xview)
-        self.feature_view_frame = ttk.Frame(canvas)
-
-        self.feature_view_frame.bind(
-            "<Configure>", lambda e: canvas.configure(scrollregion=canvas.bbox("all"))
-        )
-
-        canvas.create_window((0, 0), window=self.feature_view_frame, anchor="nw")
-
-        canvas.configure(xscrollcommand=scrollbar.set)
-
-        canvas.pack(side="top", fill="both", expand=True)
-        scrollbar.pack(side="bottom", fill="x")
-
-        self.content = tk.Text(self, width=100, height=5)
-        self.content.grid(row=2, column=0, sticky=tk.NSEW, padx=10, pady=3)
-
-
-
-class FeatureAdvancedSettingPopup:
-    """Feature Advanced Setting Popup Widget"""
-
-    def __init__(
-        self,
-        root,
-        *args,
-        features=[],
-        feature_name="",
-        args_name=[],
-        args_default_value=[],
-        **kwargs
-    ):
-        """Initialize the Feature Advanced Setting Popup Widget
-
-        Parameters
-        ----------
-        root : tk.Tk
-            Root window of the application
-        features : list
-            List of features
-        feature_name : str
-            Name of the feature
-        args_name : list
-            List of arguments name
-        args_default_value : list
-            List of arguments default value
-        """
-        # Creating popup window with this name and size/placement,
-        # PopUp is a Toplevel window
-        #: PopUp: Popup window
-        self.popup = PopUp(
-            root, kwargs["title"], "+320+180", top=False, transient=False
-        )
-        # Change background of popup window to white
-        self.popup.configure(bg="white")
-
-        # Creating content frame
-        content_frame = self.popup.get_frame()
-
-        #: dict: Dictionary of input widgets
-        self.inputs = {}
-        #: dict: Dictionary of buttons
-        self.buttons = {}
-
-        self.feature_name_widget = LabelInput(
-            parent=content_frame,
-            label="Feature Name",
-            label_args={"width": 20},
-            input_class=ttk.Combobox,
-            input_var=tk.StringVar(),
-            input_args={"width": 30, "state": "readonly"},
-        )
-        self.feature_name_widget.grid(row=0, column=0, sticky=tk.NSEW, padx=3, pady=3)
-        self.feature_name_widget.set(feature_name)
-        self.feature_name_widget.set_values(features)
-
-        separator = ttk.Separator(content_frame)
-        separator.grid(row=1, column=0, sticky=tk.NSEW, pady=10)
-
-        #: ttk.Frame: Parameter frame
-        self.parameter_frame = ttk.Frame(content_frame)
-        self.parameter_frame.grid(row=2, column=0, sticky=tk.NSEW, padx=30, pady=30)
-        #: dict: Dictionary of argument frames
-        self.arg_frames = {}
-
-    def build_widgets(self, args_name, parameter_config=None):
-        """Build widgets for the popup
+    def write_to_yaml(self, config, filename):
+        """write yaml file
 
         Parameters
         ----------
-        args_name : list
-            List of arguments name
-        parameter_config : dict
-            Dictionary of parameter configuration
+        config: dict
+            configuration dictionary
+        filename: str
+            yaml file name
         """
-        #: dict: Dictionary of input widgets
-        self.inputs = {}
-        #: dict: Dictionary of buttons
-        self.buttons = {}
-        #: dict: Dictionary of argument frames
-        self.arg_frames = {}
-
-        for child in self.parameter_frame.winfo_children():
-            child.destroy()
-        self.save_button = None
-
-        row_id = 0
-        for _, arg_name in enumerate(args_name):
-            # ref_value, value, delete button, load button
-            self.inputs[arg_name] = []
-            arg_label = ttk.Label(self.parameter_frame, text=arg_name + ":")
-            arg_label.grid(row=row_id, column=0, sticky=tk.NW)
-            row_id += 1
-            arg_frame = ttk.Frame(self.parameter_frame)
-            arg_frame.grid(row=row_id, column=0, sticky=tk.NSEW)
-            row_id += 1
-            self.arg_frames[arg_name] = arg_frame
-            if parameter_config is not None and arg_name in parameter_config:
-                for k, v in parameter_config[arg_name].items():
-                    self.add_new_row(arg_name, k, v)
-            add_button = ttk.Button(self.parameter_frame, text="Add")
-            add_button.grid(row=row_id, column=0, sticky=tk.NW, padx=3, pady=3)
-            self.buttons[arg_name] = add_button
-            row_id += 1
-            separator = ttk.Separator(self.parameter_frame)
-            separator.grid(row=row_id, column=0, sticky=tk.NSEW, pady=10)
-            row_id += 1
-
-        if len(args_name) > 1:
-            save_button = ttk.Button(self.parameter_frame, text="Save")
-            save_button.grid(row=row_id, column=0, sticky=tk.NE, padx=3, pady=3)
-            #: ttk.Button: Save button
-            self.save_button = save_button
-
-    def add_new_row(self, arg_name, k="", v=""):
-        """Add new row to the popup
-
-        Parameters
-        ----------
-        arg_name : str
-            Name of the argument
-        k : str
-            Name of the function
-        v : str
-            Value of the function
-        """
-        r = len(self.inputs[arg_name])
-        arg_frame = self.arg_frames[arg_name]
-        ref_value_entry = LabelInput(
-            parent=arg_frame,
-            label="Function Name",
-            input_class=ttk.Entry,
-            input_var=tk.StringVar(),
-            input_args={"width": 50},
-        )
-        ref_value_entry.grid(row=r, column=1, sticky=tk.NSEW, padx=3, pady=3)
-        ref_value_entry.set(k)
-        value_entry = LabelInput(
-            parent=arg_frame,
-            label="Value",
-            input_class=ttk.Entry,
-            input_var=tk.StringVar(),
-            input_args={"width": 50},
-        )
-        value_entry.grid(row=r, column=2, sticky=tk.NSEW, padx=3, pady=3)
-        value_entry.set(v)
-        load_button = ttk.Button(arg_frame, text="Load")
-        load_button.grid(row=r, column=3, sticky=tk.NSEW, padx=3, pady=3)
-        delete_button = ttk.Button(arg_frame, text="Delete")
-        delete_button.grid(row=r, column=4, sticky=tk.NSEW, padx=3, pady=3)
-        delete_button.config(command=self.delete_row(arg_name, r))
-        self.inputs[arg_name].append(
-            (ref_value_entry, value_entry, load_button, delete_button)
-        )
-
-    def delete_row(self, arg_name, r):
-        """Delete row from the popup
 
-        Parameters
-        ----------
-        arg_name : str
-            Name of the argument
-        r : int
-            Row number
-        """
-
-        def func():
-            """Function to delete row from the popup
-
-            Returns
-            -------
-            func
-                Function to delete row from the popup
-            """
-            for w in self.inputs[arg_name][r]:
-                w.grid_remove()
-            self.inputs[arg_name][r] = None
+        def write_func(prefix, config_dict, f):
+            for k in config_dict:
+                if type(config_dict[k]) == dict:
+                    f.write(f"{prefix}{k}:\n")
+                    write_func(prefix + " " * 2, config_dict[k], f)
+                elif type(config_dict[k]) == list:
+                    list_prefix = " "
+                    if k != "None":
+                        f.write(f"{prefix}{k}:\n")
+                        list_prefix = " " * 2
+                    for list_item in config_dict[k]:
+                        f.write(f"{prefix}{list_prefix}-\n")
+                        write_func(prefix + list_prefix * 2, list_item, f)
+                else:
+                    f.write(f"{prefix}{k}: {config_dict[k]}\n")
+
+        with open(filename, "w") as f:
+            f.write("microscopes:\n")
+            write_func("  ", config, f)
+
+    def create_config_window(self, id):
+        """Creates the configuration window tabs."""
+
+        tab_name = "Microscope-" + str(id)
+        microscope_tab = MicroscopeTab(
+            self.view.microscope_window,
+            root=self.view.root,
+        )
+        self.view.microscope_window.tab_list.append(tab_name)
+        for hardware_type, widgets in hardwares_dict.items():
+            if not widgets:
+                continue
+            if type(widgets) == dict:
+                microscope_tab.create_hardware_tab(hardware_type, widgets)
+            else:
+                microscope_tab.create_hardware_tab(
+                    hardware_type,
+                    hardware_widgets=widgets[1],
+                    widgets=widgets[2],
+                    top_widgets=widgets[0],
+                )
+
+        # Adding tabs to self notebook
+        self.view.microscope_window.add(
+            microscope_tab,
+            text=tab_name,
+            sticky=tk.NSEW,
+        )
+
+    def load_configuration(self):
+        """Load configuration"""
+
+        def get_widget_value(name, value_dict):
+            """Get the value from a dict"""
+            value = value_dict
+            for key in name.split("/"):
+                if key.strip() == "":
+                    return value
+                value = value.get(key, None)
+                if value is None:
+                    return None
+            return value
+
+        def get_widgets_value(widgets, value_dict):
+            """Get all key-value from valude_dict, keys are from widgets"""
+            temp = {}
+            for key in widgets:
+                if key == "frame_config":
+                    continue
+                if widgets[key][1] in ["Button", "Label"]:
+                    continue
+                value = get_widget_value(key, value_dict)
+                # widgets[key][3] is the value mapping dict
+                if widgets[key][1] != "Spinbox"and widgets[key][3]:
+                    # if the value is not valid, return the last valid value
+                    if type(widgets[key][3]) == list:
+                        reverse_value_dict = dict(map(lambda v: (v, v), widgets[key][3]))
+                    else:
+                        reverse_value_dict = dict(
+                            map(lambda v: (v[1], v[0]), widgets[key][3].items())
+                        )
+                    temp[key] = reverse_value_dict.get(value, list(reverse_value_dict.values())[-1])
+                else:
+                    temp[key] = value
+            return temp
+
+        def build_widgets_value(widgets, value_dict):
+            """According to valude_dict build values for widgets"""
+            if widgets is None or value_dict is None:
+                return [None]
+            result = []
+            ref = ""
+            format = ""
+            if "frame_config" in widgets:
+                ref = widgets["frame_config"].get("ref", "")
+                format = widgets["frame_config"].get("format", "")
+            if format.startswith("list"):
+                if ref != "" and ref.lower() != "none":
+                    value_dict = get_widget_value(ref, value_dict)
+                if type(value_dict) is not list:
+                    return [None]
+                for i in range(len(value_dict)):
+                    result.append(get_widgets_value(widgets, value_dict[i]))
+            elif format.startswith("item"):
+                format_list = format.split(";")
+                ref_list = ref.split(";")
+                for i, format_item in enumerate(format_list):
+                    k_idx = format_item[
+                        format_item.index("(") + 1 : format_item.index(",")
+                    ].strip()
+                    v_idx = format_item[
+                        format_item.index(",") + 1 : format_item.index(")")
+                    ].strip()
+                    temp_widget_values = get_widget_value(ref_list[i], value_dict)
+                    for j, k in enumerate(temp_widget_values.keys()):
+                        if len(result) < j + 1:
+                            result.append({k_idx: k, v_idx: temp_widget_values[k]})
+                        else:
+                            result[j][k_idx] = k
+                            result[j][v_idx] = temp_widget_values[k]
+            else:
+                if ref != "" and ref.lower() != "none":
+                    value_dict = get_widget_value(ref, value_dict)
+                result.append(get_widgets_value(widgets, value_dict))
+
+            return result
+        # ask file name
+        file_name = filedialog.askopenfilename(
+            defaultextension=".yml", filetypes=[("Yaml file", "*.yml *.yaml")]
+        )
+        if not file_name:
+            return
+
+        # read configuration.yaml
+        config_dict = load_yaml_file(file_name)
+        if config_dict is None or "microscopes" not in config_dict:
+            messagebox.showerror(
+                title="Configuration",
+                message="It's not a valid configuration.yaml file!"
+            )
+            return
+        
+        self.delete_microscopes()
 
-        return func
+        for i, microscope_name in enumerate(config_dict["microscopes"].keys()):
+            microscope_tab = MicroscopeTab(
+                self.view.microscope_window,
+                root=self.view.root,
+            )
+            self.view.microscope_window.add(
+                microscope_tab,
+                text=microscope_name,
+                sticky=tk.NSEW,
+            )
+            self.view.microscope_window.tab_list.append(microscope_name)
+            
+            for hardware_type, widgets in hardwares_dict.items():
+                hardware_ref_name = hardwares_config_name_dict[hardware_type]
+                # build dictionary values for widgets
+                if type(widgets) == dict:
+                    try:
+                        widgets_value = build_widgets_value(
+                            widgets,
+                            config_dict["microscopes"][microscope_name][
+                                hardware_ref_name
+                            ],
+                        )
+                    except Exception as e:
+                        widgets_value = [None]
+                    microscope_tab.create_hardware_tab(
+                        hardware_type, widgets, hardware_widgets_value=widgets_value
+                    )
+                else:
+                    try:
+                        widgets_value = [
+                            build_widgets_value(
+                                widgets[1],
+                                config_dict["microscopes"][microscope_name][
+                                    hardware_ref_name
+                                ],
+                            ),
+                            build_widgets_value(
+                                widgets[2],
+                                config_dict["microscopes"][microscope_name][
+                                    hardware_ref_name
+                                ],
+                            ),
+                        ]
+                    except:
+                        widgets_value = [[None], [None]]
+                    microscope_tab.create_hardware_tab(
+                        hardware_type,
+                        hardware_widgets=widgets[1],
+                        widgets=widgets[2],
+                        top_widgets=widgets[0],
+                        hardware_widgets_value=widgets_value[0],
+                        constants_widgets_value=widgets_value[1],
+                    )
+
+    def device_selected(self, event):
+        """Handle the event when a device is selected from the dropdown."""
+        # # Get the selected device name
+        # selected_device_name = self.view.microscope_frame.get()
+        # # Find the key in the dictionary that corresponds to the selected value
+        # selected_key = next(
+        #     key for key, value in device_types.items()
+        #     if value == selected_device_name)
+        # print(f"Selected Device Key: {selected_key}")
+        # print(f"Selected Device Name: {selected_device_name}")
+        pass
```

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/ilastik_setting_popup.py` & `navigate_micro-0.0.6/src/navigate/view/popups/ilastik_setting_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/microscope_setting_popup_window.py` & `navigate_micro-0.0.6/src/navigate/view/popups/microscope_setting_popup_window.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/plugins_popup.py` & `navigate_micro-0.0.6/src/navigate/view/popups/plugins_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/tiling_wizard_popup.py` & `navigate_micro-0.0.6/src/navigate/view/popups/tiling_wizard_popup.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/tiling_wizard_popup2.py` & `navigate_micro-0.0.6/src/navigate/view/popups/tiling_wizard_popup2.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/popups/waveform_parameter_popup_window.py` & `navigate_micro-0.0.6/src/navigate/view/popups/waveform_parameter_popup_window.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate/view/splash_screen.py` & `navigate_micro-0.0.6/src/navigate/view/splash_screen.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/src/navigate_micro.egg-info/PKG-INFO` & `navigate_micro-0.0.6/src/navigate_micro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: navigate-micro
-Version: 0.0.5
+Version: 0.0.6
 Summary: Open source, smart, light-sheet microscopy control software.
 Author: The Dean Lab, UT Southwestern Medical Center
 License: Copyright (c) 2021-2023 The University of Texas Southwestern Medical Center.
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are
@@ -73,14 +73,15 @@
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xvfb; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: jupyterlab; extra == "dev"
+Requires-Dist: pydantic-ome-ngff; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: numpydoc; extra == "docs"
 Requires-Dist: nbconvert; extra == "docs"
 Requires-Dist: sphinx<6.0.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-issues; extra == "docs"
```

### Comparing `navigate-micro-0.0.5/src/navigate_micro.egg-info/SOURCES.txt` & `navigate_micro-0.0.6/src/navigate_micro.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 src/navigate/VERSION
 src/navigate/__init__.py
 src/navigate/_commit.py
 src/navigate/main.py
 src/navigate/config/__init__.py
 src/navigate/config/config.py
 src/navigate/config/configuration.yaml
+src/navigate/config/configuration_database.py
 src/navigate/config/experiment.yml
 src/navigate/config/rest_api_config.yml
 src/navigate/config/synthetic_configuration.yaml
 src/navigate/config/waveform_constants.yml
 src/navigate/config/waveform_templates.yml
 src/navigate/controller/__init__.py
 src/navigate/controller/configuration_controller.py
+src/navigate/controller/configurator.py
 src/navigate/controller/controller.py
 src/navigate/controller/thread_pool.py
 src/navigate/controller/sub_controllers/__init__.py
 src/navigate/controller/sub_controllers/acquire_bar_controller.py
 src/navigate/controller/sub_controllers/adaptiveoptics_popup_controller.py
 src/navigate/controller/sub_controllers/autofocus_popup_controller.py
 src/navigate/controller/sub_controllers/camera_map_setting_popup_controller.py
@@ -59,19 +61,23 @@
 src/navigate/model/analysis/camera.py
 src/navigate/model/analysis/image_contrast.py
 src/navigate/model/concurrency/__init__.py
 src/navigate/model/concurrency/concurrency_tools.py
 src/navigate/model/data_sources/__init__.py
 src/navigate/model/data_sources/bdv_data_source.py
 src/navigate/model/data_sources/data_source.py
+src/navigate/model/data_sources/pyramidal_data_source.py
 src/navigate/model/data_sources/tiff_data_source.py
+src/navigate/model/data_sources/zarr_data_source.py
 src/navigate/model/devices/__init__.py
 src/navigate/model/devices/objectives.py
 src/navigate/model/devices/APIs/__init__.py
 src/navigate/model/devices/APIs/asi/__init__.py
+src/navigate/model/devices/APIs/asi/asi_MFC_controller.py
+src/navigate/model/devices/APIs/asi/asi_MS2000_controller.py
 src/navigate/model/devices/APIs/asi/asi_tiger_controller.py
 src/navigate/model/devices/APIs/coherent/ObisLaser.py
 src/navigate/model/devices/APIs/coherent/__init__.py
 src/navigate/model/devices/APIs/dynamixel/__init__.py
 src/navigate/model/devices/APIs/dynamixel/dynamixel_functions.py
 src/navigate/model/devices/APIs/hamamatsu/HamamatsuAPI.py
 src/navigate/model/devices/APIs/hamamatsu/__init__.py
@@ -102,14 +108,15 @@
 src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/stream_to_disk.py
 src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/sw_trigger.py
 src/navigate/model/devices/APIs/photometrics/PyVCAM-master/tests/test_camera.py
 src/navigate/model/devices/APIs/sutter/MP285.py
 src/navigate/model/devices/APIs/sutter/__init__.py
 src/navigate/model/devices/APIs/thorlabs/__init__.py
 src/navigate/model/devices/APIs/thorlabs/kcube_inertial.py
+src/navigate/model/devices/APIs/thorlabs/kcube_steppermotor.py
 src/navigate/model/devices/camera/__init__.py
 src/navigate/model/devices/camera/camera_base.py
 src/navigate/model/devices/camera/camera_hamamatsu.py
 src/navigate/model/devices/camera/camera_photometrics.py
 src/navigate/model/devices/camera/camera_synthetic.py
 src/navigate/model/devices/daq/__init__.py
 src/navigate/model/devices/daq/daq_base.py
@@ -139,21 +146,24 @@
 src/navigate/model/devices/remote_focus/remote_focus_synthetic.py
 src/navigate/model/devices/shutter/__init__.py
 src/navigate/model/devices/shutter/laser_shutter_base.py
 src/navigate/model/devices/shutter/laser_shutter_synthetic.py
 src/navigate/model/devices/shutter/laser_shutter_ttl.py
 src/navigate/model/devices/stages/__init__.py
 src/navigate/model/devices/stages/stage_asi.py
+src/navigate/model/devices/stages/stage_asi_MFCTwoThousand.py
+src/navigate/model/devices/stages/stage_asi_MSTwoThousand.py
 src/navigate/model/devices/stages/stage_base.py
 src/navigate/model/devices/stages/stage_galvo.py
 src/navigate/model/devices/stages/stage_mcl.py
 src/navigate/model/devices/stages/stage_pi.py
 src/navigate/model/devices/stages/stage_sutter.py
 src/navigate/model/devices/stages/stage_synthetic.py
 src/navigate/model/devices/stages/stage_tl_kcube_inertial.py
+src/navigate/model/devices/stages/stage_tl_kcube_steppermotor.py
 src/navigate/model/devices/zoom/__init__.py
 src/navigate/model/devices/zoom/zoom_base.py
 src/navigate/model/devices/zoom/zoom_dynamixel.py
 src/navigate/model/devices/zoom/zoom_synthetic.py
 src/navigate/model/features/__init__.py
 src/navigate/model/features/adaptive_optics.py
 src/navigate/model/features/auto_tile_scan.py
@@ -166,31 +176,35 @@
 src/navigate/model/features/remove_empty_tiles.py
 src/navigate/model/features/restful_features.py
 src/navigate/model/features/volume_search.py
 src/navigate/model/metadata_sources/__init__.py
 src/navigate/model/metadata_sources/bdv_metadata.py
 src/navigate/model/metadata_sources/metadata.py
 src/navigate/model/metadata_sources/ome_tiff_metadata.py
+src/navigate/model/metadata_sources/zarr_metadata.py
 src/navigate/plugins/__init__.py
 src/navigate/tools/__init__.py
 src/navigate/tools/common_dict_tools.py
 src/navigate/tools/common_functions.py
 src/navigate/tools/decorators.py
 src/navigate/tools/file_functions.py
 src/navigate/tools/image.py
 src/navigate/tools/linear_algebra.py
 src/navigate/tools/main_functions.py
 src/navigate/tools/multipos_table_tools.py
 src/navigate/tools/sdf.py
+src/navigate/tools/slicing.py
 src/navigate/tools/waveform_template_funcs.py
 src/navigate/tools/xml_tools.py
 src/navigate/view/__init__.py
+src/navigate/view/configurator_application_window.py
 src/navigate/view/main_application_window.py
 src/navigate/view/splash_screen.py
 src/navigate/view/custom_widgets/ArrowLabel.py
+src/navigate/view/custom_widgets/CollapsibleFrame.py
 src/navigate/view/custom_widgets/DockableNotebook.py
 src/navigate/view/custom_widgets/LabelInputWidgetFactory.py
 src/navigate/view/custom_widgets/__init__.py
 src/navigate/view/custom_widgets/hover.py
 src/navigate/view/custom_widgets/hoverbar.py
 src/navigate/view/custom_widgets/hovermixin.py
 src/navigate/view/custom_widgets/popup.py
```

### Comparing `navigate-micro-0.0.5/src/navigate_micro.egg-info/requires.txt` & `navigate_micro-0.0.6/src/navigate_micro.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 [dev]
 pytest
 pytest-xvfb
 pytest-cov
 pre-commit
 ipykernel
 jupyterlab
+pydantic-ome-ngff
 
 [docs]
 numpydoc
 nbconvert
 sphinx<6.0.0
 sphinx_rtd_theme
 sphinx-copybutton
```

### Comparing `navigate-micro-0.0.5/test/test_commit.py` & `navigate_micro-0.0.6/test/test_commit.py`

 * *Files identical despite different names*

### Comparing `navigate-micro-0.0.5/test/test_main.py` & `navigate_micro-0.0.6/test/test_main.py`

 * *Files identical despite different names*

