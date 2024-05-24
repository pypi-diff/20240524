# Comparing `tmp/imio_pyutils-1.0.2.tar.gz` & `tmp/imio.pyutils-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imio_pyutils-1.0.2.tar", last modified: Wed May 15 13:06:55 2024, max compression
+gzip compressed data, was "imio.pyutils-1.0.3.tar", last modified: Fri May 24 08:28:45 2024, max compression
```

## Comparing `imio_pyutils-1.0.2.tar` & `imio.pyutils-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 antoineduchene   (501) staff       (20)        0 2024-05-15 13:06:55.862451 imio_pyutils-1.0.2/
--rw-r--r--   0 antoineduchene   (501) staff       (20)     5546 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/CHANGES.rst
--rw-r--r--   0 antoineduchene   (501) staff       (20)       31 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/MANIFEST.in
--rw-r--r--   0 antoineduchene   (501) staff       (20)     1971 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/Makefile
--rw-r--r--   0 antoineduchene   (501) staff       (20)     7566 2024-05-15 13:06:55.862290 imio_pyutils-1.0.2/PKG-INFO
--rw-r--r--   0 antoineduchene   (501) staff       (20)     1286 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/README.rst
-drwxr-xr-x   0 antoineduchene   (501) staff       (20)        0 2024-05-15 13:06:55.860572 imio_pyutils-1.0.2/imio/
--rw-r--r--   0 antoineduchene   (501) staff       (20)      244 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/__init__.py
-drwxr-xr-x   0 antoineduchene   (501) staff       (20)        0 2024-05-15 13:06:55.861783 imio_pyutils-1.0.2/imio/pyutils/
--rw-r--r--   0 antoineduchene   (501) staff       (20)        0 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/__init__.py
--rw-r--r--   0 antoineduchene   (501) staff       (20)     3508 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/bs.py
--rw-r--r--   0 antoineduchene   (501) staff       (20)     4723 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/postgres.py
--rw-r--r--   0 antoineduchene   (501) staff       (20)    13626 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/system.py
--rw-r--r--   0 antoineduchene   (501) staff       (20)    12087 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/tests.py
--rw-r--r--   0 antoineduchene   (501) staff       (20)    11025 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio/pyutils/utils.py
-drwxr-xr-x   0 antoineduchene   (501) staff       (20)        0 2024-05-15 13:06:55.862077 imio_pyutils-1.0.2/imio.pyutils.egg-info/
--rw-r--r--   0 antoineduchene   (501) staff       (20)     7566 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/PKG-INFO
--rw-r--r--   0 antoineduchene   (501) staff       (20)      464 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 antoineduchene   (501) staff       (20)        1 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 antoineduchene   (501) staff       (20)        5 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/namespace_packages.txt
--rw-r--r--   0 antoineduchene   (501) staff       (20)        1 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/not-zip-safe
--rw-r--r--   0 antoineduchene   (501) staff       (20)       30 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/requires.txt
--rw-r--r--   0 antoineduchene   (501) staff       (20)        5 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/imio.pyutils.egg-info/top_level.txt
--rw-r--r--   0 antoineduchene   (501) staff       (20)       38 2024-05-15 13:06:55.862484 imio_pyutils-1.0.2/setup.cfg
--rw-r--r--   0 antoineduchene   (501) staff       (20)     1480 2024-05-15 13:06:55.000000 imio_pyutils-1.0.2/setup.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 08:28:45.512478 imio.pyutils-1.0.3/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     5630 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/CHANGES.rst
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       31 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/MANIFEST.in
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1971 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/Makefile
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     7575 2024-05-24 08:28:45.512478 imio.pyutils-1.0.3/PKG-INFO
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1286 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/README.rst
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 08:28:45.512478 imio.pyutils-1.0.3/imio/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      244 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio/__init__.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 08:28:45.512478 imio.pyutils-1.0.3/imio/pyutils/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio/pyutils/__init__.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     3508 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio/pyutils/bs.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     4723 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio/pyutils/postgres.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    13626 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio/pyutils/system.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    12087 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio/pyutils/tests.py
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)    11025 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio/pyutils/utils.py
+drwxr-xr-x   0 duchenean  (1000) duchenean  (1000)        0 2024-05-24 08:28:45.512478 imio.pyutils-1.0.3/imio.pyutils.egg-info/
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     7575 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio.pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)      464 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio.pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio.pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        5 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio.pyutils.egg-info/namespace_packages.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        1 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio.pyutils.egg-info/not-zip-safe
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       30 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio.pyutils.egg-info/requires.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)        5 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/imio.pyutils.egg-info/top_level.txt
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)       38 2024-05-24 08:28:45.512478 imio.pyutils-1.0.3/setup.cfg
+-rw-r--r--   0 duchenean  (1000) duchenean  (1000)     1480 2024-05-24 08:28:45.000000 imio.pyutils-1.0.3/setup.py
```

### Comparing `imio_pyutils-1.0.2/CHANGES.rst` & `imio.pyutils-1.0.3/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.0.3 (2024-05-24)
+------------------
+
+- Fix bad release for python2.
+  [aduchene]
+
 1.0.2 (2024-05-15)
 ------------------
 
 - Added a new helper `utils.get_ordinal_clusters` to cluster ordinal numbers based on an offset.
   [aduchene]
 
 1.0.1 (2024-04-08)
