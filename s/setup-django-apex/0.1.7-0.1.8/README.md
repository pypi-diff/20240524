# Comparing `tmp/setup_django_apex-0.1.7.tar.gz` & `tmp/setup_django_apex-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup_django_apex-0.1.7.tar", last modified: Fri May 24 12:30:11 2024, max compression
+gzip compressed data, was "setup_django_apex-0.1.8.tar", last modified: Fri May 24 13:06:22 2024, max compression
```

## Comparing `setup_django_apex-0.1.7.tar` & `setup_django_apex-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 12:30:11.255275 setup_django_apex-0.1.7/
--rw-rw-rw-   0        0        0     1174 2024-05-22 04:46:04.000000 setup_django_apex-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      765 2024-05-24 12:30:11.251251 setup_django_apex-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-22 04:34:11.000000 setup_django_apex-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 12:30:11.255275 setup_django_apex-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1254 2024-05-24 12:28:56.000000 setup_django_apex-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 12:30:11.200116 setup_django_apex-0.1.7/setup_django_apex/
--rw-rw-rw-   0        0        0        0 2024-05-22 04:26:15.000000 setup_django_apex-0.1.7/setup_django_apex/__init__.py
--rw-rw-rw-   0        0        0      321 2024-05-24 12:19:03.000000 setup_django_apex-0.1.7/setup_django_apex/installer.py
--rw-rw-rw-   0        0        0      357 2024-05-24 12:18:51.000000 setup_django_apex-0.1.7/setup_django_apex/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 12:30:11.247516 setup_django_apex-0.1.7/setup_django_apex.egg-info/
--rw-rw-rw-   0        0        0      765 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-24 12:30:11.000000 setup_django_apex-0.1.7/setup_django_apex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-24 12:30:11.241874 setup_django_apex-0.1.7/tests/
--rw-rw-rw-   0        0        0        0 2024-05-22 03:09:42.000000 setup_django_apex-0.1.7/tests/__init__.py
--rw-rw-rw-   0        0        0     2111 2024-05-22 04:43:14.000000 setup_django_apex-0.1.7/tests/mytest.py
--rw-rw-rw-   0        0        0     1195 2024-05-22 04:34:28.000000 setup_django_apex-0.1.7/tests/test_installer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:06:22.770277 setup_django_apex-0.1.8/
+-rw-rw-rw-   0        0        0     1174 2024-05-22 04:46:04.000000 setup_django_apex-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2134 2024-05-24 13:06:22.766410 setup_django_apex-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-22 04:34:11.000000 setup_django_apex-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 13:06:22.771299 setup_django_apex-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1591 2024-05-24 13:03:31.000000 setup_django_apex-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:06:22.722207 setup_django_apex-0.1.8/setup_django_apex/
+-rw-rw-rw-   0        0        0        0 2024-05-22 04:26:15.000000 setup_django_apex-0.1.8/setup_django_apex/__init__.py
+-rw-rw-rw-   0        0        0     1144 2024-05-24 13:05:58.000000 setup_django_apex-0.1.8/setup_django_apex/installer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 13:06:22.761726 setup_django_apex-0.1.8/setup_django_apex.egg-info/
+-rw-rw-rw-   0        0        0     2134 2024-05-24 13:06:22.000000 setup_django_apex-0.1.8/setup_django_apex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-24 13:06:22.000000 setup_django_apex-0.1.8/setup_django_apex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 13:06:22.000000 setup_django_apex-0.1.8/setup_django_apex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2024-05-24 13:06:22.000000 setup_django_apex-0.1.8/setup_django_apex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-05-24 13:06:22.000000 setup_django_apex-0.1.8/setup_django_apex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-24 13:06:22.000000 setup_django_apex-0.1.8/setup_django_apex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 13:06:22.757098 setup_django_apex-0.1.8/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-22 03:09:42.000000 setup_django_apex-0.1.8/tests/__init__.py
+-rw-rw-rw-   0        0        0     2111 2024-05-22 04:43:14.000000 setup_django_apex-0.1.8/tests/mytest.py
+-rw-rw-rw-   0        0        0     1195 2024-05-22 04:34:28.000000 setup_django_apex-0.1.8/tests/test_installer.py
```

### Comparing `setup_django_apex-0.1.7/LICENSE` & `setup_django_apex-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `setup_django_apex-0.1.7/tests/mytest.py` & `setup_django_apex-0.1.8/tests/mytest.py`

 * *Files identical despite different names*

### Comparing `setup_django_apex-0.1.7/tests/test_installer.py` & `setup_django_apex-0.1.8/tests/test_installer.py`

 * *Files identical despite different names*

