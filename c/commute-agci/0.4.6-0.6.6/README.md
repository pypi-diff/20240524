# Comparing `tmp/commute_agci-0.4.6.tar.gz` & `tmp/commute_agci-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commute_agci-0.4.6.tar", last modified: Thu May 23 05:03:18 2024, max compression
+gzip compressed data, was "commute_agci-0.6.6.tar", last modified: Thu May 23 07:32:05 2024, max compression
```

## Comparing `commute_agci-0.4.6.tar` & `commute_agci-0.6.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 05:03:18.873598 commute_agci-0.4.6/
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     5454 2024-05-23 05:03:18.873401 commute_agci-0.4.6/PKG-INFO
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     4758 2024-05-23 04:09:34.000000 commute_agci-0.4.6/README.md
-drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 05:03:18.872317 commute_agci-0.4.6/commute_agci/
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       69 2024-05-23 04:15:20.000000 commute_agci-0.4.6/commute_agci/__init__.py
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     1458 2024-05-23 04:02:05.000000 commute_agci-0.4.6/commute_agci/commute_agci.py
-drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 05:03:18.873127 commute_agci-0.4.6/commute_agci.egg-info/
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     5454 2024-05-23 05:03:18.000000 commute_agci-0.4.6/commute_agci.egg-info/PKG-INFO
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)      251 2024-05-23 05:03:18.000000 commute_agci-0.4.6/commute_agci.egg-info/SOURCES.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)        1 2024-05-23 05:03:18.000000 commute_agci-0.4.6/commute_agci.egg-info/dependency_links.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       30 2024-05-23 05:03:18.000000 commute_agci-0.4.6/commute_agci.egg-info/requires.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       13 2024-05-23 05:03:18.000000 commute_agci-0.4.6/commute_agci.egg-info/top_level.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       38 2024-05-23 05:03:18.873633 commute_agci-0.4.6/setup.cfg
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     1625 2024-05-23 05:02:56.000000 commute_agci-0.4.6/setup.py
+drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 07:32:05.465846 commute_agci-0.6.6/
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     5454 2024-05-23 07:32:05.465649 commute_agci-0.6.6/PKG-INFO
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     4758 2024-05-23 04:09:34.000000 commute_agci-0.6.6/README.md
+drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 07:32:05.464537 commute_agci-0.6.6/commute_agci/
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       69 2024-05-23 04:15:20.000000 commute_agci-0.6.6/commute_agci/__init__.py
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     1458 2024-05-23 04:02:05.000000 commute_agci-0.6.6/commute_agci/commute_agci.py
+drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-23 07:32:05.465381 commute_agci-0.6.6/commute_agci.egg-info/
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     5454 2024-05-23 07:32:05.000000 commute_agci-0.6.6/commute_agci.egg-info/PKG-INFO
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)      251 2024-05-23 07:32:05.000000 commute_agci-0.6.6/commute_agci.egg-info/SOURCES.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)        1 2024-05-23 07:32:05.000000 commute_agci-0.6.6/commute_agci.egg-info/dependency_links.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       30 2024-05-23 07:32:05.000000 commute_agci-0.6.6/commute_agci.egg-info/requires.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       13 2024-05-23 07:32:05.000000 commute_agci-0.6.6/commute_agci.egg-info/top_level.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       38 2024-05-23 07:32:05.465882 commute_agci-0.6.6/setup.cfg
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     1625 2024-05-23 07:31:52.000000 commute_agci-0.6.6/setup.py
```

### Comparing `commute_agci-0.4.6/PKG-INFO` & `commute_agci-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commute_agci
-Version: 0.4.6
+Version: 0.6.6
 Summary: commute_agci is a Python package for analyzing commute data.
 Home-page: https://github.com/Ryomo0797/AudioAlchemist.git
 Download-URL: https://github.com/Ryomo0797/AudioAlchemist.git
 Author: Udai kishimoto
 Author-email: s2222012@stu.musashino-u.ac.jp
 Maintainer: Udai kishimoto
 Maintainer-email: s2222012@stu.musashino-u.ac.jp
```

### Comparing `commute_agci-0.4.6/README.md` & `commute_agci-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `commute_agci-0.4.6/commute_agci/commute_agci.py` & `commute_agci-0.6.6/commute_agci/commute_agci.py`

 * *Files identical despite different names*

### Comparing `commute_agci-0.4.6/commute_agci.egg-info/PKG-INFO` & `commute_agci-0.6.6/commute_agci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commute_agci
-Version: 0.4.6
+Version: 0.6.6
 Summary: commute_agci is a Python package for analyzing commute data.
 Home-page: https://github.com/Ryomo0797/AudioAlchemist.git
 Download-URL: https://github.com/Ryomo0797/AudioAlchemist.git
 Author: Udai kishimoto
 Author-email: s2222012@stu.musashino-u.ac.jp
 Maintainer: Udai kishimoto
 Maintainer-email: s2222012@stu.musashino-u.ac.jp
```

### Comparing `commute_agci-0.4.6/setup.py` & `commute_agci-0.6.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 DESCRIPTION = 'commute_agci is a Python package for analyzing commute data.'
 NAME = 'commute_agci'
 AUTHOR = 'Udai kishimoto'
 AUTHOR_EMAIL = 's2222012@stu.musashino-u.ac.jp'
 URL = 'https://github.com/Ryomo0797/AudioAlchemist.git'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '0.4.6'
-PYTHON_REQUIRES = '>=3.6'
+VERSION = '0.6.6'
+PYTHON_REQUIRES = '>=3.8'
 INSTALL_REQUIRES = [
     'numpy',
     'pandas',
     'matplotlib',
     'scipy'
 ]
 PACKAGES = [
```

