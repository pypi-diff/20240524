# Comparing `tmp/wipac-keycloak-rest-services-1.4.92.tar.gz` & `tmp/wipac-keycloak-rest-services-1.4.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-keycloak-rest-services-1.4.92.tar", last modified: Wed May 22 18:26:19 2024, max compression
+gzip compressed data, was "wipac-keycloak-rest-services-1.4.93.tar", last modified: Fri May 24 20:28:23 2024, max compression
```

## Comparing `wipac-keycloak-rest-services-1.4.92.tar` & `wipac-keycloak-rest-services-1.4.93.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:26:19.838091 wipac-keycloak-rest-services-1.4.92/
--rw-r--r--   0 root         (0) root         (0)     1103 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4149 2024-05-22 18:26:19.838091 wipac-keycloak-rest-services-1.4.92/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3139 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:26:19.838091 wipac-keycloak-rest-services-1.4.92/krs/
--rw-r--r--   0 root         (0) root         (0)      514 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20266 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/apps.py
--rw-r--r--   0 root         (0) root         (0)    16594 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     3215 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/email.py
--rw-r--r--   0 root         (0) root         (0)    16899 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/groups.py
--rw-r--r--   0 root         (0) root         (0)     9038 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/institutions.py
--rw-r--r--   0 root         (0) root         (0)    22784 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/ldap.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/py.typed
--rw-r--r--   0 root         (0) root         (0)     5722 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/token.py
--rw-r--r--   0 root         (0) root         (0)     9039 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/users.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/krs/util.py
--rw-r--r--   0 root         (0) root         (0)     2306 2024-05-22 18:26:19.838091 wipac-keycloak-rest-services-1.4.92/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2024-05-22 18:26:17.000000 wipac-keycloak-rest-services-1.4.92/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:26:19.838091 wipac-keycloak-rest-services-1.4.92/wipac_keycloak_rest_services.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4149 2024-05-22 18:26:19.000000 wipac-keycloak-rest-services-1.4.92/wipac_keycloak_rest_services.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2024-05-22 18:26:19.000000 wipac-keycloak-rest-services-1.4.92/wipac_keycloak_rest_services.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 18:26:19.000000 wipac-keycloak-rest-services-1.4.92/wipac_keycloak_rest_services.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      222 2024-05-22 18:26:19.000000 wipac-keycloak-rest-services-1.4.92/wipac_keycloak_rest_services.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-05-22 18:26:19.000000 wipac-keycloak-rest-services-1.4.92/wipac_keycloak_rest_services.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:28:23.539024 wipac-keycloak-rest-services-1.4.93/
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4149 2024-05-24 20:28:23.539024 wipac-keycloak-rest-services-1.4.93/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:28:23.539024 wipac-keycloak-rest-services-1.4.93/krs/
+-rw-r--r--   0 root         (0) root         (0)      514 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20266 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/apps.py
+-rw-r--r--   0 root         (0) root         (0)    16594 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     3307 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/email.py
+-rw-r--r--   0 root         (0) root         (0)    16899 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/groups.py
+-rw-r--r--   0 root         (0) root         (0)     9038 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/institutions.py
+-rw-r--r--   0 root         (0) root         (0)    22784 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/ldap.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5722 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/token.py
+-rw-r--r--   0 root         (0) root         (0)     9039 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/users.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/krs/util.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-05-24 20:28:23.539024 wipac-keycloak-rest-services-1.4.93/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-24 20:28:21.000000 wipac-keycloak-rest-services-1.4.93/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:28:23.539024 wipac-keycloak-rest-services-1.4.93/wipac_keycloak_rest_services.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4149 2024-05-24 20:28:23.000000 wipac-keycloak-rest-services-1.4.93/wipac_keycloak_rest_services.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2024-05-24 20:28:23.000000 wipac-keycloak-rest-services-1.4.93/wipac_keycloak_rest_services.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 20:28:23.000000 wipac-keycloak-rest-services-1.4.93/wipac_keycloak_rest_services.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      228 2024-05-24 20:28:23.000000 wipac-keycloak-rest-services-1.4.93/wipac_keycloak_rest_services.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-05-24 20:28:23.000000 wipac-keycloak-rest-services-1.4.93/wipac_keycloak_rest_services.egg-info/top_level.txt
```

### Comparing `wipac-keycloak-rest-services-1.4.92/LICENSE` & `wipac-keycloak-rest-services-1.4.93/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.92/PKG-INFO` & `wipac-keycloak-rest-services-1.4.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.4.92
+Version: 1.4.93
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_fc_8ox28_/tmpneh8y87a_TarContainer/0/2", line 94, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.92
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.93
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
```

### Comparing `wipac-keycloak-rest-services-1.4.92/README.md` & `wipac-keycloak-rest-services-1.4.93/README.md`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.92/krs/__init__.py` & `wipac-keycloak-rest-services-1.4.93/krs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.4.92"
+__version__ = "1.4.93"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-keycloak-rest-services-1.4.92/krs/apps.py` & `wipac-keycloak-rest-services-1.4.93/krs/apps.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.92/krs/bootstrap.py` & `wipac-keycloak-rest-services-1.4.93/krs/bootstrap.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.92/krs/email.py` & `wipac-keycloak-rest-services-1.4.93/krs/email.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,22 +49,23 @@
       <p class="copyright">© WIPAC, University of Wisconsin-Madison</p>
     </footer>
   </body>
 </html>
 """
 
 
-def send_email(recipient, subject, content, headline="IceCube Identity Management", sender=None):
+def send_email(recipient, subject, content, cc=None, headline="IceCube Identity Management", sender=None):
     """
     Send an email message.
 
     Args:
-        recipient (dict): Dict with name and email, or just a string email address
+        recipient (dict|str): Dict with name and email, or just a string email address
         subject (str): Email subject
         content (str): Email content
+        cc (str|list): Email CC address(es)
         headline (str): Message headline used in HTML email body
         sender (dict): (optional) Dict with name and email, or just a string email address
     """
     config = from_environment({
         'EMAIL_SENDER': 'no-reply@icecube.wisc.edu',
         'EMAIL_SMTP_SERVER': 'localhost',
         'EMAIL_SMTP_TIMEOUT': 5,  # email should be mostly instant
@@ -93,13 +94,16 @@
         else:
             username = recipient['email']
             domain = ''
         msg['To'] = (Address(recipient['name'], username, domain),)
     else:
         msg['To'] = recipient
 
+    if cc:
+        msg['CC'] = cc
+
     msg.set_content(TEMPLATE.format(content))
     msg.add_alternative(HTML_TEMPLATE.format(content.replace('\n', '<br>'), headline=headline),
                         subtype='html')
 
     with smtplib.SMTP(config['EMAIL_SMTP_SERVER'], timeout=config['EMAIL_SMTP_TIMEOUT']) as s:
         s.send_message(msg)
```

