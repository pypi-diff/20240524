# Comparing `tmp/snappi-1.5.0.tar.gz` & `tmp/snappi-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snappi-1.5.0.tar", last modified: Fri May 17 06:50:47 2024, max compression
+gzip compressed data, was "snappi-1.5.1.tar", last modified: Fri May 24 08:00:08 2024, max compression
```

## Comparing `snappi-1.5.0.tar` & `snappi-1.5.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:50:47.550490 snappi-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-17 06:48:09.000000 snappi-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-17 06:50:47.550490 snappi-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:50:47.550490 snappi-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-17 06:48:09.000000 snappi-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:50:47.542490 snappi-1.5.0/snappi/
--rw-r--r--   0 runner    (1001) docker     (127)    62900 2024-05-17 06:49:26.000000 snappi-1.5.0/snappi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   720645 2024-05-17 06:49:26.000000 snappi-1.5.0/snappi/otg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15543 2024-05-17 06:49:26.000000 snappi-1.5.0/snappi/otg_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)  4278340 2024-05-17 06:50:26.000000 snappi-1.5.0/snappi/snappi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:50:47.546490 snappi-1.5.0/snappi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-17 06:50:47.000000 snappi-1.5.0/snappi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-17 06:50:47.000000 snappi-1.5.0/snappi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:50:47.000000 snappi-1.5.0/snappi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-17 06:50:47.000000 snappi-1.5.0/snappi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 06:50:47.000000 snappi-1.5.0/snappi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:50:47.546490 snappi-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_bgp_sr_te_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_create_meshed_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_deep_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_device_factory_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_device_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_e2e_port_flow_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_gtpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_hints.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_lag.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_layer1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_metric_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_packet_factory_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_port_factory_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_port_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_print.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_required.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_slots.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_snappi_list_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_snappi_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_snappi_object_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_snappi_object_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-17 06:48:09.000000 snappi-1.5.0/tests/test_types_and_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:00:08.725247 snappi-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-24 07:57:46.000000 snappi-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-24 08:00:08.725247 snappi-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 08:00:08.725247 snappi-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-24 07:57:46.000000 snappi-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:00:08.717247 snappi-1.5.1/snappi/
+-rw-r--r--   0 runner    (1001) docker     (127)    62900 2024-05-24 07:58:50.000000 snappi-1.5.1/snappi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   720645 2024-05-24 07:58:50.000000 snappi-1.5.1/snappi/otg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15543 2024-05-24 07:58:50.000000 snappi-1.5.1/snappi/otg_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)  4278467 2024-05-24 07:59:46.000000 snappi-1.5.1/snappi/snappi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:00:08.725247 snappi-1.5.1/snappi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2024-05-24 08:00:08.000000 snappi-1.5.1/snappi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-24 08:00:08.000000 snappi-1.5.1/snappi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:00:08.000000 snappi-1.5.1/snappi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-24 08:00:08.000000 snappi-1.5.1/snappi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 08:00:08.000000 snappi-1.5.1/snappi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:00:08.725247 snappi-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_bgp_sr_te_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_create_meshed_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_deep_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_device_factory_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_device_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_e2e_port_flow_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_gtpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_hints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_lag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_layer1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_metric_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_packet_factory_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_port_factory_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_port_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_snappi_list_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_snappi_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_snappi_object_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_snappi_object_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-24 07:57:46.000000 snappi-1.5.1/tests/test_types_and_formats.py
```

### Comparing `snappi-1.5.0/LICENSE` & `snappi-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/PKG-INFO` & `snappi-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snappi
-Version: 1.5.0
+Version: 1.5.1
 Summary: The Snappi Open Traffic Generator Python Package
 Home-page: https://github.com/open-traffic-generator/snappi
 Author: ajbalogh
 Author-email: andy.balogh@keysight.com
 License: MIT
 Keywords: snappi testing open traffic generator automation
 Classifier: Development Status :: 3 - Alpha
