# Comparing `tmp/amiya-0.0.3.tar.gz` & `tmp/amiya-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amiya-0.0.3.tar", last modified: Wed May 15 23:15:05 2024, max compression
+gzip compressed data, was "amiya-0.0.4.tar", last modified: Fri May 24 19:44:21 2024, max compression
```

## Comparing `amiya-0.0.3.tar` & `amiya-0.0.4.tar`

### file list

```diff
@@ -1,118 +1,92 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.732537 amiya-0.0.3/
--rw-rw-rw-   0        0        0     1086 2024-04-03 01:29:58.000000 amiya-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      213 2024-05-15 23:14:11.000000 amiya-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2678 2024-05-15 23:15:05.732037 amiya-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1839 2024-05-15 22:41:01.000000 amiya-0.0.3/README.md
--rw-rw-rw-   0        0        0       95 2024-05-01 05:31:02.000000 amiya-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      128 2024-05-15 22:58:42.000000 amiya-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 23:15:05.733033 amiya-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2391 2024-05-15 23:08:36.000000 amiya-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.680917 amiya-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.692933 amiya-0.0.3/src/amiya/
--rw-rw-rw-   0        0        0     1122 2024-05-01 05:27:34.000000 amiya-0.0.3/src/amiya/__init__.py
--rw-rw-rw-   0        0        0     1880 2024-05-15 22:01:51.000000 amiya-0.0.3/src/amiya/amiya.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.685918 amiya-0.0.3/src/amiya/apps/
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.697438 amiya-0.0.3/src/amiya/apps/afk-journey/
--rw-rw-rw-   0        0        0      248 2024-05-15 21:59:19.000000 amiya-0.0.3/src/amiya/apps/afk-journey/app-config.json
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.681916 amiya-0.0.3/src/amiya/apps/afk-journey/automation/
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.698458 amiya-0.0.3/src/amiya/apps/afk-journey/automation/sequence/
--rw-rw-rw-   0        0        0    59570 2024-05-15 01:49:58.000000 amiya-0.0.3/src/amiya/apps/afk-journey/automation/sequence/daily.json
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.698963 amiya-0.0.3/src/amiya/apps/chrome/
--rw-rw-rw-   0        0        0      256 2024-05-15 21:59:19.000000 amiya-0.0.3/src/amiya/apps/chrome/app-config.json
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.699463 amiya-0.0.3/src/amiya/apps/genshin-impact/
--rw-rw-rw-   0        0        0      265 2024-05-15 21:59:19.000000 amiya-0.0.3/src/amiya/apps/genshin-impact/app-config.json
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.699968 amiya-0.0.3/src/amiya/apps/honkai-star-rail/
--rw-rw-rw-   0        0        0      251 2024-05-15 21:59:19.000000 amiya-0.0.3/src/amiya/apps/honkai-star-rail/app-config.json
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.700465 amiya-0.0.3/src/amiya/apps/ld-player/
--rw-rw-rw-   0        0        0      240 2024-05-15 21:59:20.000000 amiya-0.0.3/src/amiya/apps/ld-player/app-config.json
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.683418 amiya-0.0.3/src/amiya/apps/ld-player/automation/
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.701464 amiya-0.0.3/src/amiya/apps/ld-player/automation/sequence/
--rw-rw-rw-   0        0        0    56052 2024-05-14 23:43:35.000000 amiya-0.0.3/src/amiya/apps/ld-player/automation/sequence/arknights-base.json
--rw-rw-rw-   0        0        0     3048 2024-05-04 02:32:47.000000 amiya-0.0.3/src/amiya/apps/ld-player/automation/sequence/arknights-start.json
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.701963 amiya-0.0.3/src/amiya/apps/league-of-legends/
--rw-rw-rw-   0        0        0      274 2024-05-15 21:59:20.000000 amiya-0.0.3/src/amiya/apps/league-of-legends/app-config.json
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.702464 amiya-0.0.3/src/amiya/apps/persona-5-x/
--rw-rw-rw-   0        0        0      243 2024-05-15 21:59:20.000000 amiya-0.0.3/src/amiya/apps/persona-5-x/app-config.json
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.685918 amiya-0.0.3/src/amiya/apps/persona-5-x/automation/
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.703464 amiya-0.0.3/src/amiya/apps/persona-5-x/automation/sequence/
--rw-rw-rw-   0        0        0   110959 2024-04-26 03:13:43.000000 amiya-0.0.3/src/amiya/apps/persona-5-x/automation/sequence/daily.json
--rw-rw-rw-   0        0        0    96070 2024-05-05 04:33:03.000000 amiya-0.0.3/src/amiya/apps/persona-5-x/automation/sequence/test.json
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.703966 amiya-0.0.3/src/amiya/apps/steam/
--rw-rw-rw-   0        0        0      216 2024-05-15 21:59:20.000000 amiya-0.0.3/src/amiya/apps/steam/app-config.json
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.706465 amiya-0.0.3/src/amiya/apps_manager/
--rw-rw-rw-   0        0        0     1122 2024-04-13 23:21:03.000000 amiya-0.0.3/src/amiya/apps_manager/__init__.py
--rw-rw-rw-   0        0        0     8624 2024-05-13 19:47:34.000000 amiya-0.0.3/src/amiya/apps_manager/app.py
--rw-rw-rw-   0        0        0    23221 2024-05-13 19:45:19.000000 amiya-0.0.3/src/amiya/apps_manager/apps_manager.py
--rw-rw-rw-   0        0        0     1938 2024-05-07 23:50:31.000000 amiya-0.0.3/src/amiya/apps_manager/apps_viewer.py
--rw-rw-rw-   0        0        0     3359 2024-05-13 18:16:23.000000 amiya-0.0.3/src/amiya/apps_manager/safety_monitor.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.707470 amiya-0.0.3/src/amiya/apps_manager/sync_controller/
--rw-rw-rw-   0        0        0        0 2024-04-22 19:14:02.000000 amiya-0.0.3/src/amiya/apps_manager/sync_controller/__init__.py
--rw-rw-rw-   0        0        0     2863 2024-04-26 02:54:50.000000 amiya-0.0.3/src/amiya/apps_manager/sync_controller/sync_controller.py
--rw-rw-rw-   0        0        0      539 2024-05-01 03:42:43.000000 amiya-0.0.3/src/amiya/apps_manager/sync_controller/sys_uuid_controller.py
--rw-rw-rw-   0        0        0       64 2024-04-07 04:55:43.000000 amiya-0.0.3/src/amiya/apps_manager/test.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.710489 amiya-0.0.3/src/amiya/automation_handler/
--rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:45.000000 amiya-0.0.3/src/amiya/automation_handler/__init__.py
--rw-rw-rw-   0        0        0      723 2024-04-25 02:34:30.000000 amiya-0.0.3/src/amiya/automation_handler/automation_config_handler.py
--rw-rw-rw-   0        0        0     9304 2024-05-07 23:35:45.000000 amiya-0.0.3/src/amiya/automation_handler/automation_controller.py
--rw-rw-rw-   0        0        0     7043 2024-05-15 22:11:47.000000 amiya-0.0.3/src/amiya/automation_handler/automation_recorder.py
--rw-rw-rw-   0        0        0      977 2024-04-25 02:20:57.000000 amiya-0.0.3/src/amiya/automation_handler/automation_viewer.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.712490 amiya-0.0.3/src/amiya/automation_handler/units/
--rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:54.000000 amiya-0.0.3/src/amiya/automation_handler/units/__init__.py
--rw-rw-rw-   0        0        0     4595 2024-05-05 22:30:53.000000 amiya-0.0.3/src/amiya/automation_handler/units/action.py
--rw-rw-rw-   0        0        0     1595 2024-04-25 03:15:44.000000 amiya-0.0.3/src/amiya/automation_handler/units/plate.py
--rw-rw-rw-   0        0        0     7763 2024-05-10 13:26:52.000000 amiya-0.0.3/src/amiya/automation_handler/units/sequence.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.713988 amiya-0.0.3/src/amiya/bin/
--rwxrwxrwx   0        0        0    42694 2024-05-13 19:09:05.000000 amiya-0.0.3/src/amiya/bin/focus_pid.exe
--rwxrwxrwx   0        0        0    42243 2024-05-13 19:09:04.000000 amiya-0.0.3/src/amiya/bin/get_active_pid.exe
--rwxrwxrwx   0        0        0    42845 2024-05-13 19:09:04.000000 amiya-0.0.3/src/amiya/bin/get_window_size.exe
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.714988 amiya-0.0.3/src/amiya/bin/scripts/
--rw-rw-rw-   0        0        0     1831 2024-05-13 19:09:02.000000 amiya-0.0.3/src/amiya/bin/scripts/focus_pid.c
--rw-rw-rw-   0        0        0      469 2024-04-13 02:51:25.000000 amiya-0.0.3/src/amiya/bin/scripts/get_active_pid.c
--rw-rw-rw-   0        0        0     1841 2024-04-26 04:14:54.000000 amiya-0.0.3/src/amiya/bin/scripts/get_window_size.c
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.716489 amiya-0.0.3/src/amiya/entrypoints/
--rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:03.000000 amiya-0.0.3/src/amiya/entrypoints/__init__.py
--rw-rw-rw-   0        0        0    12117 2024-05-15 22:36:22.000000 amiya-0.0.3/src/amiya/entrypoints/entrypoint_handler.py
--rw-rw-rw-   0        0        0    13338 2024-05-15 22:22:51.000000 amiya-0.0.3/src/amiya/entrypoints/entrypoints.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.717492 amiya-0.0.3/src/amiya/exceptions/
--rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:17.000000 amiya-0.0.3/src/amiya/exceptions/__init__.py
--rw-rw-rw-   0        0        0     3819 2024-05-01 04:45:51.000000 amiya-0.0.3/src/amiya/exceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.720513 amiya-0.0.3/src/amiya/module_utilities/
--rw-rw-rw-   0        0        0      214 2024-05-12 19:29:56.000000 amiya-0.0.3/src/amiya/module_utilities/__init__.py
--rw-rw-rw-   0        0        0     2579 2024-05-15 22:13:01.000000 amiya-0.0.3/src/amiya/module_utilities/continuous_click_controller.py
--rw-rw-rw-   0        0        0     3168 2024-05-12 22:48:48.000000 amiya-0.0.3/src/amiya/module_utilities/cursor_controller.py
--rw-rw-rw-   0        0        0     1245 2024-05-13 18:35:25.000000 amiya-0.0.3/src/amiya/module_utilities/dev_features.py
--rw-rw-rw-   0        0        0     2709 2024-05-07 23:22:25.000000 amiya-0.0.3/src/amiya/module_utilities/power_controller.py
--rw-rw-rw-   0        0        0     1062 2024-05-01 05:07:47.000000 amiya-0.0.3/src/amiya/module_utilities/search_controller.py
--rw-rw-rw-   0        0        0     8832 2024-05-12 16:53:49.000000 amiya-0.0.3/src/amiya/module_utilities/volume_controller.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.722016 amiya-0.0.3/src/amiya/pixel_calculator/
--rw-rw-rw-   0        0        0        0 2024-04-19 04:01:16.000000 amiya-0.0.3/src/amiya/pixel_calculator/__init__.py
--rw-rw-rw-   0        0        0     1693 2024-05-15 02:40:55.000000 amiya-0.0.3/src/amiya/pixel_calculator/pixel_calculator.py
--rw-rw-rw-   0        0        0     2830 2024-05-14 06:07:14.000000 amiya-0.0.3/src/amiya/pixel_calculator/resolution_detector.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.725515 amiya-0.0.3/src/amiya/resources/
--rw-rw-rw-   0        0        0    94080 2024-04-13 19:09:50.000000 amiya-0.0.3/src/amiya/resources/amiya-cli-2.png
--rw-rw-rw-   0        0        0   104680 2024-04-13 19:09:37.000000 amiya-0.0.3/src/amiya/resources/amiya-cli-3.png
--rw-rw-rw-   0        0        0   254392 2024-05-01 05:56:34.000000 amiya-0.0.3/src/amiya/resources/amiya-cli-4.png
--rw-rw-rw-   0        0        0    46585 2024-04-13 19:10:01.000000 amiya-0.0.3/src/amiya/resources/amiya-cli.png
--rw-rw-rw-   0        0        0   166735 2024-04-05 02:00:17.000000 amiya-0.0.3/src/amiya/resources/amiya.png
--rw-rw-rw-   0        0        0   197822 2024-04-05 17:56:21.000000 amiya-0.0.3/src/amiya/resources/amiya_with_border.png
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.727518 amiya-0.0.3/src/amiya/resources/code_snippets/
--rw-rw-rw-   0        0        0    60828 2024-04-13 19:08:35.000000 amiya-0.0.3/src/amiya/resources/code_snippets/add-app.png
--rw-rw-rw-   0        0        0    78155 2024-04-13 19:08:59.000000 amiya-0.0.3/src/amiya/resources/code_snippets/add-tag.png
--rw-rw-rw-   0        0        0    25735 2024-04-13 19:09:12.000000 amiya-0.0.3/src/amiya/resources/code_snippets/start.png
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.728826 amiya-0.0.3/src/amiya/scheduler/
--rw-rw-rw-   0        0        0        0 2024-04-23 03:48:30.000000 amiya-0.0.3/src/amiya/scheduler/__init__.py
--rw-rw-rw-   0        0        0     4458 2024-04-23 03:07:35.000000 amiya-0.0.3/src/amiya/scheduler/scheduler.py
--rw-rw-rw-   0        0        0      934 2024-04-22 21:49:58.000000 amiya-0.0.3/src/amiya/scheduler/scheduler_config_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.731036 amiya-0.0.3/src/amiya/utils/
--rw-rw-rw-   0        0        0        0 2024-04-10 04:03:44.000000 amiya-0.0.3/src/amiya/utils/__init__.py
--rw-rw-rw-   0        0        0     1652 2024-05-15 22:44:44.000000 amiya-0.0.3/src/amiya/utils/constants.py
--rw-rw-rw-   0        0        0    10960 2024-05-13 19:29:29.000000 amiya-0.0.3/src/amiya/utils/helper.py
--rw-rw-rw-   0        0        0     1039 2024-04-24 20:18:29.000000 amiya-0.0.3/src/amiya/utils/json_handler.py
--rw-rw-rw-   0        0        0     1415 2024-04-10 04:03:43.000000 amiya-0.0.3/src/amiya/utils/pynput_mapping.py
-drwxrwxrwx   0        0        0        0 2024-05-15 23:15:05.731534 amiya-0.0.3/src/amiya.egg-info/
--rw-rw-rw-   0        0        0     2678 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3253 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      117 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-15 23:15:05.000000 amiya-0.0.3/src/amiya.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.449616 amiya-0.0.4/
+-rw-rw-rw-   0        0        0     1086 2024-04-03 01:29:58.000000 amiya-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      238 2024-05-24 19:42:40.000000 amiya-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     8183 2024-05-24 19:44:21.449616 amiya-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7344 2024-05-24 19:40:47.000000 amiya-0.0.4/README.md
+-rw-rw-rw-   0        0        0       95 2024-05-01 05:31:02.000000 amiya-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      128 2024-05-15 22:58:42.000000 amiya-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 19:44:21.449616 amiya-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2378 2024-05-24 19:30:10.000000 amiya-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.408618 amiya-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.416617 amiya-0.0.4/src/amiya/
+-rw-rw-rw-   0        0        0     1122 2024-05-01 05:27:34.000000 amiya-0.0.4/src/amiya/__init__.py
+-rw-rw-rw-   0        0        0     1880 2024-05-15 22:01:51.000000 amiya-0.0.4/src/amiya/amiya.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.424615 amiya-0.0.4/src/amiya/apps_manager/
+-rw-rw-rw-   0        0        0     1122 2024-04-13 23:21:03.000000 amiya-0.0.4/src/amiya/apps_manager/__init__.py
+-rw-rw-rw-   0        0        0    10349 2024-05-24 19:29:59.000000 amiya-0.0.4/src/amiya/apps_manager/app.py
+-rw-rw-rw-   0        0        0    26191 2024-05-24 19:39:44.000000 amiya-0.0.4/src/amiya/apps_manager/apps_manager.py
+-rw-rw-rw-   0        0        0     1938 2024-05-07 23:50:31.000000 amiya-0.0.4/src/amiya/apps_manager/apps_viewer.py
+-rw-rw-rw-   0        0        0     3615 2024-05-22 01:47:54.000000 amiya-0.0.4/src/amiya/apps_manager/safety_monitor.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.425615 amiya-0.0.4/src/amiya/apps_manager/sync_controller/
+-rw-rw-rw-   0        0        0        0 2024-04-22 19:14:02.000000 amiya-0.0.4/src/amiya/apps_manager/sync_controller/__init__.py
+-rw-rw-rw-   0        0        0     4844 2024-05-22 20:27:06.000000 amiya-0.0.4/src/amiya/apps_manager/sync_controller/sync_controller.py
+-rw-rw-rw-   0        0        0      551 2024-05-22 01:59:45.000000 amiya-0.0.4/src/amiya/apps_manager/sync_controller/sys_uuid_controller.py
+-rw-rw-rw-   0        0        0       64 2024-04-07 04:55:43.000000 amiya-0.0.4/src/amiya/apps_manager/test.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.427615 amiya-0.0.4/src/amiya/automation_handler/
+-rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:45.000000 amiya-0.0.4/src/amiya/automation_handler/__init__.py
+-rw-rw-rw-   0        0        0      723 2024-04-25 02:34:30.000000 amiya-0.0.4/src/amiya/automation_handler/automation_config_handler.py
+-rw-rw-rw-   0        0        0     9304 2024-05-07 23:35:45.000000 amiya-0.0.4/src/amiya/automation_handler/automation_controller.py
+-rw-rw-rw-   0        0        0     7043 2024-05-15 22:11:47.000000 amiya-0.0.4/src/amiya/automation_handler/automation_recorder.py
+-rw-rw-rw-   0        0        0      977 2024-04-25 02:20:57.000000 amiya-0.0.4/src/amiya/automation_handler/automation_viewer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.429618 amiya-0.0.4/src/amiya/automation_handler/units/
+-rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:54.000000 amiya-0.0.4/src/amiya/automation_handler/units/__init__.py
+-rw-rw-rw-   0        0        0     4595 2024-05-05 22:30:53.000000 amiya-0.0.4/src/amiya/automation_handler/units/action.py
+-rw-rw-rw-   0        0        0     1595 2024-04-25 03:15:44.000000 amiya-0.0.4/src/amiya/automation_handler/units/plate.py
+-rw-rw-rw-   0        0        0     7763 2024-05-18 02:24:40.000000 amiya-0.0.4/src/amiya/automation_handler/units/sequence.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.431616 amiya-0.0.4/src/amiya/bin/
+-rwxrwxrwx   0        0        0    42694 2024-05-13 19:09:05.000000 amiya-0.0.4/src/amiya/bin/focus_pid.exe
+-rwxrwxrwx   0        0        0    42243 2024-05-13 19:09:04.000000 amiya-0.0.4/src/amiya/bin/get_active_pid.exe
+-rwxrwxrwx   0        0        0    42845 2024-05-13 19:09:04.000000 amiya-0.0.4/src/amiya/bin/get_window_size.exe
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.432615 amiya-0.0.4/src/amiya/bin/scripts/
+-rw-rw-rw-   0        0        0     1831 2024-05-13 19:09:02.000000 amiya-0.0.4/src/amiya/bin/scripts/focus_pid.c
+-rw-rw-rw-   0        0        0      469 2024-04-13 02:51:25.000000 amiya-0.0.4/src/amiya/bin/scripts/get_active_pid.c
+-rw-rw-rw-   0        0        0     1841 2024-04-26 04:14:54.000000 amiya-0.0.4/src/amiya/bin/scripts/get_window_size.c
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.434615 amiya-0.0.4/src/amiya/entrypoints/
+-rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:03.000000 amiya-0.0.4/src/amiya/entrypoints/__init__.py
+-rw-rw-rw-   0        0        0    13708 2024-05-23 05:45:30.000000 amiya-0.0.4/src/amiya/entrypoints/entrypoint_handler.py
+-rw-rw-rw-   0        0        0    19155 2024-05-23 05:45:19.000000 amiya-0.0.4/src/amiya/entrypoints/entrypoints.py
+-rw-rw-rw-   0        0        0     1164 2024-05-22 02:21:02.000000 amiya-0.0.4/src/amiya/entrypoints/help_format_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.435614 amiya-0.0.4/src/amiya/exceptions/
+-rw-rw-rw-   0        0        0     1122 2024-04-13 23:20:17.000000 amiya-0.0.4/src/amiya/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     4003 2024-05-24 19:02:23.000000 amiya-0.0.4/src/amiya/exceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.438618 amiya-0.0.4/src/amiya/module_utilities/
+-rw-rw-rw-   0        0        0        0 2024-05-21 21:22:58.000000 amiya-0.0.4/src/amiya/module_utilities/__init__.py
+-rw-rw-rw-   0        0        0     3429 2024-05-22 05:06:23.000000 amiya-0.0.4/src/amiya/module_utilities/continuous_click_controller.py
+-rw-rw-rw-   0        0        0     3168 2024-05-12 22:48:48.000000 amiya-0.0.4/src/amiya/module_utilities/cursor_controller.py
+-rw-rw-rw-   0        0        0     1341 2024-05-22 19:53:25.000000 amiya-0.0.4/src/amiya/module_utilities/dev_features.py
+-rw-rw-rw-   0        0        0     2849 2024-05-20 20:38:47.000000 amiya-0.0.4/src/amiya/module_utilities/power_controller.py
+-rw-rw-rw-   0        0        0     1039 2024-05-22 02:00:47.000000 amiya-0.0.4/src/amiya/module_utilities/search_controller.py
+-rw-rw-rw-   0        0        0     6122 2024-05-22 02:07:44.000000 amiya-0.0.4/src/amiya/module_utilities/url_tracker.py
+-rw-rw-rw-   0        0        0     8832 2024-05-12 16:53:49.000000 amiya-0.0.4/src/amiya/module_utilities/volume_controller.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.439616 amiya-0.0.4/src/amiya/pixel_calculator/
+-rw-rw-rw-   0        0        0        0 2024-04-19 04:01:16.000000 amiya-0.0.4/src/amiya/pixel_calculator/__init__.py
+-rw-rw-rw-   0        0        0     1695 2024-05-18 02:23:07.000000 amiya-0.0.4/src/amiya/pixel_calculator/pixel_calculator.py
+-rw-rw-rw-   0        0        0     2825 2024-05-22 01:48:14.000000 amiya-0.0.4/src/amiya/pixel_calculator/resolution_detector.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.443618 amiya-0.0.4/src/amiya/resources/
+-rw-rw-rw-   0        0        0    94080 2024-04-13 19:09:50.000000 amiya-0.0.4/src/amiya/resources/amiya-cli-2.png
+-rw-rw-rw-   0        0        0   104680 2024-04-13 19:09:37.000000 amiya-0.0.4/src/amiya/resources/amiya-cli-3.png
+-rw-rw-rw-   0        0        0   254392 2024-05-01 05:56:34.000000 amiya-0.0.4/src/amiya/resources/amiya-cli-4.png
+-rw-rw-rw-   0        0        0    46585 2024-04-13 19:10:01.000000 amiya-0.0.4/src/amiya/resources/amiya-cli.png
+-rw-rw-rw-   0        0        0   166735 2024-04-05 02:00:17.000000 amiya-0.0.4/src/amiya/resources/amiya.png
+-rw-rw-rw-   0        0        0   197822 2024-04-05 17:56:21.000000 amiya-0.0.4/src/amiya/resources/amiya_with_border.png
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.444616 amiya-0.0.4/src/amiya/resources/code_snippets/
+-rw-rw-rw-   0        0        0    60828 2024-04-13 19:08:35.000000 amiya-0.0.4/src/amiya/resources/code_snippets/add-app.png
+-rw-rw-rw-   0        0        0    78155 2024-04-13 19:08:59.000000 amiya-0.0.4/src/amiya/resources/code_snippets/add-tag.png
+-rw-rw-rw-   0        0        0    25735 2024-04-13 19:09:12.000000 amiya-0.0.4/src/amiya/resources/code_snippets/start.png
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.445616 amiya-0.0.4/src/amiya/scheduler/
+-rw-rw-rw-   0        0        0        0 2024-04-23 03:48:30.000000 amiya-0.0.4/src/amiya/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     4458 2024-04-23 03:07:35.000000 amiya-0.0.4/src/amiya/scheduler/scheduler.py
+-rw-rw-rw-   0        0        0      934 2024-04-22 21:49:58.000000 amiya-0.0.4/src/amiya/scheduler/scheduler_config_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.448615 amiya-0.0.4/src/amiya/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-10 04:03:44.000000 amiya-0.0.4/src/amiya/utils/__init__.py
+-rw-rw-rw-   0        0        0     2182 2024-05-24 19:40:52.000000 amiya-0.0.4/src/amiya/utils/constants.py
+-rw-rw-rw-   0        0        0    13516 2024-05-24 19:08:48.000000 amiya-0.0.4/src/amiya/utils/helper.py
+-rw-rw-rw-   0        0        0     1026 2024-05-22 03:12:05.000000 amiya-0.0.4/src/amiya/utils/json_handler.py
+-rw-rw-rw-   0        0        0     1415 2024-04-10 04:03:43.000000 amiya-0.0.4/src/amiya/utils/pynput_mapping.py
+drwxrwxrwx   0        0        0        0 2024-05-24 19:44:21.448615 amiya-0.0.4/src/amiya.egg-info/
+-rw-rw-rw-   0        0        0     8183 2024-05-24 19:44:21.000000 amiya-0.0.4/src/amiya.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2691 2024-05-24 19:44:21.000000 amiya-0.0.4/src/amiya.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 19:44:21.000000 amiya-0.0.4/src/amiya.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-24 19:44:21.000000 amiya-0.0.4/src/amiya.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      117 2024-05-24 19:44:21.000000 amiya-0.0.4/src/amiya.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 19:44:21.000000 amiya-0.0.4/src/amiya.egg-info/top_level.txt
```

### Comparing `amiya-0.0.3/LICENSE` & `amiya-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/setup.py` & `amiya-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 # SOFTWARE.
 
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='amiya',
-    version='0.0.3',
+    version='0.0.4',
     author='Kevin L.',
     author_email='kevinliu@vt.edu',
     description='A lightweight cross-platform automation tool for games and daily tasks!',
     long_description=open('README.md', encoding='utf-8').read() if os.path.exists('README.md') else '',
     long_description_content_type="text/markdown",
     url='http://github.com/rezeroe/amiya',
     package_dir={'': 'src'},                                                            # Tell setuptools that all packages are under src
     packages=find_packages(where='src'),                                                # Find packages in src directory
     install_requires=open('requirements.txt', encoding='utf-8').read().splitlines(),    # List of dependencies
     python_requires='>=3.6, <4',
     entry_points={
         'console_scripts': [
-            'amiya=amiya.entrypoints.entrypoints:start_amiya_cli_as_admin',
+            'amiya=amiya.entrypoints.entrypoints:start_amiya',
         ],
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Development Status :: 4 - Beta'
```

### Comparing `amiya-0.0.3/src/amiya/__init__.py` & `amiya-0.0.4/src/amiya/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/amiya.py` & `amiya-0.0.4/src/amiya/amiya.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/apps_manager/__init__.py` & `amiya-0.0.4/src/amiya/apps_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/apps_manager/app.py` & `amiya-0.0.4/src/amiya/apps_manager/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,47 +3,47 @@
 import json
 import time
 import psutil
 import subprocess
 from pathlib import Path
 from amiya.utils.constants import APPS_DIRECTORY, FOCUS_PID_EXE
 from amiya.exceptions.exceptions import *
-from amiya.utils.helper import WindowUtils, aprint
+from amiya.utils.helper import WindowUtils, aprint, LogType, color_cmd, is_admin, Printer
 from amiya.automation_handler.automation_controller import AutomationController
-from amiya.apps_manager.sync_controller.sys_uuid_controller import SysUUIDController
+from amiya.apps_manager.sync_controller.sys_uuid_controller import SYSTEM_UUID
+from amiya.utils.helper import HashCalculator
 
 APP_AUTOMATION_DIRNAME          = "automation"
 APP_CONFIG_FILENAME             = "app-config.json"
 
 class App:
     def __init__(
         self, 
         name        : str, 
-        exe_path    : str, 
-        tags        : list = [], 
-        sys_uuid    : str = SysUUIDController.system_uuid,
+        exe_path    : str,
         new         : bool = False
     ):
         self.id         = None      # Assigned automatically by the AppManager at creation
         self.name       = name
         self.exe_path   = Path(self.__parse_exe_path(exe_path))
-        self.tags       = tags
         self.verified   = self.__verify_app_path()
-        self.sys_uuid   = sys_uuid  # Used to identify whether the application is synced with the current machine
-        
+        self.exe_hash   = HashCalculator.calculate_file_hash(self.exe_path) if self.verified else None
+        self.tags       = []
+        self.sys_uuid   = SYSTEM_UUID  # Used to identify whether the application is synced with the current machine
+
         # Note that the process variable is a snapshot of the application's process. 
         # It is not always (and most likely not) up-to-date as the program continues to run. 
         # This variable is only updated when is_running() is called and therefore this variable 
         # should NEVER be used to identify the current activity/status of the application.
         #
         # This variable should ONLY be used to identify the initial status of the application
         # as its started since any callback to is_running() (while a new instance of the application
         # is created) will overwrite the previous process.
         #
-        # Use get_app_process() instead.
+        # Use get_app_process() instead to get the application's current process.
         self.process: psutil.Process = None
     
         self.app_config_dirpath     = os.path.join(APPS_DIRECTORY, self.get_reformatted_app_name())
         self.app_config_filepath    = os.path.join(self.app_config_dirpath, APP_CONFIG_FILENAME)
         self.app_automation_dirpath = os.path.join(self.app_config_dirpath, APP_AUTOMATION_DIRNAME)
         
         self.new = new
@@ -86,25 +86,32 @@
     # =======================================
     # ============| APP DRIVER | ============
     # =======================================
 
     def run(self) -> bool:
         # If the application is already running
         if self.is_running():
-            self.bring_to_foreground()
-            return True
-        
+            if is_admin():
+                self.bring_to_foreground()
+                return True
+            else:
+                ctext = Printer.to_lightred("already running")
+                aprint(f"[PID {self.process.pid}] Application `{self.name}` is {ctext} in the background.")
+                raise AmiyaExit()
+
         # If the application is not running, then start the application
-        if self.verified == True:   
-            subprocess.Popen([self.exe_path], shell=True)
+        if self.verified:
+            process = subprocess.Popen([self.exe_path], shell=True)
             
             if self.wait_to_start():
                 self.bring_to_foreground()
                 return True
+
             return False
+        
         else:
             raise Amiya_AppInvalidPathException(path=self.exe_path)
 
     def wait_to_start(self) -> bool:
         TIMEOUT = 30
         starting_time = time.time()
         while time.time() - starting_time < TIMEOUT:
@@ -113,15 +120,15 @@
             time.sleep(1)
         return False
 
     def is_running(self, timeout: int = 0) -> bool:
         if timeout == 0:
             return self.get_app_process() != None
         
-        # Timeout will ensure the application is still running after timeout seconds.
+        # Timeout will ensure the application is still running after timeout seconds
         if self.get_app_process() != None:
             time.sleep(timeout)
             return self.get_app_process() != None
         return False
     
     def get_app_process(self) -> psutil.Process:
         APP_EXE_NAME = os.path.basename(self.exe_path)
@@ -133,55 +140,78 @@
                         self.process = app_process
                         return app_process
                     
                 except Exception as ex:
                     raise AmiyaBaseException(f"Failed to identify the app's process due to an unknown error ({ex}).")
         return None
     
+    def get_app_process(self) -> psutil.Process:
+        APP_EXE_NAME = os.path.basename(self.exe_path)
+        for p in psutil.process_iter(['pid', 'name', 'exe']):
+            try:
+                if APP_EXE_NAME.replace(".exe", "") in p.info['name']:
+                    app_process = psutil.Process(p.info['pid'])
+                    if (app_process.is_running()) and (Path(app_process.exe()) == Path(self.exe_path)):
+                        self.process = app_process
+                        return app_process
+                        
+            except Exception as ex:
+                raise AmiyaBaseException(f"Failed to identify the app's process due to an unknown error ({ex}).")
+        return None
     
     def bring_to_foreground(self):
         try:
             TIMEOUT = 10
             start_time = time.time()
             while time.time() - start_time < TIMEOUT:
                 if self.is_running():
+                    
                     success = WindowUtils.bring_to_foreground(self.process.pid)
                     if success:
                         return
-        except Exception as ex:
-            raise AmiyaBaseException(f"The app '{self.name}' is currently not running, therefore can't be brought to foreground ({ex}).")
+                    else:
+                        pass # Continue to try to focus on app
+                else:
+                    raise Amiya_AppStoppedUnexpectedly()
+        
+        except Amiya_AppStoppedUnexpectedly as ex:
+            raise AmiyaBaseException(f"The app '{self.name}' stopped unexpectedly. Therefore, it can't be brought to the foreground ({ex}).")
 
-        raise AmiyaBaseException(f"The app '{self.name}' cannot be brought to foreground due to an unknown error.") 
+        raise AmiyaBaseException(f"The app '{self.name}' cannot be brought to the foreground due to an unknown error.") 
 
     # ==========================================
     # ============| APP UTILITIES | ============
     # ==========================================
 
     def to_json(self):
         return {
             "id"        : self.id,
             "name"      : self.name,
             "exe_path"  : str(self.exe_path),
+            "exe_hash"  : str(self.exe_hash),
             "tags"      : self.tags,
             "verified"  : self.verified,
             "sys_uuid"  : self.sys_uuid
         }
 
     @staticmethod
     def read_json(app_config):
         try:
             with open(app_config, "r") as rf:
                 config = json.load(rf)
                 app = App(
                     config["name"], 
-                    config["exe_path"], 
-                    config["tags"],
-                    config["sys_uuid"]
+                    config["exe_path"],
+                    new = False
                 )
-                app.id = int(config["id"])
+                app.id       = int(config["id"])
+                app.tags     = config["tags"]
+                app.exe_hash = config["exe_hash"]
+                app.sys_uuid = config["sys_uuid"]
+                
                 return app
         except Exception as ex:
             raise ex
         
     def add_tag(self, tag_name):
         self.tags.append(tag_name)
         
@@ -201,19 +231,22 @@
     
     def set_new_path(self, new_path):
         # Used for syncing apps across different machines only
         self.exe_path = Path(new_path)
         self.verified = self.__verify_app_path()
     
     def set_new_uuid(self):
-        self.sys_uuid = SysUUIDController.get_system_uuid()
+        self.sys_uuid = SYSTEM_UUID
     
     # ==========================================
     # ==========| HELPER FUNCTIONS | ===========
     # ==========================================
     def __parse_exe_path(self, exe_path: str):
-        return exe_path.replace('"', "").strip()
+        exe_path = exe_path.replace('"', "").strip()
+        if not exe_path.endswith(".exe"):
+            aprint("The path should point to an executable ending with .exe\n> Example: E:/Star Rail/launcher.exe", log_type=LogType.ERROR); raise AmiyaExit()
+        return exe_path
     
     def __verify_app_path(self):
         return self.exe_path.exists()
```

### Comparing `amiya-0.0.3/src/amiya/apps_manager/apps_manager.py` & `amiya-0.0.4/src/amiya/apps_manager/apps_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import json
 import shutil
 import time
 import signal
 from termcolor import colored
 from amiya.apps_manager.app import App, APP_CONFIG_FILENAME
 from amiya.apps_manager.apps_viewer import AppsViewer
-from amiya.utils.constants import APPS_DIRECTORY
+from amiya.utils.constants import APPS_DIRECTORY, AMIYA_PID
 from amiya.exceptions.exceptions import *
 from amiya.utils.helper import *
 from amiya.automation_handler.units.sequence import AutomationSequence
 from amiya.automation_handler.automation_viewer import AutomationViewer
 from amiya.apps_manager.safety_monitor import SafetyMonitor
 from amiya.apps_manager.sync_controller.sync_controller import AppSyncController
-from amiya.apps_manager.sync_controller.sys_uuid_controller import SysUUIDController
+from amiya.apps_manager.sync_controller.sys_uuid_controller import SYSTEM_UUID
+from amiya.module_utilities.power_controller import PowerUtils
 
 # from elevate import elevate; elevate()
 
 class AppsManager:
     os.system("")  # Enables ANSI escape characters in terminal
     
     def __init__(self, verbose=True):
@@ -34,19 +35,44 @@
         apps_name_list = os.listdir(APPS_DIRECTORY)
         apps_dict: dict[int, App] = dict()
         
         for app_name in apps_name_list:
             app_config = os.path.join(APPS_DIRECTORY, app_name, APP_CONFIG_FILENAME)
             if os.path.isfile(app_config):
                 app = App.read_json(app_config)
+                app = self.__update_hash(app)
                 apps_dict[app.id] = app
-                
+
         return apps_dict
     
-    
+    def __update_hash(self, app: App):
+        # Updates application executable's hash value automatically every time when the apps are loaded.
+        # 
+        # Syncing logic with hash:
+        # If the hash is different, path is the same: auto update exe hash
+        # Elif hash is the same, path is different (exe_name the same): force `sync`
+        # Elif both the hash and path are different (exe_name the same): force `sync`
+        # Elif hash is null: unable to `sync`
+        
+        if app.verified:
+            curr_app_exe_hash = HashCalculator.calculate_file_hash(app.exe_path)
+            if curr_app_exe_hash != app.exe_hash:
+                app.exe_hash = curr_app_exe_hash
+                app.save_app_config()
+        else:
+            # If the application's path does not exist on the current machine, do nothing.
+            # When the apps are loaded, if a path doesn't exist, then the previous hash should
+            # presist until the path is corrected and then the hash will automatically reset.
+            # If the hash is set to None on app load, then the application won't be synced 
+            # properly the next run. 
+            pass
+
+        return app
+   
+   
     # ======================================
     # ===========| CREATE APPS | ===========
     # ======================================
     
     def create_app(self, name, exe_path):
         app = App(name, exe_path, new=True)             # Create a new app object
         app.id = self.__get_next_app_id()               # Assign ID to app (int)
@@ -152,33 +178,55 @@
             app = self.apps[int(user_input)]
         else:                                   # If user provided an application tag
             tag = self.__parse_tag(tag)
             app = self.get_app_by_tag(tag)
         
         self.__safe_start_app(app)
     
+    
     def __safe_start_app(self, app: App):
-        ret = app.run()
+        aprint(f"Starting application {app.name}...", end="\r")
+        
+        try:
+            ret = app.run()
+        except Amiya_AppInvalidPathException as ex:    # Application path invalid
+            aprint(ex.message, log_type=LogType.ERROR); raise AmiyaExit()
+        
         if ret == True:
             aprint(f"[PID {app.process.pid}] Application '{app.name}' started successfully!")
         else:
             aprint(f"Application '{app.name}' failed to start.", log_type=LogType.ERROR); raise AmiyaExit()
             
             
     # ======================================
     # ==========| TERMINATE APP | ==========
     # ======================================
-         
+    
     def __safe_terminate_current_app(self):
         pid = SafetyMonitor.get_focused_pid()
+        
         try:
-            os.kill(pid, signal.SIGTERM)  # Send the SIGTERM signal to gracefully terminate the process
-            aprint(f"Current application (PID {pid}) has been closed.")
-        except OSError as e:
-            aprint(f"Failed to terminate process with PID {pid}: {e}", log_type=LogType.ERROR)
+            app_process = psutil.Process(pid)
+            app_name = app_process.name()
+        except:
+            aprint("Unable to terminate application because it is already closed.", log_type=LogType.ERROR); raise AmiyaExit()
+        
+        try:
+            if app_process.is_running():
+                app_parent_pid = app_process.ppid()                                 # Get current focused process' parent PID
+                
+                app_process.kill()                                                  # Terminate the app process
+                aprint(f"Application `{app_name}` (PID {pid}) has been closed.")
+                
+                # if AMIYA_PID != app_parent_pid:                                     # Get PPID != module PID, kill parent PID (most likely a launcher of sort)
+                #     time.sleep(3)
+                #     success = ProcessHandler.kill_pid(app_parent_pid)
+
+        except OSError as ex:
+            aprint(f"Failed to terminate process with PID {pid}: {ex}", log_type=LogType.ERROR); raise AmiyaExit()
 
 
     # ======================================
     # ============| SHOW APPS | ============
     # ======================================
 
     def show_apps(self):
@@ -266,35 +314,38 @@
             app = self.get_app_by_tag(tag)
             
         text = f"Application Configuration:"
         text += f"\nApp Name: {app.name}"
         text += f"\nApp ID: {app.id}"  
         text += f"\nApp Tags: {app.tags}"
         text += f"\nApp Config Directory: {app.app_config_dirpath}" 
+        text += f"\nApp Executable Hash: {app.exe_hash}"
         text += f"\nApp Configuration System UUID: {app.sys_uuid}"  
         aprint(text)
         
     
     def __initial_setup(self):
         if not os.path.isdir(APPS_DIRECTORY):
             os.mkdir(APPS_DIRECTORY)
             
     def __get_next_app_id(self) -> int:
+        if len(self.apps) == 0:
+            return 1
         return max(self.apps.keys()) + 1
 
     def get_app_with_id(self, user_input_id: str) -> App:
         try:
             app = self.apps[int(user_input_id)]
         except KeyError:
             aprint(f"Your input (ID {user_input_id}) does not correspond to any apps.", log_type=LogType.ERROR); raise AmiyaExit()
         except ValueError:
             aprint(f"Expected an ID (such as 0 or 1) but got '{user_input_id}'.", log_type=LogType.ERROR); raise AmiyaExit()
         return app
     
-    def get_app_by_tag(self, tag) -> App | None:
+    def get_app_by_tag(self, tag) -> App:
         for _, app in self.apps.items():
             if tag in app.tags:
                 return app
         raise Amiya_NoSuchTagException(tag)
             
     def __verify_non_empty_apps_dir(self):
         if len(self.apps) == 0:
@@ -351,15 +402,23 @@
         )
         self.__print_sequence(new_sequence_recorded)
         
 
     # =================================================
     # ================| RUN SEQUENCES | ===============
     # =================================================
