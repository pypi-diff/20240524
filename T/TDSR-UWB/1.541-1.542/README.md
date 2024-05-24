# Comparing `tmp/TDSR-UWB-1.541.tar.gz` & `tmp/TDSR-UWB-1.542.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDSR-UWB-1.541.tar", last modified: Fri May 17 13:38:11 2024, max compression
+gzip compressed data, was "TDSR-UWB-1.542.tar", last modified: Fri May 24 03:38:31 2024, max compression
```

## Comparing `TDSR-UWB-1.541.tar` & `TDSR-UWB-1.542.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-17 13:38:11.527669 TDSR-UWB-1.541/
--rw-rw-r--   0 senter    (1000) senter    (1000)       74 2024-05-09 23:00:07.000000 TDSR-UWB-1.541/LICENSE.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       37 2024-05-09 21:21:05.000000 TDSR-UWB-1.541/MANIFEST.in
--rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-17 13:38:11.527669 TDSR-UWB-1.541/PKG-INFO
--rw-rw-r--   0 senter    (1000) senter    (1000)       93 2024-05-09 23:01:32.000000 TDSR-UWB-1.541/README.md
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-17 13:38:11.523669 TDSR-UWB-1.541/TDSR-UWB/
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-17 13:38:11.523669 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-17 13:38:11.527669 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/
--rw-rw-r--   0 senter    (1000) senter    (1000)     6148 2023-03-30 19:11:25.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store
--rw-rw-r--   0 senter    (1000) senter    (1000)      161 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/.txt
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-17 13:38:11.527669 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/
--rw-rw-r--   0 senter    (1000) senter    (1000)      536 2023-03-02 20:09:11.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json
--rw-rw-r--   0 senter    (1000) senter    (1000)     9479 2023-02-26 18:51:27.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/API.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     5515 2022-12-23 02:15:12.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     5563 2022-12-23 02:08:30.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)       45 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/DATA_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      124 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/DATA_INFO.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      144 2023-08-10 03:26:43.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/DATA_REQUEST.txt
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-17 13:38:11.527669 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/Doc/
--rw-rw-r--   0 senter    (1000) senter    (1000)    12524 2022-10-06 21:41:33.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png
--rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       50 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      411 2023-03-30 02:12:35.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       47 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       64 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      111 2023-05-16 19:39:21.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       93 2023-05-16 19:38:24.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       61 2024-03-13 14:34:07.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       91 2024-03-13 02:20:50.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-03-13 14:31:51.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-13 02:21:52.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-16 16:10:28.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       51 2024-03-16 16:10:10.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       44 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONNECT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      143 2024-03-13 14:30:56.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       40 2024-03-13 01:42:44.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      379 2024-03-14 17:35:25.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       72 2024-03-14 17:30:36.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      120 2023-05-15 23:46:31.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       42 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      550 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       40 2022-12-20 14:51:26.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:18.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       43 2023-09-28 14:06:22.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      173 2024-03-13 14:33:30.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       46 2024-03-13 02:21:17.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       61 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_MESSAGE_ERROR.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       53 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       39 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       60 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       46 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       60 2024-03-13 14:32:21.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       87 2024-03-13 02:21:36.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      138 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONNECT_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       55 2024-03-13 14:35:17.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      116 2024-03-13 02:22:22.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       56 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      184 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-09-28 14:06:26.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:29.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)      348 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_INFO.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_CONFIRM.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       81 2023-05-16 19:37:46.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_REQUEST.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)    12521 2023-03-30 01:57:06.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/networking.md
--rw-rw-r--   0 senter    (1000) senter    (1000)   107545 2023-03-30 01:57:24.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf
--rw-rw-r--   0 senter    (1000) senter    (1000)     9971 2023-03-30 01:57:02.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md
--rw-rw-r--   0 senter    (1000) senter    (1000)     6747 2023-03-04 15:21:05.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md
--rw-rw-r--   0 senter    (1000) senter    (1000)      157 2022-12-08 14:50:04.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/processJSONFiles.sh
--rw-rw-r--   0 senter    (1000) senter    (1000)     1097 2023-03-02 20:30:55.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py
--rw-rw-r--   0 senter    (1000) senter    (1000)   256695 2024-05-17 13:33:41.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     6933 2024-05-17 13:19:59.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_logging.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    14427 2024-05-17 13:19:49.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    19260 2024-05-17 13:19:44.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py
--rw-rw-r--   0 senter    (1000) senter    (1000)    83414 2024-05-17 13:19:37.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_radioControl.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     4130 2024-05-17 13:19:29.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_settings.py
--rw-rw-r--   0 senter    (1000) senter    (1000)        0 2024-05-08 17:38:57.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/__init__.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     2912 2022-12-27 01:25:43.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/crc16.py
--rw-rw-r--   0 senter    (1000) senter    (1000)     2280 2024-05-16 03:20:39.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/logReader.py
--rw-rw-r--   0 senter    (1000) senter    (1000)      376 2024-04-15 16:19:41.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/logReader_Minimal.py
-drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-17 13:38:11.527669 TDSR-UWB-1.541/TDSR-UWB/TDSR_UWB.egg-info/
--rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-17 13:38:11.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO
--rw-rw-r--   0 senter    (1000) senter    (1000)     4735 2024-05-17 13:38:11.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)        1 2024-05-17 13:38:11.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_UWB.egg-info/dependency_links.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-05-17 13:38:11.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_UWB.egg-info/requires.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       13 2024-05-17 13:38:11.000000 TDSR-UWB-1.541/TDSR-UWB/TDSR_UWB.egg-info/top_level.txt
--rw-rw-r--   0 senter    (1000) senter    (1000)       38 2024-05-17 13:38:11.527669 TDSR-UWB-1.541/setup.cfg
--rw-rw-r--   0 senter    (1000) senter    (1000)     7693 2024-05-17 13:20:22.000000 TDSR-UWB-1.541/setup.py
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-24 03:38:31.374373 TDSR-UWB-1.542/
+-rw-rw-r--   0 senter    (1000) senter    (1000)       74 2024-05-09 23:00:07.000000 TDSR-UWB-1.542/LICENSE.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       37 2024-05-09 21:21:05.000000 TDSR-UWB-1.542/MANIFEST.in
+-rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-24 03:38:31.374373 TDSR-UWB-1.542/PKG-INFO
+-rw-rw-r--   0 senter    (1000) senter    (1000)       93 2024-05-09 23:01:32.000000 TDSR-UWB-1.542/README.md
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-24 03:38:31.366372 TDSR-UWB-1.542/TDSR-UWB/
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-24 03:38:31.370373 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-24 03:38:31.374373 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6148 2023-03-30 19:11:25.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store
+-rw-rw-r--   0 senter    (1000) senter    (1000)      161 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/.txt
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-24 03:38:31.374373 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/
+-rw-rw-r--   0 senter    (1000) senter    (1000)      536 2023-03-02 20:09:11.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json
+-rw-rw-r--   0 senter    (1000) senter    (1000)     9479 2023-02-26 18:51:27.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/API.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     5515 2022-12-23 02:15:12.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     5563 2022-12-23 02:08:30.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)       45 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/DATA_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      124 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/DATA_INFO.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      144 2023-08-10 03:26:43.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/DATA_REQUEST.txt
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-24 03:38:31.374373 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/Doc/
+-rw-rw-r--   0 senter    (1000) senter    (1000)    12524 2022-10-06 21:41:33.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png
+-rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       50 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_SLOT_MAP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      411 2023-03-30 02:12:35.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       47 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_GET_STATS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       64 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      405 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/NETWORKING_SET_SLOT_MAP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      111 2023-05-16 19:39:21.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       93 2023-05-16 19:38:24.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/NET_DATA_QUEUE_STATUS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       61 2024-03-13 14:34:07.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       91 2024-03-13 02:20:50.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_APPLY_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-03-13 14:31:51.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-13 02:21:52.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_DELETE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       75 2024-03-16 16:10:28.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       51 2024-03-16 16:10:10.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_ACTIVE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       44 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_CONNECT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       41 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_INFO_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      143 2024-03-13 14:30:56.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       40 2024-03-13 01:42:44.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_IP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_NODE_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      379 2024-03-14 17:35:25.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       72 2024-03-14 17:30:36.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      120 2023-05-15 23:46:31.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       42 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      550 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       40 2022-12-20 14:51:26.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:18.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       43 2023-09-28 14:06:22.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_TUNING_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      173 2024-03-13 14:33:30.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       46 2024-03-13 02:21:17.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_LIST_PRESETS_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       61 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_MESSAGE_ERROR.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       53 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       39 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_REBOOT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       60 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       46 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_RESET_FACTORY_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       60 2024-03-13 14:32:21.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       87 2024-03-13 02:21:36.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SAVE_PRESET_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      228 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      138 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_CONNECT_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       55 2024-03-13 14:35:17.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      116 2024-03-13 02:22:22.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_IP_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       77 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_NODE_CONFIG_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       56 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      184 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       48 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_STATS_CLEAR_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-09-28 14:06:26.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      136 2023-09-28 14:06:29.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_SET_TUNING_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)      348 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_INFO.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       57 2023-03-30 02:12:00.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_CONFIRM.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       81 2023-05-16 19:37:46.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RANGE_SEND_RANGE_REQUEST.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)    12521 2023-03-30 01:57:06.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/networking.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)   107545 2023-03-30 01:57:24.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf
+-rw-rw-r--   0 senter    (1000) senter    (1000)     9971 2023-03-30 01:57:02.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)     6747 2023-03-04 15:21:05.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md
+-rw-rw-r--   0 senter    (1000) senter    (1000)      157 2022-12-08 14:50:04.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/processJSONFiles.sh
+-rw-rw-r--   0 senter    (1000) senter    (1000)     1097 2023-03-02 20:30:55.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)   260166 2024-05-24 03:34:34.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     8222 2024-05-23 22:31:29.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_logging.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    14427 2024-05-19 19:23:20.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    19260 2024-05-24 03:29:16.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    83870 2024-05-24 03:27:24.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_radioControl.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     4130 2024-05-19 19:23:01.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_settings.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)        0 2024-05-08 17:38:57.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/__init__.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)     2912 2022-12-27 01:25:43.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/crc16.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)    10376 2024-05-19 21:14:09.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/logReader.py
+-rw-rw-r--   0 senter    (1000) senter    (1000)      376 2024-04-15 16:19:41.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/logReader_Minimal.py
+drwxrwxr-x   0 senter    (1000) senter    (1000)        0 2024-05-24 03:38:31.374373 TDSR-UWB-1.542/TDSR-UWB/TDSR_UWB.egg-info/
+-rw-rw-r--   0 senter    (1000) senter    (1000)      748 2024-05-24 03:38:31.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO
+-rw-rw-r--   0 senter    (1000) senter    (1000)     4735 2024-05-24 03:38:31.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)        1 2024-05-24 03:38:31.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_UWB.egg-info/dependency_links.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       62 2024-05-24 03:38:31.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_UWB.egg-info/requires.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       13 2024-05-24 03:38:31.000000 TDSR-UWB-1.542/TDSR-UWB/TDSR_UWB.egg-info/top_level.txt
+-rw-rw-r--   0 senter    (1000) senter    (1000)       38 2024-05-24 03:38:31.374373 TDSR-UWB-1.542/setup.cfg
+-rw-rw-r--   0 senter    (1000) senter    (1000)     7693 2024-05-24 03:38:06.000000 TDSR-UWB-1.542/setup.py
```

### Comparing `TDSR-UWB-1.541/PKG-INFO` & `TDSR-UWB-1.542/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDSR-UWB
-Version: 1.541
+Version: 1.542
 Summary: Support libraries for TDSR LLC UWB Radios
 Home-page: UNKNOWN
 Author: TDSR-LLC
 Author-email: contact@tdsr-uwb.com
 License: UNKNOWN
 Project-URL: Company:, https://www.tdsr-uwb.com
 Platform: UNKNOWN
