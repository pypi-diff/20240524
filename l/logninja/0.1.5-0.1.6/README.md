# Comparing `tmp/logninja-0.1.5.tar.gz` & `tmp/logninja-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logninja-0.1.5.tar", last modified: Fri May 24 18:47:12 2024, max compression
+gzip compressed data, was "logninja-0.1.6.tar", last modified: Fri May 24 20:39:30 2024, max compression
```

## Comparing `logninja-0.1.5.tar` & `logninja-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:47:12.603826 logninja-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 18:47:08.000000 logninja-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-24 18:47:12.603826 logninja-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-24 18:47:08.000000 logninja-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:47:12.603826 logninja-0.1.5/logninja/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-24 18:47:08.000000 logninja-0.1.5/logninja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:47:12.603826 logninja-0.1.5/logninja/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 18:47:08.000000 logninja-0.1.5/logninja/asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-24 18:47:08.000000 logninja-0.1.5/logninja/asgi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-24 18:47:08.000000 logninja-0.1.5/logninja/console_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-24 18:47:08.000000 logninja-0.1.5/logninja/contextvars_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-24 18:47:08.000000 logninja-0.1.5/logninja/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-24 18:47:08.000000 logninja-0.1.5/logninja/json_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-24 18:47:08.000000 logninja-0.1.5/logninja/traceback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:47:12.603826 logninja-0.1.5/logninja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-24 18:47:12.000000 logninja-0.1.5/logninja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-24 18:47:12.000000 logninja-0.1.5/logninja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:47:12.000000 logninja-0.1.5/logninja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 18:47:12.000000 logninja-0.1.5/logninja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 18:47:12.000000 logninja-0.1.5/logninja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-24 18:47:08.000000 logninja-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:47:12.603826 logninja-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:47:12.603826 logninja-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-24 18:47:08.000000 logninja-0.1.5/tests/test_json_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:30.300490 logninja-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 20:39:26.000000 logninja-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-24 20:39:30.300490 logninja-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-24 20:39:26.000000 logninja-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:30.300490 logninja-0.1.6/logninja/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:30.300490 logninja-0.1.6/logninja/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/asgi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/console_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/contextvars_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/json_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/traceback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:30.300490 logninja-0.1.6/logninja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-24 20:39:30.000000 logninja-0.1.6/logninja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-24 20:39:30.000000 logninja-0.1.6/logninja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:39:30.000000 logninja-0.1.6/logninja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 20:39:30.000000 logninja-0.1.6/logninja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 20:39:30.000000 logninja-0.1.6/logninja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-24 20:39:26.000000 logninja-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 20:39:30.300490 logninja-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:30.300490 logninja-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-24 20:39:26.000000 logninja-0.1.6/tests/test_json_formatter.py
```

### Comparing `logninja-0.1.5/LICENSE` & `logninja-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `logninja-0.1.5/PKG-INFO` & `logninja-0.1.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-Metadata-Version: 2.1
-Name: logninja
-Version: 0.1.5
-Summary: A log configuration library for Python projects.
-Author-email: Pedro Cantidio <ppcantidio@gmail.com>
-Project-URL: homepage, https://github.com/ppcantidio/logninja.py
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: starlette
-Requires-Dist: starlette<0.38.0,>=0.37.2; extra == "starlette"
+[build-system]
+requires = ["setuptools", "wheel"]
 
-# LogNinja
-Simple logging setup to be used at python applications.
+[project]
+name = "logninja"
+version = "0.1.6"
+authors = [{ name = "Pedro Cantidio", email = "ppcantidio@gmail.com" }]
+description = "A log configuration library for Python projects."
+readme = "README.md"
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+
+[project.urls]
+homepage = "https://github.com/ppcantidio/logninja.py"
+
+[project.optional-dependencies]
+starlette = ["starlette>=0.37.2,<0.38.0"]
```

### Comparing `logninja-0.1.5/logninja/__init__.py` & `logninja-0.1.6/logninja/__init__.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.5/logninja/asgi/middleware.py` & `logninja-0.1.6/logninja/asgi/middleware.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.5/logninja/decorators.py` & `logninja-0.1.6/logninja/decorators.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.5/logninja/json_formatter.py` & `logninja-0.1.6/logninja/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.5/logninja/traceback.py` & `logninja-0.1.6/logninja/traceback.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.5/tests/test_json_formatter.py` & `logninja-0.1.6/tests/test_json_formatter.py`

 * *Files identical despite different names*