-    def run_sequence(self, tag: str = None, seq_name: str = None, global_delay: int = 0, terminate_on_finish: bool = False, no_confirmation: bool = False):
+    def run_sequence(
+        self, tag: str = None, 
+        seq_name: str = None, 
+        global_delay: int = 0, 
+        terminate_on_finish: bool = False, 
+        no_confirmation: bool = False,
+        sleep_afterward: bool = False,
+        shutdown_afterward: bool = False
+    ):
         self.__verify_non_empty_apps_dir()
         
         if tag != None:
             tag = self.__parse_tag(tag)
             app = self.get_app_by_tag(tag)
         else:
             self.print_apps()
@@ -395,23 +454,31 @@
         app_process = app.get_app_process()                                    # Get application's process
         safety_monitor = SafetyMonitor(app_process)                            # Creates a safety monitor object for sequence execution safety (must be created after the app is started)
         self.__safe_execute_sequence(sequence, safety_monitor)                 # Runs the sequence (with the safety monitor)
 
         print("")
         aprint(f"[Automation {sequence.sequence_name}] Run Completed!", log_type=LogType.SUCCESS)
         
+        # ============== AFTER FINISHING ==============
         if terminate_on_finish:
             self.__safe_terminate_current_app()
         
+        if sleep_afterward:
+            power_utils = PowerUtils()
+            power_utils.sleep_pc(delay=10)
+        elif shutdown_afterward:
+            power_utils = PowerUtils()
+            power_utils.shutdown_pc(delay=10)
+            
         
     def __safe_execute_sequence(self, sequence: AutomationSequence, safety_monitor: SafetyMonitor):
         try:
             sequence.execute(safety_monitor)
         except Amiya_AppNotFocusedException:
