# Comparing `tmp/ansys-api-dbu-0.3.0.tar.gz` & `tmp/ansys_api_dbu-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-dbu-0.3.0.tar", last modified: Tue Mar 19 07:17:22 2024, max compression
+gzip compressed data, was "ansys_api_dbu-0.3.1.tar", last modified: Fri May 24 13:43:05 2024, max compression
```

## Comparing `ansys-api-dbu-0.3.0.tar` & `ansys_api_dbu-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:17:22.455933 ansys-api-dbu-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-19 07:17:22.455933 ansys-api-dbu-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:17:22.447933 ansys-api-dbu-0.3.0/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:17:22.447933 ansys-api-dbu-0.3.0/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:17:22.451933 ansys-api-dbu-0.3.0/ansys/api/dbu/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:17:22.451933 ansys-api-dbu-0.3.0/ansys/api/dbu/v0/
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/v0/admin.proto
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/v0/dbuapi.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/v0/dbuapplication.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/v0/dbumodels.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/v0/dbuwebmodels.proto
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/v0/designs.proto
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/v0/drivingdimensions.proto
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/v0/sessionmanager.proto
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/v0/streaming.proto
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/ansys/api/dbu/v0/windows.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 07:17:22.455933 ansys-api-dbu-0.3.0/ansys_api_dbu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-19 07:17:22.000000 ansys-api-dbu-0.3.0/ansys_api_dbu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-19 07:17:22.000000 ansys-api-dbu-0.3.0/ansys_api_dbu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 07:17:22.000000 ansys-api-dbu-0.3.0/ansys_api_dbu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-19 07:17:22.000000 ansys-api-dbu-0.3.0/ansys_api_dbu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-19 07:17:22.000000 ansys-api-dbu-0.3.0/ansys_api_dbu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-19 07:17:22.000000 ansys-api-dbu-0.3.0/ansys_api_dbu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 07:17:22.455933 ansys-api-dbu-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-19 07:17:13.000000 ansys-api-dbu-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.814770 ansys_api_dbu-0.3.1/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.814770 ansys_api_dbu-0.3.1/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/ansys/api/dbu/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/admin.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuapi.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuapplication.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbumodels.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuwebmodels.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/designs.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/drivingdimensions.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/sessionmanager.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/streaming.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/ansys/api/dbu/v0/windows.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 13:43:05.000000 ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:43:05.818770 ansys_api_dbu-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-24 13:42:58.000000 ansys_api_dbu-0.3.1/setup.py
```

### Comparing `ansys-api-dbu-0.3.0/LICENSE` & `ansys_api_dbu-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-dbu-0.3.0/PKG-INFO` & `ansys_api_dbu-0.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-dbu
-Version: 0.3.0
-Summary: Autogenerated Python gRPC interface package for ansys-api-dbu, built on 07:17:22 on 19 March 2024
+Version: 0.3.1
+Summary: Autogenerated Python gRPC interface package for ansys-api-dbu, built on 13:43:05 on 24 May 2024
 Home-page: https://github.com/ansys/ansys-api-dbu
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-dbu/#readme
```

### Comparing `ansys-api-dbu-0.3.0/README.md` & `ansys_api_dbu-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-dbu-0.3.0/ansys/api/dbu/v0/admin.proto` & `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/admin.proto`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,20 @@
   rpc StatusInfo(google.protobuf.Empty) returns(StatusInfoResponse);
 
   rpc SetApplicationTitle(SetApplicationTitleRequest) returns(google.protobuf.Empty);
 
   rpc CloseApplication(google.protobuf.Empty) returns(google.protobuf.Empty);
 
   rpc GetBackend(google.protobuf.Empty) returns(GetBackendResponse);
+
+  rpc ApplicationStarted(google.protobuf.Empty) returns(ApplicationStartedResponse);
+  
+  rpc SetMonikersCompressionMethod(MonikerCompressionMethodMessage) returns(google.protobuf.Empty);
+
+  rpc GetMonikersCompressionMethod(google.protobuf.Empty) returns(MonikerCompressionMethodMessage);
 }
 
 enum LogsTarget{
   CLIENT = 0;
   PATH = 1;
 }
 
@@ -80,7 +86,15 @@
   string title =1;
 }
 
 message GetBackendResponse{
   BackendType type = 1;
   VersionIdentifier version = 2;
 }
+
+message ApplicationStartedResponse{
+  bool is_startup_complete = 1;
+}
+
+message MonikerCompressionMethodMessage{
+  MonikerCompressionMethod method = 1;
+}
```