```

### Comparing `imio_pyutils-1.0.2/Makefile` & `imio.pyutils-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `imio_pyutils-1.0.2/PKG-INFO` & `imio.pyutils-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: imio.pyutils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Some python useful methods
 Home-page: https://github.com/imio/imio.pyutils/
 Author: IMIO
 Author-email: support@imio.be
 License: GPL
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.pyutils
 Project-URL: Source, https://github.com/imio/imio.pyutils
 Keywords: Python IMIO
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: setuptools
-Requires-Dist: future
-Requires-Dist: six>=1.16.0
 
 .. image:: https://github.com/IMIO/imio.pyutils/actions/workflows/main.yml/badge.svg?branch=master
     :target: https://github.com/IMIO/imio.pyutils/actions/workflows/main.yml
 
 .. image:: https://coveralls.io/repos/github/IMIO/imio.pyutils/badge.svg
     :target: https://coveralls.io/github/IMIO/imio.pyutils
 
@@ -78,14 +75,20 @@
 =====
 
 Can be run with: `bin/python -m unittest discover`
 
 Changelog
 =========
 
+1.0.3 (2024-05-24)
+------------------
+
+- Fix bad release for python2.
+  [aduchene]
+
 1.0.2 (2024-05-15)
 ------------------
 
 - Added a new helper `utils.get_ordinal_clusters` to cluster ordinal numbers based on an offset.
   [aduchene]
 
 1.0.1 (2024-04-08)
```

### Comparing `imio_pyutils-1.0.2/README.rst` & `imio.pyutils-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `imio_pyutils-1.0.2/imio/pyutils/bs.py` & `imio.pyutils-1.0.3/imio/pyutils/bs.py`

 * *Files identical despite different names*

### Comparing `imio_pyutils-1.0.2/imio/pyutils/postgres.py` & `imio.pyutils-1.0.3/imio/pyutils/postgres.py`

 * *Files identical despite different names*

### Comparing `imio_pyutils-1.0.2/imio/pyutils/system.py` & `imio.pyutils-1.0.3/imio/pyutils/system.py`

 * *Files identical despite different names*

### Comparing `imio_pyutils-1.0.2/imio/pyutils/tests.py` & `imio.pyutils-1.0.3/imio/pyutils/tests.py`

 * *Files identical despite different names*

### Comparing `imio_pyutils-1.0.2/imio/pyutils/utils.py` & `imio.pyutils-1.0.3/imio/pyutils/utils.py`

 * *Files identical despite different names*

### Comparing `imio_pyutils-1.0.2/imio.pyutils.egg-info/PKG-INFO` & `imio.pyutils-1.0.3/imio.pyutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: imio.pyutils
-Version: 1.0.2
+Version: 1.0.3
 Summary: Some python useful methods
 Home-page: https://github.com/imio/imio.pyutils/
 Author: IMIO
 Author-email: support@imio.be
 License: GPL
 Project-URL: PyPI, https://pypi.python.org/pypi/imio.pyutils
 Project-URL: Source, https://github.com/imio/imio.pyutils
 Keywords: Python IMIO
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: setuptools
-Requires-Dist: future
-Requires-Dist: six>=1.16.0
 
 .. image:: https://github.com/IMIO/imio.pyutils/actions/workflows/main.yml/badge.svg?branch=master
     :target: https://github.com/IMIO/imio.pyutils/actions/workflows/main.yml
 
 .. image:: https://coveralls.io/repos/github/IMIO/imio.pyutils/badge.svg
     :target: https://coveralls.io/github/IMIO/imio.pyutils
 
@@ -78,14 +75,20 @@
 =====
 
 Can be run with: `bin/python -m unittest discover`
 
 Changelog
 =========
 
+1.0.3 (2024-05-24)
+------------------
+
+- Fix bad release for python2.
+  [aduchene]
+
 1.0.2 (2024-05-15)
 ------------------
 
 - Added a new helper `utils.get_ordinal_clusters` to cluster ordinal numbers based on an offset.
   [aduchene]
 
 1.0.1 (2024-04-08)
```

### Comparing `imio_pyutils-1.0.2/setup.py` & `imio.pyutils-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '1.0.2'
+version = '1.0.3'
 
 setup(name='imio.pyutils',
       version=version,
       description="Some python useful methods",
       long_description=open("README.rst").read() + "\n" + open('CHANGES.rst').read(),
       # Get more strings from
       # http://pypi.python.org/pypi?:action=list_classifiers
```

