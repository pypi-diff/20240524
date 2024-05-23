# Comparing `tmp/modelscan-0.7.3.tar.gz` & `tmp/modelscan-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelscan-0.7.3.tar", max compression
+gzip compressed data, was "modelscan-0.7.4.tar", max compression
```

## Comparing `modelscan-0.7.3.tar` & `modelscan-0.7.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    10754 2024-04-16 17:14:54.806341 modelscan-0.7.3/LICENSE
--rw-r--r--   0        0        0    12564 2024-04-16 17:14:54.806341 modelscan-0.7.3/README.md
--rw-r--r--   0        0        0      156 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/__init__.py
--rw-r--r--   0        0        0       22 2024-04-16 17:15:10.714306 modelscan-0.7.3/modelscan/_version.py
--rw-r--r--   0        0        0     6154 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/cli.py
--rw-r--r--   0        0        0     2455 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/error.py
--rw-r--r--   0        0        0     4697 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/issues.py
--rw-r--r--   0        0        0       84 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/middlewares/__init__.py
--rw-r--r--   0        0        0      585 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/middlewares/format_via_extension.py
--rw-r--r--   0        0        0     1757 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/middlewares/middleware.py
--rw-r--r--   0        0        0     1458 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/model.py
--rw-r--r--   0        0        0    13141 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/modelscan.py
--rw-r--r--   0        0        0     2993 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/reports.py
--rw-r--r--   0        0        0      377 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/scanners/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/scanners/h5/__init__.py
--rw-r--r--   0        0        0     4611 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/scanners/h5/scan.py
--rw-r--r--   0        0        0        0 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/scanners/keras/__init__.py
--rw-r--r--   0        0        0     4451 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/scanners/keras/scan.py
--rw-r--r--   0        0        0        0 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/scanners/pickle/__init__.py
--rw-r--r--   0        0        0     1972 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/scanners/pickle/scan.py
--rw-r--r--   0        0        0        0 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/scanners/saved_model/__init__.py
--rw-r--r--   0        0        0     6853 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/scanners/saved_model/scan.py
--rw-r--r--   0        0        0     1652 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/scanners/scan.py
--rw-r--r--   0        0        0     4412 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/settings.py
--rw-r--r--   0        0        0      892 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/skip.py
--rw-r--r--   0        0        0     2591 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/tools/LICENSE
--rw-r--r--   0        0        0     3435 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/tools/cli_utils.py
--rw-r--r--   0        0        0     9598 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/tools/picklescanner.py
--rw-r--r--   0        0        0     2989 2024-04-16 17:14:54.822341 modelscan-0.7.3/modelscan/tools/utils.py
--rw-r--r--   0        0        0     1629 2024-04-16 17:15:11.090305 modelscan-0.7.3/pyproject.toml
--rw-r--r--   0        0        0    13840 1970-01-01 00:00:00.000000 modelscan-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    10754 2024-05-23 18:12:47.058245 modelscan-0.7.4/LICENSE
+-rw-r--r--   0        0        0    12564 2024-05-23 18:12:47.058245 modelscan-0.7.4/README.md
+-rw-r--r--   0        0        0      156 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-23 18:13:03.498335 modelscan-0.7.4/modelscan/_version.py
+-rw-r--r--   0        0        0     6154 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/cli.py
+-rw-r--r--   0        0        0     2455 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/error.py
+-rw-r--r--   0        0        0     4697 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/issues.py
+-rw-r--r--   0        0        0       84 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/middlewares/__init__.py
+-rw-r--r--   0        0        0      585 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/middlewares/format_via_extension.py
+-rw-r--r--   0        0        0     1757 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/middlewares/middleware.py
+-rw-r--r--   0        0        0     1458 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/model.py
+-rw-r--r--   0        0        0    13141 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/modelscan.py
+-rw-r--r--   0        0        0     2993 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/reports.py
+-rw-r--r--   0        0        0      377 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/scanners/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/scanners/h5/__init__.py
+-rw-r--r--   0        0        0     4680 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/scanners/h5/scan.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/scanners/keras/__init__.py
+-rw-r--r--   0        0        0     4520 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/scanners/keras/scan.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/scanners/pickle/__init__.py
+-rw-r--r--   0        0        0     2077 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/scanners/pickle/scan.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/scanners/saved_model/__init__.py
+-rw-r--r--   0        0        0     6918 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/scanners/saved_model/scan.py
+-rw-r--r--   0        0        0     1652 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/scanners/scan.py
+-rw-r--r--   0        0        0     4685 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/settings.py
+-rw-r--r--   0        0        0      892 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/skip.py
+-rw-r--r--   0        0        0     2591 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/tools/LICENSE
+-rw-r--r--   0        0        0     3435 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/tools/cli_utils.py
+-rw-r--r--   0        0        0     9598 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/tools/picklescanner.py
+-rw-r--r--   0        0        0     2989 2024-05-23 18:12:47.070245 modelscan-0.7.4/modelscan/tools/utils.py
+-rw-r--r--   0        0        0     1629 2024-05-23 18:13:03.878337 modelscan-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0    13840 1970-01-01 00:00:00.000000 modelscan-0.7.4/PKG-INFO
```

### Comparing `modelscan-0.7.3/LICENSE` & `modelscan-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/README.md` & `modelscan-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/cli.py` & `modelscan-0.7.4/modelscan/cli.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/error.py` & `modelscan-0.7.4/modelscan/error.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/issues.py` & `modelscan-0.7.4/modelscan/issues.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/middlewares/format_via_extension.py` & `modelscan-0.7.4/modelscan/middlewares/format_via_extension.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/middlewares/middleware.py` & `modelscan-0.7.4/modelscan/middlewares/middleware.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/model.py` & `modelscan-0.7.4/modelscan/model.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/modelscan.py` & `modelscan-0.7.4/modelscan/modelscan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/reports.py` & `modelscan-0.7.4/modelscan/reports.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/scanners/h5/scan.py` & `modelscan-0.7.4/modelscan/scanners/h5/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,25 @@
     DependencyError,
     JsonDecodeError,
 )
 from modelscan.skip import ModelScanSkipped, SkipCategories
 from modelscan.scanners.scan import ScanResults
 from modelscan.scanners.saved_model.scan import SavedModelLambdaDetectScan
 from modelscan.model import Model