### Comparing `wipac-keycloak-rest-services-1.4.92/krs/groups.py` & `wipac-keycloak-rest-services-1.4.93/krs/groups.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.92/krs/institutions.py` & `wipac-keycloak-rest-services-1.4.93/krs/institutions.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.92/krs/ldap.py` & `wipac-keycloak-rest-services-1.4.93/krs/ldap.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.92/krs/rabbitmq.py` & `wipac-keycloak-rest-services-1.4.93/krs/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.92/krs/token.py` & `wipac-keycloak-rest-services-1.4.93/krs/token.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.92/krs/users.py` & `wipac-keycloak-rest-services-1.4.93/krs/users.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.92/krs/util.py` & `wipac-keycloak-rest-services-1.4.93/krs/util.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.4.92/setup.cfg` & `wipac-keycloak-rest-services-1.4.93/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 minor_emoji = [minor]
 patch_emoji = [fix], [patch]
 branch = master
 
 [options]
 install_requires = 
 	aio_pika
+	attrs
 	ldap3
 	motor
 	requests
 	unidecode
 	wipac-dev-tools
 	wipac-rest-tools
 python_requires = >=3.9, <3.13
```

### Comparing `wipac-keycloak-rest-services-1.4.92/wipac_keycloak_rest_services.egg-info/PKG-INFO` & `wipac-keycloak-rest-services-1.4.93/wipac_keycloak_rest_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.4.92
+Version: 1.4.93
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_fc_8ox28_/tmpneh8y87a_TarContainer/0/20", line 94, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.92
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.93
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
```

