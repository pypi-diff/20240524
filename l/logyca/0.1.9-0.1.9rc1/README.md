# Comparing `tmp/logyca-0.1.9.tar.gz` & `tmp/logyca-0.1.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logyca-0.1.9.tar", last modified: Tue May 21 20:55:52 2024, max compression
+gzip compressed data, was "logyca-0.1.9rc1.tar", last modified: Tue May 21 19:54:14 2024, max compression
```

## Comparing `logyca-0.1.9.tar` & `logyca-0.1.9rc1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.792940 logyca-0.1.9/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca-0.1.9/LICENSE.txt
--rw-rw-rw-   0        0        0    12566 2024-05-21 20:55:52.791939 logyca-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     9559 2024-05-21 20:06:52.000000 logyca-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.720363 logyca-0.1.9/logyca/
--rw-rw-rw-   0        0        0     1727 2024-04-26 23:10:10.000000 logyca-0.1.9/logyca/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.735924 logyca-0.1.9/logyca/dependencies/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/dependencies/__init__.py
--rw-rw-rw-   0        0        0     1380 2024-04-29 13:53:22.000000 logyca-0.1.9/logyca/dependencies/api_key_simple_auth.py
--rw-rw-rw-   0        0        0     3728 2024-04-29 13:53:26.000000 logyca-0.1.9/logyca/dependencies/oauth_token.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.737943 logyca-0.1.9/logyca/schemas/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/schemas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.745938 logyca-0.1.9/logyca/schemas/input/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/schemas/input/__init__.py
--rw-rw-rw-   0        0        0      288 2024-04-23 21:48:51.000000 logyca-0.1.9/logyca/schemas/input/api_key.py
--rw-rw-rw-   0        0        0      279 2024-04-24 01:52:56.000000 logyca-0.1.9/logyca/schemas/input/claimsdto.py
--rw-rw-rw-   0        0        0      111 2024-04-24 01:42:50.000000 logyca-0.1.9/logyca/schemas/input/jwt.py
--rw-rw-rw-   0        0        0      553 2024-04-24 00:49:40.000000 logyca-0.1.9/logyca/schemas/input/oauth_token.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.758938 logyca-0.1.9/logyca/schemas/output/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/schemas/output/__init__.py
--rw-rw-rw-   0        0        0      954 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/schemas/output/apIresultdto.py
--rw-rw-rw-   0        0        0      896 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/schemas/output/apifilterexceptiondto.py
--rw-rw-rw-   0        0        0      628 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/schemas/output/healthdto.py
--rw-rw-rw-   0        0        0      138 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/schemas/output/httpexceptiondto.py
--rw-rw-rw-   0        0        0      472 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/schemas/output/tokensdto.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.760938 logyca-0.1.9/logyca/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.767938 logyca-0.1.9/logyca/utils/constants/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/utils/constants/__init__.py
--rw-rw-rw-   0        0        0      128 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/utils/constants/app.py
--rw-rw-rw-   0        0        0      724 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/utils/constants/healthenum.py
--rw-rw-rw-   0        0        0     7697 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/utils/constants/logycastatusenum.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.773936 logyca-0.1.9/logyca/utils/handlers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/utils/handlers/__init__.py
--rw-rw-rw-   0        0        0     4689 2024-04-23 15:28:59.000000 logyca-0.1.9/logyca/utils/handlers/exception_handlers.py
--rw-rw-rw-   0        0        0     2436 2024-04-23 15:22:15.000000 logyca-0.1.9/logyca/utils/handlers/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.779940 logyca-0.1.9/logyca/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9/logyca/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0      531 2024-04-26 17:40:26.000000 logyca-0.1.9/logyca/utils/helpers/datetimehelpers.py
--rw-rw-rw-   0        0        0      634 2024-04-24 02:55:02.000000 logyca-0.1.9/logyca/utils/helpers/stringshelpers.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.787941 logyca-0.1.9/logyca.egg-info/
--rw-rw-rw-   0        0        0    12566 2024-05-21 20:55:52.000000 logyca-0.1.9/logyca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1204 2024-05-21 20:55:52.000000 logyca-0.1.9/logyca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 20:55:52.000000 logyca-0.1.9/logyca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      335 2024-05-21 20:55:52.000000 logyca-0.1.9/logyca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 20:55:52.000000 logyca-0.1.9/logyca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 20:55:52.793940 logyca-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     2478 2024-05-21 20:54:44.000000 logyca-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:55:52.785941 logyca-0.1.9/tests/
--rw-rw-rw-   0        0        0     2324 2024-04-23 14:32:08.000000 logyca-0.1.9/tests/test_data_schemes.py
--rw-rw-rw-   0        0        0      221 2024-04-26 17:45:47.000000 logyca-0.1.9/tests/test_functions.py
--rw-rw-rw-   0        0        0      226 2024-04-23 14:32:08.000000 logyca-0.1.9/tests/test_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.722838 logyca-0.1.9rc1/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0    12569 2024-05-21 19:54:14.721836 logyca-0.1.9rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     9559 2024-05-21 19:42:54.000000 logyca-0.1.9rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.653241 logyca-0.1.9rc1/logyca/
+-rw-rw-rw-   0        0        0     1727 2024-04-26 23:10:10.000000 logyca-0.1.9rc1/logyca/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.667597 logyca-0.1.9rc1/logyca/dependencies/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/dependencies/__init__.py
+-rw-rw-rw-   0        0        0     1380 2024-04-29 13:53:22.000000 logyca-0.1.9rc1/logyca/dependencies/api_key_simple_auth.py
+-rw-rw-rw-   0        0        0     3728 2024-04-29 13:53:26.000000 logyca-0.1.9rc1/logyca/dependencies/oauth_token.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.668597 logyca-0.1.9rc1/logyca/schemas/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.678270 logyca-0.1.9rc1/logyca/schemas/input/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/input/__init__.py
+-rw-rw-rw-   0        0        0      288 2024-04-23 21:48:51.000000 logyca-0.1.9rc1/logyca/schemas/input/api_key.py
+-rw-rw-rw-   0        0        0      279 2024-04-24 01:52:56.000000 logyca-0.1.9rc1/logyca/schemas/input/claimsdto.py
+-rw-rw-rw-   0        0        0      111 2024-04-24 01:42:50.000000 logyca-0.1.9rc1/logyca/schemas/input/jwt.py
+-rw-rw-rw-   0        0        0      553 2024-04-24 00:49:40.000000 logyca-0.1.9rc1/logyca/schemas/input/oauth_token.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.688834 logyca-0.1.9rc1/logyca/schemas/output/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/apIresultdto.py
+-rw-rw-rw-   0        0        0      896 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/apifilterexceptiondto.py
+-rw-rw-rw-   0        0        0      628 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/healthdto.py
+-rw-rw-rw-   0        0        0      138 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/httpexceptiondto.py
+-rw-rw-rw-   0        0        0      472 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/tokensdto.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.690837 logyca-0.1.9rc1/logyca/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.697836 logyca-0.1.9rc1/logyca/utils/constants/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/constants/__init__.py
+-rw-rw-rw-   0        0        0      128 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/constants/app.py
+-rw-rw-rw-   0        0        0      724 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/constants/healthenum.py
+-rw-rw-rw-   0        0        0     7697 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/constants/logycastatusenum.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.702837 logyca-0.1.9rc1/logyca/utils/handlers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/handlers/__init__.py
+-rw-rw-rw-   0        0        0     4689 2024-04-23 15:28:59.000000 logyca-0.1.9rc1/logyca/utils/handlers/exception_handlers.py
+-rw-rw-rw-   0        0        0     2436 2024-04-23 15:22:15.000000 logyca-0.1.9rc1/logyca/utils/handlers/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.707839 logyca-0.1.9rc1/logyca/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0      531 2024-04-26 17:40:26.000000 logyca-0.1.9rc1/logyca/utils/helpers/datetimehelpers.py
+-rw-rw-rw-   0        0        0      634 2024-04-24 02:55:02.000000 logyca-0.1.9rc1/logyca/utils/helpers/stringshelpers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.716837 logyca-0.1.9rc1/logyca.egg-info/
+-rw-rw-rw-   0        0        0    12569 2024-05-21 19:54:14.000000 logyca-0.1.9rc1/logyca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1204 2024-05-21 19:54:14.000000 logyca-0.1.9rc1/logyca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 19:54:14.000000 logyca-0.1.9rc1/logyca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      335 2024-05-21 19:54:14.000000 logyca-0.1.9rc1/logyca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 19:54:14.000000 logyca-0.1.9rc1/logyca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 19:54:14.724836 logyca-0.1.9rc1/setup.cfg
+-rw-rw-rw-   0        0        0     2481 2024-05-21 19:50:21.000000 logyca-0.1.9rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.713837 logyca-0.1.9rc1/tests/
+-rw-rw-rw-   0        0        0     2324 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/tests/test_data_schemes.py
+-rw-rw-rw-   0        0        0      221 2024-04-26 17:45:47.000000 logyca-0.1.9rc1/tests/test_functions.py
+-rw-rw-rw-   0        0        0      226 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/tests/test_helpers.py
```

### Comparing `logyca-0.1.9/LICENSE.txt` & `logyca-0.1.9rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/PKG-INFO` & `logyca-0.1.9rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca
-Version: 0.1.9
+Version: 0.1.9rc1
 Summary: This package name is reserved by LOGYCA company
 Home-page: https://github.com/logyca/<soon>
 Author: Jaime Andres Cardona Carrillo
 Author-email: tecnologiaeinformacion@logyca.com
 License: MIT License
 Keywords: api result,result dto,result scheme
 Classifier: Development Status :: 4 - Beta
