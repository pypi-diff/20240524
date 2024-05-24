# Comparing `tmp/boinc_client-1.8.0.tar.gz` & `tmp/boinc_client-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boinc_client-1.8.0.tar", max compression
+gzip compressed data, was "boinc_client-1.9.0.tar", max compression
```

## Comparing `boinc_client-1.8.0.tar` & `boinc_client-1.9.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0    35148 2024-01-17 10:20:04.966132 boinc_client-1.8.0/LICENSE.md
--rw-r--r--   0        0        0     2273 2024-01-17 10:20:04.966132 boinc_client-1.8.0/README.md
--rw-r--r--   0        0        0      925 2024-01-17 10:20:16.958275 boinc_client-1.8.0/pyproject.toml
--rw-r--r--   0        0        0       28 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/__init__.py
--rw-r--r--   0        0        0     4711 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/boinc_client.py
--rw-r--r--   0        0        0        0 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/clients/__init__.py
--rw-r--r--   0        0        0     2846 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/clients/rpc_client.py
--rw-r--r--   0        0        0     1152 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/messages.py
--rw-r--r--   0        0        0        0 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/__init__.py
--rw-r--r--   0        0        0      735 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/cc_status.py
--rw-r--r--   0        0        0     5195 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/client_state.py
--rw-r--r--   0        0        0      210 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/client_update.py
--rw-r--r--   0        0        0      254 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/client_version.py
--rw-r--r--   0        0        0      532 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/disk_stats.py
--rw-r--r--   0        0        0     1190 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/file_transfer.py
--rw-r--r--   0        0        0      274 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/generic_response.py
--rw-r--r--   0        0        0     1365 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/global_preference_override.py
--rw-r--r--   0        0        0     1615 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/global_preferences.py
--rw-r--r--   0        0        0      852 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/helpers.py
--rw-r--r--   0        0        0     1340 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/host_info.py
--rw-r--r--   0        0        0      118 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/message_count.py
--rw-r--r--   0        0        0      925 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/messages.py
--rw-r--r--   0        0        0     1173 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/network_transfers.py
--rw-r--r--   0        0        0      738 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/old_results.py
--rw-r--r--   0        0        0      294 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/project_attach.py
--rw-r--r--   0        0        0     3449 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/project_status.py
--rw-r--r--   0        0        0     1167 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/projects.py
--rw-r--r--   0        0        0     1326 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/projects_stats.py
--rw-r--r--   0        0        0     1054 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/public_notice.py
--rw-r--r--   0        0        0     2185 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/result.py
--rw-r--r--   0        0        0      382 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/screensaver_tasks.py
--rw-r--r--   0        0        0      612 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/models/simple_gui_info.py
--rw-r--r--   0        0        0     2105 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/preferences.py
--rw-r--r--   0        0        0     3975 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/projects.py
--rw-r--r--   0        0        0      723 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/results.py
--rw-r--r--   0        0        0      830 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/stats.py
--rw-r--r--   0        0        0     2742 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/status.py
--rw-r--r--   0        0        0      793 2024-01-17 10:20:04.966132 boinc_client-1.8.0/src/boinc_client/versions.py
--rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 boinc_client-1.8.0/setup.py
--rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 boinc_client-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-03-06 14:06:15.774183 boinc_client-1.9.0/LICENSE.md
+-rw-r--r--   0        0        0     2339 2024-03-06 14:06:15.774183 boinc_client-1.9.0/README.md
+-rw-r--r--   0        0        0      925 2024-03-06 14:06:31.018306 boinc_client-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0       28 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/__init__.py
+-rw-r--r--   0        0        0     5215 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/boinc_client.py
+-rw-r--r--   0        0        0        0 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/clients/__init__.py
+-rw-r--r--   0        0        0     2846 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/clients/rpc_client.py
+-rw-r--r--   0        0        0     1152 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/messages.py
+-rw-r--r--   0        0        0        0 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/__init__.py
+-rw-r--r--   0        0        0      735 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/cc_status.py
+-rw-r--r--   0        0        0     5195 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/client_state.py
+-rw-r--r--   0        0        0      210 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/client_update.py
+-rw-r--r--   0        0        0      254 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/client_version.py
+-rw-r--r--   0        0        0      532 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/disk_stats.py
+-rw-r--r--   0        0        0     1190 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/file_transfer.py
+-rw-r--r--   0        0        0      274 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/generic_response.py
+-rw-r--r--   0        0        0     1365 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/global_preference_override.py
+-rw-r--r--   0        0        0     1615 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/global_preferences.py
+-rw-r--r--   0        0        0      852 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/helpers.py
+-rw-r--r--   0        0        0     1340 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/host_info.py
+-rw-r--r--   0        0        0      118 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/message_count.py
+-rw-r--r--   0        0        0      925 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/messages.py
+-rw-r--r--   0        0        0     1173 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/network_transfers.py
+-rw-r--r--   0        0        0      738 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/old_results.py
+-rw-r--r--   0        0        0      294 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/project_attach.py
+-rw-r--r--   0        0        0     3449 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/project_status.py
+-rw-r--r--   0        0        0     1167 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/projects.py
+-rw-r--r--   0        0        0     1326 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/projects_stats.py
+-rw-r--r--   0        0        0     1054 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/public_notice.py
+-rw-r--r--   0        0        0     2185 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/result.py
+-rw-r--r--   0        0        0      382 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/screensaver_tasks.py
+-rw-r--r--   0        0        0      612 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/models/simple_gui_info.py
+-rw-r--r--   0        0        0     1814 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/modes.py
+-rw-r--r--   0        0        0     2105 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/preferences.py
+-rw-r--r--   0        0        0     3975 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/projects.py
+-rw-r--r--   0        0        0      723 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/results.py
+-rw-r--r--   0        0        0      830 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/stats.py
+-rw-r--r--   0        0        0     2742 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/status.py
+-rw-r--r--   0        0        0      793 2024-03-06 14:06:15.774183 boinc_client-1.9.0/src/boinc_client/versions.py
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 boinc_client-1.9.0/setup.py
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 boinc_client-1.9.0/PKG-INFO
```

### Comparing `boinc_client-1.8.0/LICENSE.md` & `boinc_client-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/README.md` & `boinc_client-1.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # BOINC Client
 
 ![Test and Release](https://github.com/SplinterHead/boinc-client/actions/workflows/test-and-release.yml/badge.svg)
 [![boinc-client](https://snyk.io/advisor/python/boinc-client/badge.svg)](https://snyk.io/advisor/python/boinc-client)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/boinc-client)
+
 
 Python native library for interacting with a BOINC client via RPC. This library has been designed to have consistent response types.
 
 ## Usage
 
 ### Setup
```

### Comparing `boinc_client-1.8.0/pyproject.toml` & `boinc_client-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boinc-client"
-version = "1.8.0"
+version = "1.9.0"
 description = "Python API for interacting with a BOINC client via RPC"
 authors = ["Lewis England <lewis2004@hotmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 homepage = "https://github.com/SplinterHead/boinc-client"
 issues = "https://github.com/SplinterHead/boinc-client/issues"
```

### Comparing `boinc_client-1.8.0/src/boinc_client/boinc_client.py` & `boinc_client-1.9.0/src/boinc_client/boinc_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from boinc_client.clients.rpc_client import RpcClient
 
 from .messages import message_count, messages, public_notices
+from .modes import set_cpu_run_mode, set_gpu_run_mode, set_network_mode
 from .preferences import (
     get_global_prefs_file,
     get_global_prefs_override,
     get_global_prefs_working,
     read_global_prefs_override,
     set_global_prefs_override,
 )
@@ -156,7 +157,16 @@
         return set_global_prefs_override(self.rpc_client, pref_override)
 
     def get_global_prefs_working(self) -> dict:
         return get_global_prefs_working(self.rpc_client)
 
     def read_global_prefs_override(self) -> dict:
         return read_global_prefs_override(self.rpc_client)
+
+    def set_cpu_run_mode(self, run_mode: str, duration: int = 0) -> dict:
+        return set_cpu_run_mode(self.rpc_client, run_mode, duration)
+
+    def set_gpu_run_mode(self, run_mode: str, duration: int = 0) -> dict:
+        return set_gpu_run_mode(self.rpc_client, run_mode, duration)
+
+    def set_network_mode(self, run_mode: str, duration: int = 0) -> dict:
+        return set_network_mode(self.rpc_client, run_mode, duration)
```

### Comparing `boinc_client-1.8.0/src/boinc_client/clients/rpc_client.py` & `boinc_client-1.9.0/src/boinc_client/clients/rpc_client.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/messages.py` & `boinc_client-1.9.0/src/boinc_client/messages.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/cc_status.py` & `boinc_client-1.9.0/src/boinc_client/models/cc_status.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/client_state.py` & `boinc_client-1.9.0/src/boinc_client/models/client_state.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/disk_stats.py` & `boinc_client-1.9.0/src/boinc_client/models/disk_stats.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/file_transfer.py` & `boinc_client-1.9.0/src/boinc_client/models/file_transfer.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/global_preference_override.py` & `boinc_client-1.9.0/src/boinc_client/models/global_preference_override.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/global_preferences.py` & `boinc_client-1.9.0/src/boinc_client/models/global_preferences.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/helpers.py` & `boinc_client-1.9.0/src/boinc_client/models/helpers.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/host_info.py` & `boinc_client-1.9.0/src/boinc_client/models/host_info.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/messages.py` & `boinc_client-1.9.0/src/boinc_client/models/messages.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/network_transfers.py` & `boinc_client-1.9.0/src/boinc_client/models/network_transfers.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/old_results.py` & `boinc_client-1.9.0/src/boinc_client/models/old_results.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/project_status.py` & `boinc_client-1.9.0/src/boinc_client/models/project_status.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/projects.py` & `boinc_client-1.9.0/src/boinc_client/models/projects.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/projects_stats.py` & `boinc_client-1.9.0/src/boinc_client/models/projects_stats.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/public_notice.py` & `boinc_client-1.9.0/src/boinc_client/models/public_notice.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/result.py` & `boinc_client-1.9.0/src/boinc_client/models/result.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/models/simple_gui_info.py` & `boinc_client-1.9.0/src/boinc_client/models/simple_gui_info.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/preferences.py` & `boinc_client-1.9.0/src/boinc_client/preferences.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/projects.py` & `boinc_client-1.9.0/src/boinc_client/projects.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/results.py` & `boinc_client-1.9.0/src/boinc_client/results.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/stats.py` & `boinc_client-1.9.0/src/boinc_client/stats.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/status.py` & `boinc_client-1.9.0/src/boinc_client/status.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/src/boinc_client/versions.py` & `boinc_client-1.9.0/src/boinc_client/versions.py`

 * *Files identical despite different names*

### Comparing `boinc_client-1.8.0/setup.py` & `boinc_client-1.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 install_requires = \
 ['lxml>=4.9.2,<6.0.0',
  'marshmallow>=3.19.0,<4.0.0',
  'xmltodict>=0.13.0,<0.14.0']
 
 setup_kwargs = {
     'name': 'boinc-client',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': 'Python API for interacting with a BOINC client via RPC',
-    'long_description': '# BOINC Client\n\n![Test and Release](https://github.com/SplinterHead/boinc-client/actions/workflows/test-and-release.yml/badge.svg)\n[![boinc-client](https://snyk.io/advisor/python/boinc-client/badge.svg)](https://snyk.io/advisor/python/boinc-client)\n\nPython native library for interacting with a BOINC client via RPC. This library has been designed to have consistent response types.\n\n## Usage\n\n### Setup\n\n```python\nfrom boinc_client import Boinc\nfrom boinc_client.clients.rpc_client import RpcClient\n\n# Hostname or IP of the running BOINC client\nBOINC_HOSTNAME = "192.168.0.2"\n\n# Create an RPC client to connect to the BOINC socket\nrpc_client = RpcClient(hostname=BOINC_HOSTNAME)\nrpc_client.authenticate()\n\n# Create a BOINC client to interact with the RPC socket\nboinc_client = Boinc(rpc_client=rpc_client)\n```\n\n#### RPC Client options\nThe following options can be passed when creating an `RpcClient` instance\n\n| Argument   | Description                                                                | Required | Default |\n|------------|----------------------------------------------------------------------------|----------|---------|\n| `hostname` | Hostname or IP address of the BOINC client                                 | Yes      | None    |\n| `port`     | Exposed port of the BOINC client                                           | No       | 31416   |\n| `timeout`  | Seconds to wait for a successful connection to the RPC socket              | No       | 30      |\n| `password` | Password to authenticate to the BOINC client, required for most operations | No       | None    |\n\n#### Boinc options\nThe following options can be passed when creating a `Boinc` instance\n\n| Argument     | Description                        | Required | Default |\n|--------------|------------------------------------|----------|---------|\n| `rpc_client` | Instance of a configured RpcClient | Yes      | None    |\n\n### Interacting with Boinc\n\n* [Unauthorised Operations](docs/unauthorised.md)\n* [Project Operations](docs/project.md)\n\n## Contributors\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->',
+    'long_description': '# BOINC Client\n\n![Test and Release](https://github.com/SplinterHead/boinc-client/actions/workflows/test-and-release.yml/badge.svg)\n[![boinc-client](https://snyk.io/advisor/python/boinc-client/badge.svg)](https://snyk.io/advisor/python/boinc-client)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/boinc-client)\n\n\nPython native library for interacting with a BOINC client via RPC. This library has been designed to have consistent response types.\n\n## Usage\n\n### Setup\n\n```python\nfrom boinc_client import Boinc\nfrom boinc_client.clients.rpc_client import RpcClient\n\n# Hostname or IP of the running BOINC client\nBOINC_HOSTNAME = "192.168.0.2"\n\n# Create an RPC client to connect to the BOINC socket\nrpc_client = RpcClient(hostname=BOINC_HOSTNAME)\nrpc_client.authenticate()\n\n# Create a BOINC client to interact with the RPC socket\nboinc_client = Boinc(rpc_client=rpc_client)\n```\n\n#### RPC Client options\nThe following options can be passed when creating an `RpcClient` instance\n\n| Argument   | Description                                                                | Required | Default |\n|------------|----------------------------------------------------------------------------|----------|---------|\n| `hostname` | Hostname or IP address of the BOINC client                                 | Yes      | None    |\n| `port`     | Exposed port of the BOINC client                                           | No       | 31416   |\n| `timeout`  | Seconds to wait for a successful connection to the RPC socket              | No       | 30      |\n| `password` | Password to authenticate to the BOINC client, required for most operations | No       | None    |\n\n#### Boinc options\nThe following options can be passed when creating a `Boinc` instance\n\n| Argument     | Description                        | Required | Default |\n|--------------|------------------------------------|----------|---------|\n| `rpc_client` | Instance of a configured RpcClient | Yes      | None    |\n\n### Interacting with Boinc\n\n* [Unauthorised Operations](docs/unauthorised.md)\n* [Project Operations](docs/project.md)\n\n## Contributors\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->',
     'author': 'Lewis England',
     'author_email': 'lewis2004@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `boinc_client-1.8.0/PKG-INFO` & `boinc_client-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boinc-client
-Version: 1.8.0
+Version: 1.9.0
 Summary: Python API for interacting with a BOINC client via RPC
 Author: Lewis England
 Author-email: lewis2004@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,14 +16,16 @@
 Project-URL: issues, https://github.com/SplinterHead/boinc-client/issues
 Description-Content-Type: text/markdown
 
 # BOINC Client
 
 ![Test and Release](https://github.com/SplinterHead/boinc-client/actions/workflows/test-and-release.yml/badge.svg)
 [![boinc-client](https://snyk.io/advisor/python/boinc-client/badge.svg)](https://snyk.io/advisor/python/boinc-client)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/boinc-client)
+
 
 Python native library for interacting with a BOINC client via RPC. This library has been designed to have consistent response types.
 
 ## Usage
 
 ### Setup
```