@@ -12,24 +12,24 @@
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=2.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: protobuf~=4.24.4; python_version > "3.6"
+Requires-Dist: PyYAML
 Requires-Dist: protobuf~=3.15.0; python_version <= "3.6"
-Requires-Dist: requests
-Requires-Dist: grpcio~=1.35.0; python_version <= "3.6"
+Requires-Dist: protobuf~=4.24.4; python_version > "3.6"
 Requires-Dist: grpcio~=1.59.0; python_version > "3.6"
-Requires-Dist: grpcio-tools~=1.59.0; python_version > "3.6"
 Requires-Dist: grpcio-tools~=1.35.0; python_version <= "3.6"
-Requires-Dist: PyYAML
-Requires-Dist: semantic_version
+Requires-Dist: grpcio-tools~=1.59.0; python_version > "3.6"
+Requires-Dist: grpcio~=1.35.0; python_version <= "3.6"
+Requires-Dist: requests
 Requires-Dist: urllib3
+Requires-Dist: semantic_version
 Provides-Extra: ixnetwork
 Requires-Dist: snappi_ixnetwork==0.9.1; extra == "ixnetwork"
 Provides-Extra: trex
 Requires-Dist: snappi_trex; extra == "trex"
 Provides-Extra: convergence
 Requires-Dist: snappi_convergence==0.4.1; extra == "convergence"
 Provides-Extra: testing
```

### Comparing `snappi-1.5.0/setup.py` & `snappi-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/snappi/__init__.py` & `snappi-1.5.1/snappi/__init__.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/snappi/otg_pb2.py` & `snappi-1.5.1/snappi/otg_pb2.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/snappi/otg_pb2_grpc.py` & `snappi-1.5.1/snappi/otg_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/snappi/snappi.py` & `snappi-1.5.1/snappi/snappi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Open Traffic Generator API 1.5.0
+# Open Traffic Generator API 1.5.1
 # License: MIT
 
 import importlib
 import logging
 import json
 import platform
 import yaml
@@ -975,23 +975,26 @@
         return None
 
     def _raise_status_warnings(self, property_name, property_value):
         if len(self._STATUS) > 0:
 
             if isinstance(property_name, OpenApiObject):
                 if "self" in self._STATUS and property_value is None:
-                    print("[WARNING]: %s" % self._STATUS["self"])
+                    print("[WARNING]: %s" % self._STATUS["self"], file=sys.stderr)
 
                 return
 
             enum_key = "%s.%s" % (property_name, property_value)
             if property_name in self._STATUS:
-                print("[WARNING]: %s" % self._STATUS[property_name])
+                print(
+                    "[WARNING]: %s" % self._STATUS[property_name],
+                    file=sys.stderr,
+                )
             elif enum_key in self._STATUS:
