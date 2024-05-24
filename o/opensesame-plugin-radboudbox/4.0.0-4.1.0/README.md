# Comparing `tmp/opensesame_plugin_radboudbox-4.0.0.tar.gz` & `tmp/opensesame_plugin_radboudbox-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensesame_plugin_radboudbox-4.0.0.tar", max compression
+gzip compressed data, was "opensesame_plugin_radboudbox-4.1.0.tar", max compression
```

## Comparing `opensesame_plugin_radboudbox-4.0.0.tar` & `opensesame_plugin_radboudbox-4.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      349 2017-11-24 23:59:08.716781 opensesame_plugin_radboudbox-4.0.0/LICENSE.md
--rw-r--r--   0        0        0     3091 2022-11-25 14:29:09.777299 opensesame_plugin_radboudbox-4.0.0/README.md
--rw-r--r--   0        0        0      133 2023-08-15 21:37:15.068050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/__init__.py
--rw-r--r--   0        0        0     1619 2024-05-22 22:21:36.766788 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/__init__.py
--rw-r--r--   0        0        0     1665 2023-08-15 21:37:15.068050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.md
--rw-r--r--   0        0        0      762 2023-08-15 21:37:15.068050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.png
--rw-r--r--   0        0        0     4882 2023-12-04 08:47:37.911319 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.py
--rw-r--r--   0        0        0     1716 2023-08-15 21:37:15.068050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start_large.png
--rw-r--r--   0        0        0      503 2024-05-22 22:21:36.767788 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/__init__.py
--rw-r--r--   0        0        0     1236 2023-08-15 21:37:15.069050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.md
--rw-r--r--   0        0        0      755 2023-08-15 21:37:15.069050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.png
--rw-r--r--   0        0        0     2720 2023-12-04 08:47:27.403145 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.py
--rw-r--r--   0        0        0     1687 2023-08-15 21:37:15.069050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait_large.png
--rw-r--r--   0        0        0     1381 2024-05-22 22:21:36.767788 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_init/__init__.py
--rw-r--r--   0        0        0     1935 2023-08-15 21:37:15.069050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.md
--rw-r--r--   0        0        0      705 2023-08-15 21:37:15.070050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.png
--rw-r--r--   0        0        0     4393 2024-05-21 23:52:30.596367 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.py
--rw-r--r--   0        0        0     1709 2023-08-15 21:37:15.070050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init_large.png
--rw-r--r--   0        0        0     1314 2024-05-22 22:21:36.767788 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_control/__init__.py
--rw-r--r--   0        0        0     1299 2023-08-15 21:37:15.070050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.md
--rw-r--r--   0        0        0      719 2023-08-15 21:37:15.070050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.png
--rw-r--r--   0        0        0     5076 2024-05-21 23:54:53.373750 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.py
--rw-r--r--   0        0        0     1678 2023-08-15 21:37:15.071050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control_large.png
--rw-r--r--   0        0        0      979 2024-05-22 22:21:36.767788 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/__init__.py
--rw-r--r--   0        0        0     1630 2023-08-15 21:37:15.071050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.md
--rw-r--r--   0        0        0      725 2023-08-15 21:37:15.071050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.png
--rw-r--r--   0        0        0     2913 2024-05-21 23:51:14.908148 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.py
--rw-r--r--   0        0        0     1692 2023-08-15 21:37:15.071050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger_large.png
--rw-r--r--   0        0        0     1588 2024-05-22 22:21:36.767788 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/__init__.py
--rw-r--r--   0        0        0     1622 2023-08-15 21:37:15.072050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.md
--rw-r--r--   0        0        0      723 2023-08-15 21:37:15.072050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.png
--rw-r--r--   0        0        0     3741 2023-08-15 21:37:15.072050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.py
--rw-r--r--   0        0        0     1691 2023-08-15 21:37:15.072050 opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons_large.png
--rw-r--r--   0        0        0      681 2024-05-22 22:21:36.767788 opensesame_plugin_radboudbox-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     4338 1970-01-01 00:00:00.000000 opensesame_plugin_radboudbox-4.0.0/setup.py
--rw-r--r--   0        0        0     4239 1970-01-01 00:00:00.000000 opensesame_plugin_radboudbox-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0      349 2017-11-24 23:59:08.716781 opensesame_plugin_radboudbox-4.1.0/LICENSE.md
+-rw-r--r--   0        0        0     3091 2022-11-25 14:29:09.777299 opensesame_plugin_radboudbox-4.1.0/README.md
+-rw-r--r--   0        0        0      133 2023-08-15 21:37:15.068050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/__init__.py
+-rw-r--r--   0        0        0     1619 2024-05-24 08:14:16.624265 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/__init__.py
+-rw-r--r--   0        0        0     1665 2023-08-15 21:37:15.068050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.md
+-rw-r--r--   0        0        0      762 2023-08-15 21:37:15.068050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.png
+-rw-r--r--   0        0        0     4882 2023-12-04 08:47:37.911319 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.py
+-rw-r--r--   0        0        0     1716 2023-08-15 21:37:15.068050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start_large.png
+-rw-r--r--   0        0        0      503 2024-05-24 08:14:16.624265 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/__init__.py
+-rw-r--r--   0        0        0     1236 2023-08-15 21:37:15.069050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.md
+-rw-r--r--   0        0        0      755 2023-08-15 21:37:15.069050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.png
+-rw-r--r--   0        0        0     2720 2023-12-04 08:47:27.403145 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.py
+-rw-r--r--   0        0        0     1687 2023-08-15 21:37:15.069050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait_large.png
+-rw-r--r--   0        0        0     1381 2024-05-24 08:14:16.624265 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_init/__init__.py
+-rw-r--r--   0        0        0     1935 2023-08-15 21:37:15.069050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.md
+-rw-r--r--   0        0        0      705 2023-08-15 21:37:15.070050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.png
+-rw-r--r--   0        0        0     4393 2024-05-21 23:52:30.596367 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.py
+-rw-r--r--   0        0        0     1709 2023-08-15 21:37:15.070050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init_large.png
+-rw-r--r--   0        0        0     1314 2024-05-24 08:14:16.624265 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_control/__init__.py
+-rw-r--r--   0        0        0     1299 2023-08-15 21:37:15.070050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.md
+-rw-r--r--   0        0        0      719 2023-08-15 21:37:15.070050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.png
+-rw-r--r--   0        0        0     5076 2024-05-21 23:54:53.373750 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.py
+-rw-r--r--   0        0        0     1678 2023-08-15 21:37:15.071050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control_large.png
+-rw-r--r--   0        0        0      965 2024-05-24 08:14:16.624265 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/__init__.py
+-rw-r--r--   0        0        0     1630 2023-08-15 21:37:15.071050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.md
+-rw-r--r--   0        0        0      725 2023-08-15 21:37:15.071050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.png
+-rw-r--r--   0        0        0     3571 2024-05-24 08:12:21.065344 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.py
+-rw-r--r--   0        0        0     1692 2023-08-15 21:37:15.071050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger_large.png
+-rw-r--r--   0        0        0     1588 2024-05-24 08:14:16.624265 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/__init__.py
+-rw-r--r--   0        0        0     1622 2023-08-15 21:37:15.072050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.md
+-rw-r--r--   0        0        0      723 2023-08-15 21:37:15.072050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.png
+-rw-r--r--   0        0        0     3741 2023-08-15 21:37:15.072050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.py
+-rw-r--r--   0        0        0     1691 2023-08-15 21:37:15.072050 opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons_large.png
+-rw-r--r--   0        0        0      681 2024-05-24 08:14:16.624265 opensesame_plugin_radboudbox-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4338 1970-01-01 00:00:00.000000 opensesame_plugin_radboudbox-4.1.0/setup.py
+-rw-r--r--   0        0        0     4239 1970-01-01 00:00:00.000000 opensesame_plugin_radboudbox-4.1.0/PKG-INFO
```

### Comparing `opensesame_plugin_radboudbox-4.0.0/README.md` & `opensesame_plugin_radboudbox-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/__init__.py` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,10 +26,10 @@
         "type": "text",
         "label": "<b>IMPORTANT:</b> this is a multithreaded background item, it will immediately advance to the next item, it will NOT wait for the button press/release or till the timeout has ended."
     }, {
         "type": "text",
         "label": "<small><b>Note:</b> Radboudbox init item at the begin of the experiment is needed for initialization of the buttonbox</small>"
     }, {
         "type": "text",
-        "label": "<small>Radboud Buttonbox version 4.0.0</small>"
+        "label": "<small>Radboud Buttonbox version 4.1.0</small>"
     }
 ]
```

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.md` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.py` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start_large.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_start/radboudbox_get_buttons_start_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.md` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.py` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait_large.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_get_buttons_wait/radboudbox_get_buttons_wait_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_init/__init__.py` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_init/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,10 +35,10 @@
         "name": "checkbox_extended",
         "tooltip": "Buttonbox extended mode"
     }, {
         "type": "text",
         "label": "<small><b>Note:</b> Radboudbox init item at the begin of the experiment is needed for initialization of the buttonbox</small>"
     }, {
         "type": "text",
-        "label": "<small>Radboud Buttonbox version 4.0.0</small>"
+        "label": "<small>Radboud Buttonbox version 4.1.0</small>"
     }
 ]
```

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.md` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.py` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init_large.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_init/radboudbox_init_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_control/__init__.py` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_control/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,10 +36,10 @@
         "name": "line_edit_command_value",
         "tooltip": "Command Value"
     }, {
         "type": "text",
         "label": "<small><b>Note:</b> Radboudbox init item at the begin of the experiment is needed for initialization of the buttonbox</small>"
     }, {
         "type": "text",
-        "label": "<small>Radboud Buttonbox version 4.0.0</small>"
+        "label": "<small>Radboud Buttonbox version 4.1.0</small>"
     }
 ]
```

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.md` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.py` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control_large.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_control/radboudbox_send_control_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/__init__.py` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,26 +7,26 @@
     {
         "type": "line_edit",
         "var": "value",
         "label": "Value",
         "name": "line_edit_value",
         "tooltip": "Value"
     }, {
-    #     "type": "checkbox",
-    #     "var": "pulse_mode",
-    #     "label": "Enable Pulse Mode",
-    #     "name": "checkbox_pulse_mode",
-    #     "tooltip": "Pulse mode"
-    # }, {
-    #     "type": "line_edit",
-    #     "var": "pulse_time",
-    #     "label": "Pulse Time",
-    #     "name": "line_edit_pulse_time",
-    #     "tooltip": "Pulse Time"
-    # }, {
+        "type": "checkbox",
+        "var": "pulse_mode",
+        "label": "Enable Pulse Mode",
+        "name": "checkbox_pulse_mode",
+        "tooltip": "Pulse mode"
+    }, {
+        "type": "line_edit",
+        "var": "pulse_time",
+        "label": "Pulse Time (ms)",
+        "name": "line_edit_pulse_time",
+        "tooltip": "Pulse Time (ms)"
+    }, {
         "type": "text",
         "label": "<small><b>Note:</b> Radboudbox init item at the begin of the experiment is needed for initialization of the buttonbox</small>"
     }, {
         "type": "text",
-        "label": "<small>Radboud Buttonbox version 4.0.0</small>"
+        "label": "<small>Radboud Buttonbox version 4.1.0</small>"
     }
 ]
```

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.md` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.py` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 from libopensesame.oslogging import oslogger
 
 
 class RadboudboxSendTrigger(Item):
 
     def reset(self):
         self.var.value = 0
