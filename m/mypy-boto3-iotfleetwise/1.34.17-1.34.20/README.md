# Comparing `tmp/mypy-boto3-iotfleetwise-1.34.17.tar.gz` & `tmp/mypy-boto3-iotfleetwise-1.34.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotfleetwise-1.34.17.tar", last modified: Thu Jan 11 20:25:53 2024, max compression
+gzip compressed data, was "mypy-boto3-iotfleetwise-1.34.20.tar", last modified: Tue Jan 16 20:32:45 2024, max compression
```

## Comparing `mypy-boto3-iotfleetwise-1.34.17.tar` & `mypy-boto3-iotfleetwise-1.34.20.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:25:53.232409 mypy-boto3-iotfleetwise-1.34.17/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14819 2024-01-11 20:25:53.232409 mypy-boto3-iotfleetwise-1.34.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:25:53.232409 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42140 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    42137 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12911 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12911 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53084 2024-01-11 20:25:37.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53084 2024-01-11 20:25:37.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:25:53.232409 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14819 2024-01-11 20:25:53.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-11 20:25:53.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 20:25:53.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 20:25:53.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-11 20:25:53.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-11 20:25:53.000000 mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 20:25:53.232409 mypy-boto3-iotfleetwise-1.34.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-01-11 20:25:35.000000 mypy-boto3-iotfleetwise-1.34.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:45.096974 mypy-boto3-iotfleetwise-1.34.20/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-16 20:32:02.000000 mypy-boto3-iotfleetwise-1.34.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14819 2024-01-16 20:32:45.096974 mypy-boto3-iotfleetwise-1.34.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-01-16 20:32:02.000000 mypy-boto3-iotfleetwise-1.34.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:45.092974 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-01-16 20:32:02.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-01-16 20:32:02.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-16 20:32:02.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42247 2024-01-16 20:32:04.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42244 2024-01-16 20:32:03.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-01-16 20:32:04.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-01-16 20:32:04.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15658 2024-01-16 20:32:04.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-01-16 20:32:04.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:02.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53277 2024-01-16 20:32:05.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53277 2024-01-16 20:32:04.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-16 20:32:02.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 20:32:45.096974 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14819 2024-01-16 20:32:45.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-16 20:32:45.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 20:32:45.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 20:32:45.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-16 20:32:45.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-16 20:32:45.000000 mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 20:32:45.096974 mypy-boto3-iotfleetwise-1.34.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-01-16 20:32:02.000000 mypy-boto3-iotfleetwise-1.34.20/setup.py
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/LICENSE` & `mypy-boto3-iotfleetwise-1.34.20/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.34.17/PKG-INFO` & `mypy-boto3-iotfleetwise-1.34.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleetwise
-Version: 1.34.17
-Summary: Type annotations for boto3.IoTFleetWise 1.34.17 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.20
+Summary: Type annotations for boto3.IoTFleetWise 1.34.20 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.34.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/README.md` & `mypy-boto3-iotfleetwise-1.34.20/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.34.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/__init__.py` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/__init__.pyi` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/__main__.py` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTFleetWise 1.34.17\nVersion:         1.34.17\nBuilder"
+        "Type annotations for boto3.IoTFleetWise 1.34.20\nVersion:         1.34.20\nBuilder"
         " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.17")
+    print("1.34.20")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/client.py` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CompressionType,
     DiagnosticsModeType,
     EncryptionTypeType,
     ManifestStatusType,
