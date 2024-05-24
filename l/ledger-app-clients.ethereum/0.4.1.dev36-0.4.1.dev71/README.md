# Comparing `tmp/ledger_app_clients.ethereum-0.4.1.dev36.tar.gz` & `tmp/ledger_app_clients_ethereum-0.4.1.dev71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledger_app_clients.ethereum-0.4.1.dev36.tar", last modified: Thu Apr 11 16:30:41 2024, max compression
+gzip compressed data, was "ledger_app_clients_ethereum-0.4.1.dev71.tar", last modified: Fri May  3 11:16:27 2024, max compression
```

## Comparing `ledger_app_clients.ethereum-0.4.1.dev36.tar` & `ledger_app_clients_ethereum-0.4.1.dev71.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.955359 ledger_app_clients.ethereum-0.4.1.dev36/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.955359 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12851 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/command_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/eip712/
--rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/eip712/InputData.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/eip712/struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain/cal.pem
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain/domain_name.pem
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain/nft.pem
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain/set_plugin.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/tlv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-11 16:30:34.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:30:41.959359 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 16:30:41.000000 ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:16:27.768509 ledger_app_clients_ethereum-0.4.1.dev71/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-03 11:16:27.768509 ledger_app_clients_ethereum-0.4.1.dev71/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:16:27.768509 ledger_app_clients_ethereum-0.4.1.dev71/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:16:27.764509 ledger_app_clients_ethereum-0.4.1.dev71/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:16:27.764509 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:16:27.764509 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-03 11:16:27.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12851 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/command_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:16:27.764509 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/eip712/
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/eip712/InputData.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/eip712/struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:16:27.768509 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/keychain/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/keychain/cal.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/keychain/domain_name.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/keychain/nft.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/keychain/set_plugin.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/tlv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-03 11:16:21.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:16:27.768509 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients.ethereum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-03 11:16:27.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients.ethereum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-03 11:16:27.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:16:27.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients.ethereum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 11:16:27.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients.ethereum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 11:16:27.000000 ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients.ethereum.egg-info/top_level.txt
```

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/CHANGELOG.md` & `ledger_app_clients_ethereum-0.4.1.dev71/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## [0.4.1] - 2024-04-05
+## [0.4.1] - 2024-04-15
 
 ### Added
 
 - Add new function `send_raw`, allowing to send a raw payload APDU
 - Add new error code definition
 
+### Fixed
+
+- Encoding of EIP-712 bytes elements
+
 ## [0.4.0] - 2024-04-03
 
 ### Added
 
 - Changed `sync` functions of the client to not use an `async` syntax anymore
 
 ## [0.3.1] - 2024-03-12
```

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/PKG-INFO` & `ledger_app_clients_ethereum-0.4.1.dev71/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledger_app_clients.ethereum
-Version: 0.4.1.dev36
+Version: 0.4.1.dev71
 Summary: Ledger Ethereum Python client
 Author-email: Ledger <hello@ledger.fr>
 Project-URL: Home, https://github.com/LedgerHQ/app-ethereum
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/pyproject.toml` & `ledger_app_clients_ethereum-0.4.1.dev71/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/client.py` & `ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/client.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/command_builder.py` & `ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/command_builder.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/eip712/InputData.py` & `ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/eip712/InputData.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import hashlib
 import json
 import re
 import signal
 import sys
 import copy
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Optional, Union
+import struct
 
 from client import keychain
 from client.client import EthAppClient, EIP712FieldType
 
 
 # global variables
 app_client: EthAppClient = None
@@ -114,77 +115,71 @@
                                                         typesize,
                                                         array_lvls,
                                                         keyname):
         pass
     return (typename, type_enum, typesize, array_lvls)
 
 
-def encode_integer(value, typesize):
-    data = bytearray()
-
+def encode_integer(value: Union[str | int], typesize: int) -> bytes:
     # Some are already represented as integers in the JSON, but most as strings
     if isinstance(value, str):
-        base = 10
-        if value.startswith("0x"):
-            base = 16
-        value = int(value, base)
+        value = int(value, 0)
 
     if value == 0:
-        data.append(0)
+        data = b'\x00'
     else:
-        if value < 0:  # negative number, send it as unsigned
-            mask = 0
-            for i in range(typesize):  # make a mask as big as the typesize
-                mask = (mask << 8) | 0xff
-            value &= mask
-        while value > 0:
-            data.append(value & 0xff)
-            value >>= 8
-        data.reverse()
+        # biggest uint type accepted by struct.pack
+        uint64_mask = 0xffffffffffffffff
+        data = struct.pack(">QQQQ",
+                           (value >> 192) & uint64_mask,
+                           (value >> 128) & uint64_mask,
+                           (value >> 64) & uint64_mask,
+                           value & uint64_mask)
+        data = data[len(data) - typesize:]
+        data = data.lstrip(b'\x00')
     return data
 
 
-def encode_int(value, typesize):
+def encode_int(value: str, typesize: int) -> bytes:
     return encode_integer(value, typesize)
 
 
-def encode_uint(value, typesize):
+def encode_uint(value: str, typesize: int) -> bytes:
     return encode_integer(value, typesize)
 
 
-def encode_hex_string(value, size):
-    data = bytearray()
-    value = value[2:]  # skip 0x
-    byte_idx = 0
-    while byte_idx < size:
-        data.append(int(value[(byte_idx * 2):(byte_idx * 2 + 2)], 16))
-        byte_idx += 1
-    return data
+def encode_hex_string(value: str, size: int) -> bytes:
+    assert value.startswith("0x")
+    value = value[2:]
+    if len(value) < (size * 2):
+        value = value.rjust(size * 2, "0")
+    assert len(value) == (size * 2)
+    return bytes.fromhex(value)
 
 
-def encode_address(value, typesize):
+def encode_address(value: str, typesize: int) -> bytes:
     return encode_hex_string(value, 20)
 
 
-def encode_bool(value, typesize):
-    return encode_integer(value, typesize)
+def encode_bool(value: str, typesize: int) -> bytes:
+    return encode_integer(value, 1)
 
 
-def encode_string(value, typesize):
+def encode_string(value: str, typesize: int) -> bytes:
     data = bytearray()
     for char in value:
         data.append(ord(char))
     return data
 
 
-def encode_bytes_fix(value, typesize):
+def encode_bytes_fix(value: str, typesize: int) -> bytes:
     return encode_hex_string(value, typesize)
 
 
-def encode_bytes_dyn(value, typesize):
+def encode_bytes_dyn(value: str, typesize: int) -> bytes:
     # length of the value string
     # - the length of 0x (2)
     # / by the length of one byte in a hex string (2)
     return encode_hex_string(value, int((len(value) - 2) / 2))
 
 
 # set functions for each type
```

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/keychain.py` & `ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/keychain.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/response_parser.py` & `ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/response_parser.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/settings.py` & `ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/settings.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/tlv.py` & `ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/tlv.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients/ethereum/utils.py` & `ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients/ethereum/utils.py`

 * *Files identical despite different names*

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/PKG-INFO` & `ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients.ethereum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ledger_app_clients.ethereum
-Version: 0.4.1.dev36
+Version: 0.4.1.dev71
 Summary: Ledger Ethereum Python client
 Author-email: Ledger <hello@ledger.fr>
 Project-URL: Home, https://github.com/LedgerHQ/app-ethereum
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ledger_app_clients.ethereum-0.4.1.dev36/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt` & `ledger_app_clients_ethereum-0.4.1.dev71/src/ledger_app_clients.ethereum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