-                print("[WARNING]: %s" % self._STATUS[enum_key])
+                print("[WARNING]: %s" % self._STATUS[enum_key], file=sys.stderr)
 
 
 class OpenApiIter(OpenApiBase):
     """Container class for OpenApiObject
 
     Inheriting classes contain 0..n instances of an OpenAPI components/schemas
     object.
@@ -141470,23 +141473,23 @@
 class Api(object):
     """OpenApi Abstract API"""
 
     __warnings__ = []
 
     def __init__(self, **kwargs):
         self._version_meta = self.version()
-        self._version_meta.api_spec_version = "1.5.0"
-        self._version_meta.sdk_version = "1.5.0"
+        self._version_meta.api_spec_version = "1.5.1"
+        self._version_meta.sdk_version = "1.5.1"
         self._version_check = kwargs.get("version_check")
         if self._version_check is None:
             self._version_check = False
         self._version_check_err = None
 
     def add_warnings(self, msg):
-        print("[WARNING]: %s" % msg)
+        print("[WARNING]: %s" % msg, file=sys.stderr)
         self.__warnings__.append(msg)
 
     def _deserialize_error(self, err_string):
         # type: (str) -> Union[Error, None]
         err = self.error()
         try:
             err.deserialize(err_string)
```

### Comparing `snappi-1.5.0/snappi.egg-info/PKG-INFO` & `snappi-1.5.1/snappi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snappi
-Version: 1.5.0
+Version: 1.5.1
 Summary: The Snappi Open Traffic Generator Python Package
 Home-page: https://github.com/open-traffic-generator/snappi
 Author: ajbalogh
 Author-email: andy.balogh@keysight.com
 License: MIT
 Keywords: snappi testing open traffic generator automation
 Classifier: Development Status :: 3 - Alpha
@@ -12,24 +12,24 @@
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=2.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: protobuf~=4.24.4; python_version > "3.6"
+Requires-Dist: PyYAML
 Requires-Dist: protobuf~=3.15.0; python_version <= "3.6"
-Requires-Dist: requests
-Requires-Dist: grpcio~=1.35.0; python_version <= "3.6"
+Requires-Dist: protobuf~=4.24.4; python_version > "3.6"
 Requires-Dist: grpcio~=1.59.0; python_version > "3.6"
-Requires-Dist: grpcio-tools~=1.59.0; python_version > "3.6"
 Requires-Dist: grpcio-tools~=1.35.0; python_version <= "3.6"
-Requires-Dist: PyYAML
-Requires-Dist: semantic_version
+Requires-Dist: grpcio-tools~=1.59.0; python_version > "3.6"
+Requires-Dist: grpcio~=1.35.0; python_version <= "3.6"
+Requires-Dist: requests
 Requires-Dist: urllib3
+Requires-Dist: semantic_version
 Provides-Extra: ixnetwork
 Requires-Dist: snappi_ixnetwork==0.9.1; extra == "ixnetwork"
 Provides-Extra: trex
 Requires-Dist: snappi_trex; extra == "trex"
 Provides-Extra: convergence
 Requires-Dist: snappi_convergence==0.4.1; extra == "convergence"
 Provides-Extra: testing
```

### Comparing `snappi-1.5.0/snappi.egg-info/SOURCES.txt` & `snappi-1.5.1/snappi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_bgp_sr_te_policy.py` & `snappi-1.5.1/tests/test_bgp_sr_te_policy.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_capture.py` & `snappi-1.5.1/tests/test_capture.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_choice.py` & `snappi-1.5.1/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_create_meshed_flow.py` & `snappi-1.5.1/tests/test_create_meshed_flow.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_deep_copy.py` & `snappi-1.5.1/tests/test_deep_copy.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_defaults.py` & `snappi-1.5.1/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_device_factory_methods.py` & `snappi-1.5.1/tests/test_device_factory_methods.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_device_stack.py` & `snappi-1.5.1/tests/test_device_stack.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_e2e_port_flow_config.py` & `snappi-1.5.1/tests/test_e2e_port_flow_config.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_grpc_client.py` & `snappi-1.5.1/tests/test_grpc_client.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_gtpu.py` & `snappi-1.5.1/tests/test_gtpu.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_lag.py` & `snappi-1.5.1/tests/test_lag.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_metric_tag.py` & `snappi-1.5.1/tests/test_metric_tag.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_packet_factory_methods.py` & `snappi-1.5.1/tests/test_packet_factory_methods.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_port_factory_method.py` & `snappi-1.5.1/tests/test_port_factory_method.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_required.py` & `snappi-1.5.1/tests/test_required.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_slots.py` & `snappi-1.5.1/tests/test_slots.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_snappi_lists.py` & `snappi-1.5.1/tests/test_snappi_lists.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_snappi_object_equality.py` & `snappi-1.5.1/tests/test_snappi_object_equality.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_snappi_object_serialization.py` & `snappi-1.5.1/tests/test_snappi_object_serialization.py`

 * *Files identical despite different names*

### Comparing `snappi-1.5.0/tests/test_types_and_formats.py` & `snappi-1.5.1/tests/test_types_and_formats.py`

 * *Files identical despite different names*

