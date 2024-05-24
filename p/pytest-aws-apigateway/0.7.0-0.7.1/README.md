# Comparing `tmp/pytest_aws_apigateway-0.7.0.tar.gz` & `tmp/pytest_aws_apigateway-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_aws_apigateway-0.7.0.tar", last modified: Sat May 18 10:15:31 2024, max compression
+gzip compressed data, was "pytest_aws_apigateway-0.7.1.tar", last modified: Fri May 24 11:05:04 2024, max compression
```

## Comparing `pytest_aws_apigateway-0.7.0.tar` & `pytest_aws_apigateway-0.7.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.580045 pytest_aws_apigateway-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.572045 pytest_aws_apigateway-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.576045 pytest_aws_apigateway-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-18 10:15:31.580045 pytest_aws_apigateway-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.576045 pytest_aws_apigateway-0.7.0/changes/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/changes/+.fix.md
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/changes/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 10:15:31.580045 pytest_aws_apigateway-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.572045 pytest_aws_apigateway-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.576045 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.580045 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-18 10:15:31.000000 pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.576045 pytest_aws_apigateway-0.7.0/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tasks/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:31.580045 pytest_aws_apigateway-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/test_apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/test_powertools.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-18 10:15:21.000000 pytest_aws_apigateway-0.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:05:04.135987 pytest_aws_apigateway-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:05:04.127987 pytest_aws_apigateway-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:05:04.127987 pytest_aws_apigateway-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-24 11:05:04.135987 pytest_aws_apigateway-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:05:04.131987 pytest_aws_apigateway-0.7.1/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/changes/+.fix.md
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 11:05:04.135987 pytest_aws_apigateway-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:05:04.127987 pytest_aws_apigateway-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:05:04.131987 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:05:04.131987 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-24 11:05:04.000000 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-24 11:05:04.000000 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:05:04.000000 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-24 11:05:04.000000 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 11:05:04.000000 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 11:05:04.000000 pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:05:04.131987 pytest_aws_apigateway-0.7.1/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/tasks/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:05:04.131987 pytest_aws_apigateway-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/tests/test_apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/tests/test_powertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-24 11:04:57.000000 pytest_aws_apigateway-0.7.1/tox.ini
```

### Comparing `pytest_aws_apigateway-0.7.0/.github/workflows/main.yml` & `pytest_aws_apigateway-0.7.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.7.0/CHANGELOG.md` & `pytest_aws_apigateway-0.7.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# pytest-aws-apigateway 0.7.1 (2024-05-24)
+
+No significant changes.
+
+
 # pytest-aws-apigateway 0.7.0 (2024-05-18)
 
 ### Features
 
 - Can now pass in a custom lambda context.
