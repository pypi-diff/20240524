# Comparing `tmp/scrathon_payments-0.2.1.tar.gz` & `tmp/scrathon_payments-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrathon_payments-0.2.1.tar", last modified: Fri May 24 07:19:15 2024, max compression
+gzip compressed data, was "scrathon_payments-0.2.2.tar", last modified: Fri May 24 07:59:51 2024, max compression
```

## Comparing `scrathon_payments-0.2.1.tar` & `scrathon_payments-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:15.259892 scrathon_payments-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-24 07:19:11.000000 scrathon_payments-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-24 07:19:15.259892 scrathon_payments-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-24 07:19:11.000000 scrathon_payments-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:15.259892 scrathon_payments-0.2.1/ScrathonPayments/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-24 07:19:11.000000 scrathon_payments-0.2.1/ScrathonPayments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:19:15.259892 scrathon_payments-0.2.1/scrathon_payments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-24 07:19:15.000000 scrathon_payments-0.2.1/scrathon_payments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-24 07:19:15.000000 scrathon_payments-0.2.1/scrathon_payments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:19:15.000000 scrathon_payments-0.2.1/scrathon_payments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 07:19:15.000000 scrathon_payments-0.2.1/scrathon_payments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 07:19:15.000000 scrathon_payments-0.2.1/scrathon_payments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 07:19:15.259892 scrathon_payments-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 07:19:11.000000 scrathon_payments-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:59:51.599595 scrathon_payments-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-24 07:59:42.000000 scrathon_payments-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-24 07:59:51.599595 scrathon_payments-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-24 07:59:42.000000 scrathon_payments-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:59:51.599595 scrathon_payments-0.2.2/ScrathonPayments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-24 07:59:42.000000 scrathon_payments-0.2.2/ScrathonPayments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 07:59:51.599595 scrathon_payments-0.2.2/scrathon_payments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-24 07:59:51.000000 scrathon_payments-0.2.2/scrathon_payments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-24 07:59:51.000000 scrathon_payments-0.2.2/scrathon_payments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 07:59:51.000000 scrathon_payments-0.2.2/scrathon_payments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 07:59:51.000000 scrathon_payments-0.2.2/scrathon_payments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 07:59:51.000000 scrathon_payments-0.2.2/scrathon_payments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 07:59:51.599595 scrathon_payments-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 07:59:42.000000 scrathon_payments-0.2.2/setup.py
```

### Comparing `scrathon_payments-0.2.1/LICENSE` & `scrathon_payments-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.2.1/ScrathonPayments/__init__.py` & `scrathon_payments-0.2.2/ScrathonPayments/__init__.py`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.2.1/setup.py` & `scrathon_payments-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='scrathon-payments',
-    version='0.2.1',
+    version='0.2.2',
     author='Ryan_shamu',
     author_email='Ryanshamu418@gmail.com',
     description='API Wrapper for ScrathonPayments',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Ryan-shamu-YT/ScrathonPayments',
     packages=find_packages(exclude=[]),
```

