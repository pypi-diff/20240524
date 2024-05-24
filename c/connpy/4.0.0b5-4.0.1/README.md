# Comparing `tmp/connpy-4.0.0b5.tar.gz` & `tmp/connpy-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-4.0.0b5.tar", last modified: Mon Apr 22 21:19:23 2024, max compression
+gzip compressed data, was "connpy-4.0.1.tar", last modified: Fri May 24 20:59:08 2024, max compression
```

## Comparing `connpy-4.0.0b5.tar` & `connpy-4.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:19:23.135183 connpy-4.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-22 21:19:17.000000 connpy-4.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17495 2024-04-22 21:19:23.135183 connpy-4.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16385 2024-04-22 21:19:17.000000 connpy-4.0.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:19:23.131183 connpy-4.0.0b5/connpy/
--rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24877 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5181 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16438 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    74729 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    33096 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:19:23.135183 connpy-4.0.0b5/connpy/core_plugins/
--rwxr-xr-x   0 runner    (1001) docker     (127)    13827 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/core_plugins/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/core_plugins/sync_client
--rwxr-xr-x   0 runner    (1001) docker     (127)     3231 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7133 2024-04-22 21:19:17.000000 connpy-4.0.0b5/connpy/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:19:23.135183 connpy-4.0.0b5/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17495 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 21:19:23.000000 connpy-4.0.0b5/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-22 21:19:23.135183 connpy-4.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-22 21:19:17.000000 connpy-4.0.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:59:08.111229 connpy-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-24 20:59:03.000000 connpy-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18355 2024-05-24 20:59:08.111229 connpy-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17235 2024-05-24 20:59:03.000000 connpy-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:59:08.107229 connpy-4.0.1/connpy/
+-rw-r--r--   0 runner    (1001) docker     (127)    16394 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24278 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5181 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8653 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17237 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73927 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33096 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:59:08.111229 connpy-4.0.1/connpy/core_plugins/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14627 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/core_plugins/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/core_plugins/sync_client
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3345 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7133 2024-05-24 20:59:03.000000 connpy-4.0.1/connpy/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:59:08.111229 connpy-4.0.1/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18355 2024-05-24 20:59:08.000000 connpy-4.0.1/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-24 20:59:08.000000 connpy-4.0.1/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:59:08.000000 connpy-4.0.1/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-24 20:59:08.000000 connpy-4.0.1/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-24 20:59:08.000000 connpy-4.0.1/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 20:59:08.000000 connpy-4.0.1/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-24 20:59:08.111229 connpy-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-24 20:59:03.000000 connpy-4.0.1/setup.py
```

### Comparing `connpy-4.0.0b5/LICENSE` & `connpy-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b5/PKG-INFO` & `connpy-4.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 4.0.0b5
+Version: 4.0.1
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
-License: MIT License
+License: Custom Software License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
 Keywords: networking,automation,ssh,telnet,connection manager
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: System :: Networking
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,20 @@
 Requires-Dist: PyYAML
 Requires-Dist: openai
 Requires-Dist: rich
 Requires-Dist: protobuf
 Requires-Dist: google_api_python_client
 Requires-Dist: google_auth_oauthlib
 
