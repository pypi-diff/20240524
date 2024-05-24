# Comparing `tmp/openobd_protocol-0.13.0.tar.gz` & `tmp/openobd_protocol-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd_protocol-0.13.0.tar", last modified: Tue May 21 09:52:46 2024, max compression
+gzip compressed data, was "openobd_protocol-0.14.0.tar", last modified: Fri May 24 10:14:20 2024, max compression
```

## Comparing `openobd_protocol-0.13.0.tar` & `openobd_protocol-0.14.0.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.928763 openobd_protocol-0.13.0/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2457 2024-05-21 09:52:46.928763 openobd_protocol-0.13.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1895 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 09:52:46.928763 openobd_protocol-0.13.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.913763 openobd_protocol-0.13.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.919763 openobd_protocol-0.13.0/src/openobd_protocol/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/Authentication_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/Authentication_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1359 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/BasicResponse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/BasicResponse_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5065 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/BusConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/BusConfiguration_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.922763 openobd_protocol-0.13.0/src/openobd_protocol/CAN/
--rw-r--r--   0 root         (0) root         (0)     1978 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/CAN/CanServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      462 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/CAN/CanServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2751 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2565 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/CAN/Isotp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2400 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/CAN/Isotp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2349 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      405 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8395 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.924763 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/
--rw-r--r--   0 root         (0) root         (0)     2861 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/SessionServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    15019 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2778 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/Session_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2735 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/SessionController/Session_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1712 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/Status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/Status_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.927763 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/
--rw-r--r--   0 root         (0) root         (0)     1748 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2973 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterface_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4208 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-21 09:52:42.000000 openobd_protocol-0.13.0/src/openobd_protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 09:52:46.927763 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-05-21 09:52:46.000000 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1610 2024-05-21 09:52:46.000000 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 09:52:46.000000 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-05-21 09:52:46.000000 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-21 09:52:46.000000 openobd_protocol-0.13.0/src/openobd_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:14:20.920455 openobd_protocol-0.14.0/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-24 10:14:20.920455 openobd_protocol-0.14.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 10:14:20.920455 openobd_protocol-0.14.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:14:20.901454 openobd_protocol-0.14.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:14:20.908455 openobd_protocol-0.14.0/src/openobd_protocol/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/Authentication_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/Authentication_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/BasicResponse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/BasicResponse_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/BusConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/BusConfiguration_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:14:20.911455 openobd_protocol-0.14.0/src/openobd_protocol/CAN/
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/CAN/CanServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      462 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/CAN/CanServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/CAN/Isotp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/CAN/Isotp_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:14:20.914455 openobd_protocol-0.14.0/src/openobd_protocol/ConnectionMonitor/
+-rw-r--r--   0 root         (0) root         (0)     1455 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/ConnectionMonitor/ConnectionInformation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      728 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/ConnectionMonitor/ConnectionInformation_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2024 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/ConnectionMonitor/ConnectionMonitorServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      307 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/ConnectionMonitor/ConnectionMonitorServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5198 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/ConnectionMonitor/ConnectionMonitorServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8395 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:14:20.916455 openobd_protocol-0.14.0/src/openobd_protocol/SessionController/
+-rw-r--r--   0 root         (0) root         (0)     2861 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/SessionController/SessionServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    15019 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/SessionController/Session_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/SessionController/Session_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/Status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/Status_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:14:20.919455 openobd_protocol-0.14.0/src/openobd_protocol/UserInterface/
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/UserInterface/UserInterface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-24 10:14:16.000000 openobd_protocol-0.14.0/src/openobd_protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 10:14:20.919455 openobd_protocol-0.14.0/src/openobd_protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-24 10:14:20.000000 openobd_protocol-0.14.0/src/openobd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-05-24 10:14:20.000000 openobd_protocol-0.14.0/src/openobd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 10:14:20.000000 openobd_protocol-0.14.0/src/openobd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-05-24 10:14:20.000000 openobd_protocol-0.14.0/src/openobd_protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-24 10:14:20.000000 openobd_protocol-0.14.0/src/openobd_protocol.egg-info/top_level.txt
```

### Comparing `openobd_protocol-0.13.0/LICENSE` & `openobd_protocol-0.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/PKG-INFO` & `openobd_protocol-0.14.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.13.0
+Version: 0.14.0
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.13.0/pyproject.toml` & `openobd_protocol-0.14.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/Authentication_pb2.py` & `openobd_protocol-0.14.0/src/openobd_protocol/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/Authentication_pb2.pyi` & `openobd_protocol-0.14.0/src/openobd_protocol/Authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/BasicResponse_pb2.py` & `openobd_protocol-0.14.0/src/openobd_protocol/BasicResponse_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$openobd_protocol/BasicResponse.proto\x12\x1d\x63om.jifeline.OpenOBD.Protocol\"-\n\x06Result\x12\x0e\n\x06result\x18\x01 \x01(\r\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"\x0e\n\x0c\x45mptyRequestB\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$openobd_protocol/BasicResponse.proto\x12\x1d\x63om.jifeline.OpenOBD.Protocol\"-\n\x06Result\x12\x0e\n\x06result\x18\x01 \x01(\r\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"\x0e\n\x0c\x45mptyMessageB\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.BasicResponse_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
   _globals['_RESULT']._serialized_start=71
   _globals['_RESULT']._serialized_end=116