-            aprint("[Amiya Safety-Monitor] The application is unfocused during an automation sequence. Automation stopped.", log_type=LogType.ERROR)
+            aprint("[Safety-Monitor] The application is unfocused during an automation run. Automation terminated.", log_type=LogType.ERROR)
             raise AmiyaExit()
      
     def __safe_get_sequence(self, app: App, sequence_name: str) -> AutomationSequence:
         sequence = app.automation_controller.get_sequence(sequence_name)
         if sequence == None:
             aprint(f"No sequence with name '{sequence_name}' exists. Exiting.", log_type=LogType.ERROR); raise AmiyaExit()
         return sequence
@@ -453,37 +520,37 @@
     # ==================| SYNC APPS | =================
     # =================================================
     
     def sync_apps(self, verbose=True):
         self.__verify_non_empty_apps_dir()
         
         if verbose:
-            aprint(f"Sync all {len(self.apps)} applications on this machine? (This may take a while) [y/n] ", log_type=LogType.WARNING, end="")
+            aprint(f"Sync {len(self.apps)} applications on this machine? (This may take a while) [y/n] ", log_type=LogType.WARNING, end="")
             if input().strip().lower() != "y": return
         
         sync_controller = AppSyncController()
-        
+
         apps = list(self.apps.values())
-        for i in progressbar(range(len(apps)), f"Syncing: ", 40):
-            app: App = apps[i]
-            success = sync_controller.sync(app)
-            self.apps[app.id] = app
-            
+        for app in apps:
+            aprint(f"Syncing application `{app.name}`... ", end="")
+            synced_app = sync_controller.sync(app)
+            self.apps[app.id] = synced_app
+            print("Done")
         self.print_apps()
         
