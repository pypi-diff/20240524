# Comparing `tmp/quart_rpc-1.3.1.tar.gz` & `tmp/quart_rpc-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quart_rpc-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quart_rpc-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quart_rpc-1.3.1.tar` & `quart_rpc-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     3104 2024-04-17 12:02:54.084518 quart_rpc-1.3.1/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 quart_rpc-1.3.1/LICENSE
--rw-r--r--   0        0        0     4133 2024-05-24 06:19:50.481842 quart_rpc-1.3.1/README.md
--rw-r--r--   0        0        0      989 2024-04-24 13:25:20.658274 quart_rpc-1.3.1/app/__init__.py
--rw-r--r--   0        0        0     1856 2024-04-18 11:05:10.605491 quart_rpc-1.3.1/app/templates/index.html
--rw-r--r--   0        0        0      741 2024-04-16 14:38:49.181823 quart_rpc-1.3.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-24 06:19:58.114648 quart_rpc-1.3.1/quart_rpc/__init__.py
--rw-r--r--   0        0        0      164 2024-04-18 09:17:46.763194 quart_rpc-1.3.1/quart_rpc/latest.py
--rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 quart_rpc-1.3.1/quart_rpc/version_1_0/__init__.py
--rw-r--r--   0        0        0      160 2024-04-18 09:56:48.552074 quart_rpc-1.3.1/quart_rpc/version_1_0/_protocols.py
--rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 quart_rpc-1.3.1/quart_rpc/version_1_0/auth_session_key.py
--rw-r--r--   0        0        0      130 2024-04-18 11:05:19.979675 quart_rpc-1.3.1/quart_rpc/version_1_0/model.py
--rw-r--r--   0        0        0      480 2024-04-18 11:05:19.992185 quart_rpc-1.3.1/quart_rpc/version_1_0/request.py
--rw-r--r--   0        0        0     1159 2024-04-24 18:57:24.265236 quart_rpc-1.3.1/quart_rpc/version_1_0/response.py
--rw-r--r--   0        0        0     5484 2024-04-18 11:05:19.972570 quart_rpc-1.3.1/quart_rpc/version_1_0/rpc.py
--rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 quart_rpc-1.3.1/quart_rpc/version_1_0/utilities.py
--rw-r--r--   0        0        0       15 2024-04-16 14:40:40.344290 quart_rpc-1.3.1/requirements/development.txt
--rw-r--r--   0        0        0       24 2024-04-17 12:22:19.294586 quart_rpc-1.3.1/requirements/main.txt
--rw-r--r--   0        0        0      366 2024-04-24 13:25:20.658005 quart_rpc-1.3.1/test.py
--rw-r--r--   0        0        0     4772 1970-01-01 00:00:00.000000 quart_rpc-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3104 2024-04-17 12:02:54.084518 quart_rpc-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 quart_rpc-1.4.0/LICENSE
+-rw-r--r--   0        0        0     4133 2024-05-24 06:19:50.481842 quart_rpc-1.4.0/README.md
+-rw-r--r--   0        0        0      989 2024-04-24 13:25:20.658274 quart_rpc-1.4.0/app/__init__.py
+-rw-r--r--   0        0        0     1856 2024-04-18 11:05:10.605491 quart_rpc-1.4.0/app/templates/index.html
+-rw-r--r--   0        0        0      741 2024-04-16 14:38:49.181823 quart_rpc-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-24 09:35:09.674485 quart_rpc-1.4.0/quart_rpc/__init__.py
+-rw-r--r--   0        0        0       41 2024-05-24 09:18:48.891005 quart_rpc-1.4.0/quart_rpc/exceptions.py
+-rw-r--r--   0        0        0      164 2024-04-18 09:17:46.763194 quart_rpc-1.4.0/quart_rpc/latest.py
+-rw-r--r--   0        0        0     2001 2024-05-24 09:25:58.870814 quart_rpc-1.4.0/quart_rpc/validation.py
+-rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 quart_rpc-1.4.0/quart_rpc/version_1_0/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-18 09:56:48.552074 quart_rpc-1.4.0/quart_rpc/version_1_0/_protocols.py
+-rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 quart_rpc-1.4.0/quart_rpc/version_1_0/auth_session_key.py
+-rw-r--r--   0        0        0      130 2024-04-18 11:05:19.979675 quart_rpc-1.4.0/quart_rpc/version_1_0/model.py
+-rw-r--r--   0        0        0      480 2024-04-18 11:05:19.992185 quart_rpc-1.4.0/quart_rpc/version_1_0/request.py
+-rw-r--r--   0        0        0     1159 2024-04-24 18:57:24.265236 quart_rpc-1.4.0/quart_rpc/version_1_0/response.py
+-rw-r--r--   0        0        0     5484 2024-04-18 11:05:19.972570 quart_rpc-1.4.0/quart_rpc/version_1_0/rpc.py
+-rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 quart_rpc-1.4.0/quart_rpc/version_1_0/utilities.py
+-rw-r--r--   0        0        0       15 2024-04-16 14:40:40.344290 quart_rpc-1.4.0/requirements/development.txt
+-rw-r--r--   0        0        0       24 2024-04-17 12:22:19.294586 quart_rpc-1.4.0/requirements/main.txt
+-rw-r--r--   0        0        0      366 2024-04-24 13:25:20.658005 quart_rpc-1.4.0/test.py
+-rw-r--r--   0        0        0     4772 1970-01-01 00:00:00.000000 quart_rpc-1.4.0/PKG-INFO
```

### Comparing `quart_rpc-1.3.1/.gitignore` & `quart_rpc-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.3.1/LICENSE` & `quart_rpc-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.3.1/README.md` & `quart_rpc-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.3.1/app/__init__.py` & `quart_rpc-1.4.0/app/__init__.py`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.3.1/app/templates/index.html` & `quart_rpc-1.4.0/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.3.1/pyproject.toml` & `quart_rpc-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.3.1/quart_rpc/version_1_0/response.py` & `quart_rpc-1.4.0/quart_rpc/version_1_0/response.py`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.3.1/quart_rpc/version_1_0/rpc.py` & `quart_rpc-1.4.0/quart_rpc/version_1_0/rpc.py`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.3.1/quart_rpc/version_1_0/utilities.py` & `quart_rpc-1.4.0/quart_rpc/version_1_0/utilities.py`

 * *Files identical despite different names*

### Comparing `quart_rpc-1.3.1/PKG-INFO` & `quart_rpc-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quart-rpc
-Version: 1.3.1
+Version: 1.4.0
 Summary: Turn Quart into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