+    SignalNodeTypeType,
     SpoolingModeType,
     UpdateCampaignActionType,
     UpdateModeType,
     VehicleAssociationBehaviorType,
 )
 from .paginator import (
     GetVehicleStatusPaginator,
@@ -574,15 +575,20 @@
         Retrieves a list of vehicle models (model manifests).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.list_model_manifests)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#list_model_manifests)
         """
 
     def list_signal_catalog_nodes(
-        self, *, name: str, nextToken: str = ..., maxResults: int = ...
+        self,
+        *,
+        name: str,
+        nextToken: str = ...,
+        maxResults: int = ...,
+        signalNodeType: SignalNodeTypeType = ...,
     ) -> ListSignalCatalogNodesResponseTypeDef:
         """
         Lists of information about the signals (nodes) specified in a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.list_signal_catalog_nodes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#list_signal_catalog_nodes)
         """
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/client.pyi` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     CompressionType,
     DiagnosticsModeType,
     EncryptionTypeType,
     ManifestStatusType,
+    SignalNodeTypeType,
     SpoolingModeType,
     UpdateCampaignActionType,
     UpdateModeType,
     VehicleAssociationBehaviorType,
 )
 from .paginator import (
     GetVehicleStatusPaginator,
@@ -571,15 +572,20 @@
         Retrieves a list of vehicle models (model manifests).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.list_model_manifests)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#list_model_manifests)
         """
 
     def list_signal_catalog_nodes(
-        self, *, name: str, nextToken: str = ..., maxResults: int = ...
+        self,
+        *,
+        name: str,
+        nextToken: str = ...,
+        maxResults: int = ...,
+        signalNodeType: SignalNodeTypeType = ...,
     ) -> ListSignalCatalogNodesResponseTypeDef:
         """
         Lists of information about the signals (nodes) specified in a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.list_signal_catalog_nodes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/client/#list_signal_catalog_nodes)
         """
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/literals.py` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     "ManifestStatusType",
     "NetworkInterfaceTypeType",
     "NodeDataEncodingType",
     "NodeDataTypeType",
     "ROS2PrimitiveTypeType",
     "RegistrationStatusType",
     "SignalDecoderTypeType",
+    "SignalNodeTypeType",
     "SpoolingModeType",
     "StorageCompressionFormatType",
     "StructuredMessageListTypeType",
     "TriggerModeType",
     "UpdateCampaignActionType",
     "UpdateModeType",
     "VehicleAssociationBehaviorType",
@@ -136,14 +137,17 @@
     "UINT8",
     "WSTRING",
 ]
 RegistrationStatusType = Literal[
     "REGISTRATION_FAILURE", "REGISTRATION_PENDING", "REGISTRATION_SUCCESS"
 ]
 SignalDecoderTypeType = Literal["CAN_SIGNAL", "MESSAGE_SIGNAL", "OBD_SIGNAL"]
+SignalNodeTypeType = Literal[
+    "ACTUATOR", "ATTRIBUTE", "BRANCH", "CUSTOM_PROPERTY", "CUSTOM_STRUCT", "SENSOR"
+]
 SpoolingModeType = Literal["OFF", "TO_DISK"]
 StorageCompressionFormatType = Literal["GZIP", "NONE"]
 StructuredMessageListTypeType = Literal[
     "DYNAMIC_BOUNDED_CAPACITY", "DYNAMIC_UNBOUNDED_CAPACITY", "FIXED_CAPACITY"
 ]
 TriggerModeType = Literal["ALWAYS", "RISING_EDGE"]
 UpdateCampaignActionType = Literal["APPROVE", "RESUME", "SUSPEND", "UPDATE"]
@@ -497,14 +501,15 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/literals.pyi` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     "ManifestStatusType",
     "NetworkInterfaceTypeType",
     "NodeDataEncodingType",
     "NodeDataTypeType",
     "ROS2PrimitiveTypeType",
     "RegistrationStatusType",
     "SignalDecoderTypeType",
+    "SignalNodeTypeType",
     "SpoolingModeType",
     "StorageCompressionFormatType",
     "StructuredMessageListTypeType",
     "TriggerModeType",
     "UpdateCampaignActionType",
     "UpdateModeType",
     "VehicleAssociationBehaviorType",
@@ -136,14 +137,17 @@
     "UINT8",
     "WSTRING",
 ]
 RegistrationStatusType = Literal[
     "REGISTRATION_FAILURE", "REGISTRATION_PENDING", "REGISTRATION_SUCCESS"
 ]
 SignalDecoderTypeType = Literal["CAN_SIGNAL", "MESSAGE_SIGNAL", "OBD_SIGNAL"]
+SignalNodeTypeType = Literal[
+    "ACTUATOR", "ATTRIBUTE", "BRANCH", "CUSTOM_PROPERTY", "CUSTOM_STRUCT", "SENSOR"
+]
 SpoolingModeType = Literal["OFF", "TO_DISK"]
 StorageCompressionFormatType = Literal["GZIP", "NONE"]
 StructuredMessageListTypeType = Literal[
     "DYNAMIC_BOUNDED_CAPACITY", "DYNAMIC_UNBOUNDED_CAPACITY", "FIXED_CAPACITY"
 ]
 TriggerModeType = Literal["ALWAYS", "RISING_EDGE"]
 UpdateCampaignActionType = Literal["APPROVE", "RESUME", "SUSPEND", "UPDATE"]
