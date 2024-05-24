# Comparing `tmp/wacz_signing-0.3.8.tar.gz` & `tmp/wacz_signing-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wacz_signing-0.3.8.tar", max compression
+gzip compressed data, was "wacz_signing-0.3.9.tar", max compression
```

## Comparing `wacz_signing-0.3.8.tar` & `wacz_signing-0.3.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2022-10-01 19:18:01.340865 wacz_signing-0.3.8/COPYING
--rw-r--r--   0        0        0     3921 2023-03-15 19:24:50.140830 wacz_signing-0.3.8/README.md
--rw-r--r--   0        0        0      538 2024-04-19 13:25:37.777886 wacz_signing-0.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-01 14:24:50.997566 wacz_signing-0.3.8/wacz_signing/__init__.py
--rw-r--r--   0        0        0     5688 2022-10-05 19:40:58.732093 wacz_signing-0.3.8/wacz_signing/material.py
--rw-r--r--   0        0        0    11529 2024-02-29 12:43:25.426631 wacz_signing-0.3.8/wacz_signing/signer.py
--rw-r--r--   0        0        0     4748 1970-01-01 00:00:00.000000 wacz_signing-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-01 19:18:01.340865 wacz_signing-0.3.9/COPYING
+-rw-r--r--   0        0        0     3921 2023-03-15 19:24:50.140830 wacz_signing-0.3.9/README.md
+-rw-r--r--   0        0        0      538 2024-05-24 18:09:02.665690 wacz_signing-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-10-01 14:24:50.997566 wacz_signing-0.3.9/wacz_signing/__init__.py
+-rw-r--r--   0        0        0     5688 2022-10-05 19:40:58.732093 wacz_signing-0.3.9/wacz_signing/material.py
+-rw-r--r--   0        0        0    11529 2024-02-29 12:43:25.426631 wacz_signing-0.3.9/wacz_signing/signer.py
+-rw-r--r--   0        0        0     4748 1970-01-01 00:00:00.000000 wacz_signing-0.3.9/PKG-INFO
```

### Comparing `wacz_signing-0.3.8/COPYING` & `wacz_signing-0.3.9/COPYING`

 * *Files identical despite different names*

### Comparing `wacz_signing-0.3.8/README.md` & `wacz_signing-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `wacz_signing-0.3.8/pyproject.toml` & `wacz_signing-0.3.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wacz_signing"
-version = "0.3.8"
+version = "0.3.9"
 description = "A library for signing and timestamping file hashes"
 authors = ["Ben Steinberg <bsteinberg@law.harvard.edu>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `wacz_signing-0.3.8/wacz_signing/material.py` & `wacz_signing-0.3.9/wacz_signing/material.py`

 * *Files identical despite different names*

### Comparing `wacz_signing-0.3.8/wacz_signing/signer.py` & `wacz_signing-0.3.9/wacz_signing/signer.py`

 * *Files identical despite different names*

### Comparing `wacz_signing-0.3.8/PKG-INFO` & `wacz_signing-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wacz_signing
-Version: 0.3.8
+Version: 0.3.9
 Summary: A library for signing and timestamping file hashes
 License: GPL-3.0-or-later
 Author: Ben Steinberg
 Author-email: bsteinberg@law.harvard.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wacz_signing Version: 0.3.8 Summary: A library for
+Metadata-Version: 2.1 Name: wacz_signing Version: 0.3.9 Summary: A library for
 signing and timestamping file hashes License: GPL-3.0-or-later Author: Ben
 Steinberg Author-email: bsteinberg@law.harvard.edu Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later
 (GPLv3+) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: cryptography
```

