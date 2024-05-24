# Comparing `tmp/opensesame_plugin_titta_eyetracking-2.1.2.tar.gz` & `tmp/opensesame_plugin_titta_eyetracking-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensesame_plugin_titta_eyetracking-2.1.2.tar", max compression
+gzip compressed data, was "opensesame_plugin_titta_eyetracking-2.2.0.tar", max compression
```

## Comparing `opensesame_plugin_titta_eyetracking-2.1.2.tar` & `opensesame_plugin_titta_eyetracking-2.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    14184 2023-07-20 06:23:22.000000 opensesame_plugin_titta_eyetracking-2.1.2/LICENSE.md
--rw-r--r--   0        0        0     1766 2024-01-08 11:31:04.802801 opensesame_plugin_titta_eyetracking-2.1.2/README.md
--rw-r--r--   0        0        0      140 2023-06-30 14:04:59.868240 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/__init__.py
--rw-r--r--   0        0        0      462 2024-01-11 12:20:46.711995 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_calibrate/__init__.py
--rw-r--r--   0        0        0      120 2023-03-15 11:48:08.000000 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_calibrate/titta_calibrate.md
--rw-r--r--   0        0        0     1739 2023-07-05 21:20:34.165485 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_calibrate/titta_calibrate.png
--rw-r--r--   0        0        0     1848 2023-08-05 22:20:48.183281 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_calibrate/titta_calibrate.py
--rw-r--r--   0        0        0     3239 2023-07-05 21:20:14.340123 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_calibrate/titta_calibrate_large.png
--rw-r--r--   0        0        0     2659 2024-01-11 12:20:46.711995 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_init/__init__.py
--rw-r--r--   0        0        0      120 2023-03-15 11:48:08.000000 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_init/titta_init.md
--rw-r--r--   0        0        0     1487 2023-07-05 21:21:26.873534 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_init/titta_init.png
--rw-r--r--   0        0        0     2716 2024-01-11 10:09:11.715916 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_init/titta_init.py
--rw-r--r--   0        0        0     2289 2023-07-05 21:21:12.123228 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_init/titta_init_large.png
--rw-r--r--   0        0        0      665 2024-01-11 12:20:46.710995 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_save_data/__init__.py
--rw-r--r--   0        0        0      120 2024-01-11 10:08:32.044442 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_save_data/titta_save_data.md
--rw-r--r--   0        0        0      824 2024-01-11 10:08:32.044442 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_save_data/titta_save_data.png
--rw-r--r--   0        0        0     2150 2024-01-11 12:19:34.732306 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_save_data/titta_save_data.py
--rw-r--r--   0        0        0     1369 2024-01-11 10:08:32.044442 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_save_data/titta_save_data_large.png
--rw-r--r--   0        0        0      660 2024-01-11 12:20:46.711995 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_send_message/__init__.py
--rw-r--r--   0        0        0      120 2023-03-15 11:48:08.000000 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_send_message/titta_send_message.md
--rw-r--r--   0        0        0      805 2023-06-29 21:35:35.429251 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_send_message/titta_send_message.png
--rw-r--r--   0        0        0     1304 2023-08-05 22:18:18.896548 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_send_message/titta_send_message.py
--rw-r--r--   0        0        0     1305 2023-06-29 21:34:52.904459 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_send_message/titta_send_message_large.png
--rw-r--r--   0        0        0      460 2024-01-11 12:20:46.711995 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_start_recording/__init__.py
--rw-r--r--   0        0        0      120 2023-03-15 11:48:08.000000 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_start_recording/titta_start_recording.md
--rw-r--r--   0        0        0     1432 2023-07-05 21:27:48.633394 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_start_recording/titta_start_recording.png
--rw-r--r--   0        0        0     2093 2023-12-05 09:42:19.529338 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_start_recording/titta_start_recording.py
--rw-r--r--   0        0        0     2156 2023-07-05 21:27:33.213951 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_start_recording/titta_start_recording_large.png
--rw-r--r--   0        0        0      459 2024-01-11 12:20:46.711995 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_stop_recording/__init__.py
--rw-r--r--   0        0        0      120 2023-03-15 11:48:08.000000 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording.md
--rw-r--r--   0        0        0      804 2023-07-05 21:28:32.537665 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording.png
--rw-r--r--   0        0        0     2082 2024-01-11 10:08:32.045442 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording.py
--rw-r--r--   0        0        0     1304 2023-07-05 21:28:17.918240 opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording_large.png
--rw-r--r--   0        0        0      616 2024-01-11 12:20:46.724995 opensesame_plugin_titta_eyetracking-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 opensesame_plugin_titta_eyetracking-2.1.2/setup.py
--rw-r--r--   0        0        0     2580 1970-01-01 00:00:00.000000 opensesame_plugin_titta_eyetracking-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0    14184 2023-08-15 21:37:08.620970 opensesame_plugin_titta_eyetracking-2.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1766 2023-12-21 23:53:54.486564 opensesame_plugin_titta_eyetracking-2.2.0/README.md
+-rw-r--r--   0        0        0      140 2023-08-15 21:37:08.620970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/__init__.py
+-rw-r--r--   0        0        0      462 2024-05-24 13:27:40.643344 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_calibrate/__init__.py
+-rw-r--r--   0        0        0      120 2023-08-15 21:37:08.621970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_calibrate/titta_calibrate.md
+-rw-r--r--   0        0        0     1739 2023-08-15 21:37:08.621970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_calibrate/titta_calibrate.png
+-rw-r--r--   0        0        0     1848 2023-08-15 21:37:08.621970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_calibrate/titta_calibrate.py
+-rw-r--r--   0        0        0     3239 2023-08-15 21:37:08.621970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_calibrate/titta_calibrate_large.png
+-rw-r--r--   0        0        0     2659 2024-05-24 13:27:40.642343 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_init/__init__.py
+-rw-r--r--   0        0        0      120 2023-08-15 21:37:08.622970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_init/titta_init.md
+-rw-r--r--   0        0        0     1487 2023-08-15 21:37:08.622970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_init/titta_init.png
+-rw-r--r--   0        0        0     2716 2024-01-11 19:26:03.209518 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_init/titta_init.py
+-rw-r--r--   0        0        0     2289 2023-08-15 21:37:08.622970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_init/titta_init_large.png
+-rw-r--r--   0        0        0      665 2024-05-24 13:27:40.642343 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_save_data/__init__.py
+-rw-r--r--   0        0        0      120 2023-03-15 11:48:08.000000 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_save_data/titta_save_data.md
+-rw-r--r--   0        0        0      824 2024-01-10 23:20:21.249532 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_save_data/titta_save_data.png
+-rw-r--r--   0        0        0     2953 2024-05-24 13:21:35.655498 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_save_data/titta_save_data.py
+-rw-r--r--   0        0        0     1369 2024-01-10 23:20:14.391411 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_save_data/titta_save_data_large.png
+-rw-r--r--   0        0        0      660 2024-05-24 13:27:40.642343 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_send_message/__init__.py
+-rw-r--r--   0        0        0      120 2023-08-15 21:37:08.622970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_send_message/titta_send_message.md
+-rw-r--r--   0        0        0      805 2023-08-15 21:37:08.623970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_send_message/titta_send_message.png
+-rw-r--r--   0        0        0     1304 2023-08-15 21:37:08.623970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_send_message/titta_send_message.py
+-rw-r--r--   0        0        0     1305 2023-08-15 21:37:08.623970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_send_message/titta_send_message_large.png
+-rw-r--r--   0        0        0      460 2024-05-24 13:27:40.643344 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_start_recording/__init__.py
+-rw-r--r--   0        0        0      120 2023-08-15 21:37:08.623970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_start_recording/titta_start_recording.md
+-rw-r--r--   0        0        0     1432 2023-08-15 21:37:08.623970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_start_recording/titta_start_recording.png
+-rw-r--r--   0        0        0     2093 2023-12-04 08:46:15.148947 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_start_recording/titta_start_recording.py
+-rw-r--r--   0        0        0     2156 2023-08-15 21:37:08.624970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_start_recording/titta_start_recording_large.png
+-rw-r--r--   0        0        0      459 2024-05-24 13:27:40.643344 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_stop_recording/__init__.py
+-rw-r--r--   0        0        0      120 2023-08-15 21:37:08.624970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording.md
+-rw-r--r--   0        0        0      804 2023-08-15 21:37:08.624970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording.png
+-rw-r--r--   0        0        0     2082 2024-01-09 21:28:14.762142 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording.py
+-rw-r--r--   0        0        0     1304 2023-08-15 21:37:08.624970 opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording_large.png
+-rw-r--r--   0        0        0      616 2024-05-24 13:27:40.643344 opensesame_plugin_titta_eyetracking-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 opensesame_plugin_titta_eyetracking-2.2.0/setup.py
+-rw-r--r--   0        0        0     2580 1970-01-01 00:00:00.000000 opensesame_plugin_titta_eyetracking-2.2.0/PKG-INFO
```

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/LICENSE.md` & `opensesame_plugin_titta_eyetracking-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/README.md` & `opensesame_plugin_titta_eyetracking-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_calibrate/titta_calibrate.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_calibrate/titta_calibrate.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_calibrate/titta_calibrate.py` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_calibrate/titta_calibrate.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_calibrate/titta_calibrate_large.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_calibrate/titta_calibrate_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_init/__init__.py` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_init/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,10 +59,10 @@
 For questions, bug reports or to check for updates on Titta, please visit https://github.com/marcus-nystrom/Titta.\n\n\
 To minimize the risk of missing samples, the current repository uses TittaPy (pip install TittaPy), a C++ wrapper around the Tobii SDK, to pull samples made available from the eye tracker."
     }, {
         "type": "text",
         "label": "<small><b>Note:</b> Titta Init item at the begin of the experiment is needed for initialization of the Eye Tracker</small>"
     }, {
         "type": "text",
-        "label": "<small>Titta Eye Tracking version 2.1.2</small>"
+        "label": "<small>Titta Eye Tracking version 2.2.0</small>"
     }
 ]
```

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_init/titta_init.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_init/titta_init.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_init/titta_init.py` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_init/titta_init.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_init/titta_init_large.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_init/titta_init_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_save_data/__init__.py` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_save_data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,10 +11,10 @@
         "name": "checkbox_tsv_export",
         "tooltip": "Additionally export data to tsv"
     },  {
         "type": "text",
         "label": "<small><b>Note:</b> Titta Init item at the begin of the experiment is needed for initialization of the Eye Tracker</small>"
     }, {
         "type": "text",
-        "label": "<small>Titta Eye Tracking version 2.1.2</small>"
+        "label": "<small>Titta Eye Tracking version 2.2.0</small>"
     }
 ]
