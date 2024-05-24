# Comparing `tmp/pretix-payone-1.3.2.tar.gz` & `tmp/pretix_payone-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-payone-1.3.2.tar", last modified: Tue Jun 27 13:01:31 2023, max compression
+gzip compressed data, was "pretix_payone-1.3.3.tar", last modified: Fri May 24 08:27:47 2024, max compression
```

## Comparing `pretix-payone-1.3.2.tar` & `pretix_payone-1.3.3.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.123327 pretix-payone-1.3.2/
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2462 2023-06-27 13:01:31.123327 pretix-payone-1.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1390 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      773 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.111327 pretix-payone-1.3.2/pretix_payone/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10537 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/locale/de_Informal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    10484 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     8146 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/locale/django.pot
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1197 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/migrations/0002_auto_20220204_1638.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      308 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/models.py
--rw-rw-rw-   0 root         (0) root         (0)    33634 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/payment.py
--rw-rw-rw-   0 root         (0) root         (0)     2484 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.115327 pretix-payone-1.3.2/pretix_payone/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone/static/pretix_payone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/static/pretix_payone/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)     6372 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/static/pretix_payone/cc.js
--rw-rw-rw-   0 root         (0) root         (0)     3517 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/static/pretix_payone/logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.115327 pretix-payone-1.3.2/pretix_payone/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.123327 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/checkout_payment_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/checkout_payment_form.html
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/control.html
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/pending.html
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/redirect.html
--rw-rw-rw-   0 root         (0) root         (0)      601 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     8795 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pretix_payone/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.119327 pretix-payone-1.3.2/pretix_payone.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-06-27 13:01:31.000000 pretix-payone-1.3.2/pretix_payone.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1274 2023-06-27 13:01:31.000000 pretix-payone-1.3.2/pretix_payone.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-27 13:01:31.000000 pretix-payone-1.3.2/pretix_payone.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-27 13:01:31.000000 pretix-payone-1.3.2/pretix_payone.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-27 13:01:31.000000 pretix-payone-1.3.2/pretix_payone.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-27 13:01:31.123327 pretix-payone-1.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-27 13:01:31.123327 pretix-payone-1.3.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-27 13:01:01.000000 pretix-payone-1.3.2/tests/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.452028 pretix_payone-1.3.3/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2462 2024-05-24 08:27:47.452028 pretix_payone-1.3.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1390 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.448028 pretix_payone-1.3.3/pretix_payone/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-24 08:27:13.000000 pretix_payone-1.3.3/pretix_payone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      773 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.448028 pretix_payone-1.3.3/pretix_payone/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.440028 pretix_payone-1.3.3/pretix_payone/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.448028 pretix_payone-1.3.3/pretix_payone/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10537 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/locale/de/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      873 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.448028 pretix_payone-1.3.3/pretix_payone/locale/de_Informal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:27:14.000000 pretix_payone-1.3.3/pretix_payone/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.448028 pretix_payone-1.3.3/pretix_payone/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    10484 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      820 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/locale/de_Informal/LC_MESSAGES/djangojs.po
+-rw-rw-rw-   0 root         (0) root         (0)     8146 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/locale/django.pot
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/locale/djangojs.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.448028 pretix_payone-1.3.3/pretix_payone/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/migrations/0002_auto_20220204_1638.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:27:14.000000 pretix_payone-1.3.3/pretix_payone/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      308 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    33562 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2484 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.440028 pretix_payone-1.3.3/pretix_payone/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.452028 pretix_payone-1.3.3/pretix_payone/static/pretix_payone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:27:14.000000 pretix_payone-1.3.3/pretix_payone/static/pretix_payone/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)     6372 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/static/pretix_payone/cc.js
+-rw-rw-rw-   0 root         (0) root         (0)     3517 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/static/pretix_payone/logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.444028 pretix_payone-1.3.3/pretix_payone/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.452028 pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 08:27:14.000000 pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/.gitkeep
+-rw-rw-rw-   0 root         (0) root         (0)      354 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/checkout_payment_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      338 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/checkout_payment_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/control.html
+-rw-rw-rw-   0 root         (0) root         (0)      963 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/redirect.html
+-rw-rw-rw-   0 root         (0) root         (0)      601 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     8795 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pretix_payone/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.452028 pretix_payone-1.3.3/pretix_payone.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2024-05-24 08:27:47.000000 pretix_payone-1.3.3/pretix_payone.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1413 2024-05-24 08:27:47.000000 pretix_payone-1.3.3/pretix_payone.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 08:27:47.000000 pretix_payone-1.3.3/pretix_payone.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      131 2024-05-24 08:27:47.000000 pretix_payone-1.3.3/pretix_payone.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-24 08:27:47.000000 pretix_payone-1.3.3/pretix_payone.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      824 2024-05-24 08:27:47.456028 pretix_payone-1.3.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 08:27:47.452028 pretix_payone-1.3.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-05-24 08:23:16.000000 pretix_payone-1.3.3/tests/test_main.py
```

### Comparing `pretix-payone-1.3.2/LICENSE` & `pretix_payone-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/PKG-INFO` & `pretix_payone-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-payone
-Version: 1.3.2
+Version: 1.3.3
 Summary: Allows to process payments through PAYONE (formerly BS Payone)
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: 
         Copyright 2021 pretix team
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `pretix-payone-1.3.2/README.rst` & `pretix_payone-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/apps.py` & `pretix_payone-1.3.3/pretix_payone/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/locale/de/LC_MESSAGES/django.po` & `pretix_payone-1.3.3/pretix_payone/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po` & `pretix_payone-1.3.3/pretix_payone/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/locale/django.pot` & `pretix_payone-1.3.3/pretix_payone/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/migrations/0001_initial.py` & `pretix_payone-1.3.3/pretix_payone/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/migrations/0002_auto_20220204_1638.py` & `pretix_payone-1.3.3/pretix_payone/migrations/0002_auto_20220204_1638.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/payment.py` & `pretix_payone-1.3.3/pretix_payone/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ("V", _("VISA")),
     ("M", _("MasterCard")),
     ("J", _("JCB")),
     ("A", _("American Express")),
     ("D", _("Diners Club/Discover")),
     ("O", _("Maestro")),
     ("U", _("UTAP/AirPlus")),
-    ("P", _("China Union Pay"))
+    ("P", _("China Union Pay")),
     # https://docs.payone.com/display/public/PLATFORM/cardtype+-+definition
 ]
 
 
 class PayoneSettingsHolder(BasePaymentProvider):
     identifier = "payone"
     verbose_name = "PAYONE"
@@ -174,16 +174,15 @@
     def test_mode_message(self):
         if self.event.testmode:
             return mark_safe(
                 _(
                     "The PayOne plugin is operating in test mode. You can use one of <a {args}>many test "
                     "cards</a> to perform a transaction. No money will actually be transferred."
                 ).format(
-                    args='href="https://docs.payone.com/display/public/PLATFORM/Testdata" '
-                    'target="_blank"'
+                    args='href="https://docs.payone.com/security-risk-management/3d-secure#Specialremarks3DSecure-Testdata" target="_blank"'
                 )
             )
         return None
 
     @property
     def is_enabled(self) -> bool:
         return self.settings.get("_enabled", as_type=bool) and self.settings.get(
@@ -222,17 +221,14 @@
             "request": request,
             "event": self.event,
             "settings": self.settings,
             "provider": self,
         }
         return template.render(ctx)
 
-    def payment_can_retry(self, payment):
-        return self._is_still_available(order=payment.order)
-
     def payment_pending_render(self, request, payment) -> str:
         if payment.info:
             payment_info = json.loads(payment.info)
         else:
             payment_info = None
         template = get_template("pretix_payone/pending.html")
         ctx = {
@@ -454,19 +450,19 @@
             d["country"] = guess_country(self.event) or "DE"
 
         if ia.vat_id and ia.vat_id_validated:
             d["vatid"] = ia.vat_id
 
         if self.invoice_address_mandatory:
             if ia.name_parts.get("salutation"):
-                d["salutation"] = ia.get("salutation", "")[:10]
+                d["salutation"] = ia.name_parts.get("salutation", "")[:10]
             if ia.name_parts.get("title"):
-                d["title"] = ia.get("title", "")[:20]
-            if ia.address:
-                d["street"] = ia.address[:50]
+                d["title"] = ia.name_parts.get("title", "")[:20]
+            if ia.street:
+                d["street"] = ia.street[:50]
             if ia.zipcode:
                 d["zip"] = ia.zipcode[:10]
             if ia.city:
                 d["city"] = ia.city[:50]
             if ia.state and ia.country in (
                 "US",
                 "CA",
```