@@ -332,15 +332,15 @@
 - Added for new features.
 - Changed for changes in existing functionality.
 - Deprecated for soon-to-be removed features.
 - Removed for now removed features.
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
-## [0.1.9] - 2024-05-21
+## [0.1.9] - 2023-10-03
 ### Added
 - New logger functionality.
 - new authentication functionality in fastapi by dependency injection with api-key, to be used on endpoints.
 - new authentication functionality in fastapi by dependency injection with oauth (single sign on), to be used on endpoints.
 - In the samples folder of this library, there are complete working examples of using the code.
 
 ## [0.1.8] - 2023-10-03
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: logyca Version: 0.1.9 Summary: This package name is
-reserved by LOGYCA company Home-page: https://github.com/logyca/ Author: Jaime
-Andres Cardona Carrillo Author-email: tecnologiaeinformacion@logyca.com
+Metadata-Version: 2.1 Name: logyca Version: 0.1.9rc1 Summary: This package name
+is reserved by LOGYCA company Home-page: https://github.com/logyca/ Author:
+Jaime Andres Cardona Carrillo Author-email: tecnologiaeinformacion@logyca.com
 License: MIT License Keywords: api result,result dto,result scheme Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: Pydantic :: 1 Classifier: Framework :: Pydantic
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 :: Only
@@ -128,15 +128,15 @@
 m pip install logyca[test] # Linux pip install logyca # Run it pytest -s ``` --
 - # Changelog All notable changes to this project will be documented in this
 file. The format is based on [Keep a Changelog](https://keepachangelog.com/en/
 1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/
 spec/v2.0.0.html). ## Types of changes - Added for new features. - Changed for
 changes in existing functionality. - Deprecated for soon-to-be removed
 features. - Removed for now removed features. - Fixed for any bug fixes. -