```

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_save_data/titta_save_data.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_save_data/titta_save_data.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_save_data/titta_save_data.py` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,61 +4,55 @@
 """
 
 from libopensesame.py3compat import *
 from libopensesame.item import Item
 from libqtopensesame.items.qtautoplugin import QtAutoPlugin
 from libopensesame.exceptions import OSException
 from libopensesame.oslogging import oslogger
-import pandas as pd
 
 
-class TittaSaveData(Item):
-
-    def reset(self):
-        self.var.tsv_export = 'no'
+class TittaStopRecording(Item):
 
     def prepare(self):
         super().prepare()
-        self._init_var()
         self._check_init()
+        self.experiment.titta_stop_recording = True
 
     def run(self):
-        self._check_stop()
+        self._check_start()
         self.set_item_onset()
-        self.experiment.tracker.save_data()
-        
-        if self.tsv_export == 'yes':
-            df_gaze = pd.read_hdf(self.experiment.titta_file_name + '.h5', 'gaze')
-            df_msg = pd.read_hdf(self.experiment.titta_file_name + '.h5', 'msg')
-            df_gaze.to_csv(self.experiment.titta_file_name + '_gaze.tsv', sep='\t')
-            df_msg.to_csv(self.experiment.titta_file_name + '_msg.tsv', sep='\t')
+        self.experiment.tracker.stop_recording(gaze=True,
+                                               time_sync=True,
+                                               eye_image=False,
+                                               notifications=True,
+                                               external_signal=True,
+                                               positioning=True)
+        self.experiment.titta_recording = False
 
     def _check_init(self):
         if hasattr(self.experiment, "titta_dummy_mode"):
             self.dummy_mode = self.experiment.titta_dummy_mode
             self.verbose = self.experiment.titta_verbose
         else:
             raise OSException('You should have one instance of `Titta Init` at the start of your experiment')
 
-    def _check_stop(self):
-        if not hasattr(self.experiment, "titta_stop_recording"):
+    def _check_start(self):
+        if not hasattr(self.experiment, "titta_start_recording"):
             raise OSException(
-                    '`Titta Stop Recording` item is missing')
-        elif self.experiment.titta_recording:
+                    '`Titta Start Recording` item is missing')
+        else:
+            if not self.experiment.titta_recording:
                 raise OSException(
-                        'Titta still recording, you first have to stop recording before saving data')
-
-    def _init_var(self):
-        self.tsv_export = self.var.tsv_export
+                        'Titta not recording, you first have to start recording before stopping')
 
     def _show_message(self, message):
         oslogger.debug(message)
         if self.verbose == 'yes':
             print(message)
 
 
-class QtTittaSaveData(TittaSaveData, QtAutoPlugin):
+class QtTittaStopRecording(TittaStopRecording, QtAutoPlugin):
 
     def __init__(self, name, experiment, script=None):
-        TittaSaveData.__init__(self, name, experiment, script)
+        TittaStopRecording.__init__(self, name, experiment, script)
         QtAutoPlugin.__init__(self, __file__)
```

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_save_data/titta_save_data_large.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_save_data/titta_save_data_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_send_message/__init__.py` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_send_message/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,10 +11,10 @@
         "name": "line_edit_message",
         "tooltip": "Message"
     }, {
         "type": "text",
         "label": "<small><b>Note:</b> Titta Init item at the begin of the experiment is needed for initialization of the Eye Tracker</small>"
     }, {
         "type": "text",
-        "label": "<small>Titta Eye Tracking version 2.1.2</small>"
+        "label": "<small>Titta Eye Tracking version 2.2.0</small>"
     }
 ]
```

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_send_message/titta_send_message.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_send_message/titta_send_message.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_send_message/titta_send_message.py` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_send_message/titta_send_message.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_send_message/titta_send_message_large.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_send_message/titta_send_message_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_start_recording/titta_start_recording.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_start_recording/titta_start_recording.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_start_recording/titta_start_recording.py` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_start_recording/titta_start_recording.py`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_start_recording/titta_start_recording_large.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_start_recording/titta_start_recording_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording.py` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_save_data/titta_save_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,55 +4,70 @@
 """
 
 from libopensesame.py3compat import *
 from libopensesame.item import Item
 from libqtopensesame.items.qtautoplugin import QtAutoPlugin
 from libopensesame.exceptions import OSException
 from libopensesame.oslogging import oslogger
