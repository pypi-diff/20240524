# Comparing `tmp/commute_agci-0.6.1.tar.gz` & `tmp/commute_agci-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commute_agci-0.6.1.tar", last modified: Fri May 24 04:42:11 2024, max compression
+gzip compressed data, was "commute_agci-0.6.2.tar", last modified: Fri May 24 05:21:05 2024, max compression
```

## Comparing `commute_agci-0.6.1.tar` & `commute_agci-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-24 04:42:11.998332 commute_agci-0.6.1/
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     5470 2024-05-24 04:42:11.998133 commute_agci-0.6.1/PKG-INFO
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     4758 2024-05-23 04:09:34.000000 commute_agci-0.6.1/README.md
-drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-24 04:42:11.996878 commute_agci-0.6.1/commute_agci/
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       69 2024-05-23 04:15:20.000000 commute_agci-0.6.1/commute_agci/__init__.py
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     7205 2024-05-24 04:06:25.000000 commute_agci-0.6.1/commute_agci/commute_agci.py
-drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-24 04:42:11.997817 commute_agci-0.6.1/commute_agci.egg-info/
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     5470 2024-05-24 04:42:11.000000 commute_agci-0.6.1/commute_agci.egg-info/PKG-INFO
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)      251 2024-05-24 04:42:11.000000 commute_agci-0.6.1/commute_agci.egg-info/SOURCES.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)        1 2024-05-24 04:42:11.000000 commute_agci-0.6.1/commute_agci.egg-info/dependency_links.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       30 2024-05-24 04:42:11.000000 commute_agci-0.6.1/commute_agci.egg-info/requires.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       13 2024-05-24 04:42:11.000000 commute_agci-0.6.1/commute_agci.egg-info/top_level.txt
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       38 2024-05-24 04:42:11.998367 commute_agci-0.6.1/setup.cfg
--rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     1633 2024-05-24 04:42:04.000000 commute_agci-0.6.1/setup.py
+drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-24 05:21:05.041558 commute_agci-0.6.2/
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     3292 2024-05-24 05:21:05.041356 commute_agci-0.6.2/PKG-INFO
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     2581 2024-05-24 05:20:30.000000 commute_agci-0.6.2/README.md
+drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-24 05:21:05.040166 commute_agci-0.6.2/commute_agci/
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       69 2024-05-23 04:15:20.000000 commute_agci-0.6.2/commute_agci/__init__.py
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     7205 2024-05-24 04:06:25.000000 commute_agci-0.6.2/commute_agci/commute_agci.py
+drwxr-xr-x   0 kishimotosakaiyasushi   (501) staff       (20)        0 2024-05-24 05:21:05.041080 commute_agci-0.6.2/commute_agci.egg-info/
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     3292 2024-05-24 05:21:05.000000 commute_agci-0.6.2/commute_agci.egg-info/PKG-INFO
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)      251 2024-05-24 05:21:05.000000 commute_agci-0.6.2/commute_agci.egg-info/SOURCES.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)        1 2024-05-24 05:21:05.000000 commute_agci-0.6.2/commute_agci.egg-info/dependency_links.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       30 2024-05-24 05:21:05.000000 commute_agci-0.6.2/commute_agci.egg-info/requires.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       13 2024-05-24 05:21:05.000000 commute_agci-0.6.2/commute_agci.egg-info/top_level.txt
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)       38 2024-05-24 05:21:05.041596 commute_agci-0.6.2/setup.cfg
+-rw-r--r--   0 kishimotosakaiyasushi   (501) staff       (20)     1633 2024-05-24 05:20:57.000000 commute_agci-0.6.2/setup.py
```

### Comparing `commute_agci-0.6.1/commute_agci/commute_agci.py` & `commute_agci-0.6.2/commute_agci/commute_agci.py`

 * *Files identical despite different names*

### Comparing `commute_agci-0.6.1/setup.py` & `commute_agci-0.6.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 DESCRIPTION = 'commute_agci is a Python package for analyzing commute data.'
 NAME = 'commute_agci'
 AUTHOR = 'Udai kishimoto'
 AUTHOR_EMAIL = 's2222012@stu.musashino-u.ac.jp'
 URL = 'https://github.com/2222012kishimoto/dstokuron/tree/main'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '0.6.1'
+VERSION = '0.6.2'
 PYTHON_REQUIRES = '>=3.8'
 INSTALL_REQUIRES = [
     'numpy',
     'pandas',
     'matplotlib',
     'scipy'
 ]
```

