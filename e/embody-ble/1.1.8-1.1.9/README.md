# Comparing `tmp/embody_ble-1.1.8.tar.gz` & `tmp/embody_ble-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embody_ble-1.1.8.tar", max compression
+gzip compressed data, was "embody_ble-1.1.9.tar", max compression
```

## Comparing `embody_ble-1.1.8.tar` & `embody_ble-1.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-10-02 12:32:10.188004 embody_ble-1.1.8/LICENSE
--rw-r--r--   0        0        0     4413 2023-10-02 12:32:10.188004 embody_ble-1.1.8/README.md
--rw-r--r--   0        0        0     2135 2023-10-02 12:32:29.964395 embody_ble-1.1.8/pyproject.toml
--rw-r--r--   0        0        0      249 2023-10-02 12:32:10.188004 embody_ble-1.1.8/src/embodyble/__init__.py
--rw-r--r--   0        0        0      226 2023-10-02 12:32:10.188004 embody_ble-1.1.8/src/embodyble/__main__.py
--rw-r--r--   0        0        0     7024 2023-10-02 12:32:10.188004 embody_ble-1.1.8/src/embodyble/cli.py
--rw-r--r--   0        0        0    17880 2023-10-02 12:32:29.968396 embody_ble-1.1.8/src/embodyble/embodyble.py
--rw-r--r--   0        0        0      150 2023-10-02 12:32:10.188004 embody_ble-1.1.8/src/embodyble/exceptions.py
--rw-r--r--   0        0        0     1089 2023-10-02 12:32:10.188004 embody_ble-1.1.8/src/embodyble/listeners.py
--rw-r--r--   0        0        0        0 2023-10-02 12:32:10.188004 embody_ble-1.1.8/src/embodyble/py.typed
--rw-r--r--   0        0        0    24909 2023-10-02 12:32:10.188004 embody_ble-1.1.8/src/embodyble/reporting.py
--rw-r--r--   0        0        0     5325 1970-01-01 00:00:00.000000 embody_ble-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-10-09 19:13:35.406143 embody_ble-1.1.9/LICENSE
+-rw-r--r--   0        0        0     4413 2023-10-09 19:13:35.406143 embody_ble-1.1.9/README.md
+-rw-r--r--   0        0        0     2135 2023-10-09 19:13:51.454152 embody_ble-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-10-09 19:13:35.406143 embody_ble-1.1.9/src/embodyble/__init__.py
+-rw-r--r--   0        0        0      226 2023-10-09 19:13:35.406143 embody_ble-1.1.9/src/embodyble/__main__.py
+-rw-r--r--   0        0        0     7596 2023-10-09 19:13:35.406143 embody_ble-1.1.9/src/embodyble/cli.py
+-rw-r--r--   0        0        0    17880 2023-10-09 19:13:35.406143 embody_ble-1.1.9/src/embodyble/embodyble.py
+-rw-r--r--   0        0        0      150 2023-10-09 19:13:35.406143 embody_ble-1.1.9/src/embodyble/exceptions.py
+-rw-r--r--   0        0        0     1089 2023-10-09 19:13:35.406143 embody_ble-1.1.9/src/embodyble/listeners.py
+-rw-r--r--   0        0        0        0 2023-10-09 19:13:35.406143 embody_ble-1.1.9/src/embodyble/py.typed
+-rw-r--r--   0        0        0    25313 2023-10-09 19:13:35.406143 embody_ble-1.1.9/src/embodyble/reporting.py
+-rw-r--r--   0        0        0     5325 1970-01-01 00:00:00.000000 embody_ble-1.1.9/PKG-INFO
```

### Comparing `embody_ble-1.1.8/LICENSE` & `embody_ble-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.8/README.md` & `embody_ble-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.8/pyproject.toml` & `embody_ble-1.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "embody-ble"
-version = "1.1.8"
+version = "1.1.9"
 description = "Communicate with the EmBody device over BLE (bluetooth)"
 authors = ["Aidee Health AS <hello@aidee.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aidee-health/embody-ble"
 repository = "https://github.com/aidee-health/embody-ble"
 documentation = "https://github.com/aidee-health/embody-ble"
@@ -15,15 +15,15 @@
     "Development Status :: 5 - Production/Stable",
 ]
 [tool.poetry.urls]
 Changelog = "https://github.com/aidee-health/embody-ble/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-embody-serial = ">=1.0.22"
+embody-serial = ">=1.0.23"
 bleak = "^0.21.1"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
