# Comparing `tmp/nodify-0.0.7.tar.gz` & `tmp/nodify-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodify-0.0.7.tar", last modified: Thu May 23 22:59:38 2024, max compression
+gzip compressed data, was "nodify-0.0.8.tar", last modified: Thu May 23 23:16:52 2024, max compression
```

## Comparing `nodify-0.0.7.tar` & `nodify-0.0.8.tar`

### file list

```diff
@@ -1,58 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.764408 nodify-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-23 22:59:35.000000 nodify-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-23 22:59:38.764408 nodify-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 22:59:35.000000 nodify-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-23 22:59:35.000000 nodify-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 22:59:38.764408 nodify-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.752408 nodify-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.756408 nodify-0.0.7/src/nodify/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/file_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.756408 nodify-0.0.7/src/nodify/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/gui/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.760408 nodify-0.0.7/src/nodify/server/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.760408 nodify-0.0.7/src/nodify/server/flask_socketio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/flask_socketio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/flask_socketio/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/flask_socketio/emiters.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/flask_socketio/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/flask_socketio/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/pyodide.py
--rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    31650 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/server/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/syntax_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.760408 nodify-0.0.7/src/nodify/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_file_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_pythonscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_syntax_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37803 2024-05-23 22:59:35.000000 nodify-0.0.7/src/nodify/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 22:59:38.760408 nodify-0.0.7/src/nodify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 22:59:38.000000 nodify-0.0.7/src/nodify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.570665 nodify-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-23 23:16:49.000000 nodify-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-23 23:16:52.570665 nodify-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 23:16:49.000000 nodify-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-23 23:16:49.000000 nodify-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 23:16:52.570665 nodify-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.530664 nodify-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.534664 nodify-0.0.8/src/nodify/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/file_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.534664 nodify-0.0.8/src/nodify/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.538664 nodify-0.0.8/src/nodify/gui/build/
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   545651 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/icon.icns
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/safari-pinned-tab.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.530664 nodify-0.0.8/src/nodify/gui/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.538664 nodify-0.0.8/src/nodify/gui/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    31922 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/static/css/main.b71f9b9d.css
+-rw-r--r--   0 runner    (1001) docker     (127)    47005 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/static/css/main.b71f9b9d.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.542664 nodify-0.0.8/src/nodify/gui/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  5491801 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/static/js/main.e8c3f4c5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/static/js/main.e8c3f4c5.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127) 16593568 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/build/static/js/main.e8c3f4c5.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/gui/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.566664 nodify-0.0.8/src/nodify/server/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.566664 nodify-0.0.8/src/nodify/server/flask_socketio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/flask_socketio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/flask_socketio/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/flask_socketio/emiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/flask_socketio/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/flask_socketio/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31650 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/server/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/syntax_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.566664 nodify-0.0.8/src/nodify/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/tests/test_file_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/tests/test_pythonscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/tests/test_syntax_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37803 2024-05-23 23:16:49.000000 nodify-0.0.8/src/nodify/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 23:16:52.566664 nodify-0.0.8/src/nodify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-23 23:16:52.000000 nodify-0.0.8/src/nodify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-23 23:16:52.000000 nodify-0.0.8/src/nodify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 23:16:52.000000 nodify-0.0.8/src/nodify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 23:16:52.000000 nodify-0.0.8/src/nodify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-23 23:16:52.000000 nodify-0.0.8/src/nodify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 23:16:52.000000 nodify-0.0.8/src/nodify.egg-info/top_level.txt
```

### Comparing `nodify-0.0.7/LICENSE` & `nodify-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/PKG-INFO` & `nodify-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodify
-Version: 0.0.7
+Version: 0.0.8
 Summary: Supercharge your functional application with a powerful node system.
 Author-email: Pol Febrer <pfebrer96@gmail.com>
 Maintainer-email: Pol Febrer <pfebrer96@gmail.com>
 License: MIT License
         
         Copyright © 2024 Pol Febrer
```

### Comparing `nodify-0.0.7/pyproject.toml` & `nodify-0.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [project]
 requires-python = ">=3.9"
 
 name = "nodify"
 description = "Supercharge your functional application with a powerful node system."
 readme = "README.md"
 license = {file = "LICENSE"}
-version = "0.0.7"
+version = "0.0.8"
 
 dependencies = []
 
 authors = [
     {name = "Pol Febrer", email = "pfebrer96@gmail.com"}
 ]
 maintainers = [{name="Pol Febrer", email = "pfebrer96@gmail.com"}]
@@ -70,14 +70,17 @@
     "flask-socketio >= 5.0",
     "eventlet"
 ]
 
 [project.scripts]
 nodify-gui = "nodify.gui.cli:nodify_gui_cli"
 