-# Conn
+<p align="center">
+  <img src="https://private-user-images.githubusercontent.com/5794882/333731702-63c61be7-da16-4d3c-98da-cae54965d0b7.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTY1ODM3MjQsIm5iZiI6MTcxNjU4MzQyNCwicGF0aCI6Ii81Nzk0ODgyLzMzMzczMTcwMi02M2M2MWJlNy1kYTE2LTRkM2MtOThkYS1jYWU1NDk2NWQwYjcucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDUyNCUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA1MjRUMjA0MzQ0WiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9MGVjZGI3OTQ1OTFlYjY2OGM2NjQzYWNiYThiZTQ3YWMyMWMyNDZjMWIwMDJlZDVjZTU2OTlkNTM0NWEzYWZkYiZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.A3vTyO7h_HWY_IezgEZrBxdIGS_T_gXxLbzP6i2FBwU" alt="App Logo">
+</p>
+
+
+# Connpy
 [![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
 [![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 
 Connpy is a ssh and telnet connection manager and automation module for Linux, Mac and Docker
 
@@ -198,16 +203,16 @@
 
     class Preload:
         def __init__(self, connapp):
             # Applying modification to the config class instance
             connapp.config.modify(modify_config)
     ```
 
-#### Implementing Hooks with `register_pre_hook` and `register_post_hook`
-These methods allow you to define custom logic to be executed before (`register_pre_hook`) or after (`register_post_hook`) the main logic of a method. This is particularly useful for logging, auditing, preprocessing inputs, postprocessing outputs or adding functionalities.
+#### Implementing Method Hooks
+There are 2 methods that allows you to define custom logic to be executed before (`register_pre_hook`) or after (`register_post_hook`) the main logic of a method. This is particularly useful for logging, auditing, preprocessing inputs, postprocessing outputs or adding functionalities.
 
   - **Usage**: Register hooks to methods to execute additional logic before or after the main method execution.
 - **Registration Methods Signature**:
   - `register_pre_hook(pre_hook_method)`: A function that is invoked before the main method is executed. This function should do preprocessing of the arguments.
   - `register_post_hook(post_hook_method)`: A function that is invoked after the main method is executed. This function should do postprocessing of the outputs.
 - **Method Signatures for Pre-Hooks**
   - `pre_hook_method(*args, **kwargs)`
@@ -334,15 +339,15 @@
 ```
 ### Using AI
 ```
 import connpy
 conf = connpy.configfile()
 organization = 'openai-org'
 api_key = "openai-key"
-myia = ai(conf, organization, api_key)
+myia = connpy.ai(conf, organization, api_key)
 input = "go to router 1 and get me the full configuration"
 result = myia.ask(input, dryrun = False)
 print(result)
 ```
 ## http API
 With the Connpy API you can run commands on devices using http requests
```

### Comparing `connpy-4.0.0b5/README.md` & `connpy-4.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-# Conn
+<p align="center">
+  <img src="https://private-user-images.githubusercontent.com/5794882/333731702-63c61be7-da16-4d3c-98da-cae54965d0b7.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTY1ODM3MjQsIm5iZiI6MTcxNjU4MzQyNCwicGF0aCI6Ii81Nzk0ODgyLzMzMzczMTcwMi02M2M2MWJlNy1kYTE2LTRkM2MtOThkYS1jYWU1NDk2NWQwYjcucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDUyNCUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA1MjRUMjA0MzQ0WiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9MGVjZGI3OTQ1OTFlYjY2OGM2NjQzYWNiYThiZTQ3YWMyMWMyNDZjMWIwMDJlZDVjZTU2OTlkNTM0NWEzYWZkYiZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.A3vTyO7h_HWY_IezgEZrBxdIGS_T_gXxLbzP6i2FBwU" alt="App Logo">
+</p>
+
+
+# Connpy
 [![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
 [![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 
 Connpy is a ssh and telnet connection manager and automation module for Linux, Mac and Docker
 
@@ -165,16 +170,16 @@
 
     class Preload:
         def __init__(self, connapp):
             # Applying modification to the config class instance
             connapp.config.modify(modify_config)
     ```
 
-#### Implementing Hooks with `register_pre_hook` and `register_post_hook`
-These methods allow you to define custom logic to be executed before (`register_pre_hook`) or after (`register_post_hook`) the main logic of a method. This is particularly useful for logging, auditing, preprocessing inputs, postprocessing outputs or adding functionalities.
+#### Implementing Method Hooks
+There are 2 methods that allows you to define custom logic to be executed before (`register_pre_hook`) or after (`register_post_hook`) the main logic of a method. This is particularly useful for logging, auditing, preprocessing inputs, postprocessing outputs or adding functionalities.
 
   - **Usage**: Register hooks to methods to execute additional logic before or after the main method execution.
 - **Registration Methods Signature**:
   - `register_pre_hook(pre_hook_method)`: A function that is invoked before the main method is executed. This function should do preprocessing of the arguments.
   - `register_post_hook(post_hook_method)`: A function that is invoked after the main method is executed. This function should do postprocessing of the outputs.
 - **Method Signatures for Pre-Hooks**
   - `pre_hook_method(*args, **kwargs)`
@@ -301,15 +306,15 @@
 ```
 ### Using AI
 ```
 import connpy
 conf = connpy.configfile()
 organization = 'openai-org'
 api_key = "openai-key"
-myia = ai(conf, organization, api_key)
+myia = connpy.ai(conf, organization, api_key)
 input = "go to router 1 and get me the full configuration"
 result = myia.ask(input, dryrun = False)
 print(result)
 ```
 ## http API
 With the Connpy API you can run commands on devices using http requests
```

### Comparing `connpy-4.0.0b5/connpy/__init__.py` & `connpy-4.0.1/connpy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,16 +145,16 @@
 
     class Preload:
         def __init__(self, connapp):
             # Applying modification to the config class instance
             connapp.config.modify(modify_config)
     ```
 
-#### Implementing Hooks with `register_pre_hook` and `register_post_hook`
-These methods allow you to define custom logic to be executed before (`register_pre_hook`) or after (`register_post_hook`) the main logic of a method. This is particularly useful for logging, auditing, preprocessing inputs, postprocessing outputs or adding functionalities.
+#### Implementing Method Hooks
+There are 2 methods that allows you to define custom logic to be executed before (`register_pre_hook`) or after (`register_post_hook`) the main logic of a method. This is particularly useful for logging, auditing, preprocessing inputs, postprocessing outputs or adding functionalities.
 
   - **Usage**: Register hooks to methods to execute additional logic before or after the main method execution.
 - **Registration Methods Signature**:
   - `register_pre_hook(pre_hook_method)`: A function that is invoked before the main method is executed. This function should do preprocessing of the arguments.
   - `register_post_hook(post_hook_method)`: A function that is invoked after the main method is executed. This function should do postprocessing of the outputs.
 - **Method Signatures for Pre-Hooks**
   - `pre_hook_method(*args, **kwargs)`
@@ -388,15 +388,15 @@
 ```
 ### Using AI
 ```
 import connpy
 conf = connpy.configfile()
 organization = 'openai-org'
 api_key = "openai-key"
-myia = ai(conf, organization, api_key)
+myia = connpy.ai(conf, organization, api_key)
 input = "go to router 1 and get me the full configuration"
 result = myia.ask(input, dryrun = False)
 print(result)
 ```
 '''
 from .core import node,nodes
 from .configfile import configfile
@@ -409,9 +409,18 @@
 
 __all__ = ["node", "nodes", "configfile", "connapp", "ai", "Plugins"]
 __author__ = "Federico Luzzi"
 __pdoc__ = {
     'core': False,
     'completion': False,
     'api': False,
-    'plugins': False
+    'plugins': False,
+    'core_plugins': False,
+    'hooks': False,
+    'connapp.start': False,
+    'ai.deferred_class_hooks': False,
+    'configfile.deferred_class_hooks': False,
+    'node.deferred_class_hooks': False,
+    'nodes.deferred_class_hooks': False,
+    'connapp': False,
+    'connapp.encrypt': True
 }
```

### Comparing `connpy-4.0.0b5/connpy/ai.py` & `connpy-4.0.1/connpy/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,25 +174,14 @@
         self.__prompt["confirmation_function"]["parameters"]["properties"]["result"]["enum"] = ["true", "false", "none"]
         self.__prompt["confirmation_function"]["parameters"]["properties"]["response"] = {}
         self.__prompt["confirmation_function"]["parameters"]["properties"]["response"]["description"] = "If the user don't message is not an affiramtion or negation, kindly ask the user to rephrase."
         self.__prompt["confirmation_function"]["parameters"]["properties"]["response"]["type"] = "string"
         self.__prompt["confirmation_function"]["parameters"]["required"] = ["result"]
 
     @MethodHook
-    def process_string(self, s):
-        if s.startswith('[') and s.endswith(']') and not (s.startswith("['") and s.endswith("']")) and not (s.startswith('["') and s.endswith('"]')):
-            # Extract the content inside square brackets and split by comma
-            content = s[1:-1].split(',')
-            # Add single quotes around each item and join them back together with commas
-            new_content = ', '.join(f"'{item.strip()}'" for item in content)
-            # Replace the old content with the new content
-            s = '[' + new_content + ']'
-        return s
-
-    @MethodHook
     def _retry_function(self, function, max_retries, backoff_num, *args):
         #Retry openai requests
         retries = 0
         while retries < max_retries:
             try:
                 myfunction = function(*args)
                 break
```

### Comparing `connpy-4.0.0b5/connpy/api.py` & `connpy-4.0.1/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b5/connpy/completion.py` & `connpy-4.0.1/connpy/completion.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,40 +45,53 @@
             pathstrings[i] += '/'
     pathstrings = [s[2:] if s.startswith('./') else s for s in pathstrings]
     if folderonly:
         pathstrings = [s for s in pathstrings if os.path.isdir(s)]
     return pathstrings
 
 def _get_plugins(which, defaultdir):
-    enabled_files = []
-    disabled_files = []
-    all_files = []
-    all_plugins = {}
-    # Iterate over all files in the specified folder
-    for file in os.listdir(defaultdir + "/plugins"):
-        # Check if the file is a Python file
-        if file.endswith('.py'):
-            enabled_files.append(os.path.splitext(file)[0])
-            all_plugins[os.path.splitext(file)[0]] = os.path.join(defaultdir + "/plugins", file)
-        # Check if the file is a Python backup file
-        elif file.endswith('.py.bkp'):
-            disabled_files.append(os.path.splitext(os.path.splitext(file)[0])[0])
+    # Path to core_plugins relative to this script
+    core_path = os.path.dirname(os.path.realpath(__file__)) + "/core_plugins"
 
+    def get_plugins_from_directory(directory):
+        enabled_files = []
+        disabled_files = []
+        all_plugins = {}
+        # Iterate over all files in the specified folder
+        if os.path.exists(directory):
+            for file in os.listdir(directory):
+                # Check if the file is a Python file
+                if file.endswith('.py'):
+                    enabled_files.append(os.path.splitext(file)[0])
+                    all_plugins[os.path.splitext(file)[0]] = os.path.join(directory, file)
+                # Check if the file is a Python backup file
+                elif file.endswith('.py.bkp'):
+                    disabled_files.append(os.path.splitext(os.path.splitext(file)[0])[0])
+        return enabled_files, disabled_files, all_plugins
+
+    # Get plugins from both directories
+    user_enabled, user_disabled, user_all_plugins = get_plugins_from_directory(defaultdir + "/plugins")
+    core_enabled, core_disabled, core_all_plugins = get_plugins_from_directory(core_path)
+
+    # Combine the results from user and core plugins
+    enabled_files = user_enabled
+    disabled_files = user_disabled
+    all_plugins = {**user_all_plugins, **core_all_plugins}  # Merge dictionaries
+
+    # Return based on the command
     if which == "--disable":
         return enabled_files
     elif which == "--enable":
         return disabled_files
     elif which in ["--del", "--update"]:
-        all_files.extend(enabled_files)
-        all_files.extend(disabled_files)
+        all_files = enabled_files + disabled_files
         return all_files
     elif which == "all":
         return all_plugins
 
-
 def main():
     home = os.path.expanduser("~")
     defaultdir = home + '/.config/conn'
     pathfile = defaultdir + '/.folder'
     try:
         with open(pathfile, "r") as f:
             configdir = f.read().strip()
@@ -140,15 +153,15 @@
         if words[0] in ["bulk", "mv", "cp", "copy"]:
             strings=["--help"]
         if words[0] in ["--rm", "--del", "-r"]:
             strings.extend(folders)
         if words[0] in ["--rm", "--del", "-r", "--mod", "--edit", "-e", "--show", "-s", "mv", "move", "cp", "copy"]:
             strings.extend(nodes)
         if words[0] == "plugin":
-            strings = ["--help", "--add", "--update", "--del", "--enable", "--disable"]
+            strings = ["--help", "--add", "--update", "--del", "--enable", "--disable", "--list"]
         if words[0] in ["run", "import", "export"]:
             strings = ["--help"]
             if words[0] == "export":
                 pathstrings = _getcwd(words, words[0], True)
             else:
                 pathstrings = _getcwd(words, words[0])
             strings.extend(pathstrings)
```

### Comparing `connpy-4.0.0b5/connpy/configfile.py` & `connpy-4.0.1/connpy/configfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 #Imports
 import json
 import os
 import re
 from Crypto.PublicKey import RSA
+from Crypto.Cipher import PKCS1_OAEP
 from pathlib import Path
 from copy import deepcopy
 from .hooks import MethodHook, ClassHook
 
 
 
 #functions and classes
@@ -388,7 +389,36 @@
             nodes.extend(layer2)
             subfolders = [k for k,v in self.connections[f].items() if isinstance(v, dict) and v["type"] == "subfolder"]
             for s in subfolders:
                 layer3 = [k + "@" + s + "@" + f for k,v in self.connections[f][s].items() if isinstance(v, dict) and v["type"] == "connection" and ("@" + profile in v.values() or ( isinstance(v["password"],list) and "@" + profile in v["password"]))]
                 nodes.extend(layer3)
         return nodes
 
+    @MethodHook
+    def encrypt(self, password, keyfile=None):
+        '''
+        Encrypts password using RSA keyfile
+
+        ### Parameters:  
+
+            - password (str): Plaintext password to encrypt.
+
+        ### Optional Parameters:  
+
+            - keyfile  (str): Path/file to keyfile. Default is config keyfile.
+                              
+
+        ### Returns:  
+
+            str: Encrypted password.
+
+        '''
+        if keyfile is None:
+            keyfile = self.key
+        with open(keyfile) as f:
+            key = RSA.import_key(f.read())
+            f.close()
+        publickey = key.publickey()
+        encryptor = PKCS1_OAEP.new(publickey)
+        password = encryptor.encrypt(password.encode("utf-8"))
+        return str(password)
+
```

### Comparing `connpy-4.0.0b5/connpy/connapp.py` & `connpy-4.0.1/connpy/connapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python3
 #Imports
 import os
 import re
-from Crypto.PublicKey import RSA
-from Crypto.Cipher import PKCS1_OAEP
 import ast
 import argparse
 import sys
 import inquirer
 from .core import node,nodes
 from ._version import __version__
 from .api import start_api,stop_api,debug_api
@@ -1281,15 +1279,15 @@
             return False
         if "password" in answer.keys():
             if answer["password"] == "Local Password":
                 passq = [inquirer.Password("password", message="Set Password")]
                 passa = inquirer.prompt(passq)
                 if passa == None:
                     return False
-                answer["password"] = self.encrypt(passa["password"])
+                answer["password"] = self.config.encrypt(passa["password"])
             elif answer["password"] == "Profiles":
                 passq = [(inquirer.Text("password", message="Set a @profile or a comma separated list of @profiles", validate=self._pass_validation))]
                 passa = inquirer.prompt(passq)
                 if passa == None:
                     return False
                 answer["password"] = passa["password"].split(",")
             elif answer["password"] == "No Password":
@@ -1351,15 +1349,15 @@
         else:
             profile["password"] = defaults["password"]
         answer = inquirer.prompt(questions)
         if answer == None:
             return False
         if "password" in answer.keys():
             if answer["password"] != "":
-                answer["password"] = self.encrypt(answer["password"])
+                answer["password"] = self.config.encrypt(answer["password"])
         if "tags" in answer.keys() and answer["tags"]:
             answer["tags"] = ast.literal_eval(answer["tags"])
         result = {**answer, **profile}
         result["id"] = unique
         return result
 
     def _questions_bulk(self):
@@ -1379,15 +1377,15 @@
         answer = inquirer.prompt(questions)
         if answer == None:
             return False
         if "password" in answer.keys():
             if answer["password"] == "Local Password":
                 passq = [inquirer.Password("password", message="Set Password")]
                 passa = inquirer.prompt(passq)
-                answer["password"] = self.encrypt(passa["password"])
+                answer["password"] = self.config.encrypt(passa["password"])
             elif answer["password"] == "Profiles":
                 passq = [(inquirer.Text("password", message="Set a @profile or a comma separated list of @profiles", validate=self._pass_validation))]
                 passa = inquirer.prompt(passq)
                 answer["password"] = passa["password"].split(",")
             elif answer["password"] == "No Password":
                 answer["password"] = ""
         answer["type"] = "connection"
@@ -1546,35 +1544,7 @@
     vrouter1@aws:
       id: 4
     vrouterN@aws:
       id: 5
   output: null
 ...'''
 
-    def encrypt(self, password, keyfile=None):
-        '''
-        Encrypts password using RSA keyfile
-
-        ### Parameters:  
-
-            - password (str): Plaintext password to encrypt.
-
-        ### Optional Parameters:  
-
-            - keyfile  (str): Path/file to keyfile. Default is config keyfile.
-                              
-
-        ### Returns:  
-
-            str: Encrypted password.
-
-        '''
-        if keyfile is None:
-            keyfile = self.config.key
-        with open(keyfile) as f:
-            key = RSA.import_key(f.read())
-            f.close()
-        publickey = key.publickey()
-        encryptor = PKCS1_OAEP.new(publickey)
-        password = encryptor.encrypt(password.encode("utf-8"))
-        return str(password)
-
```

### Comparing `connpy-4.0.0b5/connpy/core.py` & `connpy-4.0.1/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b5/connpy/core_plugins/sync.py` & `connpy-4.0.1/connpy/core_plugins/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,29 +31,42 @@
             self.sync = False
 
     def login(self):
         creds = None
         # The file token.json stores the user's access and refresh tokens.
         if os.path.exists(self.token_file):
             creds = Credentials.from_authorized_user_file(self.token_file, self.scopes)
-        
-        # If there are no valid credentials available, let the user log in.
-        if not creds or not creds.valid:
-            if creds and creds.expired and creds.refresh_token:
-                creds.refresh(Request())
-            else:
-                flow = InstalledAppFlow.from_client_secrets_file(
-                    self.google_client, self.scopes)
-                creds = flow.run_local_server(port=0, access_type='offline')
-            
-            # Save the credentials for the next run
+
+        try:
+            # If there are no valid credentials available, let the user log in.
+            if not creds or not creds.valid:
+                if creds and creds.expired and creds.refresh_token:
+                    creds.refresh(Request())
+                else:
+                    flow = InstalledAppFlow.from_client_secrets_file(
+                        self.google_client, self.scopes)
+                    creds = flow.run_local_server(port=0, access_type='offline')
+
+                # Save the credentials for the next run
+                with open(self.token_file, 'w') as token:
+                    token.write(creds.to_json())
+
+            print("Logged in successfully.")
+
+        except RefreshError as e:
+            # If refresh fails, delete the invalid token file and start a new login flow
+            if os.path.exists(self.token_file):
+                os.remove(self.token_file)
+            print("Existing token was invalid and has been removed. Please log in again.")
+            flow = InstalledAppFlow.from_client_secrets_file(
+                self.google_client, self.scopes)
+            creds = flow.run_local_server(port=0, access_type='offline')
             with open(self.token_file, 'w') as token:
                 token.write(creds.to_json())
-
-        print("Logged in successfully.")
+            print("Logged in successfully after re-authentication.")
 
     def logout(self):
         if os.path.exists(self.token_file):
             os.remove(self.token_file)
             print("Logged out successfully.")
         else:
             print("No credentials file found. Already logged out.")
@@ -296,14 +309,16 @@
         return 0
 
     def config_listener_post(self, args, kwargs):
         if self.sync:
             if self.check_login_status() == True:
                 if not kwargs["result"]:
                     self.compress_and_upload()
+            else:
+                print("Sync cannot be performed. Please check your login status.")
         return kwargs["result"]
 
     def config_listener_pre(self, *args, **kwargs):
         try:
             self.sync = self.connapp.config.config["sync"]
         except:
             self.sync = False
```

### Comparing `connpy-4.0.0b5/connpy/hooks.py` & `connpy-4.0.1/connpy/hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 #Imports
-from functools import wraps, partial
+from functools import wraps, partial, update_wrapper
 
 #functions and classes
 
 class MethodHook:
     """Decorator class to enable Methods hooking"""
 
     def __init__(self, func):
@@ -55,14 +55,15 @@
         """Register a function to be called after the original function"""
         self.post_hooks.append(hook)
 
 class ClassHook:
     """Decorator class to enable Class Modifying"""
     def __init__(self, cls):
         self.cls = cls
+        update_wrapper(self, cls, updated=())  # Update wrapper without changing underlying items
         # Initialize deferred class hooks if they don't already exist
         if not hasattr(cls, 'deferred_class_hooks'):
             cls.deferred_class_hooks = []
 
     def __call__(self, *args, **kwargs):
         instance = self.cls(*args, **kwargs)
         # Attach instance-specific modify method
```

### Comparing `connpy-4.0.0b5/connpy/plugins.py` & `connpy-4.0.1/connpy/plugins.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b5/connpy.egg-info/PKG-INFO` & `connpy-4.0.1/connpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 4.0.0b5
+Version: 4.0.1
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
-License: MIT License
+License: Custom Software License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
 Keywords: networking,automation,ssh,telnet,connection manager
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: System :: Networking
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,20 @@
 Requires-Dist: PyYAML
 Requires-Dist: openai
 Requires-Dist: rich
 Requires-Dist: protobuf
 Requires-Dist: google_api_python_client
 Requires-Dist: google_auth_oauthlib
 
-# Conn
+<p align="center">
+  <img src="https://private-user-images.githubusercontent.com/5794882/333731702-63c61be7-da16-4d3c-98da-cae54965d0b7.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTY1ODM3MjQsIm5iZiI6MTcxNjU4MzQyNCwicGF0aCI6Ii81Nzk0ODgyLzMzMzczMTcwMi02M2M2MWJlNy1kYTE2LTRkM2MtOThkYS1jYWU1NDk2NWQwYjcucG5nP1gtQW16LUFsZ29yaXRobT1BV1M0LUhNQUMtU0hBMjU2JlgtQW16LUNyZWRlbnRpYWw9QUtJQVZDT0RZTFNBNTNQUUs0WkElMkYyMDI0MDUyNCUyRnVzLWVhc3QtMSUyRnMzJTJGYXdzNF9yZXF1ZXN0JlgtQW16LURhdGU9MjAyNDA1MjRUMjA0MzQ0WiZYLUFtei1FeHBpcmVzPTMwMCZYLUFtei1TaWduYXR1cmU9MGVjZGI3OTQ1OTFlYjY2OGM2NjQzYWNiYThiZTQ3YWMyMWMyNDZjMWIwMDJlZDVjZTU2OTlkNTM0NWEzYWZkYiZYLUFtei1TaWduZWRIZWFkZXJzPWhvc3QmYWN0b3JfaWQ9MCZrZXlfaWQ9MCZyZXBvX2lkPTAifQ.A3vTyO7h_HWY_IezgEZrBxdIGS_T_gXxLbzP6i2FBwU" alt="App Logo">
+</p>
+
+
+# Connpy
 [![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
 [![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 
 Connpy is a ssh and telnet connection manager and automation module for Linux, Mac and Docker
 
@@ -198,16 +203,16 @@
 
     class Preload:
         def __init__(self, connapp):
             # Applying modification to the config class instance
             connapp.config.modify(modify_config)
     ```
 
-#### Implementing Hooks with `register_pre_hook` and `register_post_hook`
-These methods allow you to define custom logic to be executed before (`register_pre_hook`) or after (`register_post_hook`) the main logic of a method. This is particularly useful for logging, auditing, preprocessing inputs, postprocessing outputs or adding functionalities.
+#### Implementing Method Hooks
+There are 2 methods that allows you to define custom logic to be executed before (`register_pre_hook`) or after (`register_post_hook`) the main logic of a method. This is particularly useful for logging, auditing, preprocessing inputs, postprocessing outputs or adding functionalities.
 
   - **Usage**: Register hooks to methods to execute additional logic before or after the main method execution.
 - **Registration Methods Signature**:
   - `register_pre_hook(pre_hook_method)`: A function that is invoked before the main method is executed. This function should do preprocessing of the arguments.
   - `register_post_hook(post_hook_method)`: A function that is invoked after the main method is executed. This function should do postprocessing of the outputs.
 - **Method Signatures for Pre-Hooks**
   - `pre_hook_method(*args, **kwargs)`
@@ -334,15 +339,15 @@
 ```
 ### Using AI
 ```
 import connpy
 conf = connpy.configfile()
 organization = 'openai-org'
 api_key = "openai-key"
-myia = ai(conf, organization, api_key)
+myia = connpy.ai(conf, organization, api_key)
 input = "go to router 1 and get me the full configuration"
 result = myia.ask(input, dryrun = False)
 print(result)
 ```
 ## http API
 With the Connpy API you can run commands on devices using http requests
```

### Comparing `connpy-4.0.0b5/setup.cfg` & `connpy-4.0.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 description = Connpy is a SSH/Telnet connection manager and automation module
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = networking, automation, ssh, telnet, connection manager
 author = Federico Luzzi
 author_email = fluzzi@gmail.com
 url = https://github.com/fluzzi/connpy
-license = MIT License
+license = Custom Software License
 license_files = LICENSE
 project_urls = 
 	Bug Tracker = https://github.com/fluzzi/connpy/issues
 	Documentation = https://fluzzi.github.io/connpy/
 classifiers = 
 	Development Status :: 4 - Beta
 	Topic :: System :: Networking
```