@@ -497,14 +501,15 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/paginator.py` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     ```
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
+from .literals import SignalNodeTypeType
 from .type_defs import (
     GetVehicleStatusResponseTypeDef,
     ListCampaignsResponseTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
     ListDecoderManifestSignalsResponsePaginatorTypeDef,
     ListDecoderManifestsResponseTypeDef,
     ListFleetsForVehicleResponseTypeDef,
@@ -229,15 +230,19 @@
 class ListSignalCatalogNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalognodespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        name: str,
+        signalNodeType: SignalNodeTypeType = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListSignalCatalogNodesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalognodespaginator)
         """
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/paginator.pyi` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     ```
 """
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
+from .literals import SignalNodeTypeType
 from .type_defs import (
     GetVehicleStatusResponseTypeDef,
     ListCampaignsResponseTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
     ListDecoderManifestSignalsResponsePaginatorTypeDef,
     ListDecoderManifestsResponseTypeDef,
     ListFleetsForVehicleResponseTypeDef,
@@ -218,15 +219,19 @@
 class ListSignalCatalogNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalognodespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self,
+        *,
+        name: str,
+        signalNodeType: SignalNodeTypeType = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListSignalCatalogNodesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/paginators/#listsignalcatalognodespaginator)
         """
 
 class ListSignalCatalogsPaginator(Paginator):
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/type_defs.py` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     ManifestStatusType,
     NetworkInterfaceTypeType,
     NodeDataEncodingType,
     NodeDataTypeType,
     RegistrationStatusType,
     ROS2PrimitiveTypeType,
     SignalDecoderTypeType,
+    SignalNodeTypeType,
     SpoolingModeType,
     StorageCompressionFormatType,
     StructuredMessageListTypeType,
     TriggerModeType,
     UpdateCampaignActionType,
     UpdateModeType,
     VehicleAssociationBehaviorType,
@@ -720,14 +721,15 @@
 )
 ListSignalCatalogNodesRequestRequestTypeDef = TypedDict(
     "ListSignalCatalogNodesRequestRequestTypeDef",
     {
         "name": str,
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
+        "signalNodeType": NotRequired[SignalNodeTypeType],
     },
 )
 ListSignalCatalogsRequestRequestTypeDef = TypedDict(
     "ListSignalCatalogsRequestRequestTypeDef",
     {
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
@@ -769,14 +771,15 @@
     {
         "vehicleName": str,
         "arn": str,
         "modelManifestArn": str,
         "decoderManifestArn": str,
         "creationTime": datetime,
         "lastModificationTime": datetime,
+        "attributes": NotRequired[Dict[str, str]],
     },
 )
 MessageSignalPaginatorTypeDef = TypedDict(
     "MessageSignalPaginatorTypeDef",
     {
         "topicName": str,
         "structuredMessage": "StructuredMessagePaginatorTypeDef",
@@ -1416,14 +1419,15 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
     "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
     {
         "name": str,
+        "signalNodeType": NotRequired[SignalNodeTypeType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef = TypedDict(
     "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise/type_defs.pyi` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     ManifestStatusType,
     NetworkInterfaceTypeType,
     NodeDataEncodingType,
     NodeDataTypeType,
     RegistrationStatusType,
     ROS2PrimitiveTypeType,
     SignalDecoderTypeType,
+    SignalNodeTypeType,
     SpoolingModeType,
     StorageCompressionFormatType,
     StructuredMessageListTypeType,
     TriggerModeType,
     UpdateCampaignActionType,
     UpdateModeType,
     VehicleAssociationBehaviorType,
@@ -720,14 +721,15 @@
 )
 ListSignalCatalogNodesRequestRequestTypeDef = TypedDict(
     "ListSignalCatalogNodesRequestRequestTypeDef",
     {
         "name": str,
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
+        "signalNodeType": NotRequired[SignalNodeTypeType],
     },
 )
 ListSignalCatalogsRequestRequestTypeDef = TypedDict(
     "ListSignalCatalogsRequestRequestTypeDef",
     {
         "nextToken": NotRequired[str],
         "maxResults": NotRequired[int],
@@ -769,14 +771,15 @@
     {
         "vehicleName": str,
         "arn": str,
         "modelManifestArn": str,
         "decoderManifestArn": str,
         "creationTime": datetime,
         "lastModificationTime": datetime,
+        "attributes": NotRequired[Dict[str, str]],
     },
 )
 MessageSignalPaginatorTypeDef = TypedDict(
     "MessageSignalPaginatorTypeDef",
     {
         "topicName": str,
         "structuredMessage": "StructuredMessagePaginatorTypeDef",
@@ -1416,14 +1419,15 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
     "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
     {
         "name": str,
+        "signalNodeType": NotRequired[SignalNodeTypeType],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef = TypedDict(
     "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise.egg-info/PKG-INFO` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleetwise
-Version: 1.34.17
-Summary: Type annotations for boto3.IoTFleetWise 1.34.17 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.20
+Summary: Type annotations for boto3.IoTFleetWise 1.34.20 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleetwise)](https://pepy.tech/project/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.34.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.34.20](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-iotfleetwise-1.34.17/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt` & `mypy-boto3-iotfleetwise-1.34.20/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.34.17/setup.py` & `mypy-boto3-iotfleetwise-1.34.20/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotfleetwise",
-    version="1.34.17",
+    version="1.34.20",
     packages=["mypy_boto3_iotfleetwise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTFleetWise 1.34.17 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.IoTFleetWise 1.34.20 service generated with mypy-boto3-builder"
         " 7.23.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