```

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/.DS_Store`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/API.md` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/API.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/API.template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/APIwith_cat_template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/Doc/TDSR_logo_250x134.png`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/RADIO_GET_STATS_CONFIRM.txt`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/networking.md` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/networking.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/networking.pdf`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/networking.template.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/networking_.md`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/JsonDoc/updateReadme.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_PW_GUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from TDSR_Support import TDSR_logging
 from TDSR_Support import TDSR_settings
 from TDSR_Support import TDSR_radioControl
 from TDSR_Support import TDSR_radioConnection
 
 # Primary window GUI class. All sub windows are launched from here as well.
-__version__ = "1.541"
+__version__ = "1.542"
 # Primary application window and GUI
 class MainWindow(QMainWindow):
     def __init__(self, app, *args, **kwargs):
         super(MainWindow, self).__init__(*args, **kwargs)
         title = "PennyWhistle Ranging GUI V" + __version__
         self.setWindowTitle(title)
         self.myScreen = app.primaryScreen()                      # self is mainwindow Widget and myScreen is the display it lives on
@@ -184,14 +184,18 @@
                 self.dispChipTemp.setText("-")
             else:
                 self.windowDataTransfer.radioData.reqMsgTimer.start()
                 self.radioConfigReq, addr = self.radioReq.API.radio_GetConfig_Request(self.appSettings['reqRadio'], self.configID)
                 self.radioStateReq, addr = self.radioReq.API.radio_GetState_Request(self.appSettings['reqRadio'])
                 self.radioReqNodeIDMsg, addr = self.radioReq.API.radio_GetNodeID_Request(self.appSettings['reqRadio'])
                 self.radioReqNodeID = self.radioReqNodeIDMsg['RADIO_GET_NODE_CONFIG_CONFIRM']['nodeId']
