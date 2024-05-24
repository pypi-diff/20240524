# Comparing `tmp/santa_iw-0.7.4.tar.gz` & `tmp/santa_iw-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "santa_iw-0.7.4.tar", max compression
+gzip compressed data, was "santa_iw-0.9.0.tar", max compression
```

## Comparing `santa_iw-0.7.4.tar` & `santa_iw-0.9.0.tar`

### file list

```diff
@@ -1,76 +1,100 @@
--rw-r--r--   0        0        0     1075 2024-05-09 20:26:26.420102 santa_iw-0.7.4/LICENSE.txt
--rw-r--r--   0        0        0     3351 2024-05-15 16:43:51.996453 santa_iw-0.7.4/README.md
--rw-r--r--   0        0        0     1265 2024-05-09 20:26:26.421102 santa_iw-0.7.4/Santa_IW/DBConnection.py
--rw-r--r--   0        0        0     8718 2024-05-14 18:25:52.223959 santa_iw-0.7.4/Santa_IW/DataRecording.py
--rw-r--r--   0        0        0    31302 2024-05-15 15:50:54.252006 santa_iw-0.7.4/Santa_IW/Discovery.py
--rw-r--r--   0        0        0     1651 2024-05-09 20:26:26.421102 santa_iw-0.7.4/Santa_IW/DiscoveryHelper.py
--rw-r--r--   0        0        0    12745 2024-05-14 18:21:25.055379 santa_iw-0.7.4/Santa_IW/Flask/WebGUI.py
--rw-r--r--   0        0        0        0 2024-05-09 20:26:26.421102 santa_iw-0.7.4/Santa_IW/Flask/__init__.py
--rw-r--r--   0        0        0    20496 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/static/images/santa.jpg
--rw-r--r--   0        0        0     9523 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/static/images/santa_button.jpg
--rw-r--r--   0        0        0      834 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/templates/BoostrapBase.html.jinja
--rw-r--r--   0        0        0     3524 2024-05-10 14:34:18.046847 santa_iw-0.7.4/Santa_IW/Flask/templates/NavigationBar.html.jinja
--rw-r--r--   0        0        0      894 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/templates/OfflineBoostrapBase.html.jinja
--rw-r--r--   0        0        0      976 2024-05-10 14:45:23.384624 santa_iw-0.7.4/Santa_IW/Flask/templates/control_page.html.jinja
--rw-r--r--   0        0        0     2112 2024-05-10 14:45:23.388624 santa_iw-0.7.4/Santa_IW/Flask/templates/focus_page.html.jinja
--rw-r--r--   0        0        0      550 2024-05-10 15:39:25.758191 santa_iw-0.7.4/Santa_IW/Flask/templates/page_footer.html.jinja
--rw-r--r--   0        0        0     1639 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/templates/table_analog_stats.html.jinja
--rw-r--r--   0        0        0      842 2024-05-09 20:26:26.422102 santa_iw-0.7.4/Santa_IW/Flask/templates/table_config.html.jinja
--rw-r--r--   0        0        0      895 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/Flask/templates/table_discrete_stats.html.jinja
--rw-r--r--   0        0        0      946 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/Flask/templates/table_internal_status.html.jinja
--rw-r--r--   0        0        0     1341 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/Flask/templates/table_subsystems.html.jinja
--rw-r--r--   0        0        0       59 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/PLUGIN_CONFIG/Hue.json_disabled
--rw-r--r--   0        0        0      142 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/TEMPLATES/Cockpit.json
--rw-r--r--   0        0        0      129 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/TEMPLATES/PingIntranet.json
--rw-r--r--   0        0        0      121 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/TEMPLATES/PingSloppy.json
--rw-r--r--   0        0        0      343 2024-05-10 20:34:57.538717 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/prototype_discovery.json
--rw-r--r--   0        0        0     1607 2024-05-10 14:05:28.346026 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/prototype_gnas_discovery.json
--rw-r--r--   0        0        0      626 2024-05-15 14:21:44.851032 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/prototype_runtime.json
--rw-r--r--   0        0        0      750 2024-05-14 18:21:25.062379 santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/runtime_defaults.json
--rw-r--r--   0        0        0     4546 2024-05-14 19:15:37.776775 santa_iw-0.7.4/Santa_IW/Main.py
--rw-r--r--   0        0        0     2493 2024-05-12 19:23:55.646340 santa_iw-0.7.4/Santa_IW/Naughty.py
--rw-r--r--   0        0        0     3297 2024-05-09 20:26:26.427102 santa_iw-0.7.4/Santa_IW/Node.py
--rw-r--r--   0        0        0     4975 2024-05-15 16:19:57.978116 santa_iw-0.7.4/Santa_IW/NodeFactory.py
--rw-r--r--   0        0        0     8131 2024-05-15 16:30:30.912789 santa_iw-0.7.4/Santa_IW/NorthPole.py
--rwxr-xr-x   0        0        0     4898 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/PLUGIN_MODULES/AttachHue.py
--rw-r--r--   0        0        0        0 2024-05-09 20:26:26.423102 santa_iw-0.7.4/Santa_IW/PLUGIN_MODULES/__init__.py
--rw-r--r--   0        0        0      520 2024-05-09 20:26:26.427102 santa_iw-0.7.4/Santa_IW/PluginBase.py
--rw-r--r--   0        0        0     6756 2024-05-15 16:19:57.966116 santa_iw-0.7.4/Santa_IW/PluginFactory.py
--rw-r--r--   0        0        0      687 2024-05-09 20:26:26.427102 santa_iw-0.7.4/Santa_IW/PluginType.py
--rw-r--r--   0        0        0     4087 2024-05-09 20:26:26.427102 santa_iw-0.7.4/Santa_IW/Status.py
--rw-r--r--   0        0        0    20717 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/Subassembly.py
--rwxr-xr-x   0        0        0     2658 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/ApcAccess.py
--rwxr-xr-x   0        0        0     2570 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/DiskFree.py
--rw-r--r--   0        0        0     5053 2024-05-11 13:20:54.909267 santa_iw-0.7.4/Santa_IW/TEST_MODULES/HTTPTest.py
--rwxr-xr-x   0        0        0     2677 2024-05-14 18:25:52.193959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/IPVx_Address.py
--rwxr-xr-x   0        0        0     3259 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/PendingUpdates.py
--rw-r--r--   0        0        0     7525 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/PingTest.py
--rwxr-xr-x   0        0        0     1462 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/RemoteProcess.py
--rwxr-xr-x   0        0        0     1244 2024-05-14 18:25:52.203959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/SE_Status.py
--rwxr-xr-x   0        0        0     1722 2024-05-09 20:26:26.424102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/SNMP_id.py
--rwxr-xr-x   0        0        0     7903 2024-05-14 18:25:52.231959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Sensors.py
--rwxr-xr-x   0        0        0     1259 2024-05-14 18:25:52.218959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Shares_NFS.py
--rwxr-xr-x   0        0        0     1983 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Shares_SMB.py
--rwxr-xr-x   0        0        0     4656 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/SmartCtl.py
--rwxr-xr-x   0        0        0     5921 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/SystemctlFailed.py
--rwxr-xr-x   0        0        0     3583 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/TimeMachine.py
--rwxr-xr-x   0        0        0     1433 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Uname.py
--rwxr-xr-x   0        0        0     3653 2024-05-09 20:26:26.425102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Uptime.py
--rwxr-xr-x   0        0        0     4296 2024-05-14 18:25:52.212959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/ZFS_Snapshots.py
--rwxr-xr-x   0        0        0     1026 2024-05-14 18:25:52.227959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/ZFS_Version.py
--rwxr-xr-x   0        0        0     2588 2024-05-14 18:25:52.237959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Zpool_Free.py
--rwxr-xr-x   0        0        0     2865 2024-05-14 18:25:52.234959 santa_iw-0.7.4/Santa_IW/TEST_MODULES/Zpool_Status.py
--rw-r--r--   0        0        0        0 2024-05-09 20:26:26.426102 santa_iw-0.7.4/Santa_IW/TEST_MODULES/__init__.py
--rw-r--r--   0        0        0     5020 2024-05-15 16:09:51.907602 santa_iw-0.7.4/Santa_IW/TemplateFactory.py
--rw-r--r--   0        0        0     6954 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/TestBase.py
--rw-r--r--   0        0        0     8204 2024-05-15 16:17:51.191380 santa_iw-0.7.4/Santa_IW/TestFactory.py
--rw-r--r--   0        0        0      666 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/TestType.py
--rw-r--r--   0        0        0     5150 2024-05-15 14:13:07.826048 santa_iw-0.7.4/Santa_IW/TreeRoot.py
--rw-r--r--   0        0        0     2284 2024-05-14 18:25:52.184959 santa_iw-0.7.4/Santa_IW/UnitTests/DBConnection_test.py
--rw-r--r--   0        0        0      624 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/UnitTests/Status_test.py
--rw-r--r--   0        0        0     1947 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/UnitTests/Subassembly_test.py
--rw-r--r--   0        0        0        0 2024-05-09 20:26:26.428102 santa_iw-0.7.4/Santa_IW/UnitTests/__init__.py
--rw-r--r--   0        0        0     3123 2024-05-09 20:26:26.429102 santa_iw-0.7.4/Santa_IW/Utils.py
--rw-r--r--   0        0        0        0 2024-05-09 20:26:26.429102 santa_iw-0.7.4/Santa_IW/__init__.py
--rw-r--r--   0        0        0     1793 2024-05-15 16:43:55.992477 santa_iw-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     4868 1970-01-01 00:00:00.000000 santa_iw-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-09 20:26:26.420102 santa_iw-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     2579 2024-05-24 00:41:46.523223 santa_iw-0.9.0/README.md
+-rw-r--r--   0        0        0     1523 2024-05-19 13:35:27.178624 santa_iw-0.9.0/Santa_IW/DBConnection.py
+-rw-r--r--   0        0        0     9016 2024-05-19 18:25:24.079320 santa_iw-0.9.0/Santa_IW/DataRecording.py
+-rw-r--r--   0        0        0     7882 2024-05-19 23:21:43.122614 santa_iw-0.9.0/Santa_IW/Discovery.py
+-rw-r--r--   0        0        0    13902 2024-05-19 23:21:11.572431 santa_iw-0.9.0/Santa_IW/Flask/WebGUI.py
+-rw-r--r--   0        0        0      258 2024-05-19 13:35:27.179624 santa_iw-0.9.0/Santa_IW/Flask/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-19 13:35:27.179624 santa_iw-0.9.0/Santa_IW/Flask/static/images/Images.md
+-rw-r--r--   0        0        0    16095 2024-05-15 20:24:58.190417 santa_iw-0.9.0/Santa_IW/Flask/static/images/cheese-bell-1915234.svg
+-rw-r--r--   0        0        0   174462 2024-05-15 20:24:43.431330 santa_iw-0.9.0/Santa_IW/Flask/static/images/cheese-bell-1915234_1280.png
+-rw-r--r--   0        0        0   343120 2024-05-15 20:23:17.550824 santa_iw-0.9.0/Santa_IW/Flask/static/images/christmas-3827956.svg
+-rw-r--r--   0        0        0   253410 2024-05-15 20:23:04.146745 santa_iw-0.9.0/Santa_IW/Flask/static/images/christmas-3827956_1280.png
+-rw-r--r--   0        0        0    57707 2024-05-19 13:35:27.180624 santa_iw-0.9.0/Santa_IW/Flask/static/images/christmas-3835790.svg
+-rw-r--r--   0        0        0    81320 2024-05-19 13:35:27.181624 santa_iw-0.9.0/Santa_IW/Flask/static/images/christmas-3835790_1280.png
+-rw-r--r--   0        0        0    35694 2024-05-19 13:35:27.181624 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa-1908028.svg
+-rw-r--r--   0        0        0   142048 2024-05-19 13:35:27.182624 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa-1908028_1280.png
+-rw-r--r--   0        0        0   347113 2024-05-19 18:25:24.082320 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa_circle_black.svg
+-rw-r--r--   0        0        0   347112 2024-05-19 18:25:24.084320 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa_circle_blue.svg
+-rw-r--r--   0        0        0   347112 2024-05-19 18:25:24.086320 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa_circle_gray.svg
+-rw-r--r--   0        0        0    86500 2024-05-19 13:35:27.182624 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa_circle_green.png
+-rw-r--r--   0        0        0   347107 2024-05-19 13:35:27.184624 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa_circle_green.svg
+-rw-r--r--   0        0        0   347114 2024-05-19 18:25:24.088320 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa_circle_purple.svg
+-rw-r--r--   0        0        0   347111 2024-05-19 18:25:24.091320 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa_circle_red.svg
+-rw-r--r--   0        0        0   347114 2024-05-19 18:25:24.093320 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa_circle_yellow.svg
+-rw-r--r--   0        0        0    86500 2024-05-19 13:35:27.185624 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa_outline_red.png
+-rw-r--r--   0        0        0    68325 2024-05-19 13:35:27.185624 santa_iw-0.9.0/Santa_IW/Flask/static/images/santa_outline_red.svg
+-rw-r--r--   0        0        0  1011186 2024-05-15 20:20:57.506999 santa_iw-0.9.0/Santa_IW/Flask/static/images/wind-7658818.svg
+-rw-r--r--   0        0        0   402680 2024-05-15 20:20:03.573681 santa_iw-0.9.0/Santa_IW/Flask/static/images/wind-7658818_1280.png
+-rw-r--r--   0        0        0      989 2024-05-19 13:35:27.185624 santa_iw-0.9.0/Santa_IW/Flask/templates/404_error.html.jinja
+-rw-r--r--   0        0        0      987 2024-05-19 13:35:27.185624 santa_iw-0.9.0/Santa_IW/Flask/templates/500_error.html.jinja
+-rw-r--r--   0        0        0      834 2024-05-09 20:26:26.422102 santa_iw-0.9.0/Santa_IW/Flask/templates/BoostrapBase.html.jinja
+-rw-r--r--   0        0        0     3927 2024-05-24 00:37:11.929566 santa_iw-0.9.0/Santa_IW/Flask/templates/NavigationBar.html.jinja
+-rw-r--r--   0        0        0      894 2024-05-09 20:26:26.422102 santa_iw-0.9.0/Santa_IW/Flask/templates/OfflineBoostrapBase.html.jinja
+-rw-r--r--   0        0        0      976 2024-05-10 14:45:23.384624 santa_iw-0.9.0/Santa_IW/Flask/templates/control_page.html.jinja
+-rw-r--r--   0        0        0     2112 2024-05-10 14:45:23.388624 santa_iw-0.9.0/Santa_IW/Flask/templates/focus_page.html.jinja
+-rw-r--r--   0        0        0      550 2024-05-10 15:39:25.758191 santa_iw-0.9.0/Santa_IW/Flask/templates/page_footer.html.jinja
+-rw-r--r--   0        0        0     1639 2024-05-09 20:26:26.422102 santa_iw-0.9.0/Santa_IW/Flask/templates/table_analog_stats.html.jinja
+-rw-r--r--   0        0        0      842 2024-05-09 20:26:26.422102 santa_iw-0.9.0/Santa_IW/Flask/templates/table_config.html.jinja
+-rw-r--r--   0        0        0     2320 2024-05-19 18:25:24.093320 santa_iw-0.9.0/Santa_IW/Flask/templates/table_discrete_stats.html.jinja
+-rw-r--r--   0        0        0      946 2024-05-09 20:26:26.423102 santa_iw-0.9.0/Santa_IW/Flask/templates/table_internal_status.html.jinja
+-rw-r--r--   0        0        0     1341 2024-05-09 20:26:26.423102 santa_iw-0.9.0/Santa_IW/Flask/templates/table_subsystems.html.jinja
+-rw-r--r--   0        0        0       59 2024-05-09 20:26:26.423102 santa_iw-0.9.0/Santa_IW/INSTALL_CONFIG/PLUGIN_CONFIG/Hue.json_disabled
+-rw-r--r--   0        0        0      142 2024-05-09 20:26:26.423102 santa_iw-0.9.0/Santa_IW/INSTALL_CONFIG/TEMPLATES/Cockpit.json
+-rw-r--r--   0        0        0      129 2024-05-09 20:26:26.423102 santa_iw-0.9.0/Santa_IW/INSTALL_CONFIG/TEMPLATES/PingIntranet.json
+-rw-r--r--   0        0        0      121 2024-05-09 20:26:26.423102 santa_iw-0.9.0/Santa_IW/INSTALL_CONFIG/TEMPLATES/PingSloppy.json
+-rw-r--r--   0        0        0      289 2024-05-16 20:59:34.214615 santa_iw-0.9.0/Santa_IW/INSTALL_CONFIG/prototype_discovery.json
+-rw-r--r--   0        0        0     1554 2024-05-19 23:21:43.122614 santa_iw-0.9.0/Santa_IW/INSTALL_CONFIG/prototype_gnas_discovery.json
+-rw-r--r--   0        0        0      626 2024-05-15 14:21:44.851032 santa_iw-0.9.0/Santa_IW/INSTALL_CONFIG/prototype_runtime.json
+-rw-r--r--   0        0        0      750 2024-05-14 18:21:25.062379 santa_iw-0.9.0/Santa_IW/INSTALL_CONFIG/runtime_defaults.json
+-rw-r--r--   0        0        0     4818 2024-05-19 13:35:27.186624 santa_iw-0.9.0/Santa_IW/Main.py
+-rw-r--r--   0        0        0     2751 2024-05-19 13:35:27.186624 santa_iw-0.9.0/Santa_IW/Naughty.py
+-rw-r--r--   0        0        0     3555 2024-05-19 13:35:27.186624 santa_iw-0.9.0/Santa_IW/Node.py
+-rw-r--r--   0        0        0    11375 2024-05-22 14:05:04.176733 santa_iw-0.9.0/Santa_IW/NodeDiscoveryCandidate.py
+-rw-r--r--   0        0        0     5233 2024-05-19 13:35:27.187624 santa_iw-0.9.0/Santa_IW/NodeFactory.py
+-rw-r--r--   0        0        0     8345 2024-05-19 13:35:27.187624 santa_iw-0.9.0/Santa_IW/NorthPole.py
+-rwxr-xr-x   0        0        0     5144 2024-05-19 13:35:27.187624 santa_iw-0.9.0/Santa_IW/PLUGIN_MODULES/AttachHue.py
+-rw-r--r--   0        0        0      258 2024-05-19 13:35:27.187624 santa_iw-0.9.0/Santa_IW/PLUGIN_MODULES/__init__.py
+-rw-r--r--   0        0        0      778 2024-05-19 13:35:27.187624 santa_iw-0.9.0/Santa_IW/PluginBase.py
+-rw-r--r--   0        0        0     7014 2024-05-19 13:35:27.187624 santa_iw-0.9.0/Santa_IW/PluginFactory.py
+-rw-r--r--   0        0        0     1833 2024-05-19 13:35:27.188624 santa_iw-0.9.0/Santa_IW/PluginHelper.py
+-rw-r--r--   0        0        0      945 2024-05-19 13:35:27.188624 santa_iw-0.9.0/Santa_IW/PluginType.py
+-rw-r--r--   0        0        0     4345 2024-05-19 13:35:27.188624 santa_iw-0.9.0/Santa_IW/Status.py
+-rw-r--r--   0        0        0    21087 2024-05-19 13:35:27.188624 santa_iw-0.9.0/Santa_IW/Subassembly.py
+-rwxr-xr-x   0        0        0     3343 2024-05-19 13:35:27.188624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/ApcAccess.py
+-rwxr-xr-x   0        0        0     4983 2024-05-19 13:35:27.189624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/DiskFree.py
+-rw-r--r--   0        0        0     6628 2024-05-19 13:35:27.189624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/HTTPTest.py
+-rwxr-xr-x   0        0        0     3945 2024-05-19 19:49:42.824008 santa_iw-0.9.0/Santa_IW/TEST_MODULES/IPVx_Address.py
+-rwxr-xr-x   0        0        0     3838 2024-05-19 13:35:27.189624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/PendingUpdates.py
+-rw-r--r--   0        0        0     8937 2024-05-19 13:35:27.189624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/PingTest.py
+-rwxr-xr-x   0        0        0     2746 2024-05-19 13:35:27.189624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/RemoteProcess.py
+-rwxr-xr-x   0        0        0     1884 2024-05-19 13:35:27.190624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/SE_Status.py
+-rwxr-xr-x   0        0        0     2383 2024-05-22 14:05:04.176733 santa_iw-0.9.0/Santa_IW/TEST_MODULES/SNMP_id.py
+-rwxr-xr-x   0        0        0     8547 2024-05-19 13:35:27.190624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/Sensors.py
+-rwxr-xr-x   0        0        0     2111 2024-05-19 13:35:27.190624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/Shares_NFS.py
+-rwxr-xr-x   0        0        0     3632 2024-05-19 13:35:27.190624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/Shares_SMB.py
+-rwxr-xr-x   0        0        0     6178 2024-05-19 13:35:27.190624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/SmartCtl.py
+-rwxr-xr-x   0        0        0     6518 2024-05-19 13:35:27.191624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/SystemctlFailed.py
+-rwxr-xr-x   0        0        0     4655 2024-05-19 13:35:27.191624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/TimeMachine.py
+-rwxr-xr-x   0        0        0     2126 2024-05-19 13:35:27.191624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/Uname.py
+-rwxr-xr-x   0        0        0     4218 2024-05-19 13:35:27.191624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/Uptime.py
+-rwxr-xr-x   0        0        0     7500 2024-05-19 13:35:27.191624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/ZFS_Snapshots.py
+-rwxr-xr-x   0        0        0     1748 2024-05-19 13:35:27.191624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/ZFS_Version.py
+-rwxr-xr-x   0        0        0     3445 2024-05-19 13:35:27.192624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/Zpool_Free.py
+-rwxr-xr-x   0        0        0     3718 2024-05-19 13:35:27.192624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/Zpool_Status.py
+-rw-r--r--   0        0        0      258 2024-05-19 13:35:27.192624 santa_iw-0.9.0/Santa_IW/TEST_MODULES/__init__.py
+-rw-r--r--   0        0        0     5278 2024-05-19 13:35:27.192624 santa_iw-0.9.0/Santa_IW/TemplateFactory.py
+-rw-r--r--   0        0        0     7212 2024-05-19 13:35:27.192624 santa_iw-0.9.0/Santa_IW/TestBase.py
+-rw-r--r--   0        0        0     1320 2024-05-19 13:35:27.193624 santa_iw-0.9.0/Santa_IW/TestDiscoveryBase.py
+-rw-r--r--   0        0        0     8816 2024-05-19 13:35:27.193624 santa_iw-0.9.0/Santa_IW/TestFactory.py
+-rw-r--r--   0        0        0     2093 2024-05-19 13:35:27.193624 santa_iw-0.9.0/Santa_IW/TestPluginHelper.py
+-rw-r--r--   0        0        0      924 2024-05-19 13:35:27.193624 santa_iw-0.9.0/Santa_IW/TestType.py
+-rw-r--r--   0        0        0     5892 2024-05-19 13:35:27.193624 santa_iw-0.9.0/Santa_IW/TreeRoot.py
+-rw-r--r--   0        0        0     2542 2024-05-19 13:35:27.194624 santa_iw-0.9.0/Santa_IW/UnitTests/DBConnection_test.py
+-rw-r--r--   0        0        0      882 2024-05-19 13:35:27.194624 santa_iw-0.9.0/Santa_IW/UnitTests/Status_test.py
+-rw-r--r--   0        0        0     2205 2024-05-19 13:35:27.194624 santa_iw-0.9.0/Santa_IW/UnitTests/Subassembly_test.py
+-rw-r--r--   0        0        0      258 2024-05-19 13:35:27.194624 santa_iw-0.9.0/Santa_IW/UnitTests/__init__.py
+-rw-r--r--   0        0        0     3381 2024-05-19 13:35:27.194624 santa_iw-0.9.0/Santa_IW/Utils.py
+-rw-r--r--   0        0        0      258 2024-05-19 13:35:27.194624 santa_iw-0.9.0/Santa_IW/__init__.py
+-rw-r--r--   0        0        0     1795 2024-05-24 00:37:40.529739 santa_iw-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4096 1970-01-01 00:00:00.000000 santa_iw-0.9.0/PKG-INFO
```

### Comparing `santa_iw-0.7.4/LICENSE.txt` & `santa_iw-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `santa_iw-0.7.4/README.md` & `santa_iw-0.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,36 @@
-["Santa Is Watching" (aka Santa_IW)](https://gitlab.com/SRG_gitlab/santa-is-watching) is a network monitoring tool with an 
-emphasis on ZFS and network attached storage in a homelab environment. Based upon configuration files describing your 
-system, Santa_IW periodically cycles through a suite of
-tests on your computers, disks, and network hardware. Santa_IW runs on a single Linux computer which needs ssh keys
-to run diagnostic commands on other computers in your system. Santa_IW includes a network discovery tool which takes a
-list of start and stop network addresses to scan and tries to determine what tests are appropriate for each node it
-finds. Any computer which responds to a network ping becomes a candidate for ping testing. If Santa_IW can make an 
-ssh connection to the node, it will:
-
-* look at temperature and other data reported by lm-sensors
-* look for drives listed in /etc/fstab and monitor each for disk free space
-* look for drives supported by smartctl and report SMART status on them
-* look for zfs pools and check each for status and free space
-* look for zfs volumes which seem to be getting frequent snapshots (or are listed in pyznap's config file) and monitor
-  the age of the last snapshot
-* look for failed services reported by systemctl --failed
+["Santa Is Watching" (aka Santa_IW)](https://gitlab.com/SRG_gitlab/santa-is-watching) is a network monitoring tool with 
+an emphasis on ZFS and network attached storage in a homelab environment. Santa_IW can automatically discover hardware 
+on your intranet and build up a list of appropriate tests which will run periodically to monitor your network.
+Santa_IW runs on a single Linux computer which needs ssh keys to run diagnostic commands on other computers in your system. 
+
+If Santa_IW can make an ssh connection to the node, it schedules tests, which include:
+* monitor status and free space on zfs pools
+* monitor age of most recent snapshot on zfs volumes
+  * detects failures in periodic snapshot or send/receive pipelines
+* monitor NFS and SMB volume shares
+* monitor drive health as reported by smartctl
+* monitor drives listed in /etc/fstab for disk free space
+* monitor temperature and other data reported by lm-sensors
+* monitor for failed services reported by systemctl --failed
 
-Santa_IW is written entirely in Python (3.11 or later) and its configuration files are all editable json. It ships with 20+ built in test types
+Santa_IW is written entirely in Python (3.11 or later) and its configuration files are all editable json. It ships with 21 built in test types
 and can load additional user written tests or plugins from user directories. An example plugin is provided to use a
-Philips Hue color changing light bulb to provide a GREEN/YELLOW/RED status light.
+Philips Hue color changing light bulb to provide a GREEN/YELLOW/RED system status light.
 
 A web based interface lets the user navigate up and down the hierarchy of node groups, nodes and tests to see various
 levels of detail. Tests can record numeric data where appropriate. Running averages are displayed and values over time
-can be graphed or extracted for offline processing.
+can be graphed in the GUI or extracted for offline processing. 
 
 ----
 
-Santa_IW is hosted on [GitLab](https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home) and has been developed and tested on a Linux platform. It has been run installed and run on RHEL, Fedora, Ubuntu
+Santa_IW is hosted on [GitLab](https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home) and has been developed and tested on a Linux platform. It has been installed and run on RHEL, Fedora, Ubuntu
 and Debian platforms (including Raspberry Pi 3). It is written in pure Python, but calls out to many Linux/Posix
 command line utilities. It is plausible that it might someday work on other Posix compliant platforms (macOS or BSD),
 but that is out of scope for the current effort. [For windows support...](https://en.wikipedia.org/wiki/Somebody_else%27s_problem)
 
 Santa_IW is intended for homelab use on an internal network. It does not yet have any robust authentication system and
 should not be exposed on the open internet.
 
-# 🚧 PRE-BETA RELEASE 🚧
+A Reddit group has been setup for beta test participants at https://www.reddit.com/r/Santa_IW/
 
-If you are reading this, you are a little bit early to the party, but feel free to look
-around. Installation and operating instructions are on the [wiki](https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home)
-if you are interested in a test drive. The [Roadmap page]
-(https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/Roadmap) describes some of the work pending before I start 
-inviting people to beta test. The code as-is works well, but many of the pending changes planned will invalidate the 
-documentation. Expecting new users to read the manual once is a big ask these days, so asking them to do it all 
-again after major changes would be too much.
+Santa_IW (Code and Documentation) is published under an MIT License, Copyright (c) 2024 Steven Goncalo
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `santa_iw-0.7.4/Santa_IW/DBConnection.py` & `santa_iw-0.9.0/Santa_IW/DBConnection.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import logging
 from pathlib import Path
 
 from sqlalchemy import create_engine, Engine,text,CursorResult
 
 
 class DBConnection:
