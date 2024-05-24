# Comparing `tmp/sorunlib-0.1.8.tar.gz` & `tmp/sorunlib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sorunlib-0.1.8.tar", last modified: Fri Aug 11 17:29:36 2023, max compression
+gzip compressed data, was "sorunlib-0.1.9.tar", last modified: Mon Oct 23 21:11:36 2023, max compression
```

## Comparing `sorunlib-0.1.8.tar` & `sorunlib-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 17:29:36.626143 sorunlib-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-11 17:29:21.000000 sorunlib-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-11 17:29:21.000000 sorunlib-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-08-11 17:29:36.626143 sorunlib-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-08-11 17:29:21.000000 sorunlib-0.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-11 17:29:36.626143 sorunlib-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-11 17:29:21.000000 sorunlib-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 17:29:36.622142 sorunlib-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 17:29:36.626143 sorunlib-0.1.8/src/sorunlib/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-11 17:29:21.000000 sorunlib-0.1.8/src/sorunlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-11 17:29:21.000000 sorunlib-0.1.8/src/sorunlib/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-11 17:29:36.626143 sorunlib-0.1.8/src/sorunlib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-11 17:29:21.000000 sorunlib-0.1.8/src/sorunlib/acu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-08-11 17:29:21.000000 sorunlib-0.1.8/src/sorunlib/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-11 17:29:21.000000 sorunlib-0.1.8/src/sorunlib/seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-08-11 17:29:21.000000 sorunlib-0.1.8/src/sorunlib/smurf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-08-11 17:29:21.000000 sorunlib-0.1.8/src/sorunlib/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 17:29:36.626143 sorunlib-0.1.8/src/sorunlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-08-11 17:29:36.000000 sorunlib-0.1.8/src/sorunlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-11 17:29:36.000000 sorunlib-0.1.8/src/sorunlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-11 17:29:36.000000 sorunlib-0.1.8/src/sorunlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-11 17:29:36.000000 sorunlib-0.1.8/src/sorunlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-11 17:29:36.000000 sorunlib-0.1.8/src/sorunlib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 17:29:36.626143 sorunlib-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-11 17:29:21.000000 sorunlib-0.1.8/tests/test__internal.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-11 17:29:21.000000 sorunlib-0.1.8/tests/test_acu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-08-11 17:29:21.000000 sorunlib-0.1.8/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-11 17:29:21.000000 sorunlib-0.1.8/tests/test_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-11 17:29:21.000000 sorunlib-0.1.8/tests/test_smurf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-08-11 17:29:21.000000 sorunlib-0.1.8/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    81180 2023-08-11 17:29:21.000000 sorunlib-0.1.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 21:11:36.029544 sorunlib-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-10-23 21:11:21.000000 sorunlib-0.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-10-23 21:11:21.000000 sorunlib-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2023-10-23 21:11:36.029544 sorunlib-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-10-23 21:11:21.000000 sorunlib-0.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-10-23 21:11:36.029544 sorunlib-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2023-10-23 21:11:21.000000 sorunlib-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 21:11:36.025544 sorunlib-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 21:11:36.029544 sorunlib-0.1.9/src/sorunlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2023-10-23 21:11:21.000000 sorunlib-0.1.9/src/sorunlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-10-23 21:11:21.000000 sorunlib-0.1.9/src/sorunlib/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2023-10-23 21:11:36.029544 sorunlib-0.1.9/src/sorunlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2023-10-23 21:11:21.000000 sorunlib-0.1.9/src/sorunlib/acu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2023-10-23 21:11:21.000000 sorunlib-0.1.9/src/sorunlib/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2023-10-23 21:11:21.000000 sorunlib-0.1.9/src/sorunlib/seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2023-10-23 21:11:21.000000 sorunlib-0.1.9/src/sorunlib/smurf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2023-10-23 21:11:21.000000 sorunlib-0.1.9/src/sorunlib/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 21:11:36.025544 sorunlib-0.1.9/src/sorunlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2023-10-23 21:11:36.000000 sorunlib-0.1.9/src/sorunlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2023-10-23 21:11:36.000000 sorunlib-0.1.9/src/sorunlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 21:11:36.000000 sorunlib-0.1.9/src/sorunlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-23 21:11:36.000000 sorunlib-0.1.9/src/sorunlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-23 21:11:36.000000 sorunlib-0.1.9/src/sorunlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 21:11:36.025544 sorunlib-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2023-10-23 21:11:21.000000 sorunlib-0.1.9/tests/test__internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-10-23 21:11:21.000000 sorunlib-0.1.9/tests/test_acu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2023-10-23 21:11:21.000000 sorunlib-0.1.9/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-10-23 21:11:21.000000 sorunlib-0.1.9/tests/test_seq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2023-10-23 21:11:21.000000 sorunlib-0.1.9/tests/test_smurf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2023-10-23 21:11:21.000000 sorunlib-0.1.9/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81180 2023-10-23 21:11:21.000000 sorunlib-0.1.9/versioneer.py
```

### Comparing `sorunlib-0.1.8/LICENSE.txt` & `sorunlib-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/PKG-INFO` & `sorunlib-0.1.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sorunlib
-Version: 0.1.8
+Version: 0.1.9
 Summary: OCS Control Programs for running the observatory.
 Home-page: https://github.com/simonsobs/sorunlib
 Project-URL: Source Code, https://github.com/simonsobs/sorunlib
 Project-URL: Documentation, https://sorunlib.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/simonsobs/sorunlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,17 +13,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: ocs==0.10.2
 Provides-Extra: tests
