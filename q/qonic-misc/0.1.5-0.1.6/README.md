# Comparing `tmp/qonic_misc-0.1.5.tar.gz` & `tmp/qonic_misc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qonic_misc-0.1.5.tar", last modified: Fri Sep 30 16:08:45 2022, max compression
+gzip compressed data, was "qonic_misc-0.1.6.tar", last modified: Fri May 24 20:02:47 2024, max compression
```

## Comparing `qonic_misc-0.1.5.tar` & `qonic_misc-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 16:08:45.092113 qonic_misc-0.1.5/
--rw-r--r--   0 root         (0) root         (0)     5750 2022-09-30 16:08:45.092113 qonic_misc-0.1.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5286 2022-09-30 03:49:34.000000 qonic_misc-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 16:08:45.092113 qonic_misc-0.1.5/qonic_misc/
--rw-rw-r--   0 root         (0) root         (0)     2923 2021-04-13 01:55:07.000000 qonic_misc-0.1.5/qonic_misc/OperatorChecker.py
--rw-rw-r--   0 root         (0) root         (0)    10947 2022-08-02 19:10:11.000000 qonic_misc-0.1.5/qonic_misc/RotationConversions.py
--rw-rw-r--   0 root         (0) root         (0)       88 2022-09-30 16:08:30.000000 qonic_misc-0.1.5/qonic_misc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 16:08:45.092113 qonic_misc-0.1.5/qonic_misc.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     5750 2022-09-30 16:08:44.000000 qonic_misc-0.1.5/qonic_misc.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      284 2022-09-30 16:08:44.000000 qonic_misc-0.1.5/qonic_misc.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2022-09-30 16:08:44.000000 qonic_misc-0.1.5/qonic_misc.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       32 2022-09-30 16:08:44.000000 qonic_misc-0.1.5/qonic_misc.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       11 2022-09-30 16:08:44.000000 qonic_misc-0.1.5/qonic_misc.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      131 2022-09-30 16:08:45.092113 qonic_misc-0.1.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      614 2022-09-30 16:08:17.000000 qonic_misc-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:02:47.598011 qonic_misc-0.1.6/
+-rw-r--r--   0 root         (0) root         (0)     5922 2024-05-24 20:02:47.598011 qonic_misc-0.1.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5286 2022-09-30 03:49:34.000000 qonic_misc-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:02:47.598011 qonic_misc-0.1.6/qonic_misc/
+-rw-rw-r--   0 root         (0) root         (0)     2923 2021-04-13 01:55:07.000000 qonic_misc-0.1.6/qonic_misc/OperatorChecker.py
+-rw-rw-r--   0 root         (0) root         (0)    10947 2022-08-02 19:10:11.000000 qonic_misc-0.1.6/qonic_misc/RotationConversions.py
+-rw-rw-r--   0 root         (0) root         (0)       88 2022-09-30 16:08:30.000000 qonic_misc-0.1.6/qonic_misc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:02:47.598011 qonic_misc-0.1.6/qonic_misc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5922 2024-05-24 20:02:47.000000 qonic_misc-0.1.6/qonic_misc.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      284 2024-05-24 20:02:47.000000 qonic_misc-0.1.6/qonic_misc.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-05-24 20:02:47.000000 qonic_misc-0.1.6/qonic_misc.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)      102 2024-05-24 20:02:47.000000 qonic_misc-0.1.6/qonic_misc.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       11 2024-05-24 20:02:47.000000 qonic_misc-0.1.6/qonic_misc.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      131 2024-05-24 20:02:47.598011 qonic_misc-0.1.6/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      697 2024-05-24 20:02:17.000000 qonic_misc-0.1.6/setup.py
```

### Comparing `qonic_misc-0.1.5/PKG-INFO` & `qonic_misc-0.1.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: qonic_misc
-Version: 0.1.5
-Summary: Python library with miscellaneous tools to be used in conjunction with the qonic framework
-Home-page: https://github.com/Qonic-Team/qonic-misc.git
-Author: cogrpar
-Author-email: owen.r.welsh@hotmail.com
-License: Apache License 2.0
-Download-URL: https://github.com/Qonic-Team/qonic-misc/archive/refs/heads/main.zip
-Keywords: qonic,qonic_misc
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 [![Python application](https://github.com/Qonic-Team/qonic-misc/actions/workflows/python-app.yml/badge.svg)](https://github.com/Qonic-Team/qonic-misc/actions/workflows/python-app.yml)
 [![CodeQL](https://github.com/Qonic-Team/qonic-misc/actions/workflows/codeql.yml/badge.svg)](https://github.com/Qonic-Team/qonic-misc/actions/workflows/codeql.yml)
 <sup>[`Snyk Vulnerability Report`](https://snyk.io/test/github/Qonic-Team/qonic-misc?targetFile=source_dir/requirements.txt)</sup>
 
 ## qonic-misc Python Library:
 Python library with miscellaneous tools to be used in conjunction with the qonic framework
 
@@ -108,9 +95,7 @@
         
         **Example:**
         
             >>> oc = qonic_misc.OperatorChecker
             >>> pauli_z = [[1, 0], [0, -1]] # pauli z gate
             >>> print(oc.check_unitary(pauli_z) # check to see if the pauli z gate is unitary
             True
-
-
```

### Comparing `qonic_misc-0.1.5/README.md` & `qonic_misc-0.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: qonic_misc
+Version: 0.1.6
+Summary: Python library with miscellaneous tools to be used in conjunction with the qonic framework
+Home-page: https://github.com/Qonic-Team/qonic-misc.git
+Download-URL: https://github.com/Qonic-Team/qonic-misc/archive/refs/heads/main.zip
+Author: cogrpar
+Author-email: owen.r.welsh@hotmail.com
+License: Apache License 2.0
+Keywords: qonic,qonic_misc
+Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.22.2
+Requires-Dist: tensorflow>=2.12.0rc1
+Requires-Dist: keras>=2.13.1rc0
+Requires-Dist: setuptools>=65.5.1
+Requires-Dist: werkzeug>=3.0.3
+Requires-Dist: wheel>=0.38.0
+
 [![Python application](https://github.com/Qonic-Team/qonic-misc/actions/workflows/python-app.yml/badge.svg)](https://github.com/Qonic-Team/qonic-misc/actions/workflows/python-app.yml)
 [![CodeQL](https://github.com/Qonic-Team/qonic-misc/actions/workflows/codeql.yml/badge.svg)](https://github.com/Qonic-Team/qonic-misc/actions/workflows/codeql.yml)
 <sup>[`Snyk Vulnerability Report`](https://snyk.io/test/github/Qonic-Team/qonic-misc?targetFile=source_dir/requirements.txt)</sup>
 
 ## qonic-misc Python Library:
 Python library with miscellaneous tools to be used in conjunction with the qonic framework
```

### Comparing `qonic_misc-0.1.5/qonic_misc/OperatorChecker.py` & `qonic_misc-0.1.6/qonic_misc/OperatorChecker.py`

 * *Files identical despite different names*

### Comparing `qonic_misc-0.1.5/qonic_misc/RotationConversions.py` & `qonic_misc-0.1.6/qonic_misc/RotationConversions.py`

 * *Files identical despite different names*

### Comparing `qonic_misc-0.1.5/qonic_misc.egg-info/PKG-INFO` & `qonic_misc-0.1.6/qonic_misc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
-Name: qonic-misc
-Version: 0.1.5
+Name: qonic_misc
+Version: 0.1.6
 Summary: Python library with miscellaneous tools to be used in conjunction with the qonic framework
 Home-page: https://github.com/Qonic-Team/qonic-misc.git
+Download-URL: https://github.com/Qonic-Team/qonic-misc/archive/refs/heads/main.zip
 Author: cogrpar
 Author-email: owen.r.welsh@hotmail.com
 License: Apache License 2.0
-Download-URL: https://github.com/Qonic-Team/qonic-misc/archive/refs/heads/main.zip
 Keywords: qonic,qonic_misc
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.22.2
+Requires-Dist: tensorflow>=2.12.0rc1
+Requires-Dist: keras>=2.13.1rc0
+Requires-Dist: setuptools>=65.5.1
+Requires-Dist: werkzeug>=3.0.3
+Requires-Dist: wheel>=0.38.0
 
 [![Python application](https://github.com/Qonic-Team/qonic-misc/actions/workflows/python-app.yml/badge.svg)](https://github.com/Qonic-Team/qonic-misc/actions/workflows/python-app.yml)
 [![CodeQL](https://github.com/Qonic-Team/qonic-misc/actions/workflows/codeql.yml/badge.svg)](https://github.com/Qonic-Team/qonic-misc/actions/workflows/codeql.yml)
 <sup>[`Snyk Vulnerability Report`](https://snyk.io/test/github/Qonic-Team/qonic-misc?targetFile=source_dir/requirements.txt)</sup>
 
 ## qonic-misc Python Library:
 Python library with miscellaneous tools to be used in conjunction with the qonic framework
@@ -108,9 +113,7 @@
         
         **Example:**
         
             >>> oc = qonic_misc.OperatorChecker
             >>> pauli_z = [[1, 0], [0, -1]] # pauli z gate
             >>> print(oc.check_unitary(pauli_z) # check to see if the pauli z gate is unitary
             True
-
-
```