```

### Comparing `santa_iw-0.7.4/Santa_IW/DataRecording.py` & `santa_iw-0.9.0/Santa_IW/DataRecording.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from dataclasses import dataclass
 from io import BytesIO
 from threading import Thread
 from time import sleep, time
 from typing import Optional, NamedTuple
 
 import pandas as pd
@@ -179,16 +183,16 @@
 
     def get_astat_image(self, sensor: str):
         cmd = f"SELECT time,value FROM asamples WHERE name='{sensor}'"
         df: DataFrame = pd.read_sql_query(cmd, self.get_db_engine())
         if df.empty:
             self.logger.error(f"No data available for sensor {sensor}")
             return "/dev/null"
-        df['DateTime'] = pd.to_datetime(df['time'], unit='s')
-        fig = df.plot(y='value', x='DateTime').get_figure()
+        df['DateTime'] = pd.to_datetime(df['time'], unit='s',utc=True)
+        fig = df.plot(y='value', x='DateTime',xlabel="Time UTC",title=sensor).get_figure()
         img = BytesIO()
         fig.savefig(img, format='png')
         img.seek(0)
         return img
 
     def get_sensor_stats(self, outer_name, inner_name) -> ADStatsBase:
         name = self.prefix_name(f"{outer_name}_{inner_name}")
