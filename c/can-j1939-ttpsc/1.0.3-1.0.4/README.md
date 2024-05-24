# Comparing `tmp/can-j1939-ttpsc-1.0.3.tar.gz` & `tmp/can-j1939-ttpsc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "can-j1939-ttpsc-1.0.3.tar", last modified: Thu Apr 25 08:54:04 2024, max compression
+gzip compressed data, was "can-j1939-ttpsc-1.0.4.tar", last modified: Fri May 24 12:36:23 2024, max compression
```

## Comparing `can-j1939-ttpsc-1.0.3.tar` & `can-j1939-ttpsc-1.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-04-25 08:54:04.260985 can-j1939-ttpsc-1.0.3/
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1148 2023-10-25 10:48:29.000000 can-j1939-ttpsc-1.0.3/LICENSE
--rw-r--r--   0 molinaf   (1000) molinaf   (1000)     8173 2024-04-25 08:54:04.260985 can-j1939-ttpsc-1.0.3/PKG-INFO
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     7496 2023-10-25 12:36:45.000000 can-j1939-ttpsc-1.0.3/README.rst
-drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-04-25 08:54:04.248985 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/
--rw-r--r--   0 molinaf   (1000) molinaf   (1000)     8173 2024-04-25 08:54:04.000000 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/PKG-INFO
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      618 2024-04-25 08:54:04.000000 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/SOURCES.txt
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)        1 2024-04-25 08:54:04.000000 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/dependency_links.txt
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       46 2024-04-25 08:54:04.000000 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/requires.txt
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       19 2024-04-25 08:54:04.000000 can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/top_level.txt
-drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-04-25 08:54:04.256985 can-j1939-ttpsc-1.0.3/j1939/
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      327 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/__init__.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    14753 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/controller_application.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    11844 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/diagnostic_messages.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    14995 2023-09-28 10:57:27.000000 can-j1939-ttpsc-1.0.3/j1939/electronic_control_unit.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    28786 2024-04-13 10:34:02.000000 can-j1939-ttpsc-1.0.3/j1939/j1939_21.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    46754 2024-04-13 10:34:43.000000 can-j1939-ttpsc-1.0.3/j1939/j1939_22.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     6776 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/memory_access.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1839 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/message_id.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    10322 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/name.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     5323 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/j1939/parameter_group_number.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       22 2024-04-25 08:53:45.000000 can-j1939-ttpsc-1.0.3/j1939/version.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       67 2024-04-25 08:54:04.260985 can-j1939-ttpsc-1.0.3/setup.cfg
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1216 2023-10-25 12:10:42.000000 can-j1939-ttpsc-1.0.3/setup.py
-drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-04-25 08:54:04.256985 can-j1939-ttpsc-1.0.3/test/
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     3786 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/test/test_ca.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     6705 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/test/test_ecu.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     4278 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.3/test/test_memory_access.py
-drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-04-25 08:54:04.260985 can-j1939-ttpsc-1.0.3/test_helpers/
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)        0 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.3/test_helpers/__init__.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      168 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.3/test_helpers/conftest.py
--rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     5279 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.3/test_helpers/feeder.py
+drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-05-24 12:36:23.763035 can-j1939-ttpsc-1.0.4/
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1148 2023-10-25 10:48:29.000000 can-j1939-ttpsc-1.0.4/LICENSE
+-rw-r--r--   0 molinaf   (1000) molinaf   (1000)     8173 2024-05-24 12:36:23.763035 can-j1939-ttpsc-1.0.4/PKG-INFO
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     7496 2023-10-25 12:36:45.000000 can-j1939-ttpsc-1.0.4/README.rst
+drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-05-24 12:36:23.751035 can-j1939-ttpsc-1.0.4/can_j1939_ttpsc.egg-info/
+-rw-r--r--   0 molinaf   (1000) molinaf   (1000)     8173 2024-05-24 12:36:23.000000 can-j1939-ttpsc-1.0.4/can_j1939_ttpsc.egg-info/PKG-INFO
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      618 2024-05-24 12:36:23.000000 can-j1939-ttpsc-1.0.4/can_j1939_ttpsc.egg-info/SOURCES.txt
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)        1 2024-05-24 12:36:23.000000 can-j1939-ttpsc-1.0.4/can_j1939_ttpsc.egg-info/dependency_links.txt
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       46 2024-05-24 12:36:23.000000 can-j1939-ttpsc-1.0.4/can_j1939_ttpsc.egg-info/requires.txt
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       19 2024-05-24 12:36:23.000000 can-j1939-ttpsc-1.0.4/can_j1939_ttpsc.egg-info/top_level.txt
+drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-05-24 12:36:23.759035 can-j1939-ttpsc-1.0.4/j1939/
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      327 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.4/j1939/__init__.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    14753 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.4/j1939/controller_application.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    11844 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.4/j1939/diagnostic_messages.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    14995 2023-09-28 10:57:27.000000 can-j1939-ttpsc-1.0.4/j1939/electronic_control_unit.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    30042 2024-05-21 09:43:51.000000 can-j1939-ttpsc-1.0.4/j1939/j1939_21.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    46754 2024-04-13 10:34:43.000000 can-j1939-ttpsc-1.0.4/j1939/j1939_22.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     6776 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.4/j1939/memory_access.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1839 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.4/j1939/message_id.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)    10322 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.4/j1939/name.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     5323 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.4/j1939/parameter_group_number.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       22 2024-05-21 09:44:40.000000 can-j1939-ttpsc-1.0.4/j1939/version.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)       67 2024-05-24 12:36:23.763035 can-j1939-ttpsc-1.0.4/setup.cfg
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     1216 2023-10-25 12:10:42.000000 can-j1939-ttpsc-1.0.4/setup.py
+drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-05-24 12:36:23.759035 can-j1939-ttpsc-1.0.4/test/
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     3786 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.4/test/test_ca.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     6705 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.4/test/test_ecu.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     4278 2023-09-28 10:09:24.000000 can-j1939-ttpsc-1.0.4/test/test_memory_access.py
+drwxrwxr-x   0 molinaf   (1000) molinaf   (1000)        0 2024-05-24 12:36:23.763035 can-j1939-ttpsc-1.0.4/test_helpers/
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)        0 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.4/test_helpers/__init__.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)      168 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.4/test_helpers/conftest.py
+-rw-rw-r--   0 molinaf   (1000) molinaf   (1000)     5279 2023-10-25 11:46:34.000000 can-j1939-ttpsc-1.0.4/test_helpers/feeder.py
```

### Comparing `can-j1939-ttpsc-1.0.3/LICENSE` & `can-j1939-ttpsc-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/PKG-INFO` & `can-j1939-ttpsc-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: can-j1939-ttpsc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Fork of SAE J1939 stack implementation, originally created by Juergen Heilgemeir
 Home-page: https://github.com/ttpscmolinaf/python-can-j1939
 Author: TTPSC
 License: MIT
 Keywords: CAN SAE J1939 J1939-FD J1939-22
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `can-j1939-ttpsc-1.0.3/README.rst` & `can-j1939-ttpsc-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/PKG-INFO` & `can-j1939-ttpsc-1.0.4/can_j1939_ttpsc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: can-j1939-ttpsc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Fork of SAE J1939 stack implementation, originally created by Juergen Heilgemeir
 Home-page: https://github.com/ttpscmolinaf/python-can-j1939
 Author: TTPSC
 License: MIT
 Keywords: CAN SAE J1939 J1939-FD J1939-22
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `can-j1939-ttpsc-1.0.3/can_j1939_ttpsc.egg-info/SOURCES.txt` & `can-j1939-ttpsc-1.0.4/can_j1939_ttpsc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/j1939/controller_application.py` & `can-j1939-ttpsc-1.0.4/j1939/controller_application.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/j1939/diagnostic_messages.py` & `can-j1939-ttpsc-1.0.4/j1939/diagnostic_messages.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/j1939/electronic_control_unit.py` & `can-j1939-ttpsc-1.0.4/j1939/electronic_control_unit.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/j1939/j1939_21.py` & `can-j1939-ttpsc-1.0.4/j1939/j1939_21.py`

 * *Files 2% similar despite different names*

```diff
@@ -708,24 +708,58 @@
             seconds.
             Where possible this will be timestamped in hardware.
         """
 
         mid = MessageId(can_id=can_id)
         pgn = ParameterGroupNumber()
         pgn.from_message_id(mid)
-        # Direct broadcast
-        # Removed peer to peer logic, we are interested in sniffing only.
-        """
-        As of commit https://github.com/juergenH87/python-can-j1939/commit/739c1c0baf24c07cdf32e96289595954200782b9
-        It was added the channel parameter for the notifier.
-        """
-        # Added channel param
-        self.__notify_subscribers(
-            mid.priority,
-            pgn.value,
-            mid.source_address,
-            ParameterGroupNumber.Address.GLOBAL,
-            timestamp,
-            data,
-            channel,
-        )
-        return
+
+        if pgn.is_pdu2_format:
+            # direct broadcast
+            # Added channel param
+            self.__notify_subscribers(
+                mid.priority,
+                pgn.value,
+                mid.source_address,
+                ParameterGroupNumber.Address.GLOBAL,
+                timestamp,
+                data,
+                channel,
+            )
+            return
+
+        # peer to peer
+        # pdu_specific is destination Address
+        pgn_value = pgn.value & 0x1FF00
+        dest_address = pgn.pdu_specific  # may be Address.GLOBAL
+
+        # iterate all CAs to check if we have to handle this destination address
+        if dest_address != ParameterGroupNumber.Address.GLOBAL:
+            for ca in self._cas:
+                if ca.message_acceptable(dest_address):
+                    reject = False
+                    break
+
+        if pgn_value == ParameterGroupNumber.PGN.ADDRESSCLAIM:
+            for ca in self._cas:
+                ca._process_addressclaim(mid, data, timestamp)
+        elif pgn_value == ParameterGroupNumber.PGN.REQUEST:
+            for ca in self._cas:
+                if ca.message_acceptable(dest_address):
+                    ca._process_request(mid, dest_address, data, timestamp)
+        elif pgn_value == ParameterGroupNumber.PGN.TP_CM:
+            self._process_tp_cm(mid, dest_address, data, timestamp, channel)
+        elif pgn_value == ParameterGroupNumber.PGN.DATATRANSFER:
+            self._process_tp_dt(mid, dest_address, data, timestamp, channel)
+        else:
+
+            # Added channel param
+            self.__notify_subscribers(
+                mid.priority,
+                pgn.value,
+                mid.source_address,
+                dest_address,
+                timestamp,
+                data,
+                channel,
+            )
+            return
```

### Comparing `can-j1939-ttpsc-1.0.3/j1939/j1939_22.py` & `can-j1939-ttpsc-1.0.4/j1939/j1939_22.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/j1939/memory_access.py` & `can-j1939-ttpsc-1.0.4/j1939/memory_access.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/j1939/message_id.py` & `can-j1939-ttpsc-1.0.4/j1939/message_id.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/j1939/name.py` & `can-j1939-ttpsc-1.0.4/j1939/name.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/j1939/parameter_group_number.py` & `can-j1939-ttpsc-1.0.4/j1939/parameter_group_number.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/setup.py` & `can-j1939-ttpsc-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/test/test_ca.py` & `can-j1939-ttpsc-1.0.4/test/test_ca.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/test/test_ecu.py` & `can-j1939-ttpsc-1.0.4/test/test_ecu.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/test/test_memory_access.py` & `can-j1939-ttpsc-1.0.4/test/test_memory_access.py`

 * *Files identical despite different names*

### Comparing `can-j1939-ttpsc-1.0.3/test_helpers/feeder.py` & `can-j1939-ttpsc-1.0.4/test_helpers/feeder.py`

 * *Files identical despite different names*