+Requires-Dist: pytest>=7.0.0; extra == "tests"
+Requires-Dist: pytest-cov>=3.0.0; extra == "tests"
 Provides-Extra: docs
-License-File: LICENSE.txt
+Requires-Dist: sphinx>=5.3.0; extra == "docs"
+Requires-Dist: sphinx_rtd_theme>=1.1.1; extra == "docs"
 
 ========
 sorunlib
 ========
 
 .. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/sorunlib/pytest.yml?branch=main
     :target: https://github.com/simonsobs/sorunlib/actions?query=workflow%3A%22Run+Tests%22
```

### Comparing `sorunlib-0.1.8/README.rst` & `sorunlib-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/setup.py` & `sorunlib-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/src/sorunlib/__init__.py` & `sorunlib-0.1.9/src/sorunlib/__init__.py`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/src/sorunlib/_internal.py` & `sorunlib-0.1.9/src/sorunlib/_internal.py`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/src/sorunlib/commands.py` & `sorunlib-0.1.9/src/sorunlib/commands.py`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/src/sorunlib/seq.py` & `sorunlib-0.1.9/src/sorunlib/seq.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import sorunlib as run
 from sorunlib._internal import check_response
 
 
 OP_TIMEOUT = 60
 
 
-def scan(description, stop_time, width, tag=None):
+def scan(description, stop_time, width, az_drift=0, tag=None, subtype=None):
     """Run a constant elevation scan, collecting detector data.
 
     Args:
         description (str): Description of the field/object being scanned.
         stop_time (str): Time in ISO format to scan until, i.e.
             "2022-06-21T15:58:00"
         width (float): Scan width in azimuth. The scan will start at the
             current position and move in the positive azimuth direction.
+        az_drift (float): Drift velocity in deg/s, causing scan extrema to move
+            accordingly.
         tag (str, optional): Tag or comma-separated listed of tags to attach to
             the operation. Passed through to the smurf stream command.
+        subtype (str, optional): Operation subtype used to tag the stream.
 
     """
     # Enable SMuRF streams
-    run.smurf.stream('on', tag=tag)
+    run.smurf.stream('on', subtype=subtype, tag=tag)
 
     try:
         # Grab current telescope position
         resp = run.CLIENTS['acu'].monitor.status()
         az = resp.session['data']['StatusDetailed']['Azimuth current position']
         el = resp.session['data']['StatusDetailed']['Elevation current position']
 
         # Start telescope motion
+        # az_speed and az_accel assumed from ACU defaults
+        # Can be modified by acu.set_scan_params()
         resp = run.CLIENTS['acu'].generate_scan.start(az_endpoint1=az,
                                                       az_endpoint2=az + width,
-                                                      az_speed=2,
-                                                      az_accel=2.0,
                                                       el_endpoint1=el,
                                                       el_endpoint2=el,
-                                                      el_speed=0)
+                                                      el_speed=0,
+                                                      az_drift=az_drift)
 
         if not resp.session:
             raise Exception(f"Generate Scan failed to start:\n  {resp}")
 
         # Wait until stop time
         run.commands.wait_until(stop_time)
     finally:
```

