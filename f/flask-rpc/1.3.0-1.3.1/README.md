# Comparing `tmp/flask_rpc-1.3.0.tar.gz` & `tmp/flask_rpc-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_rpc-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_rpc-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_rpc-1.3.0.tar` & `flask_rpc-1.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-1.3.0/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-1.3.0/LICENSE
--rw-r--r--   0        0        0     4221 2024-04-18 12:52:37.837069 flask_rpc-1.3.0/README.md
--rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-1.3.0/app/__init__.py
--rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-1.3.0/app/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-1.3.0/app/models/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-1.3.0/app/models/clients.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-1.3.0/app/models/users.py
--rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-1.3.0/app/rpc/__init__.py
--rw-r--r--   0        0        0      522 2024-04-18 09:59:24.864451 flask_rpc-1.3.0/app/rpc/auth/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-1.3.0/app/rpc/auth/funcs/__init__.py
--rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-1.3.0/app/rpc/auth/funcs/login.py
--rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-1.3.0/app/rpc/auth/funcs/logout.py
--rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-1.3.0/app/rpc/auth/funcs/session.py
--rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-1.3.0/app/rpc/clients/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-1.3.0/app/rpc/clients/funcs/__init__.py
--rw-r--r--   0        0        0      263 2024-04-13 11:01:57.572442 flask_rpc-1.3.0/app/rpc/tester/__init__.py
--rw-r--r--   0        0        0      293 2024-04-13 10:27:56.719801 flask_rpc-1.3.0/app/rpc/tester/funcs/__init__.py
--rw-r--r--   0        0        0     1290 2024-04-18 11:06:57.530208 flask_rpc-1.3.0/app/templates/index.html
--rw-r--r--   0        0        0       22 2024-04-24 18:59:43.378441 flask_rpc-1.3.0/flask_rpc/__init__.py
--rw-r--r--   0        0        0      164 2024-04-18 09:45:56.143643 flask_rpc-1.3.0/flask_rpc/latest.py
--rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 flask_rpc-1.3.0/flask_rpc/version_1_0/__init__.py
--rw-r--r--   0        0        0      160 2024-04-18 09:54:54.237265 flask_rpc-1.3.0/flask_rpc/version_1_0/_protocols.py
--rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 flask_rpc-1.3.0/flask_rpc/version_1_0/auth_session_key.py
--rw-r--r--   0        0        0      130 2024-04-18 11:07:12.257730 flask_rpc-1.3.0/flask_rpc/version_1_0/model.py
--rw-r--r--   0        0        0      480 2024-04-18 11:07:12.256482 flask_rpc-1.3.0/flask_rpc/version_1_0/request.py
--rw-r--r--   0        0        0     1159 2024-04-24 18:56:59.717811 flask_rpc-1.3.0/flask_rpc/version_1_0/response.py
--rw-r--r--   0        0        0     5472 2024-04-24 13:27:39.942643 flask_rpc-1.3.0/flask_rpc/version_1_0/rpc.py
--rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 flask_rpc-1.3.0/flask_rpc/version_1_0/utilities.py
--rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-1.3.0/requirements.txt
--rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-1.3.0/requirements_dev.txt
--rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-1.3.0/test.py
--rw-r--r--   0        0        0     4860 1970-01-01 00:00:00.000000 flask_rpc-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-1.3.1/LICENSE
+-rw-r--r--   0        0        0     4232 2024-05-24 06:18:27.779071 flask_rpc-1.3.1/README.md
+-rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-1.3.1/app/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-1.3.1/app/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-1.3.1/app/models/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-1.3.1/app/models/clients.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-1.3.1/app/models/users.py
+-rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-1.3.1/app/rpc/__init__.py
+-rw-r--r--   0        0        0      522 2024-04-18 09:59:24.864451 flask_rpc-1.3.1/app/rpc/auth/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-1.3.1/app/rpc/auth/funcs/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-1.3.1/app/rpc/auth/funcs/login.py
+-rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-1.3.1/app/rpc/auth/funcs/logout.py
+-rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-1.3.1/app/rpc/auth/funcs/session.py
+-rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-1.3.1/app/rpc/clients/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-1.3.1/app/rpc/clients/funcs/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-13 11:01:57.572442 flask_rpc-1.3.1/app/rpc/tester/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-13 10:27:56.719801 flask_rpc-1.3.1/app/rpc/tester/funcs/__init__.py
+-rw-r--r--   0        0        0     1290 2024-04-18 11:06:57.530208 flask_rpc-1.3.1/app/templates/index.html
+-rw-r--r--   0        0        0       22 2024-05-24 06:19:18.698645 flask_rpc-1.3.1/flask_rpc/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-18 09:45:56.143643 flask_rpc-1.3.1/flask_rpc/latest.py
+-rw-r--r--   0        0        0      244 2024-04-18 09:27:36.641998 flask_rpc-1.3.1/flask_rpc/version_1_0/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-18 09:54:54.237265 flask_rpc-1.3.1/flask_rpc/version_1_0/_protocols.py
+-rw-r--r--   0        0        0      395 2024-04-18 09:21:53.897194 flask_rpc-1.3.1/flask_rpc/version_1_0/auth_session_key.py
+-rw-r--r--   0        0        0      130 2024-04-18 11:07:12.257730 flask_rpc-1.3.1/flask_rpc/version_1_0/model.py
+-rw-r--r--   0        0        0      480 2024-04-18 11:07:12.256482 flask_rpc-1.3.1/flask_rpc/version_1_0/request.py
+-rw-r--r--   0        0        0     1159 2024-04-24 18:56:59.717811 flask_rpc-1.3.1/flask_rpc/version_1_0/response.py
+-rw-r--r--   0        0        0     5472 2024-04-24 13:27:39.942643 flask_rpc-1.3.1/flask_rpc/version_1_0/rpc.py
+-rw-r--r--   0        0        0      547 2024-04-18 10:08:33.791808 flask_rpc-1.3.1/flask_rpc/version_1_0/utilities.py
+-rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-1.3.1/requirements.txt
+-rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-1.3.1/requirements_dev.txt
+-rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-1.3.1/test.py
+-rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 flask_rpc-1.3.1/PKG-INFO
```

### Comparing `flask_rpc-1.3.0/.gitignore` & `flask_rpc-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/LICENSE` & `flask_rpc-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/README.md` & `flask_rpc-1.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 Flask - Remote Procedure Call (RPC) is a simple
 library that allows you to expose functions
 in your Flask application to be called
 remotely. It is designed to be straightforward
 to use and easy to understand.
 
