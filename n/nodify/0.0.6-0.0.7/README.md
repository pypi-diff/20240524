# Comparing `tmp/nodify-0.0.6.tar.gz` & `tmp/nodify-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodify-0.0.6.tar", last modified: Sat May 11 16:11:30 2024, max compression
+gzip compressed data, was "nodify-0.0.7.tar", last modified: Thu May 23 22:59:38 2024, max compression
```

## Comparing `nodify-0.0.6.tar` & `nodify-0.0.7.tar`

### file list

```diff
@@ -1,54 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.608688 nodify-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-11 16:11:25.000000 nodify-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-11 16:11:30.608688 nodify-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 16:11:25.000000 nodify-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-11 16:11:25.000000 nodify-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 16:11:30.608688 nodify-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.596688 nodify-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.600688 nodify-0.0.6/src/nodify/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/file_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.604688 nodify-0.0.6/src/nodify/server/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.604688 nodify-0.0.6/src/nodify/server/flask_socketio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/flask_socketio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9357 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/flask_socketio/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/flask_socketio/emiters.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/flask_socketio/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/flask_socketio/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/pyodide.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    29946 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/server/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/syntax_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.604688 nodify-0.0.6/src/nodify/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_file_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_pythonscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_syntax_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37803 2024-05-11 16:11:25.000000 nodify-0.0.6/src/nodify/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:11:30.608688 nodify-0.0.6/src/nodify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-11 16:11:30.000000 nodify-0.0.6/src/nodify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-11 16:11:30.000000 nodify-0.0.6/src/nodify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 16:11:30.000000 nodify-0.0.6/src/nodify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-11 16:11:30.000000 nodify-0.0.6/src/nodify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 16:11:30.000000 nodify-0.0.6/src/nodify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.764408 nodify-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-23 22:59:35.000000 nodify-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-23 22:59:38.764408 nodify-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 22:59:35.000000 nodify-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-23 22:59:35.000000 nodify-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:59:38.764408 nodify-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.752408 nodify-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.756408 nodify-0.0.7/src/nodify/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/file_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.756408 nodify-0.0.7/src/nodify/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/gui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.760408 nodify-0.0.7/src/nodify/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.760408 nodify-0.0.7/src/nodify/server/flask_socketio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/flask_socketio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/flask_socketio/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/flask_socketio/emiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/flask_socketio/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/flask_socketio/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31650 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/syntax_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.760408 nodify-0.0.7/src/nodify/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_file_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_pythonscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_syntax_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37803 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.760408 nodify-0.0.7/src/nodify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/top_level.txt
```

### Comparing `nodify-0.0.6/LICENSE` & `nodify-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/PKG-INFO` & `nodify-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodify
-Version: 0.0.6
+Version: 0.0.7
 Summary: Supercharge your functional application with a powerful node system.
 Author-email: Pol Febrer <pfebrer96@gmail.com>
 Maintainer-email: Pol Febrer <pfebrer96@gmail.com>
 License: MIT License
         
         Copyright © 2024 Pol Febrer
         
@@ -41,9 +41,18 @@
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
 Requires-Dist: pyvis; extra == "docs"
 Requires-Dist: networkx; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
+Provides-Extra: server
+Requires-Dist: simplejson; extra == "server"
+Provides-Extra: gui
+Requires-Dist: simplejson; extra == "gui"
+Requires-Dist: black; extra == "gui"
+Requires-Dist: isort; extra == "gui"
+Requires-Dist: flask; extra == "gui"
+Requires-Dist: flask-socketio>=5.0; extra == "gui"
+Requires-Dist: eventlet; extra == "gui"
 
 Supercharge your functional applications with nodes.
```

### Comparing `nodify-0.0.6/pyproject.toml` & `nodify-0.0.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [project]
 requires-python = ">=3.9"
 
 name = "nodify"
 description = "Supercharge your functional application with a powerful node system."
 readme = "README.md"
 license = {file = "LICENSE"}
-version = "0.0.6"
+version = "0.0.7"
 
 dependencies = []
 
 authors = [
     {name = "Pol Febrer", email = "pfebrer96@gmail.com"}
 ]
 maintainers = [{name="Pol Febrer", email = "pfebrer96@gmail.com"}]
@@ -54,14 +54,30 @@
     "sphinx-rtd-theme",
     "nbsphinx",
     "pyvis",
     "networkx",
     "matplotlib",
 ]
 
