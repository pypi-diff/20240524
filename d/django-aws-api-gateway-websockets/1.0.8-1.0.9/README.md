# Comparing `tmp/django-aws-api-gateway-websockets-1.0.8.tar.gz` & `tmp/django-aws-api-gateway-websockets-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-aws-api-gateway-websockets-1.0.8.tar", last modified: Fri Dec  9 11:52:09 2022, max compression
+gzip compressed data, was "dist/django-aws-api-gateway-websockets-1.0.9.tar", last modified: Mon Dec 12 16:39:27 2022, max compression
```

## Comparing `django-aws-api-gateway-websockets-1.0.8.tar` & `django-aws-api-gateway-websockets-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-09 11:52:09.619245 django-aws-api-gateway-websockets-1.0.8/
--rw-rw-r--   0 steve     (1000) steve     (1000)       58 2021-10-18 22:44:01.000000 django-aws-api-gateway-websockets-1.0.8/AUTHORS
--rw-rw-r--   0 steve     (1000) steve     (1000)     1068 2022-08-31 09:10:20.000000 django-aws-api-gateway-websockets-1.0.8/LICENSE
--rw-rw-r--   0 steve     (1000) steve     (1000)    28432 2022-12-09 11:52:09.619245 django-aws-api-gateway-websockets-1.0.8/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)    27519 2022-12-09 11:50:43.000000 django-aws-api-gateway-websockets-1.0.8/README.md
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-09 11:52:09.619245 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/
--rw-rw-r--   0 steve     (1000) steve     (1000)        0 2022-09-13 13:47:02.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3582 2022-12-09 09:17:47.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/admin.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      306 2022-01-17 21:05:19.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/apps.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-09 11:52:09.619245 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/management/
--rw-rw-r--   0 steve     (1000) steve     (1000)        0 2022-07-06 14:29:45.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/management/__init__.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-09 11:52:09.619245 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/management/commands/
--rw-rw-r--   0 steve     (1000) steve     (1000)        0 2022-07-06 14:29:50.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/management/commands/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      370 2022-08-31 14:29:46.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/management/commands/clearWebSocketSessions.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      612 2022-09-13 14:31:41.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/management/commands/createApiGateway.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      668 2022-07-06 14:56:50.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/management/commands/createCustomDomain.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-09 11:52:09.619245 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/migrations/
--rw-rw-r--   0 steve     (1000) steve     (1000)     2767 2022-01-17 22:00:46.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/migrations/0001_initial.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      387 2022-01-17 23:02:23.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/migrations/0002_rename_author_websocketsession_user.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     7108 2022-07-08 11:09:17.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/migrations/0003_auto_20220706_1018.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     1765 2022-12-08 18:57:06.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/migrations/0004_auto_20221208_1227.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      451 2022-12-08 19:37:34.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/migrations/0005_apigatewayadditionalroute_deployed.py
--rw-rw-r--   0 steve     (1000) steve     (1000)        0 2022-01-17 20:53:32.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/migrations/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    15285 2022-12-08 19:34:30.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/models.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    11513 2022-09-16 15:57:30.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/views.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-09 11:52:09.619245 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets.egg-info/
--rw-rw-r--   0 steve     (1000) steve     (1000)    28432 2022-12-09 11:52:09.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets.egg-info/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)     1409 2022-12-09 11:52:09.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets.egg-info/SOURCES.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        1 2022-12-09 11:52:09.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets.egg-info/dependency_links.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        1 2021-10-19 16:43:32.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets.egg-info/not-zip-safe
--rw-rw-r--   0 steve     (1000) steve     (1000)       14 2022-12-09 11:52:09.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets.egg-info/requires.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       34 2022-12-09 11:52:09.000000 django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets.egg-info/top_level.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)      852 2022-12-09 11:51:39.000000 django-aws-api-gateway-websockets-1.0.8/pyproject.toml
--rw-rw-r--   0 steve     (1000) steve     (1000)     1882 2022-12-09 11:52:09.619245 django-aws-api-gateway-websockets-1.0.8/setup.cfg
--rw-rw-r--   0 steve     (1000) steve     (1000)       38 2021-10-18 22:44:01.000000 django-aws-api-gateway-websockets-1.0.8/setup.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-12 16:39:27.257401 django-aws-api-gateway-websockets-1.0.9/
+-rw-rw-r--   0 steve     (1000) steve     (1000)       58 2021-10-18 22:44:01.000000 django-aws-api-gateway-websockets-1.0.9/AUTHORS
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1068 2022-08-31 09:10:20.000000 django-aws-api-gateway-websockets-1.0.9/LICENSE
+-rw-rw-r--   0 steve     (1000) steve     (1000)    28432 2022-12-12 16:39:27.257401 django-aws-api-gateway-websockets-1.0.9/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)    27519 2022-12-09 11:50:43.000000 django-aws-api-gateway-websockets-1.0.9/README.md
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-12 16:39:27.253401 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/
+-rw-rw-r--   0 steve     (1000) steve     (1000)        0 2022-09-13 13:47:02.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3582 2022-12-09 09:17:47.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/admin.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)      306 2022-01-17 21:05:19.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/apps.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-12 16:39:27.253401 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/management/
+-rw-rw-r--   0 steve     (1000) steve     (1000)        0 2022-07-06 14:29:45.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/management/__init__.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-12 16:39:27.253401 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/management/commands/
+-rw-rw-r--   0 steve     (1000) steve     (1000)        0 2022-07-06 14:29:50.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/management/commands/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)      370 2022-08-31 14:29:46.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/management/commands/clearWebSocketSessions.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)      612 2022-09-13 14:31:41.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/management/commands/createApiGateway.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)      668 2022-07-06 14:56:50.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/management/commands/createCustomDomain.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-12 16:39:27.257401 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/migrations/
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2767 2022-01-17 22:00:46.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/migrations/0001_initial.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)      387 2022-01-17 23:02:23.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/migrations/0002_rename_author_websocketsession_user.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     7108 2022-07-08 11:09:17.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/migrations/0003_auto_20220706_1018.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1765 2022-12-08 18:57:06.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/migrations/0004_auto_20221208_1227.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)      451 2022-12-08 19:37:34.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/migrations/0005_apigatewayadditionalroute_deployed.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)        0 2022-01-17 20:53:32.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/migrations/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    15285 2022-12-08 19:34:30.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/models.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    11521 2022-12-12 16:37:29.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/views.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-12-12 16:39:27.253401 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets.egg-info/
+-rw-rw-r--   0 steve     (1000) steve     (1000)    28432 2022-12-12 16:39:27.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets.egg-info/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1409 2022-12-12 16:39:27.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets.egg-info/SOURCES.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)        1 2022-12-12 16:39:27.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets.egg-info/dependency_links.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)        1 2021-10-19 16:43:32.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets.egg-info/not-zip-safe
+-rw-rw-r--   0 steve     (1000) steve     (1000)       14 2022-12-12 16:39:27.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets.egg-info/requires.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       34 2022-12-12 16:39:27.000000 django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets.egg-info/top_level.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)      852 2022-12-12 16:38:54.000000 django-aws-api-gateway-websockets-1.0.9/pyproject.toml
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1882 2022-12-12 16:39:27.257401 django-aws-api-gateway-websockets-1.0.9/setup.cfg
+-rw-rw-r--   0 steve     (1000) steve     (1000)       38 2021-10-18 22:44:01.000000 django-aws-api-gateway-websockets-1.0.9/setup.py
```

### Comparing `django-aws-api-gateway-websockets-1.0.8/LICENSE` & `django-aws-api-gateway-websockets-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-aws-api-gateway-websockets-1.0.8/PKG-INFO` & `django-aws-api-gateway-websockets-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-aws-api-gateway-websockets
-Version: 1.0.8
+Version: 1.0.9
 Summary: Created to allow Django projects to be used as a HTTP backend for AWS API Gateway websockets
 Home-page: https://github.com/StevenMapes/django-aws-api-gateway-websockets
 Author: Steven Mapes
 Author-email: Steven Mapes <steve@stevenmapes.com>
 License: MIT
 Project-URL: Homepage, https://github.com/StevenMapes/django-aws-api-gateway-websockets
 Project-URL: Change log, https://github.com/StevenMapes/django-aws-api-gateway-websockets/blob/main/CHANGELOG.md