-Security in case of vulnerabilities. ## [0.1.9] - 2024-05-21 ### Added - New
+Security in case of vulnerabilities. ## [0.1.9] - 2023-10-03 ### Added - New
 logger functionality. - new authentication functionality in fastapi by
 dependency injection with api-key, to be used on endpoints. - new
 authentication functionality in fastapi by dependency injection with oauth
 (single sign on), to be used on endpoints. - In the samples folder of this
 library, there are complete working examples of using the code. ## [0.1.8] -
 2023-10-03 ### Fixed - Due to a link error in the readme to internal documents
 in pypi, we chose to leave the changelog at the end of the readme. ## [0.1.7] -
```

### Comparing `logyca-0.1.9/README.md` & `logyca-0.1.9rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,15 @@
 - Added for new features.
 - Changed for changes in existing functionality.
 - Deprecated for soon-to-be removed features.
 - Removed for now removed features.
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
-## [0.1.9] - 2024-05-21
+## [0.1.9] - 2023-10-03
 ### Added
 - New logger functionality.
 - new authentication functionality in fastapi by dependency injection with api-key, to be used on endpoints.
 - new authentication functionality in fastapi by dependency injection with oauth (single sign on), to be used on endpoints.
 - In the samples folder of this library, there are complete working examples of using the code.
 
 ## [0.1.8] - 2023-10-03
