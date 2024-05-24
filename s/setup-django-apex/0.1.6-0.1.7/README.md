# Comparing `tmp/setup_django_apex-0.1.6.tar.gz` & `tmp/setup_django_apex-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup_django_apex-0.1.6.tar", last modified: Wed May 22 06:27:20 2024, max compression
+gzip compressed data, was "setup_django_apex-0.1.7.tar", last modified: Fri May 24 12:30:11 2024, max compression
```

## Comparing `setup_django_apex-0.1.6.tar` & `setup_django_apex-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 06:27:20.786666 setup_django_apex-0.1.6/
--rw-rw-rw-   0        0        0     1174 2024-05-22 04:46:04.000000 setup_django_apex-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      857 2024-05-22 06:27:20.784670 setup_django_apex-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-22 04:34:11.000000 setup_django_apex-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 06:27:20.788017 setup_django_apex-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1117 2024-05-22 06:25:20.000000 setup_django_apex-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 06:27:20.760681 setup_django_apex-0.1.6/setup_django_apex/
--rw-rw-rw-   0        0        0        0 2024-05-22 04:26:15.000000 setup_django_apex-0.1.6/setup_django_apex/__init__.py
--rw-rw-rw-   0        0        0      378 2024-05-22 06:24:21.000000 setup_django_apex-0.1.6/setup_django_apex/installer.py
--rw-rw-rw-   0        0        0      329 2024-05-22 06:25:29.000000 setup_django_apex-0.1.6/setup_django_apex/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 06:27:20.781558 setup_django_apex-0.1.6/setup_django_apex.egg-info/
--rw-rw-rw-   0        0        0      857 2024-05-22 06:27:20.000000 setup_django_apex-0.1.6/setup_django_apex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-22 06:27:20.000000 setup_django_apex-0.1.6/setup_django_apex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 06:27:20.000000 setup_django_apex-0.1.6/setup_django_apex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-22 06:27:20.000000 setup_django_apex-0.1.6/setup_django_apex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-22 06:27:20.000000 setup_django_apex-0.1.6/setup_django_apex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 06:27:20.778187 setup_django_apex-0.1.6/tests/
--rw-rw-rw-   0        0        0        0 2024-05-22 03:09:42.000000 setup_django_apex-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0     2111 2024-05-22 04:43:14.000000 setup_django_apex-0.1.6/tests/mytest.py
--rw-rw-rw-   0        0        0     1195 2024-05-22 04:34:28.000000 setup_django_apex-0.1.6/tests/test_installer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 12:30:11.255275 setup_django_apex-0.1.7/
+-rw-rw-rw-   0        0        0     1174 2024-05-22 04:46:04.000000 setup_django_apex-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      765 2024-05-24 12:30:11.251251 setup_django_apex-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-22 04:34:11.000000 setup_django_apex-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 12:30:11.255275 setup_django_apex-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1254 2024-05-24 12:28:56.000000 setup_django_apex-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 12:30:11.200116 setup_django_apex-0.1.7/setup_django_apex/
+-rw-rw-rw-   0        0        0        0 2024-05-22 04:26:15.000000 setup_django_apex-0.1.7/setup_django_apex/__init__.py
+-rw-rw-rw-   0        0        0      321 2024-05-24 12:19:03.000000 setup_django_apex-0.1.7/setup_django_apex/installer.py
+-rw-rw-rw-   0        0        0      357 2024-05-24 12:18:51.000000 setup_django_apex-0.1.7/setup_django_apex/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 12:30:11.247516 setup_django_apex-0.1.7/setup_django_apex.egg-info/
+-rw-rw-rw-   0        0        0      765 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 12:30:11.241874 setup_django_apex-0.1.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-22 03:09:42.000000 setup_django_apex-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     2111 2024-05-22 04:43:14.000000 setup_django_apex-0.1.7/tests/mytest.py
+-rw-rw-rw-   0        0        0     1195 2024-05-22 04:34:28.000000 setup_django_apex-0.1.7/tests/test_installer.py
```

### Comparing `setup_django_apex-0.1.6/LICENSE` & `setup_django_apex-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `setup_django_apex-0.1.6/PKG-INFO` & `setup_django_apex-0.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: setup_django_apex
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library to set up Django projects with multiple apps
 Home-page: https://github.com/Anirudha1821/setup_django_apex
 Author: Anirudha Udgirkar
 Author-email: anirudhaudgirkar.work.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=3.0
-Requires-Dist: django>=3.0
-Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
 
 # setup_django_apex
 
 setup_django_apex is a simple library to set up Django projects with multiple apps interactively.
 
 ## Installation
```

### Comparing `setup_django_apex-0.1.6/setup_django_apex.egg-info/PKG-INFO` & `setup_django_apex-0.1.7/setup_django_apex.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: setup_django_apex
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library to set up Django projects with multiple apps
 Home-page: https://github.com/Anirudha1821/setup_django_apex
 Author: Anirudha Udgirkar
 Author-email: anirudhaudgirkar.work.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=3.0
-Requires-Dist: django>=3.0
-Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
 
 # setup_django_apex
 
 setup_django_apex is a simple library to set up Django projects with multiple apps interactively.
 
 ## Installation
```

### Comparing `setup_django_apex-0.1.6/tests/mytest.py` & `setup_django_apex-0.1.7/tests/mytest.py`

 * *Files identical despite different names*

### Comparing `setup_django_apex-0.1.6/tests/test_installer.py` & `setup_django_apex-0.1.7/tests/test_installer.py`

 * *Files identical despite different names*