+                self.radioReqPresetMsg, addr = self.radioReq.API.radio_Get_Active_Preset_Request(self.appSettings['reqRadio'])
+                status, self.radioReqInfoMsg, addr = self.radioReq.API.radio_GetInfo_Request(self.appSettings['reqRadio'])
+                status, self.radioReqStatsMsg, addr = self.radioReq.API.radio_GetStats_Request(self.appSettings['reqRadio'])
+                status, self.radioReqSlotMsg, addr = self.radioReq.API.network_GetSlotMap_Request(self.appSettings['reqRadio'])
                 self.chipTempTimer.start()
                 self.connectedRequester = 1
             self.updateConnectReq(self.radioReq.status)
 
 # Connects to responding radio. Needed to get stats and set configuration but not needed to range.
     def radioConnectResp(self):
         if self.check_connectResp.isChecked():
@@ -529,31 +533,39 @@
                     if self.dropMenuChart.currentText() == "Filtered":
                         self.plotYT = self.radioRanging.rangeFilteredArrayAll
                     if self.dropMenuChart.currentText() == "Both":
                         self.plotYT = self.radioRanging.rangeArrayAll
                         self.plotYT2 = self.radioRanging.rangeFilteredArrayAll
                     if self.dropMenuChart.currentText() == "RxPower":
                         self.plotYT = self.radioRanging.rxPowerArrayAll
+                    if self.dropMenuChart.currentText() == "FP-Power":
+                        self.plotYT = self.radioRanging.fppArrayAll
                     if self.dropMenuChart.currentText() == "MaxNoise":
                         self.plotYT = self.radioRanging.maxNoiseArrayAll
                     if self.dropMenuChart.currentText() == "StdNoise":
                         self.plotYT = self.radioRanging.stdNoiseArrayAll
-                    if self.dropMenuChart.currentText() == "Multi":
+                    if self.dropMenuChart.currentText() == "Rng/Pwr":
                         self.plotYT = self.radioRanging.rangeArrayAll
                         self.plotYB = self.radioRanging.rxPowerArrayAll
-                    if self.dropMenuChart.currentText() == "MultiFilt":
+                    if self.dropMenuChart.currentText() == "Filt/Pwr":
                         self.plotYT = self.radioRanging.rangeFilteredArrayAll
                         self.plotYB = self.radioRanging.rxPowerArrayAll
+                    if self.dropMenuChart.currentText() == "Rng/FP-Pwr":
+                        self.plotYT = self.radioRanging.rangeArrayAll
+                        self.plotYB = self.radioRanging.fppArrayAll
+                    if self.dropMenuChart.currentText() == "Filt/FP-Pwr":
+                        self.plotYT = self.radioRanging.rangeFilteredArrayAll
+                        self.plotYB = self.radioRanging.fppArrayAll
                     if len(self.plotYT) > int(self.appSettings['chartDepth']):
                         self.plotX = self.plotX[(len(self.plotX) - int(self.appSettings['chartDepth'])):]
                         self.plotYT = self.plotYT[(len(self.plotYT) - int(self.appSettings['chartDepth'])):]
                         if (len(self.plotYT2) > 0):
                             self.plotYT2 = self.plotYT2[(len(self.plotYT2) - int(self.appSettings['chartDepth'])):]
                         self.plotYB = self.plotYB[(len(self.plotYB) - int(self.appSettings['chartDepth'])):]
-                    if "Multi" in self.dropMenuChart.currentText():
+                    if "/" in self.dropMenuChart.currentText():
                         self.chartDataT.setData(self.plotX, self.plotYT)
                         self.chartDataB.setData(self.plotX, self.plotYB)
                     else:
                         self.chartData1.setData(self.plotX, self.plotYT)
                         self.chartData2.setData(self.plotX, self.plotYT2)
                 else:
                     self.plotX = self.radioRanging.chartPointsX
@@ -563,31 +575,39 @@
                     if self.dropMenuChart.currentText() == "Filtered":
                         self.plotYT = self.radioRanging.rangeFilteredArray
                     if self.dropMenuChart.currentText() == "Both":
                         self.plotYT = self.radioRanging.rangeArray
                         self.plotYT2 = self.radioRanging.rangeFilteredArray
                     if self.dropMenuChart.currentText() == "RxPower":
                         self.plotYT = self.radioRanging.rxPowerArray
+                    if self.dropMenuChart.currentText() == "FP-Power":
+                        self.plotYT = self.radioRanging.fppArray
                     if self.dropMenuChart.currentText() == "MaxNoise":
                         self.plotYT = self.radioRanging.maxNoiseArray
                     if self.dropMenuChart.currentText() == "StdNoise":
                         self.plotYT = self.radioRanging.stdNoiseArray
-                    if self.dropMenuChart.currentText() == "Multi":
+                    if self.dropMenuChart.currentText() == "Rng/Pwr":
                         self.plotYT = self.radioRanging.rangeArray
                         self.plotYB = self.radioRanging.rxPowerArray
-                    if self.dropMenuChart.currentText() == "MultiFilt":
+                    if self.dropMenuChart.currentText() == "Filt/Pwr":
                         self.plotYT = self.radioRanging.rangeFilteredArray
                         self.plotYB = self.radioRanging.rxPowerArray
+                    if self.dropMenuChart.currentText() == "Rng/FP-Pwr":
+                        self.plotYT = self.radioRanging.rangeArray
+                        self.plotYB = self.radioRanging.fppArray
+                    if self.dropMenuChart.currentText() == "Filt/FP-Pwr":
+                        self.plotYT = self.radioRanging.rangeFilteredArray
+                        self.plotYB = self.radioRanging.fppArray
                     if len(self.plotYT) > int(self.appSettings['chartDepth']):
                         self.plotX = self.plotX[(len(self.plotX) - int(self.appSettings['chartDepth'])):]
                         self.plotYT = self.plotYT[(len(self.plotYT) - int(self.appSettings['chartDepth'])):]
                         if (len(self.plotYT2) > 0):
                             self.plotYT2 = self.plotYT2[(len(self.plotYT2) - int(self.appSettings['chartDepth'])):]
                         self.plotYB = self.plotYB[(len(self.plotYB) - int(self.appSettings['chartDepth'])):]
-                    if "Multi" in self.dropMenuChart.currentText():
+                    if "/" in self.dropMenuChart.currentText():
                         self.chartDataT.setData(self.plotX, self.plotYT)
                         self.chartDataB.setData(self.plotX, self.plotYB)
                     else:
                         self.chartData1.setData(self.plotX, self.plotYT)
                         self.chartData2.setData(self.plotX, self.plotYT2)
 
             # Case for Network data
@@ -604,39 +624,44 @@
                 tmp1 = tmp1[:shortest]
                 tmp2b = []
                 if len(tmp1) > int(self.appSettings['chartDepth']):
                     tmp1 = tmp1[(len(tmp1) - int(self.appSettings['chartDepth'])):]
                 for k in range(len(self.windowNetwork.slotMap)):
                     for j in range(len(self.windowNetwork.localSlots)):
                         if k == self.windowNetwork.localSlots[j][0]:
-                            if "Multi" not in self.dropMenuChart.currentText():
+                            if "/" not in self.dropMenuChart.currentText():
                                 if self.dropMenuChart.currentText() == "Ranges":
                                     tmp2 = self.windowNetwork.netRangeArray[k][:shortest]
                                 if self.dropMenuChart.currentText() == "Filtered":
                                     tmp2 = self.windowNetwork.netRangeFilteredArray[k][:shortest]
                                 if self.dropMenuChart.currentText() == "Both":
                                     tmp2 = self.windowNetwork.netRangeArray[k][:shortest]
                                     tmp2b = self.windowNetwork.netRangeFilteredArray[k][:shortest]
                                 if self.dropMenuChart.currentText() == "RxPower":
                                     tmp2 = self.windowNetwork.netPowerArray[k][:shortest]
+                                if self.dropMenuChart.currentText() == "FP-Power":
+                                    tmp2 = self.windowNetwork.netFppArray[k][:shortest]
                                 if self.dropMenuChart.currentText() == "MaxNoise":
                                     tmp2 = self.windowNetwork.netMaxNoiseArray[k][:shortest]
                                 if self.dropMenuChart.currentText() == "StdNoise":
                                     tmp2 = self.windowNetwork.netStdNoiseArray[k][:shortest]
                                 if len(tmp2) > int(self.appSettings['chartDepth']):
                                     tmp2 = tmp2[(len(tmp2) - int(self.appSettings['chartDepth'])):]
                                 self.windowNetwork.netPlot1[k].setData(tmp1,tmp2)
                                 self.windowNetwork.netPlot2[k].setData(tmp1,tmp2b)
                             else:
                                 tmp2 = []
-                                if self.dropMenuChart.currentText() == "Multi":
+                                if self.dropMenuChart.currentText() == "Rng/":
                                     tmp2 = self.windowNetwork.netRangeArray[k][:shortest]
-                                if self.dropMenuChart.currentText() == "MultiFilt":
+                                if self.dropMenuChart.currentText() == "Filt/":
                                     tmp2 = self.windowNetwork.netRangeFilteredArray[k][:shortest]
-                                tmp3 = self.windowNetwork.netPowerArray[k][:shortest]
+                                if self.dropMenuChart.currentText() == "/FP-Pwr":
+                                    tmp3 = self.windowNetwork.netFppArray[k][:shortest]
+                                else:
+                                    tmp3 = self.windowNetwork.netPowerArray[k][:shortest]
                                 if len(tmp2) > int(self.appSettings['chartDepth']):
                                     tmp2 = tmp2[(len(tmp2) - int(self.appSettings['chartDepth'])):]
                                 if len(tmp3) > int(self.appSettings['chartDepth']):
                                     tmp3 = tmp3[(len(tmp3) - int(self.appSettings['chartDepth'])):]
                                 self.windowNetwork.netPlotT[k].setData(tmp1,tmp2)
                                 self.windowNetwork.netPlotB[k].setData(tmp1,tmp3)
 
@@ -648,30 +673,32 @@
                 self.rangeMin = 1000000
                 self.powerMax = -200
                 self.powerMin = 0
                 self.stdNoiseMax = -10
                 self.stdNoiseMin = 20000
                 self.maxNoiseMax = -10
                 self.maxNoiseMin = 20000
-            if self.dropMenuChart.currentText() == "Ranges" or self.dropMenuChart.currentText() == "Filtered" or "Multi" in self.dropMenuChart.currentText():
+            if self.dropMenuChart.currentText() == "Ranges" or self.dropMenuChart.currentText() == "Filtered" or "/" in self.dropMenuChart.currentText():
                 self.chartScale([self.rangeMax, self.rangeMin],[self.powerMax, self.powerMin])
             if self.dropMenuChart.currentText() == "RxPower":
                 self.chartScale([self.powerMax, self.powerMin],[self.powerMax, self.powerMin])
+            if self.dropMenuChart.currentText() == "FP-Power":
+                self.chartScale([self.powerMax, self.powerMin],[self.powerMax, self.powerMin])
             if self.dropMenuChart.currentText() == "MaxNoise":
                 self.chartScale([self.maxNoiseMax, self.maxNoiseMin],[self.powerMax, self.powerMin])
             if self.dropMenuChart.currentText() == "StdNoise":
                 self.chartScale([self.stdNoiseMax, self.stdNoiseMin],[self.powerMax, self.powerMin])
         else:
             tmp = float(packet['RANGE_INFO']['precisionRangeM'])
             if tmp > self.rangeMax or tmp < self.rangeMin:
                 if tmp > self.rangeMax:
                     self.rangeMax = tmp
                 if tmp < self.rangeMin:
                     self.rangeMin = tmp
-                if self.dropMenuChart.currentText() == "Ranges" or self.dropMenuChart.currentText() == "Filtered" or "Multi" in self.dropMenuChart.currentText():
+                if self.dropMenuChart.currentText() == "Ranges" or self.dropMenuChart.currentText() == "Filtered" or "/" in self.dropMenuChart.currentText():
                     self.chartScale([self.rangeMax, self.rangeMin],[self.powerMax, self.powerMin])
             rxPower = str(packet['RANGE_INFO']['rxPower'])
             if rxPower != "-Infinity" and rxPower != "-inf":
                 rxPower = round(float(packet['RANGE_INFO']['rxPower']))
             else:
                 rxPower = -120
             if rxPower > self.powerMax or rxPower < self.powerMin:
@@ -745,15 +772,15 @@
             else:
                 self.yScalePosB = yDataB[0] * 0.8
             tmp = yDataB[1]
             if tmp > 0:
                 self.yScaleNegB = yDataB[1] * 0.8
             else:
                 self.yScaleNegB = yDataB[1] * 1.2
-        if "Multi" in self.dropMenuChart.currentText():
+        if "/" in self.dropMenuChart.currentText():
             if self.yScalePosB > -75:
                 self.yScalePosB = -75
             if self.yScaleNegB < -130:
                 self.yScaleNegB = -130
         self.dataWindowB.setYRange(self.yScaleNegB, self.yScalePosB,padding = 0)
 
 # Sets up main window GUI.
@@ -1050,15 +1077,15 @@
         self.dispChipTemp.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias + 45)
         self.dispChipTemp.resize(xWidth,yWidth)
         self.dispChipTemp.setToolTip("Internal Temperature of RF IC")
         self.dispChipTemp.setStyleSheet("QLineEdit {background-color: lightyellow;}")
         self.dispChipTemp.setAlignment(Qt.AlignmentFlag.AlignCenter)
         x = 1
         y = 0
