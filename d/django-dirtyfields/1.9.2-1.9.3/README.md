# Comparing `tmp/django-dirtyfields-1.9.2.tar.gz` & `tmp/django-dirtyfields-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dirtyfields-1.9.2.tar", last modified: Wed Apr 12 10:18:52 2023, max compression
+gzip compressed data, was "django-dirtyfields-1.9.3.tar", last modified: Fri May 24 12:21:41 2024, max compression
```

## Comparing `django-dirtyfields-1.9.2.tar` & `django-dirtyfields-1.9.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/ChangeLog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/src/dirtyfields/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/src/dirtyfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/src/dirtyfields/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-12 10:18:40.000000 django-dirtyfields-1.9.2/src/dirtyfields/dirtyfields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 10:18:52.535619 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-12 10:18:52.000000 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-12 10:18:52.000000 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 10:18:52.000000 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 10:18:52.000000 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 10:18:52.000000 django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:21:41.747439 django-dirtyfields-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-24 12:21:36.000000 django-dirtyfields-1.9.3/ChangeLog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-24 12:21:36.000000 django-dirtyfields-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-24 12:21:36.000000 django-dirtyfields-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-24 12:21:41.751439 django-dirtyfields-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-24 12:21:36.000000 django-dirtyfields-1.9.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-24 12:21:36.000000 django-dirtyfields-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-24 12:21:41.751439 django-dirtyfields-1.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:21:41.747439 django-dirtyfields-1.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:21:41.747439 django-dirtyfields-1.9.3/src/dirtyfields/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-24 12:21:36.000000 django-dirtyfields-1.9.3/src/dirtyfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-24 12:21:36.000000 django-dirtyfields-1.9.3/src/dirtyfields/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-24 12:21:36.000000 django-dirtyfields-1.9.3/src/dirtyfields/dirtyfields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 12:21:41.747439 django-dirtyfields-1.9.3/src/django_dirtyfields.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-24 12:21:41.000000 django-dirtyfields-1.9.3/src/django_dirtyfields.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-24 12:21:41.000000 django-dirtyfields-1.9.3/src/django_dirtyfields.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 12:21:41.000000 django-dirtyfields-1.9.3/src/django_dirtyfields.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 12:21:41.000000 django-dirtyfields-1.9.3/src/django_dirtyfields.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 12:21:41.000000 django-dirtyfields-1.9.3/src/django_dirtyfields.egg-info/top_level.txt
```

### Comparing `django-dirtyfields-1.9.2/ChangeLog.rst` & `django-dirtyfields-1.9.3/ChangeLog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 .. _unreleased:
 
 unreleased
 ----------
 
 
 
+.. _v1.9.3:
+
+1.9.3 (2024-05-24)
+------------------
+
+*New:*
+    - Confirm support for Python 3.12
+    - Confirm support for Django 5.0
+    - Drop support for Python 3.7
+    - Drop support for Django 2.0
+    - Drop support for Django 2.1
+
+
 .. _v1.9.2:
 
 1.9.2 (2023-04-12)
 ------------------
 
 *New:*
     - Confirm support for Django 4.2
```

### Comparing `django-dirtyfields-1.9.2/LICENSE` & `django-dirtyfields-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dirtyfields-1.9.2/PKG-INFO` & `django-dirtyfields-1.9.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dirtyfields
-Version: 1.9.2
+Version: 1.9.3
 Summary: Tracking dirty fields on a Django model instance.
 Home-page: https://github.com/romgar/django-dirtyfields
 Author: Romain Garrigues
 Maintainer: Lincoln Puzey
 License: BSD
 Project-URL: Documentation, https://django-dirtyfields.readthedocs.io/
 Project-URL: Changelog, https://github.com/romgar/django-dirtyfields/blob/develop/ChangeLog.rst
@@ -13,30 +13,29 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
-Requires-Python: >=3.7
+Classifier: Framework :: Django :: 5.0
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 Django Dirty Fields
 ===================
 
@@ -61,23 +60,23 @@
 
 This package is compatible and tested with the following Python & Django versions:
 
 
 +------------------------+-----------------------------------+
 | Django                 | Python                            |
 +========================+===================================+
-| 2.0, 2.1               | 3.7                               |
+| 2.2, 3.0, 3.1          | 3.8, 3.9                          |
 +------------------------+-----------------------------------+
-| 2.2, 3.0, 3.1          | 3.7, 3.8, 3.9                     |
+| 3.2, 4.0               | 3.8, 3.9, 3.10                    |
 +------------------------+-----------------------------------+
-| 3.2                    | 3.7, 3.8, 3.9, 3.10               |
+| 4.1                    | 3.8, 3.9, 3.10, 3.11              |
 +------------------------+-----------------------------------+
