# Comparing `tmp/burrow_cli-0.1.5.tar.gz` & `tmp/burrow_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burrow_cli-0.1.5.tar", max compression
+gzip compressed data, was "burrow_cli-0.1.6.tar", max compression
```

## Comparing `burrow_cli-0.1.5.tar` & `burrow_cli-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2024-05-24 03:38:27.323179 burrow_cli-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-05-23 13:49:53.573442 burrow_cli-0.1.5/burrow_cli/__init__.py
--rw-r--r--   0        0        0     4155 2024-05-24 06:25:31.321396 burrow_cli-0.1.5/burrow_cli/main.py
--rw-r--r--   0        0        0      602 2024-05-24 06:25:43.570398 burrow_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 burrow_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-24 03:38:27.323179 burrow_cli-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 13:49:53.573442 burrow_cli-0.1.6/burrow_cli/__init__.py
+-rw-r--r--   0        0        0     6811 2024-05-24 08:35:14.086251 burrow_cli-0.1.6/burrow_cli/main.py
+-rw-r--r--   0        0        0      602 2024-05-24 08:35:43.914925 burrow_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 burrow_cli-0.1.6/PKG-INFO
```

### Comparing `burrow_cli-0.1.5/README.md` & `burrow_cli-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `burrow_cli-0.1.5/pyproject.toml` & `burrow_cli-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burrow-cli"
-version = "0.1.5"
+version = "0.1.6"
 description = "Burrow command line app, you can launch a fractional GPU contaienr with this app, and share a link of the container to your friends, you and your friends can work colloratively together"
 authors = ["Vurtne Saerdna <vurtnesaerdna@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 burrow = "burrow_cli.main:app"
```

### Comparing `burrow_cli-0.1.5/PKG-INFO` & `burrow_cli-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burrow-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: Burrow command line app, you can launch a fractional GPU contaienr with this app, and share a link of the container to your friends, you and your friends can work colloratively together
 Author: Vurtne Saerdna
 Author-email: vurtnesaerdna@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

