# Comparing `tmp/jfk_django_core-0.0.3.tar.gz` & `tmp/jfk_django_core-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jfk_django_core-0.0.3.tar", last modified: Thu May  9 10:44:09 2024, max compression
+gzip compressed data, was "jfk_django_core-0.0.4.tar", last modified: Fri May 24 12:22:20 2024, max compression
```

## Comparing `jfk_django_core-0.0.3.tar` & `jfk_django_core-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.870851 jfk_django_core-0.0.3/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.866851 jfk_django_core-0.0.3/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      496 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/.vscode/launch.json
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      790 2024-05-09 10:44:09.869851 jfk_django_core-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.867851 jfk_django_core-0.0.3/jfk_django_core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.868851 jfk_django_core-0.0.3/jfk_django_core/admin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/admin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.868851 jfk_django_core-0.0.3/jfk_django_core/apis/
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/apis/jfk_authentication.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.869851 jfk_django_core-0.0.3/jfk_django_core/migrations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.869851 jfk_django_core-0.0.3/jfk_django_core/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7188 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/jfk_django_core/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 10:44:09.869851 jfk_django_core-0.0.3/jfk_django_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)      790 2024-05-09 10:44:09.000000 jfk_django_core-0.0.3/jfk_django_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      569 2024-05-09 10:44:09.000000 jfk_django_core-0.0.3/jfk_django_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 10:44:09.000000 jfk_django_core-0.0.3/jfk_django_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      337 2024-05-09 10:44:09.000000 jfk_django_core-0.0.3/jfk_django_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-09 10:44:09.000000 jfk_django_core-0.0.3/jfk_django_core.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 10:44:09.870851 jfk_django_core-0.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-09 10:44:02.000000 jfk_django_core-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.212600 jfk_django_core-0.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.208600 jfk_django_core-0.0.4/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/.vscode/launch.json
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      790 2024-05-24 12:22:20.212600 jfk_django_core-0.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.209600 jfk_django_core-0.0.4/jfk_django_core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.210600 jfk_django_core-0.0.4/jfk_django_core/admin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/admin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.211600 jfk_django_core-0.0.4/jfk_django_core/apis/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/apis/jfk_authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.211600 jfk_django_core-0.0.4/jfk_django_core/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.211600 jfk_django_core-0.0.4/jfk_django_core/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7168 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/viewsets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.211600 jfk_django_core-0.0.4/jfk_django_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      790 2024-05-24 12:22:20.000000 jfk_django_core-0.0.4/jfk_django_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      628 2024-05-24 12:22:20.000000 jfk_django_core-0.0.4/jfk_django_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 12:22:20.000000 jfk_django_core-0.0.4/jfk_django_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      337 2024-05-24 12:22:20.000000 jfk_django_core-0.0.4/jfk_django_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-24 12:22:20.000000 jfk_django_core-0.0.4/jfk_django_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 12:22:20.212600 jfk_django_core-0.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/setup.py
```

### Comparing `jfk_django_core-0.0.3/LICENSE` & `jfk_django_core-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jfk_django_core-0.0.3/PKG-INFO` & `jfk_django_core-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jfk-django-core
-Version: 0.0.3
+Version: 0.0.4
 Summary: JFK Django Core
 Author: JFK344
 License: All-Rights-Reserved
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=5.0.0
```

### Comparing `jfk_django_core-0.0.3/jfk_django_core/settings.py` & `jfk_django_core-0.0.4/jfk_django_core/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     },
 }
 
 # Rest Framework
 REST_FRAMEWORK = {
     'DEFAULT_AUTHENTICATION_CLASSES': (
         'rest_framework.authentication.SessionAuthentication',
-        'rest_framework.authentication.BasicAuthentication',
+        'knox.auth.TokenAuthentication',
     ),
     'DEFAULT_PERMISSION_CLASSES': (
         'rest_framework.permissions.IsAuthenticated',
     ),
     'DEFAULT_PAGINATION_CLASS': 'rest_framework.pagination.LimitOffsetPagination',
     'PAGE_SIZE': 100,
     'DEFAULT_SCHEMA_CLASS': 'drf_spectacular.openapi.AutoSchema',
```

### Comparing `jfk_django_core-0.0.3/jfk_django_core.egg-info/PKG-INFO` & `jfk_django_core-0.0.4/jfk_django_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jfk-django-core
-Version: 0.0.3
+Version: 0.0.4
 Summary: JFK Django Core
 Author: JFK344
 License: All-Rights-Reserved
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=5.0.0
```

### Comparing `jfk_django_core-0.0.3/jfk_django_core.egg-info/SOURCES.txt` & `jfk_django_core-0.0.4/jfk_django_core.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 .vscode/launch.json
 jfk_django_core/__init__.py
 jfk_django_core/apps.py
+jfk_django_core/serializers.py
 jfk_django_core/settings.py
 jfk_django_core/urls.py
+jfk_django_core/viewsets.py
 jfk_django_core.egg-info/PKG-INFO
 jfk_django_core.egg-info/SOURCES.txt
 jfk_django_core.egg-info/dependency_links.txt
 jfk_django_core.egg-info/requires.txt
 jfk_django_core.egg-info/top_level.txt
 jfk_django_core/admin/__init__.py
 jfk_django_core/apis/__init__.py
```

### Comparing `jfk_django_core-0.0.3/pyproject.toml` & `jfk_django_core-0.0.4/pyproject.toml`

 * *Files identical despite different names*

