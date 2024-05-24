# Comparing `tmp/appwrite-5.0.1.tar.gz` & `tmp/appwrite-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appwrite-5.0.1.tar", last modified: Sat Mar  9 15:44:39 2024, max compression
+gzip compressed data, was "appwrite-5.0.2.tar", last modified: Sun Mar 24 12:21:42 2024, max compression
```

## Comparing `appwrite-5.0.1.tar` & `appwrite-5.0.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-09 15:44:39.137111 appwrite-5.0.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2024-03-09 15:43:47.000000 appwrite-5.0.1/LICENSE
--rw-r--r--   0 travis    (2000) travis    (2000)     5506 2024-03-09 15:44:39.137111 appwrite-5.0.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4469 2024-03-09 15:43:47.000000 appwrite-5.0.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-09 15:44:39.129111 appwrite-5.0.1/appwrite/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7659 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-09 15:44:39.129111 appwrite-5.0.1/appwrite/encoders/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/encoders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2185 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/encoders/value_class_encoder.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-09 15:44:39.133111 appwrite-5.0.1/appwrite/enums/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      149 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/authentication_factor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       72 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/authenticator_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      394 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/browser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/compression.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/credit_card.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      168 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/execution_method.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4116 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/flag.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/image_format.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      267 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/image_gravity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/index_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/messaging_provider_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      449 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      962 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/o_auth_provider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      319 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/password_hash.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/relation_mutate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/relationship_type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/runtime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/enums/smtp_encryption.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      261 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      128 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/id.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      586 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/input_file.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      392 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/permission.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2938 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/query.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/role.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-09 15:44:39.137111 appwrite-5.0.1/appwrite/services/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19777 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3810 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/avatars.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40875 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/databases.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15943 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1036 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/graphql.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7239 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/health.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2238 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/locale.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34936 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/messaging.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9895 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/storage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8030 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/teams.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25898 2024-03-09 15:43:47.000000 appwrite-5.0.1/appwrite/services/users.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-09 15:44:39.137111 appwrite-5.0.1/appwrite.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     5506 2024-03-09 15:44:39.000000 appwrite-5.0.1/appwrite.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1394 2024-03-09 15:44:39.000000 appwrite-5.0.1/appwrite.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-09 15:44:39.000000 appwrite-5.0.1/appwrite.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2024-03-09 15:44:39.000000 appwrite-5.0.1/appwrite.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-03-09 15:44:39.000000 appwrite-5.0.1/appwrite.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2024-03-09 15:44:39.137111 appwrite-5.0.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1374 2024-03-09 15:43:47.000000 appwrite-5.0.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-24 12:21:42.712020 appwrite-5.0.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1540 2024-03-24 12:20:51.000000 appwrite-5.0.2/LICENSE
+-rw-r--r--   0 travis    (2000) travis    (2000)     5506 2024-03-24 12:21:42.712020 appwrite-5.0.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4469 2024-03-24 12:20:51.000000 appwrite-5.0.2/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-24 12:21:42.704019 appwrite-5.0.2/appwrite/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7659 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-24 12:21:42.704019 appwrite-5.0.2/appwrite/encoders/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/encoders/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2185 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/encoders/value_class_encoder.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-24 12:21:42.708020 appwrite-5.0.2/appwrite/enums/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      149 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/authentication_factor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       72 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/authenticator_type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      394 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/browser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/compression.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      458 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/credit_card.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      168 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/execution_method.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4116 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/flag.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      132 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/image_format.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      267 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/image_gravity.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      110 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/index_type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      112 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/messaging_provider_type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      449 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      962 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/o_auth_provider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      319 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/password_hash.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/relation_mutate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/relationship_type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1256 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/runtime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      101 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/enums/smtp_encryption.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      261 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      759 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/id.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      586 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/input_file.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      392 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/permission.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2938 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/query.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2390 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/role.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/service.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-24 12:21:42.708020 appwrite-5.0.2/appwrite/services/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19777 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3810 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/avatars.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40875 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/databases.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15943 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1036 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/graphql.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7239 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/health.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2238 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/locale.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34972 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/messaging.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9895 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/storage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8030 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/teams.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25898 2024-03-24 12:20:51.000000 appwrite-5.0.2/appwrite/services/users.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-24 12:21:42.712020 appwrite-5.0.2/appwrite.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     5506 2024-03-24 12:21:42.000000 appwrite-5.0.2/appwrite.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1394 2024-03-24 12:21:42.000000 appwrite-5.0.2/appwrite.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-24 12:21:42.000000 appwrite-5.0.2/appwrite.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2024-03-24 12:21:42.000000 appwrite-5.0.2/appwrite.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       60 2024-03-24 12:21:42.000000 appwrite-5.0.2/appwrite.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2024-03-24 12:21:42.712020 appwrite-5.0.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1374 2024-03-24 12:20:51.000000 appwrite-5.0.2/setup.py
```

### Comparing `appwrite-5.0.1/LICENSE` & `appwrite-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/PKG-INFO` & `appwrite-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: appwrite
-Version: 5.0.1
+Version: 5.0.2
 Summary: Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API
 Home-page: https://appwrite.io/support