-Flask-RPC uses [wRPC (Wee RPC)](https://github.com/CheeseCake87/wRPC) 
+Flask-RPC currently only uses the [weeRPC](https://github.com/CheeseCake87/weeRPC) 
 as its protocol, which is a micro JSON-based protocol that allows for
 easy communication between the client and server.
 
 This extension is designed to stay slim and provides
-methods for generating requests and request responses.
+methods for generating requests and responses.
 
 It does not enforce or validate the data passed in, or the
-data being sent back; this is left to the user to implement
-in whatever way they feel comfortable (or not at all, if there's
+data being sent back; this is left to you to implement
+in whatever way you feel comfortable (or not at all, if there's
 no need for it)
 
-Flask-RPC does validate the request coming in using
-Pydantic.
+Flask-RPC does validate the version of weeRPC on an incoming request. This 
+is to ensure that the request is structured in a way that the version 
+of RPC you are using expects.
 
-This is to ensure that the request is structured
-in the way to whatever version of Flask-RPC you are using.
+Other than that, you are free to use whatever data validation
+you feel comfortable with. Pydantic and Marshmallow are good choices.
 
-Other than that, the user is free to use whatever data validation
-they feel comfortable with. Pydantic and Marshmallow are good choices.
-
-The typical request/response cycle is as follows:
+The typical request/response cycle of weeRPC is as follows:
 
 **Request**
 
 ```json
 {
   "wrpc": 1.0,
   "function": "add_numbers",
@@ -165,15 +163,15 @@
 
 ## Security
 
 You can lock down RPC routes by using sessions and or host checking.
 
 ### Session Auth
 
-`from quart_rpc.latest import RPCAuthSessionKey`
+`from flask_rpc.latest import RPCAuthSessionKey`
 
 ```python
 ...
 RPC(
     app,  # or RPC(blueprint, ...)
     url_prefix="/rpc",
     session_auth=RPCAuthSessionKey("logged_in", [True]),
@@ -213,8 +211,8 @@
     url_prefix="/rpc",
     host_auth=["127.0.0.1:5000"],
     functions={
         "add_numbers": add_numbers
     }
 )
 ...
-```
+```
```

### Comparing `flask_rpc-1.3.0/app/__init__.py` & `flask_rpc-1.3.1/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/app/models/clients.py` & `flask_rpc-1.3.1/app/models/clients.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/app/models/users.py` & `flask_rpc-1.3.1/app/models/users.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/app/rpc/auth/__init__.py` & `flask_rpc-1.3.1/app/rpc/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/app/rpc/clients/funcs/__init__.py` & `flask_rpc-1.3.1/app/rpc/clients/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/app/templates/index.html` & `flask_rpc-1.3.1/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/flask_rpc/version_1_0/response.py` & `flask_rpc-1.3.1/flask_rpc/version_1_0/response.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/flask_rpc/version_1_0/rpc.py` & `flask_rpc-1.3.1/flask_rpc/version_1_0/rpc.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/flask_rpc/version_1_0/utilities.py` & `flask_rpc-1.3.1/flask_rpc/version_1_0/utilities.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/pyproject.toml` & `flask_rpc-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/test.py` & `flask_rpc-1.3.1/test.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-1.3.0/PKG-INFO` & `flask_rpc-1.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rpc
-Version: 1.3.0
+Version: 1.3.1
 Summary: Turn Flask into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -25,36 +25,34 @@
 
 Flask - Remote Procedure Call (RPC) is a simple
 library that allows you to expose functions
 in your Flask application to be called
 remotely. It is designed to be straightforward
 to use and easy to understand.
 
-Flask-RPC uses [wRPC (Wee RPC)](https://github.com/CheeseCake87/wRPC) 
+Flask-RPC currently only uses the [weeRPC](https://github.com/CheeseCake87/weeRPC) 
 as its protocol, which is a micro JSON-based protocol that allows for
 easy communication between the client and server.
 
 This extension is designed to stay slim and provides
-methods for generating requests and request responses.
+methods for generating requests and responses.
 
 It does not enforce or validate the data passed in, or the
-data being sent back; this is left to the user to implement
-in whatever way they feel comfortable (or not at all, if there's
+data being sent back; this is left to you to implement
+in whatever way you feel comfortable (or not at all, if there's
 no need for it)
 
-Flask-RPC does validate the request coming in using
-Pydantic.
+Flask-RPC does validate the version of weeRPC on an incoming request. This 
+is to ensure that the request is structured in a way that the version 
+of RPC you are using expects.
 
-This is to ensure that the request is structured
-in the way to whatever version of Flask-RPC you are using.
+Other than that, you are free to use whatever data validation
+you feel comfortable with. Pydantic and Marshmallow are good choices.
 
-Other than that, the user is free to use whatever data validation
-they feel comfortable with. Pydantic and Marshmallow are good choices.
-
-The typical request/response cycle is as follows:
+The typical request/response cycle of weeRPC is as follows:
 
 **Request**
 
 ```json
 {
   "wrpc": 1.0,
   "function": "add_numbers",
@@ -182,15 +180,15 @@
 
 ## Security
 
 You can lock down RPC routes by using sessions and or host checking.
 
 ### Session Auth
 
-`from quart_rpc.latest import RPCAuthSessionKey`
+`from flask_rpc.latest import RPCAuthSessionKey`
 
 ```python
 ...
 RPC(
     app,  # or RPC(blueprint, ...)
     url_prefix="/rpc",
     session_auth=RPCAuthSessionKey("logged_in", [True]),
@@ -231,7 +229,8 @@
     host_auth=["127.0.0.1:5000"],
     functions={
         "add_numbers": add_numbers
     }
 )
 ...
 ```
+
```