-        dropMenuOptions = ["Ranges", "Filtered", "Both", "RxPower", "MaxNoise", "StdNoise", "Multi", "MultiFilt"]
+        dropMenuOptions = ["Ranges", "Filtered", "Both", "RxPower", "FP-Power", "MaxNoise", "StdNoise", "Rng/Pwr", "Filt/Pwr", "Rng/FP-Pwr", "Filt/FP-Pwr"]
         self.labelDropMenuChart = QLabel(self)
         self.labelDropMenuChart.resize(xWidth,yWidth)
         self.labelDropMenuChart.move(x*xBump + xStart + xBias, yStart + y*yBump + yBias)
         self.labelDropMenuChart.setAlignment(Qt.AlignmentFlag.AlignCenter)
         self.labelDropMenuChart.setFont(self.guiFont.guiFont20)
         self.labelDropMenuChart.setText("Chart Options")
         # xWidth = 160
@@ -1348,14 +1375,16 @@
         self.guiUpdateTimer.stop()
         self.guiUpdateTimer.start()
 # tests to see if new requester IP number is valid and updates variables and GUI
     def updateReqRadio(self):
         if self.radioScanComplete == True:
             radioSelection = self.dropMenuReqRadio.currentText()
             testPass = 1
+            if self.radioMode == "ranging":
+                self.radioRanging.toggleRun()
             if radioSelection == self.dropMenuRespRadio.currentText():
                 self.dropMenuRespRadio.setCurrentIndex(0)
             if self.connectedRequester == 1:
                 self.radioReq.disconnect()
                 self.windowDataTransfer.radioData.reqMsgTimer.stop()
             self.connectedRequester = 0
             self.radioReq = None
@@ -1363,14 +1392,16 @@
             if testPass == 1:
                 self.radioConnectReq()
 # tests to see if new responder IP number is valid and updates variables and GUI
     def updateRespRadio(self):
         if self.radioScanComplete:
             radioSelection = self.dropMenuRespRadio.currentText()
             testPass = 1
+            if self.radioMode == "ranging":
+                self.radioRanging.toggleRun()
             if radioSelection == self.dropMenuReqRadio.currentText():
                 self.dropMenuReqRadio.setCurrentIndex(0)
             if self.connectedResponder == 1:
                 self.radioResp.disconnect()
             self.connectedResponder = 0
             self.radioResp = None
             self.appSettings['respRadio'] = radioSelection
@@ -1408,36 +1439,41 @@
             # self.chartScale([self.rangeMax, self.rangeMin],[self.powerMax, self.powerMin])
         if self.dropMenuChart.currentText() == "RxPower":
             self.dataWindow.setHidden(False)
             self.dataWindowT.setHidden(True)
             self.dataWindowB.setHidden(True)
             self.checkChartRange(None)
             # self.chartScale([self.powerMax, self.powerMin],[self.powerMax, self.powerMin])
+        if self.dropMenuChart.currentText() == "FP-Power":
+            self.dataWindow.setHidden(False)
+            self.dataWindowT.setHidden(True)
+            self.dataWindowB.setHidden(True)
+            self.checkChartRange(None)
         if self.dropMenuChart.currentText() == "MaxNoise":
             self.dataWindow.setHidden(False)
             self.dataWindowT.setHidden(True)
             self.dataWindowB.setHidden(True)
             self.checkChartRange(None)
             # self.chartScale([self.maxNoiseMax, self.maxNoiseMin],[self.powerMax, self.powerMin])
         if self.dropMenuChart.currentText() == "StdNoise":
             self.dataWindow.setHidden(False)
             self.dataWindowT.setHidden(True)
             self.dataWindowB.setHidden(True)
             self.checkChartRange(None)
             # self.chartScale([self.stdNoiseMax, self.stdNoiseMin],[self.powerMax, self.powerMin])
-        if "Multi" in self.dropMenuChart.currentText():
+        if "/" in self.dropMenuChart.currentText():
             self.dataWindow.setHidden(True)
             self.dataWindowT.setHidden(False)
             self.dataWindowB.setHidden(False)
             self.checkChartRange(None)
             # self.chartScale([self.rangeMax, self.rangeMin],[self.powerMax, self.powerMin])
         self.dataWindow.enableAutoRange(axis = 'x', enable = True)
         self.dataWindowT.enableAutoRange(axis = 'x', enable = True)
         self.dataWindowB.enableAutoRange(axis = 'x', enable = True)
-        filterList = {"Filtered", "Both", "MultiFilt"}
+        filterList = {"Filtered", "Both", "Filt/Pwr", "Filt/FP-Pwr"}
         if self.dropMenuChart.currentText() in filterList:
             self.rangeDispType = "filtered"
         else:
             self.rangeDispType = "precision"
         self.plotData()
 
 # tests to see if new chart depth number is valid and updates variables and GUI. Otherwise uses default.
@@ -2661,14 +2697,15 @@
             self.dropMenuPresets.addItems(["Current Active Settings"])
             self.dropMenuPresets.addItems(presets)
 
     def radioUpdateActivePreset(self):
         if self.req:
             ip = self.gui.appSettings['reqRadio']
             nameMsgActive, addr = self.gui.radioReq.API.radio_Get_Active_Preset_Request(ip)
+            self.radioReqPresetMsg = nameMsgActive
         else:
             ip = self.gui.appSettings['respRadio']
             nameMsgActive, addr = self.gui.radioReq.API.radio_Get_Active_Preset_Request(ip)
         # print(nameMsgActive)
         nameMsgActive = nameMsgActive['RADIO_GET_ACTIVE_PRESET_CONFIRM']
         nameActive = nameMsgActive['activePreset']
         self.dropMenuPresets.setCurrentText(nameActive)
@@ -3944,14 +3981,15 @@
         self.netPlot1 = []
         self.netPlot2 = []
         self.netPlotT = []
         self.netPlotB = []
         self.netRangeArray = []
         self.netRangeFilteredArray = []
         self.netPowerArray = []
+        self.netFppArray = []
         self.netMaxNoiseArray = []
         self.netStdNoiseArray = []
         self.netXArray = []
         self.netRangeCount = 0
         self.netYScale = 0
         self.netGuiTimer = QTimer()
         self.netGuiTimer.setInterval(1000)
@@ -4007,62 +4045,72 @@
             #   so that it doesn't start on any slot. Waits for the beginning to avoid starting mid-slotmap.
             if len(self.netXArray) > 0:  # only start appending once Xarray sees first slot and starts advancing
                 # if range was successful
                 if packet['RANGE_INFO']['rangeStatus'] == 0 and packet['RANGE_INFO']['precisionRangeM'] != 0.0:
                     self.gui.checkChartRange(packet)
                     # Condition RX power so that it doesn't add/plot bogus results
                     rxPower = str(packet['RANGE_INFO']['rxPower'])
+                    fpp = str(packet['RANGE_INFO']['fpp'])
                     if rxPower != "-Infinity" and rxPower != "-inf":
                         rxPower = round(float(packet['RANGE_INFO']['rxPower']))
                     else:
                         rxPower = -120