+import pandas as pd
 
 
-class TittaStopRecording(Item):
+class TittaSaveData(Item):
+
+    def reset(self):
+        self.var.tsv_export = 'no'
 
     def prepare(self):
         super().prepare()
+        self._init_var()
         self._check_init()
-        self.experiment.titta_stop_recording = True
 
     def run(self):
-        self._check_start()
+        self._check_stop()
         self.set_item_onset()
-        self.experiment.tracker.stop_recording(gaze=True,
-                                               time_sync=True,
-                                               eye_image=False,
-                                               notifications=True,
-                                               external_signal=True,
-                                               positioning=True)
-        self.experiment.titta_recording = False
+        self.experiment.tracker.save_data()
+        
+        if self.tsv_export == 'yes' and self.experiment.titta_dummy_mode == 'no':
+            df_gaze = pd.read_hdf(self.experiment.titta_file_name + '.h5', 'gaze')
+            df_msg = pd.read_hdf(self.experiment.titta_file_name + '.h5', 'msg')
+            df_external_signal = pd.read_hdf(self.experiment.titta_file_name + '.h5', 'external_signal')
+            df_calibration_history = pd.read_hdf(self.experiment.titta_file_name + '.h5', 'calibration_history')
+            df_merged = pd.concat([df_gaze, df_msg, df_external_signal])
+            df_merged.sort_values("system_time_stamp", axis = 0, ascending = True,
+                                 inplace = True, na_position ='last')
+
+            df_gaze.to_csv(self.experiment.titta_file_name + '_gaze.tsv', sep='\t')
+            df_msg.to_csv(self.experiment.titta_file_name + '_msg.tsv', sep='\t')
+            df_external_signal.to_csv(self.experiment.titta_file_name + '_external_signal.tsv', sep='\t')
+            df_calibration_history.to_csv(self.experiment.titta_file_name + '_calibration_history.tsv', sep='\t')
+            df_merged.to_csv(self.experiment.titta_file_name + '_data_merged.tsv', sep='\t')
 
     def _check_init(self):
         if hasattr(self.experiment, "titta_dummy_mode"):
             self.dummy_mode = self.experiment.titta_dummy_mode
             self.verbose = self.experiment.titta_verbose
         else:
             raise OSException('You should have one instance of `Titta Init` at the start of your experiment')
 