```

### Comparing `santa_iw-0.7.4/Santa_IW/DiscoveryHelper.py` & `santa_iw-0.9.0/Santa_IW/PluginHelper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import logging
 from typing import Type, Optional, Any
 
 from libsrg.Config import Config
 
 from Santa_IW.PluginBase import PluginBase
-from Santa_IW.TestBase import TestBase
 
 
-class DiscoveryHelper:
-    def __init__(self, loaded_class: Type[TestBase] | Type[PluginBase]):
+class PluginHelper:
+    def __init__(self, loaded_class: Type[PluginBase]):
         self.logger = logging.getLogger(__name__)
         self._loaded_class = loaded_class
         self._aliases: list[str] = []
         self._configs: dict[str, Config] = {}
 
     def alias(self, name: str, config: Optional[dict[str, Any] | Config] = None, **overrides) -> Config:
         """
@@ -34,9 +37,9 @@
         return new_config.copy()
 
     def get_all_configs(self) -> dict[str, Config]:
         if not self._aliases:
             self.alias(self._loaded_class.__name__, {})
         return self._configs
 
-    def get_loaded_class(self) -> Type[TestBase] | Type[PluginBase]:
+    def get_loaded_class(self) -> Type[PluginBase]:
         return self._loaded_class
```

### Comparing `santa_iw-0.7.4/Santa_IW/Flask/WebGUI.py` & `santa_iw-0.9.0/Santa_IW/Flask/WebGUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import datetime
 import html
 import os
 import signal
 import sys
 import threading
 from pathlib import Path
@@ -151,26 +155,44 @@
 * child_tests - test children of focus
 * body - block of preformatted text
 * time_slug - footer text (expected to include time of day)
 
         :param name:
         :return:
         """
-        now = datetime.datetime.now()
-        current_time_txt = now.strftime("%Y-%m-%d %H:%M:%S")
+        now = datetime.datetime.now(datetime.timezone.utc).astimezone()
+        current_time_txt = now.strftime("%Y-%m-%d %H:%M:%S %Z")
         self.runtime.stop()
         elapsed_time_txt = self.runtime.elapsed_asc()
         focus: Subassembly = self.find_subsystem(name) if not self.shutting_down else self.tree_root_subassembly
         version = self.config().get_item("SANTA_IW_VERSION")
         branch = self.config().get_item("branch", default="local")
+        status = focus.latest_status()
+        if status== Status.OK:
+            logo="santa_circle_green.svg"
+        elif status== Status.CRITICAL:
+            logo="santa_circle_red.svg"
+        elif status == Status.WARNING:
+            logo = "santa_circle_yellow.svg"
+        elif status== Status.UNKNOWN:
+            logo="santa_circle_purple.svg"
+        elif status== Status.NODATA:
+            logo="santa_circle_black.svg"
+        elif status== Status.MAINT:
+            logo="santa_circle_gray.svg"
+        else:
+            logo="santa_circle_blue.svg"
+
+        local_hostname = self.config().get_item("localhost_hostname", default="localhost")
         flask_config = Config({
-            "title": f"SHUTDOWN",
+            "title": f"{local_hostname} SHUTDOWN",
             "root_tint": self.tree_root_subassembly.latest_status().tint(),
             "focus_tint": focus.latest_status().tint(),
             "focus": focus,
+            "logo": logo,
             "root": self.tree_root_subassembly,
             "parent": focus.parent(),
             "stepparent": focus.stepparent(),
             "trail": [focus],
             "child_nodes": None,
             "child_tests": None,
             "suspects": None,
@@ -182,24 +204,24 @@
             "astats": None,
             "dstats": None,
             "istats": None,
             "cstats": None,
             "webgui": self,
             "refresh_interval": None,
             "focus_config_list": self.sort_config_list(focus),
-            "localhost": self.config().get_item("localhost_hostname", default="localhost"),
+            "localhost": local_hostname,
             "image": None,
         })
         if self.shutting_down:
             self.logger.info(f"Preparing shutdown page")
             flask_config.set_item("title", "SHUTDOWN")
             return flask_config
         self.logger.info(f"Preparing page for {name}")
         sub = focus
-        flask_config.set_item("title", f"Status for {focus.name()}")
+        flask_config.set_item("title", f"{local_hostname} Santa_IW")
 
         trail = []
         while sub is not None:
             trail.append(sub)
             sub = sub.parent()
         trail.reverse()
         flask_config.set_item("trail", trail)
@@ -353,7 +375,15 @@
     return response
 
 
 def get_headers(response):
     response.headers['Cache-Control'] = 'no-cache, no-store, must-revalidate'
     response.headers['Pragma'] = 'no-cache'
     response.headers['Expires'] = '0'
