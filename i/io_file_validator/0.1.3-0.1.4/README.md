# Comparing `tmp/io_file_validator-0.1.3.tar.gz` & `tmp/io_file_validator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "io_file_validator-0.1.3.tar", max compression
+gzip compressed data, was "io_file_validator-0.1.4.tar", max compression
```

## Comparing `io_file_validator-0.1.3.tar` & `io_file_validator-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2440 2024-05-19 20:29:35.171446 io_file_validator-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-19 20:29:35.171446 io_file_validator-0.1.3/io_file_validator/__init__.py
--rw-r--r--   0        0        0     3961 2024-05-19 20:29:35.171446 io_file_validator-0.1.3/io_file_validator/validator.py
--rw-r--r--   0        0        0     1071 2024-05-19 20:29:35.171446 io_file_validator-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3130 1970-01-01 00:00:00.000000 io_file_validator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2440 2024-05-24 04:41:07.385898 io_file_validator-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 04:41:07.385898 io_file_validator-0.1.4/io_file_validator/__init__.py
+-rw-r--r--   0        0        0     3961 2024-05-24 04:41:07.385898 io_file_validator-0.1.4/io_file_validator/validator.py
+-rw-r--r--   0        0        0     1056 2024-05-24 04:41:07.385898 io_file_validator-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 io_file_validator-0.1.4/PKG-INFO
```

### Comparing `io_file_validator-0.1.3/README.md` & `io_file_validator-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `io_file_validator-0.1.3/io_file_validator/validator.py` & `io_file_validator-0.1.4/io_file_validator/validator.py`

 * *Files identical despite different names*

### Comparing `io_file_validator-0.1.3/pyproject.toml` & `io_file_validator-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "io_file_validator"
-version = "0.1.3"
+version = "0.1.4"
 description = "File Validator Tool helps you validate your data with a plethora of formats"
 authors = ["Manrique Vargas <machomaxg@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 validators = "^0.28.1"
 pipx = "^1.5.0"
 wheel = "*"
-pytest = "7.4.0"
-requests = "2.31.0"
+requests = "^2.31.0"
 pandera = { version = "^0.7.2", extras = ["io"] }
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 pytest = "*"
 pylint = "^3.2.0"
 twine = "*"
-pydiggs = "0.1.3"
+pydiggs = "^0.1.3"
 lxml = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `io_file_validator-0.1.3/PKG-INFO` & `io_file_validator-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: io_file_validator
-Version: 0.1.3
+Version: 0.1.4
 Summary: File Validator Tool helps you validate your data with a plethora of formats
 Author: Manrique Vargas
 Author-email: machomaxg@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandera[io] (>=0.7.2,<0.8.0)
 Requires-Dist: pipx (>=1.5.0,<2.0.0)
-Requires-Dist: pytest (==7.4.0)
-Requires-Dist: requests (==2.31.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: validators (>=0.28.1,<0.29.0)
 Requires-Dist: wheel
 Description-Content-Type: text/markdown
 
 # Welcome to IO Bytes File Validator!
```