-    def _check_start(self):
-        if not hasattr(self.experiment, "titta_start_recording"):
+    def _check_stop(self):
+        if not hasattr(self.experiment, "titta_stop_recording"):
             raise OSException(
-                    '`Titta Start Recording` item is missing')
-        else:
-            if not self.experiment.titta_recording:
+                    '`Titta Stop Recording` item is missing')
+        elif self.experiment.titta_recording:
                 raise OSException(
-                        'Titta not recording, you first have to start recording before stopping')
+                        'Titta still recording, you first have to stop recording before saving data')
+
+    def _init_var(self):
+        self.tsv_export = self.var.tsv_export
 
     def _show_message(self, message):
         oslogger.debug(message)
         if self.verbose == 'yes':
             print(message)
 
 
-class QtTittaStopRecording(TittaStopRecording, QtAutoPlugin):
+class QtTittaSaveData(TittaSaveData, QtAutoPlugin):
 
     def __init__(self, name, experiment, script=None):
-        TittaStopRecording.__init__(self, name, experiment, script)
+        TittaSaveData.__init__(self, name, experiment, script)
         QtAutoPlugin.__init__(self, __file__)
```

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording_large.png` & `opensesame_plugin_titta_eyetracking-2.2.0/opensesame_plugins/titta/titta_stop_recording/titta_stop_recording_large.png`

 * *Files identical despite different names*

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/setup.py` & `opensesame_plugin_titta_eyetracking-2.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas', 'titta>=2.0.1', 'tittapy>=1.0.0']
 
 setup_kwargs = {
     'name': 'opensesame-plugin-titta-eyetracking',
-    'version': '2.1.2',
+    'version': '2.2.0',
     'description': 'Titta Eye Tracking plugin for OpenSesame',
     'long_description': "# OpenSesame Plugin: Titta Eye Tracking\n\n*Copyright, 2023, Bob Rosbag, Diederick C. Niehorster & Marcus Nyström*\n\n## About\n\nThis plugin implements Titta in OpenSesame for Eye Tracking. \n\nTitta is a toolbox for using eye trackers from Tobii Pro AB with Python, specifically offering integration with PsychoPy. A Matlab version that integrates with PsychToolbox is also available from https://github.com/dcnieho/Titta. For a similar toolbox for SMI eye trackers, please see www.github.com/marcus-nystrom/SMITE.\n\nCite as: Niehorster, D.C., Andersson, R. & Nystrom, M. (2020). Titta: A toolbox for creating PsychToolbox and Psychopy experiments with Tobii eye trackers. Behavior Research Methods. doi: 10.3758/s13428-020-01358-8\n\nPlease mention: Bob Rosbag as creator of this plugin\n\nFor questions, bug reports or to check for updates, please visit https://github.com/marcus-nystrom/Titta.\n\nTo minimize the risk of missing samples, the current repository uses TittaPy (pip install TittaPy), a C++ wrapper around the Tobii SDK, to pull samples made available from the eye tracker.\n\n\n## License\n\nThe Titta Eye Tracking plugin is distributed under the terms of the Creative Commons Attribution 4.0 International Public License\nThe full license should be included in the file LICENSE.md\n\n\n## Known bugs\n\n- In dummy mode, when the experiment is finished, OpenSesame will not return to the GUI. The button with the cross and text: 'Forcibly kill the experiment' has to be used to end the session and get back to the GUI. This only happens when in dummy mode and the cause resides somewhere in the 'calibrate' command.\n\n\n## Notes\n\n- One recording per experiment is working properly. Per trial recording (multiple starts en stops within an experiment) has not yet been tested.\n",
     'author': 'Bob Rosbag',
     'author_email': 'debian@bobrosbag.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dev-jam/opensesame-plugin-titta_eyetracking',
```

### Comparing `opensesame_plugin_titta_eyetracking-2.1.2/PKG-INFO` & `opensesame_plugin_titta_eyetracking-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensesame-plugin-titta-eyetracking
-Version: 2.1.2
+Version: 2.2.0
 Summary: Titta Eye Tracking plugin for OpenSesame
 Home-page: https://github.com/dev-jam/opensesame-plugin-titta_eyetracking
 License: LICENSE.md
 Author: Bob Rosbag
 Author-email: debian@bobrosbag.nl
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
```