+server = [
+    "simplejson",
+]
+
+gui = [
+    "simplejson",  # Because built-in json parses nan and JS does not understand it
+    "black",
+    "isort",
+    "flask",
+    "flask-socketio >= 5.0",
+    "eventlet"
+]
+
+[project.scripts]
+nodify-gui = "nodify.gui.cli:nodify_gui_cli"
+
 
 [tool.pytest.ini_options]
 testpaths = [
     "src"
 ]
 markers = [
     "slow: mark a test as slow",
@@ -128,28 +144,7 @@
 extend-exclude = """
 (
  ^/files/*
  | /\\..*
  | .*/\\..*
 )
 """
-
-
-[tool.cibuildwheel]
-build-verbosity = 3
-test-extras = "test"
-
-skip = [
-    "pp*",
-    "*musllinux*",
-]
-
-[tool.cibuildwheel.linux]
-
-[tool.cibuildwheel.windows]
-
-before-build = "pip install delvewheel"
-repair-wheel-command = "delvewheel repair -w {dest_dir} {wheel}"
-
-test-command = "pytest --pyargs nodify -m 'not slow'"
-
-[tool.cibuildwheel.macos]
```

### Comparing `nodify-0.0.6/src/nodify/_env.py` & `nodify-0.0.7/src/nodify/_env.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/context.py` & `nodify-0.0.7/src/nodify/context.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/conversions.py` & `nodify-0.0.7/src/nodify/conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
     scrape(output_name, output_node)
 
     def build_script(
         variables,
         include_defaults: bool = False,
         as_function: bool = False,
-        function_name: Optional[str] = "function",
+        function_name: Optional[str] = None,
     ):
 
         # Avoid duplicate variable names and create a list with all names
         variable_names = []
         for var in variables.values():
             if "key" not in var:
                 continue
@@ -196,24 +196,29 @@
             )
 
         script += "\n".join(
             [_get_import_string(module, names) for module, names in imports.items()]
         )
         script += "\n\n"
 
-        def _write_func(func, script):
+        def _write_func(func, include_vardef: bool = True):
+            script = ""
 
             if func.get("get_syntax") is not None:
                 try:
-                    script += f"{func['key']} = {func['get_syntax'](*func['args'], **func['kwargs'])}\n"
+                    if include_vardef:
+                        script += f"{func['key']} = "
+                    script += f"{func['get_syntax'](*func['args'], **func['kwargs'])}\n"
                     return script
                 except Exception as e:
                     pass
 
-            script += f"{func['key']} = {func.get('script_name', func['name'])}("
+            if include_vardef:
+                script += f"{func['key']} = "
+            script += f"{func.get('script_name', func['name'])}("
 
             # Add positional args
             if len(func["args"]) > 0:
                 script += ",".join([repr(arg) for arg in func["args"]]) + ","
 
             # Add keyword args
             if len(func["kwargs"]) > 0:
@@ -236,47 +241,59 @@
             script += ")"
             script += "\n"
 
             return script
 
         if as_function:
 
-            original_name = function_name or "function"
-            function_name = original_name
-            i = 1
-            while function_name in [*variable_names, *function_modules]:
-                function_name += f"_{i}"
-                i += 1
+            # Determine function name
+            if (
+                function_name is None
+                and len(functions) > 0
+                and functions[-1]["key"] != "output"
+            ):
+                function_name = functions[-1]["key"]
+            else:
+                if function_name is None:
+                    function_name = "function"
+
+                original_name = function_name
+                i = 1
+                while function_name in [*variable_names, *function_modules]:
+                    function_name = original_name + f"_{i}"
+                    i += 1
 
+            # Proceed to write the script
             script += f"def {function_name}("
             script += ",".join(
                 [f"{const['key']}={repr(const['value'])}" for const in constants]
             )
             script += "):\n"
 
-            for func in functions:
-                script += "    "
-                script = _write_func(func, script)
-                script += "\n"
+            if len(functions) > 0:
+                for func in functions[:-1]:
+                    script += "    "
+                    script += _write_func(func)
+                    script += "\n"
 
-            script += f"    return {functions[-1]['key'] if len(functions) > 0 else constants[0]['key']}"
+            script += f"    return {_write_func(functions[-1], include_vardef=False) if len(functions) > 0 else constants[0]['key']}"
 
         else:
             script += (
                 "\n\n# -------------------\n#    VARIABLES\n# -------------------\n\n"
             )
             for const in constants:
                 script += f"{const['key']} = {repr(const['value'])} \n"
 
             script += (
                 "\n# -------------------\n#    COMPUTATION\n# -------------------\n\n"
             )
 
             for func in functions:
-                script = _write_func(func, script)
+                script += _write_func(func)
                 script += "\n"
 
         return script
 
     script = build_script(
         variables,
         include_defaults=include_defaults,
```

### Comparing `nodify-0.0.6/src/nodify/dispatcher.py` & `nodify-0.0.7/src/nodify/dispatcher.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/errors.py` & `nodify-0.0.7/src/nodify/errors.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/file_nodes.py` & `nodify-0.0.7/src/nodify/file_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/node.py` & `nodify-0.0.7/src/nodify/node.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/operators.py` & `nodify-0.0.7/src/nodify/operators.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/parse.py` & `nodify-0.0.7/src/nodify/parse.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/registry.py` & `nodify-0.0.7/src/nodify/registry.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/server/app.py` & `nodify-0.0.7/src/nodify/server/app.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/server/cli.py` & `nodify-0.0.7/src/nodify/server/cli.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/server/flask_socketio/app.py` & `nodify-0.0.7/src/nodify/server/flask_socketio/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from ..app import App
 from ..json import CustomJsonModule
 from ..session import Session
 from ..sync import Connection
 from .emiters import emit, emit_error, emit_session
 from .sync import SocketioConnection
-from .user_management import if_user_can, listen_to_users, with_user_management
+from .user_management import if_user_can  # , listen_to_users , with_user_management
 
 # Register the environment variables that the user can tweak
 register_env_variable(
     "NODIFY_SERVER_HOST",
     "localhost",
     "The host where the GUI will run when self-hosted by the user.",
     process=str,
@@ -69,15 +69,16 @@
         self.host = None
         self.port = None
 
         self.app = Flask("NODIFY API")
 
         # No user management yet
         if False:
-            with_user_management(self.app)
+            ...
+            # with_user_management(self.app)
 
         socketio = SocketIO(
             self.app,
             cors_allowed_origins="*",
             json=CustomJsonModule(),
             manage_session=True,
             async_mode=async_mode,
@@ -88,15 +89,16 @@
         # async_mode="threading" this option can not use websockets, therefore there is less communication performance
         # however, it's the only way we can emit socket events from outside of the thread that is running the api
         # Maybe instead of threading we can use socketio.start_background_task (see https://github.com/miguelgrinberg/Flask-SocketIO/issues/876)
         # You can set this to any other async_mode if you don't plan to interact from python (i.e. only through the GUI)
         on = socketio.on
 
         if False:
-            listen_to_users(on, emit_session)
+            ...
+            # listen_to_users(on, emit_session)
 
         connection = SocketioLastUpdateEmiter(socketio)
 
         self.socketio = socketio
 
         if session is None:
             session = session_cls()
@@ -104,15 +106,14 @@
         super().__init__(session=session, connection=connection)
 
         # -------------------------------------------
         # From now on, we define the socketio events
         # -------------------------------------------
         @socketio.on_error()
         def send_error(err):
-            print("SOME ERROR", err)
             if self.session is not None:
                 self.session.logger.exception(err)
 
             emit_error(err)
             emit_session(self.session, broadcast=True)
             raise err
 
@@ -210,20 +211,19 @@
         return self.socketio.run(
             self.app, debug=debug, host=host, port=port, allow_unsafe_werkzeug=True
         )
 
     def get_server_address(self) -> str:
         return f"http://{self.host}:{self.port}"
 
-    @staticmethod
-    def open_frontend():
+    def open_frontend(self):
         """Opens the graphical interface"""
-        webbrowser.open(
-            str(Path(__file__).parent.parent.parent / "build" / "index.html")
-        )
+        from nodify.gui import open_frontend
+
+        open_frontend("socket", self.port, self.host)
 
     def launch(
         self,
         frontend: bool = True,
         server: bool = True,
         server_host: Union[str, None] = None,
         server_port: Union[int, None] = None,
@@ -245,16 +245,14 @@
             The port to use for the server.
             If not provided, it will be taken from the environment variable NODIFY_SERVER_PORT.
         server_debug: bool, optional
             Whether to run the server in debug mode.
         interactive: bool, optional
             whether an interactive console should be started.
         """
-        if frontend:
-            self.open_frontend()
 
         if not server:
             return
 
         self.threads = [
             Thread(
                 target=self.run_server,
@@ -277,13 +275,16 @@
                     },
                 )
             )
 
         for t in self.threads:
             t.start()
 
+        if frontend:
+            self.open_frontend()
+
         if interactive:
             try:
                 while 1:
                     time.sleep(0.1)
             except KeyboardInterrupt:
                 print("Please use Ctrl+D to kill the interactive console first")
```

### Comparing `nodify-0.0.6/src/nodify/server/flask_socketio/emiters.py` & `nodify-0.0.7/src/nodify/server/flask_socketio/emiters.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/server/flask_socketio/sync.py` & `nodify-0.0.7/src/nodify/server/flask_socketio/sync.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/server/flask_socketio/user_management.py` & `nodify-0.0.7/src/nodify/server/flask_socketio/user_management.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,156 +1,169 @@
 from functools import wraps
 
-from flask_login import (
-    LoginManager,
-    UserMixin,
-    current_user,
-    login_user,
-    logout_user,
-    user_logged_in,
-)
-from flask_session import Session
-from flask_socketio import emit
+try:
+    import flask_login
+
+    _FLASK_LOGIN_AVAILABLE = True
+except ImportError:
+    _FLASK_LOGIN_AVAILABLE = False
 
 __all__ = ["User", "if_user_can", "with_user_management", "listen_to_users"]
 
 __WITH_USERS__ = False
 
+if not _FLASK_LOGIN_AVAILABLE:
 
-class User(UserMixin):
-    """
-    Class used for users that are accessing the session through the GUI.
-    """
-
-    def __init__(self, id=None):
-        self.id = id
-
-        self.permissions = {
-            "see": True,
-            "edit": True,
-            "get_new_plots": False,
-            "manage_users": False,
-            "load_session": False,
-            "save_session": False,
-        }
-
-    def change_permissions(self, new_permissions):
-        """
-        Changes the permissions of this user.
-
-        This method can be executed only by:
-        - A user that has permission to manage_users (through the GUI).
-        - The launcher of the app, by executing the python method directly
-        (in the console or jupyter notebook).
+    def if_user_can(*perms):
 
-        Parameters
-        -----------
-        new_permissions: dict
-            A dictionary containing new permissions that will overwrite the old ones
+        def with_permissions_check(f):
+            return f
+
+        return with_permissions_check
+
+    def with_user_management(app):
+        pass
+
+    def listen_to_users(socketio_on):
+        pass
+
+else:
+
+    from flask_login import LoginManager, UserMixin, current_user, login_user
+    from flask_session import Session
+    from flask_socketio import emit
+
+    class User(UserMixin):
+        """
+        Class used for users that are accessing the session through the GUI.
         """
-        # If the current_user environment variable is not present, this means the
-        # method is being executed from python directly
-        if "current_user" not in locals() or current_user.has_permissions(
-            "manage_users"
-        ):
-            self.permissions = {**self.permissions, **new_permissions}
-        else:
-            raise Exception("You don't have the rights to change user permissions.")
 
-    def has_permissions(self, *perms):
+        def __init__(self, id=None):
+            self.id = id
+
+            self.permissions = {
+                "see": True,
+                "edit": True,
+                "get_new_plots": False,
+                "manage_users": False,
+                "load_session": False,
+                "save_session": False,
+            }
+
+        def change_permissions(self, new_permissions):
+            """
+            Changes the permissions of this user.
+
+            This method can be executed only by:
+            - A user that has permission to manage_users (through the GUI).
+            - The launcher of the app, by executing the python method directly
+            (in the console or jupyter notebook).
+
+            Parameters
+            -----------
+            new_permissions: dict
+                A dictionary containing new permissions that will overwrite the old ones
+            """
+            # If the current_user environment variable is not present, this means the
+            # method is being executed from python directly
+            if "current_user" not in locals() or current_user.has_permissions(
+                "manage_users"
+            ):
+                self.permissions = {**self.permissions, **new_permissions}
+            else:
+                raise Exception("You don't have the rights to change user permissions.")
+
+        def has_permissions(self, *perms):
+            """
+            Checks if the user has the provided permissions.
+
+            Parameters
+            -----------
+            *perms: str
+                The permissions that you want to check. As many as you wish.
+
+            Returns
+            ---------
+            boolean
+                only True if it fulfills ALL the requested permissions.
+            """
+            for perm in perms:
+                if not self.permissions[perm]:
+                    return False
+            else:
+                return True
+
+    def if_user_can(*perms):
         """
-        Checks if the user has the provided permissions.
+        Wrapper that restricts actions to only users with the required permissions.
+
+        Note that the permissions of each user are stored under user.permissions.
 
         Parameters
         -----------
         *perms: str
-            The permissions that you want to check. As many as you wish.
+            The permissions that must be fulfilled for the user to be able to perform this action.
 
-        Returns
-        ---------
-        boolean
-            only True if it fulfills ALL the requested permissions.
-        """
-        for perm in perms:
-            if not self.permissions[perm]:
-                return False
-        else:
-            return True
-
-
-def if_user_can(*perms):
-    """
-    Wrapper that restricts actions to only users with the required permissions.
-
-    Note that the permissions of each user are stored under user.permissions.
-
-    Parameters
-    -----------
-    *perms: str
-        The permissions that must be fulfilled for the user to be able to perform this action.
-
-        As many as you wish.
-
-    Usage
-    -------
-    This is to be used when responding to requests using flask-socketio.
-
-    ```
-    @socketio.on("destroy the world") # Indicates which events are we listening to
-    @if_user_can("use nuclear weapons") # Restricts access to only users with needed permissions
-    def destroy(*args, **kwargs):
-        # All the code here will only be executed if the user has permission to use nuclear weapons
-    ```
-    """
-
-    def with_permissions_check(f):
-
-        @wraps(f)
-        def wrapped(*args, **kwargs):
-            if __WITH_USERS__:
-                if not current_user.is_authenticated:
-                    emit("auth_required")
-                elif current_user.has_permissions(*perms):
-                    return f(*args, **kwargs)
-                else:
-                    raise Exception(
-                        f"You don't have the required permissions. \n These are your permissions: {current_user.permissions}"
-                    )
-            else:
-                return f(*args, **kwargs)
+            As many as you wish.
 
-        return wrapped
+        Usage
+        -------
+        This is to be used when responding to requests using flask-socketio.
+
+        ```
+        @socketio.on("destroy the world") # Indicates which events are we listening to
+        @if_user_can("use nuclear weapons") # Restricts access to only users with needed permissions
+        def destroy(*args, **kwargs):
+            # All the code here will only be executed if the user has permission to use nuclear weapons
+        ```
+        """
 
-    return with_permissions_check
+        def with_permissions_check(f):
 
+            @wraps(f)
+            def wrapped(*args, **kwargs):
+                if __WITH_USERS__:
+                    if not current_user.is_authenticated:
+                        emit("auth_required")
+                    elif current_user.has_permissions(*perms):
+                        return f(*args, **kwargs)
+                    else:
+                        raise Exception(
+                            f"You don't have the required permissions. \n These are your permissions: {current_user.permissions}"
+                        )
+                else:
+                    return f(*args, **kwargs)
+
+            return wrapped
 
-def with_user_management(app):
+        return with_permissions_check
 
-    # User management
-    app.config["SECRET_KEY"] = "top-secret!"
+    def with_user_management(app):
 
-    login_manager = LoginManager(app)
-    login_manager.init_app(app)
+        # User management
+        app.config["SECRET_KEY"] = "top-secret!"
 
-    Session(app)
+        login_manager = LoginManager(app)
+        login_manager.init_app(app)
 
-    @login_manager.user_loader
-    def load_user(id):
-        return User(id)
+        Session(app)
 
+        @login_manager.user_loader
+        def load_user(id):
+            return User(id)
 
-def listen_to_users(socketio_on):
-    """
-    Sets the necessary socketio event listeners to manage users.
+    def listen_to_users(socketio_on):
+        """
+        Sets the necessary socketio event listeners to manage users.
 
-    Parameters
-    ----------
-    socketio_on: socketio.on
-        The function to be used to listen to socketio events
-    """
+        Parameters
+        ----------
+        socketio_on: socketio.on
+            The function to be used to listen to socketio events
+        """
 
-    @socketio_on("login")
-    def login(username):
+        @socketio_on("login")
+        def login(username):
 
-        login_user(User(username))
+            login_user(User(username))
 
-        emit("logged_in")
+            emit("logged_in")
```

### Comparing `nodify-0.0.6/src/nodify/server/json.py` & `nodify-0.0.7/src/nodify/server/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,48 @@
 try:
     import plotly.graph_objects as go
 
     _PLOTLY_AVAILABLE = True
 except:
     _PLOTLY_AVAILABLE = False
 
-import numpy as np
+try:
+    import numpy as np
+
+    np_ndarray = np.ndarray
+    np_generic = np.generic
+    _NUMPY_AVAILABLE = True
+except:
+
+    class np_ndarray:
+        pass
+
+    class np_generic:
+        pass
+
+    _NUMPY_AVAILABLE = False
+
 import simplejson
 from simplejson.encoder import JSONEncoder
 
 from nodify import Node
 
 
 def as_jsonable(encoder, obj):
-    if isinstance(obj, np.ndarray) and not np.issubdtype(obj.dtype, np.number):
+    if (
+        _NUMPY_AVAILABLE
+        and isinstance(obj, np_ndarray)
+        and not np.issubdtype(obj.dtype, np.number)
+    ):
         return as_jsonable(encoder, obj.tolist())
     elif isinstance(obj, (list, tuple)):
         return type(obj)([as_jsonable(encoder, v) for v in obj])
     elif isinstance(obj, dict):
         return {k: as_jsonable(encoder, v) for k, v in obj.items()}
-    elif not isinstance(obj, (tuple, float, str, int, bool, type(None), np.ndarray)):
+    elif not isinstance(obj, (tuple, float, str, int, bool, type(None), np_ndarray)):
         return as_jsonable(encoder, encoder.default(obj))
     else:
         return obj
 
 
 def get_inputs_mode(
     node: Node, encoder: Optional[JSONEncoder] = None, include_defaults: bool = True
@@ -156,17 +175,17 @@
 
         if isinstance(obj, Node):
             return node_to_json(self, obj)
         elif _PLOTLY_AVAILABLE and isinstance(obj, go.Figure):
             return obj.to_plotly_json()
         elif hasattr(obj, "to_json"):
             return obj.to_json()
-        elif isinstance(obj, np.ndarray):
+        elif isinstance(obj, np_ndarray):
             return obj.tolist()
-        elif isinstance(obj, np.generic):
+        elif isinstance(obj, np_generic):
             return obj.item()
         elif isinstance(obj, pathlib.Path):
             return str(obj)
         elif isinstance(obj, type):
             return repr(obj)
 
         try:
```

### Comparing `nodify-0.0.6/src/nodify/server/launch.py` & `nodify-0.0.7/src/nodify/server/launch.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/server/registry.py` & `nodify-0.0.7/src/nodify/server/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,15 @@
             self.register_typehint_spec(typehint)
 
     def register_node_class_spec(self, encoder, node_class: Type[Node]):
 
         try:
             spec = self.get_node_class_spec(encoder, node_class)
             self._encoder.encode(spec)
-        except Exception as e:
-            print(node_class, e)
+        except:
             return
 
         self.node_class_specs[id(node_class)] = spec
 
     def get_node_class_spec(self, encoder, node_class: Type[Node]):
         """Parses a node class into a JSON object that can be sent to the client.
```

### Comparing `nodify-0.0.6/src/nodify/server/session.py` & `nodify-0.0.7/src/nodify/server/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib
 import inspect
 import logging
 import time
 from functools import wraps
 from io import BytesIO, StringIO
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 from nodify import ConstantNode, Node, Workflow, nodify_module
 from nodify.conversions import node_to_python_script, python_script_to_nodes
 from nodify.utils import (
     traverse_tree_backward,
     traverse_tree_forward,
     visit_all_connected,
@@ -32,14 +32,23 @@
             return ret
 
         return wrapper
 
     return decorator
 
 
+FILE_PLOT_REGISTRY = {}
+
+
+def register_file_plot_handler(
+    name: str, options_finder: Callable[[str], List[str]], handler: Callable
+):
+    FILE_PLOT_REGISTRY[name] = (options_finder, handler)
+
+
 class Session:
     """Base session class that implements the functionality of a session in the GUI"""
 
     # Object that dispatches session methods and automatically updates the GUI
     synced: Synchronized
 
     # Keeping track of last updates
@@ -100,14 +109,59 @@
         self.settings = {
             "file_storage_dir": ".nodify_uploaded_files",
             "keep_uploaded": False,
         }
 
         self.allowed_nodifiable = []
 
+    def supports_file_plotting(self):
+        return len(FILE_PLOT_REGISTRY) > 0
+
+    def get_file_plot_options(self, file_name: str) -> List[str]:
+        options = []
+        for name, (options_finder, _) in FILE_PLOT_REGISTRY.items():
+            options.extend(options_finder(file_name))
+        return options
+
+    def plot_uploaded_file(
+        self,
+        name: str,
+        file_bytes: Optional[BytesIO] = None,
+        method: Optional[str] = None,
+        node_name: Optional[str] = None,
+        additional_files: Dict[str, BytesIO] = {},
+    ) -> int:
+        if file_bytes is None:
+            # We will assume that the file is already written.
+            file_name = Path(name)
+            keep = True
+            dirname = file_name.parent
+        else:
+            file_name, dirname, keep = self.write_file(file_bytes, name)
+
+        additional_files_info = []
+        for n, file in additional_files.items():
+            additional_files_info.append(self.write_file(file, n))
+
+        for name, (options_finder, handler) in FILE_PLOT_REGISTRY.items():
+            if method in options_finder(file_name):
+                plot = handler(file_name, method)
+                break
+
+        self.add_node(plot, node_name or name)
+
+        if not keep:
+            self._remove_temp_file(file_name, dirname)
+
+        for file_name, dirname, keep in additional_files_info:
+            if not keep:
+                self._remove_temp_file(file_name, dirname)
+
+        return id(plot)
+
     # Functions to receive uploaded files:
     def write_file(self, file_bytes, name):
         dirname = Path(self.settings["file_storage_dir"])
         if not dirname.exists():
             dirname.mkdir()
 
         file_name = dirname / name
```

### Comparing `nodify-0.0.6/src/nodify/server/sync.py` & `nodify-0.0.7/src/nodify/server/sync.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/syntax_nodes.py` & `nodify-0.0.7/src/nodify/syntax_nodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import operator
-from typing import Any, Dict
+from typing import Any, Dict, Literal
 
 from .node import Node
 
 
 class ListNode(Node):
     @staticmethod
     def function(*items):
@@ -122,14 +122,17 @@
         return true if test else false
 
     def get_diagram_label(self):
         """Returns the label to be used in diagrams when displaying this node."""
         return "if/else"
 
 
+_CompareOp = Literal["eq", "ne", "gt", "lt", "ge", "le", "is_", "is_not", "contains"]
+
+
 class CompareNode(Node):
     _op_to_symbol = {
         "eq": "==",
         "ne": "!=",
         "gt": ">",
         "lt": "<",
         "ge": ">=",
@@ -142,22 +145,38 @@
 
     def get_syntax(self, left, op, right):
         if not isinstance(op, str):
             raise ValueError(f"Invalid operator: {op}")
         return f"{repr(left)} {self._op_to_symbol[op]} {repr(right)}"
 
     @staticmethod
-    def function(left, op: str, right):
+    def function(left, op: _CompareOp, right):
         return getattr(operator, op)(left, right)
 
     def get_diagram_label(self):
         """Returns the label to be used in diagrams when displaying this node."""
         return self._op_to_symbol.get(self._prev_evaluated_inputs.get("op"))
 
 
+_BynaryOp = Literal[
+    "add",
+    "sub",
+    "mul",
+    "truediv",
+    "floordiv",
+    "mod",
+    "pow",
+    "lshift",
+    "rshift",
+    "and",
+    "xor",
+    "or",
+]
+
+
 class BinaryOperationNode(Node):
 
     _op_to_symbol = {
         "add": "+",
         "sub": "-",
         "mul": "*",
         "truediv": "/",
@@ -168,32 +187,35 @@
         "rshift": ">>",
         "and": "&",
         "xor": "^",
         "or": "|",
     }
 
     @staticmethod
-    def function(left, op: str, right):
+    def function(left, op: _BynaryOp, right):
         return getattr(operator, op)(left, right)
 
     def get_syntax(self, left, op, right):
         if not isinstance(op, str):
             raise ValueError(f"Invalid operator: {op}")
         return f"{repr(left)} {self._op_to_symbol[op]} {repr(right)}"
 
 
+_UnaryOp = Literal["invert", "neg", "pos"]
+
+
 class UnaryOperationNode(Node):
     _op_to_symbol = {
         "invert": "~",
         "neg": "-",
         "pos": "+",
     }
 
     @staticmethod
-    def function(op: str, operand):
+    def function(op: _UnaryOp, operand):
         return getattr(operator, op)(operand)
 
     def get_syntax(self, op, operand):
         if not isinstance(op, str):
             raise ValueError(f"Invalid operator: {op}")
         return f"{self._op_to_symbol[op]}{repr(operand)}"
```

### Comparing `nodify-0.0.6/src/nodify/tests/test_context.py` & `nodify-0.0.7/src/nodify/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/tests/test_file_nodes.py` & `nodify-0.0.7/src/nodify/tests/test_file_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/tests/test_node.py` & `nodify-0.0.7/src/nodify/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/tests/test_pythonscript.py` & `nodify-0.0.7/src/nodify/tests/test_pythonscript.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/tests/test_registry.py` & `nodify-0.0.7/src/nodify/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/tests/test_syntax_nodes.py` & `nodify-0.0.7/src/nodify/tests/test_syntax_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/tests/test_utils.py` & `nodify-0.0.7/src/nodify/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/tests/test_workflow.py` & `nodify-0.0.7/src/nodify/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify/utils.py` & `nodify-0.0.7/src/nodify/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,17 @@
     This new nodified module contains only nodes (coming from functions or classes).
     The rest of variables are not copied. In fact, the new module uses the variables
     from the original module.
 
     Also, some functions might not be convertable to nodes and therefore won't be found
     in the new module.
 
+    For each module that is found while traversing, its __nodify__ function is called
+    if it exists.
+
     Parameters
     ----------
     module : ModuleType
         The module to nodify.
     node_class : Type[Node], optional
         The class from which the created nodes will inherit, by default Node.
         This can be useful for example to convert to workflows, if you pass
@@ -122,14 +125,18 @@
     if module in _nodified_modules:
         return _nodified_modules[module]
 
     # Function that recursively traverses the module and replaces functions with nodes.
     def _nodified_module(
         module: ModuleType, visited: Dict[ModuleType, ModuleType], main_module: str
     ) -> ModuleType:
+        # Call the __nodify__ function on the module if it exists.
+        if hasattr(module, "__nodify__"):
+            module.__nodify__()
+
         # This module has already been visited, so do return the already nodified module.
         if module in visited:
             return visited[module]
 
         # Create a copy of this module, with the nodified_ prefix in the name.
         noded_module = ModuleType(f"nodified_{module.__name__}")
         # Register the module as visited.
```

### Comparing `nodify-0.0.6/src/nodify/workflow.py` & `nodify-0.0.7/src/nodify/workflow.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.6/src/nodify.egg-info/PKG-INFO` & `nodify-0.0.7/src/nodify.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodify
-Version: 0.0.6
+Version: 0.0.7
 Summary: Supercharge your functional application with a powerful node system.
 Author-email: Pol Febrer <pfebrer96@gmail.com>
 Maintainer-email: Pol Febrer <pfebrer96@gmail.com>
 License: MIT License
         
         Copyright © 2024 Pol Febrer
         
@@ -41,9 +41,18 @@
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Requires-Dist: nbsphinx; extra == "docs"
 Requires-Dist: pyvis; extra == "docs"
 Requires-Dist: networkx; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
+Provides-Extra: server
+Requires-Dist: simplejson; extra == "server"
+Provides-Extra: gui
+Requires-Dist: simplejson; extra == "gui"
+Requires-Dist: black; extra == "gui"
+Requires-Dist: isort; extra == "gui"
+Requires-Dist: flask; extra == "gui"
+Requires-Dist: flask-socketio>=5.0; extra == "gui"
+Requires-Dist: eventlet; extra == "gui"
 
 Supercharge your functional applications with nodes.
```

### Comparing `nodify-0.0.6/src/nodify.egg-info/SOURCES.txt` & `nodify-0.0.7/src/nodify.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 src/nodify/registry.py
 src/nodify/syntax_nodes.py
 src/nodify/utils.py
 src/nodify/workflow.py
 src/nodify.egg-info/PKG-INFO
 src/nodify.egg-info/SOURCES.txt
 src/nodify.egg-info/dependency_links.txt
+src/nodify.egg-info/entry_points.txt
 src/nodify.egg-info/requires.txt
 src/nodify.egg-info/top_level.txt
+src/nodify/gui/__init__.py
+src/nodify/gui/cli.py
 src/nodify/server/__init__.py
 src/nodify/server/app.py
 src/nodify/server/cli.py
 src/nodify/server/json.py
 src/nodify/server/launch.py
 src/nodify/server/pyodide.py
 src/nodify/server/registry.py
```