```

#### html2text {}

```diff
@@ -89,15 +89,15 @@
 m pip install logyca[test] # Linux pip install logyca # Run it pytest -s ``` --
 - # Changelog All notable changes to this project will be documented in this
 file. The format is based on [Keep a Changelog](https://keepachangelog.com/en/
 1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/
 spec/v2.0.0.html). ## Types of changes - Added for new features. - Changed for
 changes in existing functionality. - Deprecated for soon-to-be removed
 features. - Removed for now removed features. - Fixed for any bug fixes. -
-Security in case of vulnerabilities. ## [0.1.9] - 2024-05-21 ### Added - New
+Security in case of vulnerabilities. ## [0.1.9] - 2023-10-03 ### Added - New
 logger functionality. - new authentication functionality in fastapi by
 dependency injection with api-key, to be used on endpoints. - new
 authentication functionality in fastapi by dependency injection with oauth
 (single sign on), to be used on endpoints. - In the samples folder of this
 library, there are complete working examples of using the code. ## [0.1.8] -
 2023-10-03 ### Fixed - Due to a link error in the readme to internal documents
 in pypi, we chose to leave the changelog at the end of the readme. ## [0.1.7] -
```

### Comparing `logyca-0.1.9/logyca/__init__.py` & `logyca-0.1.9rc1/logyca/__init__.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/dependencies/api_key_simple_auth.py` & `logyca-0.1.9rc1/logyca/dependencies/api_key_simple_auth.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/dependencies/oauth_token.py` & `logyca-0.1.9rc1/logyca/dependencies/oauth_token.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/schemas/input/oauth_token.py` & `logyca-0.1.9rc1/logyca/schemas/input/oauth_token.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/schemas/output/apIresultdto.py` & `logyca-0.1.9rc1/logyca/schemas/output/apIresultdto.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/schemas/output/apifilterexceptiondto.py` & `logyca-0.1.9rc1/logyca/schemas/output/apifilterexceptiondto.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/schemas/output/healthdto.py` & `logyca-0.1.9rc1/logyca/schemas/output/healthdto.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/utils/constants/healthenum.py` & `logyca-0.1.9rc1/logyca/utils/constants/healthenum.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/utils/constants/logycastatusenum.py` & `logyca-0.1.9rc1/logyca/utils/constants/logycastatusenum.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/utils/handlers/exception_handlers.py` & `logyca-0.1.9rc1/logyca/utils/handlers/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/utils/handlers/logger.py` & `logyca-0.1.9rc1/logyca/utils/handlers/logger.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/utils/helpers/datetimehelpers.py` & `logyca-0.1.9rc1/logyca/utils/helpers/datetimehelpers.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca/utils/helpers/stringshelpers.py` & `logyca-0.1.9rc1/logyca/utils/helpers/stringshelpers.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/logyca.egg-info/PKG-INFO` & `logyca-0.1.9rc1/logyca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logyca
-Version: 0.1.9
+Version: 0.1.9rc1
 Summary: This package name is reserved by LOGYCA company
 Home-page: https://github.com/logyca/<soon>
 Author: Jaime Andres Cardona Carrillo
 Author-email: tecnologiaeinformacion@logyca.com
 License: MIT License
 Keywords: api result,result dto,result scheme
 Classifier: Development Status :: 4 - Beta
