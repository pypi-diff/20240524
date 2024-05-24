# Comparing `tmp/resend-1.1.0.tar.gz` & `tmp/resend-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resend-1.1.0.tar", last modified: Fri May 17 21:47:27 2024, max compression
+gzip compressed data, was "dist/resend-1.2.0.tar", last modified: Fri May 24 20:34:32 2024, max compression
```

## Comparing `resend-1.1.0.tar` & `resend-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.891757 resend-1.1.0/
--rw-r--r--   0 derich     (501) staff       (20)     1070 2023-08-19 17:45:00.000000 resend-1.1.0/LICENSE.md
--rw-r--r--   0 derich     (501) staff       (20)     2429 2024-05-17 21:47:27.891694 resend-1.1.0/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)     1626 2024-05-17 20:02:25.000000 resend-1.1.0/README.md
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.887871 resend-1.1.0/resend/
--rw-r--r--   0 derich     (501) staff       (20)     1003 2024-05-14 01:16:37.000000 resend-1.1.0/resend/__init__.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.889125 resend-1.1.0/resend/api_keys/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.1.0/resend/api_keys/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)      998 2024-05-09 01:36:14.000000 resend-1.1.0/resend/api_keys/_api_key.py
--rw-r--r--   0 derich     (501) staff       (20)     2310 2024-05-09 01:36:14.000000 resend-1.1.0/resend/api_keys/_api_keys.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.889551 resend-1.1.0/resend/audiences/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.1.0/resend/audiences/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     1192 2024-05-09 01:36:14.000000 resend-1.1.0/resend/audiences/_audience.py
--rw-r--r--   0 derich     (501) staff       (20)     2305 2024-05-09 01:36:14.000000 resend-1.1.0/resend/audiences/_audiences.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.889973 resend-1.1.0/resend/contacts/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.1.0/resend/contacts/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     1795 2024-05-09 01:36:14.000000 resend-1.1.0/resend/contacts/_contact.py
--rw-r--r--   0 derich     (501) staff       (20)     4400 2024-05-09 01:36:14.000000 resend-1.1.0/resend/contacts/_contacts.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.890562 resend-1.1.0/resend/domains/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.1.0/resend/domains/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     1987 2024-05-09 01:36:14.000000 resend-1.1.0/resend/domains/_domain.py
--rw-r--r--   0 derich     (501) staff       (20)     3887 2024-05-09 01:36:14.000000 resend-1.1.0/resend/domains/_domains.py
--rw-r--r--   0 derich     (501) staff       (20)     1416 2024-05-09 01:36:14.000000 resend-1.1.0/resend/domains/_record.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.891411 resend-1.1.0/resend/emails/
--rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.1.0/resend/emails/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)      489 2024-05-09 01:36:14.000000 resend-1.1.0/resend/emails/_attachment.py
--rw-r--r--   0 derich     (501) staff       (20)      962 2024-05-17 20:02:25.000000 resend-1.1.0/resend/emails/_batch.py
--rw-r--r--   0 derich     (501) staff       (20)     2862 2024-05-17 20:02:25.000000 resend-1.1.0/resend/emails/_email.py
--rw-r--r--   0 derich     (501) staff       (20)     2832 2024-05-17 20:02:25.000000 resend-1.1.0/resend/emails/_emails.py
--rw-r--r--   0 derich     (501) staff       (20)      524 2024-05-09 01:36:14.000000 resend-1.1.0/resend/emails/_tag.py
--rw-r--r--   0 derich     (501) staff       (20)     6108 2024-05-17 20:02:25.000000 resend-1.1.0/resend/exceptions.py
--rw-r--r--   0 derich     (501) staff       (20)        0 2023-08-19 17:45:00.000000 resend-1.1.0/resend/py.typed
--rw-r--r--   0 derich     (501) staff       (20)     2353 2024-05-17 20:02:25.000000 resend-1.1.0/resend/request.py
--rw-r--r--   0 derich     (501) staff       (20)      448 2024-05-17 20:02:25.000000 resend-1.1.0/resend/utils.py
--rw-r--r--   0 derich     (501) staff       (20)      133 2024-05-17 21:47:23.000000 resend-1.1.0/resend/version.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-17 21:47:27.888685 resend-1.1.0/resend.egg-info/
--rw-r--r--   0 derich     (501) staff       (20)     2429 2024-05-17 21:47:27.000000 resend-1.1.0/resend.egg-info/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)      841 2024-05-17 21:47:27.000000 resend-1.1.0/resend.egg-info/SOURCES.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-17 21:47:27.000000 resend-1.1.0/resend.egg-info/dependency_links.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-14 01:37:48.000000 resend-1.1.0/resend.egg-info/not-zip-safe
--rw-r--r--   0 derich     (501) staff       (20)       35 2024-05-17 21:47:27.000000 resend-1.1.0/resend.egg-info/requires.txt
--rw-r--r--   0 derich     (501) staff       (20)        7 2024-05-17 21:47:27.000000 resend-1.1.0/resend.egg-info/top_level.txt
--rw-r--r--   0 derich     (501) staff       (20)       67 2024-05-17 21:47:27.892583 resend-1.1.0/setup.cfg
--rw-r--r--   0 derich     (501) staff       (20)     1172 2024-05-14 01:16:37.000000 resend-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.037168 resend-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-05-24 20:34:32.037361 resend-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-05-24 14:17:40.000000 resend-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.015099 resend-1.2.0/resend/
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-05-14 01:16:37.000000 resend-1.2.0/resend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.022683 resend-1.2.0/resend/api_keys/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-1.2.0/resend/api_keys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-05-09 01:36:14.000000 resend-1.2.0/resend/api_keys/_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2024-05-09 01:36:14.000000 resend-1.2.0/resend/api_keys/_api_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.025278 resend-1.2.0/resend/audiences/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-1.2.0/resend/audiences/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1192 2024-05-09 01:36:14.000000 resend-1.2.0/resend/audiences/_audience.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-05-09 01:36:14.000000 resend-1.2.0/resend/audiences/_audiences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.027560 resend-1.2.0/resend/contacts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-1.2.0/resend/contacts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2024-05-09 01:36:14.000000 resend-1.2.0/resend/contacts/_contact.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2024-05-09 01:36:14.000000 resend-1.2.0/resend/contacts/_contacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.031464 resend-1.2.0/resend/domains/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-1.2.0/resend/domains/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2024-05-09 01:36:14.000000 resend-1.2.0/resend/domains/_domain.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2024-05-09 01:36:14.000000 resend-1.2.0/resend/domains/_domains.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-05-09 01:36:14.000000 resend-1.2.0/resend/domains/_record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.036515 resend-1.2.0/resend/emails/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-1.2.0/resend/emails/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      489 2024-05-09 01:36:14.000000 resend-1.2.0/resend/emails/_attachment.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-05-24 14:17:40.000000 resend-1.2.0/resend/emails/_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2845 2024-05-24 14:17:40.000000 resend-1.2.0/resend/emails/_email.py
+-rw-r--r--   0 root         (0) root         (0)     3281 2024-05-24 19:25:50.000000 resend-1.2.0/resend/emails/_emails.py
+-rw-r--r--   0 root         (0) root         (0)      524 2024-05-09 01:36:14.000000 resend-1.2.0/resend/emails/_tag.py
+-rw-r--r--   0 root         (0) root         (0)     6108 2024-05-22 00:27:09.000000 resend-1.2.0/resend/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-19 17:45:00.000000 resend-1.2.0/resend/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2553 2024-05-24 14:17:40.000000 resend-1.2.0/resend/request.py
+-rw-r--r--   0 root         (0) root         (0)      562 2024-05-24 14:17:40.000000 resend-1.2.0/resend/utils.py
+-rw-r--r--   0 root         (0) root         (0)      133 2024-05-24 19:07:51.000000 resend-1.2.0/resend/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.020609 resend-1.2.0/resend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-05-24 20:34:31.000000 resend-1.2.0/resend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      830 2024-05-24 20:34:32.000000 resend-1.2.0/resend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 20:34:31.000000 resend-1.2.0/resend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 20:34:31.000000 resend-1.2.0/resend.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-24 20:34:31.000000 resend-1.2.0/resend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-24 20:34:31.000000 resend-1.2.0/resend.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-24 20:34:32.038063 resend-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1222 2024-05-24 14:17:40.000000 resend-1.2.0/setup.py
```

### Comparing `resend-1.1.0/PKG-INFO` & `resend-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 1.1.0
+Version: 1.2.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
+License: UNKNOWN
+Description: # Resend Python SDK
+        
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+        ![Build](https://github.com/drish/resend-py/actions/workflows/ci.yaml/badge.svg)
+        [![codecov](https://codecov.io/gh/drish/resend-py/branch/main/graph/badge.svg?token=GGD39PPFM0)](https://codecov.io/gh/drish/resend-py)
+        [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+        [![PyPI](https://img.shields.io/pypi/v/resend)](https://pypi.org/project/resend/)
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resend)](https://pypi.org/project/resend)
+        
+        ---
+        
+        ## Installation
+        
+        To install Resend Python SDK, simply execute the following command in a terminal:
+        
+        ```
+        pip install resend
+        ```
+        
+        ## Setup
+        
+        First, you need to get an API key, which is available in the [Resend Dashboard](https://resend.com).
+        
+        ```py
+        import resend
+        import os
+        
+        resend.api_key = "re_yourkey"
+        ```
+        
+        ## Example
+        
+        You can get an overview about all parameters in the [Send Email](https://resend.com/docs/api-reference/emails/send-email) API reference.
+        
+        ```py
+        import os
+        import resend
+        
+        resend.api_key = "re_yourkey"
+        
+        params: resend.Emails.SendParams = {
+            "from": "onboarding@resend.dev",
+            "to": ["delivered@resend.dev"],
+            "subject": "hi",
+            "html": "<strong>hello, world!</strong>",
+            "reply_to": "to@gmail.com",
+            "bcc": "bcc@resend.dev",
+            "cc": ["cc@resend.dev"],
+            "tags": [
+                {"name": "tag1", "value": "tagvalue1"},
+                {"name": "tag2", "value": "tagvalue2"},
+            ],
+        }
+        
+        email: resend.Email = resend.Emails.send(params)
+        print(email)
+        ```
+        
 Keywords: email,email platform
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: requests==2.31.0
-Requires-Dist: typing_extensions
-
-# Resend Python SDK
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![Build](https://github.com/drish/resend-py/actions/workflows/test.yaml/badge.svg)
-[![codecov](https://codecov.io/gh/drish/resend-py/branch/main/graph/badge.svg?token=GGD39PPFM0)](https://codecov.io/gh/drish/resend-py)
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![PyPI](https://img.shields.io/pypi/v/resend)](https://pypi.org/project/resend/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resend)](https://pypi.org/project/resend)
-
----
-
-## Installation
-
-To install Resend Python SDK, simply execute the following command in a terminal:
-
-```
-pip install resend
-```
-
-## Setup
-
-First, you need to get an API key, which is available in the [Resend Dashboard](https://resend.com).
-
-```py
-import resend
-import os
-
-resend.api_key = "re_yourkey"
-```
-
-## Example
-
-You can get an overview about all parameters in the [Send Email](https://resend.com/docs/api-reference/emails/send-email) API reference.
-
-```py
-import os
-import resend
-
-resend.api_key = "re_yourkey"
-
-params: resend.Emails.SendParams = {
-    "from_": "onboarding@resend.dev",
-    "to": ["delivered@resend.dev"],
-    "subject": "hi",
-    "html": "<strong>hello, world!</strong>",
-    "reply_to": "to@gmail.com",
-    "bcc": "bcc@resend.dev",
-    "cc": ["cc@resend.dev"],
-    "tags": [
-        {"name": "tag1", "value": "tagvalue1"},
-        {"name": "tag2", "value": "tagvalue2"},
-    ],
-}
-
-email: resend.Email = resend.Emails.send(params)
-print(email)
-```
```

### Comparing `resend-1.1.0/README.md` & `resend-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Resend Python SDK
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![Build](https://github.com/drish/resend-py/actions/workflows/test.yaml/badge.svg)
+![Build](https://github.com/drish/resend-py/actions/workflows/ci.yaml/badge.svg)
 [![codecov](https://codecov.io/gh/drish/resend-py/branch/main/graph/badge.svg?token=GGD39PPFM0)](https://codecov.io/gh/drish/resend-py)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://img.shields.io/pypi/v/resend)](https://pypi.org/project/resend/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resend)](https://pypi.org/project/resend)
 
 ---
 
@@ -35,15 +35,15 @@
 ```py
 import os
 import resend
 
 resend.api_key = "re_yourkey"
 
 params: resend.Emails.SendParams = {
-    "from_": "onboarding@resend.dev",
+    "from": "onboarding@resend.dev",
     "to": ["delivered@resend.dev"],
     "subject": "hi",
     "html": "<strong>hello, world!</strong>",
     "reply_to": "to@gmail.com",
     "bcc": "bcc@resend.dev",
     "cc": ["cc@resend.dev"],
     "tags": [
```

### Comparing `resend-1.1.0/resend/__init__.py` & `resend-1.2.0/resend/__init__.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/api_keys/_api_key.py` & `resend-1.2.0/resend/api_keys/_api_key.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/api_keys/_api_keys.py` & `resend-1.2.0/resend/api_keys/_api_keys.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/audiences/_audience.py` & `resend-1.2.0/resend/audiences/_audience.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/audiences/_audiences.py` & `resend-1.2.0/resend/audiences/_audiences.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/contacts/_contact.py` & `resend-1.2.0/resend/contacts/_contact.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/contacts/_contacts.py` & `resend-1.2.0/resend/contacts/_contacts.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/domains/_domain.py` & `resend-1.2.0/resend/domains/_domain.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/domains/_domains.py` & `resend-1.2.0/resend/domains/_domains.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/domains/_record.py` & `resend-1.2.0/resend/domains/_record.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/emails/_batch.py` & `resend-1.2.0/resend/emails/_batch.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,13 +19,14 @@
 
         Returns:
             List[Email]: A list of email objects
         """
         path = "/emails/batch"
 
         # loop through the list of params and replace "from_" or "sender" with "from"
+        # if they're present
         replaced_params = [
             replace_params(cast(Dict[Any, Any], param)) for param in params
         ]
 
         resp = request.Request(path=path, params=replaced_params, verb="post").perform()
         return [Email.new_from_request(val) for val in resp["data"]]
```

### Comparing `resend-1.1.0/resend/emails/_email.py` & `resend-1.2.0/resend/emails/_email.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,16 @@
 
         Returns:
             Email: The new Email object
         """
         email = Email(
             id=val["id"] if "id" in val else "",
             to=val["to"] if "to" in val else "",
-            # we set sender as the value from "from" here
-            # because "from" is a reserved keyword in python
+            # from is a reserved keyword in python
+            # so we set both from_ and sender here
             from_=val["from"] if "from" in val else "",
             sender=val["from"] if "from" in val else "",
             created_at=val["created_at"] if "created_at" in val else "",
             subject=val["subject"] if "subject" in val else "",
             html=val["html"] if "html" in val else "",
             text=val["text"] if "text" in val else "",
             bcc=val["bcc"] if "bcc" in val else "",
```

### Comparing `resend-1.1.0/resend/emails/_emails.py` & `resend-1.2.0/resend/emails/_emails.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,69 +4,95 @@
 
 from resend import request
 from resend.emails._attachment import Attachment
 from resend.emails._email import Email
 from resend.emails._tag import Tag
 from resend.utils import replace_params
 
+SendParamsFrom = TypedDict(
+    "SendParamsFrom",
+    {
+        "from": str,
+        "to": Union[str, List[str]],
+        "subject": str,
+        "bcc": NotRequired[Union[List[str], str]],
+        "cc": NotRequired[Union[List[str], str]],
+        "reply_to": NotRequired[Union[List[str], str]],
+        "html": NotRequired[str],
+        "text": NotRequired[str],
+        "headers": NotRequired[Dict[str, str]],
+        "attachments": NotRequired[List[Attachment]],
+        "tags": NotRequired[List[Tag]],
+    },
+)
+
+
+class SendParamsDefault(TypedDict):
+    to: Union[str, List[str]]
+    """
+    List of email addresses to send the email to.
+    """
+    subject: str
+    """
+    The subject of the email.
+    """
+    bcc: NotRequired[Union[List[str], str]]
+    """
+    Bcc
+    """
+    cc: NotRequired[Union[List[str], str]]
+    """
+    Cc
+    """
+    reply_to: NotRequired[Union[List[str], str]]
+    """
+    Reply to
+    """
+    html: NotRequired[str]
+    """
+    The HTML content of the email.
+    """
+    text: NotRequired[str]
+    """
+    The text content of the email.
+    """
+    headers: NotRequired[Dict[str, str]]
+    """
+    Custom headers to be added to the email.
+    """
+    attachments: NotRequired[List[Attachment]]
+    """
+    List of attachments to be added to the email.
+    """
+    tags: NotRequired[List[Tag]]
+    """
+    List of tags to be added to the email.
+    """
+
+
+class SendParamsFrom_(SendParamsDefault):
+    from_: str
+    """
+    The email address of the sender.
+    "from" is a reserved keyword in python.
+    So we accept either "from_" or "sender"
+    """
+
+
+class SendParamsSender(SendParamsDefault):
+    sender: str
+    """
+    The email address of the sender.
+    "from" is a reserved keyword in python.
+    So we accept either "from_" or "sender"
+    """
+
 
 class Emails:
-    class SendParams(TypedDict):
-        from_: NotRequired[str]
-        """
-        The email address of the sender.
-        "from" is a reserved keyword in python.
-        So we accept either "from_" or "sender"
-        """
-        sender: NotRequired[str]
-        """
-        The email address of the sender.
-        "from" is a reserved keyword in python.
-        So we accept either "from_" or "sender"
-        """
-        to: Union[str, List[str]]
-        """
-        List of email addresses to send the email to.
-        """
-        subject: str
-        """
-        The subject of the email.
-        """
-        bcc: NotRequired[Union[List[str], str]]
-        """
-        Bcc
-        """
-        cc: NotRequired[Union[List[str], str]]
-        """
-        Cc
-        """
-        reply_to: NotRequired[Union[List[str], str]]
-        """
-        Reply to
-        """
-        html: NotRequired[str]
-        """
-        The HTML content of the email.
-        """
-        text: NotRequired[str]
-        """
-        The text content of the email.
-        """
-        headers: NotRequired[Dict[str, str]]
-        """
-        Custom headers to be added to the email.
-        """
-        attachments: NotRequired[List[Attachment]]
-        """
-        List of attachments to be added to the email.
-        """
-        tags: NotRequired[List[Tag]]
-        """
-        List of tags to be added to the email.
-        """
+    SendParams = Union[SendParamsFrom, SendParamsFrom_, SendParamsSender]
 
     @classmethod
     def send(cls, params: SendParams) -> Email:
         """
         Send an email through the Resend Email API.
         see more: https://resend.com/docs/api-reference/emails/send-email
```

### Comparing `resend-1.1.0/resend/emails/_tag.py` & `resend-1.2.0/resend/emails/_tag.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/exceptions.py` & `resend-1.2.0/resend/exceptions.py`

 * *Files identical despite different names*

### Comparing `resend-1.1.0/resend/request.py` & `resend-1.2.0/resend/request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-from typing import Any, Dict
+from typing import Any, Dict, List, Union
 
 import requests
+from typing_extensions import Literal
 
 import resend
 from resend.exceptions import raise_for_code_and_type
 from resend.version import get_version
 
+RequestVerb = Literal["get", "post", "put", "patch", "delete"]
+
 
 # This class wraps the HTTP request creation logic
 class Request:
-
-    def __init__(self, path: str, params: Any, verb: str):
+    def __init__(
+        self,
+        path: str,
+        params: Union[Dict[Any, Any], List[Dict[Any, Any]]],
+        verb: RequestVerb,
+    ):
         self.path = path
         self.params = params
         self.verb = verb
 
     def perform(self) -> Any:
         """Is the main function that makes the HTTP request
         to the Resend API. It uses the path, params, and verb attributes
@@ -23,15 +30,14 @@
         Returns:
             Dict: The JSON response from the API
 
         Raises:
             requests.HTTPError: If the request fails
         """
         resp = self.make_request(url=f"{resend.api_url}{self.path}")
-
         # delete calls do not return a body
         if resp.text == "" and resp.status_code == 200:
             return None
 
         # handle error in case there is a statusCode attr present
         # and status != 200
         if resp.status_code != 200 and resp.json().get("statusCode"):
```

### Comparing `resend-1.1.0/resend.egg-info/PKG-INFO` & `resend-1.2.0/resend.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 1.1.0
+Version: 1.2.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
+License: UNKNOWN
+Description: # Resend Python SDK
+        
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+        ![Build](https://github.com/drish/resend-py/actions/workflows/ci.yaml/badge.svg)
+        [![codecov](https://codecov.io/gh/drish/resend-py/branch/main/graph/badge.svg?token=GGD39PPFM0)](https://codecov.io/gh/drish/resend-py)
+        [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+        [![PyPI](https://img.shields.io/pypi/v/resend)](https://pypi.org/project/resend/)
+        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resend)](https://pypi.org/project/resend)
+        
+        ---
+        
+        ## Installation
+        
+        To install Resend Python SDK, simply execute the following command in a terminal:
+        
+        ```
+        pip install resend
+        ```
+        
+        ## Setup
+        
+        First, you need to get an API key, which is available in the [Resend Dashboard](https://resend.com).
+        
+        ```py
+        import resend
+        import os
+        
+        resend.api_key = "re_yourkey"
+        ```
+        
+        ## Example
+        
+        You can get an overview about all parameters in the [Send Email](https://resend.com/docs/api-reference/emails/send-email) API reference.
+        
+        ```py
+        import os
+        import resend
+        
+        resend.api_key = "re_yourkey"
+        
+        params: resend.Emails.SendParams = {
+            "from": "onboarding@resend.dev",
+            "to": ["delivered@resend.dev"],
+            "subject": "hi",
+            "html": "<strong>hello, world!</strong>",
+            "reply_to": "to@gmail.com",
+            "bcc": "bcc@resend.dev",
+            "cc": ["cc@resend.dev"],
+            "tags": [
+                {"name": "tag1", "value": "tagvalue1"},
+                {"name": "tag2", "value": "tagvalue2"},
+            ],
+        }
+        
+        email: resend.Email = resend.Emails.send(params)
+        print(email)
+        ```
+        
 Keywords: email,email platform
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: requests==2.31.0
-Requires-Dist: typing_extensions
-
-# Resend Python SDK
-
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-![Build](https://github.com/drish/resend-py/actions/workflows/test.yaml/badge.svg)
-[![codecov](https://codecov.io/gh/drish/resend-py/branch/main/graph/badge.svg?token=GGD39PPFM0)](https://codecov.io/gh/drish/resend-py)
-[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![PyPI](https://img.shields.io/pypi/v/resend)](https://pypi.org/project/resend/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resend)](https://pypi.org/project/resend)
-
----
-
-## Installation
-
-To install Resend Python SDK, simply execute the following command in a terminal:
-
-```
-pip install resend
-```
-
-## Setup
-
-First, you need to get an API key, which is available in the [Resend Dashboard](https://resend.com).
-
-```py
-import resend
-import os
-
-resend.api_key = "re_yourkey"
-```
-
-## Example
-
-You can get an overview about all parameters in the [Send Email](https://resend.com/docs/api-reference/emails/send-email) API reference.
-
-```py
-import os
-import resend
-
-resend.api_key = "re_yourkey"
-
-params: resend.Emails.SendParams = {
-    "from_": "onboarding@resend.dev",
-    "to": ["delivered@resend.dev"],
-    "subject": "hi",
-    "html": "<strong>hello, world!</strong>",
-    "reply_to": "to@gmail.com",
-    "bcc": "bcc@resend.dev",
-    "cc": ["cc@resend.dev"],
-    "tags": [
-        {"name": "tag1", "value": "tagvalue1"},
-        {"name": "tag2", "value": "tagvalue2"},
-    ],
-}
-
-email: resend.Email = resend.Emails.send(params)
-print(email)
-```
```

### Comparing `resend-1.1.0/resend.egg-info/SOURCES.txt` & `resend-1.2.0/resend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE.md
 README.md
 setup.cfg
 setup.py
 resend/__init__.py
 resend/exceptions.py
 resend/py.typed
 resend/request.py
```

### Comparing `resend-1.1.0/setup.py` & `resend-1.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,9 +27,10 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

