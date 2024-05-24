# Comparing `tmp/scrathon_payments-0.2.3.tar.gz` & `tmp/scrathon_payments-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrathon_payments-0.2.3.tar", last modified: Fri May 24 16:11:09 2024, max compression
+gzip compressed data, was "scrathon_payments-0.2.4.tar", last modified: Fri May 24 16:14:33 2024, max compression
```

## Comparing `scrathon_payments-0.2.3.tar` & `scrathon_payments-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:11:09.131388 scrathon_payments-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-24 16:11:05.000000 scrathon_payments-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-24 16:11:09.131388 scrathon_payments-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-24 16:11:05.000000 scrathon_payments-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:11:09.131388 scrathon_payments-0.2.3/ScrathonPayments/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-24 16:11:05.000000 scrathon_payments-0.2.3/ScrathonPayments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:11:09.131388 scrathon_payments-0.2.3/scrathon_payments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-24 16:11:09.000000 scrathon_payments-0.2.3/scrathon_payments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-24 16:11:09.000000 scrathon_payments-0.2.3/scrathon_payments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:11:09.000000 scrathon_payments-0.2.3/scrathon_payments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 16:11:09.000000 scrathon_payments-0.2.3/scrathon_payments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 16:11:09.000000 scrathon_payments-0.2.3/scrathon_payments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 16:11:09.131388 scrathon_payments-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 16:11:05.000000 scrathon_payments-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:14:33.490076 scrathon_payments-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-24 16:14:29.000000 scrathon_payments-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-24 16:14:33.490076 scrathon_payments-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-24 16:14:29.000000 scrathon_payments-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:14:33.490076 scrathon_payments-0.2.4/ScrathonPayments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-24 16:14:29.000000 scrathon_payments-0.2.4/ScrathonPayments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:14:33.490076 scrathon_payments-0.2.4/scrathon_payments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-24 16:14:33.000000 scrathon_payments-0.2.4/scrathon_payments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-24 16:14:33.000000 scrathon_payments-0.2.4/scrathon_payments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:14:33.000000 scrathon_payments-0.2.4/scrathon_payments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 16:14:33.000000 scrathon_payments-0.2.4/scrathon_payments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 16:14:33.000000 scrathon_payments-0.2.4/scrathon_payments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 16:14:33.490076 scrathon_payments-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 16:14:29.000000 scrathon_payments-0.2.4/setup.py
```

### Comparing `scrathon_payments-0.2.3/LICENSE` & `scrathon_payments-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.2.3/PKG-INFO` & `scrathon_payments-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrathon-payments
-Version: 0.2.3
+Version: 0.2.4
 Summary: API Wrapper for ScrathonPayments
 Home-page: https://github.com/Ryan-shamu-YT/ScrathonPayments
 Author: Ryan_shamu
 Author-email: Ryanshamu418@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scrathon_payments-0.2.3/README.md` & `scrathon_payments-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.2.3/ScrathonPayments/__init__.py` & `scrathon_payments-0.2.4/ScrathonPayments/__init__.py`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.2.3/scrathon_payments.egg-info/PKG-INFO` & `scrathon_payments-0.2.4/scrathon_payments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrathon-payments
-Version: 0.2.3
+Version: 0.2.4
 Summary: API Wrapper for ScrathonPayments
 Home-page: https://github.com/Ryan-shamu-YT/ScrathonPayments
 Author: Ryan_shamu
 Author-email: Ryanshamu418@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scrathon_payments-0.2.3/setup.py` & `scrathon_payments-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='scrathon-payments',
-    version='0.2.3',
+    version='0.2.4',
     author='Ryan_shamu',
     author_email='Ryanshamu418@gmail.com',
     description='API Wrapper for ScrathonPayments',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Ryan-shamu-YT/ScrathonPayments',
     packages=find_packages(exclude=[]),
```