```

### Comparing `embody_ble-1.1.8/src/embodyble/cli.py` & `embody_ble-1.1.9/src/embodyble/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,14 +105,20 @@
             return
         elif parsed_args.reset:
             print(f"Resetting device: {send_helper.reset_device()}")
             return
         elif parsed_args.reboot:
             print(f"Rebooting device: {send_helper.reboot_device()}")
             return
+        elif parsed_args.activate_on_body_detect:
+            print(f"Activating on body detect: {send_helper.set_on_body_detect(True)}")
+        elif parsed_args.deactivate_on_body_detect:
+            print(
+                f"Deactivating on body detect: {send_helper.set_on_body_detect(False)}"
+            )
         elif parsed_args.report_attribute:
             attr_changed_listener = AttributeChangedListener()
             reporter = EmbodyReporter(embody_ble, attr_changed_listener)
             # invoke the start_<report_attribute>_reporting method dynamically
             getattr(reporter, f"start_{parsed_args.report_attribute}_reporting")(
                 parsed_args.report_interval
             )
@@ -211,14 +217,22 @@
     parser.add_argument(
         "--list-devices",
         help="List all available devices",
         action="store_true",
         default=None,
     )
     parser.add_argument(
+        "--activate-on-body-detect", help="Activate on body detect", action="store_true"
+    )
+    parser.add_argument(
+        "--deactivate-on-body-detect",
+        help="Deactivate on body detect",
+        action="store_true",
+    )
+    parser.add_argument(
         "--version",
         action="version",
         help="Echo version number.",
         version=f"{__version__}",
     )
     return parser
```

### Comparing `embody_ble-1.1.8/src/embodyble/embodyble.py` & `embody_ble-1.1.9/src/embodyble/embodyble.py`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.8/src/embodyble/listeners.py` & `embody_ble-1.1.9/src/embodyble/listeners.py`

 * *Files identical despite different names*

### Comparing `embody_ble-1.1.8/src/embodyble/reporting.py` & `embody_ble-1.1.9/src/embodyble/reporting.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,19 @@
             f"ioffdac_range={ioffdac_range}, led1={led1}, led2={led2}, led3={led3}, led4={led4}, "
             f"off_dac1={off_dac1}, off_dac2={off_dac2}, off_dac3={off_dac3}, relative_gain={relative_gain}"
         )
 
     def on_ecgs_ppgs_changed(self, ecgs: list[int], ppgs: list[int]) -> None:
         logging.info(f"ECGs and PPGs changed: ecgs={ecgs}, ppgs={ppgs}")
 
+    def on_on_body_detection_changed(self, on_body_detection: bool) -> None:
+        logging.info(
+            f"On body detection {'activated' if on_body_detection else 'deactivated'}"
+        )
+
 
 class AttributeChangedMessageListener(MessageListener, BleMessageListener):
     """MessageListener implementation delegating to high level callback interface."""
 
     def __init__(
         self, attr_changed_listener: Optional[AttributeChangedListener] = None
     ) -> None:
@@ -225,14 +230,17 @@
                         msg.value.led2_blinking(),
                         msg.value.led3(),
                         msg.value.led3_blinking(),
                     )
             elif isinstance(msg.value, attributes.FirmwareUpdateProgressAttribute):
                 for listener in self.__message_listeners:
                     listener.on_firmware_update_changed(msg.value.value)
+            elif isinstance(msg.value, attributes.OnBodyDetectAttribute):
+                for listener in self.__message_listeners:
+                    listener.on_on_body_detection_changed(msg.value.value)
             elif isinstance(msg.value, attributes.DiagnosticsAttribute):
                 for listener in self.__message_listeners:
                     listener.on_diagnostics_changed(
                         msg.value.value.rep_soc,
                         msg.value.value.avg_current,
                         msg.value.value.rep_cap,
                         msg.value.value.full_cap,
```

### Comparing `embody_ble-1.1.8/PKG-INFO` & `embody_ble-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: embody-ble
-Version: 1.1.8
+Version: 1.1.9
 Summary: Communicate with the EmBody device over BLE (bluetooth)
 Home-page: https://github.com/aidee-health/embody-ble
 License: MIT
 Author: Aidee Health AS
 Author-email: hello@aidee.io
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bleak (>=0.21.1,<0.22.0)
-Requires-Dist: embody-serial (>=1.0.22)
+Requires-Dist: embody-serial (>=1.0.23)
 Project-URL: Changelog, https://github.com/aidee-health/embody-ble/releases
 Project-URL: Documentation, https://github.com/aidee-health/embody-ble
 Project-URL: Repository, https://github.com/aidee-health/embody-ble
 Description-Content-Type: text/markdown
 
 # Embody BLE
```