+                    if fpp != "-Infinity" and rxPower != "-inf":
+                        fpp = round(float(packet['RANGE_INFO']['fpp']))
+                    else:
+                        fpp = -120
                     # Store the current range info in the array for the current slot, which should only be local slots
                     try:
                         self.netRangeArray[slot].append(float(packet['RANGE_INFO']['precisionRangeM']))
                     except:
                         print("a: Slot, ArraySize:", slot, len(self.netRangeArray))
                     try:
                         # THIS NEEDS TO CHANGE TO FILTERED WHEN API SUPPORTS IT
                         self.netRangeFilteredArray[slot].append(float(packet['RANGE_INFO']['filteredRangeM']))
                     except Exception as e:
                         print(e)
                         print(packet)
                         print("b: Slot, ArraySize:", slot, len(self.netRangeFilteredArray))
                     self.netPowerArray[slot].append(rxPower)
+                    self.netFppArray[slot].append(fpp)
                     self.netMaxNoiseArray[slot].append(int(packet['RANGE_INFO']['maxNoise']))
                     self.netStdNoiseArray[slot].append(int(packet['RANGE_INFO']['stdNoise']))
                 # if not a successful range
                 else:
                     # print("Process Range Error 2")
                     if self.gui.check_plotDrops.isChecked():
                         self.netRangeArray[slot].append(float(packet['RANGE_INFO']['precisionRangeM']))
                         self.netRangeFilteredArray[slot].append(float(packet['RANGE_INFO']['filteredRangeM']))
                         self.netPowerArray[slot].append(rxPower)
+                        self.netFppArray[slot].append(fpp)
                         self.netMaxNoiseArray[slot].append(int(packet['RANGE_INFO']['maxNoise']))
                         self.netStdNoiseArray[slot].append(int(packet['RANGE_INFO']['stdNoise']))
                     else:
                         if len(self.netRangeArray[slot]) > 0: #make sure we have a point to copy
                             self.netRangeArray[slot].append(self.netRangeArray[slot][len(self.netRangeArray[slot])-1])  # copy last data point
                             self.netRangeFilteredArray[slot].append(self.netRangeFilteredArray[slot][len(self.netRangeFilteredArray[slot])-1])
                             self.netPowerArray[slot].append(self.netPowerArray[slot][len(self.netPowerArray[slot])-1])
+                            self.netFppArray[slot].append(self.netFppArray[slot][len(self.netFppArray[slot])-1])
                             self.netMaxNoiseArray[slot].append(self.netMaxNoiseArray[slot][len(self.netMaxNoiseArray[slot])-1])
                             self.netStdNoiseArray[slot].append(self.netStdNoiseArray[slot][len(self.netStdNoiseArray[slot])-1])
                         else:  #if not, make up a point
                             self.netRangeArray[slot].append(0)
                             self.netRangeFilteredArray[slot].append(0)
                             self.netPowerArray[slot].append(-120)
+                            self.netFppArray[slot].append(-120)
                             self.netMaxNoiseArray[slot].append(1100)
                             self.netStdNoiseArray[slot].append(60)
         # update plot when last slot is done
         if slot == self.localSlotLast and len(self.netRangeArray[self.localSlots[0][0]]) > 0:
             if len(self.netRangeArray[0]) > int(self.gui.appSettings['memoryDepth']):
                 for i in range(len(self.netRangeArray)):
                     self.netRangeArray[i] = self.netRangeArray[i][1:]
                     self.netRangeFilteredArray[i] = self.netRangeFilteredArray[i][1:]
                     self.netPowerArray[i] = self.netPowerArray[i][1:]
+                    self.netFppArray[i] = self.netFppArray[i][1:]
                     self.netMaxNoiseArray[i] = self.netMaxNoiseArray[i][1:]
                     self.netStdNoiseArray[i] = self.netStdNoiseArray[i][1:]
                 self.netXArray = self.netXArray[1:]
             self.gui.plotData()
 
     def initGUI(self):
         self.layoutTop = QVBoxLayout()
@@ -4425,14 +4473,15 @@
                 self.populateMap()
             self.but_slotMapSetMap.setStyleSheet(self.gui.buttonSheetBlue)
 
 
     def buttonHandlerGetMap(self):
         if self.gui.connectedRequester == 1:
             status, self.slotMap, addr = self.gui.radioReq.API.network_GetSlotMap_Request(self.gui.appSettings['reqRadio'])
+            self.gui.radioReqSlotMsg = self.slotMap
             self.slotMap = self.slotMap['NETWORKING_GET_SLOT_MAP_CONFIRM']['slotMap']
         else:
             self.slotMap = []
             text = "Need to connect to a primary radio@!\n"
             self.gui.updateConsole(text)
         # print("getMapStatus", status)
         # print(self.slotMap)
@@ -4471,14 +4520,15 @@
         self.gui.chartDataT.setData(self.gui.plotX, self.gui.plotYT)
         self.gui.chartDataB.setData(self.gui.plotX, self.gui.plotYB)
         self.netXArray = []
         for i in range(len(self.netRangeArray)):
             self.netRangeArray[i] = []
             self.netRangeFilteredArray[i] = []
             self.netPowerArray[i] = []
+            self.netFppArray[i] = []
             self.netMaxNoiseArray[i] = []
             self.netStdNoiseArray[i] = []
             self.netPlot1[i].setData(self.netXArray, self.netRangeArray[i])
             self.netPlot2[i].setData(self.netXArray, self.netRangeFilteredArray[i])
             self.netPlotT[i].setData(self.netXArray, self.netRangeArray[i])
             self.netPlotB[i].setData(self.netXArray, self.netRangeArray[i])
         self.localSlotFirst = -1
@@ -4492,24 +4542,26 @@
                 plotX = []
                 # T = top chart, B = Bottom chart
                 plotYT = []
                 plotYB = []
                 rangeArray = []
                 rangeFilteredArray = []
                 powerArray = []
+                fppArray = []
                 maxNoiseArray = []
                 stdNoiseArray = []
                 self.netPlot1.append(self.gui.dataWindow.plot(plotX, plotYT, pen=self.gui.pen[i]))
                 self.netPlot2.append(self.gui.dataWindow.plot(plotX, plotYT, pen=self.gui.pen[18]))
                 self.netPlotT.append(self.gui.dataWindowT.plot(plotX, plotYT, pen=self.gui.pen[i]))
                 self.netPlotB.append(self.gui.dataWindowB.plot(plotX, plotYB, pen=self.gui.pen[i]))
                 # print(i, self.gui.pen[i].color().getRgb())
                 self.netRangeArray.append(rangeArray)
                 self.netRangeFilteredArray.append(rangeFilteredArray)
                 self.netPowerArray.append(powerArray)