### Comparing `pretix-payone-1.3.2/pretix_payone/signals.py` & `pretix_payone-1.3.3/pretix_payone/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/static/pretix_payone/cc.js` & `pretix_payone-1.3.3/pretix_payone/static/pretix_payone/cc.js`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/static/pretix_payone/logo.svg` & `pretix_payone-1.3.3/pretix_payone/static/pretix_payone/logo.svg`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html` & `pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/checkout_payment_form_cc.html`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/control.html` & `pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/control.html`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/pending.html` & `pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/pending.html`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/templates/pretix_payone/redirect.html` & `pretix_payone-1.3.3/pretix_payone/templates/pretix_payone/redirect.html`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/urls.py` & `pretix_payone-1.3.3/pretix_payone/urls.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone/views.py` & `pretix_payone-1.3.3/pretix_payone/views.py`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/pretix_payone.egg-info/PKG-INFO` & `pretix_payone-1.3.3/pretix_payone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-payone
-Version: 1.3.2
+Version: 1.3.3
 Summary: Allows to process payments through PAYONE (formerly BS Payone)
 Author-email: pretix team <support@pretix.eu>
 Maintainer-email: pretix team <support@pretix.eu>
 License: 
         Copyright 2021 pretix team
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `pretix-payone-1.3.2/pretix_payone.egg-info/SOURCES.txt` & `pretix_payone-1.3.3/pretix_payone.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 pretix_payone/views.py
 pretix_payone.egg-info/PKG-INFO
 pretix_payone.egg-info/SOURCES.txt
 pretix_payone.egg-info/dependency_links.txt
 pretix_payone.egg-info/entry_points.txt
 pretix_payone.egg-info/top_level.txt
 pretix_payone/locale/django.pot
+pretix_payone/locale/djangojs.pot
 pretix_payone/locale/de/LC_MESSAGES/django.po
+pretix_payone/locale/de/LC_MESSAGES/djangojs.po
 pretix_payone/locale/de_Informal/.gitkeep
 pretix_payone/locale/de_Informal/LC_MESSAGES/django.po
+pretix_payone/locale/de_Informal/LC_MESSAGES/djangojs.po
 pretix_payone/migrations/0001_initial.py
 pretix_payone/migrations/0002_auto_20220204_1638.py
 pretix_payone/migrations/__init__.py
 pretix_payone/static/pretix_payone/.gitkeep
 pretix_payone/static/pretix_payone/cc.js
 pretix_payone/static/pretix_payone/logo.svg
 pretix_payone/templates/pretix_payone/.gitkeep
```

### Comparing `pretix-payone-1.3.2/pyproject.toml` & `pretix_payone-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pretix-payone-1.3.2/setup.cfg` & `pretix_payone-1.3.3/setup.cfg`

 * *Files identical despite different names*