### Comparing `sorunlib-0.1.8/src/sorunlib/util.py` & `sorunlib-0.1.9/src/sorunlib/util.py`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/src/sorunlib.egg-info/PKG-INFO` & `sorunlib-0.1.9/src/sorunlib.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sorunlib
-Version: 0.1.8
+Version: 0.1.9
 Summary: OCS Control Programs for running the observatory.
 Home-page: https://github.com/simonsobs/sorunlib
 Project-URL: Source Code, https://github.com/simonsobs/sorunlib
 Project-URL: Documentation, https://sorunlib.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/simonsobs/sorunlib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -13,17 +13,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: ocs==0.10.2
 Provides-Extra: tests
+Requires-Dist: pytest>=7.0.0; extra == "tests"
+Requires-Dist: pytest-cov>=3.0.0; extra == "tests"
 Provides-Extra: docs
-License-File: LICENSE.txt
+Requires-Dist: sphinx>=5.3.0; extra == "docs"
+Requires-Dist: sphinx_rtd_theme>=1.1.1; extra == "docs"
 
 ========
 sorunlib
 ========
 
 .. image:: https://img.shields.io/github/actions/workflow/status/simonsobs/sorunlib/pytest.yml?branch=main
     :target: https://github.com/simonsobs/sorunlib/actions?query=workflow%3A%22Run+Tests%22
```

### Comparing `sorunlib-0.1.8/src/sorunlib.egg-info/SOURCES.txt` & `sorunlib-0.1.9/src/sorunlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/tests/test__internal.py` & `sorunlib-0.1.9/tests/test__internal.py`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/tests/test_commands.py` & `sorunlib-0.1.9/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/tests/test_seq.py` & `sorunlib-0.1.9/tests/test_seq.py`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/tests/test_smurf.py` & `sorunlib-0.1.9/tests/test_acu.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,78 @@
 import os
 os.environ["OCS_CONFIG_DIR"] = "./test_util/"
 
+import pytest
+
 from unittest.mock import MagicMock, patch
 
-from sorunlib import smurf
+import ocs
+from ocs.ocs_client import OCSReply
+from sorunlib import acu
 
+from util import create_session
 
-def _mock_smurf_client(instance_id):
-    smurf = MagicMock()
-    smurf.instance_id = instance_id
 
-    return smurf
+def create_acu_client(platform_type):
+    """Create an ACU client with mock monitor Process session.data.
 
+    Args:
+        platform_type (str): Either 'satp' or 'ccat'.
 
-def mocked_clients(test_mode):
-    smurf_ids = ['smurf1', 'smurf2', 'smurf3']
-    smurfs = [_mock_smurf_client(id_) for id_ in smurf_ids]
+    """
+    acu_client = MagicMock()
+    session = create_session('monitor')
+    session.data = {'PlatformType': platform_type}
+    reply = OCSReply(ocs.OK, 'msg', session.encoded())
+    acu_client.monitor.status = MagicMock(return_value=reply)
 