+        self.var.pulse_mode = 'no'
+        self.var.pulse_time = 50
 
     def prepare(self):
         super().prepare()
         self._check_init()
         self._init_var()
 
     def run(self):
@@ -40,27 +42,41 @@
             if self.var.value >= 0 and self.var.value <= 255:
                 self.value = int(self.var.value)
             else:
                 raise OSException('Trigger value should be between 0 and 255')
         else:
             raise OSException('Trigger value should be a integer')
 
+        if self.pulse_mode == 'yes':
+            if isinstance(self.var.pulse_time, int):
+                if self.var.pulse_time >= 0:
+                    self.pulse_time = int(self.var.pulse_time)
+                else:
+                    raise OSException('Trigger value should be equal to or larger than 0')
+            else:
+                raise OSException('Trigger value should be a integer')
+
         if self.dummy_mode == 'no':
             self.set_item_onset()
             self._show_message('Sending trigger value %s' % self.value)
             self.experiment.radboudbox.sendMarker(val=self.value)
+            if self.pulse_mode == 'yes':
+                self.clock.sleep(self.pulse_time)
+                self.experiment.radboudbox.sendMarker(val=0)
+
         elif self.dummy_mode == 'yes':
             self._show_message('Dummy mode enabled, NOT sending value %s' % self.value)
         else:
             self._show_message('Error with dummy mode')
 
     def _init_var(self):
         self.dummy_mode = self.experiment.radboudbox_dummy_mode
         self.verbose = self.experiment.radboudbox_verbose
         self.extended_mode = self.experiment.radboudbox_extended_mode