+[tool.setuptools.package-data]
+"nodify.gui" = ["build/*", "build/static/*/*"]
+
 
 [tool.pytest.ini_options]
 testpaths = [
     "src"
 ]
 markers = [
     "slow: mark a test as slow",
```

### Comparing `nodify-0.0.7/src/nodify/_env.py` & `nodify-0.0.8/src/nodify/_env.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/context.py` & `nodify-0.0.8/src/nodify/context.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/conversions.py` & `nodify-0.0.8/src/nodify/conversions.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/dispatcher.py` & `nodify-0.0.8/src/nodify/dispatcher.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/errors.py` & `nodify-0.0.8/src/nodify/errors.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/file_nodes.py` & `nodify-0.0.8/src/nodify/file_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/gui/__init__.py` & `nodify-0.0.8/src/nodify/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/gui/cli.py` & `nodify-0.0.8/src/nodify/gui/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
     def cli():
         parser = argparse.ArgumentParser(prog=title, description=description)
 
         parser.add_argument(
             "modules",
             type=str,
-            nargs="?",
+            nargs="*",
+            default=defaults.get("modules", ["f"]),
             help="Modules to nodify before launching the GUI",
         )
         parser.add_argument(
             "--backend",
             type=str,
             default=defaults.get("backend", "socket"),
             help="The backend to use. If 'socket', the server will be launched.",
@@ -54,18 +55,15 @@
             type=str,
             default=defaults.get("session_cls", None),
             help="The session class to instantiate to create the session. If not provided, the default session will be used.",
         )
 
         args = parser.parse_args()
 
-        if not hasattr(args, "modules"):
-            modules_to_nodify = [*modules, defaults.get("modules", [])]
-        else:
-            modules_to_nodify = [*modules, args.modules]
+        modules_to_nodify = [*modules, *(args.modules or [])]
 
         # Nodify all requested modules
         for module_string in modules_to_nodify:
             module = importlib.import_module(module_string)
             nodify_module(module)
 
         launch_gui(
```

### Comparing `nodify-0.0.7/src/nodify/node.py` & `nodify-0.0.8/src/nodify/node.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/operators.py` & `nodify-0.0.8/src/nodify/operators.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/parse.py` & `nodify-0.0.8/src/nodify/parse.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/registry.py` & `nodify-0.0.8/src/nodify/registry.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/server/app.py` & `nodify-0.0.8/src/nodify/server/app.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/server/cli.py` & `nodify-0.0.8/src/nodify/server/cli.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/server/flask_socketio/app.py` & `nodify-0.0.8/src/nodify/server/flask_socketio/app.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/server/flask_socketio/emiters.py` & `nodify-0.0.8/src/nodify/server/flask_socketio/emiters.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/server/flask_socketio/sync.py` & `nodify-0.0.8/src/nodify/server/flask_socketio/sync.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/server/flask_socketio/user_management.py` & `nodify-0.0.8/src/nodify/server/flask_socketio/user_management.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/server/json.py` & `nodify-0.0.8/src/nodify/server/json.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/server/launch.py` & `nodify-0.0.8/src/nodify/server/launch.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/server/registry.py` & `nodify-0.0.8/src/nodify/server/registry.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/server/session.py` & `nodify-0.0.8/src/nodify/server/session.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/server/sync.py` & `nodify-0.0.8/src/nodify/server/sync.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/syntax_nodes.py` & `nodify-0.0.8/src/nodify/syntax_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/tests/test_context.py` & `nodify-0.0.8/src/nodify/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/tests/test_file_nodes.py` & `nodify-0.0.8/src/nodify/tests/test_file_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/tests/test_node.py` & `nodify-0.0.8/src/nodify/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/tests/test_pythonscript.py` & `nodify-0.0.8/src/nodify/tests/test_pythonscript.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/tests/test_registry.py` & `nodify-0.0.8/src/nodify/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/tests/test_syntax_nodes.py` & `nodify-0.0.8/src/nodify/tests/test_syntax_nodes.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/tests/test_utils.py` & `nodify-0.0.8/src/nodify/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/tests/test_workflow.py` & `nodify-0.0.8/src/nodify/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/utils.py` & `nodify-0.0.8/src/nodify/utils.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify/workflow.py` & `nodify-0.0.8/src/nodify/workflow.py`

 * *Files identical despite different names*

### Comparing `nodify-0.0.7/src/nodify.egg-info/PKG-INFO` & `nodify-0.0.8/src/nodify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodify
-Version: 0.0.7
+Version: 0.0.8
 Summary: Supercharge your functional application with a powerful node system.
 Author-email: Pol Febrer <pfebrer96@gmail.com>
 Maintainer-email: Pol Febrer <pfebrer96@gmail.com>
 License: MIT License
         
         Copyright © 2024 Pol Febrer
```