-    clients = {'acu': MagicMock(),
-               'smurf': smurfs}
-
-    return clients
+    return acu_client
 
 
-@patch('sorunlib.create_clients', mocked_clients)
-def test_set_targets():
-    smurf.run.initialize(test_mode=True)
-    smurf.set_targets(['smurf1'])
-    assert len(smurf.run.CLIENTS['smurf']) == 1
-    assert smurf.run.CLIENTS['smurf'][0].instance_id == 'smurf1'
-
-
-@patch('sorunlib.create_clients', mocked_clients)
-def test_bias_step():
-    smurf.run.initialize(test_mode=True)
-    smurf.bias_step()
-    for client in smurf.run.CLIENTS['smurf']:
-        client.take_bias_steps.start.assert_called_once()
-
-
-@patch('sorunlib.create_clients', mocked_clients)
-def test_iv_curve():
-    smurf.run.initialize(test_mode=True)
-    smurf.iv_curve()
-    for client in smurf.run.CLIENTS['smurf']:
-        client.take_iv.start.assert_called_once()
-
+def mocked_clients(test_mode):
+    clients = {'acu': MagicMock(),
+               'smurf': [MagicMock(), MagicMock(), MagicMock()]}
 
-@patch('sorunlib.create_clients', mocked_clients)
-def test_uxm_setup():
-    smurf.run.initialize(test_mode=True)
-    smurf.uxm_setup()
-    for client in smurf.run.CLIENTS['smurf']:
-        client.uxm_setup.start.assert_called_once()
+    return clients
 
 
 @patch('sorunlib.create_clients', mocked_clients)
-def test_uxm_relock():
-    smurf.run.initialize(test_mode=True)
-    smurf.uxm_relock()
-    for client in smurf.run.CLIENTS['smurf']:
-        client.uxm_relock.start.assert_called_once()
+def test_move_to():
+    acu.run.initialize(test_mode=True)
+    acu.move_to(180, 60)
+    acu.run.CLIENTS['acu'].go_to.assert_called_with(az=180, el=60)
 
 
 @patch('sorunlib.create_clients', mocked_clients)
-def test_bias_dets():
-    smurf.run.initialize(test_mode=True)
-    smurf.bias_dets()
-    for client in smurf.run.CLIENTS['smurf']:
-        client.bias_dets.start.assert_called_once()
+def test_set_boresight():
+    acu.run.initialize(test_mode=True)
+    acu.run.CLIENTS['acu'] = create_acu_client('satp')
+    acu.set_boresight(20)
+    acu.run.CLIENTS['acu'].set_boresight.assert_called_with(target=20)
 
 
 @patch('sorunlib.create_clients', mocked_clients)
-def test_bgmap():
-    smurf.run.initialize(test_mode=True)
-    smurf.take_bgmap()
-    for client in smurf.run.CLIENTS['smurf']:
-        client.take_bgmap.start.assert_called_once()
+def test_set_boresight_lat():
+    acu.run.initialize(test_mode=True)
+    acu.run.CLIENTS['acu'] = create_acu_client('ccat')
+    with pytest.raises(RuntimeError):
+        acu.set_boresight(20)
 
 
 @patch('sorunlib.create_clients', mocked_clients)
-def test_take_noise():
-    smurf.run.initialize(test_mode=True)
-    smurf.take_noise()
-    for client in smurf.run.CLIENTS['smurf']:
-        client.take_noise.start.assert_called_once()
+def test_move_to_failed():
+    acu.run.initialize()
+    mocked_response = OCSReply(
+        0, 'msg', {'success': False, 'op_name': 'go_to'})
+    acu.run.CLIENTS['acu'].go_to.side_effect = [mocked_response]
+    with pytest.raises(RuntimeError):
+        acu.move_to(180, 90)
 
 
 @patch('sorunlib.create_clients', mocked_clients)
-def test_stream():
-    smurf.run.initialize(test_mode=True)
-    smurf.stream(state='on')
-    for client in smurf.run.CLIENTS['smurf']:
-        client.stream.start.assert_called_once()
+def test_set_scan_params():
+    acu.run.initialize(test_mode=True)
+    acu.set_scan_params(az_speed=2, az_accel=2, reset=True)
+    acu.run.CLIENTS['acu'].set_scan_params.assert_called_with(
+        az_speed=2,
+        az_accel=2,
+        reset=True)
```

### Comparing `sorunlib-0.1.8/tests/test_util.py` & `sorunlib-0.1.9/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `sorunlib-0.1.8/versioneer.py` & `sorunlib-0.1.9/versioneer.py`

 * *Files identical despite different names*