-        found = len([app for app in apps if app.verified == True])
+        found = len([app for app in self.apps.values() if app.verified == True])
         cmd = color_cmd("amiya cleanup")
-        aprint(f"Sync Complete - successfully synced {found}/{len(apps)} applications.\n\nTo cleanup unverified applications (unavailable on this machine), run '{cmd}'")
-        print("")
+        aprint(f"Sync Complete - successfully synced {found}/{len(apps)} applications.\n\nTo cleanup unverified applications (unavailable on this machine), run '{cmd}'\n")
         
     def verify_apps_synced(self) -> bool: 
         # Verify whether applications configured with Amiya's apps manager needs to be synced with the current machine.
         # Sync is only required when transferring the apps manager's configuration data (apps) on to a new machine.
         for app in self.apps.values():
-            if SysUUIDController.system_uuid != app.sys_uuid:
+            if SYSTEM_UUID != app.sys_uuid:
+                aprint(f"App not synced: {app.name} ({app.sys_uuid})")
                 return False
         return True
         
     def cleanup_apps(self):
         unverified_apps = [app for app in self.apps.values() if app.verified == False]
         if len(unverified_apps) == 0:
             aprint('There is no unverified application to cleanup!'); return
```

### Comparing `amiya-0.0.3/src/amiya/apps_manager/apps_viewer.py` & `amiya-0.0.4/src/amiya/apps_manager/apps_viewer.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/apps_manager/safety_monitor.py` & `amiya-0.0.4/src/amiya/apps_manager/safety_monitor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import time
 import psutil
 import subprocess
 from amiya.utils.helper import *
-from amiya.utils.constants import GET_FOCUSED_PID_EXE
-from amiya.exceptions.exceptions import AmiyaBaseException, Amiya_AppNotFocusedException
+from amiya.utils.constants import GET_FOCUSED_PID_EXE, DEVELOPMENT
+from amiya.exceptions.exceptions import AmiyaBaseException, Amiya_AppNotFocusedException, AmiyaExit
 
 class SafetyMonitor:
     def __init__(self, app_process: psutil.Process):
         self.app_process = app_process
         self.cached_pids: set[int] = set()
         self.monitor_create_time = time.time()  # Time when the SafetyMonitor is created
     
