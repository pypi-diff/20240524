# Comparing `tmp/pennylane-kq-0.0.8.tar.gz` & `tmp/pennylane-kq-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pennylane-kq-0.0.8.tar", last modified: Fri May 10 02:19:02 2024, max compression
+gzip compressed data, was "pennylane-kq-0.0.9.tar", last modified: Fri May 10 02:26:19 2024, max compression
```

## Comparing `pennylane-kq-0.0.8.tar` & `pennylane-kq-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-10 02:19:02.487699 pennylane-kq-0.0.8/
--rw-r--r--   0 ino        (501) staff       (20)     1335 2023-08-22 08:26:43.000000 pennylane-kq-0.0.8/LICENSE
--rw-r--r--   0 ino        (501) staff       (20)     1886 2024-05-10 02:19:02.487583 pennylane-kq-0.0.8/PKG-INFO
--rw-r--r--   0 ino        (501) staff       (20)     1554 2024-05-08 01:07:56.000000 pennylane-kq-0.0.8/README.md
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-10 02:19:02.486222 pennylane-kq-0.0.8/pennylane_kq/
--rw-r--r--   0 ino        (501) staff       (20)      293 2023-12-21 00:35:30.000000 pennylane-kq-0.0.8/pennylane_kq/__init__.py
--rw-r--r--   0 ino        (501) staff       (20)       97 2024-05-10 02:18:46.000000 pennylane-kq-0.0.8/pennylane_kq/_version.py
--rw-r--r--   0 ino        (501) staff       (20)     4621 2024-05-07 08:59:35.000000 pennylane-kq-0.0.8/pennylane_kq/kq_emulator.py
--rw-r--r--   0 ino        (501) staff       (20)     3479 2023-12-27 04:57:04.000000 pennylane-kq-0.0.8/pennylane_kq/kq_emulator_aws.py
--rw-r--r--   0 ino        (501) staff       (20)     3451 2023-12-27 04:56:48.000000 pennylane-kq-0.0.8/pennylane_kq/kq_hardware.py
--rw-r--r--   0 ino        (501) staff       (20)     3541 2024-05-07 08:44:16.000000 pennylane-kq-0.0.8/pennylane_kq/kq_local_emulator.py
--rw-r--r--   0 ino        (501) staff       (20)     3560 2024-05-10 02:16:32.000000 pennylane-kq-0.0.8/pennylane_kq/kq_remote_emulator.py
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-10 02:19:02.487412 pennylane-kq-0.0.8/pennylane_kq.egg-info/
--rw-r--r--   0 ino        (501) staff       (20)     1886 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/PKG-INFO
--rw-r--r--   0 ino        (501) staff       (20)      486 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/SOURCES.txt
--rw-r--r--   0 ino        (501) staff       (20)        1 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/dependency_links.txt
--rw-r--r--   0 ino        (501) staff       (20)      231 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/entry_points.txt
--rw-r--r--   0 ino        (501) staff       (20)        1 2023-11-13 13:51:28.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/not-zip-safe
--rw-r--r--   0 ino        (501) staff       (20)       22 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/requires.txt
--rw-r--r--   0 ino        (501) staff       (20)       13 2024-05-10 02:19:02.000000 pennylane-kq-0.0.8/pennylane_kq.egg-info/top_level.txt
--rw-r--r--   0 ino        (501) staff       (20)       38 2024-05-10 02:19:02.487740 pennylane-kq-0.0.8/setup.cfg
--rw-r--r--   0 ino        (501) staff       (20)     1113 2023-12-21 01:55:43.000000 pennylane-kq-0.0.8/setup.py
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-10 02:26:19.201333 pennylane-kq-0.0.9/
+-rw-r--r--   0 ino        (501) staff       (20)     1335 2023-08-22 08:26:43.000000 pennylane-kq-0.0.9/LICENSE
+-rw-r--r--   0 ino        (501) staff       (20)     1886 2024-05-10 02:26:19.201181 pennylane-kq-0.0.9/PKG-INFO
+-rw-r--r--   0 ino        (501) staff       (20)     1554 2024-05-08 01:07:56.000000 pennylane-kq-0.0.9/README.md
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-10 02:26:19.199731 pennylane-kq-0.0.9/pennylane_kq/
+-rw-r--r--   0 ino        (501) staff       (20)      353 2024-05-10 02:19:47.000000 pennylane-kq-0.0.9/pennylane_kq/__init__.py
+-rw-r--r--   0 ino        (501) staff       (20)       97 2024-05-10 02:25:46.000000 pennylane-kq-0.0.9/pennylane_kq/_version.py
+-rw-r--r--   0 ino        (501) staff       (20)     4621 2024-05-07 08:59:35.000000 pennylane-kq-0.0.9/pennylane_kq/kq_emulator.py
+-rw-r--r--   0 ino        (501) staff       (20)     3479 2023-12-27 04:57:04.000000 pennylane-kq-0.0.9/pennylane_kq/kq_emulator_aws.py
+-rw-r--r--   0 ino        (501) staff       (20)     3451 2023-12-27 04:56:48.000000 pennylane-kq-0.0.9/pennylane_kq/kq_hardware.py
+-rw-r--r--   0 ino        (501) staff       (20)     3541 2024-05-07 08:44:16.000000 pennylane-kq-0.0.9/pennylane_kq/kq_local_emulator.py
+-rw-r--r--   0 ino        (501) staff       (20)     3562 2024-05-10 02:21:49.000000 pennylane-kq-0.0.9/pennylane_kq/kq_remote_emulator.py
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-05-10 02:26:19.200932 pennylane-kq-0.0.9/pennylane_kq.egg-info/
+-rw-r--r--   0 ino        (501) staff       (20)     1886 2024-05-10 02:26:19.000000 pennylane-kq-0.0.9/pennylane_kq.egg-info/PKG-INFO
+-rw-r--r--   0 ino        (501) staff       (20)      486 2024-05-10 02:26:19.000000 pennylane-kq-0.0.9/pennylane_kq.egg-info/SOURCES.txt
+-rw-r--r--   0 ino        (501) staff       (20)        1 2024-05-10 02:26:19.000000 pennylane-kq-0.0.9/pennylane_kq.egg-info/dependency_links.txt
+-rw-r--r--   0 ino        (501) staff       (20)      292 2024-05-10 02:26:19.000000 pennylane-kq-0.0.9/pennylane_kq.egg-info/entry_points.txt
+-rw-r--r--   0 ino        (501) staff       (20)        1 2023-11-13 13:51:28.000000 pennylane-kq-0.0.9/pennylane_kq.egg-info/not-zip-safe
+-rw-r--r--   0 ino        (501) staff       (20)       22 2024-05-10 02:26:19.000000 pennylane-kq-0.0.9/pennylane_kq.egg-info/requires.txt
+-rw-r--r--   0 ino        (501) staff       (20)       13 2024-05-10 02:26:19.000000 pennylane-kq-0.0.9/pennylane_kq.egg-info/top_level.txt
+-rw-r--r--   0 ino        (501) staff       (20)       38 2024-05-10 02:26:19.201397 pennylane-kq-0.0.9/setup.cfg
+-rw-r--r--   0 ino        (501) staff       (20)     1181 2024-05-10 02:25:08.000000 pennylane-kq-0.0.9/setup.py
```

### Comparing `pennylane-kq-0.0.8/LICENSE` & `pennylane-kq-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.8/PKG-INFO` & `pennylane-kq-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-kq
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Pennylane plugin for KQ Cloud System
 Home-page: https://www.github.com/inojeon/pennylane-kq
 Author: Inho Jeon
 Author-email: inojeon@kisti.re.kr
 License: BSD-2
 Platform: UNKNOWN
 Provides: pennylane_kq