```

### Comparing `django-aws-api-gateway-websockets-1.0.8/README.md` & `django-aws-api-gateway-websockets-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/admin.py` & `django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/admin.py`

 * *Files identical despite different names*

### Comparing `django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/management/commands/createApiGateway.py` & `django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/management/commands/createApiGateway.py`

 * *Files identical despite different names*

### Comparing `django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/management/commands/createCustomDomain.py` & `django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/management/commands/createCustomDomain.py`

 * *Files identical despite different names*

### Comparing `django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/migrations/0001_initial.py` & `django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/migrations/0003_auto_20220706_1018.py` & `django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/migrations/0003_auto_20220706_1018.py`

 * *Files identical despite different names*

### Comparing `django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/migrations/0004_auto_20221208_1227.py` & `django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/migrations/0004_auto_20221208_1227.py`

 * *Files identical despite different names*

### Comparing `django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/models.py` & `django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/models.py`

 * *Files identical despite different names*

### Comparing `django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets/views.py` & `django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,17 +201,17 @@
         Checks for the expected headers.
         Tries to dispatch to the right method; if a method doesn't exist defer to the default handler.
         If the Route Selection Key is missing defer to the route selection error handler.
         If the request method isn't on the approved list then defer to the normal error handler .
         """
         if self._expected_headers(request) and self._allowed_apigateway(request):
             if request.method.lower() in self.http_method_names:
-                if "connect" == self.kwargs["route"]:
+                if "connect" == self.kwargs.get("route"):
                     handler = self.connect
-                elif "disconnect" == self.kwargs["route"]:
+                elif "disconnect" == self.kwargs.get("route"):
                     if not self._expected_useragent(request, *args, **kwargs):
                         handler = self.invalid_useragent
                     else:
                         handler = self.disconnect
                         self._add_user_to_request(request)
                 elif self.route_selection_key in self.body:
                     self._load_session(request)
```

### Comparing `django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets.egg-info/PKG-INFO` & `django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-aws-api-gateway-websockets
-Version: 1.0.8
+Version: 1.0.9
 Summary: Created to allow Django projects to be used as a HTTP backend for AWS API Gateway websockets
 Home-page: https://github.com/StevenMapes/django-aws-api-gateway-websockets
 Author: Steven Mapes
 Author-email: Steven Mapes <steve@stevenmapes.com>
 License: MIT
 Project-URL: Homepage, https://github.com/StevenMapes/django-aws-api-gateway-websockets
 Project-URL: Change log, https://github.com/StevenMapes/django-aws-api-gateway-websockets/blob/main/CHANGELOG.md
```

### Comparing `django-aws-api-gateway-websockets-1.0.8/django_aws_api_gateway_websockets.egg-info/SOURCES.txt` & `django-aws-api-gateway-websockets-1.0.9/django_aws_api_gateway_websockets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-aws-api-gateway-websockets-1.0.8/pyproject.toml` & `django-aws-api-gateway-websockets-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.isort]
 skip = [
 ".gitignore", ".dockerignore"
 ]
 
 [project]
 name = "django-aws-api-gateway-websockets"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Steven Mapes", email="steve@stevenmapes.com" },
 ]
 description = "Created to allow Django projects to be used as a HTTP backend for AWS API Gateway websockets"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `django-aws-api-gateway-websockets-1.0.8/setup.cfg` & `django-aws-api-gateway-websockets-1.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-aws-api-gateway-websockets
-version = 1.0.8
+version = 1.0.9
 description = Created to allow Django projects to be used as a HTTP backend for AWS API Gateway websockets
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Steven Mapes
 author_email = steve@stevenmapes.com
 url = https://github.com/StevenMapes/django-aws-api-gateway-websockets
 project_urls =
```