+from modelscan.settings import DefaultModelFormats
 
 logger = logging.getLogger("modelscan")
 
 
 class H5LambdaDetectScan(SavedModelLambdaDetectScan):
     def scan(
         self,
         model: Model,
     ) -> Optional[ScanResults]:
-        if "keras_h5" not in model.get_context("formats"):
+        if DefaultModelFormats.KERAS_H5 not in model.get_context("formats"):
             return None
 
         dep_error = self.handle_binary_dependencies()
         if dep_error:
             return ScanResults(
                 [],
                 [
```

### Comparing `modelscan-0.7.3/modelscan/scanners/keras/scan.py` & `modelscan-0.7.4/modelscan/scanners/keras/scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 
 from modelscan.error import DependencyError, ModelScanScannerError, JsonDecodeError
 from modelscan.skip import ModelScanSkipped, SkipCategories
 from modelscan.scanners.scan import ScanResults
 from modelscan.scanners.saved_model.scan import SavedModelLambdaDetectScan
 from modelscan.model import Model
+from modelscan.settings import DefaultModelFormats
 
 
 logger = logging.getLogger("modelscan")
 
 
 class KerasLambdaDetectScan(SavedModelLambdaDetectScan):
     def scan(self, model: Model) -> Optional[ScanResults]:
-        if "keras" not in model.get_context("formats"):
+        if DefaultModelFormats.KERAS not in model.get_context("formats"):
             return None
 
         dep_error = self.handle_binary_dependencies()
         if dep_error:
             return ScanResults(
                 [],
                 [
```

### Comparing `modelscan-0.7.3/modelscan/scanners/pickle/scan.py` & `modelscan-0.7.4/modelscan/scanners/pickle/scan.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 from modelscan.tools.utils import _is_zipfile
 from modelscan.tools.picklescanner import (
     scan_numpy,
     scan_pickle_bytes,
     scan_pytorch,
 )
 from modelscan.model import Model
+from modelscan.settings import DefaultModelFormats
 
 logger = logging.getLogger("modelscan")
 
 
 class PyTorchUnsafeOpScan(ScanBase):
     def scan(
         self,
         model: Model,
     ) -> Optional[ScanResults]:
-        if "pytorch" not in model.get_context("formats"):
+        if DefaultModelFormats.PYTORCH not in model.get_context("formats"):
             return None
 
         if _is_zipfile(model.get_source(), model.get_stream()):
             return None
 
         results = scan_pytorch(
             model=model,
@@ -41,15 +42,15 @@
 
 
 class NumpyUnsafeOpScan(ScanBase):
     def scan(
         self,
         model: Model,
     ) -> Optional[ScanResults]:
-        if "numpy" not in model.get_context("formats"):
+        if DefaultModelFormats.NUMPY not in model.get_context("formats"):
             return None
 
         results = scan_numpy(
             model=model,
             settings=self._settings,
         )
 
@@ -65,15 +66,15 @@
 
 
 class PickleUnsafeOpScan(ScanBase):
     def scan(
         self,
         model: Model,
     ) -> Optional[ScanResults]:
-        if "pickle" not in model.get_context("formats"):
+        if DefaultModelFormats.PICKLE not in model.get_context("formats"):
             return None
 
         results = scan_pickle_bytes(
             model=model,
             settings=self._settings,
         )
```

### Comparing `modelscan-0.7.3/modelscan/scanners/saved_model/scan.py` & `modelscan-0.7.4/modelscan/scanners/saved_model/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,25 @@
 from modelscan.error import (
     DependencyError,
     JsonDecodeError,
 )
 from modelscan.issues import Issue, IssueCode, IssueSeverity, OperatorIssueDetails
 from modelscan.scanners.scan import ScanBase, ScanResults
 from modelscan.model import Model
+from modelscan.settings import DefaultModelFormats
 
 logger = logging.getLogger("modelscan")
 
 
 class SavedModelScan(ScanBase):
     def scan(
         self,
         model: Model,
     ) -> Optional[ScanResults]:
-        if "tf_saved_model" not in model.get_context("formats"):
+        if DefaultModelFormats.TENSORFLOW not in model.get_context("formats"):
             return None
 
         dep_error = self.handle_binary_dependencies()
         if dep_error:
             return ScanResults(
                 [],
                 [
```

### Comparing `modelscan-0.7.3/modelscan/scanners/scan.py` & `modelscan-0.7.4/modelscan/scanners/scan.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/settings.py` & `modelscan-0.7.4/modelscan/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 import tomlkit
 
+from enum import Enum
 from typing import Any
 
 from modelscan._version import __version__
 
+
+class DefaultModelFormats(Enum):
+    TENSORFLOW = "tensorflow"
+    KERAS_H5 = "keras_h5"
+    KERAS = "keras"
+    NUMPY = "numpy"
+    PYTORCH = "pytorch"
+    PICKLE = "pickle"
+
+
 DEFAULT_REPORTING_MODULES = {
     "console": "modelscan.reports.ConsoleReport",
     "json": "modelscan.reports.JSONReport",
 }
 
 DEFAULT_SETTINGS = {
     "modelscan_version": __version__,
@@ -55,21 +66,20 @@
             "enabled": True,
             "supported_extensions": [".bin", ".pt", ".pth", ".ckpt"],
         },
     },
     "middlewares": {
         "modelscan.middlewares.FormatViaExtensionMiddleware": {
             "formats": {
-                "tf": [".pb"],
-                "tf_saved_model": [".pb"],
-                "keras_h5": [".h5"],
-                "keras": [".keras"],
-                "numpy": [".npy"],
-                "pytorch": [".bin", ".pt", ".pth", ".ckpt"],
-                "pickle": [
+                DefaultModelFormats.TENSORFLOW: [".pb"],
+                DefaultModelFormats.KERAS_H5: [".h5"],
+                DefaultModelFormats.KERAS: [".keras"],
+                DefaultModelFormats.NUMPY: [".npy"],
+                DefaultModelFormats.PYTORCH: [".bin", ".pt", ".pth", ".ckpt"],
+                DefaultModelFormats.PICKLE: [
                     ".pkl",
                     ".pickle",
                     ".joblib",
                     ".dill",
                     ".dat",
                     ".data",
                 ],
```

### Comparing `modelscan-0.7.3/modelscan/skip.py` & `modelscan-0.7.4/modelscan/skip.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/tools/LICENSE` & `modelscan-0.7.4/modelscan/tools/LICENSE`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/tools/cli_utils.py` & `modelscan-0.7.4/modelscan/tools/cli_utils.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/tools/picklescanner.py` & `modelscan-0.7.4/modelscan/tools/picklescanner.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/modelscan/tools/utils.py` & `modelscan-0.7.4/modelscan/tools/utils.py`

 * *Files identical despite different names*

### Comparing `modelscan-0.7.3/pyproject.toml` & `modelscan-0.7.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelscan"
-version = "0.7.3"
+version = "0.7.4"
 description = "The modelscan package is a cli tool for detecting unsafe operations in model files across various model serialization formats."
 authors = ["ProtectAI <community@protectai.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{ include = "modelscan" }]
 exclude = ["tests/*", "Makefile"]
```

### Comparing `modelscan-0.7.3/PKG-INFO` & `modelscan-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelscan
-Version: 0.7.3
+Version: 0.7.4
 Summary: The modelscan package is a cli tool for detecting unsafe operations in model files across various model serialization formats.
 License: Apache-2.0
 Author: ProtectAI
 Author-email: community@protectai.com
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