+                self.netFppArray.append(fppArray)
                 self.netMaxNoiseArray.append(maxNoiseArray)
                 self.netStdNoiseArray.append(stdNoiseArray)
         if len(self.localSlots) > 0:
             self.localSlotFirst = self.localSlots[0][0]
             self.localSlotLast = self.localSlots[len(self.localSlots)-1][0]
 
     def buttonHandlerShowStats(self):
```

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_logging.py` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_logging.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,70 @@
 from datetime import datetime, date
 from time import time
 from pathlib import Path
 from os import path, mkdir, makedirs
 from json import dumps
 
-__version__ = "1.541"
+__version__ = "1.542"
 
 # All application data logging functions
 class logData():
     def __init__(self, gui):
         self.gui = gui
         self.settings = gui.appSettings
         self.logFile = ""
         self.msgList = []
 
 # Creates a new filename and directory under the chosen log directory.
 #  Naming is cased on radio nodes and times logs were taken. Autogenerated filenames.
     def createTimeBasedLog(self, nodeIPs):
         if self.gui.connectedRequester == 1:
+            timeNow = datetime.now()
+            logTime = timeNow.strftime("LogDate: %m/%d/%y %H:%M:%S")
+            fileTime = {}
+            fileTime['Time'] = logTime
             self.msgList = []
             print("Time Based Log")
             today = date.today()
             nodeStr = nodeIPs[0]
             self.startDataTime = time()
             dateDirectory = "RN_NODES" + nodeStr + "_" + today.strftime("%m-%d-%y")
             dataDirectoryName = path.join(self.settings['logDirectory'],dateDirectory)
             if not path.isdir(dataDirectoryName):
                 makedirs(dataDirectoryName)
-            timeNow = datetime.now()
             self.fileDateTime = timeNow.strftime("RNS_Log_%m_%d_%y_%H_%M_%S.json")
             logFileName = path.join(dataDirectoryName,self.fileDateTime)
             self.logFile = open(logFileName,"w")
             # if self.settings['logJson'] == 1:
+            self.logFile.write(dumps(fileTime))
+            self.logFile.write("\n")
             self.logFile.write(dumps(self.gui.radioStateReq))
             self.logFile.write("\n")
             self.logFile.write(dumps(self.gui.radioConfigReq))
             self.logFile.write("\n")
             self.logFile.write(dumps(self.gui.radioReqNodeIDMsg))
+            self.logFile.write("\n")
+            self.logFile.write(dumps(self.gui.radioReqPresetMsg))
+            self.logFile.write("\n")
+            self.logFile.write(dumps(self.gui.radioReqInfoMsg))
+            self.logFile.write("\n")
+            self.logFile.write(dumps(self.gui.radioReqStatsMsg))
+            self.logFile.write("\n")
+            self.logFile.write(dumps(self.gui.radioReqSlotMsg))
             self.logFile.write("\n\n")
             print(logFileName)
 # Creates a new filename and directory under the chosen log directory. Subdirectory is created for Month/Year
 #  log was taken. Name is based on user entered base name with 4 digit increasing file counter at the end.
     def createNameBasedLog(self):
         if self.gui.connectedRequester == 1:
             self.msgList = []
+            timeNow = datetime.now()
+            logTime = timeNow.strftime("LogDate: %m/%d/%y %H:%M:%S")
+            fileTime = {}
+            fileTime['Time'] = logTime
             logFileName = self.settings['logFile']
             logFilePath = self.settings['logDirectory']
             print("Name Based Log")
             self.startDataTime = time()
             self.logFile = logFilePath + logFileName
             tmp = Path(logFilePath)
             if tmp.is_dir() == False:
@@ -70,19 +87,29 @@
                     stmp = "_" + stmp[len(stmp)-4:]
                     logFileTmp = logFileFullPath + tmp[0] + stmp
                     logFileName = Path(logFileTmp + "." + tmp[1])
                     tmpNum = tmpNum + 1
             self.logFile = logFileName
             self.logFile = open(self.logFile,"w")
             # if self.settings['logJson'] == 1:
+            self.logFile.write(dumps(fileTime))
+            self.logFile.write("\n")
             self.logFile.write(dumps(self.gui.radioStateReq))
             self.logFile.write("\n")
             self.logFile.write(dumps(self.gui.radioConfigReq))
             self.logFile.write("\n")
             self.logFile.write(dumps(self.gui.radioReqNodeIDMsg))
+            self.logFile.write("\n")
+            self.logFile.write(dumps(self.gui.radioReqPresetMsg))
+            self.logFile.write("\n")
+            self.logFile.write(dumps(self.gui.radioReqInfoMsg))
+            self.logFile.write("\n")
+            self.logFile.write(dumps(self.gui.radioReqStatsMsg))
+            self.logFile.write("\n")
+            self.logFile.write(dumps(self.gui.radioReqSlotMsg))
             self.logFile.write("\n\n")
             print(logFileName)
 # Log data to chosen log file. Can save all messages, only range_info messages, or simply ranges and message IDs
     def logToFile(self, packet, nodeIPs):
         # Start new log if logfile is closed
         if self.logFile == "":
             if self.settings['logRangeInfoOnly'] == 1 and "RANGE_INFO" in packet:
```

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_radioAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from json import dumps
 from time import sleep
 
-__version__ = "1.541"
+__version__ = "1.542"
 
 class RadioAPI:
     _msgId = 0
 
     def __init__(self, messageQueues, messageList, TxQueue):
         self.TxQueue = TxQueue
         self.messageList = messageList
```

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_radioConnection.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import serial
 import serial.tools.list_ports
 import ipaddress
 import netifaces
 
 from TDSR_Support import TDSR_radioAPI
 
-__version__ = "1.541"
+__version__ = "1.542"
 
 # Use netifaces to find local IP addresses.
 netifaces_available = False
 try:
     import netifaces
     netifaces_available = True
 
@@ -130,15 +130,15 @@
         # print(ports)
         for radio in ports:
             radios.append(radio)
             # print(radio)
         return radios
 
     def getMulticast(self):
-        timeout = 0.1
+        timeout = 0.4
         local_ipv4_interfaces = []
         ifaces = netifaces.interfaces()
         for iface in ifaces:
             addrs = netifaces.ifaddresses(iface)
             if netifaces.AF_INET in addrs.keys():
                 for local_addr_info in addrs[netifaces.AF_INET]:
                     # Confirm it has an "addr" key for the IP address (should always)
```

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_radioControl.py` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_radioControl.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from time import time, sleep
 from math import sqrt, log10
 from numpy import power
 from pathlib import Path
 from base64 import b64encode, b64decode
 from threading import Thread
 
-__version__ = "1.541"
+__version__ = "1.542"
 
 # Primary ranging functions
 class rangeCmds():
     def __init__(self, gui):
         self.gui = gui
         self.appSetup()
 
@@ -82,19 +82,21 @@
             self.errors = 0
             self.packets = 0
             self.successRateRate = 0
             self.rangeArray = []
             self.rangeFilteredArray = []
             self.rxPowerWattsArray = []
             self.rxPowerArray = []
