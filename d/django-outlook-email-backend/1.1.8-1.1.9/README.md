# Comparing `tmp/django_outlook_email_backend-1.1.8.tar.gz` & `tmp/django_outlook_email_backend-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_outlook_email_backend-1.1.8.tar", last modified: Tue May 21 16:13:25 2024, max compression
+gzip compressed data, was "django_outlook_email_backend-1.1.9.tar", last modified: Fri May 24 09:32:14 2024, max compression
```

## Comparing `django_outlook_email_backend-1.1.8.tar` & `django_outlook_email_backend-1.1.9.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:25.077023 django_outlook_email_backend-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-21 16:13:25.077023 django_outlook_email_backend-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:25.073023 django_outlook_email_backend-1.1.8/django_outlook_email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/django_outlook_email_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:25.073023 django_outlook_email_backend-1.1.8/django_outlook_email/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/exceptions/microsoft_graph_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:25.077023 django_outlook_email_backend-1.1.8/django_outlook_email/senders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/senders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:25.077023 django_outlook_email_backend-1.1.8/django_outlook_email/senders/attachments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/senders/attachments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/senders/attachments/attachments_using_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/senders/base_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/senders/content_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/senders/json_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:25.077023 django_outlook_email_backend-1.1.8/django_outlook_email/senders/microsoft_requests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/senders/microsoft_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/senders/microsoft_requests/microsoft_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/django_outlook_email/senders/mime_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:13:25.077023 django_outlook_email_backend-1.1.8/django_outlook_email_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-21 16:13:25.000000 django_outlook_email_backend-1.1.8/django_outlook_email_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 16:13:25.000000 django_outlook_email_backend-1.1.8/django_outlook_email_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 16:13:25.000000 django_outlook_email_backend-1.1.8/django_outlook_email_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 16:13:25.000000 django_outlook_email_backend-1.1.8/django_outlook_email_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 16:13:25.000000 django_outlook_email_backend-1.1.8/django_outlook_email_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 16:13:24.000000 django_outlook_email_backend-1.1.8/django_outlook_email_backend.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 16:13:25.077023 django_outlook_email_backend-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-21 16:13:21.000000 django_outlook_email_backend-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:14.342024 django_outlook_email_backend-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-24 09:32:14.342024 django_outlook_email_backend-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:14.338024 django_outlook_email_backend-1.1.9/django_outlook_email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/django_outlook_email_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:14.338024 django_outlook_email_backend-1.1.9/django_outlook_email/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/exceptions/microsoft_graph_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:14.342024 django_outlook_email_backend-1.1.9/django_outlook_email/senders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/senders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:14.342024 django_outlook_email_backend-1.1.9/django_outlook_email/senders/attachments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/senders/attachments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/senders/attachments/attachments_using_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/senders/base_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/senders/content_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:14.342024 django_outlook_email_backend-1.1.9/django_outlook_email/senders/encoders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/senders/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/senders/encoders/lazy_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/senders/json_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:14.342024 django_outlook_email_backend-1.1.9/django_outlook_email/senders/microsoft_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/senders/microsoft_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/senders/microsoft_requests/microsoft_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/django_outlook_email/senders/mime_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:32:14.342024 django_outlook_email_backend-1.1.9/django_outlook_email_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-24 09:32:14.000000 django_outlook_email_backend-1.1.9/django_outlook_email_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-24 09:32:14.000000 django_outlook_email_backend-1.1.9/django_outlook_email_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:32:14.000000 django_outlook_email_backend-1.1.9/django_outlook_email_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 09:32:14.000000 django_outlook_email_backend-1.1.9/django_outlook_email_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-24 09:32:14.000000 django_outlook_email_backend-1.1.9/django_outlook_email_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:32:14.000000 django_outlook_email_backend-1.1.9/django_outlook_email_backend.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 09:32:14.342024 django_outlook_email_backend-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-24 09:32:10.000000 django_outlook_email_backend-1.1.9/setup.py
```

### Comparing `django_outlook_email_backend-1.1.8/LICENSE` & `django_outlook_email_backend-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.8/PKG-INFO` & `django_outlook_email_backend-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_outlook_email-backend
-Version: 1.1.8
+Version: 1.1.9
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-1.1.8/README.md` & `django_outlook_email_backend-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.8/django_outlook_email/django_outlook_email_backend.py` & `django_outlook_email_backend-1.1.9/django_outlook_email/django_outlook_email_backend.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.8/django_outlook_email/senders/attachments/attachments_using_upload_session.py` & `django_outlook_email_backend-1.1.9/django_outlook_email/senders/attachments/attachments_using_upload_session.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.8/django_outlook_email/senders/content_types.py` & `django_outlook_email_backend-1.1.9/django_outlook_email/senders/content_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
 class ContentType(Enum):
-    TEXT_PLAIN = "text/plain"
+    TEXT_PLAIN = "plain"
     TEXT_HTML = "text/html"
 
 class MicrosoftContentType(Enum):
     TEXT_PLAIN = "Text"
     TEXT_HTML = "HTML"
 
     @classmethod
