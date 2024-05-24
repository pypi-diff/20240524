# Comparing `tmp/buzz_client-1.1.2.tar.gz` & `tmp/buzz_client-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buzz_client-1.1.2.tar", max compression
+gzip compressed data, was "buzz_client-1.1.3.tar", max compression
```

## Comparing `buzz_client-1.1.2.tar` & `buzz_client-1.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     2288 2024-05-21 10:16:10.377792 buzz_client-1.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-22 12:47:42.845489 buzz_client-1.1.2/buzz_client/__init__.py
--rw-r--r--   0        0        0     3702 2024-05-22 13:24:19.181286 buzz_client-1.1.2/buzz_client/cli_parser.py
--rw-r--r--   0        0        0     2617 2024-05-22 09:00:42.371384 buzz_client-1.1.2/buzz_client/client.py
--rw-r--r--   0        0        0      418 2024-05-22 13:24:19.182144 buzz_client-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2890 1970-01-01 00:00:00.000000 buzz_client-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2288 2024-05-21 10:16:10.377792 buzz_client-1.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 12:47:42.845489 buzz_client-1.1.3/buzz_client/__init__.py
+-rwxr-xr-x   0        0        0     5227 2024-05-22 13:24:19.181523 buzz_client-1.1.3/buzz_client/cli.py
+-rw-r--r--   0        0        0     3702 2024-05-22 13:24:19.181286 buzz_client-1.1.3/buzz_client/cli_parser.py
+-rw-r--r--   0        0        0     2617 2024-05-22 09:00:42.371384 buzz_client-1.1.3/buzz_client/client.py
+-rw-r--r--   0        0        0      430 2024-05-24 08:00:25.970577 buzz_client-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2890 1970-01-01 00:00:00.000000 buzz_client-1.1.3/PKG-INFO
```

### Comparing `buzz_client-1.1.2/README.md` & `buzz_client-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `buzz_client-1.1.2/buzz_client/cli_parser.py` & `buzz_client-1.1.3/buzz_client/cli_parser.py`

 * *Files identical despite different names*

### Comparing `buzz_client-1.1.2/buzz_client/client.py` & `buzz_client-1.1.3/buzz_client/client.py`

 * *Files identical despite different names*

### Comparing `buzz_client-1.1.2/PKG-INFO` & `buzz_client-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buzz-client
-Version: 1.1.2
+Version: 1.1.3
 Summary: A client for Buzz API
 License: GPL
 Author: Andrea Mistrali
 Author-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: buzz-client Version: 1.1.2 Summary: A client for
+Metadata-Version: 2.1 Name: buzz-client Version: 1.1.3 Summary: A client for
 Buzz API License: GPL Author: Andrea Mistrali Author-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: pyyaml
 (>=6.0.1,<7.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
 scriptonite (>=1.0.3,<2.0.0) Description-Content-Type: text/markdown #
```