+            self.fppArray = []
             self.rangeFPPWattsArray = []
             self.maxNoiseArray = []
             self.stdNoiseArray = []
             self.chartPointsX = []
             self.rxPowerArrayAll = []
+            self.fppArrayAll = []
             self.maxNoiseArrayAll = []
             self.stdNoiseArrayAll = []
             self.rangeArrayAll = []
             self.rangeFilteredArrayAll = []
             self.chartPointsXAll = []
             self.rangeValidSum = 0
             self.rangeFilteredValidSum = 0
@@ -141,18 +143,20 @@
             for i in self.gui.radioReq.messageQueues:
                 while not self.gui.radioReq.messageQueues[i].empty():
                     dump = self.gui.radioReq.messageQueues[i].get()
                     # print("dumping:",i)
             # print("Tx Len:", self.gui.radioReq.TxQueue.qsize())
             status = self.rangingSetup('ranging')
             if status == True:
+                status, self.gui.radioReqStatsMsg, addr = self.gui.radioReq.API.radio_GetStats_Request(self.gui.appSettings['reqRadio'])
                 self.gui.windowNetwork.netXArray = []
                 for i in range(len(self.gui.windowNetwork.netRangeArray)):
                     self.gui.windowNetwork.netRangeArray[i] = []
                     self.gui.windowNetwork.netPowerArray[i] = []
+                    self.gui.windowNetwork.netFppArray[i] = []
                     self.gui.windowNetwork.netMaxNoiseArray[i] = []
                     self.gui.windowNetwork.netStdNoiseArray[i] = []
                     self.gui.windowNetwork.netPlot1[i].setData(self.gui.windowNetwork.netXArray, self.gui.windowNetwork.netRangeArray[i])
                     self.gui.windowNetwork.netPlot2[i].setData(self.gui.windowNetwork.netXArray, self.gui.windowNetwork.netRangeArray[i])
                     self.gui.windowNetwork.netPlotT[i].setData(self.gui.windowNetwork.netXArray, self.gui.windowNetwork.netRangeArray[i])
                     self.gui.windowNetwork.netPlotB[i].setData(self.gui.windowNetwork.netXArray, self.gui.windowNetwork.netRangeArray[i])
                 self.gui.plotYT = []
@@ -365,46 +369,50 @@
             if self.gui.radioMode == 'ranging' and tmpRxPower != -120 and tmpFPPower != -120:
                 self.rangeCountValid = self.rangeCountValid + 1
                 self.rangeValidSum = self.rangeValidSum + float(packet['RANGE_INFO']['precisionRangeM'])
                 self.rangeFilteredValidSum = self.rangeFilteredValidSum + float(packet['RANGE_INFO']['filteredRangeM'])
                 self.rangeRXPowerSum = self.rangeRXPowerSum + tmpRxPowerWatts
                 self.rangeFPPowerSum = self.rangeFPPowerSum + tmpFPPowerWatts
                 self.rxPowerArray.append(tmpRxPower)
+                self.fppArray.append(tmpFPPower)
                 self.rxPowerWattsArray.append(tmpRxPowerWatts)
                 self.rangeFPPWattsArray.append(tmpFPPowerWatts)
                 self.maxNoiseArray.append(int(packet['RANGE_INFO']['maxNoise']))
                 self.stdNoiseArray.append(int(packet['RANGE_INFO']['stdNoise']))
                 self.rangeArray.append(float(packet['RANGE_INFO']['precisionRangeM']))
                 self.rangeFilteredArray.append(float(packet['RANGE_INFO']['filteredRangeM']))
                 self.chartPointsX.append(int(self.rangeCount))
             self.gui.checkChartRange(packet)
             # self.gui.plotData()
 
         self.rxPowerArrayAll.append(tmpRxPower)
+        self.fppArrayAll.append(tmpFPPower)
         self.maxNoiseArrayAll.append(int(packet['RANGE_INFO']['maxNoise']))
         self.stdNoiseArrayAll.append(int(packet['RANGE_INFO']['stdNoise']))
         self.rangeArrayAll.append(float(packet['RANGE_INFO']['precisionRangeM']))
         try:
             self.rangeFilteredArrayAll.append(float(packet['RANGE_INFO']['filteredRangeM']))
         except:
             print(packet)
         self.chartPointsXAll.append(int(self.rangeCount))
         # self.gui.checkChartRange(packet)
             # self.gui.plotData()
         if len(self.rangeArray) > int(self.gui.appSettings['memoryDepth']):
             self.rxPowerWattsArray = self.rxPowerWattsArray[1:]
             self.rxPowerArray = self.rxPowerArray[1:]
+            self.fppArray = self.fppArray[1:]
             self.rangeFPPWattsArray = self.rangeFPPWattsArray[1:]
             self.maxNoiseArray = self.maxNoiseArray[1:]
             self.stdNoiseArray = self.stdNoiseArray[1:]
             self.rangeArray = self.rangeArray[1:]
             self.rangeFilteredArray = self.rangeFilteredArray[1:]
             self.chartPointsX = self.chartPointsX[1:]
         if len(self.rangeArrayAll) > int(self.gui.appSettings['memoryDepth']):
             self.rxPowerArrayAll = self.rxPowerArrayAll[1:]
+            self.fppArrayAll = self.fppArrayAll[1:]
             self.maxNoiseArrayAll = self.maxNoiseArrayAll[1:]
             self.stdNoiseArrayAll = self.stdNoiseArrayAll[1:]
             self.rangeArrayAll = self.rangeArrayAll[1:]
             self.rangeFilteredArrayAll = self.rangeFilteredArrayAll[1:]
             self.chartPointsXAll = self.chartPointsXAll[1:]
     # Update GUI
         # self.gui.guiPacketUpdates(packet)
```

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/TDSR_settings.py` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/TDSR_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from json import dumps, loads
 
-__version__ = "1.541"
+__version__ = "1.542"
 
 # loads and saves GUI settings. Also sets default values if settings file does not include all keys.
 class appSettings():
     def __init__(self):
         self.settings = {}
 
     def settingsSetup(self):
```

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_Support/crc16.py` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_Support/crc16.py`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_UWB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDSR-UWB
-Version: 1.541
+Version: 1.542
 Summary: Support libraries for TDSR LLC UWB Radios
 Home-page: UNKNOWN
 Author: TDSR-LLC
 Author-email: contact@tdsr-uwb.com
 License: UNKNOWN
 Project-URL: Company:, https://www.tdsr-uwb.com
 Platform: UNKNOWN
```

### Comparing `TDSR-UWB-1.541/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt` & `TDSR-UWB-1.542/TDSR-UWB/TDSR_UWB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDSR-UWB-1.541/setup.py` & `TDSR-UWB-1.542/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="TDSR-UWB",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.541",  # Required
+    version="1.542",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Support libraries for TDSR LLC UWB Radios",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