### Comparing `ansys-api-dbu-0.3.0/ansys/api/dbu/v0/dbuapi.proto` & `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuapi.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-dbu-0.3.0/ansys/api/dbu/v0/dbuapplication.proto` & `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuapplication.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-dbu-0.3.0/ansys/api/dbu/v0/dbumodels.proto` & `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbumodels.proto`

 * *Files 9% similar despite different names*

```diff
@@ -82,8 +82,14 @@
 }
 
 message VersionIdentifier
 {
   int32 major_release = 1;
   int32 minor_release = 2;
   int32 service_pack = 3;
-}
+}
+
+enum MonikerCompressionMethod {
+  MONIKERCOMPRESSIONMETHOD_FULL = 0;
+  MONIKERCOMPRESSIONMETHOD_COMPRESSED = 1;
+  MONIKERCOMPRESSIONMETHOD_OBJECT_PATH = 2;
+}
```

### Comparing `ansys-api-dbu-0.3.0/ansys/api/dbu/v0/dbuwebmodels.proto` & `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/dbuwebmodels.proto`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 //
 // A Discovery session's host.
 message SessionHost {
   ObjectIdentifier id = 1;
   string name = 2;
   SessionHostStatus status = 3;
   google.protobuf.Timestamp idle_time = 4;
+  string address = 5;
+  int32 port = 6;
 }
 
 //
 // The host's status.
 enum SessionHostStatus {
   HOSTSTATUS_UNKNOWN = 0;
   HOSTSTATUS_OFF = 1;
@@ -34,14 +36,16 @@
 // A Discovery session.
 message Session
 {
   ObjectIdentifier id = 1;
   string name = 2;
   SessionStatus status = 3;
   google.protobuf.Timestamp idle_time = 4;
+  string address = 5;
+  int32 port = 6;
 }
 
 //
 // The Discovery session's status.
 enum SessionStatus {
   SESSIONSTATUS_UNKNOWN = 0;
   SESSIONSTATUS_NOT_STARTED = 1;
```

### Comparing `ansys-api-dbu-0.3.0/ansys/api/dbu/v0/designs.proto` & `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/designs.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-dbu-0.3.0/ansys/api/dbu/v0/drivingdimensions.proto` & `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/drivingdimensions.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-dbu-0.3.0/ansys/api/dbu/v0/sessionmanager.proto` & `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/sessionmanager.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-dbu-0.3.0/ansys/api/dbu/v0/windows.proto` & `ansys_api_dbu-0.3.1/ansys/api/dbu/v0/windows.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-dbu-0.3.0/ansys_api_dbu.egg-info/PKG-INFO` & `ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-dbu
-Version: 0.3.0
-Summary: Autogenerated Python gRPC interface package for ansys-api-dbu, built on 07:17:22 on 19 March 2024
+Version: 0.3.1
+Summary: Autogenerated Python gRPC interface package for ansys-api-dbu, built on 13:43:05 on 24 May 2024
 Home-page: https://github.com/ansys/ansys-api-dbu
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-dbu/#readme
```

### Comparing `ansys-api-dbu-0.3.0/ansys_api_dbu.egg-info/SOURCES.txt` & `ansys_api_dbu-0.3.1/ansys_api_dbu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansys-api-dbu-0.3.0/setup.py` & `ansys_api_dbu-0.3.1/setup.py`

 * *Files identical despite different names*