```

### Comparing `pennylane-kq-0.0.8/README.md` & `pennylane-kq-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.8/pennylane_kq/kq_emulator.py` & `pennylane-kq-0.0.9/pennylane_kq/kq_emulator.py`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.8/pennylane_kq/kq_emulator_aws.py` & `pennylane-kq-0.0.9/pennylane_kq/kq_emulator_aws.py`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.8/pennylane_kq/kq_hardware.py` & `pennylane-kq-0.0.9/pennylane_kq/kq_hardware.py`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.8/pennylane_kq/kq_local_emulator.py` & `pennylane-kq-0.0.9/pennylane_kq/kq_local_emulator.py`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.8/pennylane_kq/kq_remote_emulator.py` & `pennylane-kq-0.0.9/pennylane_kq/kq_remote_emulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 # import numpy as np
 
 import requests, json, time
 from pennylane import DeviceError, QubitDevice
 
 
-class KoreaQuantumLocalEmulator(QubitDevice):
+class KoreaQuantumRemoteEmulator(QubitDevice):
     """
     The base class for all devices that call to an external server.
     """
 
-    name = "Korea Quantum Local Emulator"
+    name = "Korea Quantum Remote Emulator"
     short_name = "kq.remote_emulator"
     pennylane_requires = ">=0.16.0"
     version = "0.0.1"
     author = "Inho Jeon"
 
     operations = {"PauliX", "RX", "CNOT", "RY", "RZ", "Hadamard"}
     observables = {"PauliZ", "PauliX", "PauliY"}
```

### Comparing `pennylane-kq-0.0.8/pennylane_kq.egg-info/PKG-INFO` & `pennylane-kq-0.0.9/pennylane_kq.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pennylane-kq
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Pennylane plugin for KQ Cloud System
 Home-page: https://www.github.com/inojeon/pennylane-kq
 Author: Inho Jeon
 Author-email: inojeon@kisti.re.kr
 License: BSD-2
 Platform: UNKNOWN
 Provides: pennylane_kq
```

### Comparing `pennylane-kq-0.0.8/setup.py` & `pennylane-kq-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 
 pennylane_devices_list = [
     "kq.emulator = pennylane_kq:KoreaQuantumEmulator",
     "kq.emulator.aws = pennylane_kq:KoreaQuantumEmulatorAWS",
     "kq.hardware = pennylane_kq:KoreaQuantumHardware",
     "kq.local_emulator = pennylane_kq:KoreaQuantumLocalEmulator",
+    "kq.remote_emulator = pennylane_kq:KoreaQuantumRemoteEmulator",
 ]
 
 # requirements = ["pennylane>=0.19,<0.30"]
 
 setup(
     name="pennylane-kq",
     version=version,
```