+
+@app.errorhandler(404)
+def page_not_found(e):
+    return render_template("404_error.html.jinja"),404
+
+@app.errorhandler(500)
+def internal_server_error(e):
+    return render_template("500_error.html.jinja"),500
```

### Comparing `santa_iw-0.7.4/Santa_IW/Flask/templates/BoostrapBase.html.jinja` & `santa_iw-0.9.0/Santa_IW/Flask/templates/BoostrapBase.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.7.4/Santa_IW/Flask/templates/NavigationBar.html.jinja` & `santa_iw-0.9.0/Santa_IW/Flask/templates/NavigationBar.html.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 <div class="container text-left">
     <div class="row">
         <div class="col col-sm-1"><a class="nav-link active" href="{{ url_for('jump',token="home") }}">
             <img
-                    src="{{ url_for('static', filename='images/santa_button.jpg') }}"
-                    class="image" style="width:100px;height:100px;" alt="Santa is watching"
+                    src="{{ url_for('static', filename='images/'+logo) }}"
+                    class="image" style="width:100px;height:100px;" alt="{{ logo }}"
             /></a>
         </div>
         <div class="col-lg-11">
             <ul class="nav">
                 <li class="nav-item">
                     <a class="nav-link active" href="{{ url_for('jump',token="home") }}">HOME</a>
                 </li>
                 <li class="nav-item">
-                    <a class="nav-link" href="{{ url_for('jump',token="naughty") }}">{{ webgui.config().get_item('tree_attention_char') }}Naughty</a>
+                    <a class="nav-link"
+                       href="{{ url_for('jump',token="naughty") }}">{{ webgui.config().get_item('tree_attention_char') }}Naughty</a>
                 </li>
                 <li class="nav-item">
                     <a class="nav-link" href="{{ url_for('jump',token="test_types") }}">Test Types</a>
                 </li>
                 {% if stepparent %}
                     <li class="nav-item">
                         <a class="nav-link"
@@ -35,33 +36,44 @@
                         <li><a class="dropdown-item"
                                href="{{ url_for("ack_page", ssname=focus.name()) }}">Ack {{ webgui.config().get_item('tree_attention_char') }}</a>
                         </li>
                         <li><a class="dropdown-item" href="{{ url_for("reset_page", ssname=focus.name()) }}">Reset
                             Stats</a></li>
                         <li><a class="dropdown-item" href="{{ url_for("run_page", ssname=focus.name()) }}">Run Tests</a>
                         </li>
-                        {% if focus.subsystem_is_enabled() %}
-                            <li><a class="dropdown-item"
-                                   href="{{ url_for("disable_page", ssname=focus.name()) }}">ENABLED->DISABLED</a></li>
-                        {% else %}
-                            <li><a class="dropdown-item"
-                                   href="{{ url_for("enable_page", ssname=focus.name()) }}">DISABLED->ENABLED</a></li>
+                        {% if False %}
+                            {% if focus.subsystem_is_enabled() %}
+                                <li><a class="dropdown-item"
+                                       href="{{ url_for("disable_page", ssname=focus.name()) }}">ENABLED->DISABLED</a>
+                                </li>
+                            {% else %}
+                                <li><a class="dropdown-item"
+                                       href="{{ url_for("enable_page", ssname=focus.name()) }}">DISABLED->ENABLED</a>
+                                </li>
+                            {% endif %}
+                            <li><a class="dropdown-item" href="{{ url_for('control') }}">Control Santa_IW</a></li>
                         {% endif %}