+        self.pulse_mode = self.var.pulse_mode
 
     def _check_init(self):
         if not hasattr(self.experiment, 'radboudbox_dummy_mode'):
             raise OSException('You should have one instance of `radboudbox_init` at the start of your experiment')
 
     def _show_message(self, message):
         oslogger.debug(message)
@@ -70,12 +86,12 @@
 
 class QtRadboudboxSendTrigger(RadboudboxSendTrigger, QtAutoPlugin):
 
     def __init__(self, name, experiment, script=None):
         RadboudboxSendTrigger.__init__(self, name, experiment, script)
         QtAutoPlugin.__init__(self, __file__)
 
-    # def init_edit_widget(self):
-    #     super().init_edit_widget()
-    #     self.line_edit_pulse_time.setEnabled(self.checkbox_pulse_mode.isChecked())
-    #     self.checkbox_pulse_mode.stateChanged.connect(
-    #         self.line_edit_pulse_time.setEnabled)
+    def init_edit_widget(self):
+        super().init_edit_widget()
+        self.line_edit_pulse_time.setEnabled(self.checkbox_pulse_mode.isChecked())
+        self.checkbox_pulse_mode.stateChanged.connect(
+            self.line_edit_pulse_time.setEnabled)
```

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger_large.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_send_trigger/radboudbox_send_trigger_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/__init__.py` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,10 +26,10 @@
         "type": "text",
         "label": "<b>IMPORTANT:</b> this is a foreground item, it will wait for the button press/release or till the timeout has ended before advancing to the next item."
     }, {
         "type": "text",
         "label": "<small><b>Note:</b> Radboudbox init item at the begin of the experiment is needed for initialization of the buttonbox</small>"
     }, {
         "type": "text",
-        "label": "<small>Radboud Buttonbox version 4.0.0</small>"
+        "label": "<small>Radboud Buttonbox version 4.1.0</small>"
     }
 ]