-Download-URL: https://github.com/appwrite/sdk-for-python/archive/5.0.1.tar.gz
+Download-URL: https://github.com/appwrite/sdk-for-python/archive/5.0.2.tar.gz
 Author: Appwrite Team
 Author-email: team@appwrite.io
 Maintainer: Appwrite Team
 Maintainer-email: team@appwrite.io
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Appwrite Python SDK
 
 ![License](https://img.shields.io/github/license/appwrite/sdk-for-python.svg?style=flat-square)
-![Version](https://img.shields.io/badge/api%20version-1.5.0-blue.svg?style=flat-square)
+![Version](https://img.shields.io/badge/api%20version-1.5.4-blue.svg?style=flat-square)
 [![Build Status](https://img.shields.io/travis/com/appwrite/sdk-generator?style=flat-square)](https://travis-ci.com/appwrite/sdk-generator)
 [![Twitter Account](https://img.shields.io/twitter/follow/appwrite?color=00acee&label=twitter&style=flat-square)](https://twitter.com/appwrite)
 [![Discord](https://img.shields.io/discord/564160730845151244?label=discord&style=flat-square)](https://appwrite.io/discord)
 
 **This SDK is compatible with Appwrite server version 1.5.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
 
 Appwrite is an open-source backend as a service server that abstract and simplify complex and repetitive development tasks behind a very simple to use REST API. Appwrite aims to help you develop your apps faster and in a more secure way. Use the Python SDK to integrate your app with the Appwrite server to easily start interacting with all of Appwrite backend APIs and tools. For full API documentation and tutorials go to [https://appwrite.io/docs](https://appwrite.io/docs)
```

### Comparing `appwrite-5.0.1/README.md` & `appwrite-5.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Appwrite Python SDK
 
 ![License](https://img.shields.io/github/license/appwrite/sdk-for-python.svg?style=flat-square)
-![Version](https://img.shields.io/badge/api%20version-1.5.0-blue.svg?style=flat-square)
+![Version](https://img.shields.io/badge/api%20version-1.5.4-blue.svg?style=flat-square)
 [![Build Status](https://img.shields.io/travis/com/appwrite/sdk-generator?style=flat-square)](https://travis-ci.com/appwrite/sdk-generator)
 [![Twitter Account](https://img.shields.io/twitter/follow/appwrite?color=00acee&label=twitter&style=flat-square)](https://twitter.com/appwrite)
 [![Discord](https://img.shields.io/discord/564160730845151244?label=discord&style=flat-square)](https://appwrite.io/discord)
 
 **This SDK is compatible with Appwrite server version 1.5.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
 
 Appwrite is an open-source backend as a service server that abstract and simplify complex and repetitive development tasks behind a very simple to use REST API. Appwrite aims to help you develop your apps faster and in a more secure way. Use the Python SDK to integrate your app with the Appwrite server to easily start interacting with all of Appwrite backend APIs and tools. For full API documentation and tutorials go to [https://appwrite.io/docs](https://appwrite.io/docs)
```

### Comparing `appwrite-5.0.1/appwrite/client.py` & `appwrite-5.0.2/appwrite/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 class Client:
     def __init__(self):
         self._chunk_size = 5*1024*1024
         self._self_signed = False
         self._endpoint = 'https://cloud.appwrite.io/v1'
         self._global_headers = {
             'content-type': '',
-            'user-agent' : 'AppwritePythonSDK/5.0.1 (${os.uname().sysname}; ${os.uname().version}; ${os.uname().machine})',
+            'user-agent' : 'AppwritePythonSDK/5.0.2 (${os.uname().sysname}; ${os.uname().version}; ${os.uname().machine})',
             'x-sdk-name': 'Python',
             'x-sdk-platform': 'server',
             'x-sdk-language': 'python',
-            'x-sdk-version': '5.0.1',
+            'x-sdk-version': '5.0.2',
             'X-Appwrite-Response-Format' : '1.5.0',
         }
 
     def set_self_signed(self, status=True):
         self._self_signed = status
         return self
```

### Comparing `appwrite-5.0.1/appwrite/encoders/value_class_encoder.py` & `appwrite-5.0.2/appwrite/encoders/value_class_encoder.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/enums/flag.py` & `appwrite-5.0.2/appwrite/enums/flag.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/enums/o_auth_provider.py` & `appwrite-5.0.2/appwrite/enums/o_auth_provider.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/enums/runtime.py` & `appwrite-5.0.2/appwrite/enums/runtime.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/input_file.py` & `appwrite-5.0.2/appwrite/input_file.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/query.py` & `appwrite-5.0.2/appwrite/query.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/role.py` & `appwrite-5.0.2/appwrite/role.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/services/account.py` & `appwrite-5.0.2/appwrite/services/account.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/services/avatars.py` & `appwrite-5.0.2/appwrite/services/avatars.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/services/databases.py` & `appwrite-5.0.2/appwrite/services/databases.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/services/functions.py` & `appwrite-5.0.2/appwrite/services/functions.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/services/graphql.py` & `appwrite-5.0.2/appwrite/services/graphql.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/services/health.py` & `appwrite-5.0.2/appwrite/services/health.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/services/locale.py` & `appwrite-5.0.2/appwrite/services/locale.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/services/messaging.py` & `appwrite-5.0.2/appwrite/services/messaging.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,54 +413,54 @@
         api_params['replyToName'] = reply_to_name
         api_params['replyToEmail'] = reply_to_email
 
         return self.client.call('patch', api_path, {
             'content-type': 'application/json',
         }, api_params)
 
-    def create_msg91_provider(self, provider_id, name, xfrom = None, sender_id = None, auth_key = None, enabled = None):
+    def create_msg91_provider(self, provider_id, name, template_id = None, sender_id = None, auth_key = None, enabled = None):
         """Create Msg91 provider"""
 
         
         api_path = '/messaging/providers/msg91'
         api_params = {}
         if provider_id is None:
             raise AppwriteException('Missing required parameter: "provider_id"')
 
         if name is None:
             raise AppwriteException('Missing required parameter: "name"')
 
 
         api_params['providerId'] = provider_id
         api_params['name'] = name
-        api_params['from'] = xfrom
+        api_params['templateId'] = template_id
         api_params['senderId'] = sender_id
         api_params['authKey'] = auth_key
         api_params['enabled'] = enabled
 
         return self.client.call('post', api_path, {
             'content-type': 'application/json',
         }, api_params)
 
-    def update_msg91_provider(self, provider_id, name = None, enabled = None, sender_id = None, auth_key = None, xfrom = None):
+    def update_msg91_provider(self, provider_id, name = None, enabled = None, template_id = None, sender_id = None, auth_key = None):
         """Update Msg91 provider"""
 
         
         api_path = '/messaging/providers/msg91/{providerId}'
         api_params = {}
         if provider_id is None:
             raise AppwriteException('Missing required parameter: "provider_id"')
 
         api_path = api_path.replace('{providerId}', provider_id)
 
         api_params['name'] = name
         api_params['enabled'] = enabled
+        api_params['templateId'] = template_id
         api_params['senderId'] = sender_id
         api_params['authKey'] = auth_key
-        api_params['from'] = xfrom
 
         return self.client.call('patch', api_path, {
             'content-type': 'application/json',
         }, api_params)
 
     def create_sendgrid_provider(self, provider_id, name, api_key = None, from_name = None, from_email = None, reply_to_name = None, reply_to_email = None, enabled = None):
         """Create Sendgrid provider"""
```

### Comparing `appwrite-5.0.1/appwrite/services/storage.py` & `appwrite-5.0.2/appwrite/services/storage.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/services/teams.py` & `appwrite-5.0.2/appwrite/services/teams.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite/services/users.py` & `appwrite-5.0.2/appwrite/services/users.py`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/appwrite.egg-info/PKG-INFO` & `appwrite-5.0.2/appwrite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: appwrite
-Version: 5.0.1
+Version: 5.0.2
 Summary: Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API
 Home-page: https://appwrite.io/support
-Download-URL: https://github.com/appwrite/sdk-for-python/archive/5.0.1.tar.gz
+Download-URL: https://github.com/appwrite/sdk-for-python/archive/5.0.2.tar.gz
 Author: Appwrite Team
 Author-email: team@appwrite.io
 Maintainer: Appwrite Team
 Maintainer-email: team@appwrite.io
 License: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Appwrite Python SDK
 
 ![License](https://img.shields.io/github/license/appwrite/sdk-for-python.svg?style=flat-square)
-![Version](https://img.shields.io/badge/api%20version-1.5.0-blue.svg?style=flat-square)
+![Version](https://img.shields.io/badge/api%20version-1.5.4-blue.svg?style=flat-square)
 [![Build Status](https://img.shields.io/travis/com/appwrite/sdk-generator?style=flat-square)](https://travis-ci.com/appwrite/sdk-generator)
 [![Twitter Account](https://img.shields.io/twitter/follow/appwrite?color=00acee&label=twitter&style=flat-square)](https://twitter.com/appwrite)
 [![Discord](https://img.shields.io/discord/564160730845151244?label=discord&style=flat-square)](https://appwrite.io/discord)
 
 **This SDK is compatible with Appwrite server version 1.5.x. For older versions, please check [previous releases](https://github.com/appwrite/sdk-for-python/releases).**
 
 Appwrite is an open-source backend as a service server that abstract and simplify complex and repetitive development tasks behind a very simple to use REST API. Appwrite aims to help you develop your apps faster and in a more secure way. Use the Python SDK to integrate your app with the Appwrite server to easily start interacting with all of Appwrite backend APIs and tools. For full API documentation and tutorials go to [https://appwrite.io/docs](https://appwrite.io/docs)
```

### Comparing `appwrite-5.0.1/appwrite.egg-info/SOURCES.txt` & `appwrite-5.0.2/appwrite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appwrite-5.0.1/setup.py` & `appwrite-5.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,25 +9,25 @@
   name = 'appwrite',
   packages = [
     'appwrite',
     'appwrite/services',
     'appwrite/encoders',
     'appwrite/enums',
   ],
-  version = '5.0.1',
+  version = '5.0.2',
   license='BSD-3-Clause',
   description = 'Appwrite is an open-source self-hosted backend server that abstract and simplify complex and repetitive development tasks behind a very simple REST API',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'Appwrite Team',
   author_email = 'team@appwrite.io',
   maintainer = 'Appwrite Team',
   maintainer_email = 'team@appwrite.io',
   url = 'https://appwrite.io/support',
-  download_url='https://github.com/appwrite/sdk-for-python/archive/5.0.1.tar.gz',
+  download_url='https://github.com/appwrite/sdk-for-python/archive/5.0.2.tar.gz',
   install_requires=[
     'requests',
   ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Environment :: Web Environment',
```

