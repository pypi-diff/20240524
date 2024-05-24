# Comparing `tmp/input4mips_validation-0.3.3.tar.gz` & `tmp/input4mips_validation-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "input4mips_validation-0.3.3.tar", max compression
+gzip compressed data, was "input4mips_validation-0.3.4.tar", max compression
```

## Comparing `input4mips_validation-0.3.3.tar` & `input4mips_validation-0.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1685 2024-05-23 11:06:41.505255 input4mips_validation-0.3.3/LICENCE
--rw-r--r--   0        0        0     3810 2024-05-23 11:06:41.505255 input4mips_validation-0.3.3/README.md
--rw-r--r--   0        0        0     5606 2024-05-23 11:06:41.505255 input4mips_validation-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      171 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/__init__.py
--rw-r--r--   0        0        0     3795 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/attrs_helpers.py
--rw-r--r--   0        0        0     1164 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/cli/__init__.py
--rw-r--r--   0        0        0     1031 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/cli/cli_logging.py
--rw-r--r--   0        0        0       39 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/__init__.py
--rw-r--r--   0        0        0     5577 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/constants.py
--rw-r--r--   0        0        0      613 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/file_id.py
--rw-r--r--   0        0        0     3688 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/inference/__init__.py
--rw-r--r--   0        0        0     4384 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/__init__.py
--rw-r--r--   0        0        0     6986 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py
--rw-r--r--   0        0        0      740 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py
--rw-r--r--   0        0        0     2257 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py
--rw-r--r--   0        0        0      779 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/email.py
--rw-r--r--   0        0        0      634 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/uuid.py
--rw-r--r--   0        0        0    10284 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/dataset.py
--rw-r--r--   0        0        0      674 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/exceptions.py
--rw-r--r--   0        0        0     3553 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/metadata.py
--rw-r--r--   0        0        0        0 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/py.typed
--rw-r--r--   0        0        0     1429 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/testing.py
--rw-r--r--   0        0        0     5886 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/time.py
--rw-r--r--   0        0        0     1691 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/validation/__init__.py
--rw-r--r--   0        0        0     4207 2024-05-23 11:06:41.509255 input4mips_validation-0.3.3/src/input4mips_validation/xarray_helpers.py
--rw-r--r--   0        0        0     4942 1970-01-01 00:00:00.000000 input4mips_validation-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1685 2024-05-24 11:21:45.804433 input4mips_validation-0.3.4/LICENCE
+-rw-r--r--   0        0        0     3810 2024-05-24 11:21:45.804433 input4mips_validation-0.3.4/README.md
+-rw-r--r--   0        0        0     5606 2024-05-24 11:21:45.804433 input4mips_validation-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      171 2024-05-24 11:21:45.804433 input4mips_validation-0.3.4/src/input4mips_validation/__init__.py
+-rw-r--r--   0        0        0     3795 2024-05-24 11:21:45.804433 input4mips_validation-0.3.4/src/input4mips_validation/attrs_helpers.py
+-rw-r--r--   0        0        0     1164 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/cli/__init__.py
+-rw-r--r--   0        0        0     1031 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/cli/cli_logging.py
+-rw-r--r--   0        0        0       39 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/__init__.py
+-rw-r--r--   0        0        0     6621 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/constants.py
+-rw-r--r--   0        0        0      613 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/file_id.py
+-rw-r--r--   0        0        0     3688 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/inference/__init__.py
+-rw-r--r--   0        0        0     4384 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/__init__.py
+-rw-r--r--   0        0        0     6986 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py
+-rw-r--r--   0        0        0      740 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py
+-rw-r--r--   0        0        0     2257 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py
+-rw-r--r--   0        0        0      779 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/email.py
+-rw-r--r--   0        0        0      634 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/uuid.py
+-rw-r--r--   0        0        0    10284 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/dataset.py
+-rw-r--r--   0        0        0      674 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/exceptions.py
+-rw-r--r--   0        0        0     3553 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/metadata.py
+-rw-r--r--   0        0        0        0 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/py.typed
+-rw-r--r--   0        0        0     1429 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/testing.py
+-rw-r--r--   0        0        0     5886 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/time.py
+-rw-r--r--   0        0        0     1691 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/validation/__init__.py
+-rw-r--r--   0        0        0     4207 2024-05-24 11:21:45.808433 input4mips_validation-0.3.4/src/input4mips_validation/xarray_helpers.py
+-rw-r--r--   0        0        0     4942 1970-01-01 00:00:00.000000 input4mips_validation-0.3.4/PKG-INFO
```

### Comparing `input4mips_validation-0.3.3/LICENCE` & `input4mips_validation-0.3.4/LICENCE`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/README.md` & `input4mips_validation-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/pyproject.toml` & `input4mips_validation-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "input4mips-validation"
-version = "0.3.3"
+version = "0.3.4"
 description = "Validation of input4MIPs data (checking file formats, metadata etc.)."
 authors = ["Zebedee Nicholls <zebedee.nicholls@climate-resource.com>"]
 readme = "README.md"
 packages = [{include = "input4mips_validation", from = "src"}]
 license = "BSD-3-Clause"
 include = ["LICENCE"]  # poetry uses US English so assumes it will be spelt LICENSE
```

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/attrs_helpers.py` & `input4mips_validation-0.3.4/src/input4mips_validation/attrs_helpers.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/cli/__init__.py` & `input4mips_validation-0.3.4/src/input4mips_validation/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/cli/cli_logging.py` & `input4mips_validation-0.3.4/src/input4mips_validation/cli/cli_logging.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/file_id.py` & `input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/file_id.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/inference/__init__.py` & `input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/__init__.py` & `input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py` & `input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py` & `input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py` & `input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/email.py` & `input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/email.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/controlled_vocabularies/validators/uuid.py` & `input4mips_validation-0.3.4/src/input4mips_validation/controlled_vocabularies/validators/uuid.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/dataset.py` & `input4mips_validation-0.3.4/src/input4mips_validation/dataset.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/exceptions.py` & `input4mips_validation-0.3.4/src/input4mips_validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/metadata.py` & `input4mips_validation-0.3.4/src/input4mips_validation/metadata.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/testing.py` & `input4mips_validation-0.3.4/src/input4mips_validation/testing.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/time.py` & `input4mips_validation-0.3.4/src/input4mips_validation/time.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/validation/__init__.py` & `input4mips_validation-0.3.4/src/input4mips_validation/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/src/input4mips_validation/xarray_helpers.py` & `input4mips_validation-0.3.4/src/input4mips_validation/xarray_helpers.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.3/PKG-INFO` & `input4mips_validation-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: input4mips-validation
-Version: 0.3.3
+Version: 0.3.4
 Summary: Validation of input4MIPs data (checking file formats, metadata etc.).
 License: BSD-3-Clause
 Author: Zebedee Nicholls
 Author-email: zebedee.nicholls@climate-resource.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