-| 4.0                    | 3.8, 3.9, 3.10                    |
+| 4.2                    | 3.8, 3.9, 3.10, 3.11, 3.12        |
 +------------------------+-----------------------------------+
-| 4.1, 4.2               | 3.8, 3.9, 3.10, 3.11              |
+| 5.0                    | 3.10, 3.11, 3.12                  |
 +------------------------+-----------------------------------+
 
 
 
 Install
 =======
```

### Comparing `django-dirtyfields-1.9.2/README.rst` & `django-dirtyfields-1.9.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 
 This package is compatible and tested with the following Python & Django versions:
 
 
 +------------------------+-----------------------------------+
 | Django                 | Python                            |
 +========================+===================================+
-| 2.0, 2.1               | 3.7                               |
+| 2.2, 3.0, 3.1          | 3.8, 3.9                          |
 +------------------------+-----------------------------------+
-| 2.2, 3.0, 3.1          | 3.7, 3.8, 3.9                     |
+| 3.2, 4.0               | 3.8, 3.9, 3.10                    |
 +------------------------+-----------------------------------+
-| 3.2                    | 3.7, 3.8, 3.9, 3.10               |
+| 4.1                    | 3.8, 3.9, 3.10, 3.11              |
 +------------------------+-----------------------------------+
-| 4.0                    | 3.8, 3.9, 3.10                    |
+| 4.2                    | 3.8, 3.9, 3.10, 3.11, 3.12        |
 +------------------------+-----------------------------------+
-| 4.1, 4.2               | 3.8, 3.9, 3.10, 3.11              |
+| 5.0                    | 3.10, 3.11, 3.12                  |
 +------------------------+-----------------------------------+
 
 
 
 Install
 =======
```

### Comparing `django-dirtyfields-1.9.2/setup.cfg` & `django-dirtyfields-1.9.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -13,43 +13,42 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Framework :: Django
-	Framework :: Django :: 2.0
-	Framework :: Django :: 2.1
 	Framework :: Django :: 2.2
 	Framework :: Django :: 3.0
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
+	Framework :: Django :: 5.0
 license = BSD
 license_files = LICENSE
 description = Tracking dirty fields on a Django model instance.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 
 [options]
 packages = find:
 package_dir = 
 	=src
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
-	Django >= 2.0
+	Django >= 2.2
 
 [options.packages.find]
 where = src
 
 [flake8]
 ignore = E133,W503
 max-line-length = 120
```

### Comparing `django-dirtyfields-1.9.2/src/dirtyfields/compare.py` & `django-dirtyfields-1.9.3/src/dirtyfields/compare.py`

 * *Files identical despite different names*

### Comparing `django-dirtyfields-1.9.2/src/dirtyfields/dirtyfields.py` & `django-dirtyfields-1.9.3/src/dirtyfields/dirtyfields.py`

 * *Files identical despite different names*

### Comparing `django-dirtyfields-1.9.2/src/django_dirtyfields.egg-info/PKG-INFO` & `django-dirtyfields-1.9.3/src/django_dirtyfields.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dirtyfields
-Version: 1.9.2
+Version: 1.9.3
 Summary: Tracking dirty fields on a Django model instance.
 Home-page: https://github.com/romgar/django-dirtyfields
 Author: Romain Garrigues
 Maintainer: Lincoln Puzey
 License: BSD
 Project-URL: Documentation, https://django-dirtyfields.readthedocs.io/
 Project-URL: Changelog, https://github.com/romgar/django-dirtyfields/blob/develop/ChangeLog.rst
@@ -13,30 +13,29 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
-Requires-Python: >=3.7
+Classifier: Framework :: Django :: 5.0
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ===================
 Django Dirty Fields
 ===================
 
@@ -61,23 +60,23 @@
 
 This package is compatible and tested with the following Python & Django versions:
 
 
 +------------------------+-----------------------------------+
 | Django                 | Python                            |
 +========================+===================================+
-| 2.0, 2.1               | 3.7                               |
+| 2.2, 3.0, 3.1          | 3.8, 3.9                          |
 +------------------------+-----------------------------------+
-| 2.2, 3.0, 3.1          | 3.7, 3.8, 3.9                     |
+| 3.2, 4.0               | 3.8, 3.9, 3.10                    |
 +------------------------+-----------------------------------+
-| 3.2                    | 3.7, 3.8, 3.9, 3.10               |
+| 4.1                    | 3.8, 3.9, 3.10, 3.11              |
 +------------------------+-----------------------------------+
-| 4.0                    | 3.8, 3.9, 3.10                    |
+| 4.2                    | 3.8, 3.9, 3.10, 3.11, 3.12        |
 +------------------------+-----------------------------------+
-| 4.1, 4.2               | 3.8, 3.9, 3.10, 3.11              |
+| 5.0                    | 3.10, 3.11, 3.12                  |
 +------------------------+-----------------------------------+
 
 
 
 Install
 =======
```

