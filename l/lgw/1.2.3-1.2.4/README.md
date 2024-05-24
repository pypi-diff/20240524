# Comparing `tmp/lgw-1.2.3.tar.gz` & `tmp/lgw-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lgw-1.2.3.tar", max compression
+gzip compressed data, was "lgw-1.2.4.tar", max compression
```

## Comparing `lgw-1.2.3.tar` & `lgw-1.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2024-05-24 13:59:06.775185 lgw-1.2.3/LICENSE
--rw-r--r--   0        0        0     8974 2024-05-24 13:59:06.775859 lgw-1.2.3/README.md
--rw-r--r--   0        0        0       36 2024-05-24 13:59:06.776063 lgw-1.2.3/lgw/__init__.py
--rw-r--r--   0        0        0     5773 2024-05-24 13:59:06.776222 lgw-1.2.3/lgw/api_gateway.py
--rw-r--r--   0        0        0     3585 2024-05-24 13:59:06.776367 lgw-1.2.3/lgw/api_gateway_domain.py
--rw-r--r--   0        0        0     5805 2024-05-24 13:59:06.776634 lgw-1.2.3/lgw/lambda_bundle.py
--rw-r--r--   0        0        0     8764 2024-05-24 13:59:06.776803 lgw-1.2.3/lgw/lambda_util.py
--rw-r--r--   0        0        0     8717 2024-05-24 13:59:06.776949 lgw-1.2.3/lgw/main.py
--rw-r--r--   0        0        0     2283 2024-05-24 13:59:06.777091 lgw-1.2.3/lgw/route53.py
--rw-r--r--   0        0        0      478 2024-05-24 13:59:06.777234 lgw-1.2.3/lgw/s3.py
--rw-r--r--   0        0        0     1402 2024-05-24 13:59:06.777425 lgw-1.2.3/lgw/settings.py
--rw-r--r--   0        0        0      284 2024-05-24 13:59:06.777777 lgw-1.2.3/lgw/util.py
--rw-r--r--   0        0        0       22 2024-05-24 15:14:25.306300 lgw-1.2.3/lgw/version.py
--rw-r--r--   0        0        0     1227 2024-05-24 15:14:17.946984 lgw-1.2.3/pyproject.toml
--rw-r--r--   0        0        0    10056 1970-01-01 00:00:00.000000 lgw-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 13:59:06.775185 lgw-1.2.4/LICENSE
+-rw-r--r--   0        0        0     8974 2024-05-24 13:59:06.775859 lgw-1.2.4/README.md
+-rw-r--r--   0        0        0       36 2024-05-24 13:59:06.776063 lgw-1.2.4/lgw/__init__.py
+-rw-r--r--   0        0        0     5773 2024-05-24 13:59:06.776222 lgw-1.2.4/lgw/api_gateway.py
+-rw-r--r--   0        0        0     3585 2024-05-24 13:59:06.776367 lgw-1.2.4/lgw/api_gateway_domain.py
+-rw-r--r--   0        0        0     5805 2024-05-24 13:59:06.776634 lgw-1.2.4/lgw/lambda_bundle.py
+-rw-r--r--   0        0        0     8764 2024-05-24 13:59:06.776803 lgw-1.2.4/lgw/lambda_util.py
+-rw-r--r--   0        0        0     8717 2024-05-24 13:59:06.776949 lgw-1.2.4/lgw/main.py
+-rw-r--r--   0        0        0     2283 2024-05-24 13:59:06.777091 lgw-1.2.4/lgw/route53.py
+-rw-r--r--   0        0        0      478 2024-05-24 13:59:06.777234 lgw-1.2.4/lgw/s3.py
+-rw-r--r--   0        0        0     1402 2024-05-24 13:59:06.777425 lgw-1.2.4/lgw/settings.py
+-rw-r--r--   0        0        0      284 2024-05-24 13:59:06.777777 lgw-1.2.4/lgw/util.py
+-rw-r--r--   0        0        0       22 2024-05-24 15:33:50.303619 lgw-1.2.4/lgw/version.py
+-rw-r--r--   0        0        0     1227 2024-05-24 15:33:56.943431 lgw-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0    10056 1970-01-01 00:00:00.000000 lgw-1.2.4/PKG-INFO
```

### Comparing `lgw-1.2.3/LICENSE` & `lgw-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lgw-1.2.3/README.md` & `lgw-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `lgw-1.2.3/lgw/api_gateway.py` & `lgw-1.2.4/lgw/api_gateway.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.3/lgw/api_gateway_domain.py` & `lgw-1.2.4/lgw/api_gateway_domain.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.3/lgw/lambda_bundle.py` & `lgw-1.2.4/lgw/lambda_bundle.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.3/lgw/lambda_util.py` & `lgw-1.2.4/lgw/lambda_util.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.3/lgw/main.py` & `lgw-1.2.4/lgw/main.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.3/lgw/route53.py` & `lgw-1.2.4/lgw/route53.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.3/lgw/settings.py` & `lgw-1.2.4/lgw/settings.py`

 * *Files identical despite different names*

### Comparing `lgw-1.2.3/pyproject.toml` & `lgw-1.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lgw"
-version = "1.2.3"
+version = "1.2.4"
 description = "Configure an AWS Gateway in front of a Lambda function."
 authors = ["Edward Q. Bridges <ebridges@roja.cc>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/ebridges/lgw"
 documentation = "https://github.com/ebridges/lgw/blob/master/README.md"
 classifiers = ["Topic :: Software Development :: Build Tools"]
```

### Comparing `lgw-1.2.3/PKG-INFO` & `lgw-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lgw
-Version: 1.2.3
+Version: 1.2.4
 Summary: Configure an AWS Gateway in front of a Lambda function.
 Home-page: https://github.com/ebridges/lgw
 License: Apache-2.0
 Author: Edward Q. Bridges
 Author-email: ebridges@roja.cc
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lgw Version: 1.2.3 Summary: Configure an AWS
+Metadata-Version: 2.1 Name: lgw Version: 1.2.4 Summary: Configure an AWS
 Gateway in front of a Lambda function. Home-page: https://github.com/ebridges/
 lgw License: Apache-2.0 Author: Edward Q. Bridges Author-email:
 ebridges@roja.cc Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