```

### Comparing `django_outlook_email_backend-1.1.8/django_outlook_email/senders/json_sender.py` & `django_outlook_email_backend-1.1.9/django_outlook_email/senders/json_sender.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from django.conf import settings
 from django_outlook_email.exceptions.microsoft_graph_exceptions import JsonSenderException, MicrosoftGraphException
 from django_outlook_email.senders.attachments.attachments_using_upload_session import UploadAttachment
 from django_outlook_email.senders.base_sender import BaseSender
 from django.core.mail.message import sanitize_address
 
+from django_outlook_email.senders.content_types import MicrosoftContentType
 from django_outlook_email.senders.microsoft_requests.microsoft_requests import MicrosoftRequests
 
 
 class JsonSender(BaseSender):
 
     def send(self, email_message):
         if not email_message.recipients():
@@ -27,15 +28,15 @@
         if not content:
             return False
 
         data = {
             "message": {
                 "body": {
                     "content": content,
-                    "contentType": "HTML"  # text/html #plain
+                    "contentType": content_type  # text/html #plain
                 },
                 "subject": email_message.subject,
                 "toRecipients": recipients,
                 "hasAttachments": False,
             }
         }
 
@@ -97,15 +98,15 @@
         if alternatives:
             content = email_message.alternatives[0][0]
             content_type = email_message.alternatives[0][1]
         else:
             content = email_message.body
             content_type = email_message.content_subtype
 
-        return content, content_type
+        return content, MicrosoftContentType.django_to_microsoft(content_type)
 
     def _get_alternatives(self, email_message):
         html_alternatives = []
         text_plain_alternatives = []
         for alternative in email_message.alternatives:
             if alternative[1] == "text/plain":
                 text_plain_alternatives.append(alternative[0])
```

### Comparing `django_outlook_email_backend-1.1.8/django_outlook_email/senders/microsoft_requests/microsoft_requests.py` & `django_outlook_email_backend-1.1.9/django_outlook_email/senders/microsoft_requests/microsoft_requests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,29 @@
+import json
+
 from django_outlook_email.exceptions.microsoft_graph_exceptions import MicrosoftGraphException
 import requests
 
+from django_outlook_email.senders.encoders.lazy_encoders import LazyEncoder
+
+
 class MicrosoftRequests:
     def __init__(self, from_email, access_token, fail_silently):
         self.from_email = from_email
         self.access_token = access_token
         self.fail_silently = fail_silently
 
     def post(self, endpoint, data):
+        data = json.dumps(data, cls=LazyEncoder)
         try:
             response = requests.post(
                 "https://graph.microsoft.com/v1.0/users/" + self.from_email + "/" + endpoint,
-                json=data,
+                data=data,
 
-                headers={"Authorization": "Bearer " + self.access_token},
+                headers={"Authorization": "Bearer " + self.access_token, 'Content-Type': 'application/json'},
             )
         except requests.exceptions.RequestException:
             if not self.fail_silently:
                 raise
             return False
 
         if response.status_code in [202, 201]:
```

### Comparing `django_outlook_email_backend-1.1.8/django_outlook_email/senders/mime_sender.py` & `django_outlook_email_backend-1.1.9/django_outlook_email/senders/mime_sender.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.8/django_outlook_email_backend.egg-info/PKG-INFO` & `django_outlook_email_backend-1.1.9/django_outlook_email_backend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_outlook_email-backend
-Version: 1.1.8
+Version: 1.1.9
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-1.1.8/django_outlook_email_backend.egg-info/SOURCES.txt` & `django_outlook_email_backend-1.1.9/django_outlook_email_backend.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 django_outlook_email/senders/__init__.py
 django_outlook_email/senders/base_sender.py
 django_outlook_email/senders/content_types.py
 django_outlook_email/senders/json_sender.py
 django_outlook_email/senders/mime_sender.py
 django_outlook_email/senders/attachments/__init__.py
 django_outlook_email/senders/attachments/attachments_using_upload_session.py
+django_outlook_email/senders/encoders/__init__.py
+django_outlook_email/senders/encoders/lazy_encoders.py
 django_outlook_email/senders/microsoft_requests/__init__.py
 django_outlook_email/senders/microsoft_requests/microsoft_requests.py
 django_outlook_email_backend.egg-info/PKG-INFO
 django_outlook_email_backend.egg-info/SOURCES.txt
 django_outlook_email_backend.egg-info/dependency_links.txt
 django_outlook_email_backend.egg-info/requires.txt
 django_outlook_email_backend.egg-info/top_level.txt
```

### Comparing `django_outlook_email_backend-1.1.8/setup.py` & `django_outlook_email_backend-1.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='django_outlook_email-backend',
-    version='1.1.8',
+    version='1.1.9',
     description='Ouauth2 outlook email backend for Django',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Marc Claramunt',
     author_email='mclaramunt@enley.com',
     license='MIT',
     zip_safe=True,
@@ -16,10 +16,10 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     url='https://github.com/enley-es/django-outlook-email-backend',
-    packages=["django_outlook_email","django_outlook_email.exceptions", "django_outlook_email.senders","django_outlook_email.senders.attachments","django_outlook_email.senders.microsoft_requests"],
+    packages=["django_outlook_email","django_outlook_email.exceptions", "django_outlook_email.senders","django_outlook_email.senders.attachments","django_outlook_email.senders.microsoft_requests","django_outlook_email.senders.encoders"],
     install_requires = ['requests~=2.25', 'msal==1.*']
 )
```