@@ -332,15 +332,15 @@
 - Added for new features.
 - Changed for changes in existing functionality.
 - Deprecated for soon-to-be removed features.
 - Removed for now removed features.
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
-## [0.1.9] - 2024-05-21
+## [0.1.9] - 2023-10-03
 ### Added
 - New logger functionality.
 - new authentication functionality in fastapi by dependency injection with api-key, to be used on endpoints.
 - new authentication functionality in fastapi by dependency injection with oauth (single sign on), to be used on endpoints.
 - In the samples folder of this library, there are complete working examples of using the code.
 
 ## [0.1.8] - 2023-10-03
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: logyca Version: 0.1.9 Summary: This package name is
-reserved by LOGYCA company Home-page: https://github.com/logyca/ Author: Jaime
-Andres Cardona Carrillo Author-email: tecnologiaeinformacion@logyca.com
+Metadata-Version: 2.1 Name: logyca Version: 0.1.9rc1 Summary: This package name
+is reserved by LOGYCA company Home-page: https://github.com/logyca/ Author:
+Jaime Andres Cardona Carrillo Author-email: tecnologiaeinformacion@logyca.com
 License: MIT License Keywords: api result,result dto,result scheme Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: Pydantic :: 1 Classifier: Framework :: Pydantic
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 :: Only
@@ -128,15 +128,15 @@
 m pip install logyca[test] # Linux pip install logyca # Run it pytest -s ``` --
 - # Changelog All notable changes to this project will be documented in this
 file. The format is based on [Keep a Changelog](https://keepachangelog.com/en/
 1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/
 spec/v2.0.0.html). ## Types of changes - Added for new features. - Changed for
 changes in existing functionality. - Deprecated for soon-to-be removed
 features. - Removed for now removed features. - Fixed for any bug fixes. -
-Security in case of vulnerabilities. ## [0.1.9] - 2024-05-21 ### Added - New
+Security in case of vulnerabilities. ## [0.1.9] - 2023-10-03 ### Added - New
 logger functionality. - new authentication functionality in fastapi by
 dependency injection with api-key, to be used on endpoints. - new
 authentication functionality in fastapi by dependency injection with oauth
 (single sign on), to be used on endpoints. - In the samples folder of this
 library, there are complete working examples of using the code. ## [0.1.8] -
 2023-10-03 ### Fixed - Due to a link error in the readme to internal documents
 in pypi, we chose to leave the changelog at the end of the readme. ## [0.1.7] -
```

### Comparing `logyca-0.1.9/logyca.egg-info/SOURCES.txt` & `logyca-0.1.9rc1/logyca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logyca-0.1.9/setup.py` & `logyca-0.1.9rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="LOGYCA"
 PACKAGE_NAME = "logyca"
-VERSION = "0.1.9"
+VERSION = "0.1.9rc1"
 
 install_requires = ["pydantic >=1.8","pytz >=2023.3"]
 install_requires_fastapi = ["fastapi>=0.96.0","starlette>=0.24.0"]
 install_requires_oauth_token = install_requires_fastapi + ["aiohttp>=3.8.5","jwt>=1.1.0"]
 install_requires_api_key_simple_auth = install_requires_fastapi
 
 extras_require = {
```

### Comparing `logyca-0.1.9/tests/test_data_schemes.py` & `logyca-0.1.9rc1/tests/test_data_schemes.py`

 * *Files identical despite different names*