```

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.md` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.py` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons_large.png` & `opensesame_plugin_radboudbox-4.1.0/opensesame_plugins/radboudbox/radboudbox_wait_buttons/radboudbox_wait_buttons_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_radboudbox-4.0.0/pyproject.toml` & `opensesame_plugin_radboudbox-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opensesame-plugin-radboudbox"
-version = "4.0.0"
+version = "4.1.0"
 description = "An OpenSesame Plug-in for collecting button responses, audio detection, voice key and sending stimulus synchronization triggers with the Radboud Buttonbox to data acquisition systems"
 authors = ["Bob Rosbag <debian@bobrosbag.nl>"]
 readme = "README.md"
 packages = [
     {include = "opensesame_plugins"},
 ]
 license = "LICENSE.md"
```

### Comparing `opensesame_plugin_radboudbox-4.0.0/setup.py` & `opensesame_plugin_radboudbox-4.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {'': ['*']}
 
 install_requires = \
 ['rusocsci']
 
 setup_kwargs = {
     'name': 'opensesame-plugin-radboudbox',
-    'version': '4.0.0',
+    'version': '4.1.0',
     'description': 'An OpenSesame Plug-in for collecting button responses, audio detection, voice key and sending stimulus synchronization triggers with the Radboud Buttonbox to data acquisition systems',
     'long_description': "OpenSesame Plug-in: Radboud Buttonbox\n==========\n\n*An OpenSesame plug-in for collecting button responses, audio detection, voice key and sending stimulus synchronization triggers with the Radboud Buttonbox to data acquisition systems.*  \n\nCopyright, 2022, Bob Rosbag\n\nThis plugin makes use of the RuSocSci python package developed by Wilbert van der Ham. Radboud Buttonbox is developed by Pascal de Water. Exact references will follow in the future. \n  \n  \n## 1. About\n--------\n\nThe Technical Support Group (Radboud University, Social Sciences) developed an USB Arduino based Buttonbox which can be used for time accurate(1ms) button press, voice key, sound key registration and sending parallel port like triggers.\nUpper case A, B, C, D, E, F are used for key presses, and lower case a, b, c, d, e, f are used for key releases. Uppercase S is used for sound key detection and uppercase V for voice key.  \n\nFor more information:\n\n<http://tsgdoc.socsci.ru.nl/index.php?title=ButtonBoxes>\n\n\nThis plug-in consist of foreground and background (multithreaded) items.\n\n\nDifference between foreground and background:\n\n- **Foreground** item starts button/signal registration until it detects an allowed button or the set duration has passed. \n- **Background** item consist of a 'start' and 'wait' item. These are fully multi-threaded. After the start of the button/signal registration, the item will immediately advance to the next item. When the experiment reaches the 'wait' item, it will wait until a button/signal has been detected by the 'start' item or the duration has passed.\n\n\nThis plug-in has six items:\n\n- **Init** initialization of the buttonbox, this should be placed at the beginning of an experiment.\n- **Wait Buttons** waits for a button press or release before continuing to the next item in the experiment\n- **Get Buttons Start** starts a new thread which monitors for button presses/releases, it will directly advance to the next item in the experiment\n- **Get buttons Wait** waits until the thread from 'Get Buttons Start' is finished (has detected a button press/release) before advancing to the next item in the experiment \n- **Send Control** send control code to the buttonbox, for example 'Calibrate Sound', 'Detect Sound'\n- **Send Trigger** for sending triggers to hardware with a parallel port\n\n\nTimestamps can be found in the logs by the name: time_response_[item_name]\n\n\nLinux, and Windows are supported (possible also OSX, not tested). The plug-in will first look for the globally installed rusocsci package. If this is not available, the shipped version will be used. Install options are listed below.\n  \n  \n## 2. LICENSE\n----------\n\nThe Radboud Buttonbox plug-in is distributed under the terms of the GNU General Public License 3.\nThe full license should be included in the file COPYING, or can be obtained from\n\n- <http://www.gnu.org/licenses/gpl.txt>\n\nThis plug-in contains works of others.\n  \n  \n## 3. Documentation\n----------------\n\nInstallation instructions and documentation on OpenSesame are available on the documentation website:\n\n- <http://osdoc.cogsci.nl/>\n",
     'author': 'Bob Rosbag',
     'author_email': 'debian@bobrosbag.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dev-jam/opensesame-plugin-radboudbox',
```

### Comparing `opensesame_plugin_radboudbox-4.0.0/PKG-INFO` & `opensesame_plugin_radboudbox-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensesame-plugin-radboudbox
-Version: 4.0.0
+Version: 4.1.0
 Summary: An OpenSesame Plug-in for collecting button responses, audio detection, voice key and sending stimulus synchronization triggers with the Radboud Buttonbox to data acquisition systems
 Home-page: https://github.com/dev-jam/opensesame-plugin-radboudbox
 License: LICENSE.md
 Author: Bob Rosbag
 Author-email: debian@bobrosbag.nl
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 2
```

