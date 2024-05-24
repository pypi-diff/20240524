# Comparing `tmp/jaanca-0.1.2rc2.tar.gz` & `tmp/jaanca-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca-0.1.2rc2.tar", last modified: Thu May 23 14:19:11 2024, max compression
+gzip compressed data, was "jaanca-0.1.3.tar", last modified: Fri May 24 20:14:06 2024, max compression
```

## Comparing `jaanca-0.1.2rc2.tar` & `jaanca-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:19:11.073271 jaanca-0.1.2rc2/
--rw-rw-rw-   0        0        0     1092 2024-05-22 20:03:18.000000 jaanca-0.1.2rc2/LICENSE.txt
--rw-rw-rw-   0        0        0     1957 2024-05-23 14:19:11.072273 jaanca-0.1.2rc2/PKG-INFO
--rw-rw-rw-   0        0        0      767 2024-05-23 14:17:17.000000 jaanca-0.1.2rc2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 14:19:11.057272 jaanca-0.1.2rc2/jaanca/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca-0.1.2rc2/jaanca/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:19:11.066272 jaanca-0.1.2rc2/jaanca/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.2rc2/jaanca/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:19:11.068271 jaanca-0.1.2rc2/jaanca/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.2rc2/jaanca/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca-0.1.2rc2/jaanca/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:19:11.071272 jaanca-0.1.2rc2/jaanca.egg-info/
--rw-rw-rw-   0        0        0     1957 2024-05-23 14:19:11.000000 jaanca-0.1.2rc2/jaanca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-23 14:19:11.000000 jaanca-0.1.2rc2/jaanca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:19:11.000000 jaanca-0.1.2rc2/jaanca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-23 14:19:11.000000 jaanca-0.1.2rc2/jaanca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 14:19:11.074274 jaanca-0.1.2rc2/setup.cfg
--rw-rw-rw-   0        0        0     1523 2024-05-23 14:18:55.000000 jaanca-0.1.2rc2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:14:05.996433 jaanca-0.1.3/
+-rw-rw-rw-   0        0        0     1092 2024-05-24 15:55:34.000000 jaanca-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     4013 2024-05-24 20:14:05.996433 jaanca-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2828 2024-05-24 20:13:55.000000 jaanca-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 20:14:05.978433 jaanca-0.1.3/jaanca/
+-rw-rw-rw-   0        0        0       70 2024-05-24 15:55:34.000000 jaanca-0.1.3/jaanca/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:14:05.988431 jaanca-0.1.3/jaanca/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca-0.1.3/jaanca/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:14:05.991431 jaanca-0.1.3/jaanca/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-05-24 15:55:34.000000 jaanca-0.1.3/jaanca/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1537 2024-05-24 15:55:34.000000 jaanca-0.1.3/jaanca/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-24 20:14:05.994433 jaanca-0.1.3/jaanca.egg-info/
+-rw-rw-rw-   0        0        0     4013 2024-05-24 20:14:05.000000 jaanca-0.1.3/jaanca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-24 20:14:05.000000 jaanca-0.1.3/jaanca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 20:14:05.000000 jaanca-0.1.3/jaanca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-24 20:14:05.000000 jaanca-0.1.3/jaanca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 20:14:05.997430 jaanca-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1520 2024-05-24 20:12:43.000000 jaanca-0.1.3/setup.py
```

### Comparing `jaanca-0.1.2rc2/LICENSE.txt` & `jaanca-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca-0.1.2rc2/jaanca/utils/helpers/chronometer.py` & `jaanca-0.1.3/jaanca/utils/helpers/chronometer.py`

 * *Files identical despite different names*

### Comparing `jaanca-0.1.2rc2/setup.py` & `jaanca-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca"
-VERSION = "0.1.2rc2"
+VERSION = "0.1.3"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME}.',
```