```

### Comparing `pytest_aws_apigateway-0.7.0/LICENSE` & `pytest_aws_apigateway-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.7.0/PKG-INFO` & `pytest_aws_apigateway-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.7.0
+Version: 0.7.1
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -62,15 +62,15 @@
 
 def test_hello_world(apigateway_mock: ApiGatewayMock):
     apigateway_mock.add_integration(
         "/", handler=handler, method="GET", endpoint="https://greetings/"
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/")
+        resp = client.get("https://greetings/")
         assert resp.json() == {"message": "Hello World!"}
 ```
 
 
 ## License
 
 `pytest-aws-apigateway` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `pytest_aws_apigateway-0.7.0/README.md` & `pytest_aws_apigateway-0.7.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 def test_hello_world(apigateway_mock: ApiGatewayMock):
     apigateway_mock.add_integration(
         "/", handler=handler, method="GET", endpoint="https://greetings/"
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/")
+        resp = client.get("https://greetings/")
         assert resp.json() == {"message": "Hello World!"}
 ```
 
 
 ## License
 
 `pytest-aws-apigateway` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `pytest_aws_apigateway-0.7.0/pyproject.toml` & `pytest_aws_apigateway-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/apigateway.py` & `pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway/apigateway.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/context.py` & `pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway/context.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway/integration.py` & `pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/PKG-INFO` & `pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.7.0
+Version: 0.7.1
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -62,15 +62,15 @@
 
 def test_hello_world(apigateway_mock: ApiGatewayMock):
     apigateway_mock.add_integration(
         "/", handler=handler, method="GET", endpoint="https://greetings/"
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/")
+        resp = client.get("https://greetings/")
         assert resp.json() == {"message": "Hello World!"}
 ```
 
 
 ## License
 
 `pytest-aws-apigateway` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `pytest_aws_apigateway-0.7.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt` & `pytest_aws_apigateway-0.7.1/src/pytest_aws_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.7.0/tasks/release.py` & `pytest_aws_apigateway-0.7.1/tasks/release.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.7.0/tests/test_apigateway.py` & `pytest_aws_apigateway-0.7.1/tests/test_apigateway.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,111 +7,111 @@
 
 
 def test_root_resource(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
         return {"statusCode": 200, "body": json.dumps({"body": "hello"})}
 
     apigateway_mock.add_integration(
-        "/", handler=handler, method="GET", endpoint="https://some/"
+        "/", handler=handler, method="GET", endpoint="https://foo/"
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/")
+        resp = client.get("https://foo/")
         assert resp.json() == {"body": "hello"}
 
 
 def test_child_resource(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
         return {"statusCode": 200, "body": json.dumps({"body": "hello"})}
 
     apigateway_mock.add_integration(
-        "/orders", handler=handler, method="GET", endpoint="https://some/"
+        "/orders", handler=handler, method="GET", endpoint="https://foo/"
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/orders")
+        resp = client.get("https://foo/orders")
         assert resp.json() == {"body": "hello"}
 
 
 def test_child_resource_with_parameter(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
         params = event["pathParameters"]
         return {"statusCode": 200, "body": json.dumps({"params": params})}
 
     apigateway_mock.add_integration(
-        "/orders/{id}", handler=handler, method="GET", endpoint="https://some/"
+        "/orders/{id}", handler=handler, method="GET", endpoint="https://foo/"
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/orders/123")
+        resp = client.get("https://foo/orders/123")
         assert resp.json() == {"params": {"id": "123"}}
 
 
 def test_invalid_output_format_returns_500(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
         return {"statusCode": "200"}
 
     apigateway_mock.add_integration(
-        "/", handler=handler, method="GET", endpoint="https://some/"
+        "/", handler=handler, method="GET", endpoint="https://foo/"
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/")
+        resp = client.get("https://foo/")
         assert resp.status_code == 500
 
 
 def test_output_dict_is_transformed_to_response(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
         return {"statusCode": 200}
 
     apigateway_mock.add_integration(
-        "/", handler=handler, method="GET", endpoint="https://some/"
+        "/", handler=handler, method="GET", endpoint="https://foo/"
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/")
+        resp = client.get("https://foo/")
         assert resp.status_code == 200
 
 
 def test_match_on_ANY_method(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
         return {"statusCode": 200, "body": json.dumps({"body": "hello"})}
 
     apigateway_mock.add_integration(
-        "/", handler=handler, method="ANY", endpoint="https://some/"
+        "/", handler=handler, method="ANY", endpoint="https://foo/"
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/")
+        resp = client.get("https://foo/")
         assert resp.json() == {"body": "hello"}
 
 
 def test_headers_are_forwarded(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
         return {"statusCode": 200, "body": json.dumps(event["headers"])}
 
     apigateway_mock.add_integration(
-        "/", handler=handler, method="ANY", endpoint="https://some/"
+        "/", handler=handler, method="ANY", endpoint="https://foo/"
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/", headers={"x-test": "testing"})
+        resp = client.get("https://foo/", headers={"x-test": "testing"})
         assert resp.json()["x-test"] == "testing"
 
 
 def test_query_strings_are_forwarded(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
         return {"statusCode": 200, "body": json.dumps(event["queryStringParameters"])}
 
     apigateway_mock.add_integration(
-        "/", handler=handler, method="ANY", endpoint="https://some/"
+        "/", handler=handler, method="ANY", endpoint="https://foo/"
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/?testing&foo=bar")
+        resp = client.get("https://foo/?testing&foo=bar")
         assert "testing" in resp.json()
         assert resp.json()["foo"] == "bar"
 
 
 def test_custom_context_object_passed_to_handler(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
         return {"statusCode": 200, "body": json.dumps({"body": context.function_name})}
@@ -123,19 +123,19 @@
         invoked_function_arn="arn:aws:lambda:us-east-1:123456789012:function:testApiGateway",
         function_name="test-handler",
         function_version="$LATEST",
         memory_limit_in_mb="128",
     )
 
     apigateway_mock.add_integration(
-        "/", handler=handler, method="GET", endpoint="https://some/", context=context
+        "/", handler=handler, method="GET", endpoint="https://foo/", context=context
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/")
+        resp = client.get("https://foo/")
         assert resp.json() == {"body": "test-handler"}
 
 
 def test_custom_context_generator_passed_to_handler(apigateway_mock: ApiGatewayMock):
     def handler(event, context):
         return {"statusCode": 200, "body": json.dumps({"body": context.function_name})}
 
@@ -147,13 +147,13 @@
             invoked_function_arn="arn:aws:lambda:us-east-1:123456789012:function:testApiGateway",
             function_name="test-handler",
             function_version="$LATEST",
             memory_limit_in_mb="128",
         )
 
     apigateway_mock.add_integration(
-        "/", handler=handler, method="GET", endpoint="https://some/", context=context
+        "/", handler=handler, method="GET", endpoint="https://foo/", context=context
     )
 
     with httpx.Client() as client:
-        resp = client.get("https://some/")
+        resp = client.get("https://foo/")
         assert resp.json() == {"body": "test-handler"}
```

### Comparing `pytest_aws_apigateway-0.7.0/tests/test_plugin.py` & `pytest_aws_apigateway-0.7.1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.7.0/tests/test_powertools.py` & `pytest_aws_apigateway-0.7.1/tests/test_powertools.py`

 * *Files identical despite different names*