@@ -19,23 +19,21 @@
         '''
         focused_pid = SafetyMonitor.get_focused_pid()
         
         # If PID == original APP's PID, return True
         if focused_pid == self.app_process.pid:
             return True
 
-        # print(f"Focused {focused_pid}")
-        # print(f"App: {self.app_process.pid}")
-        # print(f"Cached: {self.cached_pids}")
-
         if focused_pid not in self.cached_pids:
             self.__update_cached_pids()  # Update the cache if PID not found initially
             
             if focused_pid not in self.cached_pids:
-                aprint(f"Focused PID: [{focused_pid}], Original App PID: [{self.app_process.pid}], Cached PID: {self.cached_pids}", log_type=LogType.ERROR, new_line_no_prefix=False)
+                if DEVELOPMENT:
+                    print("")
+                    aprint(f"Focused PID: {focused_pid}, Original App PID: {self.app_process.pid}, Cached PIDs: {self.cached_pids}", log_type=LogType.ERROR, new_line_no_prefix=False)
                 raise Amiya_AppNotFocusedException()
             else:
                 return True
         else:
             return True
         
 
@@ -51,22 +49,31 @@
         except psutil.NoSuchProcess:
             pass
         
         
     
     
     @staticmethod
-    def get_focused_pid() -> int|None:
-        result = subprocess.run([GET_FOCUSED_PID_EXE], capture_output=True, text=True)
+    def get_focused_pid(tries: int = 3) -> int:
+        # :param tries: specifies how many times to try on failed PID fetch attempts
+        if tries <= 0:
+            aprint(f"ERROR: get_focuse_pid() cannot be called with {tries} tries.", log_type=LogType.ERROR)
+            raise AmiyaExit()
+        
     
         pid = None
-        if result.returncode == 0:
-            pid = result.stdout.strip()
-        else:
-            raise AmiyaBaseException(f"Embeded script 'GET_FOCUSED_PID' failed with return code {result.returncode}")
+        for _ in range(tries):
+            result = subprocess.run([GET_FOCUSED_PID_EXE], capture_output=True, text=True)
+            if result.returncode == 0:
+                pid = result.stdout.strip()
+                break
+            time.sleep(1)
+            
+        if pid == None:
+            raise AmiyaBaseException(f"Embeded script 'GET_FOCUSED_PID' failed after {tries} tries with return code {result.returncode}")
         
         try:
             pid = int(pid)
         except ValueError:
             raise AmiyaBaseException(f"Embeded script 'GET_FOCUSED_PID' failed to fetch PID. (Fetched PID {pid} cannot be converted into INT)")
     
         return pid
@@ -75,13 +82,8 @@
     def get_possible_pids(self) -> set:
         '''
         Get all PIDs from processes that got created after the monitor is created. 
         '''
         # for p in sorted(psutil.process_iter(), key=lambda x: x.create_time()):
         #     print(f"{p.name()}, {p.create_time()}, {p.pid}")
         
-        
-        # print(self.monitor_create_time)
-        
-        # print("\n\n")
-        
         return {p.pid for p in psutil.process_iter(['pid']) if p.create_time() > self.monitor_create_time}
```

### Comparing `amiya-0.0.3/src/amiya/apps_manager/sync_controller/sys_uuid_controller.py` & `amiya-0.0.4/src/amiya/apps_manager/sync_controller/sys_uuid_controller.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,13 +6,14 @@
     def get_system_uuid():
         try:
             result = subprocess.check_output('wmic csproduct get uuid', shell=True).decode()
             uuid = result.strip().split('\n')[1].strip()
             return uuid
         except Exception as e:
             return str(e)
-    
-    system_uuid = get_system_uuid()
 
     @staticmethod
     def print_uuid():
-        aprint(f"System UUID: {SysUUIDController.get_system_uuid()}")
+        aprint(f"System UUID: {SysUUIDController.get_system_uuid()}")
+
+
+SYSTEM_UUID = SysUUIDController.get_system_uuid()
```

### Comparing `amiya-0.0.3/src/amiya/automation_handler/__init__.py` & `amiya-0.0.4/src/amiya/automation_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/automation_handler/automation_config_handler.py` & `amiya-0.0.4/src/amiya/automation_handler/automation_config_handler.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/automation_handler/automation_controller.py` & `amiya-0.0.4/src/amiya/automation_handler/automation_controller.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/automation_handler/automation_recorder.py` & `amiya-0.0.4/src/amiya/automation_handler/automation_recorder.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/automation_handler/automation_viewer.py` & `amiya-0.0.4/src/amiya/automation_handler/automation_viewer.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/automation_handler/units/__init__.py` & `amiya-0.0.4/src/amiya/automation_handler/units/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/automation_handler/units/action.py` & `amiya-0.0.4/src/amiya/automation_handler/units/action.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/automation_handler/units/plate.py` & `amiya-0.0.4/src/amiya/automation_handler/units/plate.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/automation_handler/units/sequence.py` & `amiya-0.0.4/src/amiya/automation_handler/units/sequence.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/bin/focus_pid.exe` & `amiya-0.0.4/src/amiya/bin/focus_pid.exe`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/bin/get_active_pid.exe` & `amiya-0.0.4/src/amiya/bin/get_active_pid.exe`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/bin/get_window_size.exe` & `amiya-0.0.4/src/amiya/bin/get_window_size.exe`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/bin/scripts/focus_pid.c` & `amiya-0.0.4/src/amiya/bin/scripts/focus_pid.c`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/bin/scripts/get_window_size.c` & `amiya-0.0.4/src/amiya/bin/scripts/get_window_size.c`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/entrypoints/__init__.py` & `amiya-0.0.4/src/amiya/entrypoints/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/entrypoints/entrypoint_handler.py` & `amiya-0.0.4/src/amiya/entrypoints/entrypoint_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import multiprocessing
 import getpass
 import subprocess
+import tabulate, io
+from tabulate import tabulate
+import argparse
 
 from amiya.apps_manager.apps_manager import AppsManager
 from amiya.module_utilities.search_controller import SearchController
 from amiya.module_utilities.power_controller import PowerUtils
 from amiya.module_utilities.cursor_controller import CursorController
 from amiya.module_utilities.continuous_click_controller import ContinuousClickController
+from amiya.module_utilities.url_tracker import URLTracker
 from amiya.module_utilities.dev_features import DevController
 
 from amiya.exceptions.exceptions import *
 from amiya.utils.helper import *
 
 from amiya.scheduler.scheduler import AmiyaScheduler
 from amiya.apps_manager.sync_controller.sys_uuid_controller import SysUUIDController
 from amiya.utils import constants
-from amiya.utils.constants import VERSION, VERSION_DESC, AUTHOR, AUTHOR_DETAIL, REPOSITORY
+from amiya.utils.constants import COMMAND, VERSION, VERSION_DESC, AUTHOR, AUTHOR_DETAIL, REPOSITORY
 from amiya.module_utilities.volume_controller import AmiyaVolumeControllerUI, start_volume_control_ui
 
 
 
 class AmiyaEntrypointHandler:
     def __init__(self):
         self.apps_manager = AppsManager()
@@ -45,14 +49,16 @@
             )
         if args.refresh:
             self.dev_controller.refresh_objects()
         if args.code:
             self.dev_controller.open_dev_env()
         if args.isadmin:
             self.dev_controller.is_admin()
+        if args.home_dir:
+            self.dev_controller.verbose_home_dir()
     
     
     # =================================================
     # ====================| ABOUT | ===================
     # =================================================
     
     def version(self, args):
@@ -60,17 +66,21 @@
     
     def author(self, args):
         aprint(AUTHOR_DETAIL)
     
     def repo(self, args):
         aprint(REPOSITORY)
     
-    def print_help(self, args, parser):
-        help_cmd = color_cmd("help", with_quotes=True)
-        aprint(f"Command {help_cmd} is not implemented.")
+    # def print_help(self, args, parser):
+    #     # help_cmd = color_cmd("help", with_quotes=True)
+    #     # aprint(f"Command {help_cmd} is not implemented.")
+        
+    #     parser.print_help()
+        
+
     
     # =================================================
     # ============| ADD/REMOVE/SHOW APPS | ============
     # =================================================
     
     def add_app(self, args):
         self.apps_manager.create_app_automated()
@@ -115,15 +125,17 @@
 
     def run_automations_sequences(self, args):
         self.apps_manager.run_sequence(
             tag=args.tag, 
             seq_name=args.seq_name,
             global_delay=args.global_delay,
             terminate_on_finish=args.terminate,
-            no_confirmation=args.no_confirmation
+            no_confirmation=args.no_confirmation,
+            sleep_afterward=args.sleep,
+            shutdown_afterward=args.shutdown
         )
 
 
     # =================================================
     # ==========| APP UTILITY FEATURES | ==============
     # =================================================
 
@@ -173,15 +185,15 @@
             self.cursor_controller = CursorController(verbose_hex=False)
         
         self.cursor_controller.track_cursor()
 
 
     def click_continuously(self, args):
         cc_controller = ContinuousClickController()
-        cc_controller.click_continuously(args.count, args.delay, args.hold_time, args.start_after, args.quite)
+        cc_controller.click_continuously(args.count, args.interval, args.randomize_by, args.hold_time, args.start_after, args.quiet)
 
     def elevate(self, args):
         if is_admin():
             aprint("Already running as admin.")
             return
         
         if args.explain:
@@ -201,17 +213,24 @@
             if ui.lower() != "y":
                 return
         
         script = os.path.abspath(sys.argv[0])
         params = ' '.join([script])
         try:
             subprocess.run(["powershell", "-Command", f"Start-Process -Verb runAs {params}"])
+            aprint("Permissions granted. Please use the new terminal with the Amiya-CLI that opened.")
         except Exception as e:
             aprint(f"Failed to elevate privileges: {e}")
-        sys.exit(0)
+        raise AmiyaExit()
+
+
+    def track_url(self, args):
+        url_monitor = URLTracker()
+        url_monitor.safe_track_changes(args.url, args.interval, args.open)
+
 
     # =================================================
     # ================| SCHEDULER | ===================
     # =================================================
 
     # def run_scheduler(self, args):
     #     self.scheduler.run_scheduler()
@@ -291,38 +310,55 @@
         constants.CLI_MODE = True
         
         # ==============| PRINT TITLE |==============
         clear_screen()
         self.print_title()
         self.print_init_help()
         
+        cli_env_alert = False
         # ================| CLI LOOP |================
         while True:
             try:
                 amiya_cli = colored(f"{DatetimeHandler.get_time_str()} Amiya-CLI", "dark_grey")
                 print(f"[{amiya_cli}] > ", end="", flush=True)
                 
                 user_input = input().strip()
                 continue_loop = self.check_custom_commands(user_input)
                 if continue_loop == 1:
                     continue
                 elif continue_loop == 2:
                     break
                 
+
+                # Verify that the stdout and stderr aren't closed
+                if sys.stdout.closed or sys.stderr.closed:
+                    text = "STDOUT and STDERR" if sys.stdout.closed and sys.stderr.closed \
+                        else "STDOUT" if sys.stdout.closed \
+                        else "STDERR"
+                    aprint(f"System {text} has been closed unexpectedly. Exiting Amiya CLI environment...")
+                    sys.exit()
+
                 
-        # =============| PARSE ARGUMENT |=============    
+        # =============| PARSE ARGUMENT |=============
+                if user_input.startswith(COMMAND):
+                    user_input = user_input.lstrip(COMMAND).strip() 
+                    
+                    if not cli_env_alert:
+                        aprint(Printer.to_lightgrey(f"Currently in the Amiya CLI environment. You may call `{user_input}` directly without the `amiya` prefix."))
+                        cli_env_alert = not cli_env_alert
+                    
                 args = parser.parse_args(user_input.split())
                 if hasattr(args, 'func'):
                     try:
                         args.func(args)
                     except AmiyaExit:
                         continue
-                    # except AmiyaBaseException as ex:
-                    #     aprint(ex, log_type=LogType.ERROR)
-                    #     continue
+                    # except Exception as ex:
+                    #     aprint(f"{type(ex)}: {ex}. Exiting...", log_type=LogType.ERROR)
+                    #     exit()
                 else:
                     parser.print_help()
             
             
         # ==============| ON EXCEPTION |==============
             except KeyboardInterrupt:
                 # print("\nNote: Type 'exit' to quit.")
```

### Comparing `amiya-0.0.3/src/amiya/entrypoints/entrypoints.py` & `amiya-0.0.4/src/amiya/entrypoints/entrypoints.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,183 +5,243 @@
 import argparse
 
 import ctypes
 import subprocess
 
 from termcolor import colored
 from amiya.entrypoints.entrypoint_handler import AmiyaEntrypointHandler
-from amiya.utils.helper import aprint, atext, verify_platform, is_admin, Printer
+from amiya.entrypoints.help_format_handler import HelpFormatHandler
+from amiya.utils.helper import aprint, verify_platform, is_admin, Printer, color_cmd
+from amiya.utils.constants import COMMAND
 from amiya.exceptions.exceptions import AmiyaOSNotSupported, AmiyaExit
 
 
 class AmiyaArgParser(argparse.ArgumentParser):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.groups = []
+
+    def add_group(self, title, description=None):
+        group = {'title': title, 'description': description, 'parsers': []}
+        self.groups.append(group)
+        return group
+
+    def add_parser_to_group(self, group, parser):
+        group['parsers'].append(parser)
+        
     def error(self, message):
         command = message.split("'")[1] if "invalid choice:" in message else None
         helpt = Printer.to_purple("help")
         aprint(f"Command not recognized: {command}\nType '{helpt}' for commands list")
         self.exit(2)
-        
-        
-
 
 
 def start_amiya():
     entrypoint_handler = AmiyaEntrypointHandler()
+    help_format_handler = HelpFormatHandler()
     
-    parser = AmiyaArgParser(prog='amiya', description="Amiya CLI Automation Package")
+    parser = AmiyaArgParser(prog=COMMAND, description="Amiya CLI Automation Package")
     subparsers = parser.add_subparsers(dest='command', help='commands')
 
     help_parser = subparsers.add_parser('help', help='Show this help message and exit')
-    help_parser.set_defaults(func=lambda args: entrypoint_handler.print_help(args, parser))
+    help_parser.set_defaults(func=lambda args: help_format_handler.print_help(args, parser))
 
     # =================================================
     # =================| DEVELOPMENT | ================
     # =================================================
-
-    start_parser = subparsers.add_parser('dev', help='[DEV] Developer\'s commands.')
-    start_parser.add_argument('--objects', '-obj', action='store_true', help='Show all controller objects and their addresses.')
-    start_parser.add_argument('--refresh', '-ref', action='store_true', help='Refresh all controller objects.')
-    start_parser.add_argument('--code', '-c', action='store_true', help='Open development environment with VSCode.')
-    start_parser.add_argument('--isadmin', '-ia', action='store_true', help='Show whether the main thread has admin access.')
-    start_parser.set_defaults(func=entrypoint_handler.DEV)
-
-
-    # =================================================
-    # ====================| ABOUT | ===================
-    # =================================================
-
-    start_parser = subparsers.add_parser('version', help='Verbose module version')
-    start_parser.set_defaults(func=entrypoint_handler.version)
+    dev_group = parser.add_group('Development', 'Developer\'s commands. Open available when [constants.DEVELOPMENT=True].')
+    
+    dev_parser = subparsers.add_parser('dev', 
+        help='[DEV] Developer\'s commands.',
+        description='[DEV] Developer\'s commands.'
+    )
+    dev_parser.add_argument('--objects', '-obj', action='store_true', help='Show all controller objects and their addresses.')
+    dev_parser.add_argument('--refresh', '-ref', action='store_true', help='Refresh all controller objects.')
+    dev_parser.add_argument('--code', '-c', action='store_true', help='Open development environment with VSCode.')
+    dev_parser.add_argument('--isadmin', '-ia', action='store_true', help='Show whether the main thread has admin access.')
+    dev_parser.add_argument('--home-dir', '-dir', action='store_true', help='Verbose module home directroy')
+    dev_parser.set_defaults(func=entrypoint_handler.DEV)
+    parser.add_parser_to_group(dev_group, dev_parser)
+
+    # ================================================
+    # ===================| ABOUT | ===================
+    # ================================================
+    
+    about_group = parser.add_group('About', 'Get information about the Amiya module in general.')
+    
+    version_parser = subparsers.add_parser('version', help='Verbose module version', description='Verbose module version')
+    version_parser.set_defaults(func=entrypoint_handler.version)
+    parser.add_parser_to_group(about_group, version_parser)
                               
-    start_parser = subparsers.add_parser('author', help='Verbose module author')
-    start_parser.set_defaults(func=entrypoint_handler.author)
+    author_parser = subparsers.add_parser('author', help='Verbose module author', description='Verbose module author')
+    author_parser.set_defaults(func=entrypoint_handler.author)
+    parser.add_parser_to_group(about_group, author_parser)
+    
+    repo_parser = subparsers.add_parser('repo', help='Verbose module repository link', description='Verbose module repository link')
+    repo_parser.set_defaults(func=entrypoint_handler.repo)
+    parser.add_parser_to_group(about_group, repo_parser)
     
-    start_parser = subparsers.add_parser('repo', help='Verbose module repository link')
-    start_parser.set_defaults(func=entrypoint_handler.repo)
 
     # =================================================
     # ============| ADD/REMOVE/SHOW APPS | ============
     # =================================================
 
-    start_parser = subparsers.add_parser('add-app', help='Add a new application')
-    start_parser.set_defaults(func=entrypoint_handler.add_app)
+    apps_group = parser.add_group('App Management', 'Add, remove, and show applications in Amiya\'s app configuration.')
     
-    start_parser = subparsers.add_parser('remove-app', help='Remove an existing application')
-    start_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application to remove')
-    start_parser.set_defaults(func=entrypoint_handler.remove_app)
+    add_app_parser = subparsers.add_parser('add-app', help='Add a new application', description='Add a new application')
+    add_app_parser.set_defaults(func=entrypoint_handler.add_app)
+    parser.add_parser_to_group(apps_group, add_app_parser)
+    
+    remove_app_parser = subparsers.add_parser('remove-app', help='Remove an existing application', description='Remove an existing application')
+    remove_app_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application to remove')
+    remove_app_parser.set_defaults(func=entrypoint_handler.remove_app)
+    parser.add_parser_to_group(apps_group, remove_app_parser)
     
-    show_apps_parser = subparsers.add_parser('show-apps', help='Show applications')
+    show_apps_parser = subparsers.add_parser('show-apps', help='Show applications', description='Show applications')
     show_apps_parser.add_argument('--short', '-s', action='store_true', help='Only show the app ID, name, and verification status')
     show_apps_parser.add_argument('--full-path', '-f', action='store_true', help='Show the full path of the applications')
     show_apps_parser.set_defaults(func=entrypoint_handler.show_apps)
+    parser.add_parser_to_group(apps_group, show_apps_parser)
+    
+    show_config_parser = subparsers.add_parser('show-config', help='Show application configuration directory', description='Show application configuration directory')
+    show_config_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application to show the configuration directory of')
+    show_config_parser.add_argument('--all', '-a', action='store_true', help='Show all configuration directory paths (including automation)')
+    show_config_parser.set_defaults(func=entrypoint_handler.show_app_config_dir)
+    parser.add_parser_to_group(apps_group, show_config_parser)
 
 
-    start_parser = subparsers.add_parser('show-config', help='Show application configuration directory')
-    start_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application to show the configuration directory of')
-    start_parser.add_argument('--all', '-a', action='store_true', help='Show all configuration directory paths (including automation)')
-    start_parser.set_defaults(func=entrypoint_handler.show_app_config_dir)
-
     # =================================================
     # =================| START APPS | =================
     # =================================================
     
-    start_parser = subparsers.add_parser('start', help='Start an application')
+    start_apps_group = parser.add_group('Application Launcher', 'Start or terminate applications from the CLI.')
+    
+    start_parser = subparsers.add_parser('start', help='Start an application', description='Start an application')
     start_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application to start')
     start_parser.set_defaults(func=entrypoint_handler.start)
+    parser.add_parser_to_group(start_apps_group, start_parser)
     
     
     # =================================================
     # ==============| ADD/REMOVE TAGS | ===============
     # =================================================
     
-    start_parser = subparsers.add_parser('add-tag', help='Add a new tag to an application')
-    start_parser.set_defaults(func=entrypoint_handler.add_tag)
-    
-    start_parser = subparsers.add_parser('remove-tag', help='Remove a tag from an application')
-    start_parser.set_defaults(func=entrypoint_handler.remove_tag)
+    tags_group = parser.add_group('Tag Management', 'Add or remove tags associated with applications configured with Amiya.')
     
+    add_tag_parser = subparsers.add_parser('add-tag', help='Add a new tag to an application', description='Add a new tag to an application')
+    add_tag_parser.set_defaults(func=entrypoint_handler.add_tag)
+    parser.add_parser_to_group(tags_group, add_tag_parser)
+    
+    remove_tag_parser = subparsers.add_parser('remove-tag', help='Remove a tag from an application', description='Remove a tag from an application')
+    remove_tag_parser.set_defaults(func=entrypoint_handler.remove_tag)
+    parser.add_parser_to_group(tags_group, remove_tag_parser)
     
     # =================================================
     # ========| RECORD/LIST/RUN AUTOMATION |===========
     # =================================================
     
-    start_parser = subparsers.add_parser('list-auto', help='List all the automation sequences of the application')
-    start_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application')
-    start_parser.set_defaults(func=entrypoint_handler.list_automation_sequences)
-    
-    start_parser = subparsers.add_parser('record-auto', help='[Admin Permission Req.] Record an automation sequences of the application')
-    start_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application')
-    start_parser.set_defaults(func=entrypoint_handler.record_automation_sequences)
-
-    
-    start_parser = subparsers.add_parser('run-auto', help='[Admin Permission Req.] Record an automation sequences of the application')
-    start_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application')
-    start_parser.add_argument('seq_name', nargs='?', default=None, help='Name of the sequence to run')
-    start_parser.add_argument('--global-delay', '-g', type=int, default=-1, help='Add a global delay to the sequence during execution')
-    start_parser.add_argument('--terminate', '-t', default=False, action='store_true', help='Terminate the application on automation completion')
-    start_parser.add_argument('--no-confirmation', '-nc', default=False, action='store_true', help='Run the automation without confirmation')
-    start_parser.set_defaults(func=entrypoint_handler.run_automations_sequences)
+    automation_group = parser.add_group('Automation', 'Record, show, and run automations in applications.')
+    
+    list_auto_parser = subparsers.add_parser('list-auto', help='List all the automation sequences of the application', description='List all the automation sequences of the application')
+    list_auto_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application')
+    list_auto_parser.set_defaults(func=entrypoint_handler.list_automation_sequences)
+    parser.add_parser_to_group(automation_group, list_auto_parser)
+    
+    record_auto_parser = subparsers.add_parser('record-auto', help='[Admin Permission Req.] Record an automation sequence of the application', description='[Admin Permission Req.] Record an automation sequence of the application')
+    record_auto_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application')
+    record_auto_parser.set_defaults(func=entrypoint_handler.record_automation_sequences)
+    parser.add_parser_to_group(automation_group, record_auto_parser)
+
+    run_auto_parser = subparsers.add_parser('run-auto', help='[Admin Permission Req.] Run an automation sequence of the application', description='[Admin Permission Req.] Run an automation sequence of the application')
+    run_auto_parser.add_argument('tag', nargs='?', default=None, help='Tag of the application')
+    run_auto_parser.add_argument('seq_name', nargs='?', default=None, help='Name of the sequence to run')
+    run_auto_parser.add_argument('--global-delay', '-g', type=int, default=-1, help='Add a global delay to the sequence during execution')
+    run_auto_parser.add_argument('--terminate', '-t', default=False, action='store_true', help='Terminate the application on automation completion')
+    run_auto_parser.add_argument('--no-confirmation', '-nc', default=False, action='store_true', help='Run the automation without confirmation')
+    run_auto_parser.add_argument('--sleep', default=False, action='store_true', help='Put PC to sleep after automation finishes (overwrites --shutdown)')
+    run_auto_parser.add_argument('--shutdown', default=False, action='store_true', help='Shutdown PC after automation finishes')
+    run_auto_parser.set_defaults(func=entrypoint_handler.run_automations_sequences)
+    parser.add_parser_to_group(automation_group, run_auto_parser)
     
     
     # =================================================
     # ==========| APP UTILITY FEATURES | ==============
     # =================================================
     
-    start_parser = subparsers.add_parser('sync', help='Sync configured applications on new machine OR auto configure application executable paths')
-    start_parser.set_defaults(func=entrypoint_handler.sync)
+    app_utility_group = parser.add_group('Sync Commands', 'Sync (auto-locate) and cleanup applications across different local machines.')
     
-    start_parser = subparsers.add_parser('cleanup', help='Remove all unverified applications')
-    start_parser.set_defaults(func=entrypoint_handler.cleanup)
+    sync_parser = subparsers.add_parser('sync', help='Sync configured applications on new machine OR auto configure application executable paths', description='Sync configured applications on new machine OR auto configure application executable paths')
+    sync_parser.set_defaults(func=entrypoint_handler.sync)
+    parser.add_parser_to_group(app_utility_group, sync_parser)
+    
+    cleanup_parser = subparsers.add_parser('cleanup', help='Remove all unverified applications', description='Remove all unverified applications')
+    cleanup_parser.set_defaults(func=entrypoint_handler.cleanup)
+    parser.add_parser_to_group(app_utility_group, cleanup_parser)
     
     
     # =================================================
     # =============| UTILITY FEATURES | ===============
     # =================================================
     
-    start_parser = subparsers.add_parser('search', help='Initiate a search on the default browser')
-    start_parser.add_argument('search_content', nargs='*', default=None, help='Content of the search')
-    start_parser.set_defaults(func=entrypoint_handler.search)
+    utility_group = parser.add_group('Utility', 'Other useful and easy-to-use utilities provided by the Amiya module.')
     
-    sleep_parser = subparsers.add_parser('sleep', help='Put the PC to sleep after X seconds')
+    search_parser = subparsers.add_parser('search', help='Initiate a search on the default browser', description='Initiate a search on the default browser')
+    search_parser.add_argument('search_content', nargs='*', default=None, help='Content of the search')
+    search_parser.set_defaults(func=entrypoint_handler.search)
+    parser.add_parser_to_group(utility_group, search_parser)
+    
+    sleep_parser = subparsers.add_parser('sleep', help='Put the PC to sleep after X seconds', description='Put the PC to sleep after X seconds')
     sleep_parser.add_argument('delay', nargs='?', type=int, default=0, help='Delay in seconds before sleep')
     sleep_parser.set_defaults(func=lambda args: entrypoint_handler.sleep(args, sleep_parser))
+    parser.add_parser_to_group(utility_group, sleep_parser)
     
-    shutdown_parser = subparsers.add_parser('shutdown', help='Shutdown PC after X seconds')
+    shutdown_parser = subparsers.add_parser('shutdown', help='Shutdown PC after X seconds', description='Shutdown PC after X seconds')
     shutdown_parser.add_argument('delay', nargs='?', type=int, default=0, help='Delay in seconds before shutdown')
     shutdown_parser.set_defaults(func=lambda args: entrypoint_handler.shutdown(args, shutdown_parser))
+    parser.add_parser_to_group(utility_group, shutdown_parser)
     
-    
-    start_parser = subparsers.add_parser('uuid', help='Display system UUID')
-    start_parser.set_defaults(func=entrypoint_handler.display_system_uuid)
-    
-    
-    start_parser = subparsers.add_parser('pixel', help='Track cursor position and color')
-    start_parser.add_argument('--color', '-c', action='store_true', help='Show pixel coordinate as well as the pixel\'s color hex value.')
-    start_parser.set_defaults(func=entrypoint_handler.track_cursor)
-    
-    
-    start_parser = subparsers.add_parser('volume', help='Open simple application volume control UI')
-    start_parser.set_defaults(func=entrypoint_handler.open_volume_control_ui)
-    
-    start_parser = subparsers.add_parser('click', help='Continuously click mouse.')
-    start_parser.add_argument('--count', '-c', type=int, default=-1, help='Number of clicks. Leave empty (default) to run forever')
-    start_parser.add_argument('--delay', '-d', type=int, default=1, help=' Delay (second) between clicks')
-    start_parser.add_argument('--hold-time', '-ht', type=int, default=0.1, help='Delay (second) between click press and release')
-    start_parser.add_argument('--start-after', '-sa', type=int, default=3, help='Delay (second) before the clicks start')
-    start_parser.add_argument('--quite', '-q', action="store_true", default=False, help='Run without verbosing progress')
-    start_parser.set_defaults(func=entrypoint_handler.click_continuously)
-    
-    start_parser = subparsers.add_parser('elevate', help='Elevate `amiya` permissions.')
-    start_parser.add_argument('--explain', action='store_true', help='Explain why this is needed and what will happen.')
-    start_parser.set_defaults(func=entrypoint_handler.elevate)
-    
-    
-    # =================================================
-    # ================| SCHEDULER | ===================
-    # =================================================
+    uuid_parser = subparsers.add_parser('uuid', help='Display system UUID', description='Display system UUID')
+    uuid_parser.set_defaults(func=entrypoint_handler.display_system_uuid)
+    parser.add_parser_to_group(utility_group, uuid_parser)
+    
+    pixel_parser = subparsers.add_parser('pixel', help='Track cursor position and color', description='Track cursor position and color')
+    pixel_parser.add_argument('--color', '-c', action='store_true', help='Show pixel coordinate as well as the pixel\'s color hex value.')
+    pixel_parser.set_defaults(func=entrypoint_handler.track_cursor)
+    parser.add_parser_to_group(utility_group, pixel_parser)
+    
+    volume_parser = subparsers.add_parser('volume', help='Open simple application volume control UI', description='Open simple application volume control UI')
+    volume_parser.set_defaults(func=entrypoint_handler.open_volume_control_ui)
+    parser.add_parser_to_group(utility_group, volume_parser)
+    
+    click_parser = subparsers.add_parser('click', help='Continuously click mouse.', description='Continuously click mouse.')
+    click_parser.add_argument('--count', '-c', type=int, default=-1, help='Number of clicks. Leave empty (default) to run forever')
+    click_parser.add_argument('--interval', '-d', type=float, default=1, help='Interval delay (seconds) between clicks')
+    click_parser.add_argument('--randomize-by', type=float, default=0.0, help='Randomize the click interval by added 0 to x seconds to the interval specification.')
+    click_parser.add_argument('--hold-time', '-ht', type=float, default=0.1, help='Delay (seconds) between click press and release')
+    click_parser.add_argument('--start-after', '-sa', type=float, default=3, help='Delay (seconds) before the clicks start')
+    click_parser.add_argument('--quiet', '-q', action='store_true', default=False, help='Run without verbosing progress')
+    click_parser.set_defaults(func=entrypoint_handler.click_continuously)
+    parser.add_parser_to_group(utility_group, click_parser)
+    
+    elevate_parser = subparsers.add_parser('elevate', help='Elevate `amiya` permissions.', description='Elevate `amiya` permissions.')
+    elevate_parser.add_argument('--explain', action='store_true', help='Explain why this is needed and what will happen.')
+    elevate_parser.set_defaults(func=entrypoint_handler.elevate)
+    parser.add_parser_to_group(utility_group, elevate_parser)
+    
+    track_url_parser = subparsers.add_parser('track-url', help='Track URL to monitor anchor href changes.', description='Track URL to monitor anchor href changes.')
+    track_url_parser.add_argument('--url', type=str, default="https://mc.kurogames.com/", help='The website URL to track')
+    track_url_parser.add_argument('--interval', "-i", type=int, default=0, help='The interval duration between GET requests (seconds). Defaulted to 0.')
+    track_url_parser.add_argument('--open', "-o", action='store_true', default=False, help='Open the URL when it is detected as new.')
+    track_url_parser.set_defaults(func=entrypoint_handler.track_url)
+    parser.add_parser_to_group(utility_group, track_url_parser)
+
+    
+    # # =================================================
+    # # ================| SCHEDULER | ===================
+    # # =================================================
     
     # start_parser = subparsers.add_parser('run-scheduler', help='Start and run the scheduler')
     # start_parser.set_defaults(func=entrypoint_handler.run_scheduler)
     
     
     
     # ===========================================================================================
@@ -191,41 +251,43 @@
         raise AmiyaOSNotSupported()
     
     
     sync_needed = not entrypoint_handler.apps_synced()
     if sync_needed:
         # If sync is needed, restrict all commands except 'sync'
         def blocked_func(args):
-            text = colored('amiya sync', 'light_cyan')
-            aprint(f"Applications under Amiya's apps manager are not fully configured to run on this machine.\n\nTo sync the apps to this machine, run `{text}`")
+            text = color_cmd('amiya sync')
+            aprint(f"Applications under Amiya's apps manager are not fully configured to run on this machine.\n\nTo sync the apps to this machine, run `{text}`\n")
             raise AmiyaExit()
 
         for name, subparser in subparsers.choices.items():
             if name not in ["sync", "search", "sleep", "shutdown", "uuid", "show-config", "version", "author", "repo"]:
                 subparser.set_defaults(func=blocked_func)
     
     
     isadmin = is_admin()
     if not isadmin:
         # Certain commands require admin permissions to execute
         def blocked_func(args):
-            aprint("Insufficient permission. Please restart the terminal as an administrator.")
+            elevate_cmd = color_cmd("amiya elevate", with_quotes=True)
+            aprint(f"Insufficient permission. Run {elevate_cmd} to elevate permissions first.")
             raise AmiyaExit()
 
         for name, subparser in subparsers.choices.items():
             if name in ["record-auto", "run-auto"]:
                 subparser.set_defaults(func=blocked_func)
     
     
     # ===========================================================================================
     # >>> PARSER DRIVER
     # ===========================================================================================
     
     # Check if no command line arguments are provided
     if len(sys.argv) == 1:
+        aprint("Loading Amiya CLI environment...")
         entrypoint_handler.start_cli(parser)
     else:
         # Normal command line execution
         args = parser.parse_args()
         if hasattr(args, 'func'):
             try:
                 args.func(args)
@@ -234,16 +296,16 @@
             except AmiyaExit:
                 exit()
         else:
             parser.print_help()
             
 
 
-def start_amiya_cli_as_admin():
-    start_amiya()
+# def start_amiya_cli_as_admin():
+#     start_amiya()
     
     # # If process already have admin access
     # if is_admin():
     #     start_amiya()
     #     return
 
     # # Else, request admin permissions
```

### Comparing `amiya-0.0.3/src/amiya/exceptions/__init__.py` & `amiya-0.0.4/src/amiya/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/exceptions/exceptions.py` & `amiya-0.0.4/src/amiya/exceptions/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -69,13 +69,19 @@
         super().__init__(f"\nThe application is not focused during an automation sequence run. Automation stopped.")
 
 class AmiyaOSNotSupported(Exception):
     __module__ = 'builtins'
     def __init__(self):
         super().__init__(f"\n\n\tAs of version {VERSION} (BETA), the {BASENAME} package is only supported on the Windows OS.")
 
+class Amiya_AppStoppedUnexpectedly(Exception):
+    __module__ = 'builtins'
+    def __init__(self):
+        super().__init__(f"\n\n\tApplication stopped running unexpected.")
+
+
 # This is a special exception that is used in place of exit() to avoid IO read error in the CLI environment (to avoid closing STDOUT).
 # This error is caught and replaced with 'continue' in the CLI env and 'exit()' in the normal mode. 
 class AmiyaExit(Exception):
     __module__ = 'builtins'
     def __init__(self, message="Module internal exit requested (should be caught accordingly)."):
-        super().__init__(message)
+        super().__init__(message)
```

### Comparing `amiya-0.0.3/src/amiya/module_utilities/continuous_click_controller.py` & `amiya-0.0.4/src/amiya/module_utilities/continuous_click_controller.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,102 @@
 import time
 import pyautogui
+import random
 from pynput import keyboard
 from threading import Event
 
 from amiya.exceptions.exceptions import AmiyaExit
-from amiya.utils.helper import aprint
+from amiya.utils.helper import aprint, Printer
+
 
 class ContinuousClickController:
     def __init__(self):
         self.thread_event = Event()
         self.pause = False
-    
+        self.click_count = 0
+
+
     def click_continuously(
-        self, count: int = -1, 
-        delay: float = 1.0, 
-        hold_time: float = 0.1, 
-        start_after: float = 5.0,
-        quite: bool = False
+        self,
+        count: int          = -1,
+        interval: float     = 1.0,
+        randomize_by: float = 0.0,
+        hold_time: float    = 0.1,
+        start_after: float  = 5.0,
+        quiet: bool         = False
     ):
-        
-        aprint(f"Uniform clicking starting in {start_after} seconds, press ESC key anytime to stop...\nClick count: {"INF" if count == -1 else count}\nDelay between clicks: {delay} seconds\nTime between press and release: {hold_time} seconds\nQuite: {quite}")
-        
+        self.__verbose_start(count, interval, randomize_by, hold_time, start_after, quiet)
+
         listener = keyboard.Listener(on_press=self.__on_press)
         listener.start()
-        
+
         time.sleep(start_after)
-        
         try:
-            click_count = 0
             while True:
-                if click_count == count:
-                    break
-                
-                if self.thread_event.is_set():
+                if self.click_count == count or self.thread_event.is_set():
+                    listener.stop()
                     break
-                
-                if self.pause:
+                elif self.pause:
                     time.sleep(0.1)
                     continue
-                
-                if not quite:
-                    buffer = " " * 10
-                    x, y = pyautogui.position()
-                    aprint(f"[{click_count+1}/{"INF" if count == -1 else count}] Clicking ({x}, {y})...{buffer}", end="\r")
-                
-                pyautogui.mouseDown()
-                self.__click(hold_time, delay)
-                click_count += 1
-                
-                
-                
+
+                if not quiet:
+                    self.__verbose_click(count)
+
+                self.__click(hold_time, interval, randomize_by)
+
         except KeyboardInterrupt:
             print("")
             listener.stop()
+            time.sleep(1)
             raise AmiyaExit()
-    
-    def __click(self, hold_time, delay):
+
+
+    def __click(self, hold_time, interval, randomize_interval):
+        self.click_count += 1
+        
         pyautogui.mouseDown()
         time.sleep(hold_time)
         pyautogui.mouseUp()
-        time.sleep(delay)
-                
+        
+        time.sleep(interval)
+        time.sleep(random.uniform(0, randomize_interval))
+
+
+    def __verbose_start(self, count, interval, randomize_by, hold_time, start_after, quiet):
+        title_text = Printer.to_lightblue(f"Uniform clicking starting in {start_after} seconds, press CTRL+C or the ESC key anytime to stop...")
+        count_text = "INFINITE" if count == -1 else count
+        count_text = Printer.to_purple("Total clicks:   ") + count_text
+        interval_text = Printer.to_purple("Click interval: ") + f"{interval} seconds"
+        if randomize_by > 0:
+            interval_text += f" + random(0, {randomize_by}) seconds"
+        hold_time_text = Printer.to_purple("Hold duration:  ") + f"{hold_time} seconds"
+        
+        aprint(
+            f"{title_text} \
+            \n{count_text} \
+            \n{hold_time_text} \
+            \n{interval_text}"
+        )
+
+    def __verbose_click(self, max_count):
+        buffer          = " " * 10
+        x, y            = pyautogui.position()
+        max_count_text  = "INF" if max_count == -1 else max_count
+        aprint(f"[Count {self.click_count + 1}/{max_count_text}] Clicking ({x}, {y})...{buffer}", end="\r")
+
+
     def __on_press(self, button):
         if button == keyboard.Key.esc:
-            aprint("\nEsc key pressed, stopping...")
+            if self.click_count > 0:
+                print("")
+            aprint("Esc key pressed, stopping...")
             self.thread_event.set()
-            
+
         if button == keyboard.Key.space:
             self.pause = not self.pause
-            
+
             buffer = " " * 7
-            if self.pause == True:
+            if self.pause:
                 aprint(f"Clicks paused. Press space again to start.{buffer}", end="\r")
             else:
-                aprint(f"Clicks unpaused. Press space again to pause.{buffer}", end="\r")
+                aprint(f"Clicks unpaused. Press space again to pause.{buffer}", end="\r")
```

### Comparing `amiya-0.0.3/src/amiya/module_utilities/cursor_controller.py` & `amiya-0.0.4/src/amiya/module_utilities/cursor_controller.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/module_utilities/dev_features.py` & `amiya-0.0.4/src/amiya/module_utilities/dev_features.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,8 +23,11 @@
 
     def open_dev_env(self):
         aprint(f"Opening development environment ({HOME_DIRECTORY})...")
         os.system(f"code {HOME_DIRECTORY}")
         
     def is_admin(self):
         isadmin = bool_to_str(is_admin(), true_text="Admin", false_text="User")
-        aprint(f"Persmissions: {isadmin}")
+        aprint(f"Persmissions: {isadmin}")
+        
+    def verbose_home_dir(self):
+        aprint(f"Home directory: {HOME_DIRECTORY}")
```

### Comparing `amiya-0.0.3/src/amiya/module_utilities/power_controller.py` & `amiya-0.0.4/src/amiya/module_utilities/power_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,23 +31,28 @@
         
     def run_confirmation(self, delay: int, type: PowerType):
         aprint(f"This machine will {type.name.lower()} after {delay} seconds. Proceed? [y/n] ", end="")
         if input().lower().strip() == "y":
             return True
         return False
         
-    def sleep_pc(self, delay: int):
-        if self.run_confirmation(delay, PowerType.Sleep) == True:
+    def sleep_pc(self, delay: int, no_confirmation: bool = False):
+        if not no_confirmation:
+            confirmed = self.run_confirmation(delay, PowerType.Sleep)
+            if not confirmed:
+                return
+             
             self.wait(delay, PowerType.Sleep)
             
             ret = 0
             try:
                 ret = self.__sleep()
             except Exception as ex:
                 raise AmiyaBaseException(f"Sleep failed to execute due to {ex} with error code {ret}")
+
         
     def shutdown_pc(self, delay: int):
         if self.run_confirmation(delay, PowerType.Shutdown) == True:
             self.wait(delay, PowerType.Shutdown)
             self.__shutdown()
```

### Comparing `amiya-0.0.3/src/amiya/module_utilities/search_controller.py` & `amiya-0.0.4/src/amiya/module_utilities/search_controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from amiya.exceptions.exceptions import *
 from amiya.utils.helper import *
 
 class SearchController:
     def __init__(self):
         self.SERACH_URL = f"https://www.google.com.tr/search?q="
     
-    def search(self, search_content: str|list[str]):
+    def search(self, search_content):
         search_str = None
         if isinstance(search_content, str):
             search_str = search_content
         elif isinstance(search_content, list):
             search_str = " ".join(search_content)
         else:
             raise AmiyaBaseException("Internal Error: Search Input Type Invalid.")
@@ -21,8 +21,7 @@
         if not success:
             aprint("Search failed due to web browser availablility or invalid request.", log_type=LogType.ERROR); raise AmiyaExit()
 
     def search_automated(self):
         search_content = input(atext("What would you like to search? ")).strip()
         if len(search_content) > 0:
             self.search(search_content)
-
```

### Comparing `amiya-0.0.3/src/amiya/module_utilities/volume_controller.py` & `amiya-0.0.4/src/amiya/module_utilities/volume_controller.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/pixel_calculator/pixel_calculator.py` & `amiya-0.0.4/src/amiya/pixel_calculator/pixel_calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             
             curr_window_info = ResolutionDetector.get_window_size()
             curr_x = curr_window_info["left"]
             curr_y = curr_window_info["top"]
             curr_w = curr_window_info["width"]
             curr_h = curr_window_info["height"]
             
-            print(curr_x, curr_y, curr_w, curr_h)
+            # print(curr_x, curr_y, curr_w, curr_h)
             
             prev_x = prev_window_info["left"]
             prev_y = prev_window_info["top"]
             prev_w = prev_window_info["width"]
             prev_h = prev_window_info["height"]
             
             # Normalize the coordinate relative to the original window
```

### Comparing `amiya-0.0.3/src/amiya/pixel_calculator/resolution_detector.py` & `amiya-0.0.4/src/amiya/pixel_calculator/resolution_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # THIS IS FKING MAGIC
     # I spent 4 hours trying to figure out why every package is claiming that an 4K application has 2K resolution 
     # before I came acorss this. Apparently windows isn't DPI aware unless it's specifically set to be. In other 
     # words, this will allow the return of real pixel numbers instead of scaled values.
     windll.user32.SetProcessDPIAware()
     
     @staticmethod
-    def get_primary_monitor_size() -> dict|None:
+    def get_primary_monitor_size() -> dict:
         monitors = get_monitors()
         for m in monitors:
             if m.is_primary:
                 monitor_info = {
                     "width": m.width,
                     "height": m.height
                 }
```

### Comparing `amiya-0.0.3/src/amiya/resources/amiya-cli-2.png` & `amiya-0.0.4/src/amiya/resources/amiya-cli-2.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/resources/amiya-cli-3.png` & `amiya-0.0.4/src/amiya/resources/amiya-cli-3.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/resources/amiya-cli-4.png` & `amiya-0.0.4/src/amiya/resources/amiya-cli-4.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/resources/amiya-cli.png` & `amiya-0.0.4/src/amiya/resources/amiya-cli.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/resources/amiya.png` & `amiya-0.0.4/src/amiya/resources/amiya.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/resources/amiya_with_border.png` & `amiya-0.0.4/src/amiya/resources/amiya_with_border.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/resources/code_snippets/add-app.png` & `amiya-0.0.4/src/amiya/resources/code_snippets/add-app.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/resources/code_snippets/add-tag.png` & `amiya-0.0.4/src/amiya/resources/code_snippets/add-tag.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/resources/code_snippets/start.png` & `amiya-0.0.4/src/amiya/resources/code_snippets/start.png`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/scheduler/scheduler.py` & `amiya-0.0.4/src/amiya/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/scheduler/scheduler_config_handler.py` & `amiya-0.0.4/src/amiya/scheduler/scheduler_config_handler.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya/utils/helper.py` & `amiya-0.0.4/src/amiya/utils/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import os
 import re
 import sys
+import platform
 import shutil
 import threading
 import pyautogui
 import psutil
 import pygetwindow as gw
 import win32gui, win32process, psutil
 from enum import Enum
 from screeninfo import get_monitors
 from datetime import datetime
 from termcolor import colored
 from amiya.utils import constants
-from amiya.utils.constants import BASENAME, DATETIME_FORMAT, TIME_FORMAT # "Amiya"
+from amiya.utils.constants import BASENAME, COMMAND, DATETIME_FORMAT, TIME_FORMAT, DEVELOPMENT # "Amiya"
 
 def verify_platform() -> bool:
     """
     Verifies whether the OS is supported by the package.
     Package amiya currently only support the Windows OS.
     
     :return: true if running on Windows, false otherwise
@@ -35,39 +36,54 @@
     ERROR   = "red"
 
 def atext(text: str, log_type: LogType = LogType.NORMAL) -> str:
     prefix = colored(BASENAME, "cyan")
     rtext = colored(text, log_type.value)
     return f"[{prefix}] {rtext}"
 
-def aprint(text: str, log_type: LogType = LogType.NORMAL, end="\n", new_line_no_prefix=True, file=sys.stdout, flush=True):
+
+def aprint(
+    text: str, 
+    log_type: LogType   = LogType.NORMAL, 
+    end: str            = "\n", 
+    submodule_name: str = "", 
+    new_line_no_prefix  = True, 
+    file                = sys.stdout, 
+    flush               = True
+):
     # The new_line_no_prefix param coupled with \n in the text param will put the
     # text after the new line character on the next line, but without a prefix.
     if "\n" in text and new_line_no_prefix == True:
         text = text.replace("\n", f"\n        ")
     
+    if submodule_name:
+        submodule_name = Printer.to_purple(submodule_name)
+        submodule_name = f"[{submodule_name}] "
+        text = submodule_name + text
+    
     rtext = atext(text, log_type)
-    print(rtext, end=end, file=sys.stdout)
-    sys.stdout.flush()
+    print(rtext, end=end, file=file, flush=flush)
+
 
 def color_cmd(text: str, with_quotes: bool = False):
     text = text.lower()
     
     if constants.CLI_MODE == True:
-        text = text.replace("amiya ", "")
+        text = text.replace(COMMAND, "").strip()
     else:
-        if not text.startswith("amiya"):
-            text = f"amiya {text}"
+        if not text.startswith(COMMAND):
+            text = f"{COMMAND} {text}"
             
     colored_cmd = colored(text, "light_cyan")
     
     if with_quotes:
         return f"'{colored_cmd}'"
     return colored_cmd
 
+
 # =================================================
 # ============| CENTER TEXT HELPER | ==============
 # =================================================
 
 # DON"T CHANGE THE FOLLOWING TWO CENTER TEXT FUNCTIONS. I GOT THESE TO WORK AFTER HOURS. BOTH ARE NEEDED!
 
 def center_text(text):
@@ -109,56 +125,59 @@
         rgb = hex_to_rgb(hex_color)
         escape_seq = f"\x1b[38;2;{rgb[0]};{rgb[1]};{rgb[2]}m" # ANSI escape code for 24-bit (true color): \x1b[38;2;<r>;<g>;<b>m
         return f"{escape_seq}{text}\x1b[0m"
 
     @staticmethod
     def to_purple(text):
         return Printer.hex_text(text, "#a471bf")
+    
+    @staticmethod
+    def to_lightpurple(text):
+        return Printer.hex_text(text, "#c38ef5")
         
     @staticmethod
     def to_skyblue(text):
         return Printer.hex_text(text, "#6dcfd1")
         
     @staticmethod
     def to_lightgrey(text):
         return Printer.hex_text(text, "#8a8a8a")
 
     @staticmethod
     def to_blue(text):
-        return Printer.hex_text(text, "#6aa5fc")
+        return Printer.hex_text(text, "#3c80f0")
 
     @staticmethod
     def to_lightblue(text):
         return Printer.hex_text(text, "#8ab1f2")
     
     @staticmethod
+    def to_darkblue(text):
+        return Printer.hex_text(text, "#2a9bc3")
+    
+    @staticmethod
     def to_lightgreen(text):
         return Printer.hex_text(text, "#74d47b")
     
     @staticmethod
     def to_lightred(text):
         return Printer.hex_text(text, "#f27e82")
 
     
-
 def bool_to_str(boolean: bool, true_text="Valid", false_text="Invalid"):
     CHECKMARK = "\u2713"
     CROSSMARK = "\u2717"
     if boolean:
         return Printer.to_lightgreen(f"{CHECKMARK} {true_text}")
     return Printer.to_lightred(f"{CROSSMARK} {false_text}")
 
 # ========================================================
 # =============| PERMISSION VERIFICATION | ===============
 # ========================================================
 
-import os
-import sys
-import platform
-
 def is_admin() -> bool:
     try:
         # For Windows
         if platform.system().lower() == "windows":
             import ctypes
             return ctypes.windll.shell32.IsUserAnAdmin() != 0
 
@@ -217,14 +236,15 @@
 
 
     simplified_path = Path(drive, first_directory, '...', exe_name)
     simplified_path_str = str(simplified_path)
 
     return simplified_path_str
 
+
 # ===================================================
 # =============| DATETIME HANDLER | =================
 # ===================================================
 
 class DatetimeHandler:
     @staticmethod
     def get_datetime():
@@ -241,21 +261,20 @@
         return datetime.strftime(DATETIME_FORMAT)
     
     @staticmethod
     def str_to_datetime(datetime_str: str):
         return datetime.strptime(datetime_str, DATETIME_FORMAT)
     
     
-    
 # ===================================================
 # ===========| MESSAGE WITH SPINNER | ===============
 # ===================================================
 
 class SpinnerMessage(threading.Thread):
-    def __init__(self, start_message, end_message, spin_delay):
+    def __init__(self, start_message, end_message="", spin_delay=0.1):
         super().__init__()
         self.running = False
         self.start_message = start_message
         self.end_message = end_message
         self.spin_delay = spin_delay
 
     def verbose_start(self):
@@ -264,24 +283,30 @@
 
     def verbose_end(self):
         self.running = False
         self.join()
         time.sleep(0.1)
         aprint(f"\n{self.end_message}")
 
+    def end_run(self):
+        self.running = False
+        self.join()
+
+    # Thread function only. Doen't call directly!!!!!!
     def run(self):
         try:
             while self.running:
                 for char in '|/-\\':
                     aprint(self.start_message + " " + char, end="\r", file=sys.stdout)
                     sys.stdout.flush()
                     time.sleep(self.spin_delay)
         except KeyboardInterrupt:
             pass
         
+        
 # ===================================================
 # ==============| TERMINAL RESIZE | =================
 # ===================================================
         
 import shutil
 
 def get_terminal_size():
@@ -297,38 +322,99 @@
         # Set the desired size
         os.system(f'mode con: cols={min_cols+5} lines={current_rows}')
         
     if current_rows < min_rows:
         # Set the desired size
         os.system(f'mode con: cols={current_cols} lines={min_rows+5}')
 
+
 # ===================================================
 # ==============| TERMINAL RESIZE | =================
 # ===================================================
 
 class WindowUtils:
 
     @staticmethod
     def bring_to_foreground(pid):
-        # Try to find the window associated with the PID
         for proc in psutil.process_iter(['pid', 'name']):
             if proc.info['pid'] == pid:
-                # Get all windows and check if any belong to the target process
                 for window in gw.getAllWindows():
-                    if window._hWnd == win32gui.FindWindow(None, window.title):
-                        _, window_pid = win32process.GetWindowThreadProcessId(window._hWnd)
-                        if window_pid == pid:
-                            if window.isMinimized:
-                                window.restore()
-                            window.activate()
-                            pyautogui.click(window.left + window.width // 2, window.top + window.height // 2)
-                            return True
+                    # To be fairly honest, I have no clue what are the consequences of not matching window handles.
+                    # But I'll leave this here just in case if someone figures out if something is wrong.
+                    # if window._hWnd == win32gui.FindWindow(None, window.title):
+                    
+                    _, window_pid = win32process.GetWindowThreadProcessId(window._hWnd)
+                    if window_pid == pid:
+                        if window.isMinimized:
+                            window.restore()
+                        win32gui.SetForegroundWindow(window._hWnd)
+                        pyautogui.click(window.left + window.width // 2, window.top + window.height // 2)
+                        return True
         return False
 
     @staticmethod
     def active_window_process_name():
         try:
             _, process_ids = win32process.GetWindowThreadProcessId(win32gui.GetForegroundWindow())
             thread_id, pid = process_ids
             return (psutil.Process(pid).name(), thread_id, pid)
         except:
             return None
+
+
+# ===================================================
+# ==============| PROCESS HANDLER | =================
+# ===================================================
+
+class ProcessHandler:
+
+    @staticmethod
+    def get_related_processes(process_pid: int):
+        process = psutil.Process(process_pid)
+        if not process.is_running():
+            return None, None
+        
+        parent_procs: list[psutil.Process] = []
+        children_procs: list[psutil.Process] = []
+               
+        try:
+            parent_procs = process.parents()
+            children_procs = process.children(recursive=True)
+        except:
+            pass
+
+        return parent_procs, children_procs
+    
+    @staticmethod
+    def kill_pid(pid):
+        try:
+            proc = psutil.Process(pid)
+            if proc.is_running():
+                proc.kill()
+                return True
+        
+        except psutil.NoSuchProcess:
+            if DEVELOPMENT:
+                aprint(f"[DEV] Unabled to kill proc {pid} because it's already closed.")
+        except Exception as ex:
+            if DEVELOPMENT:
+                aprint(f"[DEV] Unabled to kill proc {pid} ({ex}).")
+        return False
+
+    
+    @staticmethod
+    def kill_pids(pids: list[int], excluding_pids: list[int] = []):
+        for pid in pids:
+            if pid not in excluding_pids:
+                ProcessHandler.kill_pid(pid)
+
+         
+import hashlib
+class HashCalculator:
+    
+    @staticmethod
+    def calculate_file_hash(file_path: str):
+        sha256_hash = hashlib.sha256()
+        with open(file_path, "rb") as f:
+            for byte_block in iter(lambda: f.read(4096), b""):
+                sha256_hash.update(byte_block)
+        return sha256_hash.hexdigest()
```

### Comparing `amiya-0.0.3/src/amiya/utils/json_handler.py` & `amiya-0.0.4/src/amiya/utils/json_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from amiya.exceptions.exceptions import *
 
 class JSONConfigHandler(ABC):
     def __init__(self, config_abs_path, config_type=dict):
         self.config_file = config_abs_path
         self.config_type = config_type
 
-    def load_config(self) -> dict|list:
+    def load_config(self):
         try:
             with open(self.config_file, "r") as rf:
                 config = json.load(rf)
                 return config
         except FileNotFoundError:
             raise Amiya_ConfigDoesNotExistException(config_file=self.config_file)
```

### Comparing `amiya-0.0.3/src/amiya/utils/pynput_mapping.py` & `amiya-0.0.4/src/amiya/utils/pynput_mapping.py`

 * *Files identical despite different names*

### Comparing `amiya-0.0.3/src/amiya.egg-info/SOURCES.txt` & `amiya-0.0.4/src/amiya.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,14 @@
 src/amiya/amiya.py
 src/amiya.egg-info/PKG-INFO
 src/amiya.egg-info/SOURCES.txt
 src/amiya.egg-info/dependency_links.txt
 src/amiya.egg-info/entry_points.txt
 src/amiya.egg-info/requires.txt
 src/amiya.egg-info/top_level.txt
-src/amiya/apps/afk-journey/app-config.json
-src/amiya/apps/afk-journey/automation/sequence/daily.json
-src/amiya/apps/chrome/app-config.json
-src/amiya/apps/genshin-impact/app-config.json
-src/amiya/apps/honkai-star-rail/app-config.json
-src/amiya/apps/ld-player/app-config.json
-src/amiya/apps/ld-player/automation/sequence/arknights-base.json
-src/amiya/apps/ld-player/automation/sequence/arknights-start.json
-src/amiya/apps/league-of-legends/app-config.json
-src/amiya/apps/persona-5-x/app-config.json
-src/amiya/apps/persona-5-x/automation/sequence/daily.json
-src/amiya/apps/persona-5-x/automation/sequence/test.json
-src/amiya/apps/steam/app-config.json
 src/amiya/apps_manager/__init__.py
 src/amiya/apps_manager/app.py
 src/amiya/apps_manager/apps_manager.py
 src/amiya/apps_manager/apps_viewer.py
 src/amiya/apps_manager/safety_monitor.py
 src/amiya/apps_manager/test.py
 src/amiya/apps_manager/sync_controller/__init__.py
@@ -48,22 +35,24 @@
 src/amiya/bin/get_window_size.exe
 src/amiya/bin/scripts/focus_pid.c
 src/amiya/bin/scripts/get_active_pid.c
 src/amiya/bin/scripts/get_window_size.c
 src/amiya/entrypoints/__init__.py
 src/amiya/entrypoints/entrypoint_handler.py
 src/amiya/entrypoints/entrypoints.py
+src/amiya/entrypoints/help_format_handler.py
 src/amiya/exceptions/__init__.py
 src/amiya/exceptions/exceptions.py
 src/amiya/module_utilities/__init__.py
 src/amiya/module_utilities/continuous_click_controller.py
 src/amiya/module_utilities/cursor_controller.py
 src/amiya/module_utilities/dev_features.py
 src/amiya/module_utilities/power_controller.py
 src/amiya/module_utilities/search_controller.py
+src/amiya/module_utilities/url_tracker.py
 src/amiya/module_utilities/volume_controller.py
 src/amiya/pixel_calculator/__init__.py
 src/amiya/pixel_calculator/pixel_calculator.py
 src/amiya/pixel_calculator/resolution_detector.py
 src/amiya/resources/amiya-cli-2.png
 src/amiya/resources/amiya-cli-3.png
 src/amiya/resources/amiya-cli-4.png
```

