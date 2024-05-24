# Comparing `tmp/qpyr-0.1.8.tar.gz` & `tmp/qpyr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qpyr-0.1.8.tar", max compression
+gzip compressed data, was "qpyr-0.1.9.tar", max compression
```

## Comparing `qpyr-0.1.8.tar` & `qpyr-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-07-12 09:48:31.886361 qpyr-0.1.8/LICENSE
--rw-r--r--   0        0        0      876 2023-12-09 10:29:37.684359 qpyr-0.1.8/README.md
--rw-r--r--   0        0        0      600 2023-12-09 10:56:19.711212 qpyr-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       27 2023-12-06 08:28:10.254229 qpyr-0.1.8/qpyr/__init__.py
--rw-r--r--   0        0        0     3589 2023-12-08 08:48:14.334295 qpyr-0.1.8/qpyr/data_masking.py
--rw-r--r--   0        0        0    14441 2023-12-08 09:35:36.050136 qpyr-0.1.8/qpyr/draw.py
--rw-r--r--   0        0        0     4048 2023-12-05 21:11:56.644258 qpyr-0.1.8/qpyr/encode.py
--rw-r--r--   0        0        0     3964 2023-12-08 08:48:14.337657 qpyr-0.1.8/qpyr/error_correction.py
--rw-r--r--   0        0        0      195 2023-12-08 09:39:51.470438 qpyr-0.1.8/qpyr/main.py
--rw-r--r--   0        0        0     1915 2023-12-05 21:11:56.647830 qpyr-0.1.8/qpyr/static.py
--rw-r--r--   0        0        0     2125 2023-12-05 21:11:56.648965 qpyr-0.1.8/qpyr/utils.py
--rw-r--r--   0        0        0     9264 2023-12-06 08:35:17.473542 qpyr-0.1.8/qrcode-example.png
--rw-r--r--   0        0        0     1446 1970-01-01 00:00:00.000000 qpyr-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-12 09:48:31.886361 qpyr-0.1.9/LICENSE
+-rw-r--r--   0        0        0      931 2023-12-09 11:02:15.095515 qpyr-0.1.9/README.md
+-rw-r--r--   0        0        0      567 2023-12-09 10:59:59.205463 qpyr-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-12-06 08:28:10.254229 qpyr-0.1.9/qpyr/__init__.py
+-rw-r--r--   0        0        0     3589 2023-12-08 08:48:14.334295 qpyr-0.1.9/qpyr/data_masking.py
+-rw-r--r--   0        0        0    14441 2023-12-08 09:35:36.050136 qpyr-0.1.9/qpyr/draw.py
+-rw-r--r--   0        0        0     4048 2023-12-05 21:11:56.644258 qpyr-0.1.9/qpyr/encode.py
+-rw-r--r--   0        0        0     3964 2023-12-08 08:48:14.337657 qpyr-0.1.9/qpyr/error_correction.py
+-rw-r--r--   0        0        0      195 2023-12-08 09:39:51.470438 qpyr-0.1.9/qpyr/main.py
+-rw-r--r--   0        0        0     1915 2023-12-05 21:11:56.647830 qpyr-0.1.9/qpyr/static.py
+-rw-r--r--   0        0        0     2125 2023-12-05 21:11:56.648965 qpyr-0.1.9/qpyr/utils.py
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 qpyr-0.1.9/PKG-INFO
```

### Comparing `qpyr-0.1.8/LICENSE` & `qpyr-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qpyr-0.1.8/README.md` & `qpyr-0.1.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 ## Basic usage
 To use the package, import and call the `main` function as follows:
 
 ```python
 import qpyr
 qpyr.main("google.com")
 ```
-<img src="./qrcode-example.png" alt="QR Code" width="200" height="200"/>
+<img src="https://github.com/sabih-h/qpyr/blob/cleanup/docs/static/qrcode-example.png" alt="QR Code" width="200" height="200"/>
 
 
 ## Contributing
 Contributions are warmly welcomed! Whether you're tackling a bug, adding a new feature, or improving documentation, your input is invaluable in making this library better.
```

### Comparing `qpyr-0.1.8/pyproject.toml` & `qpyr-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [tool.poetry]
 name = "qpyr"
-version = "0.1.8"
+version = "0.1.9"
 description = "Create QR Codes."
 authors = ["Sabi"]
 license = "Apache-2.0"
 readme = "README.md"
 keywords = ["qr", "qrcode", "qrcode-generator"]
-include = ["qrcode-example.png"]
 
 [tool.poetry.urls]
 "Source" = "https://github.com/sabih-h/qpyr"
 "Documentation" = "https://sabih-h.github.io/qpyr/"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `qpyr-0.1.8/qpyr/data_masking.py` & `qpyr-0.1.9/qpyr/data_masking.py`

 * *Files identical despite different names*

### Comparing `qpyr-0.1.8/qpyr/draw.py` & `qpyr-0.1.9/qpyr/draw.py`

 * *Files identical despite different names*

### Comparing `qpyr-0.1.8/qpyr/encode.py` & `qpyr-0.1.9/qpyr/encode.py`

 * *Files identical despite different names*

### Comparing `qpyr-0.1.8/qpyr/error_correction.py` & `qpyr-0.1.9/qpyr/error_correction.py`

 * *Files identical despite different names*

### Comparing `qpyr-0.1.8/qpyr/static.py` & `qpyr-0.1.9/qpyr/static.py`

 * *Files identical despite different names*

### Comparing `qpyr-0.1.8/qpyr/utils.py` & `qpyr-0.1.9/qpyr/utils.py`

 * *Files identical despite different names*

### Comparing `qpyr-0.1.8/PKG-INFO` & `qpyr-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpyr
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create QR Codes.
 License: Apache-2.0
 Keywords: qr,qrcode,qrcode-generator
 Author: Sabi
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -31,13 +31,13 @@
 ## Basic usage
 To use the package, import and call the `main` function as follows:
 
 ```python
 import qpyr
 qpyr.main("google.com")
 ```
-<img src="./qrcode-example.png" alt="QR Code" width="200" height="200"/>
+<img src="https://github.com/sabih-h/qpyr/blob/cleanup/docs/static/qrcode-example.png" alt="QR Code" width="200" height="200"/>
 
 
 ## Contributing
 Contributions are warmly welcomed! Whether you're tackling a bug, adding a new feature, or improving documentation, your input is invaluable in making this library better.
```