-                        <li><a class="dropdown-item" href="{{ url_for('control') }}">Control SIW</a></li>
+
                     </ul>
                 </li>
                 {#  <li>{{ current_time_txt }}<br/>on {{ localhost }} for {{ elapsed_time_txt }}</li>  #}
+                <li class="nav-item">
+                    <a class="nav-link"
+                       href="https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home">HELP/Wiki</a>
+                </li>
             </ul>
             <ul class="nav">
                 <li>
                     <pre>   {{ current_time_txt }}  </pre>
                 </li>
-                <li><pre> {{ version }} </pre></li>
                 <li>
-                    <pre>  Running on {{ localhost }} for {{ elapsed_time_txt }}  </pre>
+                    <pre> {{ version }} </pre>
+                </li>
+                <li>
+                    <pre>  Uptime {{ elapsed_time_txt }}  </pre>
                 </li>
                 <li class="nav-item">
                 </li>
             </ul>
 
         </div>
     </div>
```

### Comparing `santa_iw-0.7.4/Santa_IW/Flask/templates/OfflineBoostrapBase.html.jinja` & `santa_iw-0.9.0/Santa_IW/Flask/templates/OfflineBoostrapBase.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.7.4/Santa_IW/Flask/templates/control_page.html.jinja` & `santa_iw-0.9.0/Santa_IW/Flask/templates/control_page.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.7.4/Santa_IW/Flask/templates/focus_page.html.jinja` & `santa_iw-0.9.0/Santa_IW/Flask/templates/focus_page.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.7.4/Santa_IW/Flask/templates/page_footer.html.jinja` & `santa_iw-0.9.0/Santa_IW/Flask/templates/page_footer.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.7.4/Santa_IW/Flask/templates/table_analog_stats.html.jinja` & `santa_iw-0.9.0/Santa_IW/Flask/templates/table_analog_stats.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.7.4/Santa_IW/Flask/templates/table_config.html.jinja` & `santa_iw-0.9.0/Santa_IW/Flask/templates/table_config.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.7.4/Santa_IW/Flask/templates/table_discrete_stats.html.jinja` & `santa_iw-0.9.0/Santa_IW/Flask/templates/table_subsystems.html.jinja`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 {# define table_cap and table_subs before including #}
 {% if table_subs %}
-<br/>
+    <br/>
 
-<caption class="caption">{{ table_cap }}</caption>
-<table style="width:1200px" class="table table-striped table-bordered">
-    <thead class="table-dark">
-    <tr style="background-color:#0000c0;color:white;">
-        <th style="width:20%">Name</th>
-        <th style="width:65%">Counts</th>
-        <th style="width:15%">Count</th>
-    </tr>
-    </thead>
-    {% set fmt="{val:.8g}" %}
-    {% for stat in table_subs %}
-    {% set rowcol = 'white' %}
-    <tr style="background-color:{{ rowcol }}">
-        <td>{{ stat.name() }}</td>
-        <td>
-            {% autoescape false %}
-            {{ webgui.escape(stat.most_common_as_str(5)) }}
-            {% endautoescape %}
-        </td>
-        <td>
-            {{ fmt.format(val=stat.count()) }}
-        </td>
+    <caption class="caption">{{ table_cap }}</caption>
+    <table style="width:1200px" class="table table-striped table-bordered">
+        <thead class="table-dark">
+            <tr style="background-color:#0000c0;color:white;">
+                <th>Status</th>
+                <th>Subsystem</th>
+                <th>Annotation</th>
+            </tr>
+        </thead>
+        {% for child in table_subs %}
+            {% if child %}
+                {% set stat = child.latest_status() %}
+                {% set col = stat.html_color() %}
+                {% set rowcol = '#d0d0d0' if "__" in child.name() else 'white' %}
+                <tr style="background-color:{{ rowcol }}">
+                    <td style="color:{{ col }};background-color:black;width:8%;text-align:center">
+                       {{ stat.emoji() }} {{ stat.name }}
+                    </td>
+                    <td style="width:30%">
+                        <a href="/focus/{{ child.name() }}">{{ child.name() }}</a>
+                    </td>
+                    <td style="width:62%;font-family:monospace">
+                        {{ child.annotation() }}
+                    </td>
 
-    </tr>
-    {% endfor %}
-</table>
-<br/>
+                </tr>
+            {% endif %}
+        {% endfor %}
+    </table>
+    <br/>
 {% endif %}
```

#### html2text {}

```diff
@@ -1,9 +1,6 @@
 {# define table_cap and table_subs before including #} {% if table_subs %}
 {{ table_cap }}
-NNaammee              CCoouunnttss                       CCoouunntt
-                  {% autoescape false %} {
-{{ stat.name() }} { webgui.escape              {{ fmt.format(val=stat.count())
-                  (stat.most_common_as_str(5)) }}
-                  }} {% endautoescape %}
+SSttaattuuss                             SSuubbssyysstteemm          AAnnnnoottaattiioonn
+{{ stat.emoji() }} {{ stat.name }} _{_{_ _c_h_i_l_d_._n_a_m_e_(_)_ _}_} {{ child.annotation() }}
 
 {% endif %}
```

### Comparing `santa_iw-0.7.4/Santa_IW/Flask/templates/table_internal_status.html.jinja` & `santa_iw-0.9.0/Santa_IW/Flask/templates/table_internal_status.html.jinja`

 * *Files identical despite different names*

### Comparing `santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/prototype_gnas_discovery.json` & `santa_iw-0.9.0/Santa_IW/INSTALL_CONFIG/prototype_gnas_discovery.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.59375%*

 * *Differences: {"'additional_per_node'": "{'mbp14': OrderedDict([('suppress_discovery', ['SNMP_id'])])}",*

 * * 'delete': "['nuke_old_hosts', 'nuke_user_config', 'additional_santa_config']"}*

```diff
@@ -1,17 +1,19 @@
 {
     "additional_per_node": {
+        "mbp14": {
+            "suppress_discovery": [
+                "SNMP_id"
+            ]
+        },
         "nas0": {
             "templates": [],
             "tests": []
         }
     },
-    "additional_santa_config": {
-        "additional_item": 42
-    },
     "explicit_group_assignments": {
         "38:F7:3D": "!drop amazon",
         "68:37:E9": "!drop amazon",
         "E2:13:B7": "!randomized mac?",
         "iphone-5": "MOBILE",
         "mbp13": "MOBILE",
         "mbp14": "MOBILE",
@@ -35,16 +37,14 @@
             "propagate_child_status_in_overall": false
         },
         "NETWORK": {},
         "NONESSENTIAL": {
             "propagate_child_status_in_overall": false
         }
     },
-    "nuke_old_hosts": true,
-    "nuke_user_config": true,
     "scan_defaults": {
         "Darwin": "MOBILE",
         "Linux": "HOSTS",
         "overwrite": true,
         "unknown": "IOT"
     },
     "scans": [
```

### Comparing `santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/prototype_runtime.json` & `santa_iw-0.9.0/Santa_IW/INSTALL_CONFIG/prototype_runtime.json`

 * *Files identical despite different names*

### Comparing `santa_iw-0.7.4/Santa_IW/INSTALL_CONFIG/runtime_defaults.json` & `santa_iw-0.9.0/Santa_IW/INSTALL_CONFIG/runtime_defaults.json`

 * *Files identical despite different names*

### Comparing `santa_iw-0.7.4/Santa_IW/Main.py` & `santa_iw-0.9.0/Santa_IW/Main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import argparse
 import atexit
 import logging
 import logging.config
 import os
 import pprint
 
@@ -114,15 +118,15 @@
 
             # load the defaults file
             defaults_config = Config(np.default_runtime_file, localhost_config, startup_config)
 
             # noinspection PyUnboundLocalVariable
             primary_config = Config(np.user_runtime_file, defaults_config)
 
-            self.tree_root = TreeRoot(primary_config)
+            self.tree_root = TreeRoot(primary_config,north_pole=np)
             self.tree_root.start()
             LoggingCounter.rotate_files()
             exit(0)
 
         except Exception as e:
             self.logger.exception(f"Fatal: {type(e)} {e}", stack_info=True, exc_info=True)
             exit(1)
```

### Comparing `santa_iw-0.7.4/Santa_IW/Naughty.py` & `santa_iw-0.9.0/Santa_IW/Naughty.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from libsrg.Config import Config
 
 from Santa_IW.Node import Node
 from Santa_IW.Status import Status
 from Santa_IW.Subassembly import Subassembly
 from Santa_IW.TestBase import TestBase
```

### Comparing `santa_iw-0.7.4/Santa_IW/Node.py` & `santa_iw-0.9.0/Santa_IW/Node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import threading
 from threading import Semaphore
 
 from libsrg.Config import Config
 from libsrg.Info import Info
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
```

### Comparing `santa_iw-0.7.4/Santa_IW/NodeFactory.py` & `santa_iw-0.9.0/Santa_IW/NodeFactory.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from collections import ChainMap
 from pathlib import Path
 from typing import Any
 
 from libsrg.Config import Config
 
 from Santa_IW.Node import Node
```

### Comparing `santa_iw-0.7.4/Santa_IW/NorthPole.py` & `santa_iw-0.9.0/Santa_IW/NorthPole.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import shutil
 from pathlib import Path
 
 
 class NorthPole:
     """
     This class locates the directory tree for Santa_IW and generates a set of paths to key directories and files.
@@ -87,15 +91,15 @@
         self.setup_defaults_file = self.santa_opt_dir / 'setup_defaults.json'
         self.paths["__SETUP_DEFAULTS_FILE__"] = self.setup_defaults_file
 
         self.user_discovery_file = self.santa_user_config_dir / 'discovery.json'
         self.paths["__USER_DISCOVERY_FILE__"] = self.user_discovery_file
 
         self.user_runtime_file = self.santa_user_config_dir / 'runtime.json'
-        self.paths["__USER_RUNTIME_FILE__"] = self.user_discovery_file
+        self.paths["__USER_RUNTIME_FILE__"] = self.user_runtime_file
 
         self.default_runtime_file = self.santa_install_config_dir / 'runtime_defaults.json'
         self.paths["__INSTALL_RUNTIME_FILE__"] = self.default_runtime_file
 
         self.pyproject_toml_file = self.santa_clone_dir / 'pyproject.toml'
         self.paths["__PYPROJECT_TOML_FILE__"] = self.pyproject_toml_file
 
@@ -141,14 +145,13 @@
         :return: Path to where the file *was* before rotation
 
         """
         old = Path(f"{path}_{depth}") if depth > 0 else path
         if old.exists():
             if depth < keep_num:
                 nxt = self.rotate_out_file(path=path, depth=depth + 1, keep_num=keep_num)
+                print(f"Rotating {old} to {nxt}")
+                shutil.move(old, nxt)
             else:
-                nxt = Path(f"{path}_{depth + 1}")
-                print(f"Removing {nxt}")
-                shutil.rmtree(nxt)
-            print(f"Rotating {old} to {nxt}")
-            shutil.move(old, nxt)
+                print(f"Removing {old}")
+                shutil.rmtree(old)
         return old
```

### Comparing `santa_iw-0.7.4/Santa_IW/PLUGIN_MODULES/AttachHue.py` & `santa_iw-0.9.0/Santa_IW/PLUGIN_MODULES/AttachHue.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env  python3
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import asyncio
 import logging
 import threading
 
 from aiohue import HueBridgeV1
 from aiohue.v1.lights import Light
 from libsrg.Config import Config
@@ -51,17 +55,17 @@
                 self.last_light_status = status
                 thread= threading.Thread(target=self.helper.run_hue, args=(status,))
                 thread.start()
                 self.since_last_update.start()
                 self.num_light_updates += 1
 
 
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
+from Santa_IW.PluginHelper import PluginHelper
 
-plugin_helper: DiscoveryHelper = DiscoveryHelper(AttachHue)
+plugin_helper: PluginHelper = PluginHelper(AttachHue)
 plugin_helper.alias("AttachHue",
                     bridge="hue.home.goncalo.name",
                     hue_app_key="{{__HUE_APP_KEY__}}",
                     lightname="Santa_IW",
                     min_delay=30.0,
                     max_delay=120.0
```

### Comparing `santa_iw-0.7.4/Santa_IW/PluginFactory.py` & `santa_iw-0.9.0/Santa_IW/PluginFactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import importlib
 import importlib.util
 import sys
 from pathlib import Path
 from typing import List, Type
 
 from libsrg.Config import Config
```

### Comparing `santa_iw-0.7.4/Santa_IW/Status.py` & `santa_iw-0.9.0/Santa_IW/Status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import logging
 import threading
 from enum import Enum
 from typing import Any, Optional, Self
 
 
 # NAGIOS return codes :
```

### Comparing `santa_iw-0.7.4/Santa_IW/Subassembly.py` & `santa_iw-0.9.0/Santa_IW/Subassembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import logging
 import os
 import threading
 from collections import ChainMap
 from threading import Event
 from typing import Any, Self, Callable, Optional
 
@@ -210,15 +214,15 @@
             for child in self.children():
                 child.mark_subsystem_enabled(enable=enable, deep=deep)
 
     def subsystem_is_enabled(self):
         return self._subassembly_enabled.is_set()
 
     def start(self):
-        pass
+        self.log_internal_status(Status.OK,message="Started...")
 
     def spawn(self):
         self.logger.info(f"Spawning Subassembly {self} with direct_children {self._registered_direct_children}")
         for child in self._registered_direct_children.values():
             # noinspection PyTypeChecker
             self.logger.info(f"{self} Spawning {child}")
             child.mark_subsystem_enabled()
@@ -293,26 +297,27 @@
         self._pre_attention_status = new_status
 
     def clear_attention(self):
         for child in self.children():
             child.clear_attention()
         self._pre_attention_status = None
         self._attention_flag = False
-        self.log_internal_status(Status.NODATA, f"Cleared attention flag {self.name()}", assess=True)
+        self.log_internal_status(Status.NODATA, f"Cleared attention flag {self.name()}")
+        self.assess_overall_status(force=True)
 
     def set_annotation(self, text: str | None = None) -> None:
         self._overall_summation.set_message(text)
 
     ###################################################
     # Status Summation
     ###################################################
     def latest_status(self) -> Status:
         return self._overall_summation.worst()
 
-    def assess_overall_status(self) -> Status:
+    def assess_overall_status(self,force:bool=False) -> Status:
         with self._status_lock:
             prior_status = self._overall_summation.worst()
 
             self._child_assess_stats.sample(self._child_summation.worst())
             if self._propagate_child_status_in_overall:
                 self._overall_summation.add_from(self._child_summation)
 
@@ -327,15 +332,15 @@
             self.new_overall_status(prior_status, worst)
 
             changed = prior_status != worst
 
             # current is current elapsed time since start, without stopping timer
             age_last_status = self._since_last_notify.current()
             stale = age_last_status > self._observer_period_nochange
-            send = stale or changed or self._first_status or self._always_send_assessments
+            send = force or stale or changed or self._first_status or self._always_send_assessments
             self.update_attention(worst)
             self.logger.info(
                 f"Overall Status {worst.name}<-{prior_status.name} " +
                 f"{send=} {changed=} {stale=} {age_last_status=}")
             if send:
                 self.notify_status_observers()
                 self._first_status = False
```

### Comparing `santa_iw-0.7.4/Santa_IW/TEST_MODULES/ApcAccess.py` & `santa_iw-0.9.0/Santa_IW/TEST_MODULES/SE_Status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,56 @@
 #!/usr/bin/env  python3
-from libsrg.Config import Config
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from libsrg.Runner import Runner
-from libsrg.Statistics.ADStatsBase import ADStatsBase
-from libsrg.Statistics.AnalogStatsSlidingWindow import AnalogStatsSlidingWindow
-from libsrg.Statistics.DiscreteStatsCumulative import DiscreteStatsCumulative
 
-from Santa_IW.Subassembly import Subassembly
 from Santa_IW.TestBase import Status, TestBase
 
 
-class ApcAccess(TestBase):
-
-    def __init__(self, instance_config: Config, short_name: str, parent: Subassembly, stepparent: Subassembly):
-        super().__init__(instance_config=instance_config, parent=parent, stepparent=stepparent,
-                         short_name=short_name)  # super defines self.logger
-        self.apc_status_stats = DiscreteStatsCumulative(self.prefix_name("ReportedStatus"))
-        self.statistics_dict: [str, ADStatsBase] = {}
-        self.track_names = [
-            "LINEV", "LOADPCT", "BCHARGE", "TIMELEFT", "MBATTCHG", "MINTIMEL",
-            "MAXTIME", "BATTV", "NUMXFERS", "TONBATT",
-            "CUMONBATT", ]
-
-    def get_sensor_stats(self, outer_name, inner_name) -> ADStatsBase:
-        name = self.prefix_name(f"{outer_name}_{inner_name}")
-        if name in self.statistics_dict:
-            stat = self.statistics_dict[name]
-        else:
-            stat = AnalogStatsSlidingWindow(name=name, window=100)
-            self.statistics_dict[name] = stat
-        return stat
+# noinspection PyPep8Naming
+class SE_Status(TestBase):
 
     def run_test_once(self):
-        r = Runner("apcaccess -u", userat=self.userat, timeout=5,retries=2)
+        cmd = ["sestatus"]
+        self.logger.info(cmd)
+        r = Runner(cmd, userat=self.userat)
         ret = r.ret
-        stat = self.get_sensor_stats("APC", "return")
-        stat.sample(ret)
-        if ret != 0:
-            self.log_test_status(Status.UNKNOWN, message=f"Command Error 0x{ret:04x} {r}")
-            return
-        data = {}
-        for line in r.so_lines:
-            half = line.split(":", maxsplit=1)
-            name = half[0].strip()
-            value = half[1].strip()
-            data[name] = value
-            self.log_test_status(Status.OK, message=line)
-        for name in self.track_names:
-            if name in data:
-                value = float(data[name])
-                stat = self.get_sensor_stats("APC", name)
-                stat.sample(value)
-        status = data.get("STATUS", "missing")
-        self.apc_status_stats.sample(status)
-        if status == "ONLINE":
-            self.log_test_status(Status.OK, message=f"APC ONLINE")
+        self.logger.info(ret)
+        if ret == 127:
+            self.log_test_status(Status.OK, message="NA")
+        elif ret != 0:
+            self.log_test_status(Status.UNKNOWN, message=f"Command Error 0x{ret:04x}")
         else:
-            self.log_test_status(Status.WARNING, message=f"APC {status}")
-
+            lines = r.so_lines
+            ena = "UNKNOWN"
+            mode = "NA"
+            for line in lines:
+                parts = line.split(':')
+                if parts[0] == "SELinux status":
+                    ena = parts[1].strip()
+                if parts[0] == "Current mode":
+                    mode = parts[1].strip()
+
+            if ena == "enabled":
+                self.log_test_status(Status.OK, message=f"{ena} {mode}")
+            else:
+                self.log_test_status(Status.OK, message=f"{ena}")
+
+
+from Santa_IW.TestPluginHelper import TestPluginHelper
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
+
+
+# noinspection HttpUrlsUsage
+class LocalDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if self.can_ssh and self.kernel_name == "Linux":
+            r = Runner(f"sestatus", userat=self.userat, timeout=5)
+            if r.success:
+                self.add_test({"test_type": "SE_Status"})
 
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
 
-helper: DiscoveryHelper = DiscoveryHelper(ApcAccess)
-helper.alias("ApcAccess", {"period": 3 * TestBase.sc.minute})
+helper: TestPluginHelper = TestPluginHelper(SE_Status, LocalDiscovery)
+helper.alias("SE_Status", period=30 * TestBase.sc.minute)
```

### Comparing `santa_iw-0.7.4/Santa_IW/TEST_MODULES/HTTPTest.py` & `santa_iw-0.9.0/Santa_IW/TEST_MODULES/HTTPTest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from datetime import datetime
 from typing import Optional
 
 import requests
 from libsrg.Config import Config
 from libsrg.ElapsedTime import ElapsedTime
+from libsrg.Runner import Runner
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
 from libsrg.Statistics.DiscreteStatsCumulative import DiscreteStatsCumulative
 from requests import Response, get
 
 from Santa_IW.Subassembly import Subassembly
 from Santa_IW.TestBase import Status
 from Santa_IW.TestBase import TestBase
@@ -76,17 +81,48 @@
             return Status.OK
         except Exception as e:
             self.logger.exception(e, stack_info=True, exc_info=True)
             self.log_test_status(Status.CRITICAL, message=f"Exception: {type(e)} {str(e)}")
             return Status.CRITICAL
 
 
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
+from Santa_IW.TestPluginHelper import TestPluginHelper
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
+
+
+# noinspection HttpUrlsUsage
+class LocalDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if self.can_ssh:
+            r = Runner(f"systemctl is-enabled cockpit", userat=self.userat, timeout=5)
+            if r.success:
+                self.add_template("Cockpit")
+        urls = [f"http://{self.fqdn}", f"https://{self.fqdn}"]
+        if self.is_localhost:
+            # don't test santa interface across instances
+            # tends to pick up development testing and generate extra tests
+            # which fail when development activity pauses or stops
+            urls.append(f"http://{self.fqdn}:4242/")
+        for url_ in urls:
+            try:
+                response_: Response = get(url_, timeout=5)
+                code = response_.status_code
+                ok = code in [200]
+                self.logger.info(f"Response from {url_=} -> {code=} {ok=}")
+                if ok:
+                    self.add_test(
+                        {
+                            "test_type": "HTTPTest",
+                            "url": url_
+                        })
+            except Exception as e:
+                self.logger.warning(f"Exception while trying to get {url_=} -> {e}")
 
-helper = DiscoveryHelper(HTTPTest)
+helper = TestPluginHelper(HTTPTest,LocalDiscovery)
 # noinspection HttpUrlsUsage
 helper.alias("HTTPTest", {"allowed_status_codes": [200], "url": "http://{{fqdn}}", "period": 5 * TestBase.sc.minute})
 helper.alias("CockpitTest",
              {"allowed_status_codes": [200], "url": "https://{{fqdn}}:9090", "period": 10 * TestBase.sc.minute})
 
 if __name__ == "__main__":
     with requests.get("https://kylo.home.goncalo.name:9090", stream=True) as response:
```

### Comparing `santa_iw-0.7.4/Santa_IW/TEST_MODULES/IPVx_Address.py` & `santa_iw-0.9.0/Santa_IW/TEST_MODULES/SNMP_id.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,67 @@
 #!/usr/bin/env  python3
-import re
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 from libsrg.Runner import Runner
 
 from Santa_IW.TestBase import Status, TestBase
 
 
 # noinspection PyPep8Naming
-class IPVx_Address(TestBase):
+class SNMP_id(TestBase):
 
     # def extendParser(self):
+    #     pass
     #     # can set thresholds to allow known count of uncorrectable errors if needed
-    #     self.parser.add_argument("-g", "--global", action="store_const", dest="scope",
-    #     const="global", default="global",
-    #                              help="scope: global")
-    #     self.parser.add_argument("-l", "--link", action="store_const", dest="scope",
-    #     const="link", default="global",
-    #                              help="scope: link")
-    #     self.parser.add_argument("-4", "--ipv4", action="store_const", dest="inet",
-    #     const="inet", default="inet",
-    #                              help="inet: inet ")
-    #     self.parser.add_argument("-6", "--ipv6", action="store_const", dest="inet",
-    #     const="inet6", default="inet",
-    #                              help="inet: inet ")
 
     def run_test_once(self):
-        scope = self.config().get_item("scope", default="global")  # link
-        inet = self.config().get_item("inet", default="inet")  # inet6
-        cmd = ["ip", "-oneline", "addr"]
-        self.logger.info(cmd)
-        r = Runner(cmd, userat=self.userat)
-        ret = r.ret
-        self.logger.info(ret)
-        r2=Runner("ip r", userat=self.userat)
-        if r2.success:
-            route=r2.so_lines[0]
-            for line in r2.so_lines:
-                self.log_test_status(Status.OK,line)
-        else:
-            route=" no route"
-        if ret != 0:
-            self.log_test_status(Status.UNKNOWN, message=f"Command Error 0x{ret:04x}")
-        else:
-            lines = r.so_lines
-
-            for line in lines:
-                if "deprecated" in line:
-                    continue
-                if re.match("1:\\slo\\s", line):
-                    continue
-
-                if not re.search(r"\s" + inet + r"\s", line):
-                    continue
-                if not re.search("scope\\s" + scope + "\\s", line):
-                    continue
-                parts = line.split()
-                self.log_test_status(Status.OK, message=f"{parts[3]:<20} {route}")
-                break
-            else:
-                self.log_test_status(Status.NODATA, message=f'no match for {inet}')
 
+        community = self.config().get_item("community", secrets=True)
+
+        cmd0 = ["snmpwalk", "-c", community, "-v2c", self.fqdn, "-Ovq", ]
+        oids = ["iso.3.6.1.2.1.47.1.1.1.1.2",
+                "iso.3.6.1.2.1.47.1.1.1.1.10", "iso.3.6.1.2.1.47.1.1.1.1.11",
+                "iso.3.6.1.2.1.47.1.1.1.1.13", "iso.3.6.1.2.1.1.5.0"]
+
+        out2 = ""
+        for oid in oids:
+            cmd = cmd0.copy()
+            cmd.append(oid)
+            r = Runner(cmd, silent=True)
+            ret = r.ret
+            self.logger.info(ret)
+            if ret != 0:
+                self.log_test_status(Status.NODATA, message=f"{oid=} Command Error 0x{ret:04x}")
+            else:
+                lines = r.so_lines
+                for line in lines:
+                    sline = line.strip('"\n')
+                    self.log_test_status(Status.OK, sline)
+                    n = len(sline)
+                    if (n < 4) or (n > 30) or (sline.startswith("Slot")) or sline.startswith(
+                            "Broadcom") or sline.startswith("Stack") or sline.startswith("switch processor"):
+                        continue
+                    self.logger.info(sline)
+                    out2 = out2 + sline + " "
+        self.log_test_status(Status.OK, message=out2)
+
+
+from Santa_IW.TestPluginHelper import TestPluginHelper
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
+
+
+class SNMPDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if not self.can_snmp:
+            return
+        self.add_test(
+            {
+                "test_type": "SNMP_id",
+                "community": "{{__SNMP_COMMUNITY__}}",
+            })
 
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
 
-helper: DiscoveryHelper = DiscoveryHelper(IPVx_Address)
-helper.alias("IPV4_Address", {"scope": "global", "inet": "inet","period":5*TestBase.sc.minute})
-helper.alias("IPV6_Address", {"scope": "global", "inet": "inet6","period":5*TestBase.sc.minute})
+helper: TestPluginHelper = TestPluginHelper(SNMP_id, SNMPDiscovery)
+helper.alias("SNMP_id", {"period": 15 * TestBase.sc.minute, "community": "public"})
```

### Comparing `santa_iw-0.7.4/Santa_IW/TEST_MODULES/PendingUpdates.py` & `santa_iw-0.9.0/Santa_IW/TEST_MODULES/PendingUpdates.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env  python3
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from libsrg.Runner import Runner
 
 from Santa_IW.TestBase import Status, TestBase
 
 
 class PendingUpdates(TestBase):
 
@@ -75,11 +79,23 @@
                     self.log_test_status(Status.CRITICAL, message=f'({kernel_count}K/{package_count}P) {last}')
                 elif kernel_count >= warn_threshold:
                     self.log_test_status(Status.WARNING, message=f'({kernel_count}K/{package_count}P) {last}')
                 else:
                     self.log_test_status(Status.OK, message=f'({kernel_count}K/{package_count}P) {last}')
 
 
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
+from Santa_IW.TestPluginHelper import TestPluginHelper
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
+
+
+class LocalDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if self.can_ssh and self.kernel_name == "Linux":
+            self.add_test(
+                {
+                    "test_type": "PendingUpdates"
+                })
+
 
-helper: DiscoveryHelper = DiscoveryHelper(PendingUpdates)
-helper.alias("PendingUpdates", {"warn_threshold": 10, "crit_threshold": 20,"period":2*TestBase.sc.hour})
+helper: TestPluginHelper = TestPluginHelper(PendingUpdates, LocalDiscovery)
+helper.alias("PendingUpdates", {"warn_threshold": 10, "crit_threshold": 20, "period": 2 * TestBase.sc.hour})
```

### Comparing `santa_iw-0.7.4/Santa_IW/TEST_MODULES/PingTest.py` & `santa_iw-0.9.0/Santa_IW/TEST_MODULES/PingTest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import os
 from math import nan, isnan
 
 from libsrg.Config import Config
 from libsrg.Runner import Runner
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
 from libsrg.Statistics.AnalogStatsSlidingWindow import AnalogStatsSlidingWindow
@@ -43,15 +47,15 @@
         # Note: rate is limited to 5 hz (200ms) as a normal user
         cmd = (f"ping -q -c {ping_max_count} -w {ping_max_duration} " +
                f"-W {ping_timeout} -i {ping_interval} {self.fqdn}")
         if burst:
             cmd += "-A"
         r = Runner(cmd)
         self.logger.info(f"{self} perform_test {r}")
-        self.log_test_status(Status.NODATA,f"{r.ret=} {cmd!r}")
+        self.log_test_status(Status.NODATA, f"{r.ret=} {cmd!r}")
         # 0= some returns, 1= no returns, 2= bad address,255 ssh error
         if r.ret >= 2:
             self.log_test_status(Status.UNKNOWN, message=str(r))
         xmit = 0
         rcvd = 0
         delta = nan
         sd = 0.
@@ -84,41 +88,63 @@
             loss_percent = (xmit - rcvd) * 100. / xmit
             self.loss_percentage_stats_short_term.sample(loss_percent)
             self.loss_percentage_stats_long_term.sample(loss_percent)
         else:
             loss_percent = 100
 
         if loss_percent >= ping_loss_critical_threshold_percent:
-            self.log_test_status(Status.CRITICAL, tag="current run")
+            self.log_test_status(Status.CRITICAL, tag=f"current run loss_percent {loss_percent} >= {ping_loss_critical_threshold_percent}")
         elif loss_percent >= ping_loss_warning_threshold_percent:
-            self.log_test_status(Status.WARNING, tag="current run")
+            self.log_test_status(Status.WARNING, tag=f"current run loss_percent {loss_percent} >= {ping_loss_warning_threshold_percent}")
         else:
-            self.log_test_status(Status.OK, tag="current run")
+            self.log_test_status(Status.OK, tag=f"current run loss_percent {loss_percent} < {ping_loss_warning_threshold_percent}")
 
         # only threshold statistics after sufficient count
         if self.loss_percentage_stats_short_term.count() >= self.loss_percentage_stats_short_term.window:
             mean_loss = self.loss_percentage_stats_short_term.mean()
             if mean_loss >= ping_loss_stat_critical_threshold_percent:
-                self.log_test_status(Status.CRITICAL, tag="mean_loss")
+                self.log_test_status(Status.CRITICAL, tag=f"mean_loss {mean_loss} >= {ping_loss_stat_critical_threshold_percent}")
             elif mean_loss >= ping_loss_stat_warning_threshold_percent:
-                self.log_test_status(Status.WARNING, tag="mean_loss")
+                self.log_test_status(Status.WARNING, tag=f"mean_loss {mean_loss} >= {ping_loss_stat_warning_threshold_percent}")
             else:
-                self.log_test_status(Status.OK, tag="mean_loss")
+                self.log_test_status(Status.OK, tag=f"mean_loss {mean_loss} < {ping_loss_stat_warning_threshold_percent}")
         else:
-            self.log_test_status(Status.NODATA, "mean_loss has insufficient history")
+            self.log_test_status(Status.NODATA, f"mean_loss still building history, count {self.loss_percentage_stats_short_term.count()} < {self.loss_percentage_stats_short_term.window}")
 
         msg = (f"Ping {delta:>8.2f}({self.reply_time_stats.mean():>8.2f}) ms, sd={sd:>8.3f} " +
                f"{rcvd=:4n} of {xmit=:4n} loss " +
                f"{loss_percent: 6.2f}%({self.loss_percentage_stats_short_term.mean(): 6.2f}%)")
         self.set_annotation(msg)
 
 
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
+from Santa_IW.TestPluginHelper import TestPluginHelper
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
+
+
+class PingDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if self.can_ping and not self.can_ssh:
+            self.add_test(
+                {
+                    "test_type": "PingTest_D"
+                })
+        else:
+            if self.kernel_name=="Linux":
+                self.add_test(
+                    {
+                        "test_type": "PingTest_B"
+                    })
+            else:
+                self.add_test(
+                    {
+                        "test_type": "PingTest_C"
+                    })
 
-helper = DiscoveryHelper(PingTest)
+helper = TestPluginHelper(PingTest,PingDiscovery)
 base_config = helper.alias("PingTest_A",
                            burst=False,
                            ping_loss_critical_threshold_percent=10,
                            ping_loss_warning_threshold_percent=5,
                            ping_loss_stat_critical_threshold_percent=5,
                            ping_loss_stat_warning_threshold_percent=1,
                            ping_interval=0.0,
@@ -126,19 +152,20 @@
                            ping_max_count=1000,
                            ping_timeout=1,
                            period=1 * TestBase.sc.minute
                            )
 
 med = helper.alias("PingTest_B", base_config,
                    ping_interval=0.2,
+                   ping_max_count=100,
                    ping_loss_stat_critical_threshold_percent=8,
                    ping_loss_stat_warning_threshold_percent=4,
                    ping_loss_critical_threshold_percent=60,
                    ping_loss_warning_threshold_percent=50,
-                   period=2 * TestBase.sc.minute
+                   period=1 * TestBase.sc.minute
 
                    )
 
 slow = helper.alias("PingTest_C", med,
                     ping_interval=0.5,
                     ping_max_duration=10,
                     ping_max_count=10,
```

### Comparing `santa_iw-0.7.4/Santa_IW/TEST_MODULES/RemoteProcess.py` & `santa_iw-0.9.0/Santa_IW/TEST_MODULES/RemoteProcess.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 #!/usr/bin/env  python3
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 from libsrg.Runner import Runner
 
 from Santa_IW.TestBase import Status, TestBase
 
 
 class RemoteProcess(TestBase):
@@ -11,15 +14,14 @@
     #     self.parser.add_argument("-p", "--proc", action="store", dest="remote_proc",
     #                              default="Mail.app/Contents/MacOS/Mail", help="name of process")
 
     def run_test_once(self):
         process_name = self.config().get_item("process_name")
         process_user = self.config().get_item("process_user")
         cmd = ["ps", "-fu", process_user]
-        self.logger.info(cmd)
         r = Runner(cmd, userat=self.userat)
         ret = r.ret
         self.logger.info(ret)
         if ret != 0:
             self.logger.warning(r)
             self.log_test_status(Status.UNKNOWN, message=f"Command Error 0x{ret:04x}")
         else:
@@ -29,12 +31,43 @@
                     self.log_test_status(Status.OK, message=line)
                     break
             else:  # no break
                 self.log_test_status(Status.WARNING,
                                      message=f"Process {process_name} for user {process_user} not found")
 
 
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
+from Santa_IW.TestPluginHelper import TestPluginHelper
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
 
-helper: DiscoveryHelper = DiscoveryHelper(RemoteProcess)
+
+# noinspection HttpUrlsUsage
+class LocalDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if not self.can_ssh:
+            return
+        # I don't see any generic discovery mechanism for this test
+        # this one imac happens to run my email triage rules
+        if self.fqdn in ["imac.home.goncalo.name"]:
+            self.add_test(
+                {
+                    "test_type": "RemoteProcess",
+                    "process_name": "MacOS/Mail",
+                    "process_user": "steve",
+                    "period": 5 * TestBase.sc.minute
+                })
+        cmd = ["ps", "-fu", "root"]
+        r = Runner(cmd, userat=self.userat)
+        if r.success and "/sbin/zed" in r.so_str:
+            self.add_test(
+                {
+                    "test_type": "RemoteProcess",
+                    "process_name": "/sbin/zed",
+                    "process_user": "root",
+                    "period": 5 * TestBase.sc.minute
+                })
+
+
+
+helper: TestPluginHelper = TestPluginHelper(RemoteProcess, LocalDiscovery)
 helper.alias("RemoteProcess",
              {"process_name": "/sbin/zed", "process_user": "root", "period": 5 * TestBase.sc.minute})
```

### Comparing `santa_iw-0.7.4/Santa_IW/TEST_MODULES/Sensors.py` & `santa_iw-0.9.0/Santa_IW/TEST_MODULES/Sensors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 #!/usr/bin/env  python3
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 import json
 from typing import Any, Optional, Tuple
 
 from libsrg.Config import Config
 from libsrg.Runner import Runner
 from libsrg.Statistics.ADStatsBase import ADStatsBase
@@ -215,11 +218,25 @@
     @staticmethod
     def repack_block(block: dict[str, Any]) -> Tuple[dict[str, Any], str]:
         names = list(block.keys())
         prefix = names[0].split("_")[0].strip("0123456789")
         repacked = {key.split("_", maxsplit=1)[-1]: val for key, val in block.items()}
         return repacked, prefix
 
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
+from Santa_IW.TestPluginHelper import TestPluginHelper
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
 
-helper = DiscoveryHelper(Sensors)
+
+class LocalDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if self.can_ssh:
+            r = Runner("sensors -j", userat=self.userat, timeout=5)
+            if r.success:
+                self.add_test(
+                    {
+                        "test_type": "Sensors"
+                    })
+
+
+helper = TestPluginHelper(Sensors, LocalDiscovery)
 helper.alias("Sensors", {"period": 4 * TestBase.sc.minute})
```

### Comparing `santa_iw-0.7.4/Santa_IW/TEST_MODULES/SystemctlFailed.py` & `santa_iw-0.9.0/Santa_IW/TEST_MODULES/SystemctlFailed.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 #!/usr/bin/env  python3
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from libsrg.Config import Config
 from libsrg.ElapsedTime import ElapsedTime
 from libsrg.Runner import Runner
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
 from libsrg.Statistics.DiscreteStatsCumulative import DiscreteStatsCumulative
 
 from Santa_IW.Subassembly import Subassembly
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
 from Santa_IW.TestBase import Status, TestBase
+from Santa_IW.TestPluginHelper import TestPluginHelper
 
 
 class SystemctlFailed(TestBase):
     def __init__(self, instance_config: Config, short_name: str, parent: Subassembly, stepparent: Subassembly):
         super().__init__(instance_config=instance_config, parent=parent, stepparent=stepparent,
                          short_name=short_name)  # super defines self.logger
         self.filtered_count = AnalogStatsFading(self.prefix_name("filtered_count"))
@@ -93,15 +97,28 @@
                         self.restarted_process_count.sample(proc)
                         r = Runner(f"systemctl restart {proc}", userat=self.userat)
                         self.log_test_status(Status.MAINT, str(r))
                 else:
                     self.log_test_status(Status.MAINT, f"Too soon to restart {str(restart_set)}")
 
 
-helper = DiscoveryHelper(SystemctlFailed)
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
+
+
+class SystemctlFailedDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if self.can_ssh and self.kernel_name == "Linux":
+            self.add_test(
+                {
+                    "test_type": "SystemctlFailed"
+                })
+
+
+helper = TestPluginHelper(SystemctlFailed, SystemctlFailedDiscovery)
 
 helper.alias("SystemctlFailed",
              period=2 * TestBase.sc.minute,
              warning_cnt=1,
              critical_cnt=2,
              dont_restart_list=[
                  "plymouth-start.service",
@@ -118,9 +135,9 @@
                  "bthelper@hci0.service",
                  "plymouth-start.service",
                  "serial-getty@ttyAMA0.service",
                  "insights-client.service",
                  # "dkms.service"
              ],
              min_restart_period=15 * TestBase.sc.minute,
-             restart_enable=True
+             restart_enable=False
              )
```

### Comparing `santa_iw-0.7.4/Santa_IW/TEST_MODULES/TimeMachine.py` & `santa_iw-0.9.0/Santa_IW/TEST_MODULES/TimeMachine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env  python3
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import plistlib
 from datetime import datetime
 from pathlib import Path
 
 from libsrg.Config import Config
 from libsrg.Runner import Runner
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
@@ -79,13 +83,38 @@
             self.log_test_status(Status.CRITICAL, message=msg)
         elif age_days > warn_t:
             self.log_test_status(Status.WARNING, message=msg)
         else:
             self.log_test_status(Status.OK, message=msg)
 
 
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
+from Santa_IW.TestPluginHelper import TestPluginHelper
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
+
+
+# noinspection HttpUrlsUsage
+class LocalDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if not self.can_ssh:
+            return
+        r = Runner("zfs list -H -o mountpoint", userat=self.userat, timeout=10)
+        if not r.success:
+            return
+        for line in r.so_lines:
+            r2 = Runner(f"ls {line}/*bundle/com.apple.TimeMachine.MachineID.plist", userat=self.userat,
+                        timeout=10)
+            pth = Path(line)
+            nam = Path(pth.name).name
+            if r2.success:
+                cmd = {
+                    "test_type": "TimeMachine",
+                    "path": line,
+                    "instance_name": nam
+                }
+                self.add_test(cmd)
+
 
-helper: DiscoveryHelper = DiscoveryHelper(TimeMachine)
+helper: TestPluginHelper = TestPluginHelper(TimeMachine, LocalDiscovery)
 # no default for path
 helper.alias("TimeMachine", {"warning_threshold_days": 14, "critical_threshold_days": 21},
              period=30 * TestBase.sc.minute)
```

### Comparing `santa_iw-0.7.4/Santa_IW/TEST_MODULES/Uname.py` & `santa_iw-0.9.0/Santa_IW/TEST_MODULES/Uname.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env  python3
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from libsrg.Config import Config
 from libsrg.ElapsedTime import ElapsedTime
 from libsrg.Info import Info
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
 
 from Santa_IW.Subassembly import Subassembly
 from Santa_IW.TestBase import Status, TestBase
@@ -17,22 +21,37 @@
 
     def run_test_once(self):
         fqdn = self.config().get_item("fqdn")
         timer = ElapsedTime()
         try:
             with timer:
                 info = Info(fqdn, retries=2, timeout=10)
+                con=info.to_config()
+                for item,value in con.items():
+                    self.log_test_status(Status.OK,f"{item:<24} = {value}")
         except Exception as ex:
             self.logger.exception(ex, stack_info=True, exc_info=True)
             self.log_test_status(Status.UNKNOWN, message="Command Error fetching node info")
             return
         self.reply_stats.sample(timer.elapsed())
         how = info.uefi
         ker = info.kernel
         locked = info.kernel_dnf
         self.log_test_status(Status.OK, message=f"{how} {ker} {locked}")
 
 
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
+from Santa_IW.TestPluginHelper import TestPluginHelper
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
+
+
+class UnameDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if self.can_ssh:
+            self.add_test(
+                {
+                    "test_type": "Uname"
+                })
+
 
-helper = DiscoveryHelper(Uname)
+helper = TestPluginHelper(Uname, UnameDiscovery)
 helper.alias("Uname", period=1 * TestBase.sc.hour)
```

### Comparing `santa_iw-0.7.4/Santa_IW/TEST_MODULES/Zpool_Free.py` & `santa_iw-0.9.0/Santa_IW/TEST_MODULES/Zpool_Free.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env  python3
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 from libsrg.Config import Config
 from libsrg.Runner import Runner
 from libsrg.Statistics.AnalogStatsFading import AnalogStatsFading
 
 from Santa_IW.Subassembly import Subassembly
 from Santa_IW.TestBase import Status, TestBase
 
@@ -48,11 +52,33 @@
                     self.log_test_status(Status.CRITICAL, message=f"Used {used}% {pool}")
                 elif used > warn_t:
                     self.log_test_status(Status.WARNING, message=f"Used {used}% {pool}")
                 else:
                     self.log_test_status(Status.OK, message=f"Used {used}% {pool}")
 
 
-from Santa_IW.DiscoveryHelper import DiscoveryHelper
+from Santa_IW.TestPluginHelper import TestPluginHelper
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
+
+
+# noinspection HttpUrlsUsage
+class LocalDiscovery(TestDiscoveryBase):
+
+    def discover(self):
+        if not self.can_ssh:
+            return
+        r = Runner("zpool list -H -o name", userat=self.userat, timeout=10)
+        if not r.success:
+            return
+
+        for pool_name in r.so_lines:
+            cmd = {
+                "test_type": "Zpool_Status",
+                "instance_name": pool_name,
+                "period": 300,
+                "pool": pool_name
+            }
+            self.add_test(cmd)
+
 
-helper = DiscoveryHelper(Zpool_Free)
+helper = TestPluginHelper(Zpool_Free,LocalDiscovery)
 helper.alias("Zpool_Free", period=15 * TestBase.sc.minute)
```

### Comparing `santa_iw-0.7.4/Santa_IW/TemplateFactory.py` & `santa_iw-0.9.0/Santa_IW/TemplateFactory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import json
 from pathlib import Path
 from typing import Any
 
 from libsrg.Config import Config
 
 from Santa_IW.Status import Status
```

### Comparing `santa_iw-0.7.4/Santa_IW/TestBase.py` & `santa_iw-0.9.0/Santa_IW/TestBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import math
 import random
 from abc import ABC, abstractmethod
 from threading import Event, Thread, Timer
 from time import sleep
 from typing import Optional
```

### Comparing `santa_iw-0.7.4/Santa_IW/TestFactory.py` & `santa_iw-0.9.0/Santa_IW/TestFactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import importlib
 import importlib.util
 import sys
 from collections import Counter
 from pathlib import Path
 from typing import List, Type, Any
 
 from libsrg.Config import Config
 
 from Santa_IW.Node import Node
 from Santa_IW.Status import Status
 from Santa_IW.Subassembly import Subassembly
 from Santa_IW.TestBase import TestBase
+from Santa_IW.TestDiscoveryBase import TestDiscoveryBase
 from Santa_IW.TestType import TestType
 
 
 # noinspection DuplicatedCode
 class TestFactory(Subassembly):
 
     def __init__(self, instance_config: Config, short_name: str, parent: Subassembly):
@@ -23,14 +28,15 @@
         self.test_class_map: dict[str, Any] = {}
         self.test_type_map: dict[str, TestType] = {}
         self.test_instance_map: dict[str, TestBase] = {}
         self.tests_names_not_found: set[str] = set()
         # failure within a test type does not imply factory failure
         self._propagate_child_stats_in_overall = False
         self.test_used_by: dict[str, set[str]] = {}
+        self.classifiers: list[Type[TestDiscoveryBase]]=[]
 
     def start(self) -> None:
         self.set_annotation("Loading Test Classes...")
         self.log_internal_status(Status.OK, "Started", assess=True)
         test_dirs = self.config().get_item("test_modules_dirs")
         for test_dir in test_dirs:
             dpath = Path(test_dir).resolve()
@@ -48,15 +54,15 @@
                         self.load_testfile(testfile)
                     except Exception as e:
                         self.logger.exception(e, stack_info=True, exc_info=True)
                         self.log_internal_status(Status.CRITICAL, f"Failed to load test file {testfile} {e}",
                                                  assess=True)
 
         self.set_annotation("Done")
-        self.log_internal_status(Status.OK, message=f"Loaded {len(self.test_type_map)} test types and {len(self.test_instance_map)} test instances", assess=True)
+        self.log_internal_status(Status.OK, message=f"Loaded {len(self.test_type_map)} test types and {len(self.classifiers)} test classifiers", assess=True)
         self.logger.info("Finished")
 
     def spawn(self):
         # no new thread, but update status
         self.log_internal_status(Status.OK, message=f"Loaded {len(self.test_class_map)} Test Classes, {len(self.test_type_map)} Test Types, and {len(self.test_instance_map)} Test Instances", assess=True)
 
 
@@ -68,14 +74,17 @@
         module = importlib.util.module_from_spec(spec)
         sys.modules[module_name] = module
         spec.loader.exec_module(module)
 
         helper = module.helper
         test_class = helper.get_loaded_class()
         all_configs = helper.get_all_configs()
+        discovery_class = helper.get_discovery_class()
+        if discovery_class:
+            self.classifiers.append(discovery_class)
         self.logger.info(f"{file_path} supports DiscoveryHelper")
         self.test_class_map[module_name]= file_path
         test_types = self.config().get_item("test_types")
         for alias, config in all_configs.items():
             test_type: TestType = TestType(instance_config=config, parent=test_types, short_name=alias,
                                            test_class=test_class)
             self.test_used_by[alias] = set()
@@ -171,7 +180,10 @@
                     if not short.endswith(test_sep):
                         short += "_"
                     short += f"{n:02d}"
                 self.create_one_test(node=node, test_args=test_info, short=short)
         if self.tests_names_not_found:
             msg = f"{len(self.tests_names_not_found)} Test Classes not found "
             self.log_internal_status(Status.WARNING, msg)
+
+    def get_test_discovery_classes(self)-> list[Type[TestDiscoveryBase]]:
+        return self.classifiers
```

### Comparing `santa_iw-0.7.4/Santa_IW/TreeRoot.py` & `santa_iw-0.9.0/Santa_IW/TreeRoot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,44 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import os
 from threading import Thread
 
 from libsrg.Config import Config
 
 from Santa_IW.DataRecording import DataRecording
 from Santa_IW.Discovery import Discovery
 from Santa_IW.Flask.WebGUI import WebGUI
 from Santa_IW.Naughty import Naughty
 from Santa_IW.Node import Node
 from Santa_IW.NodeFactory import NodeFactory
+from Santa_IW.NorthPole import NorthPole
 from Santa_IW.PluginFactory import PluginFactory
 from Santa_IW.Status import Status
 from Santa_IW.Subassembly import Subassembly
 from Santa_IW.TemplateFactory import TemplateFactory
 from Santa_IW.TestFactory import TestFactory
 
 
 class TreeRoot(Subassembly):
     """
     TreeRoot class is the top level class that instantiates all classes beyond the basic command line parser.
 
     TreeRoot was previously named Monitor.
     """
 
-    def __init__(self, cli_args: Config):
+    def __init__(self, cli_args: Config,north_pole:NorthPole):
         self._my_thread = None
         tree_root_name = cli_args.get('tree_root_name')
 
         super().__init__(parent=None, short_name=tree_root_name,
                          instance_config=cli_args)  # super defines self.logger
-
+        self.north_pole = north_pole
         tree_app_name = cli_args.get('tree_app_name')
         sw_args0: Config = Config({})
         sw_args: Config = Config({"propagate_child_status_in_overall": False})
         self.sw_subsystems = Node(instance_config=sw_args0, short_name=tree_app_name, parent=self, sw_node=True)
 
         self.data_recording = DataRecording(parent=self.sw_subsystems, short_name="DataRecording",
                                             instance_config=sw_args)
@@ -59,16 +64,20 @@
         self.sw_subsystems.config().set_item("template_factory", self.template_factory)
         self.sw_subsystems.config().set_item("data_recording", self.data_recording)
         self.sw_subsystems.config().set_item("naughty", self.naughty)
         self.sw_subsystems.config().set_item("test_types", self.test_types)
         self.sw_subsystems.config().set_item("plugin_factory", self.test_factory)
         self.sw_subsystems.config().set_item("discovery", self.discovery)
 
-        secrets_file = self.config().get_item("secrets_file")
-        Config.set_secrets(secrets_file, dict(os.environ))
+        secrets_dir= self.north_pole.santa_secrets_dir
+        json_secrets= [ f for f in secrets_dir.glob("*.json")]
+        env_secrets= [ f for f in secrets_dir.glob("*.env")]
+        self.log_internal_status(Status.OK,f"Loading secrets from {json_secrets}, {env_secrets} and environment")
+        # secrets_file = self.config().get_item("secrets_file")
+        Config.set_secrets(*json_secrets,*env_secrets, dict(os.environ))
 
     def start(self) -> None:
         self.mark_subsystem_enabled()
         self.log_internal_status(Status.OK, "Creating new thread for treeroot")
         if self._my_thread is None:
             self._my_thread = Thread(target=self._run_in_thread, daemon=True, name=self.name())
             self._my_thread.start()
@@ -93,14 +102,17 @@
 
         self.set_annotation("Loading Templates...")
         self.template_factory.start()
 
         self.set_annotation("Loading Nodes...")
         self.node_factory.start()
 
+        self.set_annotation("TestTypes...")
+        self.test_types.start()
+
         self.set_annotation("Naughty List...")
         self.naughty.start()
 
         self.set_annotation("Spawning tests...")
         self.spawn()
         self.set_annotation("Running tests...")
```

### Comparing `santa_iw-0.7.4/Santa_IW/UnitTests/DBConnection_test.py` & `santa_iw-0.9.0/Santa_IW/UnitTests/DBConnection_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import math
 import os
 import unittest
 from pathlib import Path
 
 from Santa_IW.DBConnection import DBConnection
```

### Comparing `santa_iw-0.7.4/Santa_IW/UnitTests/Subassembly_test.py` & `santa_iw-0.9.0/Santa_IW/UnitTests/Subassembly_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import unittest
 
 from libsrg.Config import Config
 
 from Santa_IW.Status import Status
 from Santa_IW.Subassembly import Subassembly
```

### Comparing `santa_iw-0.7.4/Santa_IW/Utils.py` & `santa_iw-0.9.0/Santa_IW/Utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Santa Is Watching aka Santa_IW (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import argparse
 import functools
 import json
 import logging
 from collections import ChainMap
 from pathlib import Path
 from typing import Any, Callable, Optional
```

### Comparing `santa_iw-0.7.4/pyproject.toml` & `santa_iw-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Santa_IW"
-version = "0.7.4"
+version = "0.9.0"
 description = "Santa Is Watching: ZFS Aware Network Monitor"
 authors = ["Steve Goncalo <steven@goncalo.us>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
@@ -17,15 +17,15 @@
 ]
 packages= [{include='Santa_IW'}]
 # package-mode = false
 
 [tool.poetry.dependencies]
 python = "^3.11"
 jinja2 = ">=3.1.3,<3.2.0"
-libsrg = ">=5.1.1"
+libsrg = ">=5.2.3"
 sphinx = {version = "^7.3.7", optional = true, extras = ["doc"]}
 sphinx-rtd-theme = {version = "^2.0.0", optional = true, extras = ["doc"]}
 sphinxcontrib-napoleon = {version = "^0.7", optional = true, extras = ["doc"]}
 nltk = ">=3.8.1,<3.9.0"
 flask = ">=3.0.2,<3.1.0"
 requests = ">=2.31.0,<2.32.0"
 aiohue = "^4.7.1"
@@ -34,23 +34,25 @@
 numpy = "^1.26.4"
 sympy = "^1.12"
 pandas = "^2.2.2"
 sqlalchemy = "^2.0.29"
 pathvalidate = "^3.2.0"
 
 
+
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
+Wiki = "https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home"
 Homepage = "https://gitlab.com/SRG_gitlab/santa-is-watching"
 Issues = "https://gitlab.com/SRG_gitlab/santa-is-watching/-/issues"
 API = "https://srg_gitlab.gitlab.io/santa-is-watching/index.html"
-Wiki = "https://gitlab.com/SRG_gitlab/santa-is-watching/-/wikis/home"
 
 [tool.poetry.extras]
 doc = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon"]
 
 [tool.poetry.scripts]
 Santa_IW_service_run = "Santa_IW.Main:main"
 SantaSetup = "SantaSetup:main"
```