-  _globals['_EMPTYREQUEST']._serialized_start=118
-  _globals['_EMPTYREQUEST']._serialized_end=132
+  _globals['_EMPTYMESSAGE']._serialized_start=118
+  _globals['_EMPTYMESSAGE']._serialized_end=132
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/BasicResponse_pb2.pyi` & `openobd_protocol-0.14.0/src/openobd_protocol/BasicResponse_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -8,10 +8,10 @@
     __slots__ = ("result", "description")
     RESULT_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     result: int
     description: str
     def __init__(self, result: _Optional[int] = ..., description: _Optional[str] = ...) -> None: ...
 
-class EmptyRequest(_message.Message):
+class EmptyMessage(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
```

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/BusConfiguration_pb2.py` & `openobd_protocol-0.14.0/src/openobd_protocol/BusConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/BusConfiguration_pb2.pyi` & `openobd_protocol-0.14.0/src/openobd_protocol/BusConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/CAN/CanServices_pb2.py` & `openobd_protocol-0.14.0/src/openobd_protocol/CAN/CanServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/CAN/CanServices_pb2_grpc.py` & `openobd_protocol-0.14.0/src/openobd_protocol/CAN/CanServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/CAN/Isotp_pb2.py` & `openobd_protocol-0.14.0/src/openobd_protocol/CAN/Isotp_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/CAN/Isotp_pb2.pyi` & `openobd_protocol-0.14.0/src/openobd_protocol/CAN/Isotp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.py` & `openobd_protocol-0.14.0/src/openobd_protocol/RemoteDiagnosticServices_pb2.py`

 * *Files identical despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from openobd_protocol import Authentication_pb2 as openobd__protocol_dot_Authentication__pb2
 from openobd_protocol import BasicResponse_pb2 as openobd__protocol_dot_BasicResponse__pb2
 from openobd_protocol import BusConfiguration_pb2 as openobd__protocol_dot_BusConfiguration__pb2
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/openobd_protocol/RemoteDiagnosticServices.proto\x12\x1d\x63om.jifeline.OpenOBD.Protocol\x1a%openobd_protocol/Authentication.proto\x1a$openobd_protocol/BasicResponse.proto\x1a\'openobd_protocol/BusConfiguration.proto\x1a\x1dopenobd_protocol/Status.proto2\xfa\x03\n\x18RemoteDiagnosticServices\x12h\n\x0c\x63onfigureBus\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12l\n\x0e\x63onfigureBuses\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00(\x01\x12}\n\x0c\x61uthenticate\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x12\x86\x01\n\x15refreshAuthentication\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/openobd_protocol/RemoteDiagnosticServices.proto\x12\x1d\x63om.jifeline.OpenOBD.Protocol\x1a%openobd_protocol/Authentication.proto\x1a$openobd_protocol/BasicResponse.proto\x1a\'openobd_protocol/BusConfiguration.proto\x1a\x1dopenobd_protocol/Status.proto2\xfa\x03\n\x18RemoteDiagnosticServices\x12}\n\x0c\x61uthenticate\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x12h\n\x0c\x63onfigureBus\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12l\n\x0e\x63onfigureBuses\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00(\x01\x12\x86\x01\n\x15refreshAuthentication\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.RemoteDiagnosticServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
```

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py` & `openobd_protocol-0.14.0/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,81 +12,81 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
+        self.authenticate = channel.unary_unary(
+                '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/authenticate',
+                request_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.SerializeToString,
+                response_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
+                )
         self.configureBus = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/configureBus',
                 request_serializer=openobd__protocol_dot_BusConfiguration__pb2.BusConfiguration.SerializeToString,
                 response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
                 )
         self.configureBuses = channel.stream_unary(
                 '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/configureBuses',
                 request_serializer=openobd__protocol_dot_BusConfiguration__pb2.BusConfiguration.SerializeToString,
                 response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
                 )
-        self.authenticate = channel.unary_unary(
-                '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/authenticate',
-                request_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.SerializeToString,
-                response_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
-                )
         self.refreshAuthentication = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/refreshAuthentication',
                 request_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.SerializeToString,
                 response_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
                 )
 
 
 class RemoteDiagnosticServicesServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def configureBus(self, request, context):
+    def authenticate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def configureBuses(self, request_iterator, context):
+    def configureBus(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def authenticate(self, request, context):
+    def configureBuses(self, request_iterator, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def refreshAuthentication(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_RemoteDiagnosticServicesServicer_to_server(servicer, server):
     rpc_method_handlers = {
+            'authenticate': grpc.unary_unary_rpc_method_handler(
+                    servicer.authenticate,
+                    request_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.FromString,
+                    response_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.SerializeToString,
+            ),
             'configureBus': grpc.unary_unary_rpc_method_handler(
                     servicer.configureBus,
                     request_deserializer=openobd__protocol_dot_BusConfiguration__pb2.BusConfiguration.FromString,
                     response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
             ),
             'configureBuses': grpc.stream_unary_rpc_method_handler(
                     servicer.configureBuses,
                     request_deserializer=openobd__protocol_dot_BusConfiguration__pb2.BusConfiguration.FromString,
                     response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
             ),
-            'authenticate': grpc.unary_unary_rpc_method_handler(
-                    servicer.authenticate,
-                    request_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.FromString,
-                    response_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.SerializeToString,
-            ),
             'refreshAuthentication': grpc.unary_unary_rpc_method_handler(
                     servicer.refreshAuthentication,
                     request_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.FromString,
                     response_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -95,61 +95,61 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class RemoteDiagnosticServices(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def configureBus(request,
+    def authenticate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/configureBus',
-            openobd__protocol_dot_BusConfiguration__pb2.BusConfiguration.SerializeToString,
-            openobd__protocol_dot_Status__pb2.Status.FromString,
+        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/authenticate',
+            openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.SerializeToString,
+            openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def configureBuses(request_iterator,
+    def configureBus(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.stream_unary(request_iterator, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/configureBuses',
+        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/configureBus',
             openobd__protocol_dot_BusConfiguration__pb2.BusConfiguration.SerializeToString,
             openobd__protocol_dot_Status__pb2.Status.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def authenticate(request,
+    def configureBuses(request_iterator,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/authenticate',
-            openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.SerializeToString,
-            openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
+        return grpc.experimental.stream_unary(request_iterator, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/configureBuses',
+            openobd__protocol_dot_BusConfiguration__pb2.BusConfiguration.SerializeToString,
+            openobd__protocol_dot_Status__pb2.Status.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def refreshAuthentication(request,
             target,
             options=(),
```

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/SessionController/SessionServices_pb2.py` & `openobd_protocol-0.14.0/src/openobd_protocol/SessionController/SessionServices_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 from openobd_protocol.SessionController import Session_pb2 as openobd__protocol_dot_SessionController_dot_Session__pb2
 from openobd_protocol import BasicResponse_pb2 as openobd__protocol_dot_BasicResponse__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8openobd_protocol/SessionController/SessionServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\x1a\x30openobd_protocol/SessionController/Session.proto\x1a$openobd_protocol/BasicResponse.proto2\x8c\x08\n\x0fSessionServices\x12\x91\x01\n\x0fgetSessionToken\x12=.com.jifeline.OpenOBD.Protocol.SessionController.Authenticate\x1a=.com.jifeline.OpenOBD.Protocol.SessionController.SessionToken\"\x00\x12\x99\x01\n\x18startSessionOnConnection\x12=.com.jifeline.OpenOBD.Protocol.SessionController.ConnectionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x91\x01\n\x14startSessionOnTicket\x12\x39.com.jifeline.OpenOBD.Protocol.SessionController.TicketId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x97\x01\n\x17startSessionOnConnector\x12<.com.jifeline.OpenOBD.Protocol.SessionController.ConnectorId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x88\x01\n\ngetSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x8b\x01\n\rdeleteSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x81\x01\n\x0egetSessionList\x12+.com.jifeline.OpenOBD.Protocol.EmptyRequest\x1a@.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfoList\"\x00\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8openobd_protocol/SessionController/SessionServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\x1a\x30openobd_protocol/SessionController/Session.proto\x1a$openobd_protocol/BasicResponse.proto2\x8c\x08\n\x0fSessionServices\x12\x91\x01\n\x0fgetSessionToken\x12=.com.jifeline.OpenOBD.Protocol.SessionController.Authenticate\x1a=.com.jifeline.OpenOBD.Protocol.SessionController.SessionToken\"\x00\x12\x99\x01\n\x18startSessionOnConnection\x12=.com.jifeline.OpenOBD.Protocol.SessionController.ConnectionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x91\x01\n\x14startSessionOnTicket\x12\x39.com.jifeline.OpenOBD.Protocol.SessionController.TicketId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x97\x01\n\x17startSessionOnConnector\x12<.com.jifeline.OpenOBD.Protocol.SessionController.ConnectorId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x88\x01\n\ngetSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x8b\x01\n\rdeleteSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x81\x01\n\x0egetSessionList\x12+.com.jifeline.OpenOBD.Protocol.EmptyMessage\x1a@.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfoList\"\x00\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.SessionController.SessionServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
```

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py` & `openobd_protocol-0.14.0/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self.deleteSession = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/deleteSession',
                 request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.SerializeToString,
                 response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
                 )
         self.getSessionList = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSessionList',
-                request_serializer=openobd__protocol_dot_BasicResponse__pb2.EmptyRequest.SerializeToString,
+                request_serializer=openobd__protocol_dot_BasicResponse__pb2.EmptyMessage.SerializeToString,
                 response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfoList.FromString,
                 )
 
 
 class SessionServicesServicer(object):
     """
     The SessionServices are used to create an openOBD session.
@@ -148,15 +148,15 @@
             'deleteSession': grpc.unary_unary_rpc_method_handler(
                     servicer.deleteSession,
                     request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.FromString,
                     response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.SerializeToString,
             ),
             'getSessionList': grpc.unary_unary_rpc_method_handler(
                     servicer.getSessionList,
-                    request_deserializer=openobd__protocol_dot_BasicResponse__pb2.EmptyRequest.FromString,
+                    request_deserializer=openobd__protocol_dot_BasicResponse__pb2.EmptyMessage.FromString,
                     response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfoList.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'com.jifeline.OpenOBD.Protocol.SessionController.SessionServices', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
@@ -285,11 +285,11 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSessionList',
-            openobd__protocol_dot_BasicResponse__pb2.EmptyRequest.SerializeToString,
+            openobd__protocol_dot_BasicResponse__pb2.EmptyMessage.SerializeToString,
             openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfoList.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/SessionController/Session_pb2.py` & `openobd_protocol-0.14.0/src/openobd_protocol/SessionController/Session_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/SessionController/Session_pb2.pyi` & `openobd_protocol-0.14.0/src/openobd_protocol/SessionController/Session_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/Status_pb2.py` & `openobd_protocol-0.14.0/src/openobd_protocol/Status_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/Status_pb2.pyi` & `openobd_protocol-0.14.0/src/openobd_protocol/Status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py` & `openobd_protocol-0.14.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py` & `openobd_protocol-0.14.0/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterface_pb2.py` & `openobd_protocol-0.14.0/src/openobd_protocol/UserInterface/UserInterface_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi` & `openobd_protocol-0.14.0/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.13.0/src/openobd_protocol.egg-info/PKG-INFO` & `openobd_protocol-0.14.0/src/openobd_protocol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.13.0
+Version: 0.14.0
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

